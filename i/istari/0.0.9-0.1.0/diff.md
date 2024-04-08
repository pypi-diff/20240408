# Comparing `tmp/istari-0.0.9.tar.gz` & `tmp/istari-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istari-0.0.9.tar", last modified: Sun Apr  7 03:03:34 2024, max compression
+gzip compressed data, was "istari-0.1.0.tar", last modified: Mon Apr  8 18:38:02 2024, max compression
```

## Comparing `istari-0.0.9.tar` & `istari-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 03:03:34.890713 istari-0.0.9/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-07 03:03:34.890504 istari-0.0.9/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.0.9/README.md
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 03:03:34.888258 istari-0.0.9/istari/
--rw-r--r--   0 jay        (501) staff       (20)      292 2024-04-07 03:03:12.000000 istari-0.0.9/istari/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 03:03:34.888939 istari-0.0.9/istari/auth/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.0.9/istari/auth/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     3043 2024-04-06 04:11:49.000000 istari-0.0.9/istari/auth/models.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 03:03:34.889155 istari-0.0.9/istari/cli/
--rw-r--r--   0 jay        (501) staff       (20)     2246 2024-04-07 03:00:00.000000 istari-0.0.9/istari/cli/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.0.9/istari/cli/base.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 03:03:34.889438 istari-0.0.9/istari/commands/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.0.9/istari/commands/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      967 2024-04-07 01:21:57.000000 istari-0.0.9/istari/commands/startapp.py
--rw-r--r--   0 jay        (501) staff       (20)      723 2024-04-07 01:21:42.000000 istari-0.0.9/istari/commands/startproject.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 03:03:34.889798 istari-0.0.9/istari/db/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.0.9/istari/db/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     1221 2024-04-06 00:37:44.000000 istari-0.0.9/istari/db/fields.py
--rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-06 00:40:42.000000 istari-0.0.9/istari/db/models.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 03:03:34.889980 istari-0.0.9/istari/templates/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:01:40.000000 istari-0.0.9/istari/templates/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     4262 2024-04-07 02:13:43.000000 istari-0.0.9/istari/templates/commands.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 03:03:34.890258 istari-0.0.9/istari/templates/plugins/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:22:01.000000 istari-0.0.9/istari/templates/plugins/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      611 2024-04-06 21:28:02.000000 istari-0.0.9/istari/templates/plugins/base.py
--rw-r--r--   0 jay        (501) staff       (20)     1669 2024-04-07 02:17:49.000000 istari-0.0.9/istari/templates/plugins/editable.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 03:03:34.888763 istari-0.0.9/istari.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-07 03:03:34.000000 istari-0.0.9/istari.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      593 2024-04-07 03:03:34.000000 istari-0.0.9/istari.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-07 03:03:34.000000 istari-0.0.9/istari.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-07 03:03:34.000000 istari-0.0.9/istari.egg-info/entry_points.txt
--rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-07 03:03:34.000000 istari-0.0.9/istari.egg-info/top_level.txt
--rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-07 03:03:34.890744 istari-0.0.9/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.0.9/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.391557 istari-0.1.0/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-08 18:38:02.391327 istari-0.1.0/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.1.0/README.md
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.388004 istari-0.1.0/istari/
+-rw-r--r--   0 jay        (501) staff       (20)       22 2024-04-08 18:37:31.000000 istari-0.1.0/istari/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.388888 istari-0.1.0/istari/auth/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.1.0/istari/auth/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     3043 2024-04-06 04:11:49.000000 istari-0.1.0/istari/auth/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.389316 istari-0.1.0/istari/cli/
+-rw-r--r--   0 jay        (501) staff       (20)     2246 2024-04-07 03:00:00.000000 istari-0.1.0/istari/cli/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.1.0/istari/cli/base.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.389813 istari-0.1.0/istari/commands/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.1.0/istari/commands/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     2267 2024-04-08 18:18:38.000000 istari-0.1.0/istari/commands/startapp.py
+-rw-r--r--   0 jay        (501) staff       (20)      775 2024-04-07 03:12:41.000000 istari-0.1.0/istari/commands/startproject.py
+-rw-r--r--   0 jay        (501) staff       (20)      117 2024-04-07 03:09:41.000000 istari-0.1.0/istari/constants.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.390159 istari-0.1.0/istari/db/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.1.0/istari/db/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     1221 2024-04-06 00:37:44.000000 istari-0.1.0/istari/db/fields.py
+-rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-06 00:40:42.000000 istari-0.1.0/istari/db/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.390345 istari-0.1.0/istari/templates/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:01:40.000000 istari-0.1.0/istari/templates/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     4412 2024-04-08 18:29:39.000000 istari-0.1.0/istari/templates/commands.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.390843 istari-0.1.0/istari/templates/plugins/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:22:01.000000 istari-0.1.0/istari/templates/plugins/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      578 2024-04-08 17:57:08.000000 istari-0.1.0/istari/templates/plugins/base.py
+-rw-r--r--   0 jay        (501) staff       (20)     1541 2024-04-08 18:33:07.000000 istari-0.1.0/istari/templates/plugins/defaultuser.py
+-rw-r--r--   0 jay        (501) staff       (20)     1715 2024-04-08 17:57:39.000000 istari-0.1.0/istari/templates/plugins/editable.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.391042 istari-0.1.0/istari/utils/
+-rw-r--r--   0 jay        (501) staff       (20)      298 2024-04-07 03:12:18.000000 istari-0.1.0/istari/utils/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.388698 istari-0.1.0/istari.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-08 18:38:02.000000 istari-0.1.0/istari.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      678 2024-04-08 18:38:02.000000 istari-0.1.0/istari.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-08 18:38:02.000000 istari-0.1.0/istari.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-08 18:38:02.000000 istari-0.1.0/istari.egg-info/entry_points.txt
+-rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-08 18:38:02.000000 istari-0.1.0/istari.egg-info/top_level.txt
+-rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-08 18:38:02.391591 istari-0.1.0/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.1.0/setup.py
```

### Comparing `istari-0.0.9/istari/auth/models.py` & `istari-0.1.0/istari/auth/models.py`

 * *Files identical despite different names*

### Comparing `istari-0.0.9/istari/cli/__init__.py` & `istari-0.1.0/istari/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `istari-0.0.9/istari/commands/startproject.py` & `istari-0.1.0/istari/commands/startproject.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from argparse import ArgumentParser
 
-from istari import __version__, SECRET_KEY_INSECURE_PREFIX, get_random_secret_key
+from istari import __version__
+from istari.constants import SECRET_KEY_INSECURE_PREFIX
 from istari.templates.commands import TemplateCommand
+from istari.utils import get_random_secret_key
 
 
 class Command(TemplateCommand):
     template_name = 'project_template'
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument('project_name')
```

