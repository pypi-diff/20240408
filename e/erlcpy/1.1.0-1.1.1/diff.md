# Comparing `tmp/erlcpy-1.1.0.tar.gz` & `tmp/erlcpy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlcpy-1.1.0.tar", last modified: Sun Feb 25 17:37:37 2024, max compression
+gzip compressed data, was "erlcpy-1.1.1.tar", last modified: Mon Apr  8 19:45:43 2024, max compression
```

## Comparing `erlcpy-1.1.0.tar` & `erlcpy-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-25 17:37:37.651494 erlcpy-1.1.0/
--rw-rw-rw-   0        0        0     1085 2024-02-25 08:54:13.000000 erlcpy-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      363 2024-02-25 17:37:37.650494 erlcpy-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      666 2024-02-25 08:21:47.000000 erlcpy-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-25 17:37:37.640809 erlcpy-1.1.0/erlcpy/
--rw-rw-rw-   0        0        0      349 2024-02-25 09:13:02.000000 erlcpy-1.1.0/erlcpy/__init__.py
--rw-rw-rw-   0        0        0     1995 2024-02-25 17:32:34.000000 erlcpy-1.1.0/erlcpy/main.py
-drwxrwxrwx   0        0        0        0 2024-02-25 17:37:37.650494 erlcpy-1.1.0/erlcpy.egg-info/
--rw-rw-rw-   0        0        0      363 2024-02-25 17:37:37.000000 erlcpy-1.1.0/erlcpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-02-25 17:37:37.000000 erlcpy-1.1.0/erlcpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-25 17:37:37.000000 erlcpy-1.1.0/erlcpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-02-25 17:37:37.000000 erlcpy-1.1.0/erlcpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-25 17:37:37.000000 erlcpy-1.1.0/erlcpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-25 17:37:37.651494 erlcpy-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      469 2024-02-25 17:37:32.000000 erlcpy-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:45:43.921011 erlcpy-1.1.1/
+-rw-rw-rw-   0        0        0     1085 2024-02-25 08:54:13.000000 erlcpy-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      363 2024-04-08 19:45:43.919759 erlcpy-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2024-02-25 08:21:47.000000 erlcpy-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 19:45:43.902659 erlcpy-1.1.1/erlcpy/
+-rw-rw-rw-   0        0        0      381 2024-04-08 19:44:43.000000 erlcpy-1.1.1/erlcpy/__init__.py
+-rw-rw-rw-   0        0        0     2114 2024-04-08 19:44:29.000000 erlcpy-1.1.1/erlcpy/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:45:43.919759 erlcpy-1.1.1/erlcpy.egg-info/
+-rw-rw-rw-   0        0        0      363 2024-04-08 19:45:43.000000 erlcpy-1.1.1/erlcpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-08 19:45:43.000000 erlcpy-1.1.1/erlcpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 19:45:43.000000 erlcpy-1.1.1/erlcpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 19:45:43.000000 erlcpy-1.1.1/erlcpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-08 19:45:43.000000 erlcpy-1.1.1/erlcpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 19:45:43.921011 erlcpy-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      469 2024-04-08 19:45:11.000000 erlcpy-1.1.1/setup.py
```

### Comparing `erlcpy-1.1.0/LICENSE` & `erlcpy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `erlcpy-1.1.0/README.md` & `erlcpy-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `erlcpy-1.1.0/erlcpy/main.py` & `erlcpy-1.1.1/erlcpy/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,20 +41,24 @@
 
 def get_mod_calls(self):
     return self._make_get_request('server/modcalls')
 
 def get_bans(self):
     return self._make_get_request('server/bans')
 
+def get_vehicles(self):
+    return self._make_get_request('/server/vehicles')
+
 def send_command(self, command):
     return self._make_post_request('server/command', {'command': command})
 
 # Bind the methods to the class
 ServerAPI.get_server_info = get_server_info
 ServerAPI.get_players = get_players
 ServerAPI.get_join_logs = get_join_logs
 ServerAPI.get_queue = get_queue
 ServerAPI.get_kill_logs = get_kill_logs
 ServerAPI.get_command_logs = get_command_logs
 ServerAPI.get_mod_calls = get_mod_calls
 ServerAPI.get_bans = get_bans
 ServerAPI.send_command = send_command
+ServerAPI.get_vehicles = get_vehicles
```

