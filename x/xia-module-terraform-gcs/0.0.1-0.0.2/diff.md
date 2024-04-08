# Comparing `tmp/xia-module-terraform-gcs-0.0.1.tar.gz` & `tmp/xia-module-terraform-gcs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xia-module-terraform-gcs-0.0.1.tar", last modified: Mon Apr  8 18:02:01 2024, max compression
+gzip compressed data, was "xia-module-terraform-gcs-0.0.2.tar", last modified: Mon Apr  8 20:58:47 2024, max compression
```

## Comparing `xia-module-terraform-gcs-0.0.1.tar` & `xia-module-terraform-gcs-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:02:01.055909 xia-module-terraform-gcs-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 18:01:32.000000 xia-module-terraform-gcs-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 18:02:00.000000 xia-module-terraform-gcs-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 18:02:01.055909 xia-module-terraform-gcs-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 18:01:32.000000 xia-module-terraform-gcs-0.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:02:01.055909 xia-module-terraform-gcs-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-08 18:01:32.000000 xia-module-terraform-gcs-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:02:01.055909 xia-module-terraform-gcs-0.0.1/xia_module_terraform_gcs/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-08 18:01:32.000000 xia-module-terraform-gcs-0.0.1/xia_module_terraform_gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 18:01:32.000000 xia-module-terraform-gcs-0.0.1/xia_module_terraform_gcs/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:02:01.055909 xia-module-terraform-gcs-0.0.1/xia_module_terraform_gcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 18:02:00.000000 xia-module-terraform-gcs-0.0.1/xia_module_terraform_gcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 18:02:01.000000 xia-module-terraform-gcs-0.0.1/xia_module_terraform_gcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:02:00.000000 xia-module-terraform-gcs-0.0.1/xia_module_terraform_gcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 18:02:00.000000 xia-module-terraform-gcs-0.0.1/xia_module_terraform_gcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 18:02:00.000000 xia-module-terraform-gcs-0.0.1/xia_module_terraform_gcs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:58:47.284752 xia-module-terraform-gcs-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 20:58:19.000000 xia-module-terraform-gcs-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 20:58:46.000000 xia-module-terraform-gcs-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 20:58:47.284752 xia-module-terraform-gcs-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 20:58:19.000000 xia-module-terraform-gcs-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:58:47.284752 xia-module-terraform-gcs-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-08 20:58:19.000000 xia-module-terraform-gcs-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:58:47.280752 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-08 20:58:19.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 20:58:19.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:58:47.280752 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:58:47.280752 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:58:47.280752 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/activate/
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-08 20:58:19.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/activate/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-08 20:58:19.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/activate/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:58:47.284752 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 20:58:19.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/base/activate.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-08 20:58:19.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:58:47.280752 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/cicd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:58:47.284752 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/cicd/github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-08 20:58:19.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/cicd/github/workflow.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:58:47.284752 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/module/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 20:58:19.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:58:19.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs/templates/module-state-gcs/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:58:47.280752 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 20:58:47.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-08 20:58:47.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:58:47.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 20:58:47.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 20:58:47.000000 xia-module-terraform-gcs-0.0.2/xia_module_terraform_gcs.egg-info/top_level.txt
```

### Comparing `xia-module-terraform-gcs-0.0.1/LICENSE` & `xia-module-terraform-gcs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-terraform-gcs-0.0.1/setup.py` & `xia-module-terraform-gcs-0.0.2/setup.py`

 * *Files identical despite different names*

