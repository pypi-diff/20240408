# Comparing `tmp/dew_gwdata-0.80.tar.gz` & `tmp/dew_gwdata-0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dew_gwdata-0.80.tar", last modified: Wed Feb 28 01:50:59 2024, max compression
+gzip compressed data, was "dew_gwdata-0.81.tar", last modified: Mon Apr  8 04:21:22 2024, max compression
```

## Comparing `dew_gwdata-0.80.tar` & `dew_gwdata-0.81.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.898920 dew_gwdata-0.80/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-02-28 01:50:30.000000 dew_gwdata-0.80/.coveragerc
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.850920 dew_gwdata-0.80/.github/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.854920 dew_gwdata-0.80/.github/workflows/
--rw-rw-rw-   0 root         (0) root         (0)      906 2024-02-28 01:50:30.000000 dew_gwdata-0.80/.github/workflows/python-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1222 2024-02-28 01:50:30.000000 dew_gwdata-0.80/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-02-28 01:50:30.000000 dew_gwdata-0.80/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      150 2024-02-28 01:50:30.000000 dew_gwdata-0.80/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2362 2024-02-28 01:50:59.898920 dew_gwdata-0.80/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1490 2024-02-28 01:50:30.000000 dew_gwdata-0.80/README.md
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-02-28 01:50:30.000000 dew_gwdata-0.80/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.858920 dew_gwdata-0.80/dew_gwdata/
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    54243 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/_aquarius_ts.py
--rw-rw-rw-   0 root         (0) root         (0)     6112 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/_aquarius_wp.py
--rw-rw-rw-   0 root         (0) root         (0)    25093 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/_gtslogs.py
--rw-rw-rw-   0 root         (0) root         (0)     4732 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/_hydstra.py
--rw-rw-rw-   0 root         (0) root         (0)     3181 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/_sagd_api.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/_wde.py
--rw-rw-rw-   0 root         (0) root         (0)     4328 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/charts.py
--rw-rw-rw-   0 root         (0) root         (0)    65260 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/gwdata.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/las_to_alias.csv
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_dosbox.conf
--rw-rw-rw-   0 root         (0) root         (0)     4424 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_dosbox.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.858920 dew_gwdata-0.80/dew_gwdata/logger20_image/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.862920 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/A.BAT
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/BAT.BAT
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/BJT.BAT
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/C.BAT
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/CHT.BAT
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/COM.BAT
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/CONV.BAT
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/DAC.BAT
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/DBF.BAT
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/DR.BAT
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/GK.BAT
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/LAS.BAT
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/LOG.BAT
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/QA.BAT
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/QC.BAT
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/RJM.BAT
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/SD.BAT
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/SDU.BAT
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/UTILS.BAT
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/VF.BAT
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/BAT/W.BAT
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.862920 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.870920 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/AUSIND.CHT
--rw-rw-rw-   0 root         (0) root         (0)      903 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/CAL13.CHT
--rw-rw-rw-   0 root         (0) root         (0)      902 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/CAL14.CHT
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/CAL7.CHT
--rw-rw-rw-   0 root         (0) root         (0)      297 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/CAL8.CHT
--rw-rw-rw-   0 root         (0) root         (0)      729 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB1.CHT
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB1CCL.CHT
--rw-rw-rw-   0 root         (0) root         (0)      481 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB3.CHT
--rw-rw-rw-   0 root         (0) root         (0)      482 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB3CCL.CHT
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB8.CHT
--rw-rw-rw-   0 root         (0) root         (0)      727 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB8CCL.CHT
--rw-rw-rw-   0 root         (0) root         (0)      915 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DF13.CHT
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DF14.CHT
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DN13.CHT
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DN14.CHT
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G11.CHT
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G12.CHT
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G13.CHT
--rw-rw-rw-   0 root         (0) root         (0)      898 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G14.CHT
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G1API.CHT
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G3API.CHT
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G7.CHT
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G8API.CHT
--rw-rw-rw-   0 root         (0) root         (0)      882 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G9.CHT
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND1D.CHT
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND1M.CHT
--rw-rw-rw-   0 root         (0) root         (0)      665 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND2D.CHT
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND2M.CHT
--rw-rw-rw-   0 root         (0) root         (0)      289 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND3.CHT
--rw-rw-rw-   0 root         (0) root         (0)      618 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/N11.CHT
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/N7.CHT
--rw-rw-rw-   0 root         (0) root         (0)      879 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/N9.CHT
--rw-rw-rw-   0 root         (0) root         (0)      318 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/PR.CHT
--rw-rw-rw-   0 root         (0) root         (0)      319 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/PR9.CHT
--rw-rw-rw-   0 root         (0) root         (0)      301 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/PR9P3.CHT
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/SP.CHT
--rw-rw-rw-   0 root         (0) root         (0)      321 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/SP9.CHT
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/LOGGER.BAK
--rw-rw-rw-   0 root         (0) root         (0)      908 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/LOGGER.INI
--rw-rw-rw-   0 root         (0) root         (0)      145 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/LOGGER.PWD
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.870920 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/ODDENDS/
--rw-rw-rw-   0 root         (0) root         (0)    29950 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/ODDENDS/counts.exe
--rw-rw-rw-   0 root         (0) root         (0)    37208 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/ODDENDS/pclog.exe
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.870920 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/LOGGER.INI
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.870920 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/
--rw-rw-rw-   0 root         (0) root         (0)     1579 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/TOOLLIST.REF
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/default.hea
--rw-rw-rw-   0 root         (0) root         (0)     1141 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/gridlist.ref
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/logger.bak
--rw-rw-rw-   0 root         (0) root         (0)    11648 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/logger.fnt
--rw-rw-rw-   0 root         (0) root         (0)      910 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/logger.ini
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/toollist.tmp
--rw-rw-rw-   0 root         (0) root         (0)     1141 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/gridlist.ref
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/logger.dme
--rw-rw-rw-   0 root         (0) root         (0)    11648 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/logger.fnt
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/logger.id
--rw-rw-rw-   0 root         (0) root         (0)   361952 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/logger20.exe
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.874920 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/
--rw-rw-rw-   0 root         (0) root         (0)    17435 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/ADDPATH.EXE
--rw-rw-rw-   0 root         (0) root         (0)    12920 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/CAGE.EXE
--rw-rw-rw-   0 root         (0) root         (0)     4096 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/CO.COM
--rw-rw-rw-   0 root         (0) root         (0)    29950 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/COUNTS.EXE
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/FILEDIV.COM
--rw-rw-rw-   0 root         (0) root         (0)    27088 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/GMOUSE.COM
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/GY.BAT
--rw-rw-rw-   0 root         (0) root         (0)   121248 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/GYCHECK.EXE
--rw-rw-rw-   0 root         (0) root         (0)     1306 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/HISTORY.TXT
--rw-rw-rw-   0 root         (0) root         (0)     8032 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/L20COM.OLD
--rw-rw-rw-   0 root         (0) root         (0)     8064 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/L20COMIO.EXE
--rw-rw-rw-   0 root         (0) root         (0)     8016 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/LCOM.EXE
--rw-rw-rw-   0 root         (0) root         (0)    33850 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/PCLOG.EXE
--rw-rw-rw-   0 root         (0) root         (0)    29378 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/PKUNZIP.EXE
--rw-rw-rw-   0 root         (0) root         (0)    34296 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/PKZIP.EXE
--rw-rw-rw-   0 root         (0) root         (0)    47420 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/Q.EXE
--rw-rw-rw-   0 root         (0) root         (0)     1826 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/SLOWDOS.COM
--rw-rw-rw-   0 root         (0) root         (0)     1034 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/SLOWDOS.TXT
--rw-rw-rw-   0 root         (0) root         (0)     2791 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/SLOWDOS.ZIP
--rw-rw-rw-   0 root         (0) root         (0)    82328 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/SPEEDCOM.EXE
--rw-rw-rw-   0 root         (0) root         (0)    91561 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/SYSINFO.EXE
--rw-rw-rw-   0 root         (0) root         (0)     8467 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/WHEREIS.EXE
--rw-rw-rw-   0 root         (0) root         (0)    17435 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/addpath.exe
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/autoexec.bat
--rw-rw-rw-   0 root         (0) root         (0)      210 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/config.sys
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/instal20.bat
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/l20.bat
--rw-rw-rw-   0 root         (0) root         (0)     8032 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/l20comio.exe
--rw-rw-rw-   0 root         (0) root         (0)     1354 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/logger20_image/readme.txt
--rw-rw-rw-   0 root         (0) root         (0)      936 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/sageodata_database.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/sageodata_datamart.py
--rw-rw-rw-   0 root         (0) root         (0)      950 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/spreadsheets.py
--rw-rw-rw-   0 root         (0) root         (0)    10830 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.874920 dew_gwdata-0.80/dew_gwdata/wde_queries/
--rw-rw-rw-   0 root         (0) root         (0)      289 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/wde_queries/alerts.sql
--rw-rw-rw-   0 root         (0) root         (0)      263 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/wde_queries/logger_installations.sql
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/wde_queries/logger_readings.sql
--rw-rw-rw-   0 root         (0) root         (0)      389 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/wde_queries/maintenance_issues.sql
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.878920 dew_gwdata-0.80/dew_gwdata/webapp/
--rw-rw-rw-   0 root         (0) root         (0)      906 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.878920 dew_gwdata-0.80/dew_gwdata/webapp/handlers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16097 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/handlers/api.py
--rw-rw-rw-   0 root         (0) root         (0)     2928 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/handlers/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/handlers/home.py
--rw-rw-rw-   0 root         (0) root         (0)     7314 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/handlers/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4857 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/handlers/search.py
--rw-rw-rw-   0 root         (0) root         (0)    23864 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/handlers/well.py
--rw-rw-rw-   0 root         (0) root         (0)     7436 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/handlers/wells.py
--rw-rw-rw-   0 root         (0) root         (0)      901 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/log-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1029 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/main.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.878920 dew_gwdata-0.80/dew_gwdata/webapp/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4649 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/models/queries.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.878920 dew_gwdata-0.80/dew_gwdata/webapp/static/
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/static/MarkerCluster.Default.css
--rw-rw-rw-   0 root         (0) root         (0)      872 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/static/MarkerCluster.css
--rw-rw-rw-   0 root         (0) root         (0)     2927 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/static/dygraph.css
--rw-rw-rw-   0 root         (0) root         (0)   476414 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/static/dygraph.js
--rw-rw-rw-   0 root         (0) root         (0)      779 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/static/external-link.svg
--rw-rw-rw-   0 root         (0) root         (0)    71010 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/static/leaflet.markercluster-src.js
--rw-rw-rw-   0 root         (0) root         (0)     1482 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/static/style.css
--rw-rw-rw-   0 root         (0) root         (0)    23424 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/static/w3.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.882920 dew_gwdata-0.80/dew_gwdata/webapp/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2137 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/app_layout.html
--rw-rw-rw-   0 root         (0) root         (0)      342 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/app_layout_schema.html
--rw-rw-rw-   0 root         (0) root         (0)     2317 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/app_layout_well.html
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/app_layout_wells.html
--rw-rw-rw-   0 root         (0) root         (0)     4139 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/app_navbar_wells_dropdown.html
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/app_schema.html
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/app_schema_columns.html
--rw-rw-rw-   0 root         (0) root         (0)     1779 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/app_schema_data.html
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/app_schema_view.html
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/group_summary.html
--rw-rw-rw-   0 root         (0) root         (0)     3398 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/home.html
--rw-rw-rw-   0 root         (0) root         (0)     4160 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/well_combined_water_level.html
--rw-rw-rw-   0 root         (0) root         (0)     2345 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/well_construction.html
--rw-rw-rw-   0 root         (0) root         (0)     2091 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/well_drillhole_document_images.html
--rw-rw-rw-   0 root         (0) root         (0)      771 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/well_drillhole_logs.html
--rw-rw-rw-   0 root         (0) root         (0)     3543 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/well_logger_water_level.html
--rw-rw-rw-   0 root         (0) root         (0)     2315 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/well_manual_water_level.html
--rw-rw-rw-   0 root         (0) root         (0)     1343 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/well_salinity.html
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/well_summary.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/wells_data_available.html
--rw-rw-rw-   0 root         (0) root         (0)     3942 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/wells_map.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/templates/wells_summary.html
--rw-rw-rw-   0 root         (0) root         (0)     3069 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/webapp/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    26235 2024-02-28 01:50:30.000000 dew_gwdata-0.80/dew_gwdata/wilma_reports.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.898920 dew_gwdata-0.80/dew_gwdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2362 2024-02-28 01:50:59.000000 dew_gwdata-0.80/dew_gwdata.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9672 2024-02-28 01:50:59.000000 dew_gwdata-0.80/dew_gwdata.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-28 01:50:59.000000 dew_gwdata-0.80/dew_gwdata.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-02-28 01:50:59.000000 dew_gwdata-0.80/dew_gwdata.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      218 2024-02-28 01:50:59.000000 dew_gwdata-0.80/dew_gwdata.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-02-28 01:50:59.000000 dew_gwdata-0.80/dew_gwdata.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.886920 dew_gwdata-0.80/docs/
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/Makefile
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.886920 dew_gwdata-0.80/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/_static/custom.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.886920 dew_gwdata-0.80/docs/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      354 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/_templates/parent_links.html
--rw-rw-rw-   0 root         (0) root         (0)     3719 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/apidocs.rst
--rw-rw-rw-   0 root         (0) root         (0)     5124 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1738 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/charting.rst
--rw-rw-rw-   0 root         (0) root         (0)     1638 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     4227 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/dew_gwdata.objects.inv
--rw-rw-rw-   0 root         (0) root         (0)     4495 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/drillhole-details.rst
--rw-rw-rw-   0 root         (0) root         (0)    16174 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/elevation.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4491 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/elevation.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.886920 dew_gwdata-0.80/docs/figures/
--rw-rw-rw-   0 root         (0) root         (0)    25191 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/figures/extract_method.png
--rw-rw-rw-   0 root         (0) root         (0)    20070 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/figures/measured_during.png
--rw-rw-rw-   0 root         (0) root         (0)     2990 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/geophysical-logs.rst
--rw-rw-rw-   0 root         (0) root         (0)    63181 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/groups-networks.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     6185 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/gwdata-access.rst
--rw-rw-rw-   0 root         (0) root         (0)     1152 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1314 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)    16065 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/intro.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)   170314 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/tutorial-water-levels.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   173859 2024-02-28 01:50:30.000000 dew_gwdata-0.80/docs/well-summary-data.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      428 2024-02-28 01:50:30.000000 dew_gwdata-0.80/environment.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.898920 dew_gwdata-0.80/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)    18146 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/1 - How to get water levels for a few wells.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    41200 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/2 - Find all wells in a PWA or PWRA.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    49011 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/3 - Chart salinities for a well.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    23716 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/4 - See all the available predefined queries.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      666 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/How to install dew_gwdata.md
--rw-rw-rw-   0 root         (0) root         (0)      715 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1111 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/Untitled.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   190550 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/chemistry stuff.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    11488 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev - PEPS exports.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    46009 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev - aquifer monitored-Copy1.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    15146 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev - aquifer monitored.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    48794 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev - events query.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    23665 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev - hydrostrat logs integrated.ipynb
--rw-rw-rw-   0 root         (0) root         (0)  2202594 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev AQ datasets.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    28709 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev AQ locations.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   117484 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev AQTS field visits.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    56568 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev WL between dates.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     7733 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev issue .ipynb
--rw-rw-rw-   0 root         (0) root         (0)    25467 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev issue 12 - missing ref_elev causes TypeError (MOR252).ipynb
--rw-rw-rw-   0 root         (0) root         (0)   139018 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev modified_log.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    21636 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev water level times.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    56080 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev wells summary.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    56089 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/dev. wilma_cache.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    25378 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/install_fig0.png
--rw-rw-rw-   0 root         (0) root         (0)    14171 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/install_fig1.png
--rw-rw-rw-   0 root         (0) root         (0)    21321 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/install_fig3.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.898920 dew_gwdata-0.80/notebooks/issues/
--rw-rw-rw-   0 root         (0) root         (0)   115850 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/issues/11 - Hydstra QC undefined is being included.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    11549 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/issues/7 - NRM and landscapes.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1692 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/issues/Parsing identifiers from SQL.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    24698 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/issues/Untitled.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    22873 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/nb2_fig1.png
--rw-rw-rw-   0 root         (0) root         (0)    34810 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/nb3_fig1.png
--rw-rw-rw-   0 root         (0) root         (0)    17395 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/permit conditions.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    21380 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/permit numbers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    43995 2024-02-28 01:50:30.000000 dew_gwdata-0.80/notebooks/standard salinity graph.ipynb
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-02-28 01:50:30.000000 dew_gwdata-0.80/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-02-28 01:50:30.000000 dew_gwdata-0.80/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-02-28 01:50:59.898920 dew_gwdata-0.80/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1140 2024-02-28 01:50:30.000000 dew_gwdata-0.80/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-28 01:50:59.898920 dew_gwdata-0.80/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1555 2024-02-28 01:50:30.000000 dew_gwdata-0.80/tests/test_connection.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2024-02-28 01:50:30.000000 dew_gwdata-0.80/tests/test_predefined_queries.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-02-28 01:50:30.000000 dew_gwdata-0.80/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-02-28 01:50:30.000000 dew_gwdata-0.80/tests/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.128111 dew_gwdata-0.81/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-08 04:21:09.000000 dew_gwdata-0.81/.coveragerc
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.084110 dew_gwdata-0.81/.github/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.088110 dew_gwdata-0.81/.github/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)      906 2024-04-08 04:21:09.000000 dew_gwdata-0.81/.github/workflows/python-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2024-04-08 04:21:09.000000 dew_gwdata-0.81/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-08 04:21:09.000000 dew_gwdata-0.81/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      150 2024-04-08 04:21:09.000000 dew_gwdata-0.81/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-04-08 04:21:22.128111 dew_gwdata-0.81/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2024-04-08 04:21:09.000000 dew_gwdata-0.81/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-08 04:21:09.000000 dew_gwdata-0.81/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.088110 dew_gwdata-0.81/dew_gwdata/
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    54754 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/_aquarius_ts.py
+-rw-rw-rw-   0 root         (0) root         (0)     6215 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/_aquarius_wp.py
+-rw-rw-rw-   0 root         (0) root         (0)    25093 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/_gtslogs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4732 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/_hydstra.py
+-rw-rw-rw-   0 root         (0) root         (0)     3181 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/_sagd_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/_wde.py
+-rw-rw-rw-   0 root         (0) root         (0)     4328 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/charts.py
+-rw-rw-rw-   0 root         (0) root         (0)    65409 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/gwdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/las_to_alias.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_dosbox.conf
+-rw-rw-rw-   0 root         (0) root         (0)     4424 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_dosbox.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.092110 dew_gwdata-0.81/dew_gwdata/logger20_image/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.096110 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/A.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/BAT.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/BJT.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/C.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/CHT.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/COM.BAT
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/CONV.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/DAC.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/DBF.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/DR.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/GK.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/LAS.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/LOG.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/QA.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/QC.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/RJM.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/SD.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/SDU.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/UTILS.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/VF.BAT
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/BAT/W.BAT
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.096110 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.100110 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/AUSIND.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      903 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/CAL13.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      902 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/CAL14.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/CAL7.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      297 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/CAL8.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      729 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB1.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB1CCL.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      481 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB3.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB3CCL.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB8.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      727 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB8CCL.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      915 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DF13.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DF14.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DN13.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DN14.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G11.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G12.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      904 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G13.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      898 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G14.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G1API.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G3API.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G7.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G8API.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      882 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G9.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND1D.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND1M.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      665 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND2D.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND2M.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND3.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/N11.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/N7.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      879 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/N9.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      318 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/PR.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      319 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/PR9.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/PR9P3.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/SP.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/SP9.CHT
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/LOGGER.BAK
+-rw-rw-rw-   0 root         (0) root         (0)      908 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/LOGGER.INI
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/LOGGER.PWD
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.100110 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/ODDENDS/
+-rw-rw-rw-   0 root         (0) root         (0)    29950 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/ODDENDS/counts.exe
+-rw-rw-rw-   0 root         (0) root         (0)    37208 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/ODDENDS/pclog.exe
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.100110 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/
+-rw-rw-rw-   0 root         (0) root         (0)      904 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/LOGGER.INI
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.104110 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/
+-rw-rw-rw-   0 root         (0) root         (0)     1579 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/TOOLLIST.REF
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/default.hea
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/gridlist.ref
+-rw-rw-rw-   0 root         (0) root         (0)      916 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/logger.bak
+-rw-rw-rw-   0 root         (0) root         (0)    11648 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/logger.fnt
+-rw-rw-rw-   0 root         (0) root         (0)      910 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/logger.ini
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/toollist.tmp
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/gridlist.ref
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/logger.dme
+-rw-rw-rw-   0 root         (0) root         (0)    11648 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/logger.fnt
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/logger.id
+-rw-rw-rw-   0 root         (0) root         (0)   361952 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/logger20.exe
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.108110 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/
+-rw-rw-rw-   0 root         (0) root         (0)    17435 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/ADDPATH.EXE
+-rw-rw-rw-   0 root         (0) root         (0)    12920 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/CAGE.EXE
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/CO.COM
+-rw-rw-rw-   0 root         (0) root         (0)    29950 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/COUNTS.EXE
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/FILEDIV.COM
+-rw-rw-rw-   0 root         (0) root         (0)    27088 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/GMOUSE.COM
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/GY.BAT
+-rw-rw-rw-   0 root         (0) root         (0)   121248 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/GYCHECK.EXE
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/HISTORY.TXT
+-rw-rw-rw-   0 root         (0) root         (0)     8032 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/L20COM.OLD
+-rw-rw-rw-   0 root         (0) root         (0)     8064 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/L20COMIO.EXE
+-rw-rw-rw-   0 root         (0) root         (0)     8016 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/LCOM.EXE
+-rw-rw-rw-   0 root         (0) root         (0)    33850 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/PCLOG.EXE
+-rw-rw-rw-   0 root         (0) root         (0)    29378 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/PKUNZIP.EXE
+-rw-rw-rw-   0 root         (0) root         (0)    34296 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/PKZIP.EXE
+-rw-rw-rw-   0 root         (0) root         (0)    47420 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/Q.EXE
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/SLOWDOS.COM
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/SLOWDOS.TXT
+-rw-rw-rw-   0 root         (0) root         (0)     2791 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/SLOWDOS.ZIP
+-rw-rw-rw-   0 root         (0) root         (0)    82328 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/SPEEDCOM.EXE
+-rw-rw-rw-   0 root         (0) root         (0)    91561 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/SYSINFO.EXE
+-rw-rw-rw-   0 root         (0) root         (0)     8467 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/WHEREIS.EXE
+-rw-rw-rw-   0 root         (0) root         (0)    17435 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/addpath.exe
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/autoexec.bat
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/config.sys
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/instal20.bat
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/l20.bat
+-rw-rw-rw-   0 root         (0) root         (0)     8032 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/l20comio.exe
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/logger20_image/readme.txt
+-rw-rw-rw-   0 root         (0) root         (0)      936 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/sageodata_database.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/sageodata_datamart.py
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/spreadsheets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10830 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.108110 dew_gwdata-0.81/dew_gwdata/wde_queries/
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/wde_queries/alerts.sql
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/wde_queries/logger_installations.sql
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/wde_queries/logger_readings.sql
+-rw-rw-rw-   0 root         (0) root         (0)      389 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/wde_queries/maintenance_issues.sql
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.108110 dew_gwdata-0.81/dew_gwdata/webapp/
+-rw-rw-rw-   0 root         (0) root         (0)      906 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.108110 dew_gwdata-0.81/dew_gwdata/webapp/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16097 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/handlers/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2928 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/handlers/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/handlers/home.py
+-rw-rw-rw-   0 root         (0) root         (0)     7314 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/handlers/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     5019 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/handlers/search.py
+-rw-rw-rw-   0 root         (0) root         (0)    23951 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/handlers/well.py
+-rw-rw-rw-   0 root         (0) root         (0)     7436 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/handlers/wells.py
+-rw-rw-rw-   0 root         (0) root         (0)      901 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/log-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/main.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.108110 dew_gwdata-0.81/dew_gwdata/webapp/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4986 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/models/queries.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.112110 dew_gwdata-0.81/dew_gwdata/webapp/static/
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/static/MarkerCluster.Default.css
+-rw-rw-rw-   0 root         (0) root         (0)      872 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/static/MarkerCluster.css
+-rw-rw-rw-   0 root         (0) root         (0)     2927 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/static/dygraph.css
+-rw-rw-rw-   0 root         (0) root         (0)   476414 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/static/dygraph.js
+-rw-rw-rw-   0 root         (0) root         (0)      779 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/static/external-link.svg
+-rw-rw-rw-   0 root         (0) root         (0)    71010 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/static/leaflet.markercluster-src.js
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/static/style.css
+-rw-rw-rw-   0 root         (0) root         (0)    23424 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/static/w3.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.116110 dew_gwdata-0.81/dew_gwdata/webapp/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2137 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/app_layout.html
+-rw-rw-rw-   0 root         (0) root         (0)      342 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/app_layout_schema.html
+-rw-rw-rw-   0 root         (0) root         (0)     2317 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/app_layout_well.html
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/app_layout_wells.html
+-rw-rw-rw-   0 root         (0) root         (0)     4139 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/app_navbar_wells_dropdown.html
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/app_schema.html
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/app_schema_columns.html
+-rw-rw-rw-   0 root         (0) root         (0)     1779 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/app_schema_data.html
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/app_schema_view.html
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/group_summary.html
+-rw-rw-rw-   0 root         (0) root         (0)     3398 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/home.html
+-rw-rw-rw-   0 root         (0) root         (0)     4160 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/well_combined_water_level.html
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/well_construction.html
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/well_drillhole_document_images.html
+-rw-rw-rw-   0 root         (0) root         (0)      771 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/well_drillhole_logs.html
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/well_logger_water_level.html
+-rw-rw-rw-   0 root         (0) root         (0)     2315 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/well_manual_water_level.html
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/well_salinity.html
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/well_summary.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/wells_data_available.html
+-rw-rw-rw-   0 root         (0) root         (0)     3942 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/wells_map.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/templates/wells_summary.html
+-rw-rw-rw-   0 root         (0) root         (0)     3069 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/webapp/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    26235 2024-04-08 04:21:09.000000 dew_gwdata-0.81/dew_gwdata/wilma_reports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.128111 dew_gwdata-0.81/dew_gwdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-04-08 04:21:22.000000 dew_gwdata-0.81/dew_gwdata.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9672 2024-04-08 04:21:22.000000 dew_gwdata-0.81/dew_gwdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-08 04:21:22.000000 dew_gwdata-0.81/dew_gwdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-08 04:21:22.000000 dew_gwdata-0.81/dew_gwdata.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      218 2024-04-08 04:21:22.000000 dew_gwdata-0.81/dew_gwdata.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-04-08 04:21:22.000000 dew_gwdata-0.81/dew_gwdata.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.116110 dew_gwdata-0.81/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/Makefile
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.116110 dew_gwdata-0.81/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/_static/custom.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.116110 dew_gwdata-0.81/docs/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/_templates/parent_links.html
+-rw-rw-rw-   0 root         (0) root         (0)     3719 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/apidocs.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5124 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/charting.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4227 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/dew_gwdata.objects.inv
+-rw-rw-rw-   0 root         (0) root         (0)     4495 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/drillhole-details.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16174 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/elevation.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4491 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/elevation.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.116110 dew_gwdata-0.81/docs/figures/
+-rw-rw-rw-   0 root         (0) root         (0)    25191 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/figures/extract_method.png
+-rw-rw-rw-   0 root         (0) root         (0)    20070 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/figures/measured_during.png
+-rw-rw-rw-   0 root         (0) root         (0)     2990 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/geophysical-logs.rst
+-rw-rw-rw-   0 root         (0) root         (0)    63181 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/groups-networks.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     6185 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/gwdata-access.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16065 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/intro.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)   170314 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/tutorial-water-levels.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   173859 2024-04-08 04:21:09.000000 dew_gwdata-0.81/docs/well-summary-data.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      428 2024-04-08 04:21:09.000000 dew_gwdata-0.81/environment.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.124111 dew_gwdata-0.81/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)    18146 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/1 - How to get water levels for a few wells.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    41200 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/2 - Find all wells in a PWA or PWRA.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    49011 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/3 - Chart salinities for a well.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    23716 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/4 - See all the available predefined queries.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      666 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/How to install dew_gwdata.md
+-rw-rw-rw-   0 root         (0) root         (0)      715 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/Untitled.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   190550 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/chemistry stuff.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    11488 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev - PEPS exports.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    46009 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev - aquifer monitored-Copy1.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    15146 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev - aquifer monitored.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    48794 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev - events query.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    23665 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev - hydrostrat logs integrated.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)  2202594 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev AQ datasets.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    28709 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev AQ locations.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   117484 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev AQTS field visits.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    56568 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev WL between dates.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     7733 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev issue .ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    25467 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev issue 12 - missing ref_elev causes TypeError (MOR252).ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   139018 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev modified_log.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    21636 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev water level times.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    56080 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev wells summary.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    56089 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/dev. wilma_cache.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    25378 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/install_fig0.png
+-rw-rw-rw-   0 root         (0) root         (0)    14171 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/install_fig1.png
+-rw-rw-rw-   0 root         (0) root         (0)    21321 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/install_fig3.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.128111 dew_gwdata-0.81/notebooks/issues/
+-rw-rw-rw-   0 root         (0) root         (0)   115850 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/issues/11 - Hydstra QC undefined is being included.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    11549 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/issues/7 - NRM and landscapes.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/issues/Parsing identifiers from SQL.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    24698 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/issues/Untitled.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    22873 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/nb2_fig1.png
+-rw-rw-rw-   0 root         (0) root         (0)    34810 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/nb3_fig1.png
+-rw-rw-rw-   0 root         (0) root         (0)    17395 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/permit conditions.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    21380 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/permit numbers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    43995 2024-04-08 04:21:09.000000 dew_gwdata-0.81/notebooks/standard salinity graph.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-04-08 04:21:09.000000 dew_gwdata-0.81/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-04-08 04:21:09.000000 dew_gwdata-0.81/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-08 04:21:22.128111 dew_gwdata-0.81/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2024-04-08 04:21:09.000000 dew_gwdata-0.81/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:21:22.128111 dew_gwdata-0.81/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2024-04-08 04:21:09.000000 dew_gwdata-0.81/tests/test_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      787 2024-04-08 04:21:09.000000 dew_gwdata-0.81/tests/test_predefined_queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-08 04:21:09.000000 dew_gwdata-0.81/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-04-08 04:21:09.000000 dew_gwdata-0.81/tests/utils.py
```

### Comparing `dew_gwdata-0.80/.github/workflows/python-ci.yml` & `dew_gwdata-0.81/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/.gitignore` & `dew_gwdata-0.81/.gitignore`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/PKG-INFO` & `dew_gwdata-0.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dew_gwdata
-Version: 0.80
+Version: 0.81
 Summary: Python module for accessing groundwater data internally at DEW
 Home-page: http://github.com/dew-waterscience/dew_gwdata
 Author: Kent Inverarity
 Author-email: kent.inverarity@sa.gov.au
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
```

