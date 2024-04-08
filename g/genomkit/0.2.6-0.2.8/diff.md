# Comparing `tmp/genomkit-0.2.6.tar.gz` & `tmp/genomkit-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomkit-0.2.6.tar", last modified: Sat Mar  2 20:40:59 2024, max compression
+gzip compressed data, was "genomkit-0.2.8.tar", last modified: Mon Apr  8 08:58:45 2024, max compression
```

## Comparing `genomkit-0.2.6.tar` & `genomkit-0.2.8.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:59.115564 genomkit-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-02 20:40:54.000000 genomkit-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-02 20:40:59.115564 genomkit-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-02 20:40:54.000000 genomkit-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:59.111564 genomkit-0.2.6/genomkit/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:59.111564 genomkit-0.2.6/genomkit/alignments/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/alignments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/alignments/galignments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:59.111564 genomkit-0.2.6/genomkit/annotation/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/annotation/gannotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:59.111564 genomkit-0.2.6/genomkit/coverages/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/coverages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/coverages/gcoverages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:59.107565 genomkit-0.2.6/genomkit/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:59.111564 genomkit-0.2.6/genomkit/data/chrom_size/
--rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/data/chrom_size/chrom.sizes.hg19
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/data/chrom_size/chrom.sizes.hg38
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/data/chrom_size/chrom.sizes.mm10
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/data/chrom_size/chrom.sizes.mm39
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/data/chrom_size/chrom.sizes.mm9
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/data/chrom_size/chrom.sizes.tair10
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/data/chrom_size/chrom.sizes.zv10
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/data/chrom_size/chrom.sizes.zv9
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:59.115564 genomkit-0.2.6/genomkit/regions/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/regions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10103 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/regions/gregion.py
--rw-r--r--   0 runner    (1001) docker     (127)    43825 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/regions/gregions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/regions/gregions_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/regions/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/regions/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:59.115564 genomkit-0.2.6/genomkit/sequences/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/sequences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/sequences/gsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/sequences/gsequences.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/sequences/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:59.115564 genomkit-0.2.6/genomkit/variants/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/variants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/variants/gvariant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-02 20:40:54.000000 genomkit-0.2.6/genomkit/variants/gvariants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:59.111564 genomkit-0.2.6/genomkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-02 20:40:59.000000 genomkit-0.2.6/genomkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-02 20:40:59.000000 genomkit-0.2.6/genomkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 20:40:59.000000 genomkit-0.2.6/genomkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-02 20:40:59.000000 genomkit-0.2.6/genomkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-02 20:40:59.000000 genomkit-0.2.6/genomkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-02 20:40:54.000000 genomkit-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 20:40:59.115564 genomkit-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-03-02 20:40:54.000000 genomkit-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:59.115564 genomkit-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 20:40:54.000000 genomkit-0.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-03-02 20:40:54.000000 genomkit-0.2.6/tests/test_gannotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-03-02 20:40:54.000000 genomkit-0.2.6/tests/test_gcoverages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-02 20:40:54.000000 genomkit-0.2.6/tests/test_gregion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-03-02 20:40:54.000000 genomkit-0.2.6/tests/test_gregions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-02 20:40:54.000000 genomkit-0.2.6/tests/test_gsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-02 20:40:54.000000 genomkit-0.2.6/tests/test_gsequences.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:45.721935 genomkit-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 08:58:40.000000 genomkit-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-08 08:58:45.721935 genomkit-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-08 08:58:40.000000 genomkit-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:45.717935 genomkit-0.2.8/genomkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:45.717935 genomkit-0.2.8/genomkit/alignments/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/alignments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/alignments/galignments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:45.717935 genomkit-0.2.8/genomkit/annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/annotation/gannotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:45.717935 genomkit-0.2.8/genomkit/coverages/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/coverages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11782 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/coverages/gcoverages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/coverages/gcoverages_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:45.713935 genomkit-0.2.8/genomkit/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:45.717935 genomkit-0.2.8/genomkit/data/chrom_size/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/data/chrom_size/chrom.sizes.hg19
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/data/chrom_size/chrom.sizes.hg38
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/data/chrom_size/chrom.sizes.mm10
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/data/chrom_size/chrom.sizes.mm39
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/data/chrom_size/chrom.sizes.mm9
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/data/chrom_size/chrom.sizes.tair10
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/data/chrom_size/chrom.sizes.zv10
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/data/chrom_size/chrom.sizes.zv9
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:45.721935 genomkit-0.2.8/genomkit/regions/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/regions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/regions/gregion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45268 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/regions/gregions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33114 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/regions/gregions_intervaltree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/regions/gregions_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/regions/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/regions/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:45.721935 genomkit-0.2.8/genomkit/sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/sequences/gsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/sequences/gsequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/sequences/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:45.721935 genomkit-0.2.8/genomkit/variants/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/variants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/variants/gvariant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-08 08:58:40.000000 genomkit-0.2.8/genomkit/variants/gvariants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:45.717935 genomkit-0.2.8/genomkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-08 08:58:45.000000 genomkit-0.2.8/genomkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-08 08:58:45.000000 genomkit-0.2.8/genomkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:58:45.000000 genomkit-0.2.8/genomkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 08:58:45.000000 genomkit-0.2.8/genomkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 08:58:45.000000 genomkit-0.2.8/genomkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 08:58:40.000000 genomkit-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 08:58:45.721935 genomkit-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-08 08:58:40.000000 genomkit-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:45.721935 genomkit-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:58:40.000000 genomkit-0.2.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-08 08:58:40.000000 genomkit-0.2.8/tests/test_gannotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-08 08:58:40.000000 genomkit-0.2.8/tests/test_gcoverages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-08 08:58:40.000000 genomkit-0.2.8/tests/test_gregion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-04-08 08:58:40.000000 genomkit-0.2.8/tests/test_gregions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-08 08:58:40.000000 genomkit-0.2.8/tests/test_gregionstree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-08 08:58:40.000000 genomkit-0.2.8/tests/test_gsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-08 08:58:40.000000 genomkit-0.2.8/tests/test_gsequences.py
```

### Comparing `genomkit-0.2.6/LICENSE` & `genomkit-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `genomkit-0.2.6/PKG-INFO` & `genomkit-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomkit
-Version: 0.2.6
+Version: 0.2.8
 Summary: genomkit
 Home-page: https://github.com/chaochungkuo/genomkit
 Author: Chao-Chung Kuo
 Author-email: chao-chung.kuo@rwth-aachen.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `genomkit-0.2.6/README.md` & `genomkit-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `genomkit-0.2.6/genomkit/alignments/galignments.py` & `genomkit-0.2.8/genomkit/alignments/galignments.py`

 * *Files identical despite different names*

