# Comparing `tmp/flet_easy-0.2.0.dev6.tar.gz` & `tmp/flet_easy-0.2.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_easy-0.2.0.dev6.tar", last modified: Wed Mar 27 01:47:59 2024, max compression
+gzip compressed data, was "flet_easy-0.2.0.dev7.tar", last modified: Sun Apr  7 23:54:34 2024, max compression
```

## Comparing `flet_easy-0.2.0.dev6.tar` & `flet_easy-0.2.0.dev7.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0    11541 2024-03-15 03:06:45.484085 flet_easy-0.2.0.dev6/LICENSE
--rw-r--r--   0        0        0    11541 2024-03-15 03:06:45.484085 flet_easy-0.2.0.dev6/LICENSE
--rw-r--r--   0        0        0     4215 2024-03-26 17:42:58.647813 flet_easy-0.2.0.dev6/README.md
--rw-r--r--   0        0        0     4215 2024-03-26 17:42:58.647813 flet_easy-0.2.0.dev6/README.md
--rw-r--r--   0        0        0     1900 2024-03-27 01:47:59.357328 flet_easy-0.2.0.dev6/pyproject.toml
--rw-r--r--   0        0        0      375 2024-03-27 01:13:26.759383 flet_easy-0.2.0.dev6/src/flet_easy/__init__.py
--rw-r--r--   0        0        0     2290 2024-03-27 01:29:44.941365 flet_easy-0.2.0.dev6/src/flet_easy/cli/copy.py
--rw-r--r--   0        0        0     2012 2024-03-27 01:39:46.941900 flet_easy-0.2.0.dev6/src/flet_easy/cli/main.py
--rw-r--r--   0        0        0     3266 2024-03-26 17:24:35.309852 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/.gitignore
--rw-r--r--   0        0        0      213 2024-03-26 17:24:35.331489 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/README.md
--rw-r--r--   0        0        0     1020 2024-03-03 22:34:42.168739 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/favicon.png
--rw-r--r--   0        0        0    30189 2024-03-03 22:32:58.387760 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/icon.png
--rw-r--r--   0        0        0     7610 2024-03-03 22:35:51.000000 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/icons/icon-192.png
--rw-r--r--   0        0        0    33055 2024-03-03 22:35:51.000000 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/icons/icon-512.png
--rw-r--r--   0        0        0     7610 2024-03-03 22:35:52.000000 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    33055 2024-03-03 22:35:52.000000 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    56474 2024-03-03 22:35:52.000000 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/icons/loading-animation.png
--rw-r--r--   0        0        0     3626 2024-03-03 03:21:32.823185 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/index.html
--rw-r--r--   0        0        0      932 2024-03-03 03:30:40.043903 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/manifest.json
--rw-r--r--   0        0        0       82 2024-03-26 17:23:30.793735 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/components/__init__.py
--rw-r--r--   0        0        0     2406 2024-03-26 17:38:30.030351 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/components/counter.py
--rw-r--r--   0        0        0      543 2024-03-26 17:38:02.877657 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/components/swoDrawer.py
--rw-r--r--   0        0        0       43 2024-03-02 22:24:42.021795 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/controllers/__init__.py
--rw-r--r--   0        0        0     1354 2024-03-26 17:52:29.027054 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/controllers/counter.py
--rw-r--r--   0        0        0        0 2024-02-06 23:06:50.337495 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/core/__init__.py
--rw-r--r--   0        0        0     1662 2024-03-26 17:36:40.926068 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/core/config.py
--rw-r--r--   0        0        0      304 2024-03-26 17:29:58.303333 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/main.py
--rw-r--r--   0        0        0        0 2024-03-02 22:31:18.957666 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/models/__init__.py
--rw-r--r--   0        0        0       64 2024-03-02 22:29:53.511216 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/views/__init__.py
--rw-r--r--   0        0        0      623 2024-03-26 17:34:52.181051 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/views/counter.py
--rw-r--r--   0        0        0      615 2024-03-26 17:34:38.077325 flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/views/index.py
--rw-r--r--   0        0        0    10680 2024-03-27 01:21:45.778185 flet_easy-0.2.0.dev6/src/flet_easy/datasy.py
--rw-r--r--   0        0        0      124 2024-03-25 22:50:02.294677 flet_easy-0.2.0.dev6/src/flet_easy/extra.py
--rw-r--r--   0        0        0     2433 2024-03-25 23:45:31.430328 flet_easy-0.2.0.dev6/src/flet_easy/extrasJwt.py
--rw-r--r--   0        0        0    17128 2024-03-25 23:32:51.685370 flet_easy-0.2.0.dev6/src/flet_easy/fletEasy.py
--rw-r--r--   0        0        0    15891 2024-03-27 01:13:18.128343 flet_easy-0.2.0.dev6/src/flet_easy/inheritance.py
--rw-r--r--   0        0        0     1185 2024-03-25 22:51:59.196081 flet_easy-0.2.0.dev6/src/flet_easy/job.py
--rw-r--r--   0        0        0     4179 2024-03-25 23:43:23.222753 flet_easy-0.2.0.dev6/src/flet_easy/jwt.py
--rw-r--r--   0        0        0     8401 2024-03-25 23:43:02.355530 flet_easy-0.2.0.dev6/src/flet_easy/route.py
--rw-r--r--   0        0        0     1666 2024-03-25 23:14:02.368363 flet_easy-0.2.0.dev6/src/flet_easy/view_404.py
--rw-r--r--   0        0        0     5251 1970-01-01 00:00:00.000000 flet_easy-0.2.0.dev6/PKG-INFO
+-rw-r--r--   0        0        0    11541 2024-03-27 23:22:54.481270 flet_easy-0.2.0.dev7/LICENSE
+-rw-r--r--   0        0        0    11541 2024-03-27 23:22:54.481270 flet_easy-0.2.0.dev7/LICENSE
+-rw-r--r--   0        0        0     4215 2024-03-27 23:22:54.482257 flet_easy-0.2.0.dev7/README.md
+-rw-r--r--   0        0        0     4215 2024-03-27 23:22:54.482257 flet_easy-0.2.0.dev7/README.md
+-rw-r--r--   0        0        0     1564 2024-04-07 23:54:34.630972 flet_easy-0.2.0.dev7/pyproject.toml
+-rw-r--r--   0        0        0      432 2024-04-07 22:47:44.055967 flet_easy-0.2.0.dev7/src/flet_easy/__init__.py
+-rw-r--r--   0        0        0    13856 2024-03-30 00:26:40.645132 flet_easy-0.2.0.dev7/src/flet_easy/__pycache__/route.cpython-311.pyc.2038480740688
+-rw-r--r--   0        0        0     2356 2024-04-02 03:23:24.628507 flet_easy-0.2.0.dev7/src/flet_easy/cli/copy.py
+-rw-r--r--   0        0        0     2099 2024-03-27 23:30:22.585369 flet_easy-0.2.0.dev7/src/flet_easy/cli/main.py
+-rw-r--r--   0        0        0     3266 2024-03-27 23:25:17.554726 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/.gitignore
+-rw-r--r--   0        0        0      213 2024-03-27 23:25:17.554726 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/README.md
+-rw-r--r--   0        0        0     1020 2024-03-27 23:25:17.555756 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/favicon.png
+-rw-r--r--   0        0        0    30189 2024-03-27 23:25:17.556749 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icon.png
+-rw-r--r--   0        0        0     7610 2024-03-27 23:25:17.557757 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-192.png
+-rw-r--r--   0        0        0    33055 2024-03-27 23:25:17.558274 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-512.png
+-rw-r--r--   0        0        0     7610 2024-03-27 23:25:17.559303 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    33055 2024-03-27 23:25:17.560320 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    56474 2024-03-27 23:25:17.562336 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/loading-animation.png
+-rw-r--r--   0        0        0     3626 2024-03-27 23:25:17.562336 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/index.html
+-rw-r--r--   0        0        0      932 2024-03-27 23:25:17.563331 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/manifest.json
+-rw-r--r--   0        0        0       84 2024-03-27 23:30:22.582338 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/components/__init__.py
+-rw-r--r--   0        0        0     2422 2024-03-27 23:30:22.583375 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/components/counter.py
+-rw-r--r--   0        0        0      543 2024-03-27 23:25:17.564875 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/components/swoDrawer.py
+-rw-r--r--   0        0        0       44 2024-03-27 23:30:22.583375 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/controllers/__init__.py
+-rw-r--r--   0        0        0     1258 2024-03-27 23:30:22.580809 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/controllers/counter.py
+-rw-r--r--   0        0        0        0 2024-03-27 23:25:17.567392 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/core/__init__.py
+-rw-r--r--   0        0        0     1662 2024-03-27 23:25:17.568421 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/core/config.py
+-rw-r--r--   0        0        0      304 2024-03-27 23:25:17.568421 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/main.py
+-rw-r--r--   0        0        0        0 2024-03-27 23:25:17.568421 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/models/__init__.py
+-rw-r--r--   0        0        0       66 2024-03-27 23:30:22.586373 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/views/__init__.py
+-rw-r--r--   0        0        0      588 2024-03-27 23:30:22.580809 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/views/counter.py
+-rw-r--r--   0        0        0      615 2024-03-27 23:25:17.571969 flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/views/index.py
+-rw-r--r--   0        0        0    12191 2024-04-07 23:18:44.195005 flet_easy-0.2.0.dev7/src/flet_easy/datasy.py
+-rw-r--r--   0        0        0      187 2024-04-07 23:06:12.478685 flet_easy-0.2.0.dev7/src/flet_easy/extra.py
+-rw-r--r--   0        0        0     2483 2024-04-07 23:06:20.563626 flet_easy-0.2.0.dev7/src/flet_easy/extrasJwt.py
+-rw-r--r--   0        0        0    18283 2024-04-07 23:06:36.428370 flet_easy-0.2.0.dev7/src/flet_easy/fletEasy.py
+-rw-r--r--   0        0        0     9732 2024-04-07 23:06:51.294251 flet_easy-0.2.0.dev7/src/flet_easy/inheritance.py
+-rw-r--r--   0        0        0     1191 2024-04-07 23:07:10.214456 flet_easy-0.2.0.dev7/src/flet_easy/job.py
+-rw-r--r--   0        0        0     3987 2024-04-07 23:09:10.638387 flet_easy-0.2.0.dev7/src/flet_easy/jwt.py
+-rw-r--r--   0        0        0     7534 2024-04-07 23:10:13.620117 flet_easy-0.2.0.dev7/src/flet_easy/pagesy.py
+-rw-r--r--   0        0        0    11102 2024-04-07 23:13:15.908162 flet_easy-0.2.0.dev7/src/flet_easy/route.py
+-rw-r--r--   0        0        0     1540 2024-04-07 23:13:26.115988 flet_easy-0.2.0.dev7/src/flet_easy/view_404.py
+-rw-r--r--   0        0        0     5251 1970-01-01 00:00:00.000000 flet_easy-0.2.0.dev7/PKG-INFO
```

### Comparing `flet_easy-0.2.0.dev6/LICENSE` & `flet_easy-0.2.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/README.md` & `flet_easy-0.2.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/copy.py` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/copy.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 elif item.is_dir():
                     copytree(
                         item,
                         to_path / item.name,
                         ignore=ignore_patterns(*patterns_to_ignore),
                     )
             except Exception as e:
-                print(e)
+                raise Exception(e)
 
         colors = [
             "orange_red1",
             "dark_cyan",
             "gold1",
             "bright_yellow",
             "dodger_blue1",
@@ -58,13 +58,17 @@
             if path.isfile(struct / f):
                 print(f"[{colors[n_color]}] : {f} [/{colors[n_color]}] created")
                 n_color += 1
 
         print("[light_sky_blue3] : pyproject.toml [/light_sky_blue3] created")
 
         if manifest == "y":
-            print("\n[blue]● It has ended correctly. Remember to customize manifest.json and the icons in the assets folder :)[/blue]")
+            print(
+                "\n[blue]● It has ended correctly. Remember to customize manifest.json and the icons in the assets folder :)[/blue]"
+            )
         else:
             print("\n[blue]● It has finished correctly.[/blue]")
 
     except FileExistsError:
-        print(f"\n[red1 bold]Alert:[/red1 bold] A folder with the same name already exists. [green]({to_path})[/green]")
+        print(
+            f"\n[red1 bold]Alert:[/red1 bold] A folder with the same name already exists. [green]({to_path})[/green]"
+        )
```

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/main.py` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from rich.prompt import Prompt
 from rich_argparse import RichHelpFormatter
 from tomlkit import dump
 
 from .copy import _copy_template
 
-VERSION = "0.2.0.dev6"
+VERSION = "0.2.0"
 
 RichHelpFormatter.styles["argparse.text"] = "italic"
 RichHelpFormatter.styles["argparse.help"] = "light_sky_blue3"
 RichHelpFormatter.styles["argparse.prog"] = "blue"
 
 
 def init_app():
@@ -23,36 +23,47 @@
     version = Prompt.ask("Project Version", default="0.1.0")
     license = Prompt.ask(
         "Project License",
         default="MIT",
     )
     author = Prompt.ask("Project Author")
     email = Prompt.ask("Email Author")
-    manifest = Prompt.ask("Requires creation of manifest.json (Web-PWA)", choices=["n", "y"], default="n")
+    manifest = Prompt.ask(
+        "Requires creation of manifest.json (Web-PWA)", choices=["n", "y"], default="n"
+    )
 
     toml_dict["project"]["name"] = name
     toml_dict["project"]["version"] = version
     toml_dict["project"]["license"] = license
     toml_dict["project"]["authors"] = [{"name": author, "email": email}]
     toml_dict["project"]["dependencies"] = ["flet", "flet-easy"]
 
     _copy_template("templates", pwd / name, manifest)
 
     with open(f"{pwd}/{name}/pyproject.toml", "w") as file:
         dump(toml_dict, file)
 
 
 def run():
-    parser = argparse.ArgumentParser(description="CLI for Flet-Easys.", formatter_class=RichHelpFormatter)
-    parser.add_argument("--version", "-v", action="version", help=" Flet-Easy Version", version=VERSION)
+    parser = argparse.ArgumentParser(
+        description="CLI for Flet-Easys.", formatter_class=RichHelpFormatter
+    )
+    parser.add_argument(
+        "--version", "-v", action="version", help=" Flet-Easy Version", version=VERSION
+    )
 
     subparsers = parser.add_subparsers(dest="command", title="Comandos")
 
     #  Subcommand 'init'
-    subparsers.add_parser("init", aliases=["i"], help="Create the structure of the app", formatter_class=RichHelpFormatter)
+    subparsers.add_parser(
+        "init",
+        aliases=["i"],
+        help="Create the structure of the app",
+        formatter_class=RichHelpFormatter,
+    )
 
     args = parser.parse_args()
 
     if args.command == "init" or args.command == "i":
         with contextlib.suppress(KeyboardInterrupt):
             init_app()
     else:
```

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/.gitignore` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/favicon.png` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/icon.png` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icon.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/icons/icon-192.png` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/icons/icon-512.png` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/icons/loading-animation.png` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/index.html` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/index.html`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/assets/manifest.json` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/assets/manifest.json`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/components/counter.py` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/components/counter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import flet as ft
 from controllers import CounterHook
 
 
 class Counter(ft.UserControl):
-    def __init__(self, page: ft.Page, id: str, width: int | float, height: int | float = None) -> ft.Control:
+    def __init__(
+        self, page: ft.Page, id: str, width: int | float, height: int | float = None
+    ) -> ft.Control:
         super().__init__()
         self.counter = CounterHook()
         self.id = id
         self.height = height
         self.width = width
         self.page = page
         self.page.snack_bar = ft.SnackBar(ref=self.counter.alert, content=ft.Text(""))
```

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/components/swoDrawer.py` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/components/swoDrawer.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/controllers/counter.py` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/controllers/counter.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,35 +13,29 @@
             int(self.input.c.value)
             if self.input.c.value is not None and self.input.c.value != ""
             else 1
         )
 
     def is_number(self):
         if not self.input.c.value.isdigit():
