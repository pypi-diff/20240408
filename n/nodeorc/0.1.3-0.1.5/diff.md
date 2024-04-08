# Comparing `tmp/nodeorc-0.1.3.tar.gz` & `tmp/nodeorc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodeorc-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nodeorc-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nodeorc-0.1.3.tar` & `nodeorc-0.1.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      187 2024-04-08 06:23:23.469295 nodeorc-0.1.3/.env
--rw-r--r--   0        0        0     1146 2024-04-08 06:23:23.469295 nodeorc-0.1.3/.github/ISSUE_TEMPLATE/issue-report.md
--rw-r--r--   0        0        0     1547 2024-04-08 06:23:23.469295 nodeorc-0.1.3/.github/workflows/publish-release-pypi.yml
--rw-r--r--   0        0        0     2248 2024-04-08 06:23:23.469295 nodeorc-0.1.3/.github/workflows/publish-test-pypi.yml
--rw-r--r--   0        0        0     3129 2024-04-08 06:23:23.469295 nodeorc-0.1.3/.gitignore
--rw-r--r--   0        0        0      559 2024-04-08 06:23:23.469295 nodeorc-0.1.3/Dockerfile
--rw-r--r--   0        0        0    34523 2024-04-08 06:23:23.469295 nodeorc-0.1.3/LICENSE
--rw-r--r--   0        0        0    27141 2024-04-08 06:23:23.469295 nodeorc-0.1.3/README.rst
--rw-r--r--   0        0        0     1594 2024-04-08 06:23:23.469295 nodeorc-0.1.3/docker-compose-test.yml
--rw-r--r--   0        0        0  2525884 2024-04-08 06:23:23.481295 nodeorc-0.1.3/docs/static/front.jpg
--rw-r--r--   0        0        0     2718 2024-04-08 06:23:23.481295 nodeorc-0.1.3/mockserver/initializerJson.json
--rw-r--r--   0        0        0       93 2024-04-08 06:23:23.481295 nodeorc-0.1.3/mockserver/mockserver.properties
--rw-r--r--   0        0        0      445 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/__init__.py
--rw-r--r--   0        0        0     3705 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/callbacks.py
--rw-r--r--   0        0        0     5959 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/config.py
--rw-r--r--   0        0        0      681 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/db/__init__.py
--rw-r--r--   0        0        0      292 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/db/active_config.py
--rw-r--r--   0        0        0      741 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/db/init_basedata.py
--rw-r--r--   0        0        0    10813 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/db/models.py
--rw-r--r--   0        0        0     3761 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/disk_mng.py
--rw-r--r--   0        0        0     2858 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/log.py
--rw-r--r--   0        0        0    10288 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/main.py
--rw-r--r--   0        0        0      959 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/__init__.py
--rw-r--r--   0        0        0     1629 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/callback.py
--rw-r--r--   0        0        0     6378 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/callback_url.py
--rw-r--r--   0        0        0     3966 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/config.py
--rw-r--r--   0        0        0     3301 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/storage.py
--rw-r--r--   0        0        0     4356 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/subtask.py
--rw-r--r--   0        0        0     6261 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/task.py
--rw-r--r--   0        0        0      104 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/tasks/__init__.py
--rw-r--r--   0        0        0    24638 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/tasks/local_task.py
--rw-r--r--   0        0        0     8694 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/tasks/task_form.py
--rw-r--r--   0        0        0     2764 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/utils.py
--rw-r--r--   0        0        0     1282 2024-04-08 06:23:23.481295 nodeorc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      106 2024-04-08 06:23:23.481295 nodeorc-0.1.3/requirements.txt
--rw-r--r--   0        0        0      422 2024-04-08 06:23:23.481295 nodeorc-0.1.3/service/10-toggleusbstick.rules
--rw-r--r--   0        0        0     2107 2024-04-08 06:23:23.481295 nodeorc-0.1.3/service/usb-mount.sh
--rw-r--r--   0        0        0      184 2024-04-08 06:23:23.481295 nodeorc-0.1.3/service/usb-mount@.service
--rw-r--r--   0        0        0        0 2024-04-08 06:23:23.481295 nodeorc-0.1.3/settings/.gitkeep
--rw-r--r--   0        0        0      722 2024-04-08 06:23:23.481295 nodeorc-0.1.3/settings/config_template.json
--rwxr-xr-x   0        0        0    21564 2024-04-08 06:23:23.481295 nodeorc-0.1.3/setup.sh
--rw-r--r--   0        0        0     8907 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0    60249 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/examples/ngwerere_transect.nc
--rw-r--r--   0        0        0      496 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_amqp_task.py
--rw-r--r--   0        0        0      802 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_callbacks.py
--rw-r--r--   0        0        0     2493 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_config.py
--rw-r--r--   0        0        0      875 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_disk_management.py
--rw-r--r--   0        0        0      128 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_io.py
--rw-r--r--   0        0        0      726 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_s3.py
--rw-r--r--   0        0        0      184 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_task.py
--rw-r--r--   0        0        0    28618 1970-01-01 00:00:00.000000 nodeorc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      187 2024-04-08 09:17:09.970916 nodeorc-0.1.5/.env
+-rw-r--r--   0        0        0     1146 2024-04-08 09:17:09.970916 nodeorc-0.1.5/.github/ISSUE_TEMPLATE/issue-report.md
+-rw-r--r--   0        0        0     1547 2024-04-08 09:17:09.970916 nodeorc-0.1.5/.github/workflows/publish-release-pypi.yml
+-rw-r--r--   0        0        0     2248 2024-04-08 09:17:09.970916 nodeorc-0.1.5/.github/workflows/publish-test-pypi.yml
+-rw-r--r--   0        0        0     3129 2024-04-08 09:17:09.970916 nodeorc-0.1.5/.gitignore
+-rw-r--r--   0        0        0      559 2024-04-08 09:17:09.970916 nodeorc-0.1.5/Dockerfile
+-rw-r--r--   0        0        0    34523 2024-04-08 09:17:09.974916 nodeorc-0.1.5/LICENSE
+-rw-r--r--   0        0        0    27141 2024-04-08 09:17:09.974916 nodeorc-0.1.5/README.rst
+-rw-r--r--   0        0        0     1594 2024-04-08 09:17:09.974916 nodeorc-0.1.5/docker-compose-test.yml
+-rw-r--r--   0        0        0  2525884 2024-04-08 09:17:09.982916 nodeorc-0.1.5/docs/static/front.jpg
+-rw-r--r--   0        0        0     2718 2024-04-08 09:17:09.982916 nodeorc-0.1.5/mockserver/initializerJson.json
+-rw-r--r--   0        0        0       93 2024-04-08 09:17:09.982916 nodeorc-0.1.5/mockserver/mockserver.properties
+-rw-r--r--   0        0        0      445 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/__init__.py
+-rw-r--r--   0        0        0     3705 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/callbacks.py
+-rw-r--r--   0        0        0     5959 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/config.py
+-rw-r--r--   0        0        0      681 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/db/__init__.py
+-rw-r--r--   0        0        0      292 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/db/active_config.py
+-rw-r--r--   0        0        0      741 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/db/init_basedata.py
+-rw-r--r--   0        0        0    10813 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/db/models.py
+-rw-r--r--   0        0        0     3761 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/disk_mng.py
+-rw-r--r--   0        0        0     2858 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/log.py
+-rw-r--r--   0        0        0    10288 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/main.py
+-rw-r--r--   0        0        0      959 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/models/__init__.py
+-rw-r--r--   0        0        0     1629 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/models/callback.py
+-rw-r--r--   0        0        0     6378 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/models/callback_url.py
+-rw-r--r--   0        0        0     3966 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/models/config.py
+-rw-r--r--   0        0        0     3301 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/models/storage.py
+-rw-r--r--   0        0        0     4356 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/models/subtask.py
+-rw-r--r--   0        0        0     6261 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/models/task.py
+-rw-r--r--   0        0        0      104 2024-04-08 09:17:09.982916 nodeorc-0.1.5/nodeorc/tasks/__init__.py
+-rw-r--r--   0        0        0    24778 2024-04-08 09:17:09.986916 nodeorc-0.1.5/nodeorc/tasks/local_task.py
+-rw-r--r--   0        0        0     8694 2024-04-08 09:17:09.986916 nodeorc-0.1.5/nodeorc/tasks/task_form.py
+-rw-r--r--   0        0        0     2823 2024-04-08 09:17:09.986916 nodeorc-0.1.5/nodeorc/utils.py
+-rw-r--r--   0        0        0     1282 2024-04-08 09:17:09.986916 nodeorc-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      106 2024-04-08 09:17:09.986916 nodeorc-0.1.5/requirements.txt
+-rw-r--r--   0        0        0      422 2024-04-08 09:17:09.986916 nodeorc-0.1.5/service/10-toggleusbstick.rules
+-rw-r--r--   0        0        0     2107 2024-04-08 09:17:09.986916 nodeorc-0.1.5/service/usb-mount.sh
+-rw-r--r--   0        0        0      184 2024-04-08 09:17:09.986916 nodeorc-0.1.5/service/usb-mount@.service
+-rw-r--r--   0        0        0        0 2024-04-08 09:17:09.986916 nodeorc-0.1.5/settings/.gitkeep
+-rw-r--r--   0        0        0      722 2024-04-08 09:17:09.986916 nodeorc-0.1.5/settings/config_template.json
+-rwxr-xr-x   0        0        0    21564 2024-04-08 09:17:09.986916 nodeorc-0.1.5/setup.sh
+-rw-r--r--   0        0        0     8907 2024-04-08 09:17:09.986916 nodeorc-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0    60249 2024-04-08 09:17:09.986916 nodeorc-0.1.5/tests/examples/ngwerere_transect.nc
+-rw-r--r--   0        0        0      496 2024-04-08 09:17:09.986916 nodeorc-0.1.5/tests/test_amqp_task.py
+-rw-r--r--   0        0        0      802 2024-04-08 09:17:09.986916 nodeorc-0.1.5/tests/test_callbacks.py
+-rw-r--r--   0        0        0     2493 2024-04-08 09:17:09.986916 nodeorc-0.1.5/tests/test_config.py
+-rw-r--r--   0        0        0      875 2024-04-08 09:17:09.986916 nodeorc-0.1.5/tests/test_disk_management.py
+-rw-r--r--   0        0        0      128 2024-04-08 09:17:09.986916 nodeorc-0.1.5/tests/test_io.py
+-rw-r--r--   0        0        0      726 2024-04-08 09:17:09.986916 nodeorc-0.1.5/tests/test_s3.py
+-rw-r--r--   0        0        0      184 2024-04-08 09:17:09.986916 nodeorc-0.1.5/tests/test_task.py
+-rw-r--r--   0        0        0    28618 1970-01-01 00:00:00.000000 nodeorc-0.1.5/PKG-INFO
```

### Comparing `nodeorc-0.1.3/.github/ISSUE_TEMPLATE/issue-report.md` & `nodeorc-0.1.5/.github/ISSUE_TEMPLATE/issue-report.md`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/.github/workflows/publish-release-pypi.yml` & `nodeorc-0.1.5/.github/workflows/publish-release-pypi.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/.github/workflows/publish-test-pypi.yml` & `nodeorc-0.1.5/.github/workflows/publish-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/.gitignore` & `nodeorc-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/Dockerfile` & `nodeorc-0.1.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/LICENSE` & `nodeorc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/README.rst` & `nodeorc-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/docker-compose-test.yml` & `nodeorc-0.1.5/docker-compose-test.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/docs/static/front.jpg` & `nodeorc-0.1.5/docs/static/front.jpg`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/mockserver/initializerJson.json` & `nodeorc-0.1.5/mockserver/initializerJson.json`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/callbacks.py` & `nodeorc-0.1.5/nodeorc/callbacks.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/config.py` & `nodeorc-0.1.5/nodeorc/config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/db/__init__.py` & `nodeorc-0.1.5/nodeorc/db/__init__.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/db/init_basedata.py` & `nodeorc-0.1.5/nodeorc/db/init_basedata.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/db/models.py` & `nodeorc-0.1.5/nodeorc/db/models.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/disk_mng.py` & `nodeorc-0.1.5/nodeorc/disk_mng.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/log.py` & `nodeorc-0.1.5/nodeorc/log.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/main.py` & `nodeorc-0.1.5/nodeorc/main.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/models/__init__.py` & `nodeorc-0.1.5/nodeorc/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/models/callback.py` & `nodeorc-0.1.5/nodeorc/models/callback.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/models/callback_url.py` & `nodeorc-0.1.5/nodeorc/models/callback_url.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/models/config.py` & `nodeorc-0.1.5/nodeorc/models/config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/models/storage.py` & `nodeorc-0.1.5/nodeorc/models/storage.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/models/subtask.py` & `nodeorc-0.1.5/nodeorc/models/subtask.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/models/task.py` & `nodeorc-0.1.5/nodeorc/models/task.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/tasks/local_task.py` & `nodeorc-0.1.5/nodeorc/tasks/local_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,17 +326,18 @@
 
         if os.path.isdir(task_path):
             # remove any left over temporary files
             shutil.rmtree(task_path)
 
     def _shutdown_or_not(self):
         if self.settings["shutdown_after_task"]:
-            self.logger.info("Task done! Shutting down...")
-            os.system("/sbin/shutdown -h now")
-            os.system("sudo /sbin/shutdown -h now")
+            self.logger.info("Task done! Shutting down in 15 seconds")
+            os.system("/usr/bin/sleep 15 && /sbin/shutdown -h now")
+            os.system("/usr/bin/sleep 15 && /bin/sudo /sbin/shutdown -h now")
+            os.system("/usr/bin/sleep 15 && /usr/bin/sudo /sbin/shutdown -h now")
 
     def _post_callbacks(self, callbacks):
         """
         Performs callbacks in a list, and returns True when all were successful
 
         Parameters
         ----------
```

