# Comparing `tmp/checkQC-4.0.1.tar.gz` & `tmp/checkQC-4.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkQC-4.0.1.tar", last modified: Mon Mar 18 14:16:33 2024, max compression
+gzip compressed data, was "checkQC-4.0.2rc1.tar", last modified: Mon Apr  8 12:13:00 2024, max compression
```

## Comparing `checkQC-4.0.1.tar` & `checkQC-4.0.2rc1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2024-03-18 14:16:32.999577 checkQC-4.0.1/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)    35141 2022-03-09 14:47:52.000000 checkQC-4.0.1/LICENSE
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      146 2022-03-09 14:47:52.000000 checkQC-4.0.1/MANIFEST.in
--rw-r--r--   0 matilda   (1000) matilda   (1000)      717 2024-03-18 14:16:32.999577 checkQC-4.0.1/PKG-INFO
--rw-rw-r--   0 matilda   (1000) matilda   (1000)    11317 2024-03-18 13:58:41.000000 checkQC-4.0.1/README.md
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2024-03-18 14:16:32.995577 checkQC-4.0.1/checkQC/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)       23 2024-03-18 14:14:45.000000 checkQC-4.0.1/checkQC/__init__.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     5028 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/app.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     9538 2023-10-18 13:32:19.000000 checkQC-4.0.1/checkQC/config.py
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2024-03-18 14:16:32.995577 checkQC-4.0.1/checkQC/default_config/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)    14396 2023-10-18 17:44:32.000000 checkQC-4.0.1/checkQC/default_config/config.yaml
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      576 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/default_config/logger.yaml
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      836 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/exceptions.py
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2024-03-18 14:16:32.999577 checkQC-4.0.1/checkQC/handlers/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)        0 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/handlers/__init__.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1857 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/handlers/cluster_pf_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3646 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/handlers/error_rate_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     2240 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/handlers/q30_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     7911 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/handlers/qc_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1545 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/handlers/qc_handler_factory.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3248 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/handlers/reads_per_sample_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     4146 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/handlers/undetermined_percentage_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)    15676 2023-10-18 17:44:32.000000 checkQC-4.0.1/checkQC/handlers/unidentified_index_handler.py
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2024-03-18 14:16:32.999577 checkQC-4.0.1/checkQC/parsers/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)        0 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/parsers/__init__.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3958 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/parsers/demux_summary_parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3532 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/parsers/interop_parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     2245 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/parsers/parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     2098 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/parsers/samplesheet_parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3189 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/parsers/stats_json_parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     4378 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/qc_engine.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     8137 2024-03-18 13:58:41.000000 checkQC-4.0.1/checkQC/run_type_recognizer.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1498 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/run_type_summarizer.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     2937 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/runfolder_reader.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     4221 2022-03-09 14:47:52.000000 checkQC-4.0.1/checkQC/web_app.py
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2024-03-18 14:16:32.999577 checkQC-4.0.1/checkQC.egg-info/
--rw-r--r--   0 matilda   (1000) matilda   (1000)      717 2024-03-18 14:16:32.000000 checkQC-4.0.1/checkQC.egg-info/PKG-INFO
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1067 2024-03-18 14:16:32.000000 checkQC-4.0.1/checkQC.egg-info/SOURCES.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)        1 2024-03-18 14:16:32.000000 checkQC-4.0.1/checkQC.egg-info/dependency_links.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)       81 2024-03-18 14:16:32.000000 checkQC-4.0.1/checkQC.egg-info/entry_points.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)       64 2024-03-18 14:16:32.000000 checkQC-4.0.1/checkQC.egg-info/requires.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)        8 2024-03-18 14:16:32.000000 checkQC-4.0.1/checkQC.egg-info/top_level.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)       79 2024-03-18 14:16:32.999577 checkQC-4.0.1/setup.cfg
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1215 2024-03-18 13:58:41.000000 checkQC-4.0.1/setup.py
+drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2024-04-08 12:13:00.739457 checkQC-4.0.2rc1/
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)    35141 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/LICENSE
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)      146 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/MANIFEST.in
+-rw-r--r--   0 matilda   (1000) matilda   (1000)      724 2024-04-08 12:13:00.739457 checkQC-4.0.2rc1/PKG-INFO
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)    11317 2024-04-08 12:11:29.000000 checkQC-4.0.2rc1/README.md
+drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2024-04-08 12:13:00.735457 checkQC-4.0.2rc1/checkQC/
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)       27 2024-04-08 12:11:29.000000 checkQC-4.0.2rc1/checkQC/__init__.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     5028 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/app.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     9538 2023-10-18 13:32:19.000000 checkQC-4.0.2rc1/checkQC/config.py
+drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2024-04-08 12:13:00.735457 checkQC-4.0.2rc1/checkQC/default_config/
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)    14396 2023-10-18 17:44:32.000000 checkQC-4.0.2rc1/checkQC/default_config/config.yaml
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)      576 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/default_config/logger.yaml
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)      836 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/exceptions.py
+drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2024-04-08 12:13:00.739457 checkQC-4.0.2rc1/checkQC/handlers/
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)        0 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/handlers/__init__.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     1857 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/handlers/cluster_pf_handler.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     3646 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/handlers/error_rate_handler.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     2743 2024-04-08 12:11:29.000000 checkQC-4.0.2rc1/checkQC/handlers/q30_handler.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     7911 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/handlers/qc_handler.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     1545 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/handlers/qc_handler_factory.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     3248 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/handlers/reads_per_sample_handler.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     4146 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/handlers/undetermined_percentage_handler.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)    15676 2023-10-18 17:44:32.000000 checkQC-4.0.2rc1/checkQC/handlers/unidentified_index_handler.py
+drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2024-04-08 12:13:00.739457 checkQC-4.0.2rc1/checkQC/parsers/
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)        0 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/parsers/__init__.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     3958 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/parsers/demux_summary_parser.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     3555 2024-04-08 12:11:29.000000 checkQC-4.0.2rc1/checkQC/parsers/interop_parser.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     2245 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/parsers/parser.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     2098 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/parsers/samplesheet_parser.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     3189 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/parsers/stats_json_parser.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     4378 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/qc_engine.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     8137 2024-04-08 12:11:29.000000 checkQC-4.0.2rc1/checkQC/run_type_recognizer.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     1498 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/run_type_summarizer.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     2937 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/runfolder_reader.py
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     4221 2022-03-09 14:47:52.000000 checkQC-4.0.2rc1/checkQC/web_app.py
+drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2024-04-08 12:13:00.739457 checkQC-4.0.2rc1/checkQC.egg-info/
+-rw-r--r--   0 matilda   (1000) matilda   (1000)      724 2024-04-08 12:13:00.000000 checkQC-4.0.2rc1/checkQC.egg-info/PKG-INFO
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     1067 2024-04-08 12:13:00.000000 checkQC-4.0.2rc1/checkQC.egg-info/SOURCES.txt
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)        1 2024-04-08 12:13:00.000000 checkQC-4.0.2rc1/checkQC.egg-info/dependency_links.txt
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)       81 2024-04-08 12:13:00.000000 checkQC-4.0.2rc1/checkQC.egg-info/entry_points.txt
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)       64 2024-04-08 12:13:00.000000 checkQC-4.0.2rc1/checkQC.egg-info/requires.txt
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)        8 2024-04-08 12:13:00.000000 checkQC-4.0.2rc1/checkQC.egg-info/top_level.txt
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)       79 2024-04-08 12:13:00.739457 checkQC-4.0.2rc1/setup.cfg
+-rw-rw-r--   0 matilda   (1000) matilda   (1000)     1215 2024-04-08 12:11:29.000000 checkQC-4.0.2rc1/setup.py
```

### Comparing `checkQC-4.0.1/LICENSE` & `checkQC-4.0.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/PKG-INFO` & `checkQC-4.0.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: checkQC
-Version: 4.0.1
+Version: 4.0.2rc1
 Summary: A simple program to parse Illumina NGS data and check it for quality criteria.
 Home-page: https://www.github.com/Molmed/checkQC
