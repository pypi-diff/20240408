# Comparing `tmp/nanomonsv-0.7.1.tar.gz` & `tmp/nanomonsv-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomonsv-0.7.1.tar", last modified: Fri Jul 28 08:53:56 2023, max compression
+gzip compressed data, was "nanomonsv-0.7.2.tar", last modified: Mon Apr  8 05:31:17 2024, max compression
```

## Comparing `nanomonsv-0.7.1.tar` & `nanomonsv-0.7.2.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:53:56.663528 nanomonsv-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16016 2023-07-28 08:53:56.663528 nanomonsv-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:53:56.663528 nanomonsv-0.7.1/nanomonsv/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20822 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/cluster_sbnd.py
--rw-r--r--   0 runner    (1001) docker     (123)    21130 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/count_sread_by_alignment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:53:56.663528 nanomonsv-0.7.1/nanomonsv/data/
--rw-r--r--   0 runner    (1001) docker     (123)   147053 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/data/LINE1.hg19.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)    79292 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/data/LINE1.hg19.bed.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (123)   152156 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/data/LINE1.hg38.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)    82867 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/data/LINE1.hg38.bed.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/filt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/gather_support_read_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/generate_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/insert_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/locate_bp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/locate_bp_sbnd.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/long_read_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/merge_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/my_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/post_proc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15065 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/pyssw.py
--rw-r--r--   0 runner    (1001) docker     (123)    30170 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/smith_waterman.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/ssw_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/swalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/vcf_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:53:56.663528 nanomonsv-0.7.1/nanomonsv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16016 2023-07-28 08:53:56.000000 nanomonsv-0.7.1/nanomonsv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-28 08:53:56.000000 nanomonsv-0.7.1/nanomonsv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:53:56.000000 nanomonsv-0.7.1/nanomonsv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-28 08:53:56.000000 nanomonsv-0.7.1/nanomonsv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 08:53:56.000000 nanomonsv-0.7.1/nanomonsv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:53:56.663528 nanomonsv-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-08 05:31:17.544110 nanomonsv-0.7.2/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    35149 2023-06-11 06:57:47.000000 nanomonsv-0.7.2/LICENSE
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16016 2024-04-08 05:31:17.544110 nanomonsv-0.7.2/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    15220 2023-07-25 05:43:13.000000 nanomonsv-0.7.2/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-08 05:31:17.540110 nanomonsv-0.7.2/nanomonsv/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      253 2023-06-11 06:57:47.000000 nanomonsv-0.7.2/nanomonsv/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12071 2023-07-25 06:01:27.000000 nanomonsv-0.7.2/nanomonsv/arg_parser.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    20822 2024-04-04 12:08:31.000000 nanomonsv-0.7.2/nanomonsv/cluster.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8408 2023-07-25 06:01:27.000000 nanomonsv-0.7.2/nanomonsv/cluster_sbnd.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    21202 2024-04-06 03:39:05.000000 nanomonsv-0.7.2/nanomonsv/count_sread_by_alignment.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-08 05:31:17.540110 nanomonsv-0.7.2/nanomonsv/data/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       28 2024-04-06 11:38:35.000000 nanomonsv-0.7.2/nanomonsv/data/LINE1.hg19.bed.gz
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       75 2024-04-06 11:38:35.000000 nanomonsv-0.7.2/nanomonsv/data/LINE1.hg19.bed.gz.tbi
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    85507 2024-04-06 11:38:35.000000 nanomonsv-0.7.2/nanomonsv/data/LINE1.hg38.bed.gz
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    57599 2024-04-06 11:38:35.000000 nanomonsv-0.7.2/nanomonsv/data/LINE1.hg38.bed.gz.tbi
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    18301 2023-06-11 06:57:47.000000 nanomonsv-0.7.2/nanomonsv/filt.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7318 2023-07-25 06:01:27.000000 nanomonsv-0.7.2/nanomonsv/gather_support_read_seq.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16271 2023-06-23 07:20:25.000000 nanomonsv-0.7.2/nanomonsv/generate_consensus.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    27769 2023-06-11 06:57:47.000000 nanomonsv-0.7.2/nanomonsv/insert_classify.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4731 2024-04-06 03:39:05.000000 nanomonsv-0.7.2/nanomonsv/locate_bp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2428 2024-04-06 03:39:05.000000 nanomonsv-0.7.2/nanomonsv/locate_bp_sbnd.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      453 2023-06-11 06:57:47.000000 nanomonsv-0.7.2/nanomonsv/logger.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    23057 2023-06-11 06:57:47.000000 nanomonsv-0.7.2/nanomonsv/long_read_validate.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6921 2023-06-11 06:57:47.000000 nanomonsv-0.7.2/nanomonsv/merge_control.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      755 2023-06-11 06:57:47.000000 nanomonsv-0.7.2/nanomonsv/my_seq.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13405 2023-07-25 06:01:27.000000 nanomonsv-0.7.2/nanomonsv/parse.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16213 2024-04-06 03:39:05.000000 nanomonsv-0.7.2/nanomonsv/post_proc.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)    15065 2023-06-11 06:57:47.000000 nanomonsv-0.7.2/nanomonsv/pyssw.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    30170 2023-07-28 00:49:08.000000 nanomonsv-0.7.2/nanomonsv/run.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6709 2023-07-28 08:26:00.000000 nanomonsv-0.7.2/nanomonsv/smith_waterman.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11992 2023-06-11 06:57:47.000000 nanomonsv-0.7.2/nanomonsv/ssw_lib.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19609 2023-06-11 06:57:47.000000 nanomonsv-0.7.2/nanomonsv/swalign.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3690 2023-06-23 07:20:25.000000 nanomonsv-0.7.2/nanomonsv/utils.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7571 2023-06-11 06:57:47.000000 nanomonsv-0.7.2/nanomonsv/vcf_convert.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       48 2024-04-06 03:40:35.000000 nanomonsv-0.7.2/nanomonsv/version.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-08 05:31:17.544110 nanomonsv-0.7.2/nanomonsv.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16016 2024-04-08 05:31:17.000000 nanomonsv-0.7.2/nanomonsv.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      963 2024-04-08 05:31:17.000000 nanomonsv-0.7.2/nanomonsv.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-08 05:31:17.000000 nanomonsv-0.7.2/nanomonsv.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       45 2024-04-08 05:31:17.000000 nanomonsv-0.7.2/nanomonsv.egg-info/entry_points.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       10 2024-04-08 05:31:17.000000 nanomonsv-0.7.2/nanomonsv.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-08 05:31:17.544110 nanomonsv-0.7.2/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1704 2023-06-14 03:46:54.000000 nanomonsv-0.7.2/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-08 05:31:17.544110 nanomonsv-0.7.2/tests/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      268 2024-04-06 03:39:05.000000 nanomonsv-0.7.2/tests/test_main.py
```

### Comparing `nanomonsv-0.7.1/LICENSE` & `nanomonsv-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/PKG-INFO` & `nanomonsv-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomonsv
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python tools for detecting structural variation from nanopore sequence data
 Home-page: https://github.com/friend1ws/nanomonsv
 Author: Yuichi Shiraishi
 Author-email: friend1ws@gamil.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `nanomonsv-0.7.1/README.md` & `nanomonsv-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/arg_parser.py` & `nanomonsv-0.7.2/nanomonsv/arg_parser.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/cluster.py` & `nanomonsv-0.7.2/nanomonsv/cluster.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/cluster_sbnd.py` & `nanomonsv-0.7.2/nanomonsv/cluster_sbnd.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/count_sread_by_alignment.py` & `nanomonsv-0.7.2/nanomonsv/count_sread_by_alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,57 +232,57 @@
     def generate_segment_fasta_files(self):
 
         tchr1, tpos1, tdir1, tchr2, tpos2, tdir2, tinseq, tid = self.temp_key.split(',')
         tpos1, tpos2 = int(tpos1), int(tpos2)
         tinseq = '' if tinseq == "---" else tinseq
 
         # reference_local_seq
-        self.reference_segment_1 = self.reference_fasta_h.fetch(tchr1, max(tpos1 - self.validate_sequence_length - 1, 0), tpos1 + self.validate_sequence_length - 1)
-        self.reference_segment_2 = self.reference_fasta_h.fetch(tchr2, max(tpos2 - self.validate_sequence_length - 1, 0), tpos2 + self.validate_sequence_length - 1)
+        self.reference_segment_1 = self.reference_fasta_h.fetch(tchr1, max(tpos1 - self.validate_sequence_length - 1, 0), tpos1 + self.validate_sequence_length - 1).upper()
+        self.reference_segment_2 = self.reference_fasta_h.fetch(tchr2, max(tpos2 - self.validate_sequence_length - 1, 0), tpos2 + self.validate_sequence_length - 1).upper()
 
         # variant_seq
         variant_seq = ""
         if tdir1 == '+':
-            tseq = self.reference_fasta_h.fetch(tchr1, max(tpos1 - self.validate_sequence_length - 1, 0), tpos1 - 1)
+            tseq = self.reference_fasta_h.fetch(tchr1, max(tpos1 - self.validate_sequence_length - 1, 0), tpos1 - 1).upper()
         else:
-            tseq = self.reference_fasta_h.fetch(tchr1, tpos1 - 1, tpos1 + self.validate_sequence_length - 1)
+            tseq = self.reference_fasta_h.fetch(tchr1, tpos1 - 1, tpos1 + self.validate_sequence_length - 1).upper()
             tseq = reverse_complement(tseq)
 
         if tdir1 == "+":
             variant_seq = tseq + tinseq
         else:
             variant_seq = tseq + reverse_complement(tinseq)
 
         if tdir2 == '-':
-            tseq = self.reference_fasta_h.fetch(tchr2, tpos2 - 1, tpos2 + self.validate_sequence_length - 1)
+            tseq = self.reference_fasta_h.fetch(tchr2, tpos2 - 1, tpos2 + self.validate_sequence_length - 1).upper()
         else:
-            tseq = self.reference_fasta_h.fetch(tchr2, max(tpos2 - self.validate_sequence_length - 1, 0), tpos2 - 1)
+            tseq = self.reference_fasta_h.fetch(tchr2, max(tpos2 - self.validate_sequence_length - 1, 0), tpos2 - 1).upper()
             tseq = reverse_complement(tseq)
 
         variant_seq = variant_seq + tseq
 
         self.variant_segment_1 = variant_seq[:min(2 * self.validate_sequence_length, len(variant_seq))]
         self.variant_segment_2 = variant_seq[-min(2 * self.validate_sequence_length, len(variant_seq)):]
 
 
     def generate_segment_fasta_files_sbnd(self):
 
         tchr, tpos, tdir, tcontig, tid = self.temp_key.split(',')
         tpos = int(tpos)
 
         # referene_local_seq
-        self.reference_segment_1 = self.reference_fasta_h.fetch(tchr, max(tpos - self.validate_sequence_length - 1, 0), tpos + self.validate_sequence_length - 1)
+        self.reference_segment_1 = self.reference_fasta_h.fetch(tchr, max(tpos - self.validate_sequence_length - 1, 0), tpos + self.validate_sequence_length - 1).upper()
 
         # variant_seq
         variant_seq = ''
         if tdir == '+':
-            tseq = self.reference_fasta_h.fetch(tchr, max(tpos - self.validate_sequence_length - 1, 0), tpos)
+            tseq = self.reference_fasta_h.fetch(tchr, max(tpos - self.validate_sequence_length - 1, 0), tpos).upper()
             tseq = tseq + tcontig
         else:
-            tseq = self.reference_fasta_h.fetch(tchr, tpos - 1, tpos + self.validate_sequence_length - 1)
+            tseq = self.reference_fasta_h.fetch(tchr, tpos - 1, tpos + self.validate_sequence_length - 1).upper()
             tseq = reverse_complement(tseq)
         self.variant_segment_1 = tseq + tcontig
 
 
     def add_long_read_seq(self, treadid, tseq, tmapq1, tmapq2):
 
         self.readid2mapq[treadid] = [int(tmapq1) if tmapq1 != "None" else None, int(tmapq2) if tmapq2 != "None" else None]
```

