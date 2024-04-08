# Comparing `tmp/bakabakabaka-0.7.7.tar.gz` & `tmp/bakabakabaka-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bakabakabaka-0.7.7.tar", last modified: Sun Mar 20 17:24:02 2022, max compression
+gzip compressed data, was "bakabakabaka-0.8.0.tar", last modified: Mon Apr  8 21:10:54 2024, max compression
```

## Comparing `bakabakabaka-0.7.7.tar` & `bakabakabaka-0.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-20 17:24:02.266107 bakabakabaka-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-03-20 17:23:52.000000 bakabakabaka-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-03-20 17:24:02.266107 bakabakabaka-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-03-20 17:23:52.000000 bakabakabaka-0.7.7/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)    26908 2022-03-20 17:23:52.000000 bakabakabaka-0.7.7/baka.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-20 17:24:02.266107 bakabakabaka-0.7.7/bakabakabaka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-03-20 17:24:02.000000 bakabakabaka-0.7.7/bakabakabaka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-03-20 17:24:02.000000 bakabakabaka-0.7.7/bakabakabaka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-20 17:24:02.000000 bakabakabaka-0.7.7/bakabakabaka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-03-20 17:24:02.000000 bakabakabaka-0.7.7/bakabakabaka.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-03-20 17:24:02.000000 bakabakabaka-0.7.7/bakabakabaka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-20 17:24:02.266107 bakabakabaka-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-03-20 17:23:52.000000 bakabakabaka-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:54.966357 bakabakabaka-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 21:10:46.000000 bakabakabaka-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-08 21:10:54.966357 bakabakabaka-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-08 21:10:46.000000 bakabakabaka-0.8.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32081 2024-04-08 21:10:46.000000 bakabakabaka-0.8.0/baka.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:54.966357 bakabakabaka-0.8.0/bakabakabaka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-08 21:10:54.000000 bakabakabaka-0.8.0/bakabakabaka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 21:10:54.000000 bakabakabaka-0.8.0/bakabakabaka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:10:54.000000 bakabakabaka-0.8.0/bakabakabaka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 21:10:54.000000 bakabakabaka-0.8.0/bakabakabaka.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 21:10:54.000000 bakabakabaka-0.8.0/bakabakabaka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:10:54.966357 bakabakabaka-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-08 21:10:46.000000 bakabakabaka-0.8.0/setup.py
```

### Comparing `bakabakabaka-0.7.7/LICENSE` & `bakabakabaka-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bakabakabaka-0.7.7/PKG-INFO` & `bakabakabaka-0.8.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 Metadata-Version: 2.1
 Name: bakabakabaka
