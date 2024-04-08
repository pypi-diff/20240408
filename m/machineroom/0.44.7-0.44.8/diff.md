# Comparing `tmp/machineroom-0.44.7.tar.gz` & `tmp/machineroom-0.44.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.44.7.tar", last modified: Sat Mar 23 17:15:27 2024, max compression
+gzip compressed data, was "machineroom-0.44.8.tar", last modified: Mon Apr  8 17:21:27 2024, max compression
```

## Comparing `machineroom-0.44.7.tar` & `machineroom-0.44.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-23 17:15:27.949870 machineroom-0.44.7/
--rw-r--r--   0 root         (0) staff       (20)     2358 2024-02-29 11:53:06.000000 machineroom-0.44.7/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.44.7/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4392 2024-03-23 17:15:27.949697 machineroom-0.44.7/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.44.7/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-23 17:15:27.940543 machineroom-0.44.7/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.44.7/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-23 17:15:27.943685 machineroom-0.44.7/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-03-23 17:15:27.000000 machineroom-0.44.7/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4659 2024-03-23 16:46:52.000000 machineroom-0.44.7/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.44.7/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    13315 2024-03-22 10:56:07.000000 machineroom-0.44.7/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    18072 2024-03-23 17:14:57.000000 machineroom-0.44.7/machineroom/taskbase.py
--rw-r--r--   0 root         (0) staff       (20)    14366 2024-03-23 02:49:04.000000 machineroom-0.44.7/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     2759 2024-03-23 02:51:57.000000 machineroom-0.44.7/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-23 17:15:27.949053 machineroom-0.44.7/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4392 2024-03-23 17:15:27.000000 machineroom-0.44.7/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      371 2024-03-23 17:15:27.000000 machineroom-0.44.7/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-03-23 17:15:27.000000 machineroom-0.44.7/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-03-23 17:15:27.000000 machineroom-0.44.7/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-03-23 17:15:27.950744 machineroom-0.44.7/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2569 2024-03-01 08:09:46.000000 machineroom-0.44.7/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1534 2024-03-23 02:40:33.000000 machineroom-0.44.7/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-03-23 17:15:21.000000 machineroom-0.44.7/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-08 17:21:27.901847 machineroom-0.44.8/
+-rw-r--r--   0 root         (0) staff       (20)     2358 2024-02-29 11:53:06.000000 machineroom-0.44.8/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.44.8/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-08 17:21:27.901586 machineroom-0.44.8/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.44.8/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-08 17:21:27.895235 machineroom-0.44.8/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.44.8/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-08 17:21:27.898256 machineroom-0.44.8/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-08 17:21:27.000000 machineroom-0.44.8/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5253 2024-04-08 17:15:42.000000 machineroom-0.44.8/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.44.8/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    13315 2024-03-22 10:56:07.000000 machineroom-0.44.8/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    19373 2024-04-08 17:20:01.000000 machineroom-0.44.8/machineroom/taskbase.py
+-rw-r--r--   0 root         (0) staff       (20)    14368 2024-04-08 17:07:54.000000 machineroom-0.44.8/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     2759 2024-03-23 02:51:57.000000 machineroom-0.44.8/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-08 17:21:27.900807 machineroom-0.44.8/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-08 17:21:27.000000 machineroom-0.44.8/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      371 2024-04-08 17:21:27.000000 machineroom-0.44.8/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-08 17:21:27.000000 machineroom-0.44.8/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-08 17:21:27.000000 machineroom-0.44.8/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-08 17:21:27.902618 machineroom-0.44.8/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2569 2024-03-01 08:09:46.000000 machineroom-0.44.8/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1534 2024-03-23 02:40:33.000000 machineroom-0.44.8/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-08 17:21:09.000000 machineroom-0.44.8/version
```

### Comparing `machineroom-0.44.7/.gitignore` & `machineroom-0.44.8/.gitignore`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.7/LICENSE` & `machineroom-0.44.8/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.7/PKG-INFO` & `machineroom-0.44.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.44.7
+Version: 0.44.8
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.44.7/README.md` & `machineroom-0.44.8/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.7/cmdbin/connect` & `machineroom-0.44.8/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.7/machineroom/__init__.py` & `machineroom-0.44.8/machineroom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.44.7'
+__version__ = '0.44.8'
```