-            self.alert.c.content = ft.Text(
-                "Enter number", text_align="center", color="#ffffff"
-            )
+            self.alert.c.content = ft.Text("Enter number", text_align="center", color="#ffffff")
             self.alert.c.bgcolor = "#ef233c"
             self.alert.c.open = True
             self.alert.c.update()
             return False
         return True
 
     def add(self, e):
         if self.is_number():
-            self.number.c.text = str(
-                int(self.number.c.text) + self.get_input()
-            )
+            self.number.c.text = str(int(self.number.c.text) + self.get_input())
             self.number.c.update()
 
     def remove(self, e):
         if self.is_number():
-            self.number.c.text = str(
-                int(self.number.c.text) - self.get_input()
-            )
+            self.number.c.text = str(int(self.number.c.text) - self.get_input())
             self.number.c.update()
 
     def reload(self, e):
         self.number.c.text = "0"
         self.input.c.value = "1"
         self.input.c.update()
         self.number.c.update()
```

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/core/config.py` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/core/config.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/views/counter.py` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/views/counter.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 import flet_easy as fs
 from components import Counter, SwoDrawer
 
 counter = fs.AddPagesy(
     route_prefix="/counter",
 )
 
+
 # We add a second page
 @counter.page(route="/test/{id}", title="Counter")
 def counter_page(data: fs.Datasy, id: str):
     page = data.page
     view = data.view
 
     return ft.View(
-        controls=[
-            Counter(page=page, id=id, width=250),
-            SwoDrawer("Show_drawer", view.drawer)
-        ],
+        controls=[Counter(page=page, id=id, width=250), SwoDrawer("Show_drawer", view.drawer)],
         vertical_alignment=ft.MainAxisAlignment.CENTER,
         horizontal_alignment=ft.CrossAxisAlignment.CENTER,
         drawer=view.drawer,
     )
```

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/cli/templates/views/index.py` & `flet_easy-0.2.0.dev7/src/flet_easy/cli/templates/views/index.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/datasy.py` & `flet_easy-0.2.0.dev7/src/flet_easy/datasy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from datetime import datetime, timedelta, timezone
-from typing import Any
+from typing import Any, Callable, Dict
 
