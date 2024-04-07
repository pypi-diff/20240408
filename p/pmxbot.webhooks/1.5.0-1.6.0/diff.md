# Comparing `tmp/pmxbot.webhooks-1.5.0.tar.gz` & `tmp/pmxbot.webhooks-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmxbot.webhooks-1.5.0.tar", last modified: Wed Apr  3 00:50:39 2024, max compression
+gzip compressed data, was "pmxbot.webhooks-1.6.0.tar", last modified: Sun Apr  7 22:31:11 2024, max compression
```

## Comparing `pmxbot.webhooks-1.5.0.tar` & `pmxbot.webhooks-1.6.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.579632 pmxbot.webhooks-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.571632 pmxbot.webhooks-1.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.571632 pmxbot.webhooks-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-03 00:50:39.579632 pmxbot.webhooks-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.575632 pmxbot.webhooks-1.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.575632 pmxbot.webhooks-1.5.0/pmxbot/
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/pmxbot/bookmarklet-min.js
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/pmxbot/bookmarklet.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.575632 pmxbot.webhooks-1.5.0/pmxbot/compat/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/pmxbot/compat/py311.py
--rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/pmxbot/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.575632 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-03 00:50:39.000000 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-03 00:50:39.000000 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:50:39.000000 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 00:50:39.000000 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-03 00:50:39.000000 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 00:50:39.000000 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-03 00:50:39.579632 pmxbot.webhooks-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.575632 pmxbot.webhooks-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:31:11.917188 pmxbot.webhooks-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:31:11.913188 pmxbot.webhooks-1.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:31:11.913188 pmxbot.webhooks-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-07 22:31:11.917188 pmxbot.webhooks-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:31:11.917188 pmxbot.webhooks-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:31:11.917188 pmxbot.webhooks-1.6.0/pmxbot/
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/pmxbot/bookmarklet-min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/pmxbot/bookmarklet.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:31:11.917188 pmxbot.webhooks-1.6.0/pmxbot/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/pmxbot/compat/py311.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/pmxbot/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:31:11.917188 pmxbot.webhooks-1.6.0/pmxbot.webhooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-07 22:31:11.000000 pmxbot.webhooks-1.6.0/pmxbot.webhooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-07 22:31:11.000000 pmxbot.webhooks-1.6.0/pmxbot.webhooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:31:11.000000 pmxbot.webhooks-1.6.0/pmxbot.webhooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 22:31:11.000000 pmxbot.webhooks-1.6.0/pmxbot.webhooks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-07 22:31:11.000000 pmxbot.webhooks-1.6.0/pmxbot.webhooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 22:31:11.000000 pmxbot.webhooks-1.6.0/pmxbot.webhooks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 22:31:11.921188 pmxbot.webhooks-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:31:11.917188 pmxbot.webhooks-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-07 22:30:54.000000 pmxbot.webhooks-1.6.0/tox.ini
```

### Comparing `pmxbot.webhooks-1.5.0/.github/workflows/main.yml` & `pmxbot.webhooks-1.6.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pmxbot.webhooks-1.5.0/LICENSE` & `pmxbot.webhooks-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pmxbot.webhooks-1.5.0/NEWS.rst` & `pmxbot.webhooks-1.6.0/NEWS.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v1.6.0
+======
+
+Features
+--------
+
+- Instead of splitting lines, enqueue multiline messages, handled nicely by Slack. (#1)
+
+
 v1.5.0
 ======
 
 Features
 --------
 
 - Rely on PEP 420 for namespace package.
```

### Comparing `pmxbot.webhooks-1.5.0/PKG-INFO` & `pmxbot.webhooks-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmxbot.webhooks
-Version: 1.5.0
+Version: 1.6.0
 Summary: An HTTP-based webhook service for pmxbot
 Home-page: https://github.com/jaraco/pmxbot.webhooks
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pmxbot.webhooks-1.5.0/README.rst` & `pmxbot.webhooks-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `pmxbot.webhooks-1.5.0/docs/conf.py` & `pmxbot.webhooks-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pmxbot.webhooks-1.5.0/pmxbot/bookmarklet-min.js` & `pmxbot.webhooks-1.6.0/pmxbot/bookmarklet-min.js`

 * *Files identical despite different names*

### Comparing `pmxbot.webhooks-1.5.0/pmxbot/bookmarklet.js` & `pmxbot.webhooks-1.6.0/pmxbot/bookmarklet.js`

 * *Files identical despite different names*

### Comparing `pmxbot.webhooks-1.5.0/pmxbot/webhooks.py` & `pmxbot.webhooks-1.6.0/pmxbot/webhooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import re
 import os
 import json
 import logging
 import codecs
 import textwrap
 import urllib.parse
-from itertools import chain
 from typing import List, Union
 
 from .compat.py311 import resources
 
 from more_itertools import always_iterable
 import cherrypy
 import pmxbot.core
@@ -276,25 +275,23 @@
     jenkins = Jenkins()
     fogbugz = manuscript = Manuscript()
     velociraptor = Velociraptor()
 
     @classmethod
     def send_to(cls, channel, *msgs):
         cls.queue.append(pmxbot.core.SwitchChannel(channel))
-        # We must send line-by-line, so split multiline messages
-        lines = chain(*(msg.splitlines() for msg in msgs))
-        cls.queue.extend(lines)
+        cls.queue.extend(msgs)
 
     @cherrypy.expose
     @cherrypy.tools.actually_decode()
     def default(self, channel):
         lines = [line.rstrip() for line in cherrypy.request.body]
-        msg_len = sum(len(line.encode('utf-8')) for line in lines)
-        self.send_to(channel, *lines)
-        return '{msg_len} bytes queued for {channel}'.format(**locals())
+        payload = '\n'.join(lines)
+        self.send_to(channel, payload)
+        return f'{len(lines)} bytes queued for {channel}'
 
     @cherrypy.expose
     def bookmarklet(self):
         """
         Render the bookmarklet for easy installation.
         """
         return self.render_bookmarklet()
```

### Comparing `pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/PKG-INFO` & `pmxbot.webhooks-1.6.0/pmxbot.webhooks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmxbot.webhooks
-Version: 1.5.0
+Version: 1.6.0
 Summary: An HTTP-based webhook service for pmxbot
 Home-page: https://github.com/jaraco/pmxbot.webhooks
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/SOURCES.txt` & `pmxbot.webhooks-1.6.0/pmxbot.webhooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmxbot.webhooks-1.5.0/pytest.ini` & `pmxbot.webhooks-1.6.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `pmxbot.webhooks-1.5.0/setup.cfg` & `pmxbot.webhooks-1.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pmxbot.webhooks-1.5.0/tests/test_http.py` & `pmxbot.webhooks-1.6.0/tests/test_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,28 +17,27 @@
 
     def test_send_to(self):
         Server.send_to('channel', 'msg1', 'msg2', 'msg3')
         assert Server.queue == ['channel', 'msg1', 'msg2', 'msg3']
 
     def test_send_to_multiline(self):
         Server.send_to('channel', 'msg1\nmsg2', 'msg3')
-        assert Server.queue == ['channel', 'msg1', 'msg2', 'msg3']
+        assert Server.queue == ['channel', 'msg1\nmsg2', 'msg3']
 
     def test_send_to_multiple(self):
         Server.send_to('chan1', 'msg1')
         Server.send_to('chan2', 'msg2')
         Server.send_to('chan3', 'msg3\nmsg4')
         assert Server.queue == [
             'chan1',
             'msg1',
             'chan2',
             'msg2',
             'chan3',
-            'msg3',
-            'msg4',
+            'msg3\nmsg4',
         ]
 
 
 class VelociraptorTest(helper.CPWebCase):
     @staticmethod
     def setup_server():
         cherrypy.tree.mount(Server())
```

### Comparing `pmxbot.webhooks-1.5.0/tox.ini` & `pmxbot.webhooks-1.6.0/tox.ini`

 * *Files identical despite different names*

