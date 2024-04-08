# Comparing `tmp/aprsd-irc-extension-0.0.3.tar.gz` & `tmp/aprsd-irc-extension-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprsd-irc-extension-0.0.3.tar", last modified: Wed Mar  6 20:21:53 2024, max compression
+gzip compressed data, was "aprsd-irc-extension-0.0.4.tar", last modified: Mon Apr  8 21:31:43 2024, max compression
```

## Comparing `aprsd-irc-extension-0.0.3.tar` & `aprsd-irc-extension-0.0.4.tar`

### file list

```diff
@@ -1,43 +1,54 @@
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-06 20:21:53.588396 aprsd-irc-extension-0.0.3/
--rw-r--r--   0 I530566    (501) staff       (20)      501 2024-02-26 16:22:39.000000 aprsd-irc-extension-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 I530566    (501) staff       (20)       27 2024-03-06 20:21:50.000000 aprsd-irc-extension-0.0.3/AUTHORS
--rw-r--r--   0 I530566    (501) staff       (20)      523 2024-03-06 20:21:50.000000 aprsd-irc-extension-0.0.3/ChangeLog
--rw-r--r--   0 I530566    (501) staff       (20)    10142 2024-02-23 18:20:28.000000 aprsd-irc-extension-0.0.3/LICENSE
--rw-r--r--   0 I530566    (501) staff       (20)     2602 2024-03-06 20:03:30.000000 aprsd-irc-extension-0.0.3/Makefile
--rw-r--r--   0 I530566    (501) staff       (20)     5216 2024-03-06 20:21:53.588058 aprsd-irc-extension-0.0.3/PKG-INFO
--rw-r--r--   0 I530566    (501) staff       (20)     3892 2024-03-06 20:21:14.000000 aprsd-irc-extension-0.0.3/README.rst
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-06 20:21:53.511305 aprsd-irc-extension-0.0.3/aprsd_irc_extension/
--rw-r--r--   0 I530566    (501) staff       (20)      645 2024-02-28 21:36:03.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension/__init__.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-06 20:21:53.516403 aprsd-irc-extension-0.0.3/aprsd_irc_extension/cmds/
--rw-r--r--   0 I530566    (501) staff       (20)      213 2024-02-28 20:02:15.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension/cmds/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)    17551 2024-03-06 19:48:56.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension/cmds/server.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-06 20:21:53.517151 aprsd-irc-extension-0.0.3/aprsd_irc_extension/conf/
--rw-r--r--   0 I530566    (501) staff       (20)      114 2024-02-28 21:39:19.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension/conf/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)      583 2024-03-05 16:49:23.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension/conf/main.py
--rw-r--r--   0 I530566    (501) staff       (20)     2715 2024-02-28 21:39:37.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension/conf/opts.py
--rw-r--r--   0 I530566    (501) staff       (20)       58 2024-02-28 21:36:24.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension/extension.py
--rw-r--r--   0 I530566    (501) staff       (20)      711 2024-02-28 21:37:00.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension/utils.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-06 20:21:53.587459 aprsd-irc-extension-0.0.3/aprsd_irc_extension.egg-info/
--rw-r--r--   0 I530566    (501) staff       (20)     5216 2024-03-06 20:21:50.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension.egg-info/PKG-INFO
--rw-r--r--   0 I530566    (501) staff       (20)      859 2024-03-06 20:21:53.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension.egg-info/SOURCES.txt
--rw-r--r--   0 I530566    (501) staff       (20)        1 2024-03-06 20:21:50.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension.egg-info/dependency_links.txt
--rw-r--r--   0 I530566    (501) staff       (20)      131 2024-03-06 20:21:50.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension.egg-info/entry_points.txt
--rw-r--r--   0 I530566    (501) staff       (20)        1 2024-03-06 20:12:22.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension.egg-info/not-zip-safe
--rw-r--r--   0 I530566    (501) staff       (20)       46 2024-03-06 20:21:50.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension.egg-info/pbr.json
--rw-r--r--   0 I530566    (501) staff       (20)      242 2024-03-06 20:21:50.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension.egg-info/requires.txt
--rw-r--r--   0 I530566    (501) staff       (20)       20 2024-03-06 20:21:50.000000 aprsd-irc-extension-0.0.3/aprsd_irc_extension.egg-info/top_level.txt
--rw-r--r--   0 I530566    (501) staff       (20)      221 2024-02-23 18:21:49.000000 aprsd-irc-extension-0.0.3/dev-requirements.in
--rw-r--r--   0 I530566    (501) staff       (20)     3711 2024-02-23 22:07:39.000000 aprsd-irc-extension-0.0.3/dev-requirements.txt
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-06 20:21:53.582001 aprsd-irc-extension-0.0.3/docker/
--rw-r--r--   0 I530566    (501) staff       (20)       78 2024-02-25 22:38:25.000000 aprsd-irc-extension-0.0.3/docker/Dockerfile
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-06 20:21:53.586612 aprsd-irc-extension-0.0.3/docker/bin/
--rwxr-xr-x   0 I530566    (501) staff       (20)     1172 2024-02-26 16:22:39.000000 aprsd-irc-extension-0.0.3/docker/bin/irc.sh
--rw-r--r--   0 I530566    (501) staff       (20)       95 2024-02-23 18:43:31.000000 aprsd-irc-extension-0.0.3/gray.conf
--rw-r--r--   0 I530566    (501) staff       (20)      538 2024-02-28 22:13:48.000000 aprsd-irc-extension-0.0.3/pyproject.toml
--rw-r--r--   0 I530566    (501) staff       (20)       22 2024-02-28 22:04:24.000000 aprsd-irc-extension-0.0.3/requirements.in
--rw-r--r--   0 I530566    (501) staff       (20)      826 2024-02-23 22:07:33.000000 aprsd-irc-extension-0.0.3/requirements.txt
--rw-r--r--   0 I530566    (501) staff       (20)     1269 2024-03-06 20:21:53.591034 aprsd-irc-extension-0.0.3/setup.cfg
--rw-r--r--   0 I530566    (501) staff       (20)      950 2024-02-23 18:25:44.000000 aprsd-irc-extension-0.0.3/setup.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-06 20:21:53.587039 aprsd-irc-extension-0.0.3/tests/
--rw-r--r--   0 I530566    (501) staff       (20)      221 2024-02-28 19:59:15.000000 aprsd-irc-extension-0.0.3/tests/test_main.py
--rw-r--r--   0 I530566    (501) staff       (20)     2664 2024-02-28 20:00:24.000000 aprsd-irc-extension-0.0.3/tox.ini
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-08 21:31:43.264219 aprsd-irc-extension-0.0.4/
+-rw-r--r--   0 I530566    (501) staff       (20)      501 2024-02-26 16:22:39.000000 aprsd-irc-extension-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 I530566    (501) staff       (20)       68 2024-04-08 21:31:39.000000 aprsd-irc-extension-0.0.4/AUTHORS
+-rw-r--r--   0 I530566    (501) staff       (20)      929 2024-04-08 21:31:39.000000 aprsd-irc-extension-0.0.4/ChangeLog
+-rw-r--r--   0 I530566    (501) staff       (20)    10142 2024-02-23 18:20:28.000000 aprsd-irc-extension-0.0.4/LICENSE
+-rw-r--r--   0 I530566    (501) staff       (20)     2757 2024-03-13 18:56:04.000000 aprsd-irc-extension-0.0.4/Makefile
+-rw-r--r--   0 I530566    (501) staff       (20)     5382 2024-04-08 21:31:43.264050 aprsd-irc-extension-0.0.4/PKG-INFO
+-rw-r--r--   0 I530566    (501) staff       (20)     3892 2024-03-06 20:21:14.000000 aprsd-irc-extension-0.0.4/README.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     3663 2024-03-13 18:56:04.000000 aprsd-irc-extension-0.0.4/alembic.ini
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-08 21:31:43.125162 aprsd-irc-extension-0.0.4/aprsd_irc_extension/
+-rw-r--r--   0 I530566    (501) staff       (20)      645 2024-02-28 21:36:03.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/__init__.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-08 21:31:43.156822 aprsd-irc-extension-0.0.4/aprsd_irc_extension/cmds/
+-rw-r--r--   0 I530566    (501) staff       (20)      213 2024-02-28 20:02:15.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/cmds/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1648 2024-04-08 21:29:42.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/cmds/db.py
+-rw-r--r--   0 I530566    (501) staff       (20)    20877 2024-04-08 21:28:57.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/cmds/server.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-08 21:31:43.157731 aprsd-irc-extension-0.0.4/aprsd_irc_extension/conf/
+-rw-r--r--   0 I530566    (501) staff       (20)      114 2024-02-28 21:39:19.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/conf/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)      717 2024-03-13 18:56:04.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/conf/main.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2715 2024-02-28 21:39:37.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/conf/opts.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-08 21:31:43.256606 aprsd-irc-extension-0.0.4/aprsd_irc_extension/db/
+-rw-r--r--   0 I530566    (501) staff       (20)       38 2024-03-13 18:56:04.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/db/README
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2024-03-13 18:56:04.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/db/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3513 2024-03-13 18:56:04.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/db/env.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4340 2024-04-08 21:27:26.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/db/models.py
+-rw-r--r--   0 I530566    (501) staff       (20)      635 2024-03-13 18:56:04.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/db/script.py.mako
+-rw-r--r--   0 I530566    (501) staff       (20)     1662 2024-04-08 21:25:54.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/db/session.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-08 21:31:43.257015 aprsd-irc-extension-0.0.4/aprsd_irc_extension/db/versions/
+-rw-r--r--   0 I530566    (501) staff       (20)     1796 2024-04-08 21:23:38.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/db/versions/030cab1951e1_.py
+-rw-r--r--   0 I530566    (501) staff       (20)      112 2024-03-13 20:00:15.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/extension.py
+-rw-r--r--   0 I530566    (501) staff       (20)      711 2024-02-28 21:37:00.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension/utils.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-08 21:31:43.263502 aprsd-irc-extension-0.0.4/aprsd_irc_extension.egg-info/
+-rw-r--r--   0 I530566    (501) staff       (20)     5382 2024-04-08 21:31:39.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension.egg-info/PKG-INFO
+-rw-r--r--   0 I530566    (501) staff       (20)     1151 2024-04-08 21:31:43.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 I530566    (501) staff       (20)        1 2024-04-08 21:31:39.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 I530566    (501) staff       (20)      131 2024-04-08 21:31:39.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension.egg-info/entry_points.txt
+-rw-r--r--   0 I530566    (501) staff       (20)        1 2024-04-08 21:31:39.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension.egg-info/not-zip-safe
+-rw-r--r--   0 I530566    (501) staff       (20)       46 2024-04-08 21:31:39.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension.egg-info/pbr.json
+-rw-r--r--   0 I530566    (501) staff       (20)      333 2024-04-08 21:31:39.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension.egg-info/requires.txt
+-rw-r--r--   0 I530566    (501) staff       (20)       20 2024-04-08 21:31:39.000000 aprsd-irc-extension-0.0.4/aprsd_irc_extension.egg-info/top_level.txt
+-rw-r--r--   0 I530566    (501) staff       (20)      221 2024-02-23 18:21:49.000000 aprsd-irc-extension-0.0.4/dev-requirements.in
+-rw-r--r--   0 I530566    (501) staff       (20)     3712 2024-03-13 20:05:22.000000 aprsd-irc-extension-0.0.4/dev-requirements.txt
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-08 21:31:43.258882 aprsd-irc-extension-0.0.4/docker/
+-rw-r--r--   0 I530566    (501) staff       (20)       77 2024-03-13 20:00:15.000000 aprsd-irc-extension-0.0.4/docker/Dockerfile
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-08 21:31:43.262086 aprsd-irc-extension-0.0.4/docker/bin/
+-rwxr-xr-x   0 I530566    (501) staff       (20)     1213 2024-03-13 20:00:15.000000 aprsd-irc-extension-0.0.4/docker/bin/irc.sh
+-rw-r--r--   0 I530566    (501) staff       (20)       95 2024-02-23 18:43:31.000000 aprsd-irc-extension-0.0.4/gray.conf
+-rw-r--r--   0 I530566    (501) staff       (20)      538 2024-02-28 22:13:48.000000 aprsd-irc-extension-0.0.4/pyproject.toml
+-rw-r--r--   0 I530566    (501) staff       (20)       41 2024-03-13 20:03:21.000000 aprsd-irc-extension-0.0.4/requirements.in
+-rw-r--r--   0 I530566    (501) staff       (20)     1087 2024-03-13 20:05:17.000000 aprsd-irc-extension-0.0.4/requirements.txt
+-rw-r--r--   0 I530566    (501) staff       (20)     1269 2024-04-08 21:31:43.266536 aprsd-irc-extension-0.0.4/setup.cfg
+-rw-r--r--   0 I530566    (501) staff       (20)      950 2024-02-23 18:25:44.000000 aprsd-irc-extension-0.0.4/setup.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-08 21:31:43.262571 aprsd-irc-extension-0.0.4/tests/
+-rw-r--r--   0 I530566    (501) staff       (20)      221 2024-02-28 19:59:15.000000 aprsd-irc-extension-0.0.4/tests/test_main.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2664 2024-02-28 20:00:24.000000 aprsd-irc-extension-0.0.4/tox.ini
```

### Comparing `aprsd-irc-extension-0.0.3/LICENSE` & `aprsd-irc-extension-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aprsd-irc-extension-0.0.3/Makefile` & `aprsd-irc-extension-0.0.4/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -79,7 +79,14 @@
 update-requirements: dev  ## Update the requirements.txt and dev-requirements.txt files
 	rm requirements.txt
 	rm dev-requirements.txt
 	touch requirements.txt
 	touch dev-requirements.txt
 	$(VENV)/pip-compile --resolver backtracking --annotation-style line requirements.in
 	$(VENV)/pip-compile --resolver backtracking --annotation-style line dev-requirements.in
