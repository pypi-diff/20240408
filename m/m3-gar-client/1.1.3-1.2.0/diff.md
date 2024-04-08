# Comparing `tmp/m3-gar-client-1.1.3.tar.gz` & `tmp/m3-gar-client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3-gar-client-1.1.3.tar", last modified: Mon Apr  1 12:01:59 2024, max compression
+gzip compressed data, was "m3-gar-client-1.2.0.tar", last modified: Mon Apr  8 12:22:17 2024, max compression
```

## Comparing `m3-gar-client-1.1.3.tar` & `m3-gar-client-1.2.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.302293 m3-gar-client-1.1.3/
--rw-r--r--   0 toor      (1000) toor      (1000)      565 2021-10-28 11:22:58.000000 m3-gar-client-1.1.3/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      153 2021-10-28 11:22:58.000000 m3-gar-client-1.1.3/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     5666 2024-04-01 12:01:59.301293 m3-gar-client-1.1.3/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     4056 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.286293 m3-gar-client-1.1.3/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)      497 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/requirements/_base.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       13 2021-10-28 11:22:58.000000 m3-gar-client-1.1.3/requirements/prod.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-04-01 12:01:59.302293 m3-gar-client-1.1.3/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2795 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.284293 m3-gar-client-1.1.3/src/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.287293 m3-gar-client-1.1.3/src/m3_gar_client/
--rw-r--r--   0 toor      (1000) toor      (1000)     1163 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      446 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/apps.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.290293 m3-gar-client-1.1.3/src/m3_gar_client/backends/
--rw-r--r--   0 toor      (1000) toor      (1000)       70 2021-10-28 11:22:58.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5336 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/base.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.291293 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/
--rw-r--r--   0 toor      (1000) toor      (1000)      127 2021-10-28 11:22:58.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4925 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/base.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.292293 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy/
--rw-r--r--   0 toor      (1000) toor      (1000)     2043 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4244 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy/actions.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.294293 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/
--rw-r--r--   0 toor      (1000) toor      (1000)     1762 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      480 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/authentication.py
--rw-r--r--   0 toor      (1000) toor      (1000)      198 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/const.py
--rw-r--r--   0 toor      (1000) toor      (1000)      694 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/urls.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3310 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/views.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9941 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/server.py
--rw-r--r--   0 toor      (1000) toor      (1000)    34905 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)    24834 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/data.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.294293 m3-gar-client-1.1.3/src/m3_gar_client/management/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 09:04:10.000000 m3-gar-client-1.1.3/src/m3_gar_client/management/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.295293 m3-gar-client-1.1.3/src/m3_gar_client/management/commands/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 09:04:10.000000 m3-gar-client-1.1.3/src/m3_gar_client/management/commands/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      454 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/management/commands/clear_gar_cache.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.283293 m3-gar-client-1.1.3/src/m3_gar_client/static/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.283293 m3-gar-client-1.1.3/src/m3_gar_client/static/m3/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.283293 m3-gar-client-1.1.3/src/m3_gar_client/static/m3/js/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.295293 m3-gar-client-1.1.3/src/m3_gar_client/static/m3/js/gar/
--rw-r--r--   0 toor      (1000) toor      (1000)    37035 2024-03-18 09:04:10.000000 m3-gar-client-1.1.3/src/m3_gar_client/static/m3/js/gar/AddressPanel.js
--rw-r--r--   0 toor      (1000) toor      (1000)     6454 2024-03-18 09:04:10.000000 m3-gar-client-1.1.3/src/m3_gar_client/static/m3/js/gar/AddressPanelPatch.js
--rw-r--r--   0 toor      (1000) toor      (1000)    27594 2024-03-30 11:52:02.000000 m3-gar-client-1.1.3/src/m3_gar_client/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)    12473 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/m3_gar_client/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.299293 m3-gar-client-1.1.3/src/m3_gar_client.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     5666 2024-04-01 12:01:59.000000 m3-gar-client-1.1.3/src/m3_gar_client.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     1636 2024-04-01 12:01:59.000000 m3-gar-client-1.1.3/src/m3_gar_client.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       43 2024-04-01 12:01:59.000000 m3-gar-client-1.1.3/src/m3_gar_client.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      177 2024-04-01 12:01:59.000000 m3-gar-client-1.1.3/src/m3_gar_client.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       14 2024-04-01 12:01:59.000000 m3-gar-client-1.1.3/src/m3_gar_client.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.297293 m3-gar-client-1.1.3/src/testapp/
--rw-r--r--   0 toor      (1000) toor      (1000)       50 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/testapp/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      399 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/testapp/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)      401 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/testapp/asgi.py
--rwxr-xr-x   0 toor      (1000) toor      (1000)      688 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/testapp/manage.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3498 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/testapp/settings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:59.298293 m3-gar-client-1.1.3/src/testapp/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/testapp/tests/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2090 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/testapp/tests/test_backend_responses.py
--rw-r--r--   0 toor      (1000) toor      (1000)      988 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/testapp/tests/test_defaults.py
--rw-r--r--   0 toor      (1000) toor      (1000)      768 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/testapp/urls.py
--rw-r--r--   0 toor      (1000) toor      (1000)      401 2024-04-01 12:01:53.000000 m3-gar-client-1.1.3/src/testapp/wsgi.py
--rw-r--r--   0 toor      (1000) toor      (1000)      448 2024-04-01 12:01:59.000000 m3-gar-client-1.1.3/version.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.469910 m3-gar-client-1.2.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)      565 2021-10-28 11:22:58.000000 m3-gar-client-1.2.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      153 2021-10-28 11:22:58.000000 m3-gar-client-1.2.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     5666 2024-04-08 12:22:17.468910 m3-gar-client-1.2.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     4056 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.448910 m3-gar-client-1.2.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)      497 2024-04-08 12:22:13.000000 m3-gar-client-1.2.0/requirements/_base.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       13 2021-10-28 11:22:58.000000 m3-gar-client-1.2.0/requirements/prod.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-04-08 12:22:17.469910 m3-gar-client-1.2.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2795 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.445910 m3-gar-client-1.2.0/src/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.450910 m3-gar-client-1.2.0/src/m3_gar_client/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1163 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      446 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/apps.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.453910 m3-gar-client-1.2.0/src/m3_gar_client/backends/
+-rw-r--r--   0 toor      (1000) toor      (1000)       70 2021-10-28 11:22:58.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5336 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/base.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.455910 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/
+-rw-r--r--   0 toor      (1000) toor      (1000)      127 2021-10-28 11:22:58.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4925 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/base.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.455910 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy/
+-rw-r--r--   0 toor      (1000) toor      (1000)     2043 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5401 2024-04-08 12:22:13.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy/actions.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.457910 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1762 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      480 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/authentication.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      198 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      694 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/urls.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3450 2024-04-08 12:22:13.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/views.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9941 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/server.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    36778 2024-04-08 12:22:13.000000 m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      725 2024-04-08 12:22:13.000000 m3-gar-client-1.2.0/src/m3_gar_client/const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    24834 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/data.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.457910 m3-gar-client-1.2.0/src/m3_gar_client/management/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 09:04:10.000000 m3-gar-client-1.2.0/src/m3_gar_client/management/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.458910 m3-gar-client-1.2.0/src/m3_gar_client/management/commands/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 09:04:10.000000 m3-gar-client-1.2.0/src/m3_gar_client/management/commands/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      454 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/management/commands/clear_gar_cache.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.440910 m3-gar-client-1.2.0/src/m3_gar_client/static/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.440910 m3-gar-client-1.2.0/src/m3_gar_client/static/m3/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.440910 m3-gar-client-1.2.0/src/m3_gar_client/static/m3/js/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.460910 m3-gar-client-1.2.0/src/m3_gar_client/static/m3/js/gar/
+-rw-r--r--   0 toor      (1000) toor      (1000)    37035 2024-03-18 09:04:10.000000 m3-gar-client-1.2.0/src/m3_gar_client/static/m3/js/gar/AddressPanel.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     6454 2024-03-18 09:04:10.000000 m3-gar-client-1.2.0/src/m3_gar_client/static/m3/js/gar/AddressPanelPatch.js
+-rw-r--r--   0 toor      (1000) toor      (1000)    28471 2024-04-08 12:22:13.000000 m3-gar-client-1.2.0/src/m3_gar_client/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    12473 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/m3_gar_client/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.467910 m3-gar-client-1.2.0/src/m3_gar_client.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5666 2024-04-08 12:22:17.000000 m3-gar-client-1.2.0/src/m3_gar_client.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1663 2024-04-08 12:22:17.000000 m3-gar-client-1.2.0/src/m3_gar_client.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       43 2024-04-08 12:22:17.000000 m3-gar-client-1.2.0/src/m3_gar_client.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      177 2024-04-08 12:22:17.000000 m3-gar-client-1.2.0/src/m3_gar_client.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       14 2024-04-08 12:22:17.000000 m3-gar-client-1.2.0/src/m3_gar_client.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.464910 m3-gar-client-1.2.0/src/testapp/
+-rw-r--r--   0 toor      (1000) toor      (1000)       50 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/testapp/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      399 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/testapp/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      401 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/testapp/asgi.py
+-rwxr-xr-x   0 toor      (1000) toor      (1000)      688 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/testapp/manage.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3498 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/testapp/settings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-08 12:22:17.465910 m3-gar-client-1.2.0/src/testapp/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/testapp/tests/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2090 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/testapp/tests/test_backend_responses.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      988 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/testapp/tests/test_defaults.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      768 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/testapp/urls.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      401 2024-04-01 12:01:53.000000 m3-gar-client-1.2.0/src/testapp/wsgi.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      448 2024-04-08 12:22:17.000000 m3-gar-client-1.2.0/version.conf
```

### Comparing `m3-gar-client-1.1.3/LICENSE` & `m3-gar-client-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/PKG-INFO` & `m3-gar-client-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3-gar-client
-Version: 1.1.3
+Version: 1.2.0
 Summary: UI клиент для сервера ГАР m3-rest-gar
 Home-page: https://stash.bars-open.ru/projects/M3/repos/m3-gar-client
 Author: BARS Group
 Author-email: bars@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
