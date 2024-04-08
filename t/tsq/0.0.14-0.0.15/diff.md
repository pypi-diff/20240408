# Comparing `tmp/tsq-0.0.14.tar.gz` & `tmp/tsq-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsq-0.0.14.tar", last modified: Sat Mar 16 08:23:36 2024, max compression
+gzip compressed data, was "tsq-0.0.15.tar", last modified: Mon Apr  8 13:59:29 2024, max compression
```

## Comparing `tsq-0.0.14.tar` & `tsq-0.0.15.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-03-16 08:23:36.798607 tsq-0.0.14/
--rw-r--r--   0 ko         (501) staff       (20)     1061 2024-02-15 08:38:56.000000 tsq-0.0.14/LICENSE.md
--rw-r--r--   0 ko         (501) staff       (20)      770 2024-03-16 08:23:36.798401 tsq-0.0.14/PKG-INFO
--rw-r--r--   0 ko         (501) staff       (20)      220 2024-02-21 13:05:14.000000 tsq-0.0.14/README.md
--rw-r--r--   0 ko         (501) staff       (20)      712 2024-03-16 08:19:43.000000 tsq-0.0.14/pyproject.toml
--rw-r--r--   0 ko         (501) staff       (20)       38 2024-03-16 08:23:36.798649 tsq-0.0.14/setup.cfg
-drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-03-16 08:23:36.793036 tsq-0.0.14/taskq/
--rw-r--r--   0 ko         (501) staff       (20)        0 2024-02-15 09:23:36.000000 tsq-0.0.14/taskq/__init__.py
-drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-03-16 08:23:36.795699 tsq-0.0.14/taskq/actions/
--rw-r--r--   0 ko         (501) staff       (20)       92 2024-02-21 12:49:38.000000 tsq-0.0.14/taskq/actions/__init__.py
--rw-r--r--   0 ko         (501) staff       (20)     4885 2024-03-16 08:13:38.000000 tsq-0.0.14/taskq/actions/add.py
--rw-r--r--   0 ko         (501) staff       (20)     1522 2024-03-16 08:13:56.000000 tsq-0.0.14/taskq/actions/backend.py
--rw-r--r--   0 ko         (501) staff       (20)     2184 2024-02-21 12:48:15.000000 tsq-0.0.14/taskq/actions/base.py
--rw-r--r--   0 ko         (501) staff       (20)     1718 2024-02-21 18:53:59.000000 tsq-0.0.14/taskq/actions/config.py
--rw-r--r--   0 ko         (501) staff       (20)     2556 2024-02-21 12:59:28.000000 tsq-0.0.14/taskq/actions/filter.py
--rw-r--r--   0 ko         (501) staff       (20)    11868 2024-03-16 08:14:20.000000 tsq-0.0.14/taskq/actions/read.py
--rw-r--r--   0 ko         (501) staff       (20)     3067 2024-03-16 08:14:50.000000 tsq-0.0.14/taskq/actions/write.py
-drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-03-16 08:23:36.797109 tsq-0.0.14/taskq/backends/
--rw-r--r--   0 ko         (501) staff       (20)       76 2024-02-21 12:49:57.000000 tsq-0.0.14/taskq/backends/__init__.py
--rw-r--r--   0 ko         (501) staff       (20)     1446 2024-02-21 12:44:07.000000 tsq-0.0.14/taskq/backends/base.py
--rw-r--r--   0 ko         (501) staff       (20)      807 2024-02-21 12:38:43.000000 tsq-0.0.14/taskq/backends/dummy.py
--rw-r--r--   0 ko         (501) staff       (20)     6653 2024-03-16 08:15:26.000000 tsq-0.0.14/taskq/backends/ts.py
--rw-r--r--   0 ko         (501) staff       (20)     3659 2024-02-21 18:48:56.000000 tsq-0.0.14/taskq/cli.py
--rw-r--r--   0 ko         (501) staff       (20)     1561 2024-02-21 12:17:48.000000 tsq-0.0.14/taskq/common.py
--rw-r--r--   0 ko         (501) staff       (20)      770 2024-02-15 15:26:07.000000 tsq-0.0.14/taskq/utils.py
-drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-03-16 08:23:36.798197 tsq-0.0.14/tsq.egg-info/
--rw-r--r--   0 ko         (501) staff       (20)      770 2024-03-16 08:23:36.000000 tsq-0.0.14/tsq.egg-info/PKG-INFO
--rw-r--r--   0 ko         (501) staff       (20)      543 2024-03-16 08:23:36.000000 tsq-0.0.14/tsq.egg-info/SOURCES.txt
--rw-r--r--   0 ko         (501) staff       (20)        1 2024-03-16 08:23:36.000000 tsq-0.0.14/tsq.egg-info/dependency_links.txt
--rw-r--r--   0 ko         (501) staff       (20)       38 2024-03-16 08:23:36.000000 tsq-0.0.14/tsq.egg-info/entry_points.txt
--rw-r--r--   0 ko         (501) staff       (20)       45 2024-03-16 08:23:36.000000 tsq-0.0.14/tsq.egg-info/requires.txt
--rw-r--r--   0 ko         (501) staff       (20)        6 2024-03-16 08:23:36.000000 tsq-0.0.14/tsq.egg-info/top_level.txt
+drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-08 13:59:29.049893 tsq-0.0.15/
+-rw-r--r--   0 ko         (501) staff       (20)     1061 2024-02-15 08:38:56.000000 tsq-0.0.15/LICENSE.md
+-rw-r--r--   0 ko         (501) staff       (20)      770 2024-04-08 13:59:29.049659 tsq-0.0.15/PKG-INFO
+-rw-r--r--   0 ko         (501) staff       (20)      220 2024-02-21 13:05:14.000000 tsq-0.0.15/README.md
+-rw-r--r--   0 ko         (501) staff       (20)      781 2024-04-08 13:59:23.000000 tsq-0.0.15/pyproject.toml
+-rw-r--r--   0 ko         (501) staff       (20)       38 2024-04-08 13:59:29.049934 tsq-0.0.15/setup.cfg
+drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-08 13:59:29.046458 tsq-0.0.15/taskq/
+-rw-r--r--   0 ko         (501) staff       (20)       23 2024-03-27 07:03:11.000000 tsq-0.0.15/taskq/__init__.py
+drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-08 13:59:29.047582 tsq-0.0.15/taskq/actions/
+-rw-r--r--   0 ko         (501) staff       (20)       92 2024-02-21 12:49:38.000000 tsq-0.0.15/taskq/actions/__init__.py
+-rw-r--r--   0 ko         (501) staff       (20)     5141 2024-04-08 13:58:20.000000 tsq-0.0.15/taskq/actions/add.py
+-rw-r--r--   0 ko         (501) staff       (20)     1522 2024-03-16 08:13:56.000000 tsq-0.0.15/taskq/actions/backend.py
+-rw-r--r--   0 ko         (501) staff       (20)     2356 2024-03-27 06:54:37.000000 tsq-0.0.15/taskq/actions/base.py
+-rw-r--r--   0 ko         (501) staff       (20)     1800 2024-03-25 17:22:30.000000 tsq-0.0.15/taskq/actions/config.py
+-rw-r--r--   0 ko         (501) staff       (20)     2556 2024-02-21 12:59:28.000000 tsq-0.0.15/taskq/actions/filter.py
+-rw-r--r--   0 ko         (501) staff       (20)    11868 2024-03-26 09:21:45.000000 tsq-0.0.15/taskq/actions/read.py
+-rw-r--r--   0 ko         (501) staff       (20)     3067 2024-03-16 08:14:50.000000 tsq-0.0.15/taskq/actions/write.py
+drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-08 13:59:29.048280 tsq-0.0.15/taskq/backends/
+-rw-r--r--   0 ko         (501) staff       (20)      106 2024-03-27 18:02:23.000000 tsq-0.0.15/taskq/backends/__init__.py
+-rw-r--r--   0 ko         (501) staff       (20)     2671 2024-03-27 17:15:39.000000 tsq-0.0.15/taskq/backends/base.py
+-rw-r--r--   0 ko         (501) staff       (20)     1087 2024-03-27 17:19:10.000000 tsq-0.0.15/taskq/backends/dummy.py
+-rw-r--r--   0 ko         (501) staff       (20)     5690 2024-03-28 19:49:01.000000 tsq-0.0.15/taskq/backends/ts.py
+-rw-r--r--   0 ko         (501) staff       (20)     3928 2024-03-27 18:07:00.000000 tsq-0.0.15/taskq/cli.py
+-rw-r--r--   0 ko         (501) staff       (20)     1561 2024-02-21 12:17:48.000000 tsq-0.0.15/taskq/common.py
+-rw-r--r--   0 ko         (501) staff       (20)      770 2024-02-15 15:26:07.000000 tsq-0.0.15/taskq/utils.py
+drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-08 13:59:29.049297 tsq-0.0.15/tsq.egg-info/
+-rw-r--r--   0 ko         (501) staff       (20)      770 2024-04-08 13:59:29.000000 tsq-0.0.15/tsq.egg-info/PKG-INFO
+-rw-r--r--   0 ko         (501) staff       (20)      543 2024-04-08 13:59:29.000000 tsq-0.0.15/tsq.egg-info/SOURCES.txt
+-rw-r--r--   0 ko         (501) staff       (20)        1 2024-04-08 13:59:29.000000 tsq-0.0.15/tsq.egg-info/dependency_links.txt
+-rw-r--r--   0 ko         (501) staff       (20)       38 2024-04-08 13:59:29.000000 tsq-0.0.15/tsq.egg-info/entry_points.txt
+-rw-r--r--   0 ko         (501) staff       (20)       45 2024-04-08 13:59:29.000000 tsq-0.0.15/tsq.egg-info/requires.txt
+-rw-r--r--   0 ko         (501) staff       (20)        6 2024-04-08 13:59:29.000000 tsq-0.0.15/tsq.egg-info/top_level.txt
```

### Comparing `tsq-0.0.14/LICENSE.md` & `tsq-0.0.15/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tsq-0.0.14/PKG-INFO` & `tsq-0.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsq
-Version: 0.0.14
+Version: 0.0.15
 Summary: A Friendly Task Scheduler Frontend
 Author: admk
 Project-URL: Homepage, https://github.com/admk/tu
 Project-URL: Issues, https://github.com/admk/tu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tsq-0.0.14/pyproject.toml` & `tsq-0.0.15/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tsq"