+
+
+db-setup: dev  ## create the database
+	$(VENV)/alembic upgrade head
+
+db-revision: dev  ## Create a new revision
+	$(VENV)/alembic revision --autogenerate
```

### Comparing `aprsd-irc-extension-0.0.3/PKG-INFO` & `aprsd-irc-extension-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd-irc-extension
-Version: 0.0.3
+Version: 0.0.4
 Summary: An Extension to Ham radio APRSD Daemon to act like an irc server for APRS
 Home-page: http://aprsd.readthedocs.org
 Author: Walter A. Boring IV
 Author-email: waboring@hemna.com
 License: Apache
 Project-URL: Source, https://github.com/hemna/aprsd-irc
 Project-URL: Tracker, https://github.com/hemna/aprsd-irc/issues
@@ -14,27 +14,32 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: alembic==1.13.1
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: click==8.1.7
 Requires-Dist: debtcollector==3.0.0
 Requires-Dist: idna==3.6
+Requires-Dist: mako==1.3.2
+Requires-Dist: markupsafe==2.1.5
 Requires-Dist: netaddr==1.2.1
 Requires-Dist: oslo-config==9.4.0
 Requires-Dist: oslo-i18n==6.3.0
 Requires-Dist: pbr==6.0.0
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: rfc3986==2.0.0
+Requires-Dist: sqlalchemy==2.0.28
 Requires-Dist: stevedore==5.2.0
