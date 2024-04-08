# Comparing `tmp/dhlab_toolkit-0.1.0a1.tar.gz` & `tmp/dhlab_toolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhlab_toolkit-0.1.0a1.tar", max compression
+gzip compressed data, was "dhlab_toolkit-0.2.0.tar", max compression
```

## Comparing `dhlab_toolkit-0.1.0a1.tar` & `dhlab_toolkit-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1076 2023-07-12 09:17:09.879945 dhlab_toolkit-0.1.0a1/LICENSE
--rw-r--r--   0        0        0      104 2023-08-28 10:23:55.750811 dhlab_toolkit-0.1.0a1/README.md
--rw-r--r--   0        0        0        0 2023-07-12 09:17:22.972039 dhlab_toolkit-0.1.0a1/dhlab_toolkit/__init__.py
--rw-r--r--   0        0        0      363 2023-07-12 10:58:07.132344 dhlab_toolkit-0.1.0a1/dhlab_toolkit/constants.py
--rw-r--r--   0        0        0     4261 2023-07-12 12:07:25.499254 dhlab_toolkit-0.1.0a1/dhlab_toolkit/geo_data.py
--rw-r--r--   0        0        0    15394 2023-07-12 10:21:52.601440 dhlab_toolkit-0.1.0a1/dhlab_toolkit/graph_networkx_louvain.py
--rw-r--r--   0        0        0   126476 2023-07-12 10:25:50.955327 dhlab_toolkit-0.1.0a1/dhlab_toolkit/trigram_lang_model/nno_trilangmodel.json
--rw-r--r--   0        0        0   126751 2023-07-12 10:25:50.955327 dhlab_toolkit-0.1.0a1/dhlab_toolkit/trigram_lang_model/nob_trilangmodel.json
--rw-r--r--   0        0        0       41 2023-08-29 11:07:53.491805 dhlab_toolkit-0.1.0a1/dhlab_toolkit/visualization/__init__.py
--rw-r--r--   0        0        0     1677 2023-07-12 10:28:48.548731 dhlab_toolkit-0.1.0a1/dhlab_toolkit/visualization/cloud.py
--rw-r--r--   0        0        0      286 2023-07-12 10:28:48.548731 dhlab_toolkit-0.1.0a1/dhlab_toolkit/visualization/heatmap.py
--rw-r--r--   0        0        0       54 2023-08-29 11:07:31.836015 dhlab_toolkit-0.1.0a1/dhlab_toolkit/wordbank/__init__.py
--rw-r--r--   0        0        0     2462 2023-08-29 11:02:53.454572 dhlab_toolkit-0.1.0a1/dhlab_toolkit/wordbank/api.py
--rw-r--r--   0        0        0     1959 2023-08-29 11:03:19.146348 dhlab_toolkit-0.1.0a1/dhlab_toolkit/wordbank/wordbank.py
--rw-r--r--   0        0        0      433 2023-08-29 11:15:51.870909 dhlab_toolkit-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 dhlab_toolkit-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-15 09:20:54.635045 dhlab_toolkit-0.2.0/LICENSE
+-rw-r--r--   0        0        0      104 2024-03-15 09:20:54.635045 dhlab_toolkit-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-15 09:20:54.635045 dhlab_toolkit-0.2.0/dhlab_toolkit/__init__.py
+-rw-r--r--   0        0        0      363 2024-03-15 09:20:54.635045 dhlab_toolkit-0.2.0/dhlab_toolkit/constants.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:01:41.019045 dhlab_toolkit-0.2.0/dhlab_toolkit/g2p/__init__.py
+-rw-r--r--   0        0        0     2016 2024-04-08 14:03:01.831614 dhlab_toolkit-0.2.0/dhlab_toolkit/g2p/g2p_models.py
+-rw-r--r--   0        0        0     4261 2024-03-15 09:20:54.635045 dhlab_toolkit-0.2.0/dhlab_toolkit/geo_data.py
+-rw-r--r--   0        0        0    15394 2024-03-15 09:20:54.635045 dhlab_toolkit-0.2.0/dhlab_toolkit/graph_networkx_louvain.py
+-rw-r--r--   0        0        0   126476 2024-03-15 09:20:54.639045 dhlab_toolkit-0.2.0/dhlab_toolkit/trigram_lang_model/nno_trilangmodel.json
+-rw-r--r--   0        0        0   126751 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/trigram_lang_model/nob_trilangmodel.json
+-rw-r--r--   0        0        0       41 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/visualization/__init__.py
+-rw-r--r--   0        0        0     1677 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/visualization/cloud.py
+-rw-r--r--   0        0        0      286 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/visualization/heatmap.py
+-rw-r--r--   0        0        0       54 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/wordbank/__init__.py
+-rw-r--r--   0        0        0     2462 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/wordbank/api.py
+-rw-r--r--   0        0        0     1959 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/wordbank/wordbank.py
+-rw-r--r--   0        0        0      490 2024-04-08 14:02:40.563462 dhlab_toolkit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 dhlab_toolkit-0.2.0/PKG-INFO
```

### Comparing `dhlab_toolkit-0.1.0a1/LICENSE` & `dhlab_toolkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.1.0a1/dhlab_toolkit/geo_data.py` & `dhlab_toolkit-0.2.0/dhlab_toolkit/geo_data.py`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.1.0a1/dhlab_toolkit/graph_networkx_louvain.py` & `dhlab_toolkit-0.2.0/dhlab_toolkit/graph_networkx_louvain.py`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.1.0a1/dhlab_toolkit/trigram_lang_model/nno_trilangmodel.json` & `dhlab_toolkit-0.2.0/dhlab_toolkit/trigram_lang_model/nno_trilangmodel.json`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.1.0a1/dhlab_toolkit/trigram_lang_model/nob_trilangmodel.json` & `dhlab_toolkit-0.2.0/dhlab_toolkit/trigram_lang_model/nob_trilangmodel.json`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.1.0a1/dhlab_toolkit/visualization/cloud.py` & `dhlab_toolkit-0.2.0/dhlab_toolkit/visualization/cloud.py`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.1.0a1/dhlab_toolkit/wordbank/api.py` & `dhlab_toolkit-0.2.0/dhlab_toolkit/wordbank/api.py`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.1.0a1/dhlab_toolkit/wordbank/wordbank.py` & `dhlab_toolkit-0.2.0/dhlab_toolkit/wordbank/wordbank.py`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.1.0a1/PKG-INFO` & `dhlab_toolkit-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
-Name: dhlab-toolkit
-Version: 0.1.0a1
+Name: dhlab_toolkit
+Version: 0.2.0
 Summary: 
-Author: Nasjonalbiblioteket
+Author: Nasjonalbiblioteket 
 Author-email: dhlab@nb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: google-cloud-storage (>=2.16.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: phonetisaurus (>=0.3.0,<0.4.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Description-Content-Type: text/markdown
 
 # dhlab toolkit
 Toolkit and models for working with National Library digital humanities laboratory data
```