@@ -26,15 +26,15 @@
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests<3,>=2
 Requires-Dist: django<5.1,>=2.2
-Requires-Dist: m3-gar-constants>=1.0.3
+Requires-Dist: m3-gar-constants>=1.0.4
 Provides-Extra: oauth2
 Requires-Dist: oauthlib<3.3,>=2; extra == "oauth2"
 Requires-Dist: requests-oauthlib<=1.3.1; extra == "oauth2"
 Provides-Extra: m3
 Requires-Dist: m3-core<4,>=2.2.16; extra == "m3"
 Requires-Dist: m3-ui<3,>=2.0.8; extra == "m3"
 Provides-Extra: rest
```

### Comparing `m3-gar-client-1.1.3/README.rst` & `m3-gar-client-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/setup.py` & `m3-gar-client-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/__init__.py` & `m3-gar-client-1.2.0/src/m3_gar_client/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/backends/base.py` & `m3-gar-client-1.2.0/src/m3_gar_client/backends/base.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/base.py` & `m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/base.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy/__init__.py` & `m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/__init__.py` & `m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/urls.py` & `m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/urls.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/views.py` & `m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,16 +72,19 @@
     )
 
     # Признак того, что необходимо корректировать пользовательский ввод
     correct_keyboard_input = True
     loader_cls: Type[LoaderBase]
 
     def post(self, request):