### Comparing `machineroom-0.44.7/machineroom/const.py` & `machineroom-0.44.8/machineroom/const.py`

 * *Files 11% similar despite different names*

```diff
@@ -109,7 +109,26 @@
 DOCKER_STOP_REMOVE = """{COMMAND_DOCKER} rm $({COMMAND_DOCKER} stop $(sudo docker ps -a | grep "{CONTAINER_NAME}" | cut -d " " -f 1))"""
 DOCKER_LAUNCH_LINE = """{COMMAND_DOCKER} run -d -v {VOLUME} --restart unless-stopped --name {NODE_NAME} {IMAGE}:{VERSION} {COMMAND}"""
 DOCKER_STOP_ID = """{COMMAND_DOCKER} stop {CID}"""
 DOCKER_STOP_RM = """{COMMAND_DOCKER} rm {CID}"""
 DOCKER_STOP_CONTAIN_NAME = """{COMMAND_DOCKER} ps -a | grep '{CONTAINER_NAME}' | awk '{{print $1}}' | xargs {COMMAND_DOCKER} stop"""
 DOCKER_RM_NAME_BASED = """{COMMAND_DOCKER} ps -a | grep '{CONTAINER_NAME}' | awk '{{print $1}}' | xargs -r {COMMAND_DOCKER} rm -f"""
 DOCKER_RM_VOLUME = """{COMMAND_DOCKER} volume ls -qf dangling=true -f name={CONTAINER_NAME} | xargs -r {COMMAND_DOCKER} volume rm"""
+DOCKER_LOG_REVIEW = """COMMAND_DOCKER ps -a --filter "name=__CONTAINER_KEYWORD" --format "{{.ID}}" | shuf -n 1 | xargs docker logs --tail __RECENT_LINES"""
+
+BACKUP_CACHE_FAST = """
+# Define the path to the file
+path_to_file="_CFP_"
+# Check if the file exists
+if [ -f "$path_to_file" ]; then
+    # Go to the directory of the file
+    cd "$(dirname "$path_to_file")" || exit
+    # Gzip the file
+    while :
+        do
+            tar -czvf _FR_ $(basename "$path_to_file")
+            if [ $? -eq 0 ]; then
+                break
+            fi
+        done
+    echo "compress file success"
+fi"""
```

### Comparing `machineroom-0.44.7/machineroom/schema.json` & `machineroom-0.44.8/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.7/machineroom/sql.py` & `machineroom-0.44.8/machineroom/sql.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.7/machineroom/taskbase.py` & `machineroom-0.44.8/machineroom/taskbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,20 +42,14 @@
     if if_not_exist is True:
         if exists(c, remote_path) is False:
             c.put(local_path, remote_path)
     else:
         c.put(local_path, remote_path)
 
 
-def download_cache_file(c: Connection, cache_file_name: str):
-    remote_path = os.path.join(Config.REMOTE_WS, "cache", cache_file_name)
-    local_path = os.path.join(Config.WS_LOCAL, "cache", cache_file_name)
-    c.get(remote_path, local_path)
-
-
 # https://fabric-zh.readthedocs.io/_/downloads/zh-cn/latest/pdf/
 def detect_cert(c: Connection) -> bool:
     r = c.run("cat ~/.ssh/authorized_keys", warn=True)
     line = str(r.stdout.strip().replace("\n", ""))
     t = True if Config.MY_KEY_FEATURE in line else False
     if t is True:
         print(f"certification found {Config.MY_KEY_FEATURE}")
@@ -159,14 +153,50 @@
     cmd0 = f'cd {working_path} && {Config.BASH} {bash_file}'
     cmd1 = f'cd {working_path} && echo "" > {bash_file}'
     result = c.run(cmd0, pty=True, timeout=3000, warn=True)
     if result.ok and empty_content_after_execution:
         result = c.run(cmd1, pty=True, timeout=3600, warn=True)
     return result
 
