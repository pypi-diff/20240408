# Comparing `tmp/lazyqsar-0.3.tar.gz` & `tmp/lazyqsar-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyqsar-0.3.tar", last modified: Mon Sep 25 12:02:06 2023, max compression
+gzip compressed data, was "/home/gturon/github/ersilia-os/lazy-qsar/dist/.tmp-a1xf0k1u/lazyqsar-0.4.tar", last modified: Mon Apr  8 10:05:23 2024, max compression
```

## Comparing `lazyqsar-0.3.tar` & `lazyqsar-0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 gemmaturon   (501) staff       (20)        0 2023-09-25 12:02:06.998814 lazyqsar-0.3/
--rw-r--r--   0 gemmaturon   (501) staff       (20)    35149 2023-09-25 11:38:37.000000 lazyqsar-0.3/LICENSE
--rw-r--r--   0 gemmaturon   (501) staff       (20)       24 2023-09-25 11:54:31.000000 lazyqsar-0.3/MANIFEST.in
--rw-r--r--   0 gemmaturon   (501) staff       (20)     4137 2023-09-25 12:02:06.998699 lazyqsar-0.3/PKG-INFO
--rw-r--r--   0 gemmaturon   (501) staff       (20)     3244 2023-07-11 10:39:17.000000 lazyqsar-0.3/README.md
-drwxr-xr-x   0 gemmaturon   (501) staff       (20)        0 2023-09-25 12:02:06.996772 lazyqsar-0.3/lazyqsar/
--rw-r--r--   0 gemmaturon   (501) staff       (20)      359 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/__init__.py
-drwxr-xr-x   0 gemmaturon   (501) staff       (20)        0 2023-09-25 12:02:06.997992 lazyqsar-0.3/lazyqsar/binary/
--rw-r--r--   0 gemmaturon   (501) staff       (20)        0 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/binary/__init__.py
--rw-r--r--   0 gemmaturon   (501) staff       (20)     2095 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/binary/classic.py
--rw-r--r--   0 gemmaturon   (501) staff       (20)     2749 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/binary/eosembedding.py
--rw-r--r--   0 gemmaturon   (501) staff       (20)     2128 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/binary/maccs.py
--rw-r--r--   0 gemmaturon   (501) staff       (20)     2094 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/binary/mordred.py
--rw-r--r--   0 gemmaturon   (501) staff       (20)     2738 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/binary/morgan.py
--rw-r--r--   0 gemmaturon   (501) staff       (20)     2088 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/binary/rdkit.py
-drwxr-xr-x   0 gemmaturon   (501) staff       (20)        0 2023-09-25 12:02:06.998212 lazyqsar-0.3/lazyqsar/descriptors/
--rw-r--r--   0 gemmaturon   (501) staff       (20)        0 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/descriptors/__init__.py
--rw-r--r--   0 gemmaturon   (501) staff       (20)    17691 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/descriptors/descriptors.py
-drwxr-xr-x   0 gemmaturon   (501) staff       (20)        0 2023-09-25 12:02:06.998528 lazyqsar-0.3/lazyqsar/regression/
--rw-r--r--   0 gemmaturon   (501) staff       (20)        0 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/regression/__init__.py
--rw-r--r--   0 gemmaturon   (501) staff       (20)     2172 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/regression/eosembedding.py
--rw-r--r--   0 gemmaturon   (501) staff       (20)     2163 2023-07-11 10:39:17.000000 lazyqsar-0.3/lazyqsar/regression/morgan.py
-drwxr-xr-x   0 gemmaturon   (501) staff       (20)        0 2023-09-25 12:02:06.997251 lazyqsar-0.3/lazyqsar.egg-info/
--rw-r--r--   0 gemmaturon   (501) staff       (20)     4137 2023-09-25 12:02:06.000000 lazyqsar-0.3/lazyqsar.egg-info/PKG-INFO
--rw-r--r--   0 gemmaturon   (501) staff       (20)      592 2023-09-25 12:02:06.000000 lazyqsar-0.3/lazyqsar.egg-info/SOURCES.txt
--rw-r--r--   0 gemmaturon   (501) staff       (20)        1 2023-09-25 12:02:06.000000 lazyqsar-0.3/lazyqsar.egg-info/dependency_links.txt
--rw-r--r--   0 gemmaturon   (501) staff       (20)       51 2023-09-25 12:02:06.000000 lazyqsar-0.3/lazyqsar.egg-info/requires.txt
--rw-r--r--   0 gemmaturon   (501) staff       (20)        9 2023-09-25 12:02:06.000000 lazyqsar-0.3/lazyqsar.egg-info/top_level.txt
--rw-r--r--   0 gemmaturon   (501) staff       (20)       51 2023-09-25 11:30:49.000000 lazyqsar-0.3/requirements.txt
--rw-r--r--   0 gemmaturon   (501) staff       (20)       38 2023-09-25 12:02:06.998857 lazyqsar-0.3/setup.cfg
--rw-r--r--   0 gemmaturon   (501) staff       (20)     1364 2023-09-25 12:01:59.000000 lazyqsar-0.3/setup.py
+drwxrwxr-x   0 gturon    (1000) gturon    (1000)        0 2024-04-08 10:05:23.000000 lazyqsar-0.4/
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)    35149 2023-11-23 10:29:52.000000 lazyqsar-0.4/LICENSE
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)       24 2023-11-23 10:29:52.000000 lazyqsar-0.4/MANIFEST.in
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)     4137 2024-04-08 10:05:23.000000 lazyqsar-0.4/PKG-INFO
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)     3244 2023-11-23 10:29:52.000000 lazyqsar-0.4/README.md
+drwxrwxr-x   0 gturon    (1000) gturon    (1000)        0 2024-04-08 10:05:23.000000 lazyqsar-0.4/lazyqsar/
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)      359 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/__init__.py
+drwxrwxr-x   0 gturon    (1000) gturon    (1000)        0 2024-04-08 10:05:23.000000 lazyqsar-0.4/lazyqsar/binary/
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)        0 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/binary/__init__.py
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)     2095 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/binary/classic.py
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)     2749 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/binary/eosembedding.py
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)     2128 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/binary/maccs.py
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)     2094 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/binary/mordred.py
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)     2738 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/binary/morgan.py
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)     2088 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/binary/rdkit.py
+drwxrwxr-x   0 gturon    (1000) gturon    (1000)        0 2024-04-08 10:05:23.000000 lazyqsar-0.4/lazyqsar/descriptors/
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)        0 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/descriptors/__init__.py
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)    17691 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/descriptors/descriptors.py
+drwxrwxr-x   0 gturon    (1000) gturon    (1000)        0 2024-04-08 10:05:23.000000 lazyqsar-0.4/lazyqsar/regression/
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)        0 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/regression/__init__.py
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)     2172 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/regression/eosembedding.py
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)     2163 2023-11-23 10:29:52.000000 lazyqsar-0.4/lazyqsar/regression/morgan.py
+drwxrwxr-x   0 gturon    (1000) gturon    (1000)        0 2024-04-08 10:05:23.000000 lazyqsar-0.4/lazyqsar.egg-info/
+-rw-r--r--   0 gturon    (1000) gturon    (1000)     4137 2024-04-08 10:05:23.000000 lazyqsar-0.4/lazyqsar.egg-info/PKG-INFO
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)      592 2024-04-08 10:05:23.000000 lazyqsar-0.4/lazyqsar.egg-info/SOURCES.txt
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)        1 2024-04-08 10:05:23.000000 lazyqsar-0.4/lazyqsar.egg-info/dependency_links.txt
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)       71 2024-04-08 10:05:23.000000 lazyqsar-0.4/lazyqsar.egg-info/requires.txt
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)        9 2024-04-08 10:05:23.000000 lazyqsar-0.4/lazyqsar.egg-info/top_level.txt
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)       71 2024-04-08 10:03:04.000000 lazyqsar-0.4/requirements.txt
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)       38 2024-04-08 10:05:23.000000 lazyqsar-0.4/setup.cfg
+-rw-rw-r--   0 gturon    (1000) gturon    (1000)     1364 2024-04-08 10:04:36.000000 lazyqsar-0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `lazyqsar-0.3/LICENSE` & `lazyqsar-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyqsar-0.3/PKG-INFO` & `lazyqsar-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqsar
-Version: 0.3
+Version: 0.4
 Summary: A library to quickly build QSAR models
 Home-page: https://github.com/ersilia-os/lazy-qsar
 Author: Miquel Duran-Frigola
 Author-email: miquel@ersilia.io
 License: GPLv3
 Project-URL: Source Code, https://github.com/ersilia-os/lazy-qsar
 Keywords: qsar machine-learning chemistry computer-aided-drug-design
```