+        result = self._get_loader(request).load()
+
         return self._build_response(
-            self._get_loader(request).load()
+            data=result.rows,
+            total=result.total,
         )
 
     def _get_loader(self, request):
         """Возвращает инстанс загрузчика данных."""
         args, kwargs = self._get_loader_params(request)
         return self.loader_cls(*args, **kwargs)
 
@@ -89,18 +92,18 @@
         filter_ = request.POST.get('filter', '')
 
         if self.correct_keyboard_input and filter_:
             filter_ = correct_keyboard_layout(filter_)
 
         return (filter_, ), {}
 
-    def _build_response(self, data):
+    def _build_response(self, data, total):
         return Response({
             'rows': data,
-            'total': len(data)
+            'total': total,
         })
 
 
 class ParentSearchMixin(AbstractSearchView):
     def _get_loader_params(self, request):
         args, kwargs = super()._get_loader_params(request)
         kwargs.update(parent_id=request.POST['parent'])
@@ -125,15 +128,18 @@
 
 class HouseOrSteadSearchView(ParentSearchMixin, AbstractSearchView):
 
     correct_keyboard_input = False
     loader_cls = UIHouseOrSteadLoader
 
     def post(self, request):
+        result = self._get_loader(request).load()
+
         return self._build_response(
-            self._get_loader(request).load()
+            data=result.rows,
+            total=result.total,
         )
 
 
 class ApartmentSearchView(ParentSearchMixin, AbstractSearchView):
     correct_keyboard_input = False
     loader_cls = UIApartmentLoader