+Requires-Dist: typing-extensions==4.10.0
 Requires-Dist: urllib3==2.2.1
 Requires-Dist: wrapt==1.16.0
 
 ========================================
 APRSD extension add irc server via APRS!
 ========================================
```

### Comparing `aprsd-irc-extension-0.0.3/README.rst` & `aprsd-irc-extension-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `aprsd-irc-extension-0.0.3/aprsd_irc_extension/__init__.py` & `aprsd-irc-extension-0.0.4/aprsd_irc_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-irc-extension-0.0.3/aprsd_irc_extension/cmds/server.py` & `aprsd-irc-extension-0.0.4/aprsd_irc_extension/cmds/server.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 import signal
 import sys
 import time
 
 import click
 from oslo_config import cfg
 
+
 import aprsd
+from aprsd import cli_helper, client, packets, stats
+from aprsd import threads as aprsd_threads
+from aprsd.threads import tx, registry, keep_alive
+
+from aprsd_irc_extension.db import models
+from aprsd_irc_extension.db import session as db_session
 import aprsd_irc_extension
 from aprsd_irc_extension import cmds, utils
 from aprsd_irc_extension import conf  # noqa
-from aprsd import cli_helper, client, packets, stats
-from aprsd import threads as aprsd_threads
-from aprsd.threads import tx, registry
-from aprsd.utils import objectstore
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
 
 def signal_handler(sig, frame):
@@ -31,119 +34,174 @@
                 datetime.datetime.now(),
             ),
         )
         time.sleep(1.5)
         packets.PacketTrack().save()
         packets.WatchList().save()
         packets.SeenList().save()
-        IRChannels().save()
         LOG.info(stats.APRSDStats())
         # signal.signal(signal.SIGTERM, sys.exit(0))
         # sys.exit(0)
 
 
 class InvalidChannelName(Exception):
     pass
 
 
-class IRCChannel:
-    """Base class for an IRC Channel."""
+class ChannelService:
+    """Class for handling channel related commands."""
 
-    def __init__(self, name):
-        self.name = name
-        self.users = set()
-        self.messages = []
-
-    def join(self, user):
-        self.users.add(user)
-        LOG.info(f"{user} has joined {self.name}")
+    @staticmethod
+    def join(channel: str, user: str) -> models.Channel:
+        """User wants to join a channel."""
+        LOG.info(f"{user} has joined {channel}")
+        session = db_session.get_session()
+        user_obj = models.ChannelUsers(user=user)
+        ch = models.Channel.find_by_name(session, channel)
+        ch.users.append(user_obj)
         pkt = packets.MessagePacket(
             from_call=CONF.callsign,
             to_call=user,
-            message_text=f"Welcome to channel {self.name}",
+            message_text=f"Welcome to channel {channel}",
         )
         tx.send(pkt)
         time.sleep(1)
         tx.send(packets.MessagePacket(
             from_call=CONF.callsign,
             to_call=user,
-            message_text=f"Use /leave {self.name} to leave",
+            message_text=f"Use /leave {channel} to leave",
         ))
+        ch.save(session)
+        session.remove()
+        return channel
+
+    @staticmethod
+    def leave(channel: str, user: str) -> models.Channel:
+        """User wants to leave a channel."""
+        LOG.info(f"{user} wants to leave channel {channel}")
+        session = db_session.get_session()
+        ch = models.Channel.find_by_name(session, channel)
+        LOG.info(repr(ch))
+        found = False
+        for user_obj in ch.users:
+            if user_obj.user == user:
+                found = True
+                session.delete(user_obj)
+                session.flush()
+                session.commit()
+                pkt = packets.MessagePacket(
+                    from_call=CONF.callsign,
+                    to_call=user,
+                    message_text=f"Left channel {channel}",
+                )
+                tx.send(pkt)
 
-    def leave(self, user):
-        if user in self.users:
-            self.users.remove(user)
-            LOG.info(f"{user} has left {self.name}")
-            pkt = packets.MessagePacket(
-                from_call=CONF.callsign,
-                to_call=user,
-                message_text=f"Left channel {self.name}",
-            )
-            tx.send(pkt)
-        else:
-            LOG.warning(f"{user} not in channel {self.name}")
+        if not found:
+            LOG.warning(f"{user} not in channel {channel}")
             pkt = packets.MessagePacket(
                 from_call=CONF.callsign,
                 to_call=user,
-                message_text=f"not in channel {self.name}",
+                message_text=f"not in channel {channel}",
             )
             tx.send(pkt)
 
-    def add_message(self, pkt):
-        self.messages.append(pkt)
+        session.remove()
+        return channel
 
-    def list(self, user):
-        IRChannels().list(user)
+    @staticmethod
+    def add_message(channel: str, pkt: packets.MessagePacket) -> models.Channel:
+        """Add a message to the channel."""
+        LOG.info(f"Adding message to channel {channel}")
+        session = db_session.get_session()
+        ch = models.Channel.find_by_name(session, channel)
+        ch.messages.append(models.ChannelMessages.new_message(pkt))
+        ch.save(session)
+        session.remove()
+        return channel
 
 
-class IRChannels(objectstore.ObjectStoreMixin):
+class IRChannels:
     """List of IRC Channels."""
     _instance = None
     lock = threading.Lock()
     data: dict = {}
+    db_session = None
 
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
-            cls._instance._init_store()
             cls._instance.data = {}
+            cls._instance._load()
         return cls._instance
 
-    def list(self, packet):
+    def __len__(self):
+        return len(self.data)
+
+    def __iter__(self):
+        return iter(self.data)
+
+    def _load(self):
+        LOG.info("IRChannels: Loading channels from DB")
+        session = db_session.get_session()
+        channels = session.query(models.Channel).all()
+        for ch in channels:
+            LOG.info(f"IRChannels: Loading channel {ch}")
+            users = []
+            for user in ch.users:
+                users.append(user.user)
+            LOG.info(f"IRChannels: Loading messages {len(ch.messages)}")
+            self.data[ch.name] = users
+
+        LOG.info(f"IRChannels: Loaded {len(self.data)} channels from DB")
+        session.remove()
+
+    def get(self, id):
+        with self.lock:
+            return self.data[id]
+
+    def list(self, packet) -> None:
+        """Send a list of channels and count of users in channel."""
+        channels = models.Channel.get_all_channels()
         user = packet.from_call
-        for channel_name in self.data:
-            ch = self.get_channel(channel_name)
+        for ch in channels:
             pkt = packets.MessagePacket(
                 from_call=CONF.callsign,
                 to_call=user,
                 message_text=f"Channel {ch.name} Users({len(ch.users)})",
             )
             tx.send(pkt)
 
-    def add_channel(self, name):
+    def add_channel(self, name: str):
         if not name.startswith("#"):
             raise InvalidChannelName(
                 "Channel name must start with #")
         if name not in self.data:
-            self.data[name] = IRCChannel(name)
-        return self.data.get(name)
+            models.Channel.create_channel(name)
+            # initialize w/o users
+            self.data[name] = []
 
-    def remove_channel(self, name):
+    def remove_channel(self, name: str) -> None:
         if not name.startswith("#"):
             raise InvalidChannelName(
                 "Channel name must start with #")
         if name in self.data:
             del self.data[name]
 
-    def get_channel(self, name):
+    def get_channel(self, name: str) -> models.Channel:
         if not name.startswith("#"):
             raise InvalidChannelName(
                 "Channel name must start with #")
         return self.data.get(name)
 
+    def channel_exists(self, name: str) -> bool:
+        if not name.startswith("#"):
+            raise InvalidChannelName(
+                "Channel name must start with #")
+        return name in self.data
+
 
 class APRSDIRCProcessPacketThread(aprsd_threads.APRSDProcessPacketThread):
     # Commands for IRC Channels
     commands = {
         "/join": {"cmd": "join",
                   "desc": "/join #channel or /j #channel - Join a channel"},
         "/leave": {"cmd": "leave",
@@ -201,59 +259,71 @@
         for command in self.short_server_commands:
             if message.startswith(command):
                 return self.short_server_commands[command]
         return None
 
     def _user_channel_count(self, user):
         """How many channels is a user in?"""
+        LOG.info(f"Checking how many channels {user} is in")
+        LOG.info(f"IRChannels().data: {IRChannels().data}")
         count = 0
         found = {}
-        for ch in IRChannels().data:
-            ch = IRChannels().get(ch)
-            if user in ch.users:
-                count += 1
-                found[ch.name] = ch
-                continue
+        session = db_session.get_session()
+        for name in IRChannels():
+            ch = models.Channel.find_by_name(session, name)
+            LOG.info(f"Checking channel {ch.name} : {ch.users}")
+            for user_ojb in ch.users:
+                if user_ojb.user == user:
+                    count += 1
+                    found[ch.name] = ch.name
+                    continue
+        session.remove()
 
+        LOG.info(f"User {user} is in {count} channels")
         return count, found
 
     def process_channel_command(self, packet, command_name, channel_name):
         fromcall = packet.from_call
         message = packet.get("message_text")
         ch = None
         if not channel_name:
             # They didn't specify a channel name
             # If this is leave
             # find how many channels the user is in
             if command_name == "/leave" or command_name == "/l":
                 count, found = self._user_channel_count(fromcall)
                 if count == 1:
-                    ch = found.popitem()[1]
-                    channel_name = ch.name
+                    channel_name = found.popitem()[1]
                 else:
                     channel_names = ", ".join(found.keys())
                     LOG.info(f"User {fromcall} is in {count} channels ({channel_names}). "
                              "Need to specify channel when leaving.")
                     tx.send(packets.MessagePacket(
                         from_call=CONF.callsign,
                         to_call=fromcall,
                         message_text="Need to specify channel when leaving. /leave #channel",
                     ))
                     return
 
+        session = None
         try:
-            ch = IRChannels().get_channel(channel_name)
+            if IRChannels().channel_exists(channel_name):
+                session = db_session.get_session()
+                ch = models.Channel.find_by_name(session, channel_name)
         except InvalidChannelName as e:
             LOG.error(f"Failed to add channel: {e}")
             tx.send(packets.MessagePacket(
                 from_call=CONF.callsign,
                 to_call=fromcall,
                 message_text="Channel name must start with #",
             ))
             return
+        finally:
+            if session:
+                session.remove()
 
         if not ch:
             ch = IRChannels().add_channel(channel_name)
 
         cmd_dict = self.get_channel_command(message)
         LOG.warning(f"cmd_dict: {cmd_dict}")
         if not cmd_dict:
@@ -262,21 +332,18 @@
                 packets.MessagePacket(
                     from_call=CONF.callsign,
                     to_call=fromcall,
                     message_text=f"Unknown command: {command_name}",
                 )
             )
             return
-        cmd = getattr(ch, cmd_dict["cmd"])
-        cmd(fromcall)
 
-        # if they are the last user to leave the channel, delete the channel
-        if command_name == "/leave" or command_name == "/l":
-            if not ch.users and not CONF.aprsd_irc_extension.default_channel:
-                IRChannels().remove_channel(ch.name)
+        svc = ChannelService
+        cmd = getattr(svc, cmd_dict["cmd"])
+        cmd(channel_name, fromcall)
         return
 
     def process_irc_command(self, packet):
         message = packet.get("message_text")
         msg_parts = message.split()
         command_name = msg_parts[0]
         try:
@@ -339,65 +406,84 @@
                         message_text=f"{cmd['desc']}",
                     ))
                 return
 
             # If not a channel command, then it's a message
             # to a channel or user
             channel_name = message.split()[0]
-            LOG.info(f"Send message to channel {channel_name}")
+            LOG.info(f"Send message to channel {channel_name}??")
+            ch = None
+            session = db_session.get_session()
             try:
                 ch = irc_channels.get_channel(channel_name)
             except InvalidChannelName as e:
                 count, found = self._user_channel_count(fromcall)
                 if count == 1:
-                    ch = found.popitem()[1]
-                    channel_name = ch.name
-                    message = f"{ch.name} {message}"
+                    channel_name = found.popitem()[1]
+                    message = f"{channel_name} {message}"
+                    ch = models.Channel.find_by_name(session, channel_name)
                 elif count > 1:
                     LOG.info("Failed to get channel from a user message. User in more than 1 channel")
                     tx.send(packets.MessagePacket(
                         from_call=CONF.callsign,
                         to_call=fromcall,
-                        message_text="Need to specify channel when sending a message. /msg #channel message",
+                        message_text="Need to specify channel when sending a message. '#channel msg'",
                     ))
+                    session.remove()
+                    return
+                elif count == 0:
+                    LOG.error(f"User is not in any channels: {e}")
+                    tx.send(packets.MessagePacket(
+                        from_call=CONF.callsign,
+                        to_call=fromcall,
+                        message_text="Must join a channel to send a message. try /list",
+                    ))
+                    session.remove()
                     return
                 else:
                     LOG.error(f"Failed to get channel: {e}")
                     tx.send(packets.MessagePacket(
                         from_call=CONF.callsign,
                         to_call=fromcall,
                         message_text="Channel name must start with #",
                     ))
+                    session.remove()
                     return
 
             if ch:
-                if fromcall not in ch.users:
+                found = False
+                for user_obj in ch.users:
+                    if user_obj.user == fromcall:
+                        found = True
+
+                if not found:
                     LOG.error(f"{fromcall} not in channel {channel_name}")
                     tx.send(packets.MessagePacket(
                         from_call=CONF.callsign,
                         to_call=fromcall,
                         message_text=f"{fromcall} not in channel {channel_name}",
                     ))
                     tx.send(packets.MessagePacket(
                         from_call=CONF.callsign,
                         to_call=fromcall,
                         message_text=f"Send /join {channel_name} to join channel",
                     ))
-
+                    session.remove()
                     return
 
                 msg = message.replace(ch.name, f"{ch.name} {fromcall}")
-                for user in ch.users:
-                    if user != fromcall:
+                for user_obj in ch.users:
+                    if user_obj.user != fromcall:
                         tx.send(packets.MessagePacket(
                             from_call=CONF.callsign,
-                            to_call=user,
+                            to_call=user_obj.user,
                             message_text=msg,
                         ))
-                ch.add_message(packet)
+                session.remove()
+                ChannelService.add_message(ch.name, packet)
             else:
                 LOG.error(f"Channel {channel_name} not found")
                 tx.send(packets.MessagePacket(
                     from_call=CONF.callsign,
                     to_call=fromcall,
                     message_text=f"Channel {channel_name} not found",
                 ))
@@ -415,18 +501,18 @@
     def __init__(self):
         super().__init__("ChannelInfo")
         self._loop_cnt = 1
 
     def loop(self):
         # Only dump out the stats every 60 seconds
         if self._loop_cnt % 60 == 0:
-            irc_channels = IRChannels()
+            session = db_session.get_session()
+            irc_channels = session.query(models.Channel).all()
             for ch in irc_channels:
-                ch = irc_channels.get(ch)
-                LOG.info(f"Channel: {ch.name} Users({len(ch.users)}): {ch.users}")
+                LOG.info(repr(ch))
         self._loop_cnt += 1
         time.sleep(1)
         return True
 
 
 @cmds.irc.command()
 @cli_helper.add_options(cli_helper.common_options)
@@ -438,14 +524,15 @@
     show_default=True,
     default=False,
     help="Flush out all old aged messages on disk.",
 )
 @click.pass_context
 @cli_helper.process_standard_options
 def server(ctx, flush):
+    """Run an APRS IRC server."""
     signal.signal(signal.SIGINT, signal_handler)
     signal.signal(signal.SIGTERM, signal_handler)
 
     level, msg = utils._check_version()
     if level:
         LOG.warning(msg)
     else:
@@ -472,27 +559,25 @@
     # Now load the msgTrack from disk if any
     packets.PacketList()
     if flush:
         LOG.debug("Deleting saved objects.")
         packets.PacketTrack().flush()
         packets.WatchList().flush()
         packets.SeenList().flush()
-        IRChannels().flush()
     else:
         # Try and load saved MsgTrack list
         LOG.debug("Loading saved objects.")
         packets.PacketTrack().load()
         packets.WatchList().load()
         packets.SeenList().load()
-        IRChannels().load()
 
     # Make sure the #lounge channel exists
     IRChannels().add_channel("#lounge")
 
-    keepalive = aprsd_threads.KeepAliveThread()
+    keepalive = keep_alive.KeepAliveThread()
     keepalive.start()
 
     rx_thread = aprsd_threads.APRSDDupeRXThread(
         packet_queue=aprsd_threads.packet_queue,
     )
     process_thread = APRSDIRCProcessPacketThread(
         packet_queue=aprsd_threads.packet_queue,
@@ -508,11 +593,11 @@
         LOG.info("Beacon Enabled.  Starting Beacon thread.")
         bcn_thread = tx.BeaconSendThread()
         bcn_thread.start()
 
     rx_thread.start()
     process_thread.start()
     channel_info_thread.start()
-    packets.PacketTrack().restart()
+    packets.PacketTrack()
 
     rx_thread.join()
     keepalive.join()
```

