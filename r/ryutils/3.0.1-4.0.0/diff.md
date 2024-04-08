# Comparing `tmp/ryutils-3.0.1.tar.gz` & `tmp/ryutils-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryutils-3.0.1.tar", last modified: Sun Mar 10 08:04:43 2024, max compression
+gzip compressed data, was "ryutils-4.0.0.tar", last modified: Mon Apr  8 06:35:47 2024, max compression
```

## Comparing `ryutils-3.0.1.tar` & `ryutils-4.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 08:04:43.404157 ryutils-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-10 08:04:38.000000 ryutils-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-10 08:04:38.000000 ryutils-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-03-10 08:04:43.404157 ryutils-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-10 08:04:38.000000 ryutils-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-10 08:04:38.000000 ryutils-3.0.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-10 08:04:38.000000 ryutils-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-10 08:04:38.000000 ryutils-3.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 08:04:43.400156 ryutils-3.0.1/ryutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/fmt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/short_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 08:04:43.404157 ryutils-3.0.1/ryutils/sms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/sms/telegram_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/sms/twilio_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-03-10 08:04:38.000000 ryutils-3.0.1/ryutils/web2_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 08:04:43.404157 ryutils-3.0.1/ryutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-03-10 08:04:43.000000 ryutils-3.0.1/ryutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-10 08:04:43.000000 ryutils-3.0.1/ryutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 08:04:43.000000 ryutils-3.0.1/ryutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-10 08:04:43.000000 ryutils-3.0.1/ryutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-10 08:04:43.000000 ryutils-3.0.1/ryutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 08:04:43.404157 ryutils-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-10 08:04:38.000000 ryutils-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:47.647941 ryutils-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 06:35:43.000000 ryutils-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 06:35:43.000000 ryutils-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-08 06:35:47.647941 ryutils-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 06:35:43.000000 ryutils-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 06:35:43.000000 ryutils-4.0.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-08 06:35:43.000000 ryutils-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-08 06:35:43.000000 ryutils-4.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:47.643941 ryutils-4.0.0/ryutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/fmt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/short_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:47.647941 ryutils-4.0.0/ryutils/sms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/sms/telegram_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/sms/twilio_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/web2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:47.647941 ryutils-4.0.0/ryutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-08 06:35:47.000000 ryutils-4.0.0/ryutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 06:35:47.000000 ryutils-4.0.0/ryutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:35:47.000000 ryutils-4.0.0/ryutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-08 06:35:47.000000 ryutils-4.0.0/ryutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 06:35:47.000000 ryutils-4.0.0/ryutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 06:35:47.647941 ryutils-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-08 06:35:43.000000 ryutils-4.0.0/setup.py
```

### Comparing `ryutils-3.0.1/LICENSE` & `ryutils-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ryutils-3.0.1/pyproject.toml` & `ryutils-4.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [tool.black]
 line-length = 100