```

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/server.py` & `m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/server.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/backends/m3_rest_gar/utils.py` & `m3-gar-client-1.2.0/src/m3_gar_client/backends/m3_rest_gar/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,21 @@
     ABC,
     abstractmethod,
 )
 from itertools import (
     chain,
     count,
 )
+from typing import (
+    Generator,
+    List,
+    NamedTuple,
+    Optional,
+    Tuple,
+)
 
 from m3_gar_constants import (
     DEFAULT_PAGE_LIMIT,
     GAR_HIERARCHY_MUN,
     GAR_LEVELS_PLACE,
     GAR_LEVELS_STREET,
 )
@@ -268,14 +275,20 @@
         'displayName': _get_display_name,
     }
 
 
 # -----------------------------------------------------------------------------
 # Загрузчики данных с сервера m3-rest-gar.
 
+class LoaderResult(NamedTuple):
+    """Результат загрузки данных."""
+
+    rows: List[dict]
+    total: int
+
 
 class LoaderBase(ABC):
     """Базовый класс для загрузчиков объектов ГАР.
 
     Attributes:
         filter_string: Строка для фильтрации объектов.
         timeout: Timeout запросов к серверу ГАР в секундах.
@@ -354,48 +367,75 @@
 
         result = {
             filter_param: self.filter_string,
         }
 
         return result
 
-    def load_raw(self, page=None):
+    def load_raw_page(self, page_number: int, params: Optional[dict] = None) -> Tuple[Generator, bool, int]:
+        """Возвращает данные конкретной страницы адресных объектов в исходном виде.
+
+        Также возвращает признак наличия следующей страницы с данными и общее число найденных объектов.
+        """
+        if params is None:
+            params = self._get_params()
+
+        results = ()
+        total_count = 0
+        has_next_page = False
+
+        drf_data = self._load_page(params, page_number)
+
+        if drf_data:
+            total_count = drf_data['count']
+            results = drf_data['results']
+            has_next_page = drf_data.get('next') or False
+
+        result_data = (
+            object_data
+            for object_data in (self._process_object_data(drf_data) for drf_data in results)
+            if self._filter(object_data)
+        )
+
+        return result_data, has_next_page, total_count
+
+    def load_raw(self, page: Optional[int] = None) -> Generator:
         """Возвращает данные адресных объектов в исходном виде.
 
         Args:
             page: Номера страницы для загрузки данных. ``None`` указывает на необходимость загрузки всех страниц.
         """
 
         from django.conf import (
             settings,
         )
 
-        # Значение PAGE_LIMIT по умолчанию 5. С большим PAGE_LIMIT можно заддосить ГАР
         page_limit = settings.GAR.get('PAGE_LIMIT', DEFAULT_PAGE_LIMIT)
 
         if page is None:
             pages = count(start=1)
         else:
             pages = range(page, page + 1)
 
         params = self._get_params()
 
         for page_number in pages:
-            drf_data = self._load_page(params, page_number)
-            if drf_data:
-                for drf_object_data in drf_data['results']:
-                    object_data = self._process_object_data(drf_object_data)
-                    if self._filter(object_data):
-                        yield object_data
+            result_data, has_next_page, total_count = self.load_raw_page(page_number, params)
 
-                if not drf_data['next'] or page_number >= page_limit:
-                    break
-            else:
+            yield from result_data
+
+            if not has_next_page or page_number >= page_limit:
                 break
 
+    def load_page_results(self, page_number: int) -> Tuple[Generator, int]:
+        """Возвращает данные в соответствии с параметрами загрузчика по указанной странице."""
+        result_data, _, total_count = self.load_raw_page(page_number)
+
+        return (self._build_result(data) for data in result_data), total_count
+
     def load_results(self, page=None):
         """Возвращает данные в соответствии с параметрами загрузчика.
 
         Args:
             page: Номера страницы для загрузки данных. ``None`` указывает на необходимость загрузки всех страниц.
         """
 
@@ -414,25 +454,30 @@
 
         Args:
             data: Кортеж словарей с данными загруженных объектов ГАР.
         """
 
         return sorted(data, key=self._sort_key)
 
-    def load(self, page=None):
+    def load(self, page: Optional[int] = None) -> LoaderResult:
         """Загружает данные с сервера ГАР.
 
         Args:
             page: Номера страницы для загрузки данных. ``None`` указывает на необходимость загрузки всех страниц.
         """
+        if page is None:
+            data = self.load_results()
+            total = None
+        else:
+            data, total = self.load_page_results(page)
 
-        data = tuple(self.load_results(page))
-        result = self._process_result(data)
+        rows = self._process_result(data)
+        total = total or len(rows)
 
-        return result
+        return LoaderResult(rows=rows, total=total)
 
 
 class ParentFilterMixin:
     """Миксин для загрузчиков, которые используют id родительского объекта в запросах к серверу ГАР."""
 
     @property
     @abstractmethod
@@ -785,19 +830,23 @@
 
     """Фасад для загрузки домов и участков."""
 
     def __init__(self, *args, **kwargs):
         self._house_loader = UIHouseLoader(*args, **kwargs)
         self._stead_loader = UISteadLoader(*args, **kwargs)
 
-    def load(self, page=None):
-        return list((
-            *self._house_loader.load(page=page),
-            *self._stead_loader.load(page=page)
-        ))
+    def load(self, page: Optional[int] = None) -> LoaderResult:
+        house_result = self._house_loader.load(page=page)
+        stead_result = self._stead_loader.load(page=page)
+        total = house_result.total + stead_result.total
+
+        return LoaderResult(
+            rows=list(chain(house_result.rows, stead_result.rows)),
+            total=total,
+        )
 
 
 class UIApartmentLoader(ApartmentLoader):
 
     _mapper_class = UIApartmentMapper
 
 
@@ -814,25 +863,25 @@
 
     Returns:
         Адресный объект
 
     Exceptions:
         requests.ConnectionError: если не удалось соединиться с сервером ГАР
     """
-    result = None
+    address_object = None
 
     if obj_id:
         response = server.get('/addrobj/{}/'.format(obj_id), timeout=timeout)
 
         if response and response.status_code == http_client.OK:
             response_data = response.json()
             mapped_data = map_object_data(AddressObjectMapper, response_data)
-            result = AddressObject(**mapped_data)
+            address_object = AddressObject(**mapped_data)
 
-    return result
+    return address_object
 
 
 def find_address_objects(
     filter_string,
     levels=None,
     typenames=None,
     parent_id=None,
@@ -871,19 +920,19 @@
     assert stead_id is not None
 
     response = server.get('/steads/{}/'.format(stead_id), timeout=timeout)
 
     if response and response.status_code == http_client.OK:
         response_data = response.json()
         mapped_data = map_object_data(SteadMapper, response_data)
-        result = Stead(**mapped_data)
+        stead = Stead(**mapped_data)
     else:
-        result = None
+        stead = None
 
-    return result
+    return stead
 
 
 def get_house(house_id, timeout=None):
     """Возвращает информацию о здании по его ID в ГАР.
 
     Args:
         house_id: ID здания.
@@ -911,57 +960,61 @@
         house_number: Номер дома.
         parent_id: ID родительского объекта.
         building_number: Номер корпуса.
         structure_number: Номер строения.
         timeout: Timeout запросов к серверу ГАР в секундах.
     """
 
-    houses = HouseLoader(
+    result = HouseLoader(
         house_number,
         parent_id=parent_id,
         exact=True,
         timeout=timeout,
     ).load()
 
+    houses = result.rows
+
     if len(houses) > 1:
         _filter = lambda house: (
             house['building_number'] == building_number and
             house['structure_number'] == structure_number
         )
         houses = list(filter(_filter, houses))
 
     if len(houses) == 1:
-        result = House(**houses[0])
+        house = House(**houses[0])
     else:
-        result = None
+        house = None
 
-    return result
+    return house
 
 
 def find_stead(number='', parent_id=None, timeout=None):
     """Возвращает информацию об участке по его номеру.
 
     :param str number: Номер участка.
     :param parent_id: ID родительского объекта.
     :param float timeout: Timeout запросов к серверу ГАР в секундах.
 
     :rtype: m3_gar_client.data.Stead or NoneType
     """
-    steads = SteadLoader(
+    result = SteadLoader(
         number,
         parent_id=parent_id,
         timeout=timeout,
     ).load()
 
+    steads = result.rows
+
     if len(steads) == 1:
-        result = Stead(**steads[0])
+        stead = Stead(**steads[0])
     else:
-        result = None
+        stead = None
 
-    return result
+    return stead
 
 
 def get_apartment(apartment_id, timeout=None):
     """Возвращает информацию о помещении по его ID в ГАР.
 
     Args:
         apartment_id: ID помещения.
@@ -970,43 +1023,45 @@
     assert apartment_id is not None
 
     response = server.get('/apartments/{}/'.format(apartment_id), timeout=timeout)
 
     if response and response.status_code == http_client.OK:
         response_data = response.json()
         mapped_data = map_object_data(ApartmentMapper, response_data)
-        result = Apartment(**mapped_data)
+        apartment = Apartment(**mapped_data)
     else:
-        result = None
+        apartment = None
 
-    return result
+    return apartment
 
 
 def find_apartment(number='', parent_id=None, timeout=None):
     """Возвращает информацию о помещении по его номеру.
 
     Args:
         number: Номер квартиры.
         parent_id: ID родительского объекта.
         timeout: Timeout запросов к серверу ГАР в секундах.
     """
 
-    apartments = ApartmentLoader(
+    result = ApartmentLoader(
         number,
         parent_id=parent_id,
         exact=True,
         timeout=timeout,
     ).load()
 
+    apartments = result.rows
+
     if len(apartments) == 1:
-        result = Apartment(**apartments[0])
+        apartment = Apartment(**apartments[0])
     else:
-        result = None
+        apartment = None
 
-    return result
+    return apartment
 
 
 def flatten_object_data(raw_object_data):
     """Преобразует данные объекта ГАР к "плоскому" виду.
 
     Args:
         raw_object_data: Необработанные данные объекта ГАР, полученные с сервера m3-rest-gar.
```

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/data.py` & `m3-gar-client-1.2.0/src/m3_gar_client/data.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/static/m3/js/gar/AddressPanel.js` & `m3-gar-client-1.2.0/src/m3_gar_client/static/m3/js/gar/AddressPanel.js`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/static/m3/js/gar/AddressPanelPatch.js` & `m3-gar-client-1.2.0/src/m3_gar_client/static/m3/js/gar/AddressPanelPatch.js`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/ui.py` & `m3-gar-client-1.2.0/src/m3_gar_client/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import json
 import warnings
 