### Comparing `aprsd-irc-extension-0.0.3/aprsd_irc_extension/conf/opts.py` & `aprsd-irc-extension-0.0.4/aprsd_irc_extension/conf/opts.py`

 * *Files identical despite different names*

### Comparing `aprsd-irc-extension-0.0.3/aprsd_irc_extension/utils.py` & `aprsd-irc-extension-0.0.4/aprsd_irc_extension/utils.py`

 * *Files identical despite different names*

### Comparing `aprsd-irc-extension-0.0.3/aprsd_irc_extension.egg-info/PKG-INFO` & `aprsd-irc-extension-0.0.4/aprsd_irc_extension.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd-irc-extension
-Version: 0.0.3
+Version: 0.0.4
 Summary: An Extension to Ham radio APRSD Daemon to act like an irc server for APRS
 Home-page: http://aprsd.readthedocs.org
 Author: Walter A. Boring IV
 Author-email: waboring@hemna.com
 License: Apache
 Project-URL: Source, https://github.com/hemna/aprsd-irc
 Project-URL: Tracker, https://github.com/hemna/aprsd-irc/issues
@@ -14,27 +14,32 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: alembic==1.13.1
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: click==8.1.7
 Requires-Dist: debtcollector==3.0.0
 Requires-Dist: idna==3.6