-Download-URL: https://github.com/Molmed/checkQC/archive/4.0.1.tar.gz
+Download-URL: https://github.com/Molmed/checkQC/archive/4.0.2-rc1.tar.gz
 Author: Johan Dahlberg, SNP&SEQ Technology Platform, Uppsala University
 Author-email: johan.dahlberg@medsci.uu.se
 License: GPLv3
 Keywords: bioinformatics,ngs,quality control
 Requires-Python: >3.10, <3.11
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `checkQC-4.0.1/README.md` & `checkQC-4.0.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/app.py` & `checkQC-4.0.2rc1/checkQC/app.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/config.py` & `checkQC-4.0.2rc1/checkQC/config.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/default_config/config.yaml` & `checkQC-4.0.2rc1/checkQC/default_config/config.yaml`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/default_config/logger.yaml` & `checkQC-4.0.2rc1/checkQC/default_config/logger.yaml`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/exceptions.py` & `checkQC-4.0.2rc1/checkQC/exceptions.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/handlers/cluster_pf_handler.py` & `checkQC-4.0.2rc1/checkQC/handlers/cluster_pf_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/handlers/error_rate_handler.py` & `checkQC-4.0.2rc1/checkQC/handlers/error_rate_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/handlers/q30_handler.py` & `checkQC-4.0.2rc1/checkQC/handlers/q30_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,29 +24,55 @@
     def collect(self, signal):
         key, value = signal
         if key == "percent_q30":
             self.error_results.append(value)
 
     def check_qc(self):
 
+        index_count = 0
+        non_index_count = 0
         for error_dict in self.error_results:
             lane_nbr = int(error_dict["lane"])
-            read = error_dict["read"]
             percent_q30 = error_dict["percent_q30"]
-
+            is_index_read = error_dict.get("is_index_read", False)
+            read_or_index_text = "index read" if is_index_read else "read"
+            # Differentiate read values for indexed from non-indexed reads
+            index_count += 1 if is_index_read else 0
+            non_index_count += 1 if not is_index_read else 0
+            
+            read = index_count if is_index_read else non_index_count
+            
             if self.error() != self.UNKNOWN and percent_q30 < self.error():
-                yield QCErrorFatal("%Q30 {:.2f} was too low on lane: {} for read: {}".format(percent_q30,
-                                                                                             lane_nbr,
-                                                                                             read),
-                                   ordering=lane_nbr,
-                                   data={"lane": lane_nbr, "read": read,
-                                         "percent_q30": percent_q30, "threshold": self.error()})
+                yield QCErrorFatal(
+                    "%Q30 {:.2f} was too low on lane: {} for {}: {}".format(
+                        percent_q30,
+                        lane_nbr,
+                        read_or_index_text,
+                        read
+                    ),
+                    ordering=lane_nbr,
+                    data={
+                        "lane": lane_nbr, 
+                        "read": read,
+                        "percent_q30": percent_q30, 
+                        "threshold": self.error()
+                    }
+                )
             elif self.warning() != self.UNKNOWN and percent_q30 < self.warning():
-                yield QCErrorWarning("%Q30 {:.2f} was too low on lane: {} for read: {}".format(percent_q30,
-                                                                                               lane_nbr,
-                                                                                               read),
-                                     ordering=lane_nbr,
-                                     data={"lane": lane_nbr, "read": read,
-                                           "percent_q30": percent_q30, "threshold": self.warning()})
+                yield QCErrorWarning(
+                    "%Q30 {:.2f} was too low on lane: {} for {}: {}".format(
+                        percent_q30,
+                        lane_nbr,
+                        read_or_index_text,
+                        read
+                    ),
+                    ordering=lane_nbr,
+                    data={
+                        "lane": lane_nbr, 
+                        "read": read,
+                        "percent_q30": percent_q30, 
+                        "threshold": self.warning()
+                    }
+                )
             else:
                 continue
```

