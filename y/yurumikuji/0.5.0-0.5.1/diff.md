# Comparing `tmp/yurumikuji-0.5.0.tar.gz` & `tmp/yurumikuji-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yurumikuji-0.5.0.tar", last modified: Thu Apr  4 12:27:48 2024, max compression
+gzip compressed data, was "yurumikuji-0.5.1.tar", last modified: Mon Apr  8 13:54:54 2024, max compression
```

## Comparing `yurumikuji-0.5.0.tar` & `yurumikuji-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:27:48.637964 yurumikuji-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-04 12:27:40.000000 yurumikuji-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-04 12:27:48.637964 yurumikuji-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-04 12:27:40.000000 yurumikuji-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:27:48.637964 yurumikuji-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-04 12:27:40.000000 yurumikuji-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:27:48.637964 yurumikuji-0.5.0/yurumikuji/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-04 12:27:40.000000 yurumikuji-0.5.0/yurumikuji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-04 12:27:40.000000 yurumikuji-0.5.0/yurumikuji/yurumikuji.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:27:48.637964 yurumikuji-0.5.0/yurumikuji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-04 12:27:48.000000 yurumikuji-0.5.0/yurumikuji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-04 12:27:48.000000 yurumikuji-0.5.0/yurumikuji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:27:48.000000 yurumikuji-0.5.0/yurumikuji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 12:27:48.000000 yurumikuji-0.5.0/yurumikuji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 12:27:48.000000 yurumikuji-0.5.0/yurumikuji.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:54:54.453450 yurumikuji-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-08 13:54:44.000000 yurumikuji-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-08 13:54:54.453450 yurumikuji-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-08 13:54:44.000000 yurumikuji-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:54:54.453450 yurumikuji-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-08 13:54:44.000000 yurumikuji-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:54:54.449450 yurumikuji-0.5.1/yurumikuji/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-08 13:54:44.000000 yurumikuji-0.5.1/yurumikuji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-08 13:54:44.000000 yurumikuji-0.5.1/yurumikuji/yurumikuji.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:54:54.453450 yurumikuji-0.5.1/yurumikuji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-08 13:54:54.000000 yurumikuji-0.5.1/yurumikuji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 13:54:54.000000 yurumikuji-0.5.1/yurumikuji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:54:54.000000 yurumikuji-0.5.1/yurumikuji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 13:54:54.000000 yurumikuji-0.5.1/yurumikuji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 13:54:54.000000 yurumikuji-0.5.1/yurumikuji.egg-info/top_level.txt
```

### Comparing `yurumikuji-0.5.0/LICENSE` & `yurumikuji-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yurumikuji-0.5.0/PKG-INFO` & `yurumikuji-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yurumikuji
-Version: 0.5.0
+Version: 0.5.1
 Summary: kamidana(jinja2 cli) slack additonal.
 Home-page: https://github.com/srz-zumix/yurumikuji/
 Author: srz_zumix
 Author-email: zumix.cpp@gmail.com
 License: MIT
 Keywords: Slack,Jinja2
 Platform: any
```

### Comparing `yurumikuji-0.5.0/README.md` & `yurumikuji-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `yurumikuji-0.5.0/setup.py` & `yurumikuji-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `yurumikuji-0.5.0/yurumikuji/__init__.py` & `yurumikuji-0.5.1/yurumikuji/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = 'srz_zumix'
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 
 __copyright__ = '2021 %s ' % __author__
 __license__ = """
 The MIT License (MIT)
 
 Copyright (c) %s
```

### Comparing `yurumikuji-0.5.0/yurumikuji/yurumikuji.py` & `yurumikuji-0.5.1/yurumikuji/yurumikuji.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 load_dotenv()
 
 client = WebClient(token=os.environ['SLACK_TOKEN'])
 
 
 def on_error(e):
-    if os.environ['SLACK_API_ERROR_RAISE'].lower() == 'true':
+    if os.getenv('SLACK_API_ERROR_RAISE', 'false').lower() == 'true':
         raise e
     return e
 
 
 @as_filter
 def slack_user_id(v):
     try:
```

### Comparing `yurumikuji-0.5.0/yurumikuji.egg-info/PKG-INFO` & `yurumikuji-0.5.1/yurumikuji.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yurumikuji
-Version: 0.5.0
+Version: 0.5.1
 Summary: kamidana(jinja2 cli) slack additonal.
 Home-page: https://github.com/srz-zumix/yurumikuji/
 Author: srz_zumix
 Author-email: zumix.cpp@gmail.com
 License: MIT
 Keywords: Slack,Jinja2
 Platform: any
```