+Requires-Dist: mako==1.3.2
+Requires-Dist: markupsafe==2.1.5
 Requires-Dist: netaddr==1.2.1
 Requires-Dist: oslo-config==9.4.0
 Requires-Dist: oslo-i18n==6.3.0
 Requires-Dist: pbr==6.0.0
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: rfc3986==2.0.0
+Requires-Dist: sqlalchemy==2.0.28
 Requires-Dist: stevedore==5.2.0
+Requires-Dist: typing-extensions==4.10.0
 Requires-Dist: urllib3==2.2.1
 Requires-Dist: wrapt==1.16.0
 
 ========================================
 APRSD extension add irc server via APRS!
 ========================================
```

### Comparing `aprsd-irc-extension-0.0.3/dev-requirements.txt` & `aprsd-irc-extension-0.0.4/dev-requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 #    pip-compile --annotation-style=line dev-requirements.in
 #
 add-trailing-comma==3.1.0  # via gray
 alabaster==0.7.16         # via sphinx
 autoflake==1.5.3          # via gray
 babel==2.14.0             # via sphinx
 black==24.2.0             # via gray
-build==1.0.3              # via pip-tools
-cachetools==5.3.2         # via tox
+build==1.1.1              # via pip-tools
+cachetools==5.3.3         # via tox
 certifi==2024.2.2         # via requests
 cfgv==3.4.0               # via pre-commit
 chardet==5.2.0            # via tox
 charset-normalizer==3.3.2  # via requests
 click==8.1.7              # via black, fixit, moreorless, pip-tools
 colorama==0.4.6           # via tox
 commonmark==0.9.1         # via rich