### Comparing `checkQC-4.0.1/checkQC/handlers/qc_handler.py` & `checkQC-4.0.2rc1/checkQC/handlers/qc_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/handlers/qc_handler_factory.py` & `checkQC-4.0.2rc1/checkQC/handlers/qc_handler_factory.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/handlers/reads_per_sample_handler.py` & `checkQC-4.0.2rc1/checkQC/handlers/reads_per_sample_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/handlers/undetermined_percentage_handler.py` & `checkQC-4.0.2rc1/checkQC/handlers/undetermined_percentage_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/handlers/unidentified_index_handler.py` & `checkQC-4.0.2rc1/checkQC/handlers/unidentified_index_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/parsers/demux_summary_parser.py` & `checkQC-4.0.2rc1/checkQC/parsers/demux_summary_parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/parsers/interop_parser.py` & `checkQC-4.0.2rc1/checkQC/parsers/interop_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,30 +49,33 @@
         py_interop_run_metrics.list_summary_metrics_to_load(valid_to_load)
         run_metrics.read(self.runfolder, valid_to_load)
 
         summary = py_interop_summary.run_summary()
         py_interop_summary.summarize_run_metrics(run_metrics, summary)
 
         lanes = summary.lane_count()
-        reads = self.get_non_index_reads(summary)
+
         for lane in range(lanes):
             # The interop library uses zero based indexing, however most people uses read 1/2
             # to denote the different reads, this enumeration is used to transform from
             # zero based indexing to this form. /JD 2017-10-27
