# Comparing `tmp/rhdzmota-3.1.0.tar.gz` & `tmp/rhdzmota-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhdzmota-3.1.0.tar", last modified: Thu Mar 14 02:30:31 2024, max compression
+gzip compressed data, was "rhdzmota-3.1.1.tar", last modified: Sun Apr  7 23:42:58 2024, max compression
```

## Comparing `rhdzmota-3.1.0.tar` & `rhdzmota-3.1.1.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.832006 rhdzmota-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-14 02:30:31.832006 rhdzmota-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.828006 rhdzmota-3.1.0/bin/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/bin/rhdzmota
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 02:30:31.832006 rhdzmota-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.828006 rhdzmota-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.828006 rhdzmota-3.1.0/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.828006 rhdzmota-3.1.0/src/main/rhdzmota/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/celery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.828006 rhdzmota-3.1.0/src/main/rhdzmota/celery_workers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/celery_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/celery_workers/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.828006 rhdzmota-3.1.0/src/main/rhdzmota/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/cli/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.828006 rhdzmota-3.1.0/src/main/rhdzmota/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/ext/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.832006 rhdzmota-3.1.0/src/main/rhdzmota/google_services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/google_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/google_services/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/google_services/gmail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.832006 rhdzmota-3.1.0/src/main/rhdzmota/heartbeat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/heartbeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/heartbeat/daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/heartbeat/daemon_heart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.832006 rhdzmota-3.1.0/src/main/rhdzmota/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/interface/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.832006 rhdzmota-3.1.0/src/main/rhdzmota/iso3166/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/iso3166/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/iso3166/country_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.832006 rhdzmota-3.1.0/src/main/rhdzmota/iso3166/datafiles/
--rw-r--r--   0 runner    (1001) docker     (127)    25179 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/iso3166/datafiles/countries.json
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/iso3166/datafiles/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/iso3166/datafiles/mx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/iso3166/datafiles/us.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.832006 rhdzmota-3.1.0/src/main/rhdzmota/mail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/mail/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/mail/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.832006 rhdzmota-3.1.0/src/main/rhdzmota/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/utils/gists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/utils/json_web_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/utils/rsa_encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/utils/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.832006 rhdzmota-3.1.0/src/main/rhdzmota/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-03-14 02:30:14.000000 rhdzmota-3.1.0/src/main/rhdzmota/wrappers/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:30:31.828006 rhdzmota-3.1.0/src/main/rhdzmota.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-14 02:30:31.000000 rhdzmota-3.1.0/src/main/rhdzmota.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-14 02:30:31.000000 rhdzmota-3.1.0/src/main/rhdzmota.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 02:30:31.000000 rhdzmota-3.1.0/src/main/rhdzmota.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-14 02:30:31.000000 rhdzmota-3.1.0/src/main/rhdzmota.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-14 02:30:31.000000 rhdzmota-3.1.0/src/main/rhdzmota.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 02:30:31.000000 rhdzmota-3.1.0/src/main/rhdzmota.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.843347 rhdzmota-3.1.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/bin/rhdzmota
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.843347 rhdzmota-3.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.843347 rhdzmota-3.1.1/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.843347 rhdzmota-3.1.1/src/main/rhdzmota/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/celery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.843347 rhdzmota-3.1.1/src/main/rhdzmota/celery_workers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/celery_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/celery_workers/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/src/main/rhdzmota/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/cli/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/src/main/rhdzmota/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/ext/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/src/main/rhdzmota/google_services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/google_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/google_services/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/google_services/gmail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/src/main/rhdzmota/heartbeat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/heartbeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/heartbeat/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/heartbeat/daemon_heart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/src/main/rhdzmota/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/interface/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/src/main/rhdzmota/iso3166/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/iso3166/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/iso3166/country_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/src/main/rhdzmota/iso3166/datafiles/
+-rw-r--r--   0 runner    (1001) docker     (127)    25179 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/iso3166/datafiles/countries.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/iso3166/datafiles/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/iso3166/datafiles/mx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/iso3166/datafiles/us.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/src/main/rhdzmota/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/mail/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/mail/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/src/main/rhdzmota/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/utils/gists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/utils/json_web_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/utils/rsa_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/utils/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/version
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.847347 rhdzmota-3.1.1/src/main/rhdzmota/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-07 23:42:43.000000 rhdzmota-3.1.1/src/main/rhdzmota/wrappers/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:58.843347 rhdzmota-3.1.1/src/main/rhdzmota.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-07 23:42:58.000000 rhdzmota-3.1.1/src/main/rhdzmota.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-07 23:42:58.000000 rhdzmota-3.1.1/src/main/rhdzmota.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:42:58.000000 rhdzmota-3.1.1/src/main/rhdzmota.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-07 23:42:58.000000 rhdzmota-3.1.1/src/main/rhdzmota.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-07 23:42:58.000000 rhdzmota-3.1.1/src/main/rhdzmota.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 23:42:58.000000 rhdzmota-3.1.1/src/main/rhdzmota.egg-info/top_level.txt
```

### Comparing `rhdzmota-3.1.0/PKG-INFO` & `rhdzmota-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhdzmota
-Version: 3.1.0
+Version: 3.1.1
 Summary: RHDZMOTA Package
 Home-page: https://github.com/rhdzmota/package.rhdzmota.com
 Author: Rodrigo H. Mota
 Author-email: info@rhdzmota.com
 Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 Provides-Extra: baseline