### Comparing `nodeorc-0.1.3/nodeorc/tasks/task_form.py` & `nodeorc-0.1.5/nodeorc/tasks/task_form.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/nodeorc/utils.py` & `nodeorc-0.1.5/nodeorc/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     # first check if bucket is available
     r = check_bucket(s3, bucket_name)
     if r["code"] == 200:
         return s3.Bucket(bucket_name)
     else:
         return None
 
+
 def upload_io(obj, bucket, dest=None, logger=logging):
     """
     Uploads BytesIO obj representation of data in file 'fn' in bucket
     """
 
     r = bucket.upload_fileobj(obj, dest)
     logger.info(f"{bucket}/{dest} created")
@@ -98,8 +99,9 @@
     else:
         return False
 
 
 def reboot_now():
     os.system("/sbin/shutdown -r now")
     # in case this fails, do a sudo shutdown
-    os.system("sudo /sbin/shutdown -r now")
+    os.system("/bin/sudo /sbin/shutdown -r now")
+    os.system("/usr/bin/sudo /sbin/shutdown -r now")
```

### Comparing `nodeorc-0.1.3/pyproject.toml` & `nodeorc-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/service/usb-mount.sh` & `nodeorc-0.1.5/service/usb-mount.sh`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/settings/config_template.json` & `nodeorc-0.1.5/settings/config_template.json`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/setup.sh` & `nodeorc-0.1.5/setup.sh`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/tests/conftest.py` & `nodeorc-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/tests/examples/ngwerere_transect.nc` & `nodeorc-0.1.5/tests/examples/ngwerere_transect.nc`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/tests/test_callbacks.py` & `nodeorc-0.1.5/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/tests/test_config.py` & `nodeorc-0.1.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/tests/test_disk_management.py` & `nodeorc-0.1.5/tests/test_disk_management.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/tests/test_s3.py` & `nodeorc-0.1.5/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.3/PKG-INFO` & `nodeorc-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodeorc
-Version: 0.1.3
+Version: 0.1.5
 Summary: NodeORC: Automated edge and cloud image-based discharge estimation with OpenRiverCam
 Author-email: Hessel Winsemius <winsemius@rainbowsensing.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