### Comparing `lazyqsar-0.3/README.md` & `lazyqsar-0.4/README.md`

 * *Files identical despite different names*

### Comparing `lazyqsar-0.3/lazyqsar/binary/classic.py` & `lazyqsar-0.4/lazyqsar/binary/classic.py`

 * *Files identical despite different names*

### Comparing `lazyqsar-0.3/lazyqsar/binary/eosembedding.py` & `lazyqsar-0.4/lazyqsar/binary/eosembedding.py`

 * *Files identical despite different names*

### Comparing `lazyqsar-0.3/lazyqsar/binary/maccs.py` & `lazyqsar-0.4/lazyqsar/binary/maccs.py`

 * *Files identical despite different names*

### Comparing `lazyqsar-0.3/lazyqsar/binary/mordred.py` & `lazyqsar-0.4/lazyqsar/binary/mordred.py`

 * *Files identical despite different names*

### Comparing `lazyqsar-0.3/lazyqsar/binary/morgan.py` & `lazyqsar-0.4/lazyqsar/binary/morgan.py`

 * *Files identical despite different names*

### Comparing `lazyqsar-0.3/lazyqsar/binary/rdkit.py` & `lazyqsar-0.4/lazyqsar/binary/rdkit.py`

 * *Files identical despite different names*

