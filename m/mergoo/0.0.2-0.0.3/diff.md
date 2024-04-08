# Comparing `tmp/mergoo-0.0.2.tar.gz` & `tmp/mergoo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergoo-0.0.2.tar", last modified: Mon Apr  8 10:30:05 2024, max compression
+gzip compressed data, was "mergoo-0.0.3.tar", last modified: Mon Apr  8 10:59:04 2024, max compression
```

## Comparing `mergoo-0.0.2.tar` & `mergoo-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 10:30:05.988190 mergoo-0.0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7651 2024-04-08 10:00:06.000000 mergoo-0.0.2/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      271 2024-04-08 10:30:05.988190 mergoo-0.0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5078 2024-04-08 10:00:06.000000 mergoo-0.0.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 10:30:05.988190 mergoo-0.0.2/mergoo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      271 2024-04-08 10:30:05.000000 mergoo-0.0.2/mergoo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2024-04-08 10:30:05.000000 mergoo-0.0.2/mergoo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-08 10:30:05.000000 mergoo-0.0.2/mergoo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      145 2024-04-08 10:30:05.000000 mergoo-0.0.2/mergoo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-08 10:30:05.000000 mergoo-0.0.2/mergoo.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-08 10:30:05.988190 mergoo-0.0.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      663 2024-04-08 10:29:19.000000 mergoo-0.0.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 10:59:04.331060 mergoo-0.0.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7651 2024-04-08 10:00:06.000000 mergoo-0.0.3/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5830 2024-04-08 10:59:04.327060 mergoo-0.0.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5078 2024-04-08 10:00:06.000000 mergoo-0.0.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 10:59:04.327060 mergoo-0.0.3/mergoo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8273 2024-04-08 10:00:06.000000 mergoo-0.0.3/mergoo/compose_experts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2688 2024-04-08 10:00:06.000000 mergoo-0.0.3/mergoo/compose_layers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9649 2024-04-08 10:00:06.000000 mergoo-0.0.3/mergoo/safe_saving.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 10:59:04.327060 mergoo-0.0.3/mergoo.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5830 2024-04-08 10:59:04.000000 mergoo-0.0.3/mergoo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2024-04-08 10:59:04.000000 mergoo-0.0.3/mergoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-08 10:59:04.000000 mergoo-0.0.3/mergoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      163 2024-04-08 10:59:04.000000 mergoo-0.0.3/mergoo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-04-08 10:59:04.000000 mergoo-0.0.3/mergoo.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      946 2024-04-08 10:58:27.000000 mergoo-0.0.3/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-08 10:59:04.331060 mergoo-0.0.3/setup.cfg
```

### Comparing `mergoo-0.0.2/LICENSE` & `mergoo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.2/README.md` & `mergoo-0.0.3/README.md`

 * *Files identical despite different names*

