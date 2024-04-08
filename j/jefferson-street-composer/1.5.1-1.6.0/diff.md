# Comparing `tmp/jefferson_street_composer-1.5.1.tar.gz` & `tmp/jefferson-street-composer-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jefferson_street_composer-1.5.1.tar", max compression
+gzip compressed data, was "jefferson-street-composer-1.6.0.tar", max compression
```

## Comparing `jefferson_street_composer-1.5.1.tar` & `jefferson-street-composer-1.6.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2023-04-19 00:26:26.692765 jefferson_street_composer-1.5.1/README.md
--rw-r--r--   0        0        0       99 2023-04-19 00:26:26.693182 jefferson_street_composer-1.5.1/jefferson_street_composer/__init__.py
--rw-r--r--   0        0        0      115 2023-04-19 00:26:26.693492 jefferson_street_composer-1.5.1/jefferson_street_composer/services/__init__.py
--rw-r--r--   0        0        0      131 2023-04-19 00:26:26.693835 jefferson_street_composer-1.5.1/jefferson_street_composer/services/specifications/__init__.py
--rw-r--r--   0        0        0     2600 2024-03-31 06:04:58.825814 jefferson_street_composer-1.5.1/jefferson_street_composer/services/specifications/base_ingest_dag.py
--rw-r--r--   0        0        0      489 2024-03-31 06:05:03.748288 jefferson_street_composer-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 jefferson_street_composer-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 00:26:26.692765 jefferson-street-composer-1.6.0/README.md
+-rw-r--r--   0        0        0       99 2023-04-19 00:26:26.693182 jefferson-street-composer-1.6.0/jefferson_street_composer/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-19 00:26:26.693492 jefferson-street-composer-1.6.0/jefferson_street_composer/services/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-19 00:26:26.693835 jefferson-street-composer-1.6.0/jefferson_street_composer/services/specifications/__init__.py
+-rw-r--r--   0        0        0     2600 2024-04-08 00:25:41.995531 jefferson-street-composer-1.6.0/jefferson_street_composer/services/specifications/base_ingest_dag.py
+-rw-r--r--   0        0        0      489 2024-04-08 00:26:06.241520 jefferson-street-composer-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 jefferson-street-composer-1.6.0/setup.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 jefferson-street-composer-1.6.0/PKG-INFO
```

### Comparing `jefferson_street_composer-1.5.1/jefferson_street_composer/services/specifications/base_ingest_dag.py` & `jefferson-street-composer-1.6.0/jefferson_street_composer/services/specifications/base_ingest_dag.py`

 * *Files identical despite different names*