-max-line-length = 100
-target-version = ['py38']
+target-version = ['py311']
 include = '\.pyi?$'
 # 'extend-exclude' excludes files or directories in addition to the defaults
 extend-exclude = '''
 # A regex preceded with ^/ will apply only to files and directories
 # in the root of the project.
 (
   ^/foo.py    # exclude a file named foo.py in the root of the project
```

### Comparing `ryutils-3.0.1/requirements.txt` & `ryutils-4.0.0/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,82 @@
-aiohttp==3.9.1
+aiohttp==3.9.3
 aiohttp-retry==2.8.3
 aiosignal==1.3.1
-anyio==4.2.0
-astroid==3.0.2
+anyio==4.3.0
+astroid==3.1.0
 attrs==23.2.0
+backports.tarfile==1.0.0
 beautifulsoup4==4.12.3
-black==23.12.1
-build==1.0.3
-cachetools==5.3.2
-certifi==2023.11.17
+black==24.3.0
+build==1.2.1
+cachetools==5.3.3
+certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 click==8.1.7
-cryptography==42.0.1
+cryptography==42.0.5
 cssselect==1.2.0
-cssutils==2.9.0
-dill==0.3.7
+cssutils==2.10.2
+dill==0.3.8
 docutils==0.20.1
 free_proxy==1.1.1
 frozenlist==1.4.1
-gevent==23.9.1
+gevent==24.2.1
 gitdb==4.0.11
 greenlet==3.0.3
 h11==0.14.0
-httpcore==1.0.2
-httpx==0.25.2
+httpcore==1.0.5
+httpx==0.27.0
 idna==3.6
-importlib-metadata==7.0.1
+importlib_metadata==7.1.0
 isort==5.13.2
-jaraco.classes==3.3.0
+jaraco.classes==3.4.0
+jaraco.context==5.3.0
+jaraco.functools==4.0.0
 jeepney==0.8.0
-keyring==24.3.0
-lxml==5.1.0
+keyring==25.1.0
+lxml==5.2.1
 markdown-it-py==3.0.0
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==10.2.0
-multidict==6.0.4
-mypy==1.8.0
+multidict==6.0.5
+mypy==1.9.0
 mypy-extensions==1.0.0
-nh3==0.2.15
-packaging==23.2
+nh3==0.2.17
+packaging==24.0
 pathspec==0.12.1
-peewee==3.17.0
-pkginfo==1.9.6
-platformdirs==4.1.0
+peewee==3.17.1
+pkginfo==1.10.0
+platformdirs==4.2.0
 premailer==3.10.0
-pycparser==2.21
+pycparser==2.22
 Pygments==2.17.2
 PyJWT==2.8.0
-pylint==3.0.3
+pylint==3.1.0
 pyproject_hooks==1.0.0
 pyshorteners==1.0.1
-python-telegram-bot==20.7
-pytz==2023.3.post1
-readme-renderer==42.0
+python-telegram-bot==21.0.1
+pytz==2024.1
+readme_renderer==43.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
-rich==13.7.0
+rich==13.7.1
 SecretStorage==3.3.3
 six==1.16.0
 smmap==5.0.1
-sniffio==1.3.0
+sniffio==1.3.1
 soupsieve==2.5
 termcolor==2.4.0
-tomlkit==0.12.3
-twilio==8.12.0
-twine==4.0.2
-types-pytz==2023.3.1.1
-typing_extensions==4.9.0
-urllib3==2.1.0
+tomlkit==0.12.4
+twilio==9.0.4
+twine==5.0.0
+types-pytz==2024.1.0.20240203
+typing_extensions==4.11.0
+urllib3==2.2.1
 yagmail==0.15.293
 yarl==1.9.4
 yaspin==3.0.1
-zipp==3.17.0
+zipp==3.18.1
 zope.event==5.0
-zope.interface==6.1
+zope.interface==6.2
```

### Comparing `ryutils-3.0.1/ryutils/async_utils.py` & `ryutils-4.0.0/ryutils/async_utils.py`

 * *Files identical despite different names*

### Comparing `ryutils-3.0.1/ryutils/csv_logger.py` & `ryutils-4.0.0/ryutils/csv_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Utility script that helps write transactions to a spreadsheet
 """
+
 import csv
 import json
 import os
 import typing as T
 
 from ryutils import log
```

### Comparing `ryutils-3.0.1/ryutils/dict_util.py` & `ryutils-4.0.0/ryutils/dict_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-3.0.1/ryutils/email_util.py` & `ryutils-4.0.0/ryutils/email_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-3.0.1/ryutils/fmt_util.py` & `ryutils-4.0.0/ryutils/fmt_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-3.0.1/ryutils/log.py` & `ryutils-4.0.0/ryutils/log.py`

 * *Files identical despite different names*

### Comparing `ryutils-3.0.1/ryutils/proxies.py` & `ryutils-4.0.0/ryutils/proxies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Get proxies from various sources.
 """
+
 import typing as T
 
 from fp.fp import FreeProxy
 
 from ryutils import log
```

### Comparing `ryutils-3.0.1/ryutils/sms/telegram_util.py` & `ryutils-4.0.0/ryutils/sms/telegram_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-3.0.1/ryutils/sms/twilio_util.py` & `ryutils-4.0.0/ryutils/sms/twilio_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-3.0.1/ryutils/web2_client.py` & `ryutils-4.0.0/ryutils/web2_client.py`

 * *Files identical despite different names*

### Comparing `ryutils-3.0.1/ryutils.egg-info/SOURCES.txt` & `ryutils-4.0.0/ryutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryutils-3.0.1/setup.py` & `ryutils-4.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 from setuptools import find_packages, setup
 
 required = []
-with open("requirements.txt", encoding="utf-8") as infile:
-    required = infile.read().splitlines()
+
+# with open("requirements.txt", encoding="utf-8") as infile:
+#     required = infile.read().splitlines()
+
+required += [
+    "free_proxy>=1.1.1",
+    "pyshorteners>=1.0.1",
+    "python-telegram-bot>=21.0.1",
+    "pytz>=2024.1",
+    "requests>=2.31.0",
+    "twilio>=9.0.4",
+    "yagmail>=0.15.293",
+    "yaspin>=3.0.1",
+]
 
 LONG_DESCRIPTION = ""
 with open("README.md", encoding="utf-8") as infile:
     LONG_DESCRIPTION = infile.read()
 
 VERSION = "0.0.0"
 with open("VERSION", encoding="utf-8") as infile:
@@ -24,12 +36,10 @@
     package_data={"ryutils": ["py.typed"]},
     install_requires=required,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

