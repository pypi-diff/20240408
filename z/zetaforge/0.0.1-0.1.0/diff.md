# Comparing `tmp/zetaforge-0.0.1.tar.gz` & `tmp/zetaforge-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zetaforge-0.0.1.tar", last modified: Fri Aug 25 17:03:28 2023, max compression
+gzip compressed data, was "zetaforge-0.1.0.tar", last modified: Mon Apr  8 17:39:52 2024, max compression
```

## Comparing `zetaforge-0.0.1.tar` & `zetaforge-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,24 @@
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-08-25 17:03:28.649744 zetaforge-0.0.1/
--rw-r--r--   0 jon        (501) staff       (20)     1112 2023-08-25 17:03:28.649622 zetaforge-0.0.1/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)        0 2023-08-25 17:01:46.000000 zetaforge-0.0.1/README.md
--rw-r--r--   0 jon        (501) staff       (20)       38 2023-08-25 17:03:28.649775 zetaforge-0.0.1/setup.cfg
--rw-r--r--   0 jon        (501) staff       (20)     2047 2023-08-25 17:03:25.000000 zetaforge-0.0.1/setup.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-08-25 17:03:28.648982 zetaforge-0.0.1/zetaforge/
--rw-r--r--   0 jon        (501) staff       (20)       22 2023-08-25 17:00:15.000000 zetaforge-0.0.1/zetaforge/__init__.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-08-25 17:03:28.649481 zetaforge-0.0.1/zetaforge.egg-info/
--rw-r--r--   0 jon        (501) staff       (20)     1112 2023-08-25 17:03:28.000000 zetaforge-0.0.1/zetaforge.egg-info/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      204 2023-08-25 17:03:28.000000 zetaforge-0.0.1/zetaforge.egg-info/SOURCES.txt
--rw-r--r--   0 jon        (501) staff       (20)        1 2023-08-25 17:03:28.000000 zetaforge-0.0.1/zetaforge.egg-info/dependency_links.txt
--rw-r--r--   0 jon        (501) staff       (20)       16 2023-08-25 17:03:28.000000 zetaforge-0.0.1/zetaforge.egg-info/requires.txt
--rw-r--r--   0 jon        (501) staff       (20)       10 2023-08-25 17:03:28.000000 zetaforge-0.0.1/zetaforge.egg-info/top_level.txt
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-08 17:39:52.829220 zetaforge-0.1.0/
+-rw-r--r--   0 jon        (501) staff       (20)      190 2024-04-08 17:39:52.829077 zetaforge-0.1.0/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)     5172 2024-01-25 16:14:41.000000 zetaforge-0.1.0/README.md
+-rw-r--r--   0 jon        (501) staff       (20)      104 2024-03-27 00:08:10.000000 zetaforge-0.1.0/pyproject.toml
+-rw-r--r--   0 jon        (501) staff       (20)       38 2024-04-08 17:39:52.829266 zetaforge-0.1.0/setup.cfg
+-rw-r--r--   0 jon        (501) staff       (20)     1869 2024-04-07 00:30:52.000000 zetaforge-0.1.0/setup.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-08 17:39:52.827883 zetaforge-0.1.0/zetaforge/
+-rw-r--r--   0 jon        (501) staff       (20)       22 2024-04-08 17:39:52.000000 zetaforge-0.1.0/zetaforge/__init__.py
+-rw-r--r--   0 jon        (501) staff       (20)     1617 2024-04-07 00:30:52.000000 zetaforge-0.1.0/zetaforge/check_forge_dependencies.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-08 17:39:52.828648 zetaforge-0.1.0/zetaforge/executables/
+-rw-r--r--   0 jon        (501) staff       (20)      122 2024-03-27 00:08:10.000000 zetaforge-0.1.0/zetaforge/executables/README.md
+-rw-r--r--   0 jon        (501) staff       (20)     3391 2024-04-07 00:30:52.000000 zetaforge-0.1.0/zetaforge/forge_cli.py
+-rw-r--r--   0 jon        (501) staff       (20)    14283 2024-04-07 00:30:52.000000 zetaforge-0.1.0/zetaforge/forge_runner.py
+-rw-r--r--   0 jon        (501) staff       (20)    11862 2024-04-08 16:35:30.000000 zetaforge-0.1.0/zetaforge/install_forge_dependencies.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-08 17:39:52.828871 zetaforge-0.1.0/zetaforge/utils/
+-rw-r--r--   0 jon        (501) staff       (20)     2959 2024-04-07 00:30:52.000000 zetaforge-0.1.0/zetaforge/utils/build.yaml
+-rw-r--r--   0 jon        (501) staff       (20)    37294 2024-03-27 00:08:10.000000 zetaforge-0.1.0/zetaforge/utils/install.yaml
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-08 17:39:52.828546 zetaforge-0.1.0/zetaforge.egg-info/
+-rw-r--r--   0 jon        (501) staff       (20)      190 2024-04-08 17:39:52.000000 zetaforge-0.1.0/zetaforge.egg-info/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)      470 2024-04-08 17:39:52.000000 zetaforge-0.1.0/zetaforge.egg-info/SOURCES.txt
+-rw-r--r--   0 jon        (501) staff       (20)        1 2024-04-08 17:39:52.000000 zetaforge-0.1.0/zetaforge.egg-info/dependency_links.txt
+-rw-r--r--   0 jon        (501) staff       (20)       55 2024-04-08 17:39:52.000000 zetaforge-0.1.0/zetaforge.egg-info/entry_points.txt
+-rw-r--r--   0 jon        (501) staff       (20)       65 2024-04-08 17:39:52.000000 zetaforge-0.1.0/zetaforge.egg-info/requires.txt
+-rw-r--r--   0 jon        (501) staff       (20)       10 2024-04-08 17:39:52.000000 zetaforge-0.1.0/zetaforge.egg-info/top_level.txt
```

