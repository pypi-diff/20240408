# Comparing `tmp/chesscli-0.2.6.tar.gz` & `tmp/chesscli-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chesscli-0.2.6.tar", last modified: Mon Apr  8 03:12:51 2024, max compression
+gzip compressed data, was "chesscli-0.2.7.tar", last modified: Mon Apr  8 03:26:14 2024, max compression
```

## Comparing `chesscli-0.2.6.tar` & `chesscli-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 03:12:51.246160 chesscli-0.2.6/
--rw-rw-rw-   0        0        0     1093 2024-04-08 02:36:45.000000 chesscli-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      245 2024-04-08 03:12:51.244782 chesscli-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1944 2024-04-07 23:49:46.000000 chesscli-0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 03:12:51.246160 chesscli-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      502 2024-04-08 03:11:23.000000 chesscli-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:12:51.222037 chesscli-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 03:12:51.230076 chesscli-0.2.6/src/chesscli/
--rw-rw-rw-   0        0        0        0 2024-04-08 02:03:35.000000 chesscli-0.2.6/src/chesscli/__init__.py
--rw-rw-rw-   0        0        0       64 2024-04-08 01:53:52.000000 chesscli-0.2.6/src/chesscli/__main__.py
--rw-rw-rw-   0        0        0     3123 2024-04-08 02:34:37.000000 chesscli-0.2.6/src/chesscli/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:12:51.243779 chesscli-0.2.6/src/chesscli.egg-info/
--rw-rw-rw-   0        0        0      245 2024-04-08 03:12:51.000000 chesscli-0.2.6/src/chesscli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2024-04-08 03:12:51.000000 chesscli-0.2.6/src/chesscli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 03:12:51.000000 chesscli-0.2.6/src/chesscli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-08 03:12:51.000000 chesscli-0.2.6/src/chesscli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2024-04-08 03:12:51.000000 chesscli-0.2.6/src/chesscli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-08 03:12:51.000000 chesscli-0.2.6/src/chesscli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 03:26:14.251483 chesscli-0.2.7/
+-rw-rw-rw-   0        0        0     1093 2024-04-08 02:36:45.000000 chesscli-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      245 2024-04-08 03:26:14.250479 chesscli-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1944 2024-04-07 23:49:46.000000 chesscli-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 03:26:14.251483 chesscli-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      502 2024-04-08 03:26:10.000000 chesscli-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:26:14.221661 chesscli-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 03:26:14.228031 chesscli-0.2.7/src/chesscli/
+-rw-rw-rw-   0        0        0        0 2024-04-08 02:03:35.000000 chesscli-0.2.7/src/chesscli/__init__.py
+-rw-rw-rw-   0        0        0       64 2024-04-08 01:53:52.000000 chesscli-0.2.7/src/chesscli/__main__.py
+-rw-rw-rw-   0        0        0     3037 2024-04-08 03:24:30.000000 chesscli-0.2.7/src/chesscli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:26:14.248475 chesscli-0.2.7/src/chesscli.egg-info/
+-rw-rw-rw-   0        0        0      245 2024-04-08 03:26:14.000000 chesscli-0.2.7/src/chesscli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2024-04-08 03:26:14.000000 chesscli-0.2.7/src/chesscli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 03:26:14.000000 chesscli-0.2.7/src/chesscli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-08 03:26:14.000000 chesscli-0.2.7/src/chesscli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2024-04-08 03:26:14.000000 chesscli-0.2.7/src/chesscli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 03:26:14.000000 chesscli-0.2.7/src/chesscli.egg-info/top_level.txt
```

### Comparing `chesscli-0.2.6/LICENSE` & `chesscli-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chesscli-0.2.6/README.md` & `chesscli-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `chesscli-0.2.6/src/chesscli/main.py` & `chesscli-0.2.7/src/chesscli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,17 +42,18 @@
     subprocess.run(["docker-compose", "down"], cwd=repo_path.as_posix(), check=True)
     typer.echo("Docker containers stopped.")
     
     
 @app.command()
 def test():
     repo_path = get_repo_path_from_config()
-    subprocess.run(['pip', 'install', '-r', 'requirements.txt'], cwd=(repo_path / 'backend').as_posix(), check=True)
-    subprocess.run(['python', '-m', 'pytest', 'tests/'], cwd=(repo_path / 'backend').as_posix(), check=True)
-    typer.echo("Running Tests..")
+    try:
+        subprocess.run(['python', '-m', 'pytest', 'tests/'], cwd=(repo_path / 'backend').as_posix(), check=True)
+    except:
+        typer.echo("Some tests fail!")
     
 
 @app.command()
 def setup():
     default_repo_url = "https://github.com/neelthepatel8/chessgame"
     default_clone_folder = Path.home() / "dev/proj/chess/game"
```

