# Comparing `tmp/execnet-2.1.0.tar.gz` & `tmp/execnet-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Apr  5 18:23:17 2024, max compression
+gzip compressed data, last modified: Sun Apr  7 20:33:21 2024, max compression
```

## Comparing `execnet-2.1.0.tar` & `execnet-2.1.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      604 2024-04-05 18:23:17.000000 execnet-2.1.0/tox.ini
--rw-r--r--   0        0        0     3197 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/Makefile
--rw-r--r--   0        0        0        2 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/__init__.py
--rw-r--r--   0        0        0     8005 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/basics.rst
--rw-r--r--   0        0        0       98 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/changelog.rst
--rw-r--r--   0        0        0     6478 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/conf.py
--rw-r--r--   0        0        0      603 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/examples.rst
--rw-r--r--   0        0        0     1239 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/implnotes.rst
--rw-r--r--   0        0        0     3308 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/index.rst
--rw-r--r--   0        0        0      798 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/install.rst
--rw-r--r--   0        0        0      726 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/support.rst
--rw-r--r--   0        0        0    24123 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/_static/basic1.png
--rw-r--r--   0        0        0    10202 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/_static/codespeak.png
--rw-r--r--   0        0        0    36750 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/_static/execnet.png
--rw-r--r--   0        0        0    17805 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/_static/pythonring.png
--rw-r--r--   0        0        0      806 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/_templates/indexsidebar.html
--rw-r--r--   0        0        0      843 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/_templates/layout.html
--rw-r--r--   0        0        0      379 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/conftest.py
--rw-r--r--   0        0        0      342 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/funcmultiplier.py
--rw-r--r--   0        0        0     4844 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/hybridpython.rst
--rw-r--r--   0        0        0      954 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/popen_read_multiple.py
--rw-r--r--   0        0        0      392 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/py3topy2.py
--rw-r--r--   0        0        0      702 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/redirect_remote_output.py
--rw-r--r--   0        0        0      142 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/remote1.py
--rw-r--r--   0        0        0      279 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/remotecmd.py
--rw-r--r--   0        0        0      243 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/servefiles.py
--rw-r--r--   0        0        0     3887 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/svn-sync-repo.py
--rw-r--r--   0        0        0     4858 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/sysinfo.py
--rw-r--r--   0        0        0     1348 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/taskserver.py
--rw-r--r--   0        0        0     2003 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_debug.rst
--rw-r--r--   0        0        0       47 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_funcmultiplier.py
--rw-r--r--   0        0        0     3501 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_group.rst
--rw-r--r--   0        0        0     6271 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_info.rst
--rw-r--r--   0        0        0     2990 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_multi.rst
--rw-r--r--   0        0        0      746 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_proxy.rst
--rw-r--r--   0        0        0      573 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_ssh_fileserver.rst
--rw-r--r--   0        0        0     1157 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/__init__.py
--rw-r--r--   0        0        0      411 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/_version.py
--rw-r--r--   0        0        0     7783 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/gateway.py
--rw-r--r--   0        0        0    59128 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/gateway_base.py
--rw-r--r--   0        0        0     2770 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/gateway_bootstrap.py
--rw-r--r--   0        0        0     8052 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/gateway_io.py
--rw-r--r--   0        0        0     2956 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/gateway_socket.py
--rw-r--r--   0        0        0    11714 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/multi.py
--rw-r--r--   0        0        0        0 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/py.typed
--rw-r--r--   0        0        0     8874 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/rsync.py
--rw-r--r--   0        0        0     4208 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/rsync_remote.py
--rw-r--r--   0        0        0     2256 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/xspec.py
--rw-r--r--   0        0        0        2 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/script/__init__.py
--rw-r--r--   0        0        0      418 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/script/loop_socketserver.py
--rw-r--r--   0        0        0      304 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/script/quitserver.py
--rw-r--r--   0        0        0     2601 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/script/shell.py
--rw-r--r--   0        0        0     3935 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/script/socketserver.py
--rw-r--r--   0        0        0     3181 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/script/socketserverservice.py
--rw-r--r--   0        0        0     6275 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/conftest.py
--rw-r--r--   0        0        0    13407 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_basics.py
--rw-r--r--   0        0        0    12780 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_channel.py
--rw-r--r--   0        0        0      847 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_compatibility_regressions.py
--rw-r--r--   0        0        0    21016 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_gateway.py
--rw-r--r--   0        0        0     8435 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_multi.py
--rw-r--r--   0        0        0    10438 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_rsync.py
--rw-r--r--   0        0        0     3767 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_serializer.py
--rw-r--r--   0        0        0     4785 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_termination.py
--rw-r--r--   0        0        0     5499 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_threadpool.py
--rw-r--r--   0        0        0     9218 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_xspec.py
--rw-r--r--   0        0        0      188 2024-04-05 18:23:17.000000 execnet-2.1.0/.gitignore
--rw-r--r--   0        0        0     1054 2024-04-05 18:23:17.000000 execnet-2.1.0/LICENSE
--rw-r--r--   0        0        0     1574 2024-04-05 18:23:17.000000 execnet-2.1.0/README.rst
--rw-r--r--   0        0        0     2901 2024-04-05 18:23:17.000000 execnet-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2905 2024-04-05 18:23:17.000000 execnet-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-04-07 20:33:21.000000 execnet-2.1.1/tox.ini
+-rw-r--r--   0        0        0     3197 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/Makefile
+-rw-r--r--   0        0        0        2 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/__init__.py
+-rw-r--r--   0        0        0     8005 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/basics.rst
+-rw-r--r--   0        0        0       98 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/changelog.rst
+-rw-r--r--   0        0        0     6478 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/conf.py
+-rw-r--r--   0        0        0      603 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/examples.rst
+-rw-r--r--   0        0        0     1239 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/implnotes.rst
+-rw-r--r--   0        0        0     3308 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/index.rst
+-rw-r--r--   0        0        0      798 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/install.rst
+-rw-r--r--   0        0        0      726 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/support.rst
+-rw-r--r--   0        0        0    24123 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/_static/basic1.png
+-rw-r--r--   0        0        0    10202 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/_static/codespeak.png
+-rw-r--r--   0        0        0    36750 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/_static/execnet.png
+-rw-r--r--   0        0        0    17805 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/_static/pythonring.png
+-rw-r--r--   0        0        0      806 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/_templates/indexsidebar.html
+-rw-r--r--   0        0        0      843 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/_templates/layout.html
+-rw-r--r--   0        0        0      379 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/conftest.py
+-rw-r--r--   0        0        0      342 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/funcmultiplier.py
+-rw-r--r--   0        0        0     4844 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/hybridpython.rst
+-rw-r--r--   0        0        0      954 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/popen_read_multiple.py
+-rw-r--r--   0        0        0      392 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/py3topy2.py
+-rw-r--r--   0        0        0      702 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/redirect_remote_output.py
+-rw-r--r--   0        0        0      142 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/remote1.py
+-rw-r--r--   0        0        0      279 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/remotecmd.py
+-rw-r--r--   0        0        0      243 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/servefiles.py
+-rw-r--r--   0        0        0     3887 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/svn-sync-repo.py
+-rw-r--r--   0        0        0     4858 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/sysinfo.py
+-rw-r--r--   0        0        0     1348 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/taskserver.py
+-rw-r--r--   0        0        0     2003 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/test_debug.rst
+-rw-r--r--   0        0        0       47 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/test_funcmultiplier.py
+-rw-r--r--   0        0        0     3501 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/test_group.rst
+-rw-r--r--   0        0        0     6271 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/test_info.rst
+-rw-r--r--   0        0        0     2990 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/test_multi.rst
+-rw-r--r--   0        0        0      746 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/test_proxy.rst
+-rw-r--r--   0        0        0      573 2024-04-07 20:33:21.000000 execnet-2.1.1/doc/example/test_ssh_fileserver.rst
+-rw-r--r--   0        0        0     1157 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/_version.py
+-rw-r--r--   0        0        0     7783 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/gateway.py
+-rw-r--r--   0        0        0    59089 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/gateway_base.py
+-rw-r--r--   0        0        0     2770 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/gateway_bootstrap.py
+-rw-r--r--   0        0        0     8052 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/gateway_io.py
+-rw-r--r--   0        0        0     2956 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/gateway_socket.py
+-rw-r--r--   0        0        0    11714 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/multi.py
+-rw-r--r--   0        0        0        0 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/py.typed
+-rw-r--r--   0        0        0     8874 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/rsync.py
+-rw-r--r--   0        0        0     4208 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/rsync_remote.py
+-rw-r--r--   0        0        0     2256 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/xspec.py
+-rw-r--r--   0        0        0        2 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/script/__init__.py
+-rw-r--r--   0        0        0      418 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/script/loop_socketserver.py
+-rw-r--r--   0        0        0      304 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/script/quitserver.py
+-rw-r--r--   0        0        0     2601 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/script/shell.py
+-rw-r--r--   0        0        0     3935 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/script/socketserver.py
+-rw-r--r--   0        0        0     3181 2024-04-07 20:33:21.000000 execnet-2.1.1/src/execnet/script/socketserverservice.py
+-rw-r--r--   0        0        0     6275 2024-04-07 20:33:21.000000 execnet-2.1.1/testing/conftest.py
+-rw-r--r--   0        0        0    13407 2024-04-07 20:33:21.000000 execnet-2.1.1/testing/test_basics.py
+-rw-r--r--   0        0        0    12780 2024-04-07 20:33:21.000000 execnet-2.1.1/testing/test_channel.py
+-rw-r--r--   0        0        0      847 2024-04-07 20:33:21.000000 execnet-2.1.1/testing/test_compatibility_regressions.py
+-rw-r--r--   0        0        0    21016 2024-04-07 20:33:21.000000 execnet-2.1.1/testing/test_gateway.py
+-rw-r--r--   0        0        0     8435 2024-04-07 20:33:21.000000 execnet-2.1.1/testing/test_multi.py
+-rw-r--r--   0        0        0    10438 2024-04-07 20:33:21.000000 execnet-2.1.1/testing/test_rsync.py
+-rw-r--r--   0        0        0     3903 2024-04-07 20:33:21.000000 execnet-2.1.1/testing/test_serializer.py
+-rw-r--r--   0        0        0     4785 2024-04-07 20:33:21.000000 execnet-2.1.1/testing/test_termination.py
+-rw-r--r--   0        0        0     5499 2024-04-07 20:33:21.000000 execnet-2.1.1/testing/test_threadpool.py
+-rw-r--r--   0        0        0     9218 2024-04-07 20:33:21.000000 execnet-2.1.1/testing/test_xspec.py
+-rw-r--r--   0        0        0      188 2024-04-07 20:33:21.000000 execnet-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1054 2024-04-07 20:33:21.000000 execnet-2.1.1/LICENSE
+-rw-r--r--   0        0        0     1574 2024-04-07 20:33:21.000000 execnet-2.1.1/README.rst
+-rw-r--r--   0        0        0     2901 2024-04-07 20:33:21.000000 execnet-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2905 2024-04-07 20:33:21.000000 execnet-2.1.1/PKG-INFO
```

### Comparing `execnet-2.1.0/tox.ini` & `execnet-2.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/Makefile` & `execnet-2.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/basics.rst` & `execnet-2.1.1/doc/basics.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/conf.py` & `execnet-2.1.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/examples.rst` & `execnet-2.1.1/doc/examples.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/implnotes.rst` & `execnet-2.1.1/doc/implnotes.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/index.rst` & `execnet-2.1.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/install.rst` & `execnet-2.1.1/doc/install.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/support.rst` & `execnet-2.1.1/doc/support.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/_static/basic1.png` & `execnet-2.1.1/doc/_static/basic1.png`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/_static/codespeak.png` & `execnet-2.1.1/doc/_static/codespeak.png`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/_static/execnet.png` & `execnet-2.1.1/doc/_static/execnet.png`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/_static/pythonring.png` & `execnet-2.1.1/doc/_static/pythonring.png`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/_templates/indexsidebar.html` & `execnet-2.1.1/doc/_templates/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/_templates/layout.html` & `execnet-2.1.1/doc/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/example/hybridpython.rst` & `execnet-2.1.1/doc/example/hybridpython.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/example/popen_read_multiple.py` & `execnet-2.1.1/doc/example/popen_read_multiple.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/example/redirect_remote_output.py` & `execnet-2.1.1/doc/example/redirect_remote_output.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/example/svn-sync-repo.py` & `execnet-2.1.1/doc/example/svn-sync-repo.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/example/sysinfo.py` & `execnet-2.1.1/doc/example/sysinfo.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/example/taskserver.py` & `execnet-2.1.1/doc/example/taskserver.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/example/test_debug.rst` & `execnet-2.1.1/doc/example/test_debug.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/example/test_group.rst` & `execnet-2.1.1/doc/example/test_group.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/example/test_info.rst` & `execnet-2.1.1/doc/example/test_info.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/example/test_multi.rst` & `execnet-2.1.1/doc/example/test_multi.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/example/test_proxy.rst` & `execnet-2.1.1/doc/example/test_proxy.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/doc/example/test_ssh_fileserver.rst` & `execnet-2.1.1/doc/example/test_ssh_fileserver.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/src/execnet/__init__.py` & `execnet-2.1.1/src/execnet/__init__.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/src/execnet/gateway.py` & `execnet-2.1.1/src/execnet/gateway.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/src/execnet/gateway_base.py` & `execnet-2.1.1/src/execnet/gateway_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1387,17 +1387,15 @@
         channel_or_gateway: Channel | BaseGateway | None = None,
         strconfig: tuple[bool, bool] | None = None,
     ) -> None:
         if isinstance(channel_or_gateway, Channel):
             gw: BaseGateway | None = channel_or_gateway.gateway
         else:
             gw = channel_or_gateway