@@ -33,30 +33,30 @@
 iniconfig==2.0.0          # via pytest
 isort==5.13.2             # via -r dev-requirements.in, gray
 jinja2==3.1.3             # via sphinx
 libcst==1.2.0             # via fixit
 markupsafe==2.1.5         # via jinja2
 mccabe==0.7.0             # via flake8
 moreorless==0.4.0         # via fixit
-mypy==1.8.0               # via -r dev-requirements.in
+mypy==1.9.0               # via -r dev-requirements.in
 mypy-extensions==1.0.0    # via black, mypy, typing-inspect
 nodeenv==1.8.0            # via pre-commit
-packaging==23.2           # via black, build, fixit, pyproject-api, pytest, sphinx, tox
+packaging==24.0           # via black, build, fixit, pyproject-api, pytest, sphinx, tox
 pathspec==0.12.1          # via black, trailrunner
 pep8-naming==0.13.3       # via -r dev-requirements.in
-pip-tools==7.4.0          # via -r dev-requirements.in
+pip-tools==7.4.1          # via -r dev-requirements.in
 platformdirs==4.2.0       # via black, tox, virtualenv
 pluggy==1.4.0             # via pytest, tox
 pre-commit==3.6.2         # via -r dev-requirements.in
 pycodestyle==2.11.1       # via flake8
 pyflakes==3.2.0           # via autoflake, flake8
 pygments==2.17.2          # via rich, sphinx
 pyproject-api==1.6.1      # via tox
 pyproject-hooks==1.0.0    # via build, pip-tools
