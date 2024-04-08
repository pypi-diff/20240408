# Comparing `tmp/Shimarin-0.1.2.tar.gz` & `tmp/Shimarin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimarin-0.1.2.tar", last modified: Tue Jul 25 12:48:11 2023, max compression
+gzip compressed data, was "Shimarin-0.1.3.tar", last modified: Mon Apr  8 18:22:55 2024, max compression
```

## Comparing `Shimarin-0.1.2.tar` & `Shimarin-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.690329 Shimarin-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-25 12:48:11.690329 Shimarin-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-25 12:47:58.000000 Shimarin-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.686329 Shimarin-0.1.2/Shimarin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.690329 Shimarin-0.1.2/Shimarin/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/client/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/client/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.686329 Shimarin-0.1.2/Shimarin/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.690329 Shimarin-0.1.2/Shimarin/plugins/flask_api/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/plugins/flask_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/plugins/flask_api/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.690329 Shimarin-0.1.2/Shimarin/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/server/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/server/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.690329 Shimarin-0.1.2/Shimarin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-25 12:48:11.000000 Shimarin-0.1.2/Shimarin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-25 12:48:11.000000 Shimarin-0.1.2/Shimarin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:48:11.000000 Shimarin-0.1.2/Shimarin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:48:11.000000 Shimarin-0.1.2/Shimarin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 12:48:11.000000 Shimarin-0.1.2/Shimarin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 12:48:11.000000 Shimarin-0.1.2/Shimarin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-25 12:47:58.000000 Shimarin-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-25 12:48:11.694329 Shimarin-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:22:55.646724 Shimarin-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-08 18:22:55.642724 Shimarin-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-08 18:22:47.000000 Shimarin-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:22:55.642724 Shimarin-0.1.3/Shimarin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:22:47.000000 Shimarin-0.1.3/Shimarin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:22:55.642724 Shimarin-0.1.3/Shimarin/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:22:47.000000 Shimarin-0.1.3/Shimarin/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-08 18:22:47.000000 Shimarin-0.1.3/Shimarin/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-08 18:22:47.000000 Shimarin-0.1.3/Shimarin/client/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-08 18:22:47.000000 Shimarin-0.1.3/Shimarin/client/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:22:55.638724 Shimarin-0.1.3/Shimarin/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:22:55.642724 Shimarin-0.1.3/Shimarin/plugins/flask_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 18:22:47.000000 Shimarin-0.1.3/Shimarin/plugins/flask_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-08 18:22:47.000000 Shimarin-0.1.3/Shimarin/plugins/flask_api/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:22:55.642724 Shimarin-0.1.3/Shimarin/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:22:47.000000 Shimarin-0.1.3/Shimarin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-08 18:22:47.000000 Shimarin-0.1.3/Shimarin/server/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 18:22:47.000000 Shimarin-0.1.3/Shimarin/server/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:22:55.642724 Shimarin-0.1.3/Shimarin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-08 18:22:55.000000 Shimarin-0.1.3/Shimarin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-08 18:22:55.000000 Shimarin-0.1.3/Shimarin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:22:55.000000 Shimarin-0.1.3/Shimarin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:22:55.000000 Shimarin-0.1.3/Shimarin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 18:22:55.000000 Shimarin-0.1.3/Shimarin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 18:22:55.000000 Shimarin-0.1.3/Shimarin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 18:22:47.000000 Shimarin-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-08 18:22:55.646724 Shimarin-0.1.3/setup.cfg
```

### Comparing `Shimarin-0.1.2/Shimarin/client/events.py` & `Shimarin-0.1.3/Shimarin/client/events.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.1.2/Shimarin/client/networking.py` & `Shimarin-0.1.3/Shimarin/client/networking.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.1.2/Shimarin/plugins/flask_api/server.py` & `Shimarin-0.1.3/Shimarin/plugins/flask_api/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 from Shimarin.server import events
 from flask import Flask, request
 
 
 emitter = events.EventEmitter()
 app = Flask("server")
 
+CONTEXT_PATH = os.getenv("CONTEXT_PATH", "")
+
 
 def login():
     if ((USERNAME := os.getenv("SHIMARIN_USERNAME") and (PASSWORD := os.getenv("SHIMARIN_PASSWORD")))):
         if (username := request.headers.get("username")) and (
             password := request.headers.get("password")
         ):
             if username != USERNAME or password != PASSWORD:
                 return {"ok": False, "message": "Invalid credentials!"}, 401
         else:
             return {"ok": False, "message": "Invalid credentials!"}, 401
     return {"ok": True, "message": "Authentication disabled"}, 200
 
 
-@app.route("/events", methods=["GET"])
+@app.route(CONTEXT_PATH + "/events", methods=["GET"])
 async def events_route():
     r = login()
     if (r[0]['ok'] is False):
         return r
     fetch = request.args.get("fetch")
     events_to_send = 1
     if fetch:
@@ -33,15 +35,15 @@
     for _ in range(events_to_send):
         last_ev = await emitter.fetch_event()
         if last_ev.event_type:
             events.append(last_ev.json())
     return events
 
 
-@app.route("/callback")
+@app.route(CONTEXT_PATH + "/callback")
 async def reply_route():
     r = login()
     if (r[0]['ok'] is False):
         return r
     data = request.get_json(silent=True)
     if data:
         identifier = data["identifier"]
```

### Comparing `Shimarin-0.1.2/Shimarin/server/events.py` & `Shimarin-0.1.3/Shimarin/server/events.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.1.2/Shimarin.egg-info/SOURCES.txt` & `Shimarin-0.1.3/Shimarin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shimarin-0.1.2/setup.cfg` & `Shimarin-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Shimarin
-version = 0.1.2
+version = 0.1.3
 description = asynchronous event-based communication between client and server
 author = Kamuri Amorim
 author_email = myk.gata14@gmail.com
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kamuridesu/Shimarin
 keywords = python events client server asynchronous
```