+from django.conf import (
+    settings,
+)
 from m3_ext.ui.base import (
     BaseExtComponent,
 )
 from m3_ext.ui.containers.containers import (
     ExtContainer,
 )
 from m3_ext.ui.fields.simple import (
@@ -13,22 +16,28 @@
     ExtStringField,
     ExtTextArea,
 )
 from m3_ext.ui.misc.store import (
     ExtJsonStore,
 )
 from m3_gar_constants import (
+    RESULT_PAGE_SIZE,
     UI_LEVEL_FLAT,
     UI_LEVEL_HOUSE,
     UI_LEVEL_PLACE,
     UI_LEVEL_STREET,
     UI_LEVELS,
 )
 
 import m3_gar_client
+from m3_gar_client.const import (
+    DEFAULT_FIELD_IS_PAGINATED,
+    DEFAULT_FIELD_MIN_CHARS,
+    DEFAULT_FIELD_QUERY_DELAY_MS,
+)
 from m3_gar_client.data import (
     ObjectDictAdapter,
     ObjectMapper,
 )
 from m3_gar_client.utils import (
     cached_property,
     get_address_object,
@@ -177,15 +186,15 @@
             name=self._names_of_fields['place_name'],
             label=self._labels_text['place_name'],
             display_field='fullName',
             value_field='fullName',
             query_param='filter',
             hide_trigger=True,
             force_selection=self.gar_only,
-            min_chars=2,
+            min_chars=settings.GAR.get('FIELD_MIN_CHARS', DEFAULT_FIELD_MIN_CHARS),
             empty_text='Название субъекта/города/населенного пункта/ЭПС',
             read_only=self.read_only,
             allow_blank=self.allow_blank,
             list_width=1000,
             fields=[
                 'objectId',
                 'level',
@@ -197,14 +206,22 @@
                 url=self.backend.place_search_url,
                 id_property='objectId',
                 root='rows',
                 total_property='total',
             ),
         )
 