+# Back up related commands
+def safe_cache_backup(c: Connection, local_file_name: str):
+    """
+    safely backup the working cache file in the remote server
+    download the gz db to local
+    """
+    original_rm = os.path.join(Config.REMOTE_WS, "cache", "cache.db")
+    remote_path = os.path.join(Config.REMOTE_WS, "cache", local_file_name)
+    t = BACKUP_CACHE_FAST.replace("_CFP_", original_rm).replace("_FR_", local_file_name)
+    exec_shell_program(c, "/tmp", t)
+    local_path = os.path.join(Config.WS_LOCAL, "cache", "server_backups", local_file_name)
+    c.get(remote_path, local_path)
+    print("Download successful")
+    return local_path
+
+
+def open_backup_cache_local(local_path) -> str:
+    """
+    the final local path of the cache file backup
+    """
+    local_fz = os.path.join(Config.WS_LOCAL, "cache", "server_backups", "cache.db")
+    (p, f) = os.path.split(local_path)
+    # local_compressed = os.path.join(WS_LOCAL, "cache", local_file_name)
+    # local_fz = os.path.join(WS_LOCAL, "cache", local_file_name.replace(".tar.gz", ""))
+    # db_name_x = f.replace(".tar.gz", "")
+    # local_pd = os.path.join(WS_LOCAL, "cache")
+    local_cmd = f'cd {p} && tar -xvf {f}'
+    print(local_cmd)
+    os.system(local_cmd)
+    # os.renames("cache.db", db_name_x)
+    os.chdir(Config.WS_LOCAL)
+    # return os.path.join(p, db_name_x)
+    return local_fz
+
+
+# Docker related commands in library
 
 def exec_docker_compose(c: Connection, working_path: str, yml_file: str, upgrade: bool = False) -> Result:
     cmd0 = f"cd {working_path} &&"
     if yml_file == "docker-compose.yml":
         if upgrade:
             cmd0 = cmd0 + f"{Config.DOCKER_COMPOSE} pull &&"
         cmd1 = cmd0 + f'{Config.DOCKER_COMPOSE} up -d'
@@ -246,18 +276,22 @@
     cmd_line_go = DOCKER_RM_VOLUME.format(
         COMMAND_DOCKER=Config.DOCKER,
         CONTAINER_NAME=container_name
     )
     return c.run(cmd_line_go, pty=True, timeout=1900, warn=True, echo=True)
 
 
-def download_cache_file_with_server_side(c: Connection, server: int):
-    remote_path = os.path.join(Config.REMOTE_WS, "cache", "cache.db")
-    local_path = os.path.join(Config.WS_LOCAL, "cache", f"server_cache_{server}.db")
-    c.get(remote_path, local_path)
+def log_review(c: Connection, container_word: str, log_recent_lines: int):
+    """
+    show the docker logs
+    """
+    pick_logs = DOCKER_LOG_REVIEW.replace("COMMAND_DOCKER", Config.DOCKER)
+    pick_logs = pick_logs.replace("__CONTAINER_KEYWORD", container_word)
+    pick_logs = pick_logs.replace("__RECENT_LINES", log_recent_lines)
+    return c.run(pick_logs, pty=True, timeout=1900, warn=True, echo=True)
 
 
 def exec_container_program(c: Connection, container_id: str, bash_line: str) -> Result:
     cmd2 = f'{Config.DOCKER} exec {container_id} {bash_line} &'
     return c.run(cmd2, pty=True, timeout=900, warn=True)
```

### Comparing `machineroom-0.44.7/machineroom/util.py` & `machineroom-0.44.8/machineroom/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,15 @@
             "user": line[2],
             "pass": line[3]
         }
         self.current_id = line[0]
         self.current_host = line[1]
         self.current_user = line[2]
         self.current_pass = line[3]
-        print(f"######## Now enter server ID#{n}: {line[0]} {line[1]}")
+        print(f"## ☎️ Now enter network ID#{n}: {line[0]} {line[1]}")
         return tmp
 
     def use_next_node(self) -> dict:
         self._srv_index = self._srv_index + 1
         return self.read_serv_at(self._srv_index)
```

### Comparing `machineroom-0.44.7/machineroom/worker.py` & `machineroom-0.44.8/machineroom/worker.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.7/machineroom.egg-info/PKG-INFO` & `machineroom-0.44.8/machineroom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.44.7
+Version: 0.44.8
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.44.7/setup.py` & `machineroom-0.44.8/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.7/update` & `machineroom-0.44.8/update`

 * *Files identical despite different names*