### Comparing `nanomonsv-0.7.1/nanomonsv/filt.py` & `nanomonsv-0.7.2/nanomonsv/filt.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/gather_support_read_seq.py` & `nanomonsv-0.7.2/nanomonsv/gather_support_read_seq.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/generate_consensus.py` & `nanomonsv-0.7.2/nanomonsv/generate_consensus.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/insert_classify.py` & `nanomonsv-0.7.2/nanomonsv/insert_classify.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/locate_bp.py` & `nanomonsv-0.7.2/nanomonsv/locate_bp.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 
         bstart1, bend1 = max(int(start1) - rd_margin, 1), int(end1) + rd_margin
         bstart2, bend2 = max(int(start2) - rd_margin, 1), int(end2) + rd_margin
 
         if ref_len1 < bend1: bend1 = ref_len1
         if ref_len2 < bend2: bend2 = ref_len2    
 
-        region1_seq = fasta_file_ins.fetch(chr1, bstart1 - 1, bend1)
-        region2_seq = fasta_file_ins.fetch(chr2, bstart2 - 1, bend2)
+        region1_seq = fasta_file_ins.fetch(chr1, bstart1 - 1, bend1).upper()
+        region2_seq = fasta_file_ins.fetch(chr2, bstart2 - 1, bend2).upper()
+        
 
         if dir1 == '-': region1_seq = reverse_complement(region1_seq)
         if dir2 == '+': region2_seq = reverse_complement(region2_seq)
 
         sret = smith_waterman.sw_jump(contig, region1_seq, region2_seq,
                                       match_score = sw_jump_params[0], mismatch_penalty = sw_jump_params[1],
                                       gap_cost = sw_jump_params[2], jump_cost = sw_jump_params[3])