### Comparing `lazyqsar-0.3/lazyqsar/descriptors/descriptors.py` & `lazyqsar-0.4/lazyqsar/descriptors/descriptors.py`

 * *Files identical despite different names*

### Comparing `lazyqsar-0.3/lazyqsar/regression/eosembedding.py` & `lazyqsar-0.4/lazyqsar/regression/eosembedding.py`

 * *Files identical despite different names*

### Comparing `lazyqsar-0.3/lazyqsar/regression/morgan.py` & `lazyqsar-0.4/lazyqsar/regression/morgan.py`

 * *Files identical despite different names*

### Comparing `lazyqsar-0.3/lazyqsar.egg-info/PKG-INFO` & `lazyqsar-0.4/lazyqsar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqsar
-Version: 0.3
+Version: 0.4
 Summary: A library to quickly build QSAR models
 Home-page: https://github.com/ersilia-os/lazy-qsar
 Author: Miquel Duran-Frigola
 Author-email: miquel@ersilia.io
 License: GPLv3
 Project-URL: Source Code, https://github.com/ersilia-os/lazy-qsar
 Keywords: qsar machine-learning chemistry computer-aided-drug-design
```

### Comparing `lazyqsar-0.3/lazyqsar.egg-info/SOURCES.txt` & `lazyqsar-0.4/lazyqsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazyqsar-0.3/setup.py` & `lazyqsar-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 
 setup(
     name="lazyqsar",
-    version="0.3",
+    version="0.4",
     author="Miquel Duran-Frigola",
     author_email="miquel@ersilia.io",
     url="https://github.com/ersilia-os/lazy-qsar",
     description="A library to quickly build QSAR models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPLv3",
```

