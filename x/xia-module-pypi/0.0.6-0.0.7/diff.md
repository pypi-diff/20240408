# Comparing `tmp/xia-module-pypi-0.0.6.tar.gz` & `tmp/xia-module-pypi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xia-module-pypi-0.0.6.tar", last modified: Sat Apr  6 16:38:14 2024, max compression
+gzip compressed data, was "xia-module-pypi-0.0.7.tar", last modified: Mon Apr  8 17:59:27 2024, max compression
```

## Comparing `xia-module-pypi-0.0.6.tar` & `xia-module-pypi-0.0.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-06 16:38:14.000000 xia-module-pypi-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.638709 xia-module-pypi-0.0.6/xia_module_pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/pypi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.638709 xia-module-pypi-0.0.6/xia_module_pypi/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.638709 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/activate/
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/activate/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/base/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/base/activate.tf
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.638709 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/cicd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/cicd/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.638709 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/cicd/github/workflow.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/init/
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/init/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/init/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/init/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/init/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/init/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/module/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/template/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/template/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.638709 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.638709 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/cicd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/cicd/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.638709 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/cicd/github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/cicd/github/workflow.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/init/
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/init/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/init/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/init/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/init/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/init/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.642709 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/template/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 16:38:06.000000 xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/template/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:38:14.638709 xia-module-pypi-0.0.6/xia_module_pypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-06 16:38:14.000000 xia-module-pypi-0.0.6/xia_module_pypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-06 16:38:14.000000 xia-module-pypi-0.0.6/xia_module_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:38:14.000000 xia-module-pypi-0.0.6/xia_module_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 16:38:14.000000 xia-module-pypi-0.0.6/xia_module_pypi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 16:38:14.000000 xia-module-pypi-0.0.6/xia_module_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.694775 xia-module-pypi-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 17:59:27.000000 xia-module-pypi-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-08 17:59:27.694775 xia-module-pypi-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:59:27.694775 xia-module-pypi-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.690775 xia-module-pypi-0.0.7/xia_module_pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.686775 xia-module-pypi-0.0.7/xia_module_pypi/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.686775 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.690775 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/activate/
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/activate/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.690775 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/base/activate.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.686775 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/cicd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.690775 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/cicd/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.686775 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.690775 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/cicd/github/workflow.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.690775 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/init/
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/init/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/init/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/init/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/init/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/init/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.690775 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.690775 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/template/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.686775 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.686775 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/cicd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.690775 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/cicd/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.686775 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/cicd/github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.690775 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/cicd/github/workflow.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.690775 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/init/
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/init/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/init/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/init/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/init/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/init/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.694775 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 17:59:14.000000 xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/template/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:59:27.690775 xia-module-pypi-0.0.7/xia_module_pypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-08 17:59:27.000000 xia-module-pypi-0.0.7/xia_module_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-08 17:59:27.000000 xia-module-pypi-0.0.7/xia_module_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:59:27.000000 xia-module-pypi-0.0.7/xia_module_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 17:59:27.000000 xia-module-pypi-0.0.7/xia_module_pypi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 17:59:27.000000 xia-module-pypi-0.0.7/xia_module_pypi.egg-info/top_level.txt
```

### Comparing `xia-module-pypi-0.0.6/LICENSE` & `xia-module-pypi-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/setup.py` & `xia-module-pypi-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi/pypi.py` & `xia-module-pypi-0.0.7/xia_module_pypi/pypi.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,13 +15,15 @@
     def _build_template_module(self, **kwargs):
         if self._check_package():
             return
         package_name = kwargs.get("package_name", os.path.basename(os.getcwd()))
         os.makedirs(package_name.replace("-", "_"), exist_ok=True)
         template = self.env.get_template("__init__.py.jinja")
         content = template.render(**kwargs)
-        with open(f'{package_name.replace("-", "_")}/__init__.py', "w") as fp:
+        init_file_name = f'{package_name.replace("-", "_")}/__init__.py'
+        with open(init_file_name, "w") as fp:
             fp.write(content)
+        self.git_add(init_file_name)
 
     def _build_template(self, **kwargs):
         # Step 1: Build
         self._build_template_module(**kwargs)
```

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/activate/main.tf` & `xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/activate/main.tf`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf` & `xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/action.yml` & `xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/action.yml`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/cicd/github/workflow.yml` & `xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/cicd/github/workflow.yml`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/init/.gitignore` & `xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/init/.gitignore`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/init/LICENSE` & `xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/init/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi/templates/gcp-module-pypi/init/setup.py` & `xia-module-pypi-0.0.7/xia_module_pypi/templates/gcp-module-pypi/init/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml` & `xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/init/.gitignore` & `xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/init/.gitignore`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/init/LICENSE` & `xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/init/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi/templates/module-pypi/init/setup.py` & `xia-module-pypi-0.0.7/xia_module_pypi/templates/module-pypi/init/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.6/xia_module_pypi.egg-info/SOURCES.txt` & `xia-module-pypi-0.0.7/xia_module_pypi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