@@ -58,15 +59,15 @@
         return(bp_pos1, bp_pos2, inseq)
     
     else:
     
         contig_start = contig[:min(i_margin, len(contig))]
         contig_end = contig[-min(i_margin, len(contig)):]
 
-        region_seq = fasta_file_ins.fetch(chr1, max(0, start1 - 100), end2 + 100)
+        region_seq = fasta_file_ins.fetch(chr1, max(0, start1 - 100), end2 + 100).upper()
         sret = smith_waterman.sw_jump(region_seq, contig_start, contig_end,
                                       match_score = sw_jump_params[0], mismatch_penalty = sw_jump_params[1], 
                                       gap_cost = sw_jump_params[2], jump_cost = sw_jump_params[3])
 
         if sret is None: return(None)
         score, region_align, contig_start_align, contig_end_align, region_seq, contig_seq = sret
```

### Comparing `nanomonsv-0.7.1/nanomonsv/locate_bp_sbnd.py` & `nanomonsv-0.7.2/nanomonsv/locate_bp_sbnd.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 from .my_seq import reverse_complement
 
 from .logger import get_logger
 
 logger = get_logger(__name__)
 
-       
+
 def get_refined_bp_sbnd(tconsensus, fasta_file_h, tchr, tstart, tend, tdir, hout_log, margin = 200):
 
     tconsensus_part = tconsensus[:1000] if len(tconsensus) > 1000 else tconsensus
 
     ref_len = fasta_file_h.get_reference_length(tchr)
     if tstart < 1: tstart = 1
     if ref_len < tend: tend = ref_len 
 
     if tdir == '+':