+        if settings.GAR.get('FIELD_IS_PAGINATED', DEFAULT_FIELD_IS_PAGINATED):
+            result.page_size = RESULT_PAGE_SIZE
+
+        result._put_config_value(
+            'queryDelay',
+            settings.GAR.get('FIELD_QUERY_DELAY_MS', DEFAULT_FIELD_QUERY_DELAY_MS)
+        )
+
         self.backend.configure_place_field(result)
 
         return result
 
     @cached_property
     def field__place_id(self):
         """Поле для хранения ID населенного пункта.
@@ -242,15 +259,15 @@
             name=self._names_of_fields['street_name'],
             label=self._labels_text['street_name'],
             display_field='name',
             value_field='name',
             query_param='filter',
             hide_trigger=True,
             force_selection=self.gar_only,
-            min_chars=2,
+            min_chars=settings.GAR.get('FIELD_MIN_CHARS', DEFAULT_FIELD_MIN_CHARS),
             empty_text='Название улицы/микрорайона',
             read_only=self.read_only,
             fields=[
                 'objectId',
                 'level',
                 'shortName',
                 'typeFullName',
@@ -264,14 +281,22 @@
                 root='rows',
                 total_property='total',
             ),
         )
 
         self.backend.configure_street_field(result)
 
+        if settings.GAR.get('FIELD_IS_PAGINATED', DEFAULT_FIELD_IS_PAGINATED):
+            result.page_size = RESULT_PAGE_SIZE
+
+        result._put_config_value(
+            'queryDelay',
+            settings.GAR.get('FIELD_QUERY_DELAY_MS', DEFAULT_FIELD_QUERY_DELAY_MS)
+        )
+
         return result
 
     @cached_property
     def field__street_id(self):
         """Поле для хранения ID улицы.
 
         :rtype: m3_ext.ui.fields.simple.ExtHiddenField