-version = "0.0.14"
 authors = [
   { name="admk" },
 ]
 description = "A Friendly Task Scheduler Frontend"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -18,17 +17,21 @@
     "blessed >= 1.20.0",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dynamic = ["version"]
 
 [project.scripts]
 tq = "taskq.cli:main"
 
 [project.urls]
 Homepage = "https://github.com/admk/tu"
 Issues = "https://github.com/admk/tu/issues"
 
 [tool.setuptools.packages.find]
 include = ["taskq", "taskq.*"]
+
+[tool.setuptools.dynamic]
+version = {attr = "taskq.__version__"}
```

### Comparing `tsq-0.0.14/taskq/actions/add.py` & `tsq-0.0.15/taskq/actions/add.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,25 +20,30 @@
             'type': int,
             'default': None,
             'help': 'Number of slots required.',
         },
         ('-u', '--unique'): {
             'action': 'store_true',
             'help':
-                'Only add unique commands.'
+                'Only add unique commands. '
                 'If a command is already in the queue, '
                 'it will also be skipped.',
         },
         ('-f', '--from-file'): {
             'type': str,
             'default': None,
             'help':
                 'Read commands from a file, one per line. '
                 'If "-", read from standard input.',
         },
+        ('-s', '--separator'): {
+            'type': str,
+            'default': ',',
+            'help': 'Separator for arguments from standard input.',
+        },
         ('command', ): {
             'type': str,
             'nargs': argparse.REMAINDER,
             'help': 'The command to run.',
         },
     }
 
