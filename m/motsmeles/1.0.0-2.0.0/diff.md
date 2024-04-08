# Comparing `tmp/motsmeles-1.0.0.tar.gz` & `tmp/motsmeles-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motsmeles-1.0.0.tar", max compression
+gzip compressed data, was "motsmeles-2.0.0.tar", max compression
```

## Comparing `motsmeles-1.0.0.tar` & `motsmeles-2.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       40 2024-04-05 17:58:54.337348 motsmeles-1.0.0/README.md
--rw-r--r--   0        0        0     6386 2024-04-05 18:06:19.819340 motsmeles-1.0.0/motsmeles.py
--rw-r--r--   0        0        0      352 2024-04-05 18:06:40.680862 motsmeles-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 motsmeles-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      930 2024-04-08 09:40:56.625407 motsmeles-2.0.0/README.md
+-rw-r--r--   0        0        0     7458 2024-04-08 09:37:18.533778 motsmeles-2.0.0/motsmeles.py
+-rw-r--r--   0        0        0      402 2024-04-08 09:45:19.741954 motsmeles-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 motsmeles-2.0.0/PKG-INFO
```

