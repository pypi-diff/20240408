# Comparing `tmp/pyunifiprotect-5.1.2.tar.gz` & `tmp/pyunifiprotect-5.1.3.tar.gz`

## Comparing `pyunifiprotect-5.1.2.tar` & `pyunifiprotect-5.1.3.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/__init__.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/__main__.py
--rw-r--r--   0        0        0    61141 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/api.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/py.typed
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/release_cache.json
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/stream.py
--rw-r--r--   0        0        0    17996 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/utils.py
--rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/websocket.py
--rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/cli/__init__.py
--rw-r--r--   0        0        0    36594 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/cli/backup.py
--rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/cli/base.py
--rw-r--r--   0        0        0    17035 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/cli/cameras.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/cli/chimes.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/cli/doorlocks.py
--rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/cli/events.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/cli/lights.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/cli/liveviews.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/cli/nvr.py
--rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/cli/sensors.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/cli/viewers.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/data/__init__.py
--rw-r--r--   0        0        0    37904 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/data/base.py
--rw-r--r--   0        0        0    21954 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/data/bootstrap.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/data/convert.py
--rw-r--r--   0        0        0   101900 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/data/devices.py
--rw-r--r--   0        0        0    38059 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/data/nvr.py
--rw-r--r--   0        0        0    15212 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/data/types.py
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/data/user.py
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/data/websocket.py
--rw-r--r--   0        0        0    18784 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/test_util/__init__.py
--rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyunifiprotect/test_util/anonymize.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/LICENSE
--rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/README.md
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/pyproject.toml
--rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.2/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/__init__.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/__main__.py
+-rw-r--r--   0        0        0    61141 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/api.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/py.typed
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/stream.py
+-rw-r--r--   0        0        0    17996 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/utils.py
+-rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/websocket.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/__init__.py
+-rw-r--r--   0        0        0    36594 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/backup.py
+-rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/base.py
+-rw-r--r--   0        0        0    17035 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/cameras.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/chimes.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/doorlocks.py
+-rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/events.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/lights.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/liveviews.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/nvr.py
+-rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/sensors.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/viewers.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/__init__.py
+-rw-r--r--   0        0        0    37904 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/base.py
+-rw-r--r--   0        0        0    21954 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/bootstrap.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/convert.py
+-rw-r--r--   0        0        0   101900 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/devices.py
+-rw-r--r--   0        0        0    38059 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/nvr.py
+-rw-r--r--   0        0        0    15212 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/types.py
+-rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/user.py
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/websocket.py
+-rw-r--r--   0        0        0    18784 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/test_util/__init__.py
+-rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/test_util/anonymize.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/LICENSE
+-rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/README.md
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyproject.toml
+-rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/PKG-INFO
```

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/api.py` & `pyunifiprotect-5.1.3/pyunifiprotect/api.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/exceptions.py` & `pyunifiprotect-5.1.3/pyunifiprotect/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/stream.py` & `pyunifiprotect-5.1.3/pyunifiprotect/stream.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/utils.py` & `pyunifiprotect-5.1.3/pyunifiprotect/utils.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/websocket.py` & `pyunifiprotect-5.1.3/pyunifiprotect/websocket.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/cli/__init__.py` & `pyunifiprotect-5.1.3/pyunifiprotect/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/cli/backup.py` & `pyunifiprotect-5.1.3/pyunifiprotect/cli/backup.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/cli/base.py` & `pyunifiprotect-5.1.3/pyunifiprotect/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/cli/cameras.py` & `pyunifiprotect-5.1.3/pyunifiprotect/cli/cameras.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/cli/chimes.py` & `pyunifiprotect-5.1.3/pyunifiprotect/cli/chimes.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/cli/doorlocks.py` & `pyunifiprotect-5.1.3/pyunifiprotect/cli/doorlocks.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/cli/events.py` & `pyunifiprotect-5.1.3/pyunifiprotect/cli/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 app = typer.Typer(rich_markup_mode="rich")
 
 ARG_EVENT_ID = typer.Argument(None, help="ID of camera to select for subcommands")
 OPTION_START = typer.Option(None, "-s", "--start")
 OPTION_END = typer.Option(None, "-e", "--end")
 OPTION_LIMIT = typer.Option(None, "-l", "--limit")
+OPTION_OFFSET = typer.Option(None, "-o", "--offet")
 OPTION_TYPES = typer.Option(None, "-t", "--type")
 OPTION_SMART_TYPES = typer.Option(
     None,
     "-d",
     "--smart-detect",
     help="If provided, will only return smartDetectZone events",
 )
@@ -42,14 +43,15 @@
 @app.callback(invoke_without_command=True)
 def main(
     ctx: typer.Context,
     event_id: Optional[str] = ARG_EVENT_ID,
     start: Optional[datetime] = OPTION_START,
     end: Optional[datetime] = OPTION_END,
     limit: Optional[int] = OPTION_LIMIT,
+    offset: Optional[int] = OPTION_OFFSET,
     types: Optional[list[d.EventType]] = OPTION_TYPES,
     smart_types: Optional[list[d.SmartDetectObjectType]] = OPTION_SMART_TYPES,
 ) -> None:
     """Events CLI.
 
     Returns list of events from the last 24 hours without any arguments passed.
     """
@@ -81,14 +83,15 @@
             smart_types = None
         events = base.run(
             ctx,
             protect.get_events(
                 start=start,
                 end=end,
                 limit=limit,
+                offset=offset,
                 types=types,
                 smart_detect_types=smart_types,
             ),
         )
         ctx.obj.events = {}
         for event in events:
             ctx.obj.events[event.id] = event
```

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/cli/lights.py` & `pyunifiprotect-5.1.3/pyunifiprotect/cli/lights.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/cli/liveviews.py` & `pyunifiprotect-5.1.3/pyunifiprotect/cli/liveviews.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/cli/nvr.py` & `pyunifiprotect-5.1.3/pyunifiprotect/cli/nvr.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/cli/sensors.py` & `pyunifiprotect-5.1.3/pyunifiprotect/cli/sensors.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/cli/viewers.py` & `pyunifiprotect-5.1.3/pyunifiprotect/cli/viewers.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/data/__init__.py` & `pyunifiprotect-5.1.3/pyunifiprotect/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/data/base.py` & `pyunifiprotect-5.1.3/pyunifiprotect/data/base.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/data/bootstrap.py` & `pyunifiprotect-5.1.3/pyunifiprotect/data/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/data/convert.py` & `pyunifiprotect-5.1.3/pyunifiprotect/data/convert.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/data/devices.py` & `pyunifiprotect-5.1.3/pyunifiprotect/data/devices.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/data/nvr.py` & `pyunifiprotect-5.1.3/pyunifiprotect/data/nvr.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/data/types.py` & `pyunifiprotect-5.1.3/pyunifiprotect/data/types.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/data/user.py` & `pyunifiprotect-5.1.3/pyunifiprotect/data/user.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/data/websocket.py` & `pyunifiprotect-5.1.3/pyunifiprotect/data/websocket.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/test_util/__init__.py` & `pyunifiprotect-5.1.3/pyunifiprotect/test_util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyunifiprotect/test_util/anonymize.py` & `pyunifiprotect-5.1.3/pyunifiprotect/test_util/anonymize.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/.gitignore` & `pyunifiprotect-5.1.3/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # settings.json is user-specific overrides for devcontainer.json
 .vscode/settings.json
 test-data
 ufp-data
 *.mp3
 *.mp4
 *.js
+*.json
+*.csv
 backup
 .benchmarks
 .ruff_cache
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
```

### Comparing `pyunifiprotect-5.1.2/LICENSE` & `pyunifiprotect-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/README.md` & `pyunifiprotect-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/pyproject.toml` & `pyunifiprotect-5.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.2/PKG-INFO` & `pyunifiprotect-5.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyunifiprotect
-Version: 5.1.2
+Version: 5.1.3
 Summary: Unofficial UniFi Protect Python API and CLI
 Project-URL: Source Code, https://github.com/AngellusMortis/pyunifiprotect/
 Project-URL: Documentation, https://angellusmortis.github.io/pyunifiprotect/latest/
 Project-URL: Bug Reports, https://github.com/AngellusMortis/pyunifiprotect/issues/
 Project-URL: Changelog, https://github.com/AngellusMortis/pyunifiprotect/releases/
 Author-email: Bjarne Riis <bjarne@briis.com>, Christopher Bailey <cbailey@mort.is>
 Maintainer-email: Christopher Bailey <cbailey@mort.is>, "J. Nick Koston" <nick@koston.org>
```