-            for new_read_nbr, original_read_nbr in enumerate(reads):
-                read = summary.at(original_read_nbr).at(lane)
+            for read_nbr in range(summary.size()):
+                read = summary.at(read_nbr).at(lane)
                 error_rate = read.error_rate().mean()
                 percent_q30 = read.percent_gt_q30()
                 percent_phix_aligned = read.percent_aligned().mean()
+                is_index_read = summary.at(read_nbr).read().is_index()
+                
                 self._send_to_subscribers(("error_rate",
-                                           {"lane": lane+1, "read": new_read_nbr+1, "error_rate": error_rate}))
+                                        {"lane": lane+1, "read": read_nbr+1, "error_rate": error_rate}))
                 self._send_to_subscribers(("percent_q30",
-                                           {"lane": lane+1, "read": new_read_nbr+1, "percent_q30": percent_q30}))
+                                        {"lane": lane+1, "read": read_nbr+1, "percent_q30": percent_q30, "is_index_read":is_index_read}))
                 self._send_to_subscribers(("percent_phix",
-                                           {"lane": lane+1, "read": new_read_nbr+1, "percent_phix": percent_phix_aligned}))
+                                        {"lane": lane+1, "read": read_nbr+1, "percent_phix": percent_phix_aligned}))
+
 
     def __eq__(self, other):
         if isinstance(other, self.__class__) and self.runfolder == other.runfolder:
             return True
         else:
             return False
```

### Comparing `checkQC-4.0.1/checkQC/parsers/parser.py` & `checkQC-4.0.2rc1/checkQC/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/parsers/samplesheet_parser.py` & `checkQC-4.0.2rc1/checkQC/parsers/samplesheet_parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/parsers/stats_json_parser.py` & `checkQC-4.0.2rc1/checkQC/parsers/stats_json_parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/qc_engine.py` & `checkQC-4.0.2rc1/checkQC/qc_engine.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/run_type_recognizer.py` & `checkQC-4.0.2rc1/checkQC/run_type_recognizer.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/run_type_summarizer.py` & `checkQC-4.0.2rc1/checkQC/run_type_summarizer.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/runfolder_reader.py` & `checkQC-4.0.2rc1/checkQC/runfolder_reader.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC/web_app.py` & `checkQC-4.0.2rc1/checkQC/web_app.py`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/checkQC.egg-info/PKG-INFO` & `checkQC-4.0.2rc1/checkQC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: checkQC
-Version: 4.0.1
+Version: 4.0.2rc1
 Summary: A simple program to parse Illumina NGS data and check it for quality criteria.
 Home-page: https://www.github.com/Molmed/checkQC
-Download-URL: https://github.com/Molmed/checkQC/archive/4.0.1.tar.gz
+Download-URL: https://github.com/Molmed/checkQC/archive/4.0.2-rc1.tar.gz
 Author: Johan Dahlberg, SNP&SEQ Technology Platform, Uppsala University
 Author-email: johan.dahlberg@medsci.uu.se
 License: GPLv3
 Keywords: bioinformatics,ngs,quality control
 Requires-Python: >3.10, <3.11
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `checkQC-4.0.1/checkQC.egg-info/SOURCES.txt` & `checkQC-4.0.2rc1/checkQC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `checkQC-4.0.1/setup.py` & `checkQC-4.0.2rc1/setup.py`

 * *Files identical despite different names*