@@ -80,15 +85,15 @@
 
     @classmethod
     def _extrapolate_sets(cls, commands):
         return cls._regex_extrapolate(
             commands, r'\{([^}]+)\}', lambda s: s.split(','))
 
     @staticmethod
-    def _extrapolate_inputs(command, from_file):
+    def _extrapolate_inputs(command, from_file, sep=','):
         if not STDIN_TTY:
             inputs = sys.stdin.read().split('\n')
         else:
             inputs = []
         if from_file == '-':
             commands = inputs
         elif from_file:
@@ -106,25 +111,27 @@
             # nothing in stdin, so we can't extrapolate arguments
             return commands
         new_commands = []
         for line in inputs:
             line = line.strip()
             if not line:
                 continue
-            args = line.split(',')
+            args = line.split(sep)
             for c in commands:
                 for j, a in enumerate(args):
-                    c = c.replace(f'@{j + 1}', a)
+                    c = c.replace(f'@{j + 1}', a.strip())
                 new_commands.append(c)
-        return [c for c in new_commands if c]
+        return new_commands
 
     def main(self, args):
-        commands = self._extrapolate_inputs(args.command, args.from_file)
+        commands = self._extrapolate_inputs(
+            args.command, args.from_file, args.separator)
         commands = self._extrapolate_ranges(commands)
         commands = self._extrapolate_sets(commands)