-        if channel_or_gateway is None:
-            strconfig = None
-        else:
+        if channel_or_gateway is not None:
             strconfig = channel_or_gateway._strconfig
         if strconfig:
             self.py2str_as_py3str, self.py3str_as_py2str = strconfig
         self.stream = stream
         if gw is None:
             self.channelfactory = None
         else:
```

### Comparing `execnet-2.1.0/src/execnet/gateway_bootstrap.py` & `execnet-2.1.1/src/execnet/gateway_bootstrap.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/src/execnet/gateway_io.py` & `execnet-2.1.1/src/execnet/gateway_io.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/src/execnet/gateway_socket.py` & `execnet-2.1.1/src/execnet/gateway_socket.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/src/execnet/multi.py` & `execnet-2.1.1/src/execnet/multi.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/src/execnet/rsync.py` & `execnet-2.1.1/src/execnet/rsync.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/src/execnet/rsync_remote.py` & `execnet-2.1.1/src/execnet/rsync_remote.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/src/execnet/xspec.py` & `execnet-2.1.1/src/execnet/xspec.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/src/execnet/script/shell.py` & `execnet-2.1.1/src/execnet/script/shell.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/src/execnet/script/socketserver.py` & `execnet-2.1.1/src/execnet/script/socketserver.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/src/execnet/script/socketserverservice.py` & `execnet-2.1.1/src/execnet/script/socketserverservice.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/testing/conftest.py` & `execnet-2.1.1/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/testing/test_basics.py` & `execnet-2.1.1/testing/test_basics.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/testing/test_channel.py` & `execnet-2.1.1/testing/test_channel.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/testing/test_compatibility_regressions.py` & `execnet-2.1.1/testing/test_compatibility_regressions.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/testing/test_gateway.py` & `execnet-2.1.1/testing/test_gateway.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/testing/test_multi.py` & `execnet-2.1.1/testing/test_multi.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/testing/test_rsync.py` & `execnet-2.1.1/testing/test_rsync.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/testing/test_serializer.py` & `execnet-2.1.1/testing/test_serializer.py`

 * *Files 10% similar despite different names*

```diff
@@ -159,7 +159,12 @@
 
 
 def test_tuple_nested_with_empty_in_between(dump, load) -> None:
     p = dump("(1, (), 3)")
     tp, s = load(p)
     assert tp == "tuple"
     assert s == "(1, (), 3)"
+
+
+def test_py2_string_loads() -> None:
+    """Regression test for #267."""
+    assert execnet.loads(b"\x02M\x00\x00\x00\x01aQ") == b"a"
```

### Comparing `execnet-2.1.0/testing/test_termination.py` & `execnet-2.1.1/testing/test_termination.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/testing/test_threadpool.py` & `execnet-2.1.1/testing/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/testing/test_xspec.py` & `execnet-2.1.1/testing/test_xspec.py`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/LICENSE` & `execnet-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/README.rst` & `execnet-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/pyproject.toml` & `execnet-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `execnet-2.1.0/PKG-INFO` & `execnet-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: execnet
-Version: 2.1.0
+Version: 2.1.1
 Summary: execnet: rapid multi-Python deployment
 Project-URL: Homepage, https://execnet.readthedocs.io/en/latest/
 Author: holger krekel and others
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

