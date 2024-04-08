# Comparing `tmp/nodeorc-0.1.2.tar.gz` & `tmp/nodeorc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodeorc-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nodeorc-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nodeorc-0.1.2.tar` & `nodeorc-0.1.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      187 2024-04-07 15:12:23.219626 nodeorc-0.1.2/.env
--rw-r--r--   0        0        0     1146 2024-04-07 15:12:23.219626 nodeorc-0.1.2/.github/ISSUE_TEMPLATE/issue-report.md
--rw-r--r--   0        0        0     1547 2024-04-07 15:12:23.219626 nodeorc-0.1.2/.github/workflows/publish-release-pypi.yml
--rw-r--r--   0        0        0     2247 2024-04-07 15:12:23.219626 nodeorc-0.1.2/.github/workflows/publish-test-pypi.yml
--rw-r--r--   0        0        0     3129 2024-04-07 15:12:23.219626 nodeorc-0.1.2/.gitignore
--rw-r--r--   0        0        0      559 2024-04-07 15:12:23.219626 nodeorc-0.1.2/Dockerfile
--rw-r--r--   0        0        0    34523 2024-04-07 15:12:23.219626 nodeorc-0.1.2/LICENSE
--rw-r--r--   0        0        0    27141 2024-04-07 15:12:23.219626 nodeorc-0.1.2/README.rst
--rw-r--r--   0        0        0     1594 2024-04-07 15:12:23.219626 nodeorc-0.1.2/docker-compose-test.yml
--rw-r--r--   0        0        0  2525884 2024-04-07 15:12:23.227625 nodeorc-0.1.2/docs/static/front.jpg
--rw-r--r--   0        0        0     2718 2024-04-07 15:12:23.227625 nodeorc-0.1.2/mockserver/initializerJson.json
--rw-r--r--   0        0        0       93 2024-04-07 15:12:23.227625 nodeorc-0.1.2/mockserver/mockserver.properties
--rw-r--r--   0        0        0      445 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/__init__.py
--rw-r--r--   0        0        0     3705 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/callbacks.py
--rw-r--r--   0        0        0     5959 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/config.py
--rw-r--r--   0        0        0      681 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/db/__init__.py
--rw-r--r--   0        0        0      292 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/db/active_config.py
--rw-r--r--   0        0        0      741 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/db/init_basedata.py
--rw-r--r--   0        0        0    10813 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/db/models.py
--rw-r--r--   0        0        0     3761 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/disk_mng.py
--rw-r--r--   0        0        0     2858 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/log.py
--rw-r--r--   0        0        0    10288 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/main.py
--rw-r--r--   0        0        0      959 2024-04-07 15:12:23.227625 nodeorc-0.1.2/nodeorc/models/__init__.py
--rw-r--r--   0        0        0     1629 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/models/callback.py
--rw-r--r--   0        0        0     6378 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/models/callback_url.py
--rw-r--r--   0        0        0     3966 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/models/config.py
--rw-r--r--   0        0        0     3301 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/models/storage.py
--rw-r--r--   0        0        0     4356 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/models/subtask.py
--rw-r--r--   0        0        0     6261 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/models/task.py
--rw-r--r--   0        0        0      104 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/tasks/__init__.py
--rw-r--r--   0        0        0    24586 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/tasks/local_task.py
--rw-r--r--   0        0        0     8694 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/tasks/task_form.py
--rw-r--r--   0        0        0     2758 2024-04-07 15:12:23.231626 nodeorc-0.1.2/nodeorc/utils.py
--rw-r--r--   0        0        0     1282 2024-04-07 15:12:23.231626 nodeorc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      106 2024-04-07 15:12:23.231626 nodeorc-0.1.2/requirements.txt
--rw-r--r--   0        0        0      422 2024-04-07 15:12:23.231626 nodeorc-0.1.2/service/10-toggleusbstick.rules
--rw-r--r--   0        0        0     2467 2024-04-07 15:12:23.231626 nodeorc-0.1.2/service/usb-mount.sh
--rw-r--r--   0        0        0      184 2024-04-07 15:12:23.231626 nodeorc-0.1.2/service/usb-mount@.service
--rw-r--r--   0        0        0        0 2024-04-07 15:12:23.231626 nodeorc-0.1.2/settings/.gitkeep
--rw-r--r--   0        0        0      722 2024-04-07 15:12:23.231626 nodeorc-0.1.2/settings/config_template.json
--rwxr-xr-x   0        0        0    18699 2024-04-07 15:12:23.231626 nodeorc-0.1.2/setup.sh
--rw-r--r--   0        0        0     8907 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0    60249 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/examples/ngwerere_transect.nc
--rw-r--r--   0        0        0      496 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_amqp_task.py
--rw-r--r--   0        0        0      802 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_callbacks.py
--rw-r--r--   0        0        0     2493 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_config.py
--rw-r--r--   0        0        0      875 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_disk_management.py
--rw-r--r--   0        0        0      128 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_io.py
--rw-r--r--   0        0        0      726 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_s3.py
--rw-r--r--   0        0        0      184 2024-04-07 15:12:23.231626 nodeorc-0.1.2/tests/test_task.py
--rw-r--r--   0        0        0    28618 1970-01-01 00:00:00.000000 nodeorc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      187 2024-04-08 06:23:23.469295 nodeorc-0.1.3/.env
+-rw-r--r--   0        0        0     1146 2024-04-08 06:23:23.469295 nodeorc-0.1.3/.github/ISSUE_TEMPLATE/issue-report.md
+-rw-r--r--   0        0        0     1547 2024-04-08 06:23:23.469295 nodeorc-0.1.3/.github/workflows/publish-release-pypi.yml
+-rw-r--r--   0        0        0     2248 2024-04-08 06:23:23.469295 nodeorc-0.1.3/.github/workflows/publish-test-pypi.yml
+-rw-r--r--   0        0        0     3129 2024-04-08 06:23:23.469295 nodeorc-0.1.3/.gitignore
+-rw-r--r--   0        0        0      559 2024-04-08 06:23:23.469295 nodeorc-0.1.3/Dockerfile
+-rw-r--r--   0        0        0    34523 2024-04-08 06:23:23.469295 nodeorc-0.1.3/LICENSE
+-rw-r--r--   0        0        0    27141 2024-04-08 06:23:23.469295 nodeorc-0.1.3/README.rst
+-rw-r--r--   0        0        0     1594 2024-04-08 06:23:23.469295 nodeorc-0.1.3/docker-compose-test.yml
+-rw-r--r--   0        0        0  2525884 2024-04-08 06:23:23.481295 nodeorc-0.1.3/docs/static/front.jpg
+-rw-r--r--   0        0        0     2718 2024-04-08 06:23:23.481295 nodeorc-0.1.3/mockserver/initializerJson.json
+-rw-r--r--   0        0        0       93 2024-04-08 06:23:23.481295 nodeorc-0.1.3/mockserver/mockserver.properties
+-rw-r--r--   0        0        0      445 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/__init__.py
+-rw-r--r--   0        0        0     3705 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/callbacks.py
+-rw-r--r--   0        0        0     5959 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/config.py
+-rw-r--r--   0        0        0      681 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/db/__init__.py
+-rw-r--r--   0        0        0      292 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/db/active_config.py
+-rw-r--r--   0        0        0      741 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/db/init_basedata.py
+-rw-r--r--   0        0        0    10813 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/db/models.py
+-rw-r--r--   0        0        0     3761 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/disk_mng.py
+-rw-r--r--   0        0        0     2858 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/log.py
+-rw-r--r--   0        0        0    10288 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/main.py
+-rw-r--r--   0        0        0      959 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/__init__.py
+-rw-r--r--   0        0        0     1629 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/callback.py
+-rw-r--r--   0        0        0     6378 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/callback_url.py
+-rw-r--r--   0        0        0     3966 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/config.py
+-rw-r--r--   0        0        0     3301 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/storage.py
+-rw-r--r--   0        0        0     4356 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/subtask.py
+-rw-r--r--   0        0        0     6261 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/models/task.py
+-rw-r--r--   0        0        0      104 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/tasks/__init__.py
+-rw-r--r--   0        0        0    24638 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/tasks/local_task.py
+-rw-r--r--   0        0        0     8694 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/tasks/task_form.py
+-rw-r--r--   0        0        0     2764 2024-04-08 06:23:23.481295 nodeorc-0.1.3/nodeorc/utils.py
+-rw-r--r--   0        0        0     1282 2024-04-08 06:23:23.481295 nodeorc-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      106 2024-04-08 06:23:23.481295 nodeorc-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      422 2024-04-08 06:23:23.481295 nodeorc-0.1.3/service/10-toggleusbstick.rules
+-rw-r--r--   0        0        0     2107 2024-04-08 06:23:23.481295 nodeorc-0.1.3/service/usb-mount.sh
+-rw-r--r--   0        0        0      184 2024-04-08 06:23:23.481295 nodeorc-0.1.3/service/usb-mount@.service
+-rw-r--r--   0        0        0        0 2024-04-08 06:23:23.481295 nodeorc-0.1.3/settings/.gitkeep
+-rw-r--r--   0        0        0      722 2024-04-08 06:23:23.481295 nodeorc-0.1.3/settings/config_template.json
+-rwxr-xr-x   0        0        0    21564 2024-04-08 06:23:23.481295 nodeorc-0.1.3/setup.sh
+-rw-r--r--   0        0        0     8907 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0    60249 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/examples/ngwerere_transect.nc
+-rw-r--r--   0        0        0      496 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_amqp_task.py
+-rw-r--r--   0        0        0      802 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_callbacks.py
+-rw-r--r--   0        0        0     2493 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_config.py
+-rw-r--r--   0        0        0      875 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_disk_management.py
+-rw-r--r--   0        0        0      128 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_io.py
+-rw-r--r--   0        0        0      726 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_s3.py
+-rw-r--r--   0        0        0      184 2024-04-08 06:23:23.481295 nodeorc-0.1.3/tests/test_task.py
+-rw-r--r--   0        0        0    28618 1970-01-01 00:00:00.000000 nodeorc-0.1.3/PKG-INFO
```

### Comparing `nodeorc-0.1.2/.github/ISSUE_TEMPLATE/issue-report.md` & `nodeorc-0.1.3/.github/ISSUE_TEMPLATE/issue-report.md`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/.github/workflows/publish-release-pypi.yml` & `nodeorc-0.1.3/.github/workflows/publish-release-pypi.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/.github/workflows/publish-test-pypi.yml` & `nodeorc-0.1.3/.github/workflows/publish-test-pypi.yml`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
           repo_token: ${{ secrets.GITHUB_TOKEN }}
           tag: ${{ github.ref_name }}
           file: setup.sh
           overwrite: false
 
   upload-to-test-pypi:
     needs: test-built-dist
