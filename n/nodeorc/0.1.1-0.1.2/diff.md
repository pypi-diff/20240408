# Comparing `tmp/nodeorc-0.1.1.tar.gz` & `tmp/nodeorc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodeorc-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nodeorc-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nodeorc-0.1.1.tar` & `nodeorc-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      187 2024-04-07 13:03:36.868016 nodeorc-0.1.1/.env
--rw-r--r--   0        0        0     1146 2024-04-07 13:03:36.872016 nodeorc-0.1.1/.github/ISSUE_TEMPLATE/issue-report.md
--rw-r--r--   0        0        0     1547 2024-04-07 13:03:36.872016 nodeorc-0.1.1/.github/workflows/publish-release-pypi.yml
--rw-r--r--   0        0        0     2244 2024-04-07 13:03:36.872016 nodeorc-0.1.1/.github/workflows/publish-test-pypi.yml
--rw-r--r--   0        0        0     3129 2024-04-07 13:03:36.872016 nodeorc-0.1.1/.gitignore
--rw-r--r--   0        0        0      559 2024-04-07 13:03:36.872016 nodeorc-0.1.1/Dockerfile
--rw-r--r--   0        0        0    34523 2024-04-07 13:03:36.872016 nodeorc-0.1.1/LICENSE
--rw-r--r--   0        0        0    27141 2024-04-07 13:03:36.872016 nodeorc-0.1.1/README.rst
--rw-r--r--   0        0        0     1594 2024-04-07 13:03:36.872016 nodeorc-0.1.1/docker-compose-test.yml
--rw-r--r--   0        0        0  2525884 2024-04-07 13:03:36.880016 nodeorc-0.1.1/docs/static/front.jpg
--rw-r--r--   0        0        0     2718 2024-04-07 13:03:36.880016 nodeorc-0.1.1/mockserver/initializerJson.json
--rw-r--r--   0        0        0       93 2024-04-07 13:03:36.880016 nodeorc-0.1.1/mockserver/mockserver.properties
--rw-r--r--   0        0        0      445 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/__init__.py
--rw-r--r--   0        0        0     3705 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/callbacks.py
--rw-r--r--   0        0        0     5959 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/config.py
--rw-r--r--   0        0        0      681 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/db/__init__.py
--rw-r--r--   0        0        0      292 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/db/active_config.py
--rw-r--r--   0        0        0      741 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/db/init_basedata.py
--rw-r--r--   0        0        0    10813 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/db/models.py
--rw-r--r--   0        0        0     3761 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/disk_mng.py
--rw-r--r--   0        0        0     2858 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/log.py
--rw-r--r--   0        0        0    10288 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/main.py
--rw-r--r--   0        0        0      959 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/__init__.py
--rw-r--r--   0        0        0     1629 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/callback.py
--rw-r--r--   0        0        0     6378 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/callback_url.py
--rw-r--r--   0        0        0     3966 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/config.py
--rw-r--r--   0        0        0     3301 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/storage.py
--rw-r--r--   0        0        0     4356 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/subtask.py
--rw-r--r--   0        0        0     6261 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/task.py
--rw-r--r--   0        0        0      104 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/tasks/__init__.py
--rw-r--r--   0        0        0    24586 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/tasks/local_task.py
--rw-r--r--   0        0        0     8694 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/tasks/task_form.py
--rw-r--r--   0        0        0     2764 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/utils.py
--rw-r--r--   0        0        0     1282 2024-04-07 13:03:36.884016 nodeorc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      106 2024-04-07 13:03:36.884016 nodeorc-0.1.1/requirements.txt
--rw-r--r--   0        0        0      422 2024-04-07 13:03:36.884016 nodeorc-0.1.1/service/10-toggleusbstick.rules
--rw-r--r--   0        0        0     2467 2024-04-07 13:03:36.884016 nodeorc-0.1.1/service/usb-mount.sh
--rw-r--r--   0        0        0      184 2024-04-07 13:03:36.884016 nodeorc-0.1.1/service/usb-mount@.service
--rw-r--r--   0        0        0        0 2024-04-07 13:03:36.884016 nodeorc-0.1.1/settings/.gitkeep
--rw-r--r--   0        0        0      722 2024-04-07 13:03:36.884016 nodeorc-0.1.1/settings/config_template.json
--rwxr-xr-x   0        0        0    18699 2024-04-07 13:03:36.884016 nodeorc-0.1.1/setup.sh
--rw-r--r--   0        0        0     8907 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0    60249 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/examples/ngwerere_transect.nc
--rw-r--r--   0        0        0      496 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_amqp_task.py
--rw-r--r--   0        0        0      802 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_callbacks.py
--rw-r--r--   0        0        0     2493 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_config.py
--rw-r--r--   0        0        0      875 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_disk_management.py
--rw-r--r--   0        0        0      128 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_io.py
--rw-r--r--   0        0        0      726 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_s3.py
--rw-r--r--   0        0        0      184 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_task.py
--rw-r--r--   0        0        0    28618 1970-01-01 00:00:00.000000 nodeorc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      187 2024-04-07 15:12:23.219626 nodeorc-0.1.2/.env
+-rw-r--r--   0        0        0     1146 2024-04-07 15:12:23.219626 nodeorc-0.1.2/.github/ISSUE_TEMPLATE/issue-report.md
+-rw-r--r--   0        0        0     1547 2024-04-07 15:12:23.219626 nodeorc-0.1.2/.github/workflows/publish-release-pypi.yml
+-rw-r--r--   0        0        0     2247 2024-04-07 15:12:23.219626 nodeorc-0.1.2/.github/workflows/publish-test-pypi.yml
+-rw-r--r--   0        0        0     3129 2024-04-07 15:12:23.219626 nodeorc-0.1.2/.gitignore
+-rw-r--r--   0        0        0      559 2024-04-07 15:12:23.219626 nodeorc-0.1.2/Dockerfile
+-rw-r--r--   0        0        0    34523 2024-04-07 15:12:23.219626 nodeorc-0.1.2/LICENSE
+-rw-r--r--   0        0        0    27141 2024-04-07 15:12:23.219626 nodeorc-0.1.2/README.rst
+-rw-r--r--   0        0        0     1594 2024-04-07 15:12:23.219626 nodeorc-0.1.2/docker-compose-test.yml
+-rw-r--r--   0        0        0  2525884 2024-04-07 15:12:23.227625 nodeorc-0.1.2/docs/static/front.jpg
+-rw-r--r--   0        0        0     2718 2024-04-07 15:12:23.227625 nodeorc-0.1.2/mockserver/initializerJson.json
+-rw-r--r--   0        0        0       93 2024-04-07 15:12:23.227625 nodeorc-0.1.2/mockserver/mockserver.properties
+-rw-r--r--   0        0        0      445 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/__init__.py
+-rw-r--r--   0        0        0     3705 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/callbacks.py
+-rw-r--r--   0        0        0     5959 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/config.py
+-rw-r--r--   0        0        0      681 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/db/__init__.py
+-rw-r--r--   0        0        0      292 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/db/active_config.py
+-rw-r--r--   0        0        0      741 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/db/init_basedata.py
+-rw-r--r--   0        0        0    10813 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/db/models.py
+-rw-r--r--   0        0        0     3761 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/disk_mng.py
+-rw-r--r--   0        0        0     2858 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/log.py
+-rw-r--r--   0        0        0    10288 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/main.py
+-rw-r--r--   0        0        0      959 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/models/__init__.py
+-rw-r--r--   0        0        0     1629 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/models/callback.py
+-rw-r--r--   0        0        0     6378 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/models/callback_url.py
+-rw-r--r--   0        0        0     3966 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/models/config.py
+-rw-r--r--   0        0        0     3301 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/models/storage.py
+-rw-r--r--   0        0        0     4356 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/models/subtask.py
+-rw-r--r--   0        0        0     6261 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/models/task.py
+-rw-r--r--   0        0        0      104 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/tasks/__init__.py
+-rw-r--r--   0        0        0    24586 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/tasks/local_task.py
+-rw-r--r--   0        0        0     8694 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/tasks/task_form.py
+-rw-r--r--   0        0        0     2758 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/utils.py
+-rw-r--r--   0        0        0     1282 2024-04-07 15:12:23.231626 nodeorc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      106 2024-04-07 15:12:23.231626 nodeorc-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      422 2024-04-07 15:12:23.231626 nodeorc-0.1.2/service/10-toggleusbstick.rules
+-rw-r--r--   0        0        0     2467 2024-04-07 15:12:23.231626 nodeorc-0.1.2/service/usb-mount.sh
+-rw-r--r--   0        0        0      184 2024-04-07 15:12:23.231626 nodeorc-0.1.2/service/usb-mount@.service
+-rw-r--r--   0        0        0        0 2024-04-07 15:12:23.231626 nodeorc-0.1.2/settings/.gitkeep
+-rw-r--r--   0        0        0      722 2024-04-07 15:12:23.231626 nodeorc-0.1.2/settings/config_template.json
+-rwxr-xr-x   0        0        0    18699 2024-04-07 15:12:23.231626 nodeorc-0.1.2/setup.sh
+-rw-r--r--   0        0        0     8907 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0    60249 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/examples/ngwerere_transect.nc
+-rw-r--r--   0        0        0      496 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_amqp_task.py
+-rw-r--r--   0        0        0      802 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_callbacks.py
+-rw-r--r--   0        0        0     2493 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_config.py
+-rw-r--r--   0        0        0      875 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_disk_management.py
+-rw-r--r--   0        0        0      128 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_io.py
+-rw-r--r--   0        0        0      726 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_s3.py
+-rw-r--r--   0        0        0      184 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_task.py
+-rw-r--r--   0        0        0    28618 1970-01-01 00:00:00.000000 nodeorc-0.1.2/PKG-INFO
```

### Comparing `nodeorc-0.1.1/.github/ISSUE_TEMPLATE/issue-report.md` & `nodeorc-0.1.2/.github/ISSUE_TEMPLATE/issue-report.md`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/.github/workflows/publish-release-pypi.yml` & `nodeorc-0.1.2/.github/workflows/publish-release-pypi.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/.github/workflows/publish-test-pypi.yml` & `nodeorc-0.1.2/.github/workflows/publish-test-pypi.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ---
 name: Build and Upload NodeORC to Test-PyPI
 
 on:
   release:
     types:
       - published
-  push:
-    tags:
-      - v*
+#  push:
+#    tags:
+#      - v*
   workflow_dispatch:
 
 jobs:
   build-artifacts:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
```