### Comparing `dew_gwdata-0.80/README.md` & `dew_gwdata-0.81/README.md`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/__init__.py` & `dew_gwdata-0.81/dew_gwdata/__init__.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/_aquarius_ts.py` & `dew_gwdata-0.81/dew_gwdata/_aquarius_ts.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,18 +334,20 @@
                     "UniqueId",
                     "PrimaryFolder",
                     "LastModified",
                     "Publish",
                     "Tags",
                 ]
             )
-        df.loc[:, "tags"] = [
-            "|".join([t["Key"] + ":" + t["Value"] for t in tag_list])
-            for tag_list in df.Tags
-        ]
+        df["tags"] = df.Tags
+        # df["tags"] = "JIRA GD-10"
+        # df.loc[:, "tags"] = [
+        #     "|".join([t["Key"] + ":" + t["Value"] for t in tag_list])
+        #     for tag_list in df.Tags
+        # ]
         df = df[[c for c in df.columns if not c in ("Tags", "IsExternalLocation")]]
         df = df.rename(
             columns={
                 "Name": "loc_name",
                 "Identifier": "loc_id",
                 "UniqueId": "loc_uid",
                 "PrimaryFolder": "folder",
@@ -1144,31 +1146,42 @@
             "2021-09-05T12:00:05.000000+09:30"
         utc_is_null (bool): weird quirk - AQTS gives the
             "start of time" value and "end of time"
             values (years 0000 and 9999) the UTC
             timezone which makes for confusion later on.
             If True, convert any values in UTC to
             ``pd.NaT``.
+    
+    Also deals with the fact AQTS actually uses - :-( -
+    the ISO8601-compliant "24:00:00", which Python
+    doesn't understand.
 
     Returns:
         list of tz-aware datetime objects.
 
     """
     pattern = re.compile(
         r"(\d{4}-\d{2}-\d{2})T(\d{2}:\d{2}:\d{2})\.\d*([-+]{1}\d{2}):(\d{2})"
     )
     format_str = "%Y-%m-%d %H:%M:%S %z"
 
     converted_values = []
     for value in values:
         match = pattern.match(value)
+        date_match = match.group(1)
+        time_match = match.group(2)
+        if match.group(2) == "24:00:00":
+            date = datetime.date.fromisoformat(match.group(1))
+            date += datetime.timedelta(days=1)
+            date_match = date.strftime("%Y-%m-%d")
+            time_match = "00:00:00"
         timestamp = (
-            match.group(1)
+            date_match
             + " "
-            + match.group(2)
+            + time_match
             + " "
             + match.group(3)
             + match.group(4)
         )
         tzone = match.group(3) + match.group(4)
         if tzone[1:] == "0000" and utc_is_null:
             converted_values.append(pd.NaT)
```

### Comparing `dew_gwdata-0.80/dew_gwdata/_aquarius_wp.py` & `dew_gwdata-0.81/dew_gwdata/_aquarius_wp.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         param = "SWL"
     elif param == "rswl":
         param = "RSWL"
     elif param == "ec":
         param = "EC Corr"
     elif param == "tds":
         param = "TDS from EC"
+    elif param == "rainfall":
+        param = "Rainfall"
     else:
         raise KeyError(f"param {repr(param)} not known")
     return param
 
 
 class DEWAquariusWebPortal:
     def __init__(self, server=None, env="prod"):
@@ -46,15 +48,15 @@
         self.portal = aquarius_webportal.AquariusWebPortal(server)
 
     def find_logger_datasets(self, unit_hyphen, param="swl"):
         """Obtain groundwater logger datasets.
 
         Args:
             unit_hyphen (str): unit number in hyphenated form e.g. '7025-808'
-            param (str): either "dtw", "swl", "rswl", "ec", "tds"
+            param (str): either "dtw", "swl", "rswl", "ec", "tds", "rainfall"
             resample_freq (str): a pandas re-sampling frequency or None for
                 the raw data.
 
         """
         param = resolve_param_name(param)
 
         dsets = self.portal.fetch_datasets(param_name=param)
@@ -63,15 +65,15 @@
 
         return dsets
 
     def get_best_available_logger_dataset(self, unit_hyphen, param="swl", **kwargs):
         """Return best available dataset for well.
 
         unit_hyphen (str): groundwater location in AQWP
-        param (str): "dtw", "swl", "rswl", "ec", or "tds".
+        param (str): "dtw", "swl", "rswl", "ec", "tds", or "rainfall"
         freq (str): either "as-recorded" (data points as they exist) or a pandas
             frequency string e.g "6H", "2d" etc.
         max_gap_days (float): maximum allowable gap between data points in days
         keep_grades (tuple): grades to keep. 1 = telemetry, 10 = water level outside
             of recordable range, 15 = poor which GW Team uses to mean "unusable",
             20 = fair, 30 = good. Use None to keep all measurements.
         extra_data_types (str/sequence): The additional metadata fields
@@ -82,15 +84,15 @@
         finish (pd.Timestamp): latest data to retrieve - None by default
 
         Returns:
             list of pd.DataFrame: each df is guaranteed to have no gaps in the
             timestamp column > max_gap_days. The columns of each dataframe are:
 
                 - "timestamp": pd.Timestamp - tz-aware with timezone UTC+09:30 i.e. ACST
-                - the parameter, titled either "dtw", "swl", "rswl", "ec", or "tds"
+                - the parameter, titled either "dtw", "swl", "rswl", "ec", "tds", or "rainfall"
                 - "chunk_id" - this integer increments from 0, 1, 2 depending on how
                     many gaps were found in the data (gaps > max_gap_days above)
 
         """
         dsets = self.find_logger_datasets(unit_hyphen, param)
         for idx, dset in dsets.iterrows():
             if "Best Available" in dset.label:
@@ -125,15 +127,15 @@
             finish (pd.Timestamp): latest data to retrieve - None by default
 
         Returns:
             list of pd.DataFrame: each df is guaranteed to have no gaps in the
             timestamp column > max_gap_days. The columns of each dataframe are:
 
                 - "timestamp": pd.Timestamp - tz-aware with timezone UTC+09:30 i.e. ACST
-                - the parameter, titled either "dtw", "swl", "rswl", "ec", or "tds"
+                - the parameter, titled either "dtw", "swl", "rswl", "ec", "tds" or "rainfall"
                 - "chunk_id" - this integer increments from 0, 1, 2 depending on how
                   many gaps were found in the data (gaps > max_gap_days above)
 
         """
         if extra_data_types:
             assert list(sorted(extra_data_types)) in (
                 ["grade"],
```

### Comparing `dew_gwdata-0.80/dew_gwdata/_gtslogs.py` & `dew_gwdata-0.81/dew_gwdata/_gtslogs.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/_hydstra.py` & `dew_gwdata-0.81/dew_gwdata/_hydstra.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/_sagd_api.py` & `dew_gwdata-0.81/dew_gwdata/_sagd_api.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/charts.py` & `dew_gwdata-0.81/dew_gwdata/charts.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/gwdata.py` & `dew_gwdata-0.81/dew_gwdata/gwdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,27 +42,22 @@
             replaced wells.
         conn (sageodata_db.Connection): server
         aq (dew_gwdata.DEWAquarius): server
         ts_agg_ndays (int): aggregate continuous TS data from AQTS to
             a given number of days
         ts_agg_methods (dict): how to aggregate AQ TS data.
             None means to use :func:`dew_gwdata.reduce_to_interval`'s
-            default argument.
+            default argument which assumes the dataset parameter being
+            sought is "Depth to Water".
 
     Other keyword arguments are passed to
     :func:`dew_gwdata.DEWAquarius.fetch_timeseries_data`
 
     Aquarius data is retrieved from Aquarius TimeSeries production.
 
-    Note that by default the logger data from Hydstra is requested as the
-    mean of every 5 day window of data. You can increase the frequency (and
-    time taken for the request) by using the *interval* and *multiplier* keyword
-    arguments to this function. They are documented in
-    :func:`dew_gwdata.fetch_hydstra_dtw_data`.
-
     Returns:
         :class:`pandas.DataFrame`
 
     """
     if conn is None:
         conn = connect_to_sageodata()
     if aq is None:
@@ -114,23 +109,24 @@
                 ts_uid = aq_md2.ts_uid.iloc[0]
                 print(f"one found - using {ts_uid}")
             else:
                 ts_uid = aq_md2.ts_uid.iloc[0]
                 logger.warning(f"multiple timeseries: using {ts_uid}")
             if not ts_uid is None:
                 print(f"Fetching AQTS data for {aq_locid} ts_uid={ts_uid}")
-                dfs = aq.fetch_timeseries_data(ts_uid=ts_uid)
+                dfs = aq.fetch_timeseries_data(ts_uid=ts_uid, **kwargs)
                 df = join_logger_data_intervals(dfs, param_if_empty="dtw")
                 #     locid=aq_locid, param="Depth to Water", label=label, label_startswith=False
                 # )
                 print(f"fetched {len(df)} data points")
                 print(
                     f"before reduction to {ts_agg_ndays} days ts_agg_methods={ts_agg_methods}: {len(df)} data points, {df.columns}"
                 )
                 if len(df):
+                    print(f"df columns = {df.columns}")
                     df = reduce_to_interval(
                         df, ts_agg_ndays, dt_col="timestamp", aggs=ts_agg_methods
                     )
                 else:
                     print("skipped reduction - df has no records")
                 print(f"after reduction: {len(df)} data points, {df.columns}")
                 df = df.rename(
@@ -193,28 +189,33 @@
 ):
     """Reduce to a less frequent daily interval e.g. daily, weekly, monthly.
 
     Args:
         df (pandas.DataFrame): dataset
         ndays (int): number of days (interval length)
         dt_col (str): name of column in *df* containing the timestamps
+        aggs (dict): optional dictionary. keys are column names and values
+            are functions to aggregate (or string value shortcuts used in pandas
+            groupby.aggregate e.g. "mean", "min", "first").
 
     Returns:
         A pandas.DataFrame. The index is a set of datetime objects spaced at an
         interval of *ndays*; the values are those from *data_col*, aggregated by
         the method *agg_method*.
 
     """
     if aggs is None:
         aggs = {
-            "Depth to Water": "mean",
             "grade": "min",
             "approval": "first",
             "qualifier": "first",
         }
+        for col in ["Depth to Water", "dtw", "SWL", "swl", "RSWL", "rswl", "tds", "ec"]:
+            if col in df.columns:
+                aggs[col] = "mean"
     print(f"Reducing data by ndays={ndays} dt_col={dt_col} aggs={aggs}")
     offset = pd.Timedelta(ndays, "d") / 2
     grouper = pd.Grouper(key=dt_col, freq=f"{ndays:.0f}d", label="left")
     print(f"offset={offset} grouper={grouper}")
     df2 = df.groupby(grouper)[list(aggs.keys())].agg(aggs)
     df2 = df2.shift(1, freq=(offset)).reset_index()
     return df2
```

### Comparing `dew_gwdata-0.80/dew_gwdata/las_to_alias.csv` & `dew_gwdata-0.81/dew_gwdata/las_to_alias.csv`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_dosbox.conf` & `dew_gwdata-0.81/dew_gwdata/logger20_dosbox.conf`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_dosbox.py` & `dew_gwdata-0.81/dew_gwdata/logger20_dosbox.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/CAL13.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/CAL13.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/CAL14.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/CAL14.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB1.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB1.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB1CCL.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB1CCL.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB8.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB8.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB8CCL.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DB8CCL.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DF13.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DF13.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DF14.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DF14.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DN13.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DN13.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/DN14.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/DN14.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G11.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G11.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G12.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G12.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G13.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G13.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G14.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G14.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G1API.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G1API.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G7.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G7.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G8API.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G8API.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/G9.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/G9.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND1D.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND1D.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND1M.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND1M.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND2D.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND2D.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND2M.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/IND2M.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/N11.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/N11.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/CHARTS/N9.CHT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/CHARTS/N9.CHT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/LOGGER.BAK` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/LOGGER.BAK`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/LOGGER.INI` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/LOGGER.INI`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/ODDENDS/counts.exe` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/ODDENDS/counts.exe`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/ODDENDS/pclog.exe` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/ODDENDS/pclog.exe`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/LOGGER.INI` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/LOGGER.INI`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/TOOLLIST.REF` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/TOOLLIST.REF`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/gridlist.ref` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/gridlist.ref`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/logger.bak` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/logger.bak`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/logger.fnt` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/logger.fnt`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/logger.ini` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/PROJECTS/TMP/logger.ini`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/gridlist.ref` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/gridlist.ref`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/logger.fnt` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/logger.fnt`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/LOGGER20/logger20.exe` & `dew_gwdata-0.81/dew_gwdata/logger20_image/LOGGER20/logger20.exe`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/ADDPATH.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/ADDPATH.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/CAGE.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/CAGE.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/CO.COM` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/CO.COM`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/COUNTS.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/COUNTS.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/GMOUSE.COM` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/GMOUSE.COM`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/GYCHECK.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/GYCHECK.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/HISTORY.TXT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/HISTORY.TXT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/L20COM.OLD` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/L20COM.OLD`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/L20COMIO.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/L20COMIO.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/LCOM.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/LCOM.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/PCLOG.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/PCLOG.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/PKUNZIP.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/PKUNZIP.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/PKZIP.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/PKZIP.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/Q.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/Q.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/SLOWDOS.COM` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/SLOWDOS.COM`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/SLOWDOS.TXT` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/SLOWDOS.TXT`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/SLOWDOS.ZIP` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/SLOWDOS.ZIP`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/SPEEDCOM.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/SPEEDCOM.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/SYSINFO.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/SYSINFO.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/UTILS/WHEREIS.EXE` & `dew_gwdata-0.81/dew_gwdata/logger20_image/UTILS/WHEREIS.EXE`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/addpath.exe` & `dew_gwdata-0.81/dew_gwdata/logger20_image/addpath.exe`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/l20comio.exe` & `dew_gwdata-0.81/dew_gwdata/logger20_image/l20comio.exe`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/logger20_image/readme.txt` & `dew_gwdata-0.81/dew_gwdata/logger20_image/readme.txt`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/sageodata_database.py` & `dew_gwdata-0.81/dew_gwdata/sageodata_database.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/spreadsheets.py` & `dew_gwdata-0.81/dew_gwdata/spreadsheets.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/utils.py` & `dew_gwdata-0.81/dew_gwdata/utils.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/README.md` & `dew_gwdata-0.81/dew_gwdata/webapp/README.md`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/handlers/api.py` & `dew_gwdata-0.81/dew_gwdata/webapp/handlers/api.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/handlers/groups.py` & `dew_gwdata-0.81/dew_gwdata/webapp/handlers/groups.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/handlers/home.py` & `dew_gwdata-0.81/dew_gwdata/webapp/handlers/home.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/handlers/schema.py` & `dew_gwdata-0.81/dew_gwdata/webapp/handlers/schema.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/handlers/search.py` & `dew_gwdata-0.81/dew_gwdata/webapp/handlers/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,18 +80,22 @@
     types = []
     if unit_no:
         types.append("unit_no")
     if obs_no:
         types.append("obs_no")
     if dh_no:
         types.append("dh_no")
+    print(f"looking for types: {types}")
     wells = db.find_wells(query, types=types).df()
+    print(f"Found wells: \n{wells}")
     if len(wells) == 0:
         raise Exception("No wells found")
     elif len(wells) == 1:
+        if redirect_to == "wells_summary":
+            redirect_to = "well_summary"
         return RedirectResponse(
             f"/app/{redirect_to}?dh_no={wells.iloc[0].dh_no:.0f}&env={env}"
         )
     else:
         url_str = webapp_utils.dhnos_to_urlstr(wells.dh_no)
         return RedirectResponse(f"/app/{redirect_to}?url_str={url_str}&env={env}")
```

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/handlers/well.py` & `dew_gwdata-0.81/dew_gwdata/webapp/handlers/well.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,31 +349,32 @@
         f"&start={start_str}"
         f"&finish={finish_str}"
         f"&env={env}"
         f"&aqts_env={aqts_env}"
         f"&format=csv"
     )
     dsets = gd.get_logger_interval_details(dfs)
-    dsets["csv_download"] = dsets.apply(
-        lambda row: (
-            f"<a href='"
-            f"/api/well_best_available_combined_water_level_data"
-            f"?url_str={url_str}"
-            f"&param={param}"
-            f"&freq={freq}"
-            f"&keep_grades={keep_grades_str}"
-            f"&max_gap_days={int(max_gap_days)}"
-            f"&start={row.start_timestamp.strftime('%Y-%m-%d %H:%M:%S')}"
-            f"&finish={row.finish_timestamp.strftime('%Y-%m-%d %H:%M:%S')}"
-            f"&env={env}"
-            f"&aqts_env={aqts_env}"
-            f"&format=csv"
-            f"'>{row.dataset_length}-row CSV</a>"
-        ), axis=1
-    )
+    if len(dsets):
+        dsets["csv_download"] = dsets.apply(
+            lambda row: (
+                f"<a href='"
+                f"/api/well_best_available_combined_water_level_data"
+                f"?url_str={url_str}"
+                f"&param={param}"
+                f"&freq={freq}"
+                f"&keep_grades={keep_grades_str}"
+                f"&max_gap_days={int(max_gap_days)}"
+                f"&start={row.start_timestamp.strftime('%Y-%m-%d %H:%M:%S')}"
+                f"&finish={row.finish_timestamp.strftime('%Y-%m-%d %H:%M:%S')}"
+                f"&env={env}"
+                f"&aqts_env={aqts_env}"
+                f"&format=csv"
+                f"'>{row.dataset_length}-row CSV</a>"
+            ), axis=1
+        )
     dsets_table = webapp_utils.frame_to_html(dsets)
 
     return templates.TemplateResponse(
         "well_combined_water_level.html",
         {
             "request": request,
             "env": env,
```

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/handlers/wells.py` & `dew_gwdata-0.81/dew_gwdata/webapp/handlers/wells.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/log-config.yaml` & `dew_gwdata-0.81/dew_gwdata/webapp/log-config.yaml`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/main.py` & `dew_gwdata-0.81/dew_gwdata/webapp/main.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/models/queries.py` & `dew_gwdata-0.81/dew_gwdata/webapp/models/queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,14 +113,26 @@
 
         elif self.name_fragment:
             wells = db.drillhole_details_by_name_search(self.name_fragment)
             name = f"Search for '{self.name_fragment}'"
             name_safe = f"search_{self.name_fragment}"
             query_params = [f"name_fragment={self.name_fragment}"]
 
+        else:
+            wells = db.drillhole_details([0])
+            name = f"Empty search??"
+            name_safe = f"empty"
+            query_params = [
+                f"idq=",
+                f"idq_unit_no=1",
+                f"idq_obs_no=1",
+                f"idq_dh_no=0",
+                f"idq_dh_no_as_req=0",
+            ]
+
         if self.sort == "dh_no":
             query_params.append("sort=dh_no")
         elif self.sort == "unit_hyphen":
             query_params.append("sort=unit_hyphen")
 
         # Filter
         ## TODO
```

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/static/MarkerCluster.Default.css` & `dew_gwdata-0.81/dew_gwdata/webapp/static/MarkerCluster.Default.css`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/static/MarkerCluster.css` & `dew_gwdata-0.81/dew_gwdata/webapp/static/MarkerCluster.css`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/static/dygraph.css` & `dew_gwdata-0.81/dew_gwdata/webapp/static/dygraph.css`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/static/dygraph.js` & `dew_gwdata-0.81/dew_gwdata/webapp/static/dygraph.js`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/static/external-link.svg` & `dew_gwdata-0.81/dew_gwdata/webapp/static/external-link.svg`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/static/leaflet.markercluster-src.js` & `dew_gwdata-0.81/dew_gwdata/webapp/static/leaflet.markercluster-src.js`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/static/style.css` & `dew_gwdata-0.81/dew_gwdata/webapp/static/style.css`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/static/w3.css` & `dew_gwdata-0.81/dew_gwdata/webapp/static/w3.css`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/app_layout.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/app_layout.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/app_layout_well.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/app_layout_well.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/app_layout_wells.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/app_layout_wells.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/app_navbar_wells_dropdown.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/app_navbar_wells_dropdown.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/app_schema.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/app_schema.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/app_schema_columns.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/app_schema_columns.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/app_schema_data.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/app_schema_data.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/home.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/home.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/well_combined_water_level.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/well_combined_water_level.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/well_construction.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/well_construction.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/well_drillhole_document_images.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/well_drillhole_document_images.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/well_drillhole_logs.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/well_drillhole_logs.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/well_logger_water_level.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/well_logger_water_level.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/well_manual_water_level.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/well_manual_water_level.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/well_salinity.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/well_salinity.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/well_summary.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/well_summary.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/templates/wells_map.html` & `dew_gwdata-0.81/dew_gwdata/webapp/templates/wells_map.html`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/webapp/utils.py` & `dew_gwdata-0.81/dew_gwdata/webapp/utils.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata/wilma_reports.py` & `dew_gwdata-0.81/dew_gwdata/wilma_reports.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/dew_gwdata.egg-info/PKG-INFO` & `dew_gwdata-0.81/dew_gwdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dew_gwdata
-Version: 0.80
+Version: 0.81
 Summary: Python module for accessing groundwater data internally at DEW
 Home-page: http://github.com/dew-waterscience/dew_gwdata
 Author: Kent Inverarity
 Author-email: kent.inverarity@sa.gov.au
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
```

### Comparing `dew_gwdata-0.80/dew_gwdata.egg-info/SOURCES.txt` & `dew_gwdata-0.81/dew_gwdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/Makefile` & `dew_gwdata-0.81/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/apidocs.rst` & `dew_gwdata-0.81/docs/apidocs.rst`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/changelog.rst` & `dew_gwdata-0.81/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/charting.rst` & `dew_gwdata-0.81/docs/charting.rst`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/conf.py` & `dew_gwdata-0.81/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/dew_gwdata.objects.inv` & `dew_gwdata-0.81/docs/dew_gwdata.objects.inv`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/drillhole-details.rst` & `dew_gwdata-0.81/docs/drillhole-details.rst`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/elevation.ipynb` & `dew_gwdata-0.81/docs/elevation.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/elevation.md` & `dew_gwdata-0.81/docs/elevation.md`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/figures/extract_method.png` & `dew_gwdata-0.81/docs/figures/extract_method.png`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/figures/measured_during.png` & `dew_gwdata-0.81/docs/figures/measured_during.png`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/geophysical-logs.rst` & `dew_gwdata-0.81/docs/geophysical-logs.rst`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/groups-networks.ipynb` & `dew_gwdata-0.81/docs/groups-networks.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/gwdata-access.rst` & `dew_gwdata-0.81/docs/gwdata-access.rst`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/index.rst` & `dew_gwdata-0.81/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/installation.rst` & `dew_gwdata-0.81/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/intro.ipynb` & `dew_gwdata-0.81/docs/intro.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/make.bat` & `dew_gwdata-0.81/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/tutorial-water-levels.ipynb` & `dew_gwdata-0.81/docs/tutorial-water-levels.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/docs/well-summary-data.ipynb` & `dew_gwdata-0.81/docs/well-summary-data.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/1 - How to get water levels for a few wells.ipynb` & `dew_gwdata-0.81/notebooks/1 - How to get water levels for a few wells.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/2 - Find all wells in a PWA or PWRA.ipynb` & `dew_gwdata-0.81/notebooks/2 - Find all wells in a PWA or PWRA.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/3 - Chart salinities for a well.ipynb` & `dew_gwdata-0.81/notebooks/3 - Chart salinities for a well.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/4 - See all the available predefined queries.ipynb` & `dew_gwdata-0.81/notebooks/4 - See all the available predefined queries.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/How to install dew_gwdata.md` & `dew_gwdata-0.81/notebooks/How to install dew_gwdata.md`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/README.md` & `dew_gwdata-0.81/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/Untitled.ipynb` & `dew_gwdata-0.81/notebooks/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/chemistry stuff.ipynb` & `dew_gwdata-0.81/notebooks/chemistry stuff.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev - PEPS exports.ipynb` & `dew_gwdata-0.81/notebooks/dev - PEPS exports.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev - aquifer monitored-Copy1.ipynb` & `dew_gwdata-0.81/notebooks/dev - aquifer monitored-Copy1.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev - aquifer monitored.ipynb` & `dew_gwdata-0.81/notebooks/dev - aquifer monitored.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev - events query.ipynb` & `dew_gwdata-0.81/notebooks/dev - events query.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev - hydrostrat logs integrated.ipynb` & `dew_gwdata-0.81/notebooks/dev - hydrostrat logs integrated.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev AQ datasets.ipynb` & `dew_gwdata-0.81/notebooks/dev AQ datasets.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev AQ locations.ipynb` & `dew_gwdata-0.81/notebooks/dev AQ locations.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev AQTS field visits.ipynb` & `dew_gwdata-0.81/notebooks/dev AQTS field visits.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev WL between dates.ipynb` & `dew_gwdata-0.81/notebooks/dev WL between dates.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev issue .ipynb` & `dew_gwdata-0.81/notebooks/dev issue .ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev issue 12 - missing ref_elev causes TypeError (MOR252).ipynb` & `dew_gwdata-0.81/notebooks/dev issue 12 - missing ref_elev causes TypeError (MOR252).ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev modified_log.ipynb` & `dew_gwdata-0.81/notebooks/dev modified_log.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev water level times.ipynb` & `dew_gwdata-0.81/notebooks/dev water level times.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev wells summary.ipynb` & `dew_gwdata-0.81/notebooks/dev wells summary.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/dev. wilma_cache.ipynb` & `dew_gwdata-0.81/notebooks/dev. wilma_cache.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/install_fig0.png` & `dew_gwdata-0.81/notebooks/install_fig0.png`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/install_fig1.png` & `dew_gwdata-0.81/notebooks/install_fig1.png`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/install_fig3.png` & `dew_gwdata-0.81/notebooks/install_fig3.png`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/issues/11 - Hydstra QC undefined is being included.ipynb` & `dew_gwdata-0.81/notebooks/issues/11 - Hydstra QC undefined is being included.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/issues/7 - NRM and landscapes.ipynb` & `dew_gwdata-0.81/notebooks/issues/7 - NRM and landscapes.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/issues/Parsing identifiers from SQL.ipynb` & `dew_gwdata-0.81/notebooks/issues/Parsing identifiers from SQL.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/issues/Untitled.ipynb` & `dew_gwdata-0.81/notebooks/issues/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/nb2_fig1.png` & `dew_gwdata-0.81/notebooks/nb2_fig1.png`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/nb3_fig1.png` & `dew_gwdata-0.81/notebooks/nb3_fig1.png`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/permit conditions.ipynb` & `dew_gwdata-0.81/notebooks/permit conditions.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/permit numbers.ipynb` & `dew_gwdata-0.81/notebooks/permit numbers.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/notebooks/standard salinity graph.ipynb` & `dew_gwdata-0.81/notebooks/standard salinity graph.ipynb`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/setup.py` & `dew_gwdata-0.81/setup.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/tests/test_connection.py` & `dew_gwdata-0.81/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `dew_gwdata-0.80/tests/test_predefined_queries.py` & `dew_gwdata-0.81/tests/test_predefined_queries.py`

 * *Files identical despite different names*