-pytest==8.0.1             # via -r dev-requirements.in, pytest-cov
+pytest==8.1.1             # via -r dev-requirements.in, pytest-cov
 pytest-cov==4.1.0         # via -r dev-requirements.in
 pyupgrade==3.15.1         # via gray
 pyyaml==6.0.1             # via libcst, pre-commit
 requests==2.31.0          # via sphinx
 rich==12.6.0              # via gray
 snowballstemmer==2.2.0    # via sphinx
 sphinx==7.2.6             # via -r dev-requirements.in
@@ -65,20 +65,20 @@
 sphinxcontrib-htmlhelp==2.0.5  # via sphinx
 sphinxcontrib-jsmath==1.0.1  # via sphinx
 sphinxcontrib-qthelp==1.0.7  # via sphinx
 sphinxcontrib-serializinghtml==1.1.10  # via sphinx
 tokenize-rt==5.2.0        # via add-trailing-comma, pyupgrade
 toml==0.10.2              # via autoflake
 tomli==2.0.1              # via black, build, coverage, fixit, mypy, pip-tools, pyproject-api, pyproject-hooks, pytest, tox
-tox==4.13.0               # via -r dev-requirements.in
+tox==4.14.1               # via -r dev-requirements.in
 trailrunner==1.4.0        # via fixit