-        qseq = fasta_file_h.fetch(tchr, max(int(tstart) - margin, 0), int(tend))
+        qseq = fasta_file_h.fetch(tchr, max(int(tstart) - margin, 0), int(tend)).upper()
     else:
-        qseq = fasta_file_h.fetch(tchr, max(int(tstart) - 1, 0), int(tend) + margin)
+        qseq = fasta_file_h.fetch(tchr, max(int(tstart) - 1, 0), int(tend) + margin).upper()
         qseq = reverse_complement(qseq)
 
     user_matrix = parasail.matrix_create("ACGT", 1, -2)
     res = parasail.ssw(qseq, tconsensus, 3, 1, user_matrix)
     if res is None:
         logger.debug(f"Alignment for breakpoint localization failed for {tchr},{tstart},{tend},{tdir}")
         return None
@@ -37,15 +37,15 @@
     else:
         bp_pos_reference = tstart + (len(qseq) - res.read_end1 - 1) 
 
     tconsensus_after = tconsensus[(res.ref_end1 + 1):]
 
     return (bp_pos_reference, tconsensus_after)
 
- 
+
 def locate_bp_sbnd(consensus_file, output_file, reference_fasta, debug):
 
     fasta_file_ins = pysam.FastaFile(reference_fasta)
 
     with open(consensus_file, 'r') as hin, open(output_file, 'w') as hout, \
         open(output_file + ".locate_bp.sbnd.log", 'w') as hout_log:
         for line in hin:
```

### Comparing `nanomonsv-0.7.1/nanomonsv/long_read_validate.py` & `nanomonsv-0.7.2/nanomonsv/long_read_validate.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/merge_control.py` & `nanomonsv-0.7.2/nanomonsv/merge_control.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/my_seq.py` & `nanomonsv-0.7.2/nanomonsv/my_seq.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/parse.py` & `nanomonsv-0.7.2/nanomonsv/parse.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/post_proc.py` & `nanomonsv-0.7.2/nanomonsv/post_proc.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,33 +87,33 @@
         # only apply when the first sv is not insertion and the second sv is insertion type
         if len(sv.inseq) >= self.min_indel_size or len(ins.inseq) < self.min_indel_size: return 
 
         if not (sv.chr1 == ins.chr1 and abs(sv.pos1 - ins.pos1) <= self.bp_dist_margin) and \
             not (sv.chr2 == ins.chr2 and abs(sv.pos2 - ins.pos2) <= self.bp_dist_margin):
             return 
 