### Comparing `istari-0.0.9/istari/db/fields.py` & `istari-0.1.0/istari/db/fields.py`

 * *Files identical despite different names*

### Comparing `istari-0.0.9/istari/db/models.py` & `istari-0.1.0/istari/db/models.py`

 * *Files identical despite different names*

### Comparing `istari-0.0.9/istari/templates/commands.py` & `istari-0.1.0/istari/templates/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from argparse import ArgumentParser
 import importlib
 import pkgutil
 from pathlib import Path
 
-from istari import BASE_DIR
+from istari.constants import BASE_DIR
 from istari.cli.base import BaseCommand
 from istari.templates.plugins.base import BasePlugin
 
 
 EXCLUDE_DIRS = ['.git', '__pycache__']
 
 EXCLUDE_EXTS = ['.pyc', '.pyo', '.pyd', '.py.class', '.DS_Store']
@@ -79,25 +79,30 @@
     def process_plugins(self, **options):
         for plugin, instance in self.plugins.items():
             flag = options.get(plugin, False)
             if flag is False:
                 if input(f'{instance.get_help()}? (yes/no) [no]: ') in ['yes', 'y']:
                     flag = True
             if flag:
-                instance.process(self.target_dir)
+                instance.process(**options)
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         self.plugins = self.load_available_plugins('istari.templates.plugins')
         for plugin, instance in self.plugins.items():
             flag = plugin.replace('_', '-')
             parser.add_argument(f'--{flag}', action='store_true', dest=plugin, help=instance.get_help())
 
     def handle(self, **options):
+        options.setdefault('ignore_plugins', False)
+        options.setdefault('target_dir', Path.cwd())
+
         self.template_dir = BASE_DIR / 'templates' / self.get_template_name()
 
-        self.target_dir = options.get('target_dir', Path.cwd())
+        self.target_dir = options.get('target_dir')
         self.variables = options.get('variables', {})
         self.exclude_dirs = options.get('exclude_dirs', EXCLUDE_DIRS)
         self.exclude_exts = options.get('exclude_exts', EXCLUDE_EXTS)
 
         self.process_template()
-        self.process_plugins(**options)
+
+        if options['ignore_plugins'] is False:
+            self.process_plugins(**options)
```

### Comparing `istari-0.0.9/istari/templates/plugins/base.py` & `istari-0.1.0/istari/templates/plugins/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from pathlib import Path
-
 class BasePlugin:
     help = None
 
     template = None
 
     def get_help(self):
         assert self.help is not None, (
@@ -13,9 +11,9 @@
 
     def get_template(self):
         assert self.template is not None, (
             f'{self.__class__.__name__} must define `.template` or implement `.get_template()`'
         )
         return self.template
 
-    def process(self, target_dir: Path):
+    def process(self, **options):
         raise NotImplementedError(f'{self.__class__.__name__} must implement `.process()`')
```

### Comparing `istari-0.0.9/istari/templates/plugins/editable.py` & `istari-0.1.0/istari/templates/plugins/editable.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from istari import BASE_DIR
+from istari.constants import BASE_DIR
 from istari.templates.plugins.base import BasePlugin
 
 
 class Plugin(BasePlugin):
     help = 'Install istari in editable mode'
 
     template = 'project'
@@ -35,15 +35,16 @@
         while not contents[fp].startswith('.PHONY'):
             fp += 1
         fp -= 1
         contents.insert(fp, f"\t{value}\n")
         with open(path, 'w') as f:
             f.writelines(contents)
 
-    def process(self, target_dir: Path):
+    def process(self, **options):
+        target_dir = options['target_dir']
         self.append_to_compose_volumes(
             f'{BASE_DIR.parent}:/usr/app/istari',
             target_dir / 'compose.yaml',
         )
         self.append_to_makefile_command(
             'up',
             'docker exec -it ${NAME}_django pip install -e /usr/app/istari',
```

### Comparing `istari-0.0.9/istari.egg-info/SOURCES.txt` & `istari-0.1.0/istari.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 istari/__init__.py
+istari/constants.py
 istari.egg-info/PKG-INFO
 istari.egg-info/SOURCES.txt
 istari.egg-info/dependency_links.txt
 istari.egg-info/entry_points.txt
 istari.egg-info/top_level.txt
 istari/auth/__init__.py
 istari/auth/models.py
@@ -16,8 +17,10 @@
 istari/db/__init__.py
 istari/db/fields.py
 istari/db/models.py
 istari/templates/__init__.py
 istari/templates/commands.py
 istari/templates/plugins/__init__.py
 istari/templates/plugins/base.py
-istari/templates/plugins/editable.py
+istari/templates/plugins/defaultuser.py
+istari/templates/plugins/editable.py
+istari/utils/__init__.py
```