### Comparing `nodeorc-0.1.1/.gitignore` & `nodeorc-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/Dockerfile` & `nodeorc-0.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/LICENSE` & `nodeorc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/README.rst` & `nodeorc-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/docker-compose-test.yml` & `nodeorc-0.1.2/docker-compose-test.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/docs/static/front.jpg` & `nodeorc-0.1.2/docs/static/front.jpg`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/mockserver/initializerJson.json` & `nodeorc-0.1.2/mockserver/initializerJson.json`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/callbacks.py` & `nodeorc-0.1.2/nodeorc/callbacks.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/config.py` & `nodeorc-0.1.2/nodeorc/config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/db/__init__.py` & `nodeorc-0.1.2/nodeorc/db/__init__.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/db/init_basedata.py` & `nodeorc-0.1.2/nodeorc/db/init_basedata.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/db/models.py` & `nodeorc-0.1.2/nodeorc/db/models.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/disk_mng.py` & `nodeorc-0.1.2/nodeorc/disk_mng.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/log.py` & `nodeorc-0.1.2/nodeorc/log.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/main.py` & `nodeorc-0.1.2/nodeorc/main.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/models/__init__.py` & `nodeorc-0.1.2/nodeorc/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/models/callback.py` & `nodeorc-0.1.2/nodeorc/models/callback.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/models/callback_url.py` & `nodeorc-0.1.2/nodeorc/models/callback_url.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/models/config.py` & `nodeorc-0.1.2/nodeorc/models/config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/models/storage.py` & `nodeorc-0.1.2/nodeorc/models/storage.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/models/subtask.py` & `nodeorc-0.1.2/nodeorc/models/subtask.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/models/task.py` & `nodeorc-0.1.2/nodeorc/models/task.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/tasks/local_task.py` & `nodeorc-0.1.2/nodeorc/tasks/local_task.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/tasks/task_form.py` & `nodeorc-0.1.2/nodeorc/tasks/task_form.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/nodeorc/utils.py` & `nodeorc-0.1.2/nodeorc/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,10 +96,10 @@
     if size1 != os.path.getsize(fn):
         return True
     else:
         return False
 
 
 def reboot_now():