-        ins_seg = self.reference_h.fetch(ins.chr1, max(ins.pos1 - self.validate_seg_len - self.bp_dist_margin - 1, 0), ins.pos1 - 1)
+        ins_seg = self.reference_h.fetch(ins.chr1, max(ins.pos1 - self.validate_seg_len - self.bp_dist_margin - 1, 0), ins.pos1 - 1).upper()
         ins_seg = ins_seg + ins.inseq
-        ins_seg = ins_seg + self.reference_h.fetch(ins.chr1, ins.pos2 - 1, ins.pos2 + self.validate_seg_len + self.bp_dist_margin - 1)
+        ins_seg = ins_seg + self.reference_h.fetch(ins.chr1, ins.pos2 - 1, ins.pos2 + self.validate_seg_len + self.bp_dist_margin - 1).upper()
 
         if sv.dir1 == '+':
-            tseq = self.reference_h.fetch(sv.chr1, max(sv.pos1 - self.validate_seg_len - 1, 0), sv.pos1 - 1)
+            tseq = self.reference_h.fetch(sv.chr1, max(sv.pos1 - self.validate_seg_len - 1, 0), sv.pos1 - 1).upper()
         else:
-            tseq = self.reference_h.fetch(sv.chr1, sv.pos1 - 1, sv.pos1 + self.validate_seg_len - 1) 
+            tseq = self.reference_h.fetch(sv.chr1, sv.pos1 - 1, sv.pos1 + self.validate_seg_len - 1).upper()
             tseq = reverse_complement(tseq)
 
         if sv.dir1 == '+':
             sv_seg = tseq + sv.inseq
         else:
             sv_seg = tseq + reverse_complement(sv.inseq)
 
         if sv.dir2 == '-':
-            tseq = self.reference_h.fetch(sv.chr2, sv.pos2 - 1, sv.pos2 + self.validate_seg_len - 1)
+            tseq = self.reference_h.fetch(sv.chr2, sv.pos2 - 1, sv.pos2 + self.validate_seg_len - 1).upper()
         else:
-            tseq = self.reference_h.fetch(sv.chr2, max(sv.pos2 - self.validate_seg_len - 1, 0), sv.pos2 - 1)
+            tseq = self.reference_h.fetch(sv.chr2, max(sv.pos2 - self.validate_seg_len - 1, 0), sv.pos2 - 1).upper()
             tseq = reverse_complement(tseq)
  
         sv_seg = sv_seg + tseq
 
         user_matrix = parasail.matrix_create("ACGT", 2, -2)
         res = parasail.ssw(sv_seg, ins_seg, 3, 1, user_matrix)
         res_r = parasail.ssw(reverse_complement(sv_seg), ins_seg, 3, 1, user_matrix)
```

### Comparing `nanomonsv-0.7.1/nanomonsv/pyssw.py` & `nanomonsv-0.7.2/nanomonsv/pyssw.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/run.py` & `nanomonsv-0.7.2/nanomonsv/run.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/smith_waterman.py` & `nanomonsv-0.7.2/nanomonsv/smith_waterman.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/ssw_lib.py` & `nanomonsv-0.7.2/nanomonsv/ssw_lib.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/swalign.py` & `nanomonsv-0.7.2/nanomonsv/swalign.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/utils.py` & `nanomonsv-0.7.2/nanomonsv/utils.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv/vcf_convert.py` & `nanomonsv-0.7.2/nanomonsv/vcf_convert.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.1/nanomonsv.egg-info/PKG-INFO` & `nanomonsv-0.7.2/nanomonsv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomonsv
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python tools for detecting structural variation from nanopore sequence data
 Home-page: https://github.com/friend1ws/nanomonsv
 Author: Yuichi Shiraishi
 Author-email: friend1ws@gamil.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `nanomonsv-0.7.1/nanomonsv.egg-info/SOURCES.txt` & `nanomonsv-0.7.2/nanomonsv.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,8 +30,9 @@
 nanomonsv.egg-info/SOURCES.txt
 nanomonsv.egg-info/dependency_links.txt
 nanomonsv.egg-info/entry_points.txt
 nanomonsv.egg-info/top_level.txt
 nanomonsv/data/LINE1.hg19.bed.gz
 nanomonsv/data/LINE1.hg19.bed.gz.tbi
 nanomonsv/data/LINE1.hg38.bed.gz
-nanomonsv/data/LINE1.hg38.bed.gz.tbi
+nanomonsv/data/LINE1.hg38.bed.gz.tbi
+tests/test_main.py
```

### Comparing `nanomonsv-0.7.1/setup.py` & `nanomonsv-0.7.2/setup.py`

 * *Files identical despite different names*