+        commands = [c.strip() for c in commands if c.strip()]
         if args.unique:
             info = self.backend.full_info(None, FilterArgs())
             queued_commands = [i['command'] for i in info]
             commands = list(dict.fromkeys(commands))
             skipped = [c for c in commands if c in queued_commands]
             commands = [c for c in commands if c not in queued_commands]
             if skipped:
```

### Comparing `tsq-0.0.14/taskq/actions/backend.py` & `tsq-0.0.15/taskq/actions/backend.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.14/taskq/actions/base.py` & `tsq-0.0.15/taskq/actions/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod
 from typing import Mapping, Type
 
-from ..backends import BACKENDS
+from ..backends import BACKENDS, BackendNotFoundError
 
 
 class ActionBase:
     def __init__(self, name, parser_kwargs):
         super().__init__()
         self.options = {}
         self.name = name
@@ -22,15 +22,19 @@
         args = self.transform_args(args)
         backend = config['backend']
         try:
             backend_cls = BACKENDS[backend]
         except KeyError:
             print(f'Invalid backend: {backend}')
             backend_cls = BACKENDS['dummy']
-        self.backend = backend_cls(backend, config)
+        try:
+            self.backend = backend_cls(backend, config)
+        except BackendNotFoundError as e:
+            print(f'Backend {backend!r} not available, reason: {e}.')
+            return 1
         return self.main(args)
 
 
 class DryActionBase(ActionBase):
     dry_options = {
         ('-d', '--dry-run'): {
             'action': 'store_true',
```

### Comparing `tsq-0.0.14/taskq/actions/config.py` & `tsq-0.0.15/taskq/actions/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,12 +43,15 @@
         config = dict_simplify(copy.deepcopy(self.backend.config))
         if args.key is None:
             print(tomlkit.dumps(config).rstrip())
             return
         if args.value is None:
             print(self.getset(config, args.key))
             return
-        with open(args.rc_file, 'r', encoding='utf-8') as f:
-            rc_config = tomlkit.load(f)
+        try:
+            with open(args.rc_file, 'r', encoding='utf-8') as f:
+                rc_config = tomlkit.load(f)
+        except FileNotFoundError:
+            rc_config = {}
         self.getset(rc_config, args.key, args.value)
         with open(args.rc_file, 'w', encoding='utf-8') as f:
             f.write(tomlkit.dumps(rc_config))
```

### Comparing `tsq-0.0.14/taskq/actions/filter.py` & `tsq-0.0.15/taskq/actions/filter.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.14/taskq/actions/read.py` & `tsq-0.0.15/taskq/actions/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
         elif args.export_format == 'toml':
             import toml
             return toml.dumps({'job': info})
         else:
             raise ValueError(f'Unknown format: {args.export_format}')
 
 
-@register_action('outputs', 'Show job outputs', aliases=['out'])
+@register_action('outputs', 'show job outputs', aliases=['out'])
 class OutputsAction(ReadActionBase):
     outputs_options = {
         ('-i', '--interactive'): {
             'action': 'store_true',
             'help': 'Follow the output.',
         },
         ('-t', '--tail'): {
@@ -316,15 +316,15 @@
         try:
             self.backend.output(info[0], args.tail, shell=True)
         except KeyboardInterrupt:
             pass
         return 0
 
 
-@register_action('wait', 'Wait for jobs to finish', aliases=['w'])
+@register_action('wait', 'wait for jobs to finish', aliases=['w'])
 class WaitAction(ReadActionBase):
     wait_options = {
         ('-p', '--progress'): {
             'action': 'store_true',
             'help': 'Show progress bar.',
         },
     }
```

### Comparing `tsq-0.0.14/taskq/actions/write.py` & `tsq-0.0.15/taskq/actions/write.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.14/taskq/backends/dummy.py` & `tsq-0.0.15/taskq/backends/dummy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 from .base import register_backend, BackendBase
 
 
 @register_backend('dummy')
 class DummyBackend(BackendBase):
+    def __init__(self, name, config):
+        config['command'] = None
+        super().__init__(name, config)
+
     def backend_info(self):
         return {
             'name': 'dummy',
-            'command': None,
+            'command': '',
             'version': '0.0.0',
         }
 
     def backend_kill(self, args):
-        pass
+        print(args)
 
     def backend_command(self, command, commit=True):
-        return command
+        return command, commit
 
     def job_info(self, ids=None, filters=None):
+        print(ids, filters)
         return []
 
     def full_info(
         self, ids=None, filters=None, extra_func=None, tqdm_disable=False
     ):
+        print(ids, filters)
         return []
 
     def output(self, info, tail, shell=False):
-        pass
+        print(info, tail, shell)
 
     def add(self, command, gpus, slots, commit=True):
+        print(repr(command), gpus, slots, commit)
         return 0
 
     def kill(self, info, commit=True):
-        pass
+        print(info, commit)
 
     def remove(self, info, commit=True):
-        pass
+        print(info, commit)
```

### Comparing `tsq-0.0.14/taskq/backends/ts.py` & `tsq-0.0.15/taskq/backends/ts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,80 +1,54 @@
-import os
 import re
 import shlex
 import datetime
-import subprocess
 
 from ..common import tqdm, STATUSES, file_tail_lines, tail_lines, dict_simplify
 from .base import register_backend, BackendBase
 
 
 @register_backend('ts')
 class TaskSpoolerBackend(BackendBase):
     def __init__(self, name, config):
         super().__init__(name, config)
-        group = self.config.get('group', 'default')
+        socket = self.config.get('socket', 'default')
         slots = self.config.get('slots')
-        if slots == 'auto':
-            try:
-                nv = subprocess.check_output(['nvidia-smi', '-L'])
-                slots = len(nv.splitlines())
-            except (FileNotFoundError, subprocess.CalledProcessError):
-                slots = 1
         self.env.setdefault('TS_SLOTS', str(slots))
-        self.env.setdefault('TS_SOCKET', f'/tmp/ts-{group}.sock')
+        self.env.setdefault('TS_SOCKET', f'/tmp/ts-{socket}.sock')
         self.env = dict_simplify(self.env, not_value=True)
-        self._ts_command = self.config.get('command', 'ts')
-
-    def _ts(self, *args, commit=True, shell=False, check=True):
-        cmd = [self._ts_command] + [str(a) for a in args]
-        if not commit:
-            print(' '.join(cmd))
-            return None
-        env = dict(os.environ, **self.env)
-        if shell:
-            subprocess.run(' '.join(cmd), shell=True, env=env, check=check)
-            return None
-        p = subprocess.run(
-            cmd, capture_output=True, env=env, check=check)
-        out = p.stdout.decode('utf-8').strip()
-        out += p.stderr.decode('utf-8').strip()
-        return out
+        self.backend_getset('slots', slots)
 
     def backend_getset(self, key, value=None):
         slot_keys = [
             'slots',
             f'backends.{self.name}.slots',
             f'groups.{self.config["group"]}.slots'
         ]
         if key in slot_keys:
             if value is None:
-                return int(self._ts('-S') or -1)
-            return self._ts('-S', value)
+                return int(self.exec('-S') or -1)
+            return self.exec('-S', value)
 
     def backend_info(self):
         info = {
             'name': 'Task Spooler',
-            'command': self._ts_command,
+            'command': self._command,
         }
-        version = self._ts('-V') or ''
+        version = self.exec('-V') or ''
         result = re.search(r'(v[\.\d]+)', version)
         if result:
             info['version'] = result.group(1)
         return info
 
     def backend_kill(self, args):
-        self._ts('-K')
-
-    def backend_command(self, command, commit=True):
-        return self._ts(*command, commit=True, check=False)
+        self.exec('-K')
 
     def job_info(self, ids=None, filters=None):
         info = []
-        tsout = self._ts()
+        tsout = self.exec()
         if not tsout:
             return info
         for l in tsout.splitlines()[1:]:
             l = l.strip().split()
             if l[1] == 'finished':
                 job_id, status, _, exitcode, *_ = l
                 exitcode = int(exitcode)
@@ -118,68 +92,68 @@
         return datetime.datetime.strptime(time, '%a %b %d %H:%M:%S %Y')
 
     def full_info(
         self, ids=None, filters=None, extra_func=None, tqdm_disable=False
     ):
         info = self.job_info(ids, filters)
         for i in tqdm(info, disable=tqdm_disable, desc='info'):
-            ji = self._ts('-i', i['id'])
+            ji = self.exec('-i', i['id'])
             start_time = self.get_time(ji, 'Start time: ')
             end_time = self.get_time(ji, 'End time: ')
             if not start_time:
                 delta = None
             elif not end_time:
                 delta = datetime.datetime.now() - start_time
             else:
                 delta = end_time - start_time
             try:
-                pid = int(self._ts('-p', i['id'], check=False) or -1)
+                pid = int(self.exec('-p', i['id'], check=False) or -1)
             except ValueError:
                 pid = None
             new_info = {
                 'command': self.get_line(ji, 'Command: '),
                 'slots_required':
                     int(self.get_line(ji, 'Slots required: ') or 1),
                 'gpus_required':
                     int(self.get_line(ji, 'GPUs required: ') or 0),
                 'gpu_ids': self.get_line(ji, 'GPU IDs: '),
                 'enqueue_time': self.get_time(ji, 'Enqueue time: '),
                 'start_time': start_time,
                 'end_time': end_time,
                 'time_run': delta,
-                'output_file': self._ts('-o', i['id'], check=False),
+                'output_file': self.exec('-o', i['id'], check=False),
                 'pid': pid,
             }
             i.update({k: v for k, v in new_info.items() if v is not None})
             if extra_func:
                 extra_func(i)
         return info
 
     def output(self, info, tail, shell=False):
         if shell:
-            self._ts('-c', info['id'], check=False, shell=True)
+            self.exec('-c', info['id'], check=False, shell=True)
             return ''
         if info['status'] in ['success', 'failed', 'killed']:
-            return tail_lines(self._ts('-c', info['id'], check=False), tail)
-        f = info.get('output_file') or self._ts('-o', info['id'], check=False)
+            return tail_lines(self.exec('-c', info['id'], check=False), tail)
+        f = info.get('output_file') or self.exec('-o', info['id'], check=False)
         return file_tail_lines(f, tail) if f else ''
 
     def add(self, command, gpus=None, slots=None, commit=True):
         torun = []
         alloc_config = self.config.get('alloc', {})
         gpus = gpus if gpus is not None else alloc_config.get('gpus', 1)
         slots = slots if slots is not None else alloc_config.get('slots', 1)
         if gpus > 0:
             torun += ['-G', gpus]
         torun += ['-N', slots]
         command = command.replace('\n', '\\n')
         torun += shlex.split(command)
-        return self._ts(*torun, commit=commit)
+        return self.exec(*torun, commit=commit)
 
     def kill(self, info, commit=True):
-        self._ts('-k', info['id'], commit=commit)
+        self.exec('-k', info['id'], commit=commit)
 
     def remove(self, info, commit=True):
         if info['status'] == 'running':
             self.kill(info, commit=commit)
-            self._ts('-w', info['id'], commit=commit, check=False)
-        return self._ts('-r', info['id'], commit=commit)
+            self.exec('-w', info['id'], commit=commit, check=False)
+        return self.exec('-r', info['id'], commit=commit)
```

### Comparing `tsq-0.0.14/taskq/cli.py` & `tsq-0.0.15/taskq/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import os
 import sys
 import argparse
 
 import tomlkit
 
+from . import __version__
 from .common import dict_merge
 from .actions import INFO
 from .backends import BACKENDS
 
 
 class CLI:
     base_options = {
+        ('-V', '--version'): {
+            'action': 'store_true',
+            'help': 'print the version and exit',
+        },
         ('-rc', '--rc-file'): {
             'type': str,
             'default': None,
             'help':
                 'The configuration file to use. '
                 'If not provided, it reads from "~/.config/tq.toml" '
                 'and "./.tq.toml".'
@@ -89,14 +94,17 @@
 
     def main(self, args=None):
         args = args or sys.argv[1:]
         if all(a not in INFO['aliases'] for a in args):
             if '-h' in args or '--help' in args:
                 self.parser.print_help()
                 sys.exit(0)
+            if '-V' in args or '--version' in args:
+                print(__version__)
+                sys.exit(0)
             args = [INFO['default']] + args
         args = self.parser.parse_args(args)
         config = self._load_config(args)
         config = self._resolve_config(args, config)
         try:
             action = INFO['aliases'][args.action]
             action_func = INFO['actions'][action]
```

### Comparing `tsq-0.0.14/taskq/common.py` & `tsq-0.0.15/taskq/common.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.14/taskq/utils.py` & `tsq-0.0.15/taskq/utils.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.14/tsq.egg-info/PKG-INFO` & `tsq-0.0.15/tsq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsq
-Version: 0.0.14
+Version: 0.0.15
 Summary: A Friendly Task Scheduler Frontend
 Author: admk
 Project-URL: Homepage, https://github.com/admk/tu
 Project-URL: Issues, https://github.com/admk/tu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tsq-0.0.14/tsq.egg-info/SOURCES.txt` & `tsq-0.0.15/tsq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