### Comparing `genomkit-0.2.6/genomkit/annotation/gannotation.py` & `genomkit-0.2.8/genomkit/annotation/gannotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.load_data()
 
     def load_data(self):
         """Load the file."""
         open_func = gzip.open if self.file_path.endswith('.gz') else open
         total_lines = sum(1 for _ in open_func(self.file_path, 'rt'))
         with open_func(self.file_path, 'rt') as f:
-            for line in tqdm(f, total=total_lines, desc="Loading Data"):
+            for line in tqdm(f, total=total_lines, desc="Loading GTF"):
                 if line.startswith('#'):
                     continue
                 fields = line.strip().split('\t')
                 if self.file_format == 'gtf':
                     feature_type = fields[2]
                     attributes = dict(item.strip().split(' ')
                                       for item in fields[8].split(';')
```

### Comparing `genomkit-0.2.6/genomkit/regions/gregion.py` & `genomkit-0.2.8/genomkit/regions/gregion.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,36 +232,40 @@
         :param center: Define the new center, defaults to "mid_point", other
                        options are "5prime" and "3prime"
         :type center: str, optional
         :return: A resized GRegion
         :rtype: GRegion
         """
         if center == "mid_point":
-            center = int(0.5*(self.end-self.start))
+            center = self.start + int(0.5*(self.end-self.start))
             if self.orientation == "-":
-                start = center+extend_upstream
-                end = center-extend_downstream
+                start = center-extend_downstream
+                end = center+extend_upstream
             else:
                 start = center-extend_upstream
                 end = center+extend_downstream
         elif center == "5prime":
             if self.orientation == "-":
                 center = self.end
-                start = center+extend_upstream
-                end = center-extend_downstream
+                start = center-extend_downstream
+                end = center+extend_upstream
             else:
                 center = self.start
                 start = center-extend_upstream
                 end = center+extend_downstream
         elif center == "3prime":
             if self.orientation == "-":
                 center = self.start
-                start = center+extend_upstream
-                end = center-extend_downstream
+                start = center-extend_downstream
+                end = center+extend_upstream
             else:
                 center = self.end
                 start = center-extend_upstream
                 end = center+extend_downstream
+        if start < 0:
+            start = 0
+        if end < 0:
+            end = 0
         res = GRegion(sequence=self.sequence, start=start, end=end,
                       orientation=self.orientation, score=self.score,
                       name=self.name, data=self.data)
         return res
```

### Comparing `genomkit-0.2.6/genomkit/regions/gregions.py` & `genomkit-0.2.8/genomkit/regions/gregions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from genomkit import GRegion
 import copy
 import numpy as np
 from .io import load_BED
 import os
 import sys
 from copy import deepcopy
+from tqdm import tqdm
 
 
 ###########################################################################
 # GRegions
 ###########################################################################
 class GRegions:
     """
@@ -288,136 +289,143 @@
         """
         new_regions = GRegions(self.name)
         if len(self) == 0 or len(target) == 0:
             return new_regions
         else:
             a = copy.deepcopy(self)
             b = copy.deepcopy(target)
-            if not a.sorted:
-                a.sort()
-            if not b.sorted:
-                b.sort()
-            if mode == "OVERLAP":
-                a.merge()
-                b.merge()
+            # if not a.sorted:
+            #     a.sort()
+            # if not b.sorted:
+            #     b.sort()
+            # if mode == "OVERLAP":
+            #     a.merge()
+            #     b.merge()
 
             iter_a = iter(a)
             s = next(iter_a)
             last_j = len(b) - 1
             j = 0
             cont_loop = True
             pre_inter = 0
             cont_overlap = False
             # OVERLAP ###############################
             if mode == "OVERLAP":
-                while cont_loop:
-                    # When the regions overlap
-                    if s.overlap(b[j]):
-                        new_regions.add(GRegion(sequence=s.sequence,
-                                                start=max(s.start, b[j].start),
-                                                end=min(s.end, b[j].end),
-                                                name=s.name,
-                                                orientation=s.orientation,
-                                                data=s.data))
-                        if not cont_overlap:
-                            pre_inter = j
-                        if j == last_j:
+                with tqdm(total=len(b), desc="Calculate intersects") as pbar:
+                    while cont_loop:
+                        # When the regions overlap
+                        if s.overlap(b[j]):
+                            new_regions.add(GRegion(sequence=s.sequence,
+                                                    start=max(s.start,
+                                                              b[j].start),
+                                                    end=min(s.end, b[j].end),
+                                                    name=s.name,
+                                                    orientation=s.orientation,
+                                                    data=s.data))
+                            if not cont_overlap:
+                                pre_inter = j
+                            if j == last_j:
+                                try:
+                                    s = next(iter_a)
+                                except StopIteration:
+                                    cont_loop = False
+                            else:
+                                j += 1
+                            cont_overlap = True
+
+                        elif s < b[j]:
                             try:
                                 s = next(iter_a)
+                                if s.sequence == b[j].sequence and \
+                                        pre_inter > 0:
+                                    j = pre_inter
+                                cont_overlap = False
                             except StopIteration:
                                 cont_loop = False
-                        else:
-                            j += 1
-                        cont_overlap = True
-
-                    elif s < b[j]:
-                        try:
-                            s = next(iter_a)
-                            if s.sequence == b[j].sequence and pre_inter > 0:
-                                j = pre_inter
-                            cont_overlap = False
-                        except StopIteration:
-                            cont_loop = False
 
-                    elif s > b[j]:
-                        if j == last_j:
-                            cont_loop = False
+                        elif s > b[j]:
+                            if j == last_j:
+                                cont_loop = False
+                            else:
+                                j += 1
+                                cont_overlap = False
                         else:
-                            j += 1
-                            cont_overlap = False
-                    else:
-                        try:
-                            s = next(iter_a)
-                        except StopIteration:
-                            cont_loop = False
-
+                            try:
+                                s = next(iter_a)
+                            except StopIteration:
+                                cont_loop = False
+                        pbar.update(1)
             # ORIGINAL ###############################
             if mode == "ORIGINAL":
-                while cont_loop:
-                    # When the regions overlap
-                    if s.overlap(b[j]):
-                        new_regions.add(s)
-                        try:
-                            s = next(iter_a)
-                        except StopIteration:
-                            cont_loop = False
-                    elif s < b[j]:
-                        try:
-                            s = next(iter_a)
-                        except StopIteration:
-                            cont_loop = False
-                    elif s > b[j]:
-                        if j == last_j:
-                            cont_loop = False
-                        else:
-                            j += 1
-                    else:
-                        try:
-                            s = next(iter_a)
-                        except StopIteration:
-                            cont_loop = False
-            # COMP_INCL ###############################
-            if mode == "COMP_INCL":
-                while cont_loop:
-                    # When the regions overlap
-                    if s.overlap(b[j]):
-                        if s.start >= b[j].start and s.end <= b[j].end:
+                with tqdm(total=len(b), desc="Calculate intersects") as pbar:
+                    while cont_loop:
+                        # When the regions overlap
+                        if s.overlap(b[j]):
                             new_regions.add(s)
-                        if not cont_overlap:
-                            pre_inter = j
-                        if j == last_j:
                             try:
                                 s = next(iter_a)
                             except StopIteration:
                                 cont_loop = False
+                        elif s < b[j]:
+                            try:
+                                s = next(iter_a)
+                            except StopIteration:
+                                cont_loop = False
+                        elif s > b[j]:
+                            if j == last_j:
+                                cont_loop = False
+                            else:
+                                j += 1
                         else:
-                            j += 1
-                        cont_overlap = True
+                            try:
+                                s = next(iter_a)
+                            except StopIteration:
+                                cont_loop = False
+                        pbar.update(1)
+            # COMP_INCL ###############################
+            if mode == "COMP_INCL":
+                with tqdm(total=len(b), desc="Calculate intersects") as pbar:
+                    while cont_loop:
+                        # When the regions overlap
+                        if s.overlap(b[j]):
+                            if s.start >= b[j].start and s.end <= b[j].end:
+                                new_regions.add(s)
+                            if not cont_overlap:
+                                pre_inter = j
+                            if j == last_j:
+                                try:
+                                    s = next(iter_a)
+                                except StopIteration:
+                                    cont_loop = False
+                            else:
+                                j += 1
+                            cont_overlap = True
 
-                    elif s < b[j]:
-                        try:
-                            s = next(iter_a)
-                            if s.sequence == b[j].sequence and pre_inter > 0:
-                                j = pre_inter
-                            cont_overlap = False
-                        except StopIteration:
-                            cont_loop = False
+                        elif s < b[j]:
+                            try:
+                                s = next(iter_a)
+                                if s.sequence == b[j].sequence and \
+                                        pre_inter > 0:
+                                    j = pre_inter
+                                cont_overlap = False
+                            except StopIteration:
+                                cont_loop = False
 
-                    elif s > b[j]:
-                        if j == last_j:
-                            cont_loop = False
+                        elif s > b[j]:
+                            if j == last_j:
+                                cont_loop = False
+                            else:
+                                j += 1
+                                cont_overlap = False
                         else:
-                            j += 1
-                            cont_overlap = False
-                    else:
-                        try:
-                            s = next(iter_a)
-                        except StopIteration:
-                            cont_loop = False
-
+                            try:
+                                s = next(iter_a)
+                            except StopIteration:
+                                cont_loop = False
+                        pbar.update(1)
             # if rm_duplicates:
             new_regions.remove_duplicates()
             # new_regions.sort()
             return new_regions
 
     def remove_duplicates(self, sort: bool = True):
         """
@@ -948,23 +956,24 @@
         from genomkit import GSequences
         if os.path.exists(FASTA_file):
             fasta = GSequences(load=FASTA_file)
         else:
             print(FASTA_file + " is not found.")
             sys.exit()
         res = GSequences(name=self.name)
-        for region in self.elements:
+        for region in tqdm(self.elements, desc="Get GSequences"):
             seq = fasta.get_sequence(name=region.sequence,
                                      start=region.start,
                                      end=region.end)
-            seq.name = region.name
-            seq.data = region.data
-            if region.orientation == "-":
-                seq.reverse_complement()
-            res.add(seq)
+            if seq:
+                seq.name = str(region)
+                seq.data = region.data
+                if region.orientation == "-":
+                    seq.reverse_complement()
+                res.add(seq)
         return res
 
     def cluster(self, max_distance):
         """Cluster the regions with a certain distance and return a new
         GRegions.
 
         :param max_distance: Maximal distance for combining
@@ -1027,34 +1036,44 @@
             if r.name in names:
                 res.add(r)
         if inplace:
             self.elements = res.elements
         else:
             return res
 
-    def filter_by_score(self, larger_than=0, smaller_than=0, inplace=False):
-        """Filter the elements by the given list of names
+    def filter_by_score(self, larger_than=None, smaller_than=None, inplace=False):
+        """Filter the elements by the given range of scores
 
         :param larger_than: Define the minimal cutoff. Any region with the
                             score larger than this value will be returned.
         :type larger_than: float
         :param smaller_than: Define the maximal cutoff. Any region with the
                             score smaller than this value will be returned.
         :type smaller_than: float
         :param inplace: Define whether this operation will be applied on the
                         same object (True) or return a new object.
         :type inplace: bool, default to True
         :return: A GRegions with filtered regions
         :rtype: GRegions
         """
         res = GRegions(name=self.name)
-        for r in self.elements:
-            if r.score > larger_than:
-                res.add(r)
-            elif r.score < smaller_than:
-                res.add(r)
-            else:
-                continue
+        if larger_than and smaller_than:
+            for r in self.elements:
+                if larger_than < r.score < smaller_than:
+                    res.add(r)
+        elif larger_than and not smaller_than:
+            for r in self.elements:
+                if r.score > larger_than:
+                    res.add(r)
+        elif not larger_than and smaller_than:
+            for r in self.elements:
+                if r.score < smaller_than:
+                    res.add(r)
         if inplace:
             self.elements = res.elements
         else:
             return res
+
+    # def rename_by_GRegions(self, name_source, strandness: bool = True,
+    #                        inplace: bool = True):
+    #     assert isinstance(name_source, GRegions)
+
```

### Comparing `genomkit-0.2.6/genomkit/regions/util.py` & `genomkit-0.2.8/genomkit/regions/util.py`

 * *Files identical despite different names*

### Comparing `genomkit-0.2.6/genomkit/sequences/gsequence.py` & `genomkit-0.2.8/genomkit/sequences/gsequence.py`

 * *Files identical despite different names*

### Comparing `genomkit-0.2.6/genomkit/sequences/gsequences.py` & `genomkit-0.2.8/genomkit/sequences/gsequences.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,13 +126,13 @@
         :rtype: GSequence
         """
         for seq in self.elements:
             if seq.name == name:
                 return seq.slice_sequence(start, end)
 
     def write_FASTA(self, filename: str, data: bool = False,
-                    gz: bool = True):
+                    gz: bool = False):
         write_FASTA(seqs=self, filename=filename, data=data, gz=gz)
 
     def write_FASTQ(self, filename: str, data: bool = False,
                     gz: bool = True):
         write_FASTQ(seqs=self, filename=filename, data=data, gz=gz)
```

### Comparing `genomkit-0.2.6/genomkit/sequences/io.py` & `genomkit-0.2.8/genomkit/sequences/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from tqdm import tqdm
 import gzip
+import re
 
 
 ###########################################################################
 # IO functions
 ###########################################################################
 def load_FASTA(file):
     if isinstance(file, str):  # If file is a filename
@@ -16,39 +17,39 @@
 def load_FASTA_from_file(file):
     from genomkit import GSequence, GSequences
     res = GSequences()
     current_sequence_id = None
     current_sequence = ""
     total_lines = sum(1 for line in file if not line.startswith("#"))
     file.seek(0)  # Reset file pointer to the beginning
-    with tqdm(total=total_lines) as pbar:
+    with tqdm(total=total_lines, desc="Load FASTA") as pbar:
         for line in file:
             line = line.strip()
             if line.startswith("#"):
                 continue
             elif line.startswith(">"):
                 # If there was a previously stored sequence, store it
                 if current_sequence_id is not None:
-                    infos = current_sequence_id.split()
-                    name = infos[0]
+                    infos = re.split(r'[ |;,-]', current_sequence_id)
+                    name = infos[0].split(".")[0]
                     data = infos[1:]
                     res.add(GSequence(sequence=current_sequence,
                                       name=name, data=data))
                 # Extract the sequence ID
                 current_sequence_id = line[1:]
                 # Start a new sequence
                 current_sequence = ""
             else:  # Sequence line
                 # Append the sequence line to the current sequence
                 current_sequence += line
             pbar.update(1)
         # Store the last sequence
         if current_sequence_id is not None:
-            infos = current_sequence_id.split()
-            name = infos[0]
+            infos = re.split(r'[ |;,-]', current_sequence_id)
+            name = infos[0].split(".")[0]
             data = infos[1:]
             res.add(GSequence(sequence=current_sequence,
                               name=name, data=data))
     return res
 
 
 def load_FASTQ(file):
@@ -64,15 +65,15 @@
     res = GSequences()
     current_sequence_id = None
     current_sequence = ""
     current_quality = ""
     total_records = sum(1 for _ in file) // 4  # Calculate total records
     file.seek(0)  # Reset file pointer to the beginning
 
-    with tqdm(total=total_records) as pbar:
+    with tqdm(total=total_records, desc="Load FASTQ") as pbar:
         for line_num, line in enumerate(file):
             line = line.strip()
             if line.startswith("#"):
                 continue
             elif line_num % 4 == 0:  # Sequence header line
                 # If there was a previously stored sequence, store it
                 if current_sequence_id is not None:
@@ -101,15 +102,15 @@
                               quality=current_quality,
                               name=current_sequence_id))
             pbar.update(1)  # Update progress bar
     return res
 
 
 def write_FASTA(seqs, filename: str, data: bool = False,
-                gz: bool = True):
+                gz: bool = False):
     if gz:
         with gzip.open(filename, "wt") as fasta_file:
             write_fasta_content(seqs, fasta_file, data)
     else:
         with open(filename, "w") as fasta_file:
             write_fasta_content(seqs, fasta_file, data)
```

### Comparing `genomkit-0.2.6/genomkit/variants/gvariant.py` & `genomkit-0.2.8/genomkit/variants/gvariant.py`

 * *Files identical despite different names*

### Comparing `genomkit-0.2.6/genomkit/variants/gvariants.py` & `genomkit-0.2.8/genomkit/variants/gvariants.py`

 * *Files identical despite different names*

### Comparing `genomkit-0.2.6/genomkit.egg-info/PKG-INFO` & `genomkit-0.2.8/genomkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomkit
-Version: 0.2.6
+Version: 0.2.8
 Summary: genomkit
 Home-page: https://github.com/chaochungkuo/genomkit
 Author: Chao-Chung Kuo
 Author-email: chao-chung.kuo@rwth-aachen.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `genomkit-0.2.6/genomkit.egg-info/SOURCES.txt` & `genomkit-0.2.8/genomkit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 genomkit.egg-info/top_level.txt
 genomkit/alignments/__init__.py
 genomkit/alignments/galignments.py
 genomkit/annotation/__init__.py
 genomkit/annotation/gannotation.py
 genomkit/coverages/__init__.py
 genomkit/coverages/gcoverages.py
+genomkit/coverages/gcoverages_set.py
 genomkit/data/chrom_size/chrom.sizes.hg19
 genomkit/data/chrom_size/chrom.sizes.hg38
 genomkit/data/chrom_size/chrom.sizes.mm10
 genomkit/data/chrom_size/chrom.sizes.mm39
 genomkit/data/chrom_size/chrom.sizes.mm9
 genomkit/data/chrom_size/chrom.sizes.tair10
 genomkit/data/chrom_size/chrom.sizes.zv10
 genomkit/data/chrom_size/chrom.sizes.zv9
 genomkit/regions/__init__.py
 genomkit/regions/gregion.py
 genomkit/regions/gregions.py
+genomkit/regions/gregions_intervaltree.py
 genomkit/regions/gregions_set.py
 genomkit/regions/io.py
 genomkit/regions/util.py
 genomkit/sequences/__init__.py
 genomkit/sequences/gsequence.py
 genomkit/sequences/gsequences.py
 genomkit/sequences/io.py
@@ -36,9 +38,10 @@
 genomkit/variants/gvariant.py
 genomkit/variants/gvariants.py
 tests/__init__.py
 tests/test_gannotation.py
 tests/test_gcoverages.py
 tests/test_gregion.py
 tests/test_gregions.py
+tests/test_gregionstree.py
 tests/test_gsequence.py
 tests/test_gsequences.py
```

### Comparing `genomkit-0.2.6/setup.py` & `genomkit-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `genomkit-0.2.6/tests/test_gannotation.py` & `genomkit-0.2.8/tests/test_gannotation.py`

 * *Files identical despite different names*

### Comparing `genomkit-0.2.6/tests/test_gregion.py` & `genomkit-0.2.8/tests/test_gregion.py`

 * *Files identical despite different names*

### Comparing `genomkit-0.2.6/tests/test_gregions.py` & `genomkit-0.2.8/tests/test_gregions.py`

 * *Files identical despite different names*

### Comparing `genomkit-0.2.6/tests/test_gsequence.py` & `genomkit-0.2.8/tests/test_gsequence.py`

 * *Files identical despite different names*

### Comparing `genomkit-0.2.6/tests/test_gsequences.py` & `genomkit-0.2.8/tests/test_gsequences.py`

 * *Files identical despite different names*