```

### Comparing `rhdzmota-3.1.0/README.md` & `rhdzmota-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/requirements.txt` & `rhdzmota-3.1.1/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 typing_extensions==4.3.0: develop
 typed-ast==1.5.4: develop
 scalene==1.3.12: develop
 ipython==7.34.0: develop
 jupyter==1.0.0: develop
 
 # RHDZMOTA Extensions
-rhdzmota-extension-hello-world==0.1.0: ext.hello_world
-rhdzmota-extension-streamlit-webapps==0.5.0: ext.streamlit_webapps
+rhdzmota-extension-hello-world>=0.1.2,<1.0.0: ext.hello_world
+rhdzmota-extension-streamlit-webapps>=0.5.1,<1.0.0: ext.streamlit_webapps
 
 # Tools Exclusive
 rsa==4.8: standalone
 psutil==5.9.2: standalone
 
 # Celery Exclusive
 celery[redis]==5.1.2: celery
```

### Comparing `rhdzmota-3.1.0/setup.py` & `rhdzmota-3.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "DEPS_FILE",
     default="",
 )
 
 with open("requirements.txt", "r") as file:
     requirements = [line for line in file.read().splitlines() if line and not line.startswith("#")]
 
-with open(os.path.join(CODEBASE_PATH, "rhdzmota", "VERSION"), "r") as file:
+with open(os.path.join(CODEBASE_PATH, "rhdzmota", "version"), "r") as file:
     version = file.read().strip()
 
 with open("README.md") as file:
     readme = file.read()
 
 
 def get_extras_requires(requirement_list: List[str]) -> Dict[str, List[str]]:
@@ -78,15 +78,16 @@
     author_email="info@rhdzmota.com",
     packages=find_namespace_packages(where=CODEBASE_PATH),
     package_dir={
         "": CODEBASE_PATH
     },
     package_data={
         "": [
-            os.path.join("iso3166", "datafiles", "*.json"),
+            os.path.join(CODEBASE_PATH, "rhdzmota", "iso3166", "datafiles", "*.json"),
+            os.path.join(CODEBASE_PATH, "rhdzmota", "version"),
         ]
     },
     entry_points={
         "console_scripts": [
             "rhdzmota=rhdzmota.cli.main:main",
             "rhdzmota.ext=rhdzmota.cli.ext:ext",
         ]
```

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/celery.py` & `rhdzmota-3.1.1/src/main/rhdzmota/celery.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/cli/ext.py` & `rhdzmota-3.1.1/src/main/rhdzmota/cli/ext.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,14 +29,36 @@
                 self.module_name_cli,
             ]
         )
 
     def get_extension_module(self, extension: str):
         return importlib.import_module(self.get_import_pattern(extension=extension))
 
+    def version(
+            self,
+            extension: str,
+            overwrite_version_import_pattern: Optional[str] = None,
+            overwrite_version_varname: Optional[str] = None,
+            path: bool = False,
+            fail: bool = False,
+    ):
+        version_varname = overwrite_version_varname or "version"
+        version_import_pattern = overwrite_version_import_pattern or ".".join([
+            "rhdzmota",
+            "ext",
+            f"{extension}_version",
+        ])
+        version_module = importlib.import_module(version_import_pattern)
+        version = getattr(version_module, version_varname)
+        if not version and fail:
+            raise ValueError(
+                f"Version not found for extension {extension}: {version_import_pattern}"
+            )
+        return version.filepath if path else version.value
+
     def execute(self, extension: str, command: str, *args, **kwargs):
         extension_module = self.get_extension_module(extension=extension)
         ext_cli = getattr(extension_module, "CLI")
         with ext_cli(
             extension_import_pattern=self.get_import_pattern(extension),
         ) as cli:
             cmd = getattr(cli, command)
```

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/cli/main.py` & `rhdzmota-3.1.1/src/main/rhdzmota/cli/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import time
 from typing import Optional
 
 from rhdzmota.settings import logger_manager
 from rhdzmota.interface.cli import CLIBase
 from rhdzmota.utils.gists import Gist
+from rhdzmota.version import version
 
 
 logger = logger_manager.get_logger(name=__name__)
 
 
 class CLI(CLIBase):
 
@@ -27,21 +28,19 @@
         if save:
             with open(filename, "w") as file:
                 file.write(code)
         return f"\n\n{code}"
 
     @property
     def version_filepath(self) -> str:
-        path = os.path.join(os.path.dirname(__file__), "..")
-        return os.path.join(path, "VERSION")
+        return version.filepath
 
     @property
     def version_value(self) -> str:
-        with open(self.version_filepath, "r") as file:
-            return file.read()
+        return version.value
 
     @CLIBase.Formatter()
     def version(self, path: bool = False):
         if not path:
             return self.version_value
         return self.version_filepath
```

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/google_services/auth.py` & `rhdzmota-3.1.1/src/main/rhdzmota/google_services/auth.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/google_services/gmail.py` & `rhdzmota-3.1.1/src/main/rhdzmota/google_services/gmail.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/heartbeat/daemon.py` & `rhdzmota-3.1.1/src/main/rhdzmota/heartbeat/daemon.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/heartbeat/daemon_heart.py` & `rhdzmota-3.1.1/src/main/rhdzmota/heartbeat/daemon_heart.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/interface/cli.py` & `rhdzmota-3.1.1/src/main/rhdzmota/interface/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -35,14 +35,38 @@
             extension_import_pattern: Optional[str] = None,
     ):
         self.extension_import_pattern = extension_import_pattern
         self.now = dt.datetime.utcnow().isoformat()
         self.start = time.perf_counter()
         self.end = None
 
+    def standard_version_import_pattern(self) -> str:
+        *base_imports, _ = self.extension_import_pattern.split(".")
+        return ".".join(base_imports) + "_version"
+
+    def version(
+            self,
+            overwrite_version_import_pattern: Optional[str] = None,
+            overwrite_version_varname: Optional[str] = None,
+            path: bool = False,
+            fail: bool = False,
+    ):
+        import importlib
+
+        version_varname = overwrite_version_varname or "version"
+        version_import_pattern = overwrite_version_import_pattern or \
+            self.standard_version_import_pattern()
+        version_module = importlib.import_module(version_import_pattern)
+        version = getattr(version_module, version_varname)
+        if not version and fail:
+            raise ValueError(
+                f"Version ({version_varname}) not found: {version_import_pattern}"
+            )
+        return version.filepath if path else version.value
+
     def now(self, local: bool = False) -> str:
         return (dt.datetime.utcnow() if not local else dt.datetime.now()).isoformat()
 
     def hello(
             self,
             recipient: Optional[str] = None,
             sleep: int = 1,
```

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/iso3166/country_codes.py` & `rhdzmota-3.1.1/src/main/rhdzmota/iso3166/country_codes.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/iso3166/datafiles/countries.json` & `rhdzmota-3.1.1/src/main/rhdzmota/iso3166/datafiles/countries.json`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/iso3166/datafiles/mx.json` & `rhdzmota-3.1.1/src/main/rhdzmota/iso3166/datafiles/mx.json`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/iso3166/datafiles/us.json` & `rhdzmota-3.1.1/src/main/rhdzmota/iso3166/datafiles/us.json`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/mail/message.py` & `rhdzmota-3.1.1/src/main/rhdzmota/mail/message.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/mail/server.py` & `rhdzmota-3.1.1/src/main/rhdzmota/mail/server.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/settings.py` & `rhdzmota-3.1.1/src/main/rhdzmota/settings.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/utils/gists.py` & `rhdzmota-3.1.1/src/main/rhdzmota/utils/gists.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/utils/json_web_token.py` & `rhdzmota-3.1.1/src/main/rhdzmota/utils/json_web_token.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/utils/misc.py` & `rhdzmota-3.1.1/src/main/rhdzmota/utils/misc.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/utils/rsa_encryption.py` & `rhdzmota-3.1.1/src/main/rhdzmota/utils/rsa_encryption.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/utils/runtime.py` & `rhdzmota-3.1.1/src/main/rhdzmota/utils/runtime.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota/wrappers/sentry.py` & `rhdzmota-3.1.1/src/main/rhdzmota/wrappers/sentry.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota.egg-info/PKG-INFO` & `rhdzmota-3.1.1/src/main/rhdzmota.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhdzmota
-Version: 3.1.0
+Version: 3.1.1
 Summary: RHDZMOTA Package
 Home-page: https://github.com/rhdzmota/package.rhdzmota.com
 Author: Rodrigo H. Mota
 Author-email: info@rhdzmota.com
 Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 Provides-Extra: baseline
```

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota.egg-info/SOURCES.txt` & `rhdzmota-3.1.1/src/main/rhdzmota.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 bin/rhdzmota
-src/main/rhdzmota/VERSION
 src/main/rhdzmota/__main__.py
 src/main/rhdzmota/celery.py
 src/main/rhdzmota/settings.py
+src/main/rhdzmota/version
+src/main/rhdzmota/version.py
 src/main/rhdzmota.egg-info/PKG-INFO
 src/main/rhdzmota.egg-info/SOURCES.txt
 src/main/rhdzmota.egg-info/dependency_links.txt
 src/main/rhdzmota.egg-info/entry_points.txt
 src/main/rhdzmota.egg-info/requires.txt
 src/main/rhdzmota.egg-info/top_level.txt
 src/main/rhdzmota/celery_workers/__init__.py
```

### Comparing `rhdzmota-3.1.0/src/main/rhdzmota.egg-info/requires.txt` & `rhdzmota-3.1.1/src/main/rhdzmota.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-pyyaml==6.0.1
-fire==0.4.0
-psutil==5.9.2
 requests==2.31.0
-rsa==4.8
-
-[all]
-typed-ast==1.5.4
-google-auth-oauthlib==0.5.3
-scalene==1.3.12
-jupyter==1.0.0
+fire==0.4.0
 rsa==4.8
 pyyaml==6.0.1
 psutil==5.9.2
+
+[all]
 pycodestyle==2.7.0
-google-api-python-client==2.63.0
-Flask==2.0.1
-fire==0.4.0
-ipython==7.34.0
-rhdzmota-extension-streamlit-webapps==0.5.0
+jupyter==1.0.0
 requests==2.31.0
-waitress==2.0.0
+fire==0.4.0
+flower==1.2.0
+pyyaml==6.0.1
+mypy-extensions==0.4.3
 PyJWT==2.3.0
-typing_extensions==4.3.0
-sentry-sdk==1.40.6
 mypy==0.971
-mypy-extensions==0.4.3
-rhdzmota-extension-hello-world==0.1.0
-flower==1.2.0
+typed-ast==1.5.4
+Flask==2.0.1
+rhdzmota-extension-hello-world<1.0.0,>=0.1.2
+psutil==5.9.2
 celery[redis]==5.1.2
+rhdzmota-extension-streamlit-webapps<1.0.0,>=0.5.1
+waitress==2.0.0
+rsa==4.8
+sentry-sdk==1.40.6
+scalene==1.3.12
+google-api-python-client==2.63.0
 oauth2client==4.1.3
+google-auth-oauthlib==0.5.3
+typing_extensions==4.3.0
+ipython==7.34.0
 
 [backend]
-Flask==2.0.1
-fire==0.4.0
+waitress==2.0.0
 requests==2.31.0
+fire==0.4.0
 rsa==4.8
-PyJWT==2.3.0
-waitress==2.0.0
-sentry-sdk==1.40.6
 pyyaml==6.0.1
+sentry-sdk==1.40.6
+PyJWT==2.3.0
+Flask==2.0.1
 psutil==5.9.2
 
 [baseline]
-pyyaml==6.0.1
-fire==0.4.0
-psutil==5.9.2
 requests==2.31.0
+fire==0.4.0
 rsa==4.8
+pyyaml==6.0.1
+psutil==5.9.2
 
 [celery]
-fire==0.4.0
 requests==2.31.0
-psutil==5.9.2
+fire==0.4.0
 rsa==4.8
-sentry-sdk==1.40.6
-pyyaml==6.0.1
 flower==1.2.0
+pyyaml==6.0.1
+sentry-sdk==1.40.6
+psutil==5.9.2
 celery[redis]==5.1.2
 
 [develop]
-typed-ast==1.5.4
 pycodestyle==2.7.0
-ipython==7.34.0
-fire==0.4.0
-scalene==1.3.12
-requests==2.31.0
 jupyter==1.0.0
+requests==2.31.0
+fire==0.4.0
 rsa==4.8
-typing_extensions==4.3.0
+pyyaml==6.0.1
 sentry-sdk==1.40.6
-mypy==0.971
+scalene==1.3.12
 mypy-extensions==0.4.3
-pyyaml==6.0.1
+mypy==0.971
+typed-ast==1.5.4
 psutil==5.9.2
+typing_extensions==4.3.0
+ipython==7.34.0
 
 [ext.hello_world]
-sentry-sdk==1.40.6
-rhdzmota-extension-hello-world==0.1.0
-pyyaml==6.0.1
+requests==2.31.0
 fire==0.4.0
 rsa==4.8
-requests==2.31.0
+rhdzmota-extension-hello-world<1.0.0,>=0.1.2
+pyyaml==6.0.1
 psutil==5.9.2
+sentry-sdk==1.40.6
 
 [ext.streamlit_webapps]
-fire==0.4.0
-rhdzmota-extension-streamlit-webapps==0.5.0
+rhdzmota-extension-streamlit-webapps<1.0.0,>=0.5.1
 requests==2.31.0
+fire==0.4.0
 rsa==4.8
 pyyaml==6.0.1
 psutil==5.9.2
 
 [google_services]
-google-auth-oauthlib==0.5.3
-google-api-python-client==2.63.0
-fire==0.4.0
 requests==2.31.0
+fire==0.4.0
 rsa==4.8
-sentry-sdk==1.40.6
 pyyaml==6.0.1
-psutil==5.9.2
+sentry-sdk==1.40.6
+google-api-python-client==2.63.0
 oauth2client==4.1.3
+psutil==5.9.2
+google-auth-oauthlib==0.5.3
 
 [standalone]
-sentry-sdk==1.40.6
-pyyaml==6.0.1
-fire==0.4.0
-psutil==5.9.2
 requests==2.31.0
+fire==0.4.0
 rsa==4.8
+pyyaml==6.0.1
+psutil==5.9.2
+sentry-sdk==1.40.6
 
 [tools]
-sentry-sdk==1.40.6
-pyyaml==6.0.1
+requests==2.31.0
 fire==0.4.0
 rsa==4.8
-requests==2.31.0
+pyyaml==6.0.1
 psutil==5.9.2
 PyJWT==2.3.0
+sentry-sdk==1.40.6
```