```

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client/utils.py` & `m3-gar-client-1.2.0/src/m3_gar_client/utils.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client.egg-info/PKG-INFO` & `m3-gar-client-1.2.0/src/m3_gar_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3-gar-client
-Version: 1.1.3
+Version: 1.2.0
 Summary: UI клиент для сервера ГАР m3-rest-gar
 Home-page: https://stash.bars-open.ru/projects/M3/repos/m3-gar-client
 Author: BARS Group
 Author-email: bars@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
@@ -26,15 +26,15 @@
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests<3,>=2
 Requires-Dist: django<5.1,>=2.2
-Requires-Dist: m3-gar-constants>=1.0.3
+Requires-Dist: m3-gar-constants>=1.0.4
 Provides-Extra: oauth2
 Requires-Dist: oauthlib<3.3,>=2; extra == "oauth2"
 Requires-Dist: requests-oauthlib<=1.3.1; extra == "oauth2"
 Provides-Extra: m3
 Requires-Dist: m3-core<4,>=2.2.16; extra == "m3"
 Requires-Dist: m3-ui<3,>=2.0.8; extra == "m3"
 Provides-Extra: rest
```

### Comparing `m3-gar-client-1.1.3/src/m3_gar_client.egg-info/SOURCES.txt` & `m3-gar-client-1.2.0/src/m3_gar_client.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.rst
 setup.py
 version.conf
 requirements/_base.txt
 requirements/prod.txt
 src/m3_gar_client/__init__.py
 src/m3_gar_client/apps.py
+src/m3_gar_client/const.py
 src/m3_gar_client/data.py
 src/m3_gar_client/ui.py
 src/m3_gar_client/utils.py
 src/m3_gar_client.egg-info/PKG-INFO
 src/m3_gar_client.egg-info/SOURCES.txt
 src/m3_gar_client.egg-info/dependency_links.txt
 src/m3_gar_client.egg-info/requires.txt
```

### Comparing `m3-gar-client-1.1.3/src/testapp/manage.py` & `m3-gar-client-1.2.0/src/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/testapp/settings.py` & `m3-gar-client-1.2.0/src/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/testapp/tests/test_backend_responses.py` & `m3-gar-client-1.2.0/src/testapp/tests/test_backend_responses.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/testapp/tests/test_defaults.py` & `m3-gar-client-1.2.0/src/testapp/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.3/src/testapp/urls.py` & `m3-gar-client-1.2.0/src/testapp/urls.py`

 * *Files identical despite different names*