-Version: 0.7.7
+Version: 0.8.0
 Summary: the stupid configuration tracker using the stupid content tracker
 Home-page: https://github.com/elesiuta/baka
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # baka admin konfiguration assistant
-This is mostly just a wrapper for some git and rsync commands I made to help with managing my home server  
+This is mostly just a wrapper around git along with some other commands to help with managing servers or home directories  
 If you're looking for something similar but not stupid, see [etckeeper](https://wiki.archlinux.org/title/Etckeeper) or other [alternatives](https://wiki.archlinux.org/title/Dotfiles)  
 Otherwise, you can install from [PyPI](https://pypi.org/project/bakabakabaka/) with `pip install bakabakabaka`  
 ```
 usage: baka [--dry-run] <argument>
 
 the stupid configuration tracker using the stupid content tracker
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   --version      show program's version number and exit
   --init         open config, init git repo, add files then commit
   --commit msg   git add and commit your changes to tracked files
   --push         git push (caution, ensure remote is private)
+  --pull         git pull (does not restore files over system)
   --untrack ...  untrack path(s) from git
   --install ...  install package(s) and commit changes
   --remove ...   remove package(s) and commit changes
   --upgrade      upgrade packages on system and commit changes
   --docker ...   usage: --docker <up|down|pull> <all|names...>
+  --podman ...   usage: --podman <up|down|pull> <all|names...>
+  --file ...     usage: --file <save|restore> <all|names...>
   --job name     run commands for job with name
   --list         show list of jobs
-  --sysck        run commands for system checks and commit output
+  --sysck        run commands for system checks and commits output
   --scan         run commands for scanning system, prints and commits output
   --diff         show git diff --color-words
   --log          show pretty git log
   --show         show most recent commit
+  -e             toggles 'exit_non_zero' setting for current run of job
+  -y             supplies 'y' to job commands, similar to yes | job
   -i             force job to run in interactive mode
   -n, --dry-run  print commands instead of executing them
 ```
-
-
```

### Comparing `bakabakabaka-0.7.7/README.md` & `bakabakabaka-0.8.0/bakabakabaka.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,46 @@
+Metadata-Version: 2.1
+Name: bakabakabaka
+Version: 0.8.0
+Summary: the stupid configuration tracker using the stupid content tracker
+Home-page: https://github.com/elesiuta/baka
+License: GPLv3
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # baka admin konfiguration assistant
-This is mostly just a wrapper for some git and rsync commands I made to help with managing my home server  
+This is mostly just a wrapper around git along with some other commands to help with managing servers or home directories  
 If you're looking for something similar but not stupid, see [etckeeper](https://wiki.archlinux.org/title/Etckeeper) or other [alternatives](https://wiki.archlinux.org/title/Dotfiles)  
 Otherwise, you can install from [PyPI](https://pypi.org/project/bakabakabaka/) with `pip install bakabakabaka`  
 ```
 usage: baka [--dry-run] <argument>
 
 the stupid configuration tracker using the stupid content tracker
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   --version      show program's version number and exit
   --init         open config, init git repo, add files then commit
   --commit msg   git add and commit your changes to tracked files
   --push         git push (caution, ensure remote is private)
+  --pull         git pull (does not restore files over system)
   --untrack ...  untrack path(s) from git
   --install ...  install package(s) and commit changes
   --remove ...   remove package(s) and commit changes
   --upgrade      upgrade packages on system and commit changes
   --docker ...   usage: --docker <up|down|pull> <all|names...>
+  --podman ...   usage: --podman <up|down|pull> <all|names...>
+  --file ...     usage: --file <save|restore> <all|names...>
   --job name     run commands for job with name
   --list         show list of jobs
-  --sysck        run commands for system checks and commit output
+  --sysck        run commands for system checks and commits output
   --scan         run commands for scanning system, prints and commits output
   --diff         show git diff --color-words
   --log          show pretty git log
   --show         show most recent commit
+  -e             toggles 'exit_non_zero' setting for current run of job
+  -y             supplies 'y' to job commands, similar to yes | job
   -i             force job to run in interactive mode
   -n, --dry-run  print commands instead of executing them
 ```
```

### Comparing `bakabakabaka-0.7.7/baka.py` & `bakabakabaka-0.8.0/baka.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,86 +15,106 @@
 
 # https://github.com/elesiuta/baka
 
 import argparse
 import datetime
 import email
 import email.mime.text
+import hashlib
 import json
 import os
 import shlex
 import shutil
 import smtplib
+import socket
 import subprocess
 import sys
 import time
 
-VERSION = "0.7.7"
+VERSION = "0.8.0"
 BASE_PATH = os.path.expanduser("~/.baka")
 
 
 def init_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(description="the stupid configuration tracker using the stupid content tracker",
                                      usage="%(prog)s [--dry-run] <argument>")
     parser.add_argument("--version", action="version", version=VERSION)
     maingrp = parser.add_mutually_exclusive_group()
-    maingrp.add_argument("--_copy_conditional_paths", dest="copy_conditional_paths", action="store_true",
+    maingrp.add_argument("--_hash_and_copy_files", dest="hash_and_copy_files", action="store_true",
                          help=argparse.SUPPRESS)
     maingrp.add_argument("--init", dest="init", action="store_true",
                          help="open config, init git repo, add files then commit")
     maingrp.add_argument("--commit", dest="commit", type=str, metavar="msg",
                          help="git add and commit your changes to tracked files")
     maingrp.add_argument("--push", dest="push", action="store_true",
                          help="git push (caution, ensure remote is private)")
+    maingrp.add_argument("--pull", dest="pull", action="store_true",
+                         help="git pull (does not restore files over system)")
     maingrp.add_argument("--untrack", dest="untrack", nargs=argparse.REMAINDER,
                          help="untrack path(s) from git")
     maingrp.add_argument("--install", dest="install", nargs=argparse.REMAINDER,
                          help="install package(s) and commit changes")
     maingrp.add_argument("--remove", dest="remove", nargs=argparse.REMAINDER, default=None,
                          help="remove package(s) and commit changes")
     maingrp.add_argument("--upgrade", dest="upgrade", action="store_true",
                          help="upgrade packages on system and commit changes")
     maingrp.add_argument("--docker", dest="docker", nargs=argparse.REMAINDER,
                          help="usage: --docker <up|down|pull> <all|names...>")
+    maingrp.add_argument("--podman", dest="podman", nargs=argparse.REMAINDER,
+                         help="usage: --podman <up|down|pull> <all|names...>")
+    maingrp.add_argument("--file", dest="file", nargs=argparse.REMAINDER,
+                         help="usage: --file <save|restore> <all|names...>")
     maingrp.add_argument("--job", dest="job", type=str, metavar="name",
                          help="run commands for job with name")
     maingrp.add_argument("--list", dest="list", action="store_true",
                          help="show list of jobs")
     maingrp.add_argument("--sysck", dest="system_checks", action="store_true",
-                         help="run commands for system checks and commit output")
+                         help="run commands for system checks and commits output")
     maingrp.add_argument("--scan", dest="system_scans", action="store_true",
                          help="run commands for scanning system, prints and commits output")
     maingrp.add_argument("--diff", dest="diff", action="store_true",
                          help="show git diff --color-words")
     maingrp.add_argument("--log", dest="log", action="store_true",
                          help="show pretty git log")
     maingrp.add_argument("--show", dest="show", action="store_true",
                          help="show most recent commit")
+    parser.add_argument("-e", dest="exit_zero_toggle", action="store_true",
+                        help="toggles 'exit_non_zero' setting for current run of job")
+    parser.add_argument("-y", dest="yes", action="store_true",
+                        help="supplies 'y' to job commands, similar to yes | job")
     parser.add_argument("-i", dest="interactive", action="store_true",
                         help="force job to run in interactive mode")
     parser.add_argument("-n", "--dry-run", dest="dry_run", action="store_true",
                         help="print commands instead of executing them")
     return parser
 
 
 class Config:
     def __init__(self):
         # default config
         self.cmd_install = ["sudo", "apt", "install"]
         self.cmd_remove = ["sudo", "apt", "autoremove", "--purge"]
-        self.cmd_upgrade = ["bash", "-c", "sudo apt update && sudo apt upgrade"]
+        self.cmd_upgrade = ["bash", "-c", "sudo apt update && sudo apt dist-upgrade"]
         self.email = {
             "cc": None,
             "from": "myemail@domain.com",
             "html": True,
             "smtp_server": "smtp.domain.com",
             "smtp_port": 587,
             "smtp_username": "username",
             "smtp_password": "password"
         }
+        self.files = {
+            "example_file_a": {
+                "src": "path/to/file",
+            },
+            "example_file_b": {
+                "cmd": ["echo", "command to generate file"],
+            }
+        }
         self.jobs = {
             "example_job_name": {
                 "commands": [
                     ["echo", "hello world"],
                     ["echo", "task completed"]
                 ],
                 "email": {
@@ -132,106 +152,137 @@
             os.path.expanduser("~/.kde/share"): {"max_depth": 3, "max_size": 128000},
             os.path.expanduser("~/.local/share"): {"max_depth": 3, "max_size": 128000, "exclude": ["application_state"]},
         }.items() if os.path.exists(k)}
         # read config file and set values, or write if it does not exist
         config_path = os.path.join(BASE_PATH, "config.json")
         if os.path.exists(config_path):
             with open(config_path, "r", encoding="utf-8", errors="surrogateescape") as json_file:
-                config = json.load(json_file)
+                # remove comments from json file
+                raw_text = json_file.readlines()
+                for i in reversed(range(len(raw_text))):
+                    if raw_text[i].lstrip().startswith("#"):
+                        _ = raw_text.pop(i)
+                config = json.loads("".join(raw_text))
             for key in config:
                 if config[key] is not None and hasattr(self, key):
                     self.__setattr__(key, config[key])
             for tracked_path in self.tracked_paths:
                 assert os.path.isabs(tracked_path)
         else:
             if not os.path.isdir(os.path.dirname(config_path)):
                 os.makedirs(os.path.dirname(config_path))
             with open(config_path, "w", encoding="utf-8", errors="surrogateescape") as json_file:
                 json.dump(vars(self), json_file, indent=2, separators=(',', ': '), sort_keys=True, ensure_ascii=False)
+        # get the system hostname, usually /etc/hostname but can override with .baka/hostname (not in config.json or committed)
+        if os.path.exists(os.path.join(BASE_PATH, "hostname")):
+            with open(os.path.join(BASE_PATH, "hostname"), "r") as f:
+                self.hostname = f.read().strip()
+        else:
+            self.hostname = socket.gethostname()
 
 
 def os_stat_tracked_files(config: "Config") -> None:
     stat = {}
     for tracked_path in list(config.tracked_paths):
         if os.path.isdir(tracked_path):
-            for root, dirs, files in os.walk(BASE_PATH + tracked_path):
+            for root, dirs, files in os.walk(BASE_PATH + tracked_path, followlinks=False):
                 for file_or_folder in files + dirs:
                     file_path = "/" + os.path.relpath(os.path.join(root, file_or_folder), BASE_PATH)
                     if os.path.exists(file_path):
                         file_stat = os.stat(file_path)
                         stat[file_path] = {"mode": oct(file_stat.st_mode), "uid": file_stat.st_uid, "gid": file_stat.st_gid}
         elif os.path.isfile(tracked_path):
             file_path = tracked_path
             if os.path.exists(BASE_PATH + file_path):
                 file_stat = os.stat(file_path)
                 stat[file_path] = {"mode": oct(file_stat.st_mode), "uid": file_stat.st_uid, "gid": file_stat.st_gid}
     with open(os.path.join(BASE_PATH, "stat.json"), "w", encoding="utf-8", errors="surrogateescape") as json_file:
         json.dump(stat, json_file, indent=2, separators=(',', ': '), sort_keys=True, ensure_ascii=False)
 
 
-def copy_conditional_paths(config: "Config") -> None:
+def hash_and_copy_files(config: "Config") -> None:
+    # also keep track of hashes, need to read the files anyways and can save on writes
+    new_hashes = {}
+    old_hashes = {}
+    if os.path.exists(os.path.join(BASE_PATH, "sha256.json")):
+        with open(os.path.join(BASE_PATH, "sha256.json"), "r", encoding="utf-8", errors="surrogateescape") as json_file:
+            old_hashes = json.load(json_file)
     for tracked_path in config.tracked_paths:
-        if config.tracked_paths[tracked_path]:
-            conditions = {"exclude": [], "file_starts_with": "", "path_starts_with": "", "max_depth": None, "max_size": None}
-            for condition in config.tracked_paths[tracked_path]:
-                conditions[condition] = config.tracked_paths[tracked_path][condition]
-            for root, dirs, files in os.walk(tracked_path):
-                relpath = os.path.relpath(root, tracked_path)
-                if root.startswith(BASE_PATH):
+        # set default values (no conditions) and load conditions for which files to track/copy
+        conditions = {"exclude": [], "file_starts_with": "", "path_starts_with": "", "max_depth": None, "max_size": None, "test_utf_readable": True}
+        for condition in config.tracked_paths[tracked_path]:
+            conditions[condition] = config.tracked_paths[tracked_path][condition]
+        for root, dirs, files in os.walk(tracked_path, followlinks=False):
+            # check conditions
+            relpath = os.path.relpath(root, tracked_path)
+            if root.startswith(BASE_PATH):
+                del dirs
+                continue
+            if conditions["path_starts_with"] and not (relpath.startswith(conditions["path_starts_with"]) or conditions["path_starts_with"].startswith(relpath)):
+                del dirs
+                continue
+            for file in files:
+                file_path = os.path.join(root, file)
+                file_relpath = os.path.relpath(file_path, tracked_path)
+                if conditions["max_depth"] and file_relpath.count("/") >= conditions["max_depth"]:
                     del dirs
+                    break
+                if conditions["exclude"] and any(e in file_relpath for e in conditions["exclude"]):
                     continue
-                if conditions["path_starts_with"] and not (relpath.startswith(conditions["path_starts_with"]) or conditions["path_starts_with"].startswith(relpath)):
-                    del dirs
+                if conditions["file_starts_with"] and not file.startswith(conditions["file_starts_with"]):
                     continue
-                for file in files:
-                    file_path = os.path.join(root, file)
-                    file_relpath = os.path.relpath(file_path, tracked_path)
-                    if conditions["max_depth"] and file_relpath.count("/") >= conditions["max_depth"]:
-                        del dirs
-                        break
-                    if conditions["exclude"] and any(e in file_relpath for e in conditions["exclude"]):
-                        continue
-                    if conditions["file_starts_with"] and not file.startswith(conditions["file_starts_with"]):
-                        continue
-                    if conditions["path_starts_with"] and not file_relpath.startswith(conditions["path_starts_with"]):
+                if conditions["path_starts_with"] and not file_relpath.startswith(conditions["path_starts_with"]):
+                    continue
+                try:
+                    if conditions["max_size"] and not os.path.islink(file_path) and os.stat(file_path).st_size > conditions["max_size"]:
                         continue
-                    try:
-                        if conditions["max_size"] and not os.path.islink(file_path) and os.stat(file_path).st_size > conditions["max_size"]:
+                    if not os.path.isfile(file_path):
+                        raise FileNotFoundError("not a file")
+                    if conditions["test_utf_readable"]:
+                        try:
+                            with open(file_path, "r", encoding="utf-8") as f:
+                                _ = f.read(1)
+                        except UnicodeDecodeError:
                             continue
-                        if not os.path.isfile(file_path):
-                            continue
-                        with open(file_path, "r", encoding="utf-8") as f:
-                            _ = f.read(1)
-                        copy_path = BASE_PATH + file_path
-                        if os.path.exists(copy_path) and not os.path.islink(copy_path):
-                            os.chmod(copy_path, 0o200)
-                        elif not os.path.isdir(os.path.dirname(copy_path)):
-                            os.makedirs(os.path.dirname(copy_path))
-                        shutil.copy2(file_path, copy_path, follow_symlinks=False)
-                    except Exception:
-                        pass
-            for root, dirs, files in os.walk(BASE_PATH + tracked_path):
-                for file in files:
-                    if not os.path.exists("/" + os.path.relpath(os.path.join(root, file), BASE_PATH)):
-                        if not os.path.islink(os.path.join(root, file)):
-                            os.chmod(os.path.join(root, file), 0o200)
-                        os.remove(os.path.join(root, file))
-
-
-def rsync_and_git_add_all(config: "Config") -> list:
-    cmds = []
-    if any(config.tracked_paths[tracked_path] for tracked_path in config.tracked_paths):
-        cmds.append([sys.executable, os.path.abspath(__file__), "--_copy_conditional_paths"])
-    for tracked_path in config.tracked_paths:
-        if not config.tracked_paths[tracked_path]:
-            assert not (tracked_path.startswith(BASE_PATH) or BASE_PATH.startswith(tracked_path)), "directory recursion"
-            if not os.path.exists(os.path.dirname(BASE_PATH + tracked_path)):
-                os.makedirs(os.path.dirname(BASE_PATH + tracked_path))
-            cmds.append(["rsync", "-rlpt", "--delete", tracked_path, os.path.dirname(BASE_PATH + tracked_path)])
-    cmds.append(["git", "add", "--ignore-errors", "--all"])
+                    # all conditions met, hash and copy file if changed
+                    copy_path = BASE_PATH + file_path
+                    with open(file_path, "rb") as f:
+                        file_contents = f.read()
+                        new_hash = hashlib.sha256(file_contents).hexdigest()
+                        new_hashes[file_path] = new_hash
+                    if new_hash == old_hashes.get(file_path, ""):
+                        continue
+                    # dest might be readonly since permissions are copied, temporarily make it writable
+                    if os.path.exists(copy_path) and not os.path.islink(copy_path):
+                        os.chmod(copy_path, 0o200)
+                    elif not os.path.isdir(os.path.dirname(copy_path)):
+                        os.makedirs(os.path.dirname(copy_path))
+                    with open(copy_path, "wb") as f:
+                        f.write(file_contents)
+                    shutil.copystat(file_path, copy_path, follow_symlinks=False)
+                    del file_contents
+                except Exception as e:
+                    print("Error: %s %s for %s" % (type(e).__name__, e.args, file_path), file=sys.stderr)
+        # remove copies of tracked files that no longer exist on system
+        for root, dirs, files in os.walk(BASE_PATH + tracked_path):
+            for file in files:
+                if not os.path.exists("/" + os.path.relpath(os.path.join(root, file), BASE_PATH)):
+                    if not os.path.islink(os.path.join(root, file)):
+                        os.chmod(os.path.join(root, file), 0o200)
+                    os.remove(os.path.join(root, file))
+    # write new hashes
+    with open(os.path.join(BASE_PATH, "sha256.json"), "w", encoding="utf-8", errors="surrogateescape") as json_file:
+        json.dump(new_hashes, json_file, indent=2, separators=(',', ': '), sort_keys=True, ensure_ascii=False)
+
+
+def copy_and_git_add_all() -> list[list[str]]:
+    cmds = [
+        [sys.executable, os.path.abspath(__file__), "--_hash_and_copy_files"],
+        ["git", "add", "--ignore-errors", "--all"]
+    ]
     return cmds
 
 
 def send_email(config_email: dict, job_email: dict, body: str) -> int:
     message = email.message.EmailMessage()
     message["From"] = config_email["from"]
     message["To"] = job_email["to"]
@@ -246,74 +297,88 @@
         smtp_server_instance.starttls()
         smtp_server_instance.login(config_email["smtp_username"], config_email["smtp_password"])
         smtp_server_instance.send_message(message)
     return 0
 
 
 def main() -> int:
+    if sys.flags.optimize > 0:
+        print("Warning: baka does not function properly with the -O (optimize) flag", file=sys.stderr)
     # parse arguments
     parser = init_parser()
     args = parser.parse_args()
     # init config
     config = Config()
     # change cwd to repo folder
     original_cwd = os.getcwd()
     os.chdir(BASE_PATH)
     # select commands
-    if args.copy_conditional_paths:
-        copy_conditional_paths(config)
+    if args.hash_and_copy_files:
+        hash_and_copy_files(config)
         return 0
     elif args.init:
         # option to edit then reload config
         _ = input("Press enter to open your config file with nano")
         if args.dry_run:
             print(shlex.join(["nano", os.path.join(BASE_PATH, "config.json")]))
         else:
             subprocess.run(["nano", os.path.join(BASE_PATH, "config.json")])
         config = Config()
         # git commands
         cmds = [
             ["git", "init"],
             ["git", "config", "user.name", "baka admin"],
-            ["git", "config", "user.email", "baka@" + os.uname().nodename],
+            ["git", "config", "user.email", "baka@" + config.hostname],
             ["touch", "error.log"],
             ["bash", "-c", "echo '"
                 "history.log\n"
+                "hostname\n"
                 "docker/**\n"
                 "ignore/**\n"
+                "!**/config.php\n"
+                "!**/*.ini\n"
+                "!**/*.json\n"
+                "!**/*.toml\n"
+                "!**/*.xml\n"
+                "!**/*.yaml\n"
+                "!**/*.yml\n"
                 "*~\n"
                 "*-old\n"
                 "*.cache\n"
                 "*.dpkg-bak\n"
                 "*.dpkg-dist\n"
                 "*.dpkg-new\n"
                 "*.dpkg-old\n"
                 "**/fish_history\n"
                 "**/xonsh-*.json\n"
             "' > .gitignore"],
             ["bash", "-c", "read -p 'Press enter to open .gitignore with nano'"],
             ["nano", os.path.join(BASE_PATH, ".gitignore")],
             ["bash", "-c", "read -p 'Press enter to add files to repository'"],
-            *rsync_and_git_add_all(config),
+            *copy_and_git_add_all(),
             ["mkdir", "-p", "docker"],
             ["mkdir", "-p", "ignore"],
             ["mkdir", "-p", "scripts"],
             ["mkdir", "-p", "syscks"],
             ["mkdir", "-p", "scans"],
             ["git", "commit", "-m", "baka initial commit"]
         ]
     elif args.commit:
         cmds = [
-            *rsync_and_git_add_all(config),
+            *copy_and_git_add_all(),
             ["git", "commit", "-m", "baka commit " + args.commit]
         ]
     elif args.push:
         cmds = [
             ["git", "push"]
         ]
+    elif args.pull:
+        cmds = [
+            ["git", "pull"]
+        ]
     elif args.untrack:
         paths = []
         for path in sorted(args.untrack):
             if os.path.isabs(path):
                 paths.append(os.path.normpath(os.path.relpath(path)))
             else:
                 paths.append(os.path.normpath(os.path.relpath(os.path.join(original_cwd, path))))
@@ -323,84 +388,114 @@
             ["git", "rm", "-r", "--cached", *paths],
             ["bash", "-c", "echo \"\n# baka untrack\n%s\" >> .gitignore" % "\n".join(paths)],
             ["git", "add", ".gitignore"],
             ["git", "commit", "-m", "baka untrack %s" % " ".join(paths)]
         ]
     elif args.install:
         cmds = [
-            *rsync_and_git_add_all(config),
+            *copy_and_git_add_all(),
             ["git", "commit", "-m", "baka pre-install"],
             config.cmd_install + args.install,
-            *rsync_and_git_add_all(config),
+            *copy_and_git_add_all(),
             ["git", "commit", "-m", "baka install " + " ".join(args.install)]
         ]
     elif args.remove is not None:
         cmds = [
-            *rsync_and_git_add_all(config),
+            *copy_and_git_add_all(),
             ["git", "commit", "-m", "baka pre-remove"],
             config.cmd_remove + args.remove,
-            *rsync_and_git_add_all(config),
+            *copy_and_git_add_all(),
             ["git", "commit", "-m", "baka remove " + " ".join(args.remove)]
         ]
     elif args.upgrade:
         cmds = [
-            *rsync_and_git_add_all(config),
+            *copy_and_git_add_all(),
             ["git", "commit", "-m", "baka pre-upgrade"],
             config.cmd_upgrade,
-            *rsync_and_git_add_all(config),
+            *copy_and_git_add_all(),
             ["git", "commit", "-m", "baka upgrade"]
         ]
-    elif args.docker:
+    elif args.docker or args.podman:
+        compose: str = "sudo docker-compose" if args.docker else "podman-compose"
+        args.docker = args.docker if args.docker else args.podman
         assert args.docker[0] in ["up", "down", "pull"] and len(args.docker) >= 2
         assert args.docker[1] != "all" or (args.docker[1] == "all" and len(args.docker) == 2)
-        cmd = "up -d" if args.docker[0] == "up" else args.docker[0]
+        compose_arg = "up -d" if args.docker[0] == "up" else args.docker[0]
         cmds = []
         if args.docker[1] == "all":
             for folder in sorted(os.listdir("docker")):
                 if not os.path.exists(os.path.join("docker", folder, ".dockerignore")):
-                    assert os.path.exists(os.path.join("docker", folder, "docker-compose.yml"))
-                    cmds.append(["bash", "-c", "cd docker/%s && sudo docker-compose %s" % (folder, cmd)])
+                    cmds.append(["bash", "-c", f"cd docker/{folder} && {compose} {compose_arg}"])
         else:
             for folder in args.docker[1:]:
-                assert os.path.exists(os.path.join("docker", folder, "docker-compose.yml"))
-                cmds.append(["bash", "-c", "cd docker/%s && sudo docker-compose %s" % (folder, cmd)])
+                cmds.append(["bash", "-c", f"cd docker/{folder} && {compose} {compose_arg}"])
+    elif args.file:
+        assert args.file[0] in ["save", "restore", "s", "r"] and len(args.file) >= 2
+        assert args.file[1] != "all" or (args.file[1] == "all" and len(args.file) == 2)
+        file_list = config.files.keys() if args.file[1] == "all" else args.file[1:]
+        cmds = [
+            ["git", "add", "--ignore-errors", "--all"],
+            ["git", "commit", "-m", f"baka pre-file {config.hostname}"]
+        ]
+        current_os = "windows" if os.name == "nt" else "linux"
+        not_current_os_abbrev = "l" if current_os == "windows" else "w"
+        copy_command = ["cp", "-f"] if current_os == "linux" else ["copy", "/Y"]
+        os.path.makedirs(os.path.join(BASE_PATH, config.hostname), exist_ok=True)
+        for file in file_list:
+            assert len(config.files[file]) == 1
+            file_key = list(config.files[file].keys())[0]
+            if not_current_os_abbrev in file_key.split("_"):
+                continue
+            if args.file[0] in ["save", "s"]:
+                if "src" in file_key.split("_"):
+                    cmds.append([*copy_command, config.files[file][file_key], os.path.join(BASE_PATH, config.hostname, file)])
+                elif "cmd" in config.files[file]:
+                    cmds.append(["BAKA_DEST", os.path.join(BASE_PATH, config.hostname, file), *config.files[file]["cmd"]])
+            elif args.file[0] in ["restore", "r"]:
+                if "src" in file_key.split("_"):
+                    cmds.append([*copy_command, os.path.join(BASE_PATH, config.hostname, file), config.files[file][file_key]])
+        cmds.append(["git", "add", "--ignore-errors", "--all"])
+        cmds.append(["git", "commit", "-m", f"baka file {config.hostname}"])
     elif args.job:
         if args.interactive:
             config.jobs[args.job]["interactive"] = True
+        if args.exit_zero_toggle:
+            exit_non_zero = "exit_non_zero" in config.jobs[args.job] and config.jobs[args.job]["exit_non_zero"]
+            config.jobs[args.job]["exit_non_zero"] = not exit_non_zero
         cmds = config.jobs[args.job]["commands"]
     elif args.list:
         cmds = [
             ["echo", "Prompt\tExit!0\tJob Name\n========================"],
             *[["echo", "%s\t%s\t%s" % ("interactive" in config.jobs[job] and config.jobs[job]["interactive"],
                                        "exit_non_zero" in config.jobs[job] and config.jobs[job]["exit_non_zero"],
                                        job)] for job in config.jobs]
         ]
     elif args.system_checks:
         assert ("history" not in config.system_checks)
         assert all([key not in config.system_scans for key in config.system_checks])
         cmds = [
-            *rsync_and_git_add_all(config),
+            *copy_and_git_add_all(),
             ["git", "commit", "-m", "baka pre-sysck"],
             *[["bash", "-c", "%s > syscks/%s.log" % (config.system_checks[key], key)] for key in config.system_checks],
             ["git", "add", "--ignore-errors", "--all"],
             ["git", "commit", "-m", "baka sysck"]
         ]
     elif args.system_scans:
         assert ("history" not in config.system_scans)
         assert all([key not in config.system_checks for key in config.system_scans])
         cmds = [
-            *rsync_and_git_add_all(config),
+            *copy_and_git_add_all(),
             ["git", "commit", "-m", "baka pre-scan"],
             *[["bash", "-c", "%s | tee scans/%s.log" % (config.system_scans[key], key)] for key in config.system_scans],
             ["git", "add", "--ignore-errors", "--all"],
             ["git", "commit", "-m", "baka scan"]
         ]
     elif args.diff:
         cmds = [
-            *rsync_and_git_add_all(config),
+            *copy_and_git_add_all(),
             ["git", "status", "-sb"],
             ["git", "diff", "--color-words", "--cached", "--minimal"]
         ]
     elif args.log:
         cmds = [[
             "git", "log", "--abbrev-commit", "--all", "--decorate", "--graph", "--stat",
             "--format=format:%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset)%C(bold yellow)%d%C(reset)%n%C(bold white)%s%C(reset)%C(dim white) - %an%C(reset)"
@@ -446,22 +541,23 @@
                         elif response.strip().lower().startswith("n"):
                             break
                         elif response.strip().lower().startswith("s"):
                             continue
                         else:
                             print("\033[91mInvalid response, exiting\033[0m")
                             break
+                    proc_input = "y\n" if args.yes else None
                     proc_out = subprocess.PIPE
                     proc_err = subprocess.PIPE
                     if not capture_output:
                         if verbosity in ["debug", "info"]:
                             proc_out = sys.stdout
                         if verbosity in ["debug", "info", "error"]:
                             proc_err = sys.stderr
-                    proc = subprocess.run(cmd, stdout=proc_out, stderr=proc_err)
+                    proc = subprocess.run(cmd, stdout=proc_out, stderr=proc_err, input=proc_input)
                     if proc.returncode != 0:
                         if "exit_non_zero" in config.jobs[args.job] and config.jobs[args.job]["exit_non_zero"]:
                             return_code = proc.returncode
                             error_message = "Error: baka job encountered a non-zero return code for `%s`, exiting" % shlex.join(cmd)
                             command_output.append(error_message)
                             print(error_message, file=sys.stderr)
                             break
@@ -475,24 +571,28 @@
                             print("\n")
                         command_output.append(">>> " + shlex.join(cmd))
                         command_output.append(proc.stdout.decode().strip())
                         command_output.append(proc.stderr.decode().strip())
                         command_output.append("\n")
                     elif verbosity in ["debug", "info", "error"]:
                         print("")
-                elif cmd[0] == "rsync":
-                    # hide permission errors for rsync, otherwise run command normally
-                    proc = subprocess.run(cmd, stderr=subprocess.PIPE, universal_newlines=True)
-                    for line in proc.stderr.splitlines():
-                        if line and "Permission denied (13)" not in line and "(see previous errors) (code 23)" not in line:
-                            print(line, file=sys.stderr)
-                    pending_stat = True
+                elif args.file:
+                    # save outputs of non-copy commands as files, otherwise run command normally
+                    if cmd[0] == "BAKA_DEST":
+                        dest = cmd[1]
+                        with open(dest, "w", encoding="utf-8", errors="surrogateescape") as f:
+                            proc = subprocess.run(cmd[2:], capture_output=True, text=True)
+                            f.write(proc.stdout)
+                    else:
+                        proc = subprocess.run(cmd)
+                    if proc.returncode != 0 and not (cmd[0] == "git" and cmd[1] == "commit"):
+                        return_code += 1
                 else:
                     # run command normally
-                    if cmd == [sys.executable, os.path.abspath(__file__), "--_copy_conditional_paths"]:
+                    if cmd == [sys.executable, os.path.abspath(__file__), "--_hash_and_copy_files"]:
                         pending_stat = True
                     elif pending_stat:
                         os_stat_tracked_files(config)
                         pending_stat = False
                     proc = subprocess.run(cmd)
                     if proc.returncode != 0 and not (cmd[0] == "git" and cmd[1] == "commit"):
                         return_code += 1
```

### Comparing `bakabakabaka-0.7.7/setup.py` & `bakabakabaka-0.8.0/setup.py`

 * *Files identical despite different names*