-from flet import (
-    ControlEvent,
-    Page,
-    View,
-)
+from flet import Page
 
-from flet_easy.extra import Msg
+from flet_easy.extra import Msg, Redirect
 from flet_easy.extrasJwt import (
     SecretKey,
     _decode_payload_async,
     encode_verified,
 )
-from flet_easy.inheritance import Keyboardsy, Resizesy, SessionStorageEdit
+from flet_easy.inheritance import Keyboardsy, Resizesy, SessionStorageEdit, Viewsy
 from flet_easy.job import Job
 
 
 class Datasy:
     """
     The decorated function will always receive a parameter which is `data` (can be any name), which will make an object of type `Datasy` of `Flet-Easy`.
 
@@ -39,65 +35,73 @@
         * `get_all` : Get the dictionary of all shared values.
     ----
     * `on_keyboard_event` : get event values to use in the page.
     * `on_resize` : get event values to use in the page.
     * `logout` : method to close sessions of all sections in the browser (client storage), requires as parameter the key or the control (the parameter key of the control must have the value to delete), this is to avoid creating an extra function.
     * `login` : method to create sessions of all sections in the browser (client storage), requires as parameters the key and the value, the same used in the `page.client_storage.set` method.
     * `go` : Method to change the path of the application, in order to reduce the code, you must assign the value of the `key` parameter of the `control` used, for example buttons.
+    * `route` : route provided by the route event, it is useful when using middlewares to check if the route is assecible.
+    * `redirect` : To redirect to a path before the page loads, it is used in middleware.
     """
 
     def __init__(
         self,
         page: Page,
         route_prefix: str,
         route_init: str,
         route_login: str,
         secret_key: str,
         auto_logout: bool,
+        page_on_keyboard: Keyboardsy,
+        page_on_resize: Resizesy,
         login_async: bool = False,
+        go: Callable[[str], None] = None,
     ) -> None:
         self.__page: Page = page
-        self.__url_params: dict = None
-        self.__view: View = None
-        self.__route_prefix: str = route_prefix
-        self.__route_init: str = route_init
-        self.__route_login: str = route_login
+        self.__url_params: Dict[str, Any] = None
+        self.__view: Viewsy = None
+        self.__route_prefix = route_prefix
+        self.__route_init = route_init
+        self.__route_login = route_login
         self.__share = SessionStorageEdit(self.__page)
-        self.__on_keyboard_event: Keyboardsy = None
-        self.__on_resize: Resizesy = None
+        self.__on_keyboard_event = page_on_keyboard
+        self.__on_resize = page_on_resize
+        self.__route: str = None
+        self.__go = go
 
         self.__secret_key: SecretKey = secret_key
         self.__key_login: str = None
         self.__auto_logout: bool = auto_logout
         self.__sleep: int = 1
         self._login_done: bool = False
         self._login_async: bool = login_async
+        self._check_event_router: bool = False
 
     @property
     def page(self):
         return self.__page
 
     @page.setter
     def page(self, page: object):
         self.__page = page
 
     @property
     def url_params(self):
         return self.__url_params
 
     @url_params.setter
-    def url_params(self, url_params: dict):
+    def url_params(self, url_params: Dict[str, Any]):
         self.__url_params = url_params
 
     @property
     def view(self):
         return self.__view
 
     @view.setter
