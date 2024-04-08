# Comparing `tmp/pyprland-2.2.2.tar.gz` & `tmp/pyprland-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.2.2.tar", max compression
+gzip compressed data, was "pyprland-2.2.3.tar", max compression
```

## Comparing `pyprland-2.2.2.tar` & `pyprland-2.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.2/LICENSE
--rw-r--r--   0        0        0     4150 2024-04-06 14:33:59.923958 pyprland-2.2.2/README.md
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.2/pyprland/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.2/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.2/pyprland/adapters/colors.py
--rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.2/pyprland/adapters/menus.py
--rwxr-xr-x   0        0        0    15682 2024-04-06 14:37:27.351505 pyprland-2.2.2/pyprland/command.py
--rwxr-xr-x   0        0        0    15808 2024-04-05 22:08:40.562254 pyprland-2.2.2/pyprland/command.py.orig
--rw-r--r--   0        0        0     4190 2024-04-06 13:35:14.309864 pyprland-2.2.2/pyprland/common.py
--rw-r--r--   0        0        0     5948 2024-03-31 20:05:57.091220 pyprland-2.2.2/pyprland/ipc.py
--rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.2/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.2/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.2.2/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.2/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0     2589 2024-04-06 13:35:14.309864 pyprland-2.2.2/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.2/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.2/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.2/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.2.2/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.2.2/pyprland/plugins/monitors.py.orig
--rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.2/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0        0 2024-04-04 16:21:22.101700 pyprland-2.2.2/pyprland/plugins/nohup.out
--rw-r--r--   0        0        0     1309 2024-04-06 13:35:25.146759 pyprland-2.2.2/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0    35361 2024-04-06 13:37:10.612283 pyprland-2.2.2/pyprland/plugins/scratchpads.py
--rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.2/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     4149 2024-04-06 13:38:00.979983 pyprland-2.2.2/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     3983 2024-04-05 20:13:47.397221 pyprland-2.2.2/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.2/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.2/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     3764 2024-04-05 20:13:47.397221 pyprland-2.2.2/pyprland/plugins/wallpapers.py
--rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.2.2/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0      725 2024-04-06 14:37:27.341505 pyprland-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 pyprland-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.3/LICENSE
+-rw-r--r--   0        0        0     4128 2024-04-07 10:28:36.716804 pyprland-2.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.3/pyprland/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.3/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.3/pyprland/adapters/colors.py
+-rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.3/pyprland/adapters/menus.py
+-rwxr-xr-x   0        0        0    15682 2024-04-08 16:06:45.965533 pyprland-2.2.3/pyprland/command.py
+-rwxr-xr-x   0        0        0    15808 2024-04-05 22:08:40.562254 pyprland-2.2.3/pyprland/command.py.orig
+-rw-r--r--   0        0        0     4190 2024-04-06 13:35:14.309864 pyprland-2.2.3/pyprland/common.py
+-rw-r--r--   0        0        0     5948 2024-03-31 20:05:57.091220 pyprland-2.2.3/pyprland/ipc.py
+-rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.3/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.3/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.2.3/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.3/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0     2589 2024-04-06 13:35:14.309864 pyprland-2.2.3/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.3/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.3/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.3/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.2.3/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.2.3/pyprland/plugins/monitors.py.orig
+-rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.3/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0        0 2024-04-04 16:21:22.101700 pyprland-2.2.3/pyprland/plugins/nohup.out
+-rw-r--r--   0        0        0     1309 2024-04-06 13:35:25.146759 pyprland-2.2.3/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0    35361 2024-04-06 13:37:10.612283 pyprland-2.2.3/pyprland/plugins/scratchpads.py
+-rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.3/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     4149 2024-04-06 13:38:00.979983 pyprland-2.2.3/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     3983 2024-04-05 20:13:47.397221 pyprland-2.2.3/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.3/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.3/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     3776 2024-04-08 16:06:05.055461 pyprland-2.2.3/pyprland/plugins/wallpapers.py
+-rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.2.3/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0      725 2024-04-08 16:06:45.952200 pyprland-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4667 1970-01-01 00:00:00.000000 pyprland-2.2.3/PKG-INFO
```

### Comparing `pyprland-2.2.2/LICENSE` & `pyprland-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/README.md` & `pyprland-2.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 - [You NEED This in your Hyprland Config - LibrePhoenix (video)](https://www.youtube.com/watch?v=CwGlm-rpok4) - October 2023 (*Now [TOML](https://toml.io/en/) format is preferred over [JSON](https://www.w3schools.com/js/js_json_intro.asp))
 
 
 ## Dependencies
 
 - **Hyprland** >= 0.37
 - **Python** >= 3.11
-- **aiofiles** python package (since Pyprland >= 2.0)
+- **aiofiles** (Python package)
 
 ## Latest major changes
 
 > [!note]
 > Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
 ### 2.2
```

#### html2text {}

```diff
@@ -18,32 +18,32 @@
 allrepos/pyprland.svg)](https://repology.org/project/pyprland/versions) ð
 Hear what others are saying: - ["It just works very very well" - The Linux Cast
 (video)](https://youtu.be/Cjn0SFyyucY?si=hGb0TM9IDvlbcD6A&t=131) - February
 2024 - [You NEED This in your Hyprland Config - LibrePhoenix (video)](https://
 www.youtube.com/watch?v=CwGlm-rpok4) - October 2023 (*Now [TOML](https://
 toml.io/en/) format is preferred over [JSON](https://www.w3schools.com/js/
 js_json_intro.asp)) ## Dependencies - **Hyprland** >= 0.37 - **Python** >= 3.11
-- **aiofiles** python package (since Pyprland >= 2.0) ## Latest major changes >
-[!note] > Check the [Releases change log](https://github.com/hyprland-
-community/pyprland/releases) for more information ### 2.2 - Added [wallpapers]
-(https://github.com/hyprland-community/pyprland/wiki/wallpapers) and
-[system_notifier](https://github.com/hyprland-community/pyprland/wiki/
-system_notifier) plugins. ### 2.1 - Requires Hyprland >= 0.37 - [Monitors]
-(https://github.com/hyprland-community/pyprland/wiki/monitors) plugin
-improvements. ### 2.0 - New dependency: [aiofiles](https://pypi.org/project/
-aiofiles/) - Added [hysteresis](https://github.com/hyprland-community/pyprland/
-wiki/scratchpads#hysteresis-optional) support for [scratchpads](https://
-github.com/hyprland-community/pyprland/wiki/scratchpads). ### 1.10 - New
-[fetch_client_menu](https://github.com/hyprland-community/pyprland/wiki/
-fetch_client_menu) and [shortcuts_menu](https://github.com/hyprland-community/
-pyprland/wiki/shortcuts_menu) plugins. ### 1.9 - Introduced [shortcuts_menu]
-(https://github.com/hyprland-community/pyprland/wiki/shortcuts_menu) plugin.
-### 1.8 - Requires Hyprland >= 0.30 - Added [layout_center](https://github.com/
-hyprland-community/pyprland/wiki/layout_center) plugin. ## Developers
-Contribute to Pyprland in various ways: - Report bugs or propose features
-[here](https://github.com/hyprland-community/pyprland/issues). - Improve our
-[wiki](https://github.com/hyprland-community/pyprland/wiki) or write new
-plugins. - Enhance test coverage in our [tests](https://github.com/hyprland-
-community/pyprland/tree/main/tests). Check out the [creating a pull request]
-(https://docs.github.com/fr/pull-requests/collaborating-with-pull-requests/
-proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
-document for guidance. ## Star History_[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
+- **aiofiles** (Python package) ## Latest major changes > [!note] > Check the
+[Releases change log](https://github.com/hyprland-community/pyprland/releases)
+for more information ### 2.2 - Added [wallpapers](https://github.com/hyprland-
+community/pyprland/wiki/wallpapers) and [system_notifier](https://github.com/
+hyprland-community/pyprland/wiki/system_notifier) plugins. ### 2.1 - Requires
+Hyprland >= 0.37 - [Monitors](https://github.com/hyprland-community/pyprland/
+wiki/monitors) plugin improvements. ### 2.0 - New dependency: [aiofiles](https:
+//pypi.org/project/aiofiles/) - Added [hysteresis](https://github.com/hyprland-
+community/pyprland/wiki/scratchpads#hysteresis-optional) support for
+[scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads).
+### 1.10 - New [fetch_client_menu](https://github.com/hyprland-community/
+pyprland/wiki/fetch_client_menu) and [shortcuts_menu](https://github.com/
+hyprland-community/pyprland/wiki/shortcuts_menu) plugins. ### 1.9 - Introduced
+[shortcuts_menu](https://github.com/hyprland-community/pyprland/wiki/
+shortcuts_menu) plugin. ### 1.8 - Requires Hyprland >= 0.30 - Added
+[layout_center](https://github.com/hyprland-community/pyprland/wiki/
+layout_center) plugin. ## Developers Contribute to Pyprland in various ways: -
+Report bugs or propose features [here](https://github.com/hyprland-community/
+pyprland/issues). - Improve our [wiki](https://github.com/hyprland-community/
+pyprland/wiki) or write new plugins. - Enhance test coverage in our [tests]
+(https://github.com/hyprland-community/pyprland/tree/main/tests). Check out the
+[creating a pull request](https://docs.github.com/fr/pull-requests/
+collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-
+requests/creating-a-pull-request) document for guidance. ## Star History_[_S_t_a_r
+_H_i_s_t_o_r_y_ _C_h_a_r_t_]
```

### Comparing `pyprland-2.2.2/pyprland/adapters/menus.py` & `pyprland-2.2.3/pyprland/adapters/menus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/command.py` & `pyprland-2.2.3/pyprland/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,15 @@
 
 
 async def run_client():
     "Runs the client (CLI)"
     manager = Pyprland()
 
     if sys.argv[1] == "version":
-        print("2.2.2")  # Automatically updated version
+        print("2.2.3")  # Automatically updated version
         return
 
     if sys.argv[1] in ("--help", "-h", "help"):
         await manager.load_config(init=False)
 
         def format_doc(txt):
             return txt.split("\n")[0]
```

### Comparing `pyprland-2.2.2/pyprland/command.py.orig` & `pyprland-2.2.3/pyprland/command.py.orig`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/common.py` & `pyprland-2.2.3/pyprland/common.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/ipc.py` & `pyprland-2.2.3/pyprland/ipc.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/expose.py` & `pyprland-2.2.3/pyprland/plugins/expose.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/fetch_client_menu.py` & `pyprland-2.2.3/pyprland/plugins/fetch_client_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/interface.py` & `pyprland-2.2.3/pyprland/plugins/interface.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/layout_center.py` & `pyprland-2.2.3/pyprland/plugins/layout_center.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/lost_windows.py` & `pyprland-2.2.3/pyprland/plugins/lost_windows.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/magnify.py` & `pyprland-2.2.3/pyprland/plugins/magnify.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/monitors.py` & `pyprland-2.2.3/pyprland/plugins/monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/monitors.py.orig` & `pyprland-2.2.3/pyprland/plugins/monitors.py.orig`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/monitors_v0.py` & `pyprland-2.2.3/pyprland/plugins/monitors_v0.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/pyprland.py` & `pyprland-2.2.3/pyprland/plugins/pyprland.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/scratchpads.py` & `pyprland-2.2.3/pyprland/plugins/scratchpads.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/shift_monitors.py` & `pyprland-2.2.3/pyprland/plugins/shift_monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.2.3/pyprland/plugins/shortcuts_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/system_notifier.py` & `pyprland-2.2.3/pyprland/plugins/system_notifier.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/toggle_dpms.py` & `pyprland-2.2.3/pyprland/plugins/toggle_dpms.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/toggle_special.py` & `pyprland-2.2.3/pyprland/plugins/toggle_special.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyprland/plugins/wallpapers.py` & `pyprland-2.2.3/pyprland/plugins/wallpapers.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "Returns files matching `extension` in given `path`. Can optionally `recurse` subfolders."
     for fname in await listdir(path):
         ext = fname.rsplit(".", 1)[-1]
         full_path = os.path.join(path, fname)
         if ext.lower() in extensions:
             yield full_path
         elif recurse and os.path.isdir(full_path):
-            async for v in iter_dir(full_path, True):
+            async for v in iter_dir(full_path, extensions, True):
                 yield v
 
 
 class Extension(CastBoolMixin, Plugin):
     "Manages the background image"
 
     default_extensions: set[str] | list[str] = set(("png", "jpg", "jpeg"))
```

### Comparing `pyprland-2.2.2/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.2.3/pyprland/plugins/workspaces_follow_focus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.2/pyproject.toml` & `pyprland-2.2.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprland"
-version = "2.2.2"
+version = "2.2.3"
 description = "Hyperland plugin system - batteries included"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyprland"}]
 homepage = "https://github.com/hyprland-community/pyprland/"
```

### Comparing `pyprland-2.2.2/PKG-INFO` & `pyprland-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.2.2
+Version: 2.2.3
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -39,15 +39,15 @@
 - [You NEED This in your Hyprland Config - LibrePhoenix (video)](https://www.youtube.com/watch?v=CwGlm-rpok4) - October 2023 (*Now [TOML](https://toml.io/en/) format is preferred over [JSON](https://www.w3schools.com/js/js_json_intro.asp))
 
 
 ## Dependencies
 
 - **Hyprland** >= 0.37
 - **Python** >= 3.11
-- **aiofiles** python package (since Pyprland >= 2.0)
+- **aiofiles** (Python package)
 
 ## Latest major changes
 
 > [!note]
 > Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
 ### 2.2
```