-    if: github.event_name == 'push'
+#    if: github.event_name == 'push'
     runs-on: ubuntu-latest
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: releases
           path: dist
       - name: Publish package to TestPyPI
```

### Comparing `nodeorc-0.1.2/.gitignore` & `nodeorc-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/Dockerfile` & `nodeorc-0.1.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/LICENSE` & `nodeorc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/README.rst` & `nodeorc-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/docker-compose-test.yml` & `nodeorc-0.1.3/docker-compose-test.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/docs/static/front.jpg` & `nodeorc-0.1.3/docs/static/front.jpg`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/mockserver/initializerJson.json` & `nodeorc-0.1.3/mockserver/initializerJson.json`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/callbacks.py` & `nodeorc-0.1.3/nodeorc/callbacks.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/config.py` & `nodeorc-0.1.3/nodeorc/config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/db/__init__.py` & `nodeorc-0.1.3/nodeorc/db/__init__.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/db/init_basedata.py` & `nodeorc-0.1.3/nodeorc/db/init_basedata.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/db/models.py` & `nodeorc-0.1.3/nodeorc/db/models.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/disk_mng.py` & `nodeorc-0.1.3/nodeorc/disk_mng.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/log.py` & `nodeorc-0.1.3/nodeorc/log.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/main.py` & `nodeorc-0.1.3/nodeorc/main.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/models/__init__.py` & `nodeorc-0.1.3/nodeorc/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/models/callback.py` & `nodeorc-0.1.3/nodeorc/models/callback.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/models/callback_url.py` & `nodeorc-0.1.3/nodeorc/models/callback_url.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/models/config.py` & `nodeorc-0.1.3/nodeorc/models/config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/models/storage.py` & `nodeorc-0.1.3/nodeorc/models/storage.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/models/subtask.py` & `nodeorc-0.1.3/nodeorc/models/subtask.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/models/task.py` & `nodeorc-0.1.3/nodeorc/models/task.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/tasks/local_task.py` & `nodeorc-0.1.3/nodeorc/tasks/local_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,15 @@
             # remove any left over temporary files
             shutil.rmtree(task_path)
 
     def _shutdown_or_not(self):
         if self.settings["shutdown_after_task"]:
             self.logger.info("Task done! Shutting down...")
             os.system("/sbin/shutdown -h now")