-    def view(self, view: View):
+    def view(self, view: Viewsy):
         self.__view = view
 
     @property
     def route_prefix(self):
         return self.__route_prefix
 
     @route_prefix.setter
@@ -149,32 +153,40 @@
     def auto_logout(self):
         return self.__auto_logout
 
     @property
     def secret_key(self):
         return self.__secret_key
 
+    @property
+    def route(self):
+        return self.__route
+
+    @route.setter
+    def route(self, route: str):
+        self.__route = route
+
     """--------- login authentication : asynchronously | synchronously -------"""
 
     def _login_done_evaluate(self):
         return self._login_done
 
-    def _create_task_login_update(self, decode: dict[str, Any]):
+    def _create_task_login_update(self, decode: Dict[str, Any]):
         """Updates the login status, in case it does not exist it creates a new task that checks the user's login status."""
         time_exp = datetime.fromtimestamp(float(decode.get("exp")), tz=timezone.utc)
         time_now = datetime.now(tz=timezone.utc)
         time_res = time_exp - time_now
         self._login_done = True
         Job(
-            self.logout,
-            self.key_login,
+            func=self.logout,
+            key=self.key_login,
             every=time_res,
-            sleep_time=self.__sleep,
             page=self.page,
             login_done=self._login_done_evaluate,
+            sleep_time=self.__sleep,
         ).start()
 
     def logout(self, key: str):
         """Closes the sessions of all browser tabs or the device used, which has been previously configured with the `login` method.
 
         ### Example:
         ```python
@@ -185,100 +197,129 @@
         def dashboard(data:fs.Datasy)
             return ft.View(
                 controls=[
                     ft.FilledButton('Logout', onclick=data.logout('key-login')),
             )
         ```
         """
-        if self.page.web:
-            self.page.pubsub.send_all_on_topic(self.page.client_ip, Msg("logout", key))
-        else:
-            self.page.client_storage.remove_async(key)
-            self.page.go(self.route_login)
+
+        def execute():
+            assert self.route_login is not None, "Adds a login path in the FletEasy Class"
+            if self.page.web:
+                self.page.pubsub.send_all_on_topic(self.page.client_ip, Msg("logout", key))
+            else:
+                self.page.run_task(self.page.client_storage.remove_async, key)
+                self.page.go(self.route_login)
+
+        return lambda _=None: execute()
 
     async def __logaut_init(self, topic, msg: Msg):
         if msg.method == "login":
-            self.page.run_task(self.page.client_storage.set_async, msg.key, msg.value)
+            self._check_event_router = False
+            await self.page.client_storage.set_async(msg.key, msg.value.get("value"))
+            if self.page.route == self.route_login:
+                self.page.go(msg.value.get("next_route"))
 
         elif msg.method == "logout":
             self._login_done = False
-            self.page.run_task(self.page.client_storage.remove_async, msg.key)
+            self._check_event_router = False
+            await self.page.client_storage.remove_async(msg.key)
             self.page.go(self.route_login)
 
         elif msg.method == "updateLogin":
             self._login_done = msg.value
 
         elif msg.method == "updateLoginSessions":
             self._login_done = msg.value
             self._create_task_login_update(
                 decode=await _decode_payload_async(
                     page=self.page,
                     key_login=self.key_login,
-                    secret_key=(self.secret_key.secret if self.secret_key.secret is not None else self.secret_key.pem_key.public),
+                    secret_key=(
+                        self.secret_key.secret
+                        if self.secret_key.secret is not None
+                        else self.secret_key.pem_key.public
+                    ),
                     algorithms=self.secret_key.algorithm,
                 )
             )
         else:
-            Exception("Method not implemented in logout_init method.")
+            raise ValueError("Method not implemented in logout_init method.")
 
     def _create_login(self):
         """Create the connection between sessions."""
         self.page.pubsub.subscribe_topic(self.page.client_ip, self.__logaut_init)
 
     def _create_tasks(self, time_expiry: timedelta, key: str, sleep: int) -> None:
         """Creates the logout task when logging in."""
         if time_expiry is not None:
             Job(
-                self.logout,
-                key,
+                func=self.logout,
+                key=key,
                 every=time_expiry,
-                sleep_time=sleep,
                 page=self.page,
                 login_done=self._login_done_evaluate,
+                sleep_time=sleep,
             ).start()
 
     def login(
         self,
         key: str,
-        value: dict[str, Any] | Any,
+        value: Dict[str, Any] | Any,
+        next_route: str,
         time_expiry: timedelta = None,
-        next_route: str = None,
         sleep: int = 1,
     ):
         """Registering in the client's storage the key and value in all browser sessions.
 
         ### Parameters to use:
 
         * `key` : It is the identifier to store the value in the client storage.
         * `value` : Recommend to use a dict if you use JWT.
+        * `next_route` : Redirect to next route after creating login.
         * `time_expiry` : Time to expire the session, use the `timedelta` class  to configure. (Optional)
-        * `next_route` : Redirect to next route after creating login. (Optional)
         * `sleep` : Time to do login checks, default is 1s. (Optional)
         """
-        if self.__secret_key.Jwt:
+        if time_expiry:
+            assert isinstance(
+                value, Dict
+            ), "Use a dict in login method values or don't use time_expiry."
+            assert (
+                self.__secret_key is not None
+            ), "Set the secret_key in the FletEasy class parameter or don't use time_expiry."
+
+        if self.__secret_key:
             evaluate_secret_key(self)
             self.__key_login = key
             self.__sleep = sleep
             value = encode_verified(self.secret_key, value, time_expiry)
             self._login_done = True
 
             if self.__auto_logout:
                 self._create_tasks(time_expiry, key, sleep)
 
-        self.page.run_task(self.page.client_storage.set_async, key, value)
-        self.page.pubsub.send_others_on_topic(self.page.client_ip, Msg("login", key, value))
-
-        if next_route is not None:
-            self.page.go(next_route)
+        if self.page.web:
+            self.page.pubsub.send_all_on_topic(
+                self.page.client_ip, Msg("login", key, {"value": value, "next_route": next_route})
+            )
+        else:
+            self.page.run_task(self.page.client_storage.set_async, key, value)
+            self.__go(next_route)
 
     """ Page go  """
 
-    def go(self, route: ControlEvent | str):
-        """To change the path of the app, in order to reduce code, you must assign the value of the `key` parameter of the `control` used, for example buttons."""
-        if isinstance(route, str):
-            return lambda _: self.page.go(route)
-        else:
-            return lambda _: self.page.go(route.control.key)
+    def go(self, route: str):
+        """To change the application path, it is important for better validation to avoid using `page.go()`."""
+        return lambda _=None: self.__go(route)
+
+    def redirect(self, route: str):
+        """Useful if you do not want to access a route that has already been sent."""
+        return Redirect(route)
 
 
 def evaluate_secret_key(data: Datasy):