-typing-extensions==4.9.0  # via black, libcst, mypy, typing-inspect
+typing-extensions==4.10.0  # via black, libcst, mypy, typing-inspect
 typing-inspect==0.9.0     # via libcst
 unify==0.5                # via gray
 untokenize==0.1.1         # via unify
 urllib3==2.2.1            # via requests
 virtualenv==20.25.1       # via pre-commit, tox
-wheel==0.42.0             # via pip-tools
+wheel==0.43.0             # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `aprsd-irc-extension-0.0.3/docker/bin/irc.sh` & `aprsd-irc-extension-0.0.4/docker/bin/irc.sh`

 * *Files 4% similar despite different names*

```diff
@@ -36,8 +36,10 @@
 if [ ! -e "$APRSD_CONFIG" ]; then
     echo "'$APRSD_CONFIG' File does not exist. Creating."
     aprsd sample-config > $APRSD_CONFIG
 fi
 
 export COLUMNS=200
 python3 -m rich.diagnose
+pip freeze
+aprsd irc db -c $APRSD_CONFIG
 exec aprsd irc server -c $APRSD_CONFIG --loglevel ${LOG_LEVEL}
```

### Comparing `aprsd-irc-extension-0.0.3/pyproject.toml` & `aprsd-irc-extension-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aprsd-irc-extension-0.0.3/requirements.txt` & `aprsd-irc-extension-0.0.4/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --annotation-style=line requirements.in
 #
+alembic==1.13.1           # via -r requirements.in
 certifi==2024.2.2         # via requests
 charset-normalizer==3.3.2  # via requests
 click==8.1.7              # via -r requirements.in
 debtcollector==3.0.0      # via oslo-config
 idna==3.6                 # via requests
+mako==1.3.2               # via alembic
+markupsafe==2.1.5         # via mako
 netaddr==1.2.1            # via oslo-config
 oslo-config==9.4.0        # via -r requirements.in
 oslo-i18n==6.3.0          # via oslo-config
-pbr==6.0.0                # via oslo-i18n, stevedore
+pbr==6.0.0                # via -r requirements.in, oslo-i18n, stevedore
 pyyaml==6.0.1             # via oslo-config
 requests==2.31.0          # via oslo-config
 rfc3986==2.0.0            # via oslo-config
+sqlalchemy==2.0.28        # via -r requirements.in, alembic
 stevedore==5.2.0          # via oslo-config
+typing-extensions==4.10.0  # via alembic, sqlalchemy
 urllib3==2.2.1            # via requests
 wrapt==1.16.0             # via debtcollector
```

### Comparing `aprsd-irc-extension-0.0.3/setup.cfg` & `aprsd-irc-extension-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `aprsd-irc-extension-0.0.3/setup.py` & `aprsd-irc-extension-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `aprsd-irc-extension-0.0.3/tox.ini` & `aprsd-irc-extension-0.0.4/tox.ini`

 * *Files identical despite different names*