-    os.system("/sbin/shutdown -r now")
+    os.system("/sbin/shutdown now")
     # in case this fails, do a sudo shutdown
-    os.system("sudo /sbin/shutdown -r now")
+    os.system("sudo /sbin/shutdown now")
```

### Comparing `nodeorc-0.1.1/pyproject.toml` & `nodeorc-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/service/usb-mount.sh` & `nodeorc-0.1.2/service/usb-mount.sh`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/settings/config_template.json` & `nodeorc-0.1.2/settings/config_template.json`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/setup.sh` & `nodeorc-0.1.2/setup.sh`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/tests/conftest.py` & `nodeorc-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/tests/examples/ngwerere_transect.nc` & `nodeorc-0.1.2/tests/examples/ngwerere_transect.nc`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/tests/test_callbacks.py` & `nodeorc-0.1.2/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/tests/test_config.py` & `nodeorc-0.1.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/tests/test_disk_management.py` & `nodeorc-0.1.2/tests/test_disk_management.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/tests/test_s3.py` & `nodeorc-0.1.2/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.1/PKG-INFO` & `nodeorc-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodeorc
-Version: 0.1.1
+Version: 0.1.2
 Summary: NodeORC: Automated edge and cloud image-based discharge estimation with OpenRiverCam
 Author-email: Hessel Winsemius <winsemius@rainbowsensing.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