-    assert data.secret_key.secret is None and data.secret_key.algorithm == "RS256" or data.secret_key.pem_key is None and data.secret_key.algorithm == "HS256", "The algorithm is not set correctly in the 'secret_key' parameter of the 'FletEasy' class."
+    assert (
+        data.secret_key.secret is None
+        and data.secret_key.algorithm == "RS256"
+        or data.secret_key.pem_key is None
+        and data.secret_key.algorithm == "HS256"
+    ), "The algorithm is not set correctly in the 'secret_key' parameter of the 'FletEasy' class."
```

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/extrasJwt.py` & `flet_easy-0.2.0.dev7/src/flet_easy/extrasJwt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from datetime import datetime, timezone
-from typing import Any
+from typing import Any, Dict
 
 from flet import Page
 from jwt import decode, encode
 
 
 @dataclass
 class Algorithm:
@@ -24,41 +24,43 @@
 
     algorithm: str = "HS256"
     secret: str = None
     pem_key: PemKey = None
     Jwt: bool = False
 
 
-def _time_exp(time_expiry: timezone, payload: dict[str, Any]) -> dict[str, Any]:
+def _time_exp(time_expiry: timezone, payload: Dict[str, Any]) -> dict[str, Any]:
     if time_expiry is not None:
         payload["exp"] = datetime.now(tz=timezone.utc) + time_expiry
     return payload
 
 
-def encode_RS256(payload: dict[str, Any], private: str, time_expiry: timezone = None) -> str:
+def encode_RS256(payload: Dict[str, Any], private: str, time_expiry: timezone = None) -> str:
     payload = _time_exp(time_expiry, payload)
     return encode(
         payload=payload,
         key=private,
         algorithm="RS256",
     )
 
 
-def encode_HS256(payload: dict[str, Any], secret_key: str, time_expiry: timezone = None) -> str:
+def encode_HS256(payload: Dict[str, Any], secret_key: str, time_expiry: timezone = None) -> str:
     payload = _time_exp(time_expiry, payload)
     return encode(
         payload=payload,
         key=secret_key,
         algorithm="HS256",
     )
 
 
 def encode_verified(secret_key: SecretKey, value: str, time_expiration) -> str | None:
     """Verify the possible encryption of the value sent."""
-    assert secret_key.algorithm is not None, "The secret_key algorithm is not supported, only (RS256, HS256) is accepted."
+    assert (
+        secret_key.algorithm is not None
+    ), "The secret_key algorithm is not supported, only (RS256, HS256) is accepted."
 
     if secret_key.algorithm == "RS256":
         return encode_RS256(
             payload=value,
             private=secret_key.pem_key.private,
             time_expiry=time_expiration,
         )
@@ -68,16 +70,20 @@
             secret_key=secret_key.secret,
             time_expiry=time_expiration,
         )
     else:
         Exception("Algorithm not implemented in encode_verified method.")
 
 
-async def _decode_payload_async(page: Page, key_login: str, secret_key: str, algorithms: str) -> dict[str, Any]:
+async def _decode_payload_async(
+    page: Page, key_login: str, secret_key: str, algorithms: str
+) -> Dict[str, Any]:
     """Decodes the payload stored in the client storage."""
-    assert secret_key is not None, "The secret_key algorithm is not supported, only (RS256, HS256) is accepted."
+    assert (
+        secret_key is not None
+    ), "The secret_key algorithm is not supported, only (RS256, HS256) is accepted."
 
     return decode(
         jwt=await page.client_storage.get_async(key_login),
         key=secret_key,
         algorithms=[algorithms],
     )
```

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/fletEasy.py` & `flet_easy-0.2.0.dev7/src/flet_easy/fletEasy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 try:
     from flet import AppView, Page, WebRenderer, app
 except ImportError:
     raise Exception('Install "flet" the latest version available -> pip install flet --upgrade.')
 
 from functools import wraps
-from typing import Callable, Optional
+from typing import Any, Callable, Dict, List, Optional
 
+from flet import View
+
+from flet_easy.datasy import Datasy
 from flet_easy.extrasJwt import SecretKey