+            os.system("sudo /sbin/shutdown -h now")
 
     def _post_callbacks(self, callbacks):
         """
         Performs callbacks in a list, and returns True when all were successful
 
         Parameters
         ----------
```

### Comparing `nodeorc-0.1.2/nodeorc/tasks/task_form.py` & `nodeorc-0.1.3/nodeorc/tasks/task_form.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/nodeorc/utils.py` & `nodeorc-0.1.3/nodeorc/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,10 +96,10 @@
     if size1 != os.path.getsize(fn):
         return True
     else:
         return False
 
 
 def reboot_now():
-    os.system("/sbin/shutdown now")
+    os.system("/sbin/shutdown -r now")
     # in case this fails, do a sudo shutdown
-    os.system("sudo /sbin/shutdown now")
+    os.system("sudo /sbin/shutdown -r now")
```

### Comparing `nodeorc-0.1.2/pyproject.toml` & `nodeorc-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/service/usb-mount.sh` & `nodeorc-0.1.3/service/usb-mount.sh`

 * *Files 10% similar despite different names*

```diff
@@ -29,26 +29,14 @@
         echo "Warning: a device is already mounted at ${MOUNT_POINT}"
         exit 1
     fi
 
     # Get info for this drive: $ID_FS_LABEL, $ID_FS_UUID, and $ID_FS_TYPE
     eval $(/sbin/blkid -o udev ${DEVICE})
 
-    # # Figure out a mount point to use
-    # LABEL=${ID_FS_LABEL}
-    # if [[ -z "${LABEL}" ]]; then
-    #     LABEL=${DEVBASE}
-    # elif /bin/grep -q " /media/${LABEL} " /etc/mtab; then
-    #     # Already in use, make a unique one
-    #     LABEL+="-${DEVBASE}"
-    # fi
-    # MOUNT_POINT="/media/${LABEL}"
-    # 
-    # echo "Mount point: ${MOUNT_POINT}"
-
     /bin/mkdir -p ${MOUNT_POINT}
 
     # Global mount options
     OPTS="rw,relatime"
 
     # File system type specific mount options
     if [[ ${ID_FS_TYPE} == "vfat" ]]; then
```

### Comparing `nodeorc-0.1.2/settings/config_template.json` & `nodeorc-0.1.3/settings/config_template.json`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/setup.sh` & `nodeorc-0.1.3/setup.sh`

 * *Files 13% similar despite different names*

```diff
@@ -262,18 +262,126 @@
         export URL="N/A"
         export PASSWD_STRING="N/A"
     fi
 
 }
 
 setup_usb_mount() {
-    export usb_mount_script="${SCRIPT_FOLDER}/service/usb-mount.sh"
-    export usb_mount_service="${SCRIPT_FOLDER}/service/usb-mount@.service"
-    export udev_rule_usb="${SCRIPT_FOLDER}/service/10-toggleusbstick.rules"
+    export usb_mount_script="${HOME}/.nodeorc/service/usb-mount.sh"
+    export usb_mount_service="${HOME}/.nodeorc/service/usb-mount@.service"
+    export udev_rule_usb="${HOME}/.nodeorc/service/10-toggleusbstick.rules"
+	mkdir ${HOME}/.nodeorc/service
+	# create scripts
+	cat ${usb_mount_script} <<EOF
+#!/bin/bash
 
+# This script is called from our systemd unit file to mount or unmount
+# a USB drive.
+# adapted from https://serverfault.com/questions/766506/automount-usb-drives-with-systemd
+
+usage()
+{
+    echo "Usage: $0 {add|remove} device_name (e.g. sdb1)"
+    exit 1
+}
+
+if [[ $# -ne 2 ]]; then
+    usage
+fi
+
+ACTION=$1
+DEVBASE=$2
+DEVICE="/dev/${DEVBASE}"
+
+# See if this drive is already mounted, and if so where
+# MOUNT_POINT=$(/bin/mount | /bin/grep ${DEVICE} | /usr/bin/awk '{ print $3 }')
+MOUNT_POINT="/mnt/usb"
+
+do_mount()
+
+{
+    if [[ -d /mnt/usb ]] ; then
+        echo "Warning: a device is already mounted at ${MOUNT_POINT}"
+        exit 1
+    fi
+
+    # Get info for this drive: $ID_FS_LABEL, $ID_FS_UUID, and $ID_FS_TYPE
+    eval $(/sbin/blkid -o udev ${DEVICE})
+
+    /bin/mkdir -p ${MOUNT_POINT}
+
+    # Global mount options
+    OPTS="rw,relatime"
+
+    # File system type specific mount options
+    if [[ ${ID_FS_TYPE} == "vfat" ]]; then
+        OPTS+=",users,gid=100,umask=000,shortname=mixed,utf8=1,flush"
+    fi
+
+    if ! /bin/mount -o ${OPTS} ${DEVICE} ${MOUNT_POINT}; then
+        echo "Error mounting ${DEVICE} (status = $?)"
+        /bin/rmdir ${MOUNT_POINT}
+        exit 1
+    fi
+
+    echo "**** Mounted ${DEVICE} at ${MOUNT_POINT} ****"
+}
+
+do_unmount()
+{
+    if [[ -z ${MOUNT_POINT} ]]; then
+        echo "Warning: ${DEVICE} is not mounted"
+    else
+        /bin/umount -l ${DEVICE}
+        echo "**** Unmounted ${DEVICE}"
+    fi
+
+    # Delete all empty dirs in /media that aren't being used as mount
+    # points. This is kind of overkill, but if the drive was unmounted
+    # prior to removal we no longer know its mount point, and we don't
+    # want to leave it orphaned...
+    for f in /mnt/* ; do
+        if [[ -n $(/usr/bin/find "$f" -maxdepth 0 -type d -empty) ]]; then
+            if ! /bin/grep -q " $f " /etc/mtab; then
+                echo "**** Removing mount point $f"
+                /bin/rmdir "$f"
+            fi
+        fi
+    done
+}
+
+case "${ACTION}" in
+    add)
+        do_mount
+        ;;
+    remove)
+        do_unmount
+        ;;
+    *)
+        usage
+        ;;
+esac
+EOF
+	cat ${usb_mount_service} <<EOF
+[Unit]
+Description=Mount USB drive at /mnt/usb
+
+[Service]
+Type=oneshot
+RemainAfterExit=yes
+ExecStart=/usr/local/bin/usb-mount.sh add %i
+ExecStop=/usr/local/bin/usb-mount.sh remove %i
+EOF
+
+	cat ${udev_rule_usb} <<EOF
+SUBSYSTEMS=="usb", KERNEL=="sd[a-z][0-9]", ACTION=="add", RUN+="/bin/systemctl start usb-mount@%k.service"
+SUBSYSTEMS=="usb", KERNEL=="sd[a-z][0-9]", ACTION=="remove", RUN+="/bin/systemctl stop usb-mount@%k.service"
+SUBSYSTEMS=="usb", KERNEL=="sd[a-z]", ACTION=="add", RUN+="/bin/systemctl start usb-mount@%k.service"
+SUBSYSTEMS=="usb", KERNEL=="sd[a-z]", ACTION=="remove", RUN+="/bin/systemctl stop usb-mount@%k.service"
+EOF
     # move usb mount in place and make executable
     echo "Making USB mount script available for running as a service"
     sudo cp $usb_mount_script /usr/local/bin
     # make usb mount script executable
     sudo chmod +x /usr/local/bin/usb-mount.sh
 
     # setup a systemctl service for mounting USB drives
```

### Comparing `nodeorc-0.1.2/tests/conftest.py` & `nodeorc-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/tests/examples/ngwerere_transect.nc` & `nodeorc-0.1.3/tests/examples/ngwerere_transect.nc`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/tests/test_callbacks.py` & `nodeorc-0.1.3/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/tests/test_config.py` & `nodeorc-0.1.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/tests/test_disk_management.py` & `nodeorc-0.1.3/tests/test_disk_management.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/tests/test_s3.py` & `nodeorc-0.1.3/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.2/PKG-INFO` & `nodeorc-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodeorc
-Version: 0.1.2
+Version: 0.1.3
 Summary: NodeORC: Automated edge and cloud image-based discharge estimation with OpenRiverCam
 Author-email: Hessel Winsemius <winsemius@rainbowsensing.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

