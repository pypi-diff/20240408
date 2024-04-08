# Comparing `tmp/telegram_collector-0.1.0.tar.gz` & `tmp/telegram_collector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_collector-0.1.0.tar", last modified: Sun Apr  7 15:50:34 2024, max compression
+gzip compressed data, was "telegram_collector-0.1.1.tar", last modified: Mon Apr  8 10:33:37 2024, max compression
```

## Comparing `telegram_collector-0.1.0.tar` & `telegram_collector-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 15:50:34.992291 telegram_collector-0.1.0/
--rw-rw-rw-   0        0        0      287 2024-04-07 15:50:34.991274 telegram_collector-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-07 15:50:34.992291 telegram_collector-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      540 2024-04-07 15:48:31.000000 telegram_collector-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:50:34.979948 telegram_collector-0.1.0/telegram_collector/
--rw-rw-rw-   0        0        0     4947 2024-04-07 15:40:00.000000 telegram_collector-0.1.0/telegram_collector/__init__.py
--rw-rw-rw-   0        0        0     1893 2024-04-07 15:48:31.000000 telegram_collector-0.1.0/telegram_collector/__main__.py
--rw-rw-rw-   0        0        0     2560 2024-04-02 12:28:41.000000 telegram_collector-0.1.0/telegram_collector/util.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:50:34.990131 telegram_collector-0.1.0/telegram_collector.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-07 15:50:34.000000 telegram_collector-0.1.0/telegram_collector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-04-07 15:50:34.000000 telegram_collector-0.1.0/telegram_collector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 15:50:34.000000 telegram_collector-0.1.0/telegram_collector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-07 15:50:34.000000 telegram_collector-0.1.0/telegram_collector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-07 15:50:34.000000 telegram_collector-0.1.0/telegram_collector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-07 15:50:34.000000 telegram_collector-0.1.0/telegram_collector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 10:33:37.201979 telegram_collector-0.1.1/
+-rw-rw-rw-   0        0        0      287 2024-04-08 10:33:37.201979 telegram_collector-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-08 10:33:37.201979 telegram_collector-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      540 2024-04-08 10:33:34.000000 telegram_collector-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:33:37.191056 telegram_collector-0.1.1/telegram_collector/
+-rw-rw-rw-   0        0        0     4947 2024-04-07 15:40:00.000000 telegram_collector-0.1.1/telegram_collector/__init__.py
+-rw-rw-rw-   0        0        0     1893 2024-04-07 15:48:31.000000 telegram_collector-0.1.1/telegram_collector/__main__.py
+-rw-rw-rw-   0        0        0     2560 2024-04-02 12:28:41.000000 telegram_collector-0.1.1/telegram_collector/util.py
+drwxrwxrwx   0        0        0        0 2024-04-08 10:33:37.200980 telegram_collector-0.1.1/telegram_collector.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-04-08 10:33:37.000000 telegram_collector-0.1.1/telegram_collector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-04-08 10:33:37.000000 telegram_collector-0.1.1/telegram_collector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 10:33:37.000000 telegram_collector-0.1.1/telegram_collector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-08 10:33:37.000000 telegram_collector-0.1.1/telegram_collector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-08 10:33:37.000000 telegram_collector-0.1.1/telegram_collector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-08 10:33:37.000000 telegram_collector-0.1.1/telegram_collector.egg-info/top_level.txt
```

### Comparing `telegram_collector-0.1.0/setup.py` & `telegram_collector-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='telegram_collector',
-    version='0.1.0',
+    version='0.1.1',
     author='fengleicn',
     author_email='fengleisemail@gmail.com',
     url='https://github.com/fengleicn/telegram_collector',
     description=u'收集电报群组的视频图片消息',
     packages=['telegram_collector'],
     install_requires=['telethon', 'python_socks'],
     entry_points={
```

### Comparing `telegram_collector-0.1.0/telegram_collector/__init__.py` & `telegram_collector-0.1.1/telegram_collector/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_collector-0.1.0/telegram_collector/__main__.py` & `telegram_collector-0.1.1/telegram_collector/__main__.py`

 * *Files identical despite different names*

### Comparing `telegram_collector-0.1.0/telegram_collector/util.py` & `telegram_collector-0.1.1/telegram_collector/util.py`

 * *Files identical despite different names*