-from flet_easy.inheritance import AddPagesy, Pagesy, Viewsy
+from flet_easy.inheritance import Viewsy
+from flet_easy.pagesy import AddPagesy, Middleware, Pagesy
 from flet_easy.route import FletEasyX
 
 
 class FletEasy:
     """we create the app object, in it you can configure:
     * The path that is different from '/'.
     * The initial path when initializing the app
@@ -19,111 +23,107 @@
 
     Example:
     ```python
     import flet as ft
     import flet_easy as fs
 
     app = fs.FletEasy(
-        route_prefix='/index',
-        route_init='/index/hi',
+        route_prefix="/index",
+        route_init="/index/hi",
     )
 
+
     @app.view()
     async def view(page: ft.Page):
         def modify_theme():
             if page.theme_mode == ft.ThemeMode.DARK:
                 page.theme_mode = ft.ThemeMode.LIGHT
             else:
                 page.theme_mode = ft.ThemeMode.DARK
+
         async def theme(e):
             if page.theme_mode == ft.ThemeMode.SYSTEM:
                 modify_theme()
             modify_theme()
             await page.update_async()
+
         async def go_home(e):
-            await page.go_async('/index/hi')
+            await page.go_async("/index/hi")
+
         return fs.Viewsy(
             appbar=ft.AppBar(
                 title=ft.Text("AppBar Example"),
                 center_title=False,
                 bgcolor=ft.colors.SURFACE_VARIANT,
                 actions=[
-                    ft.IconButton(ft.icons.WB_SUNNY_OUTLINED,
-                                  on_click=theme
-                                  ),
+                    ft.IconButton(ft.icons.WB_SUNNY_OUTLINED, on_click=theme),
                     ft.PopupMenuButton(
                         items=[
-                            ft.PopupMenuItem(
-                                text="🔥 Home",
-                                on_click=go_home
-                            ),
+                            ft.PopupMenuItem(text="🔥 Home", on_click=go_home),
                         ]
                     ),
                 ],
             ),
             vertical_alignment=ft.MainAxisAlignment.CENTER,
-            horizontal_alignment=ft.CrossAxisAlignment.CENTER
+            horizontal_alignment=ft.CrossAxisAlignment.CENTER,
         )
 
-    @app.page('/hi', page_clear=True)
+
+    @app.page("/hi", page_clear=True)
     async def index_page(data: fs.Datasy):
         page = data.page
         view = data.view
-        page.title = 'Index - Home'
+        page.title = "Index - Home"
 
-        view.appbar.title = ft.Text('Index - Home')
+        view.appbar.title = ft.Text("Index - Home")
 
         async def go_test(e):
-            await page.go_async(f'/index/test/10/user/junior')
-
+            await page.go_async(f"/index/test/10/user/junior")
 
         return ft.View(
-            '/index/hi',
+            "/index/hi",
             controls=[
-
-                ft.Text('Menú', size=40),
+                ft.Text("Menú", size=40),
                 ft.ElevatedButton(
-                    'Go to Test', on_click=go_test,
-                )
-
+                    "Go to Test",
+                    on_click=go_test,
+                ),
             ],
             appbar=view.appbar,
             vertical_alignment=ft.MainAxisAlignment.CENTER,
-            horizontal_alignment=ft.CrossAxisAlignment.CENTER
+            horizontal_alignment=ft.CrossAxisAlignment.CENTER,
         )
 
-    @app.page('/test/{id:d}/user/{name:l}')
-    async def test_page(data: fs.Datasy, id:int, name:str):
+
+    @app.page("/test/{id:d}/user/{name:l}")
+    async def test_page(data: fs.Datasy, id: int, name: str):
         page = data.page
         view = data.view
 
-        page.title = 'Test'
-        view.appbar.title = ft.Text('test')
+        page.title = "Test"
+        view.appbar.title = ft.Text("test")
 
         async def go_index(e):
-            await page.go_async(f'/index/hi')
+            await page.go_async(f"/index/hi")
 
         return ft.View(
-            '/index/test',
+            "/index/test",
             controls=[
-
-                ft.Text(f'Test {data.url_params}'),
-                ft.Text(f'Test Id is: {id}'),
-                ft.ElevatedButton(
-                    'Go to Home', on_click=go_index),
-
+                ft.Text(f"Test {data.url_params}"),
+                ft.Text(f"Test Id is: {id}"),
+                ft.ElevatedButton("Go to Home", on_click=go_index),
             ],
             appbar=view.appbar,
             vertical_alignment=ft.MainAxisAlignment.CENTER,
-            horizontal_alignment=ft.CrossAxisAlignment.CENTER
+            horizontal_alignment=ft.CrossAxisAlignment.CENTER,
         )
 
+
     # Execute the app (synchronous / asynchronous)
     app.run()
-
     ```
     """
 
     def __init__(
         self,
         route_prefix: str = None,
         route_init: str = "/",
@@ -136,21 +136,22 @@
         self.__route_prefix = route_prefix
         self.__route_init = route_init
         self.__route_login = route_login
         self.__on_resize = on_resize
         self.__on_Keyboard = on_Keyboard
         self.__secret_key = secret_key
         self.__auto_logout = auto_logout
-        self.__config_login: Callable = None
+        self.__config_login: Callable[[Datasy], View] = None
         # ----
         self.__pages = set()
         self.__page_404: Pagesy = None
         self.__view_data: Viewsy = None
-        self.__view_config: Callable = None
-        self.__config_event: Callable = None
+        self.__view_config: Callable[[Datasy], None] = None
+        self.__config_event: Callable[[Datasy], None] = None
+        self.__middlewares: Middleware = None
 
     # -------------------------------------------------------------------
     # -- initialize / Supports async
 
     def run(
         self,
         name="",
@@ -161,15 +162,15 @@
         upload_dir=None,
         web_renderer: WebRenderer = WebRenderer.CANVAS_KIT,
         use_color_emoji=False,
         route_url_strategy="path",
         export_asgi_app: bool = False,
         fastapi: bool = False,
     ) -> Page:
-        """* Execute the app. | Supports async and fastapi."""
+        """* Execute the app. | Soporta async, fastapi y export_asgi_app."""
 
         def main(page: Page):
             app = FletEasyX(
                 page=page,
                 route_prefix=self.__route_prefix,
                 route_init=self.__route_init,
                 route_login=self.__route_login,
@@ -179,67 +180,79 @@
                 view_data=self.__view_data,
                 view_config=self.__view_config,
                 config_event_handler=self.__config_event,
                 on_resize=self.__on_resize,
                 on_Keyboard=self.__on_Keyboard,
                 secret_key=self.__secret_key,
                 auto_logout=self.__auto_logout,
+                middleware=self.__middlewares,
             )
 
             app.run()
 
         if fastapi:
             return main
         try:
-            app(
+            return app(
                 target=main,
                 name=name,
                 host=host,
                 port=port,
                 view=view,
                 assets_dir=assets_dir,
                 upload_dir=upload_dir,
                 web_renderer=web_renderer,
                 use_color_emoji=use_color_emoji,
                 route_url_strategy=route_url_strategy,
                 export_asgi_app=export_asgi_app,
             )
         except RuntimeError:
-            Exception("If you are using fastapi from flet, set the 'fastapi = True' parameter of the run() method.")
+            raise Exception(
+                "Ifs you are using fastapi from flet, set the 'fastapi = True' parameter of the run() method."
+            )
 
     # -- decorators --------------------------------
 
-    def __decorator(self, value: str, data: dict = None):
+    def __decorator(self, value: str, data: Dict[str, Any] = None):
         def decorator(func: Callable):
             @wraps(func)
             def wrapper(data, *args, **kwargs):
                 return func(data, *args, **kwargs)
 
             if data:
-                route = (self.__route_prefix if data.get("route") == "/" else self.__route_prefix + data.get("route")) if self.__route_prefix and data.get("route") else data.get("route")
+                route = (
+                    (
+                        self.__route_prefix
+                        if data.get("route") == "/"
+                        else self.__route_prefix + data.get("route")
+                    )
+                    if self.__route_prefix and data.get("route")
+                    else data.get("route")
+                )
 
             if value == "page_404":
                 self.__page_404 = Pagesy(route, func, data.get("title"), data.get("page_clear"))
             elif value == "page":
                 self.__pages.add(
                     Pagesy(
                         route=route,
                         view=func,
                         title=data.get("title"),
                         clear=data.get("page_clear"),
                         share_data=data.get("share_data"),
                         protected_route=data.get("protected_route"),
                         custom_params=data.get("custom_params"),
+                        middleware=data.get("middleware"),
                     )
                 )
             return wrapper
 
         return decorator
 
-    def add_pages(self, group_pages: list[AddPagesy]):
+    def add_pages(self, group_pages: List[AddPagesy]):
         """Add pages from other archives
         * In the list you enter objects of class `AddPagesy` from other .py files.
 
         Example:
         ```python
         app.add_pages([index, test, contador, login, task])
         ```
@@ -256,55 +269,58 @@
     def page(
         self,
         route: str,
         title: str = None,
         page_clear: bool = False,
         share_data: bool = False,
         protected_route: bool = False,
-        custom_params: dict = None,
+        custom_params: Dict[str, Any] = None,
+        middleware: Middleware = None,
     ):
         """Decorator to add a new page to the app, you need the following parameters:
         * route: text string of the url, for example(`'/FletEasy'`).
         * `title` : Define the title of the page. (optional).
         * clear: Removes the pages from the `page.views` list of flet. (optional)
+        * `share_data` : It is a boolean value, which is useful if you want to share data between pages, in a more restricted way. (optional)
         * protected_route: Protects the route of the page, according to the configuration of the `login` decorator of the `FletEasy` class. (optional)
         * custom_params: To add validation of parameters in the custom url using a list, where the key is the name of the parameter validation and the value is the custom function that must report a boolean value.
+        * `middleware` : It acts as an intermediary between different software components, intercepting and processing requests and responses. They allow adding functionalities to an application in a flexible and modular way. (optional)
 
         -> The decorated function must receive a parameter, for example `data:fs.Datasy`.
 
         Example:
         ```python
         import flet as ft
         import flet_easy as fs
 
         app = fs.FletEasy(
-            route_prefix='/FletEasy',
-            route_init='/FletEasy',
+            route_prefix="/FletEasy",
+            route_init="/FletEasy",
         )
 
-        @app.page('/', title='FletEasy')
+
+        @app.page("/", title="FletEasy")
         async def index_page(data: fs.Datasy):
             return ft.View(
-                route='/FletEasy',
-                controls=[
-                    ft.Text('FletEasy')
-                ],
+                route="/FletEasy",
+                controls=[ft.Text("FletEasy")],
                 vertical_alignment=view.vertical_alignment,
-                horizontal_alignment=view.horizontal_alignment
+                horizontal_alignment=view.horizontal_alignment,
             )
         ```
         """
 
         data = {
             "route": route,
             "title": title,
             "page_clear": page_clear,
             "share_data": share_data,
             "protected_route": protected_route,
             "custom_params": custom_params,
+            "middleware": middleware,
         }
         return self.__decorator("page", data)
 
     def page_404(
         self,
         route: str = None,
         title: str = None,
@@ -319,181 +335,182 @@
 
         Example:
         ```python
         import flet as ft
         import flet_easy as fs
 
         app = fs.FletEasy(
-            route_prefix='/FletEasy',
-            route_init='/FletEasy',
+            route_prefix="/FletEasy",
+            route_init="/FletEasy",
         )
 
-        @app.page_404('/FletEasy-404', title='Error 404', page_clear=True)
-        async def page404(data: fs.Datasy):
 
+        @app.page_404("/FletEasy-404", title="Error 404", page_clear=True)
+        async def page404(data: fs.Datasy):
             return ft.View(
-                route='/error404',
+                route="/error404",
                 controls=[
-                    ft.Text(f'Error 404', size=30),
+                    ft.Text(f"Error 404", size=30),
                 ],
                 vertical_alignment=ft.MainAxisAlignment.CENTER,
-                horizontal_alignment=ft.CrossAxisAlignment.CENTER
+                horizontal_alignment=ft.CrossAxisAlignment.CENTER,
             )
         ```
         """
         data = {"route": route, "title": title, "page_clear": page_clear}
         return self.__decorator("page_404", data)
 
-    def view(self, func):
+    def view(self, func: Callable[[Datasy], Viewsy]):
         """
         Decorator to add custom controls to the application, the decorator function will return the `Viewsy` class of `FletEasy`. Which will be obtained in functions with `data:fs.Datasy` parameter and can be added to the page view decorated with `data.view` of `FletEasy` class.
 
         * The decorator function must receive a mandatory parameter, for example: `data:ft.Datasy`.
         * Add universal controls to use on more than one page in an easy way.
 
         Example:
         ```python
         import flet as ft
         import flet_easy as fs
 
         app = fs.FletEasy(
-            route_prefix='/FletEasy',
-            route_init='/FletEasy',
+            route_prefix="/FletEasy",
+            route_init="/FletEasy",
         )
 
+
         @app.view
         async def view(data: fs.Datasy):
-
             page = data.page
 
             def modify_theme():
                 if page.theme_mode == ft.ThemeMode.DARK:
                     page.theme_mode = ft.ThemeMode.LIGHT
                 else:
                     page.theme_mode = ft.ThemeMode.DARK
 
             async def theme(e):
-
                 if page.theme_mode == ft.ThemeMode.SYSTEM:
                     modify_theme()
 
                 modify_theme()
                 await page.update_async()
 
             async def go_home(e):
-                await page.go_async('/FletEasy')
+                await page.go_async("/FletEasy")
 
             return fs.Viewsy(
                 appbar=ft.AppBar(
                     title=ft.Text("AppBar Example"),
                     center_title=False,
                     bgcolor=ft.colors.SURFACE_VARIANT,
                     actions=[
-                        ft.IconButton(ft.icons.WB_SUNNY_OUTLINED,
-                                      on_click=theme
-                                      ),
+                        ft.IconButton(ft.icons.WB_SUNNY_OUTLINED, on_click=theme),
                         ft.PopupMenuButton(
                             items=[
-                                ft.PopupMenuItem(
-                                    text="🔥 Home",
-                                    on_click=go_home
-                                ),
+                                ft.PopupMenuItem(text="🔥 Home", on_click=go_home),
                             ]
                         ),
                     ],
                 ),
                 vertical_alignment=ft.MainAxisAlignment.CENTER,
-                horizontal_alignment=ft.CrossAxisAlignment.CENTER
+                horizontal_alignment=ft.CrossAxisAlignment.CENTER,
             )
         ```
         """
         self.__view_data = func
 
-    def config(self, func):
+    def config(self, func: Callable[[Datasy], None]):
         """Decorator to add a custom configuration to the app:
 
         * The decorator function must receive a mandatory parameter, for example: `page:ft.Page`. Which can be used to make universal app configurations.
         * The decorator function does not return anything.
 
         Example:
         ```python
         import flet as ft
         import flet_easy as fs
 
         app = fs.FletEasy()
 
+
         @app.config
         async def config(page: ft.Page):
             theme = ft.Theme()
             platforms = ["android", "ios", "macos", "linux", "windows"]
             for platform in platforms:  # Removing animation on route change.
-                setattr(theme.page_transitions, platform,
-                        ft.PageTransitionTheme.NONE)
+                setattr(theme.page_transitions, platform, ft.PageTransitionTheme.NONE)
 
             theme.text_theme = ft.TextTheme()
             page.theme = theme
-
         ```
         """
         self.__view_config = func
 
-    def login(self, func):
+    def login(self, func: Callable[[Datasy], bool]):
         """Decorator to add a login configuration to the app (protected_route):
 
         * The decorator function must receive a mandatory parameter, for example: `page:ft.Page`. Which can be used to get information and perform universal settings of the app.
         * The decorator function must `return a boolean`.
 
         Example:
         ```python
         import flet as ft
         import flet_easy as fs
 
         app = fs.FletEasy()
 
+
         # Basic demo example for login test
         @app.login
         async def login_x(page: ft.Page):
             v = [False, True, False, False, True]
             value = v[random.randint(0, 4)]
             return value
         ```
         """
         self.__config_login = func
 
-    def config_event_handler(self, func):
+    def config_event_handler(self, func: Callable[[Datasy], None]):
         """Decorator to add charter event settings -> https://flet.dev/docs/controls/page#events
 
         Example:
         ```python
         @app.config_event_handler
         async def event_handler(page: ft.Page):
-
             async def on_disconnect_async(e):
                 print("Disconnect test application")
 
             page.on_disconnect = on_disconnect_async
         ```
         """
 
         self.__config_event = func
 
-    def add_routes(self, add_views: list[Pagesy]):
+    def add_routes(self, add_views: List[Pagesy]):
         """-> Add routes without the use of decorators.
 
         Example:
         ```python
-        app.add_routes(add_views=[
-            fs.Pagesy('/hi', index_page, True),
-            fs.Pagesy('/test/{id:d}/user/{name:l}', test_page, protected_route=True),
-            fs.Pagesy('/counter', counter_page),
-            fs.Pagesy('/task', task_page),
-            fs.Pagesy('/login/user', login_page),
-        ])
+        app.add_routes(
+            add_views=[
+                fs.Pagesy("/hi", index_page, True),
+                fs.Pagesy(
+                    "/test/{id:d}/user/{name:l}", test_page, protected_route=True
+                ),
+                fs.Pagesy("/counter", counter_page),
+                fs.Pagesy("/task", task_page),
+                fs.Pagesy("/login/user", login_page),
+            ]
+        )
         ```
         """
 
         assert len(add_views) != 0, "add view (add_view) in 'add_routes'."
         for page in add_views:
             if self.__route_prefix:
                 page.route = self.__route_prefix + page.route
 
             self.__pages.add(page)
+
+    def add_middleware(self, middleware: Middleware):
+        """The function that will act as middleware will receive as a single mandatory parameter `data : Datasy` and its structure or content may vary depending on the context and the specific requirements of the middleware."""
+        self.__middlewares = middleware
```

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/job.py` & `flet_easy-0.2.0.dev7/src/flet_easy/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 class Job:
     """Create time-definite tasks"""
 
     def __init__(
         self,
         func: Callable,
-        *arg,
+        key: str,
         every: timedelta,
-        sleep_time: int = 1,
         page: Page,
         login_done: bool,
+        sleep_time: int = 1,
     ):
         self.func = func
-        self.arg = arg
+        self.key = key
         self.every = every
         self.sleep_time = sleep_time
         self.task_running = False
         self.page = page
         self.login_done = login_done
         self.next_run_time = datetime.now() + self.every
 
@@ -36,11 +36,11 @@
             self.task_running = True
             self.page.run_task(self.run_task)
 
     async def run_task(self):
         while datetime.now() <= self.next_run_time and self.login_done():
             await sleep(self.sleep_time)
         if self.login_done():
-            self.func(self.arg)
+            self.func(self.key)()
 
     def stop(self):
         self.task_running = False
```

### Comparing `flet_easy-0.2.0.dev6/src/flet_easy/jwt.py` & `flet_easy-0.2.0.dev7/src/flet_easy/jwt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from secrets import token_bytes
-from typing import Any, Union
+from typing import Any, Dict, Union
 
 from jwt import DecodeError, ExpiredSignatureError, InvalidKeyError
 from rsa import newkeys
 
 from flet_easy.datasy import Datasy, evaluate_secret_key
 from flet_easy.extra import Msg
 from flet_easy.extrasJwt import _decode_payload_async
 
 
 class EasyKey:
     """To obtain a `secret_key` more easily, support algorithms [ HS256, RS256 ]
 
     ### Example:
-    ```
+    ```python
     import flet_easy as fs
 
     key = fs.EasyKey()
 
     # --- HS256
     SECRET_KEY = key.secret_key()
 
@@ -25,95 +25,92 @@
     PRIVATE_KEY = key.private_key()
     PUBLIC_KEY = key.public_key()
     ```
     """
 
     def __init__(self):
         (public_key, private_key) = newkeys(2048)
-        self.public_key = public_key
-        self.private_key = private_key
+        self.public = public_key
+        self.private = private_key
 
-    def private(self) -> str:
-        return self.private_key.save_pkcs1().decode("utf-8")
+    def private_key(self) -> str:
+        return self.private.save_pkcs1().decode("utf-8")
 
-    def public(self) -> str:
-        return self.public_key.save_pkcs1().decode("utf-8")
+    def public_key(self) -> str:
+        return self.public.save_pkcs1().decode("utf-8")
 
     def secret_key(self) -> str:
         return token_bytes(64).hex().encode("utf-8")
 
 
-async def _handle_decode_errors(data: Datasy, key_login: str) -> Union[dict[str, Any], bool]:
+async def _handle_decode_errors(data: Datasy, key_login: str) -> Union[Dict[str, Any], bool]:
     """decodes the jwt and updates the browser sessions."""
     try:
         evaluate_secret_key(data)
 
         if not await data.page.client_storage.contains_key_async(key_login):
             return False
 
         if data.auto_logout and not data._login_done:
-            data.page.pubsub.send_others_on_topic(data.page.client_ip, Msg("updateLogin", value=data._login_done))
+            data.page.pubsub.send_others_on_topic(
+                data.page.client_ip, Msg("updateLogin", value=data._login_done)
+            )
 
         decode = await _decode_payload_async(
             page=data.page,
             key_login=key_login,
-            secret_key=(data.secret_key.secret if data.secret_key.secret is not None else data.secret_key.pem_key.public),
+            secret_key=(
+                data.secret_key.secret
+                if data.secret_key.secret is not None
+                else data.secret_key.pem_key.public
+            ),
             algorithms=data.secret_key.algorithm,
         )
 
         """ It checks if there is a logout time, if there is a logout task running and finally if the user wants to create a logout task. """
         if decode.get("exp") and not data._login_done and data.auto_logout:
             data._create_task_login_update(decode)
 
         return decode
 
     except ExpiredSignatureError:
-        data.logout(key_login)
+        data.logout(key_login)()
         return False
     except InvalidKeyError:
-        data.logout(key_login)
+        data.logout(key_login)()
         return False
     except DecodeError as e:
-        data.logout(key_login)
+        data.logout(key_login)()
         Exception(
             "Decoding error, possibly there is a double use of the 'client_storage' 'key', Secret key invalid! or ",
             e,
         )
         return False
     except Exception as e:
-        data.logout(key_login)
-        Exception("Login error:", e)
-        return False
+        data.logout(key_login)()
+        raise Exception("Login error:", e)
 
 
-def decode(key_login: str, data: Datasy) -> dict[str, Any] | bool:
+def decode(key_login: str, data: Datasy) -> Dict[str, Any] | bool:
     """decodes the jwt and updates the browser sessions.
 
     ### Parameters to use:
     * `key_login` : key used to store data in the client, also used in the `login` method of `Datasy`.
     * `data` : Instance object of the `Datasy` class.
     """
     assert not data._login_async, "Use the 'decode_async' method instead of 'decode'."
-    assert data.secret_key.Jwt, "Activate the 'jwt' parameter of the 'login' method to be able to use the 'decode' method, the methods are of the class (Datasy)."
-    
-    value = data.page.run_task(_handle_decode_errors, data, key_login).result()
-    if value:
-        return value
-    else:
-        return False
+    assert data.secret_key is not None, "set the 'secret_key' in the class parameter (FletEasy)."
 
+    return data.page.run_task(_handle_decode_errors, data, key_login).result()
 
-async def decode_async(key_login: str, data: Datasy) -> dict[str, Any] | bool:
+
+async def decode_async(key_login: str, data: Datasy) -> Dict[str, Any] | bool:
     """decodes the jwt and updates the browser sessions.
 
     ### Parameters to use:
     * `key_login` : key used to store data in the client, also used in the `login` method of `Datasy`.
     * `data` : Instance object of the `Datasy` class.
     """
     assert data._login_async, "Use the 'decode' method instead of 'decode_async'."
-    assert data.secret_key.Jwt, "Activate the 'jwt' parameter of the 'login' method to be able to use the 'decode_async' method, the methods are of the class (Datasy)."
-    
-    value = await _handle_decode_errors(data, key_login)
-    if value:
-        return value
-    else:
-        return False
+    assert data.secret_key is not None, "set the 'secret_key' in the class parameter (FletEasy)."
+
+    return await _handle_decode_errors(data, key_login)
```

### Comparing `flet_easy-0.2.0.dev6/PKG-INFO` & `flet_easy-0.2.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-easy
-Version: 0.2.0.dev6
+Version: 0.2.0.dev7
 Summary: Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features.
 Keywords: flet easy flet python flet router
 Author-Email: Daxexs <Daxexsdev@gmail.com>
 License: apache-2.0
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

