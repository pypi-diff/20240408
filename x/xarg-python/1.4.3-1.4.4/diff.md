# Comparing `tmp/xarg-python-1.4.3.tar.gz` & `tmp/xarg-python-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarg-python-1.4.3.tar", last modified: Sun Apr  7 18:23:28 2024, max compression
+gzip compressed data, was "xarg-python-1.4.4.tar", last modified: Mon Apr  8 16:20:14 2024, max compression
```

## Comparing `xarg-python-1.4.3.tar` & `xarg-python-1.4.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 18:23:28.192449 xarg-python-1.4.3/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-08-28 15:46:08.000000 xarg-python-1.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1320 2024-04-07 18:23:28.192449 xarg-python-1.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      656 2023-11-23 15:08:18.000000 xarg-python-1.4.3/README.md
--rw-r--r--   0 root         (0) root         (0)      579 2024-04-07 18:23:28.192449 xarg-python-1.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      779 2024-03-31 14:51:50.000000 xarg-python-1.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 18:23:28.182449 xarg-python-1.4.3/xarg/
--rw-r--r--   0 root         (0) root         (0)      490 2024-04-06 10:39:58.000000 xarg-python-1.4.3/xarg/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22718 2024-04-07 18:19:56.000000 xarg-python-1.4.3/xarg/actuator.py
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-07 18:22:33.000000 xarg-python-1.4.3/xarg/attribute.py
--rw-r--r--   0 root         (0) root         (0)     9216 2024-04-06 18:33:10.000000 xarg-python-1.4.3/xarg/colorful.py
--rw-r--r--   0 root         (0) root         (0)     8184 2024-03-31 14:53:08.000000 xarg-python-1.4.3/xarg/complete.py
--rw-r--r--   0 root         (0) root         (0)     3218 2024-04-07 18:03:05.000000 xarg-python-1.4.3/xarg/logger.py
--rw-r--r--   0 root         (0) root         (0)     8479 2024-03-31 14:51:50.000000 xarg-python-1.4.3/xarg/parser.py
--rw-r--r--   0 root         (0) root         (0)     2216 2024-03-31 14:25:54.000000 xarg-python-1.4.3/xarg/safefile.py
--rw-r--r--   0 root         (0) root         (0)     8482 2024-03-31 14:49:33.000000 xarg-python-1.4.3/xarg/scanner.py
--rw-r--r--   0 root         (0) root         (0)     1236 2024-03-31 15:00:43.000000 xarg-python-1.4.3/xarg/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 18:23:28.192449 xarg-python-1.4.3/xarg_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1320 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:20:14.108264 xarg-python-1.4.4/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-08-28 15:46:08.000000 xarg-python-1.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-04-08 16:20:14.108264 xarg-python-1.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      656 2023-11-23 15:08:18.000000 xarg-python-1.4.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      579 2024-04-08 16:20:14.108264 xarg-python-1.4.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      779 2024-03-31 14:51:50.000000 xarg-python-1.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:20:14.098264 xarg-python-1.4.4/xarg/
+-rw-r--r--   0 root         (0) root         (0)      490 2024-04-06 10:39:58.000000 xarg-python-1.4.4/xarg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22139 2024-04-08 16:13:46.000000 xarg-python-1.4.4/xarg/actuator.py
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-08 16:17:56.000000 xarg-python-1.4.4/xarg/attribute.py
+-rw-r--r--   0 root         (0) root         (0)     9216 2024-04-06 18:33:10.000000 xarg-python-1.4.4/xarg/colorful.py
+-rw-r--r--   0 root         (0) root         (0)     8184 2024-03-31 14:53:08.000000 xarg-python-1.4.4/xarg/complete.py
+-rw-r--r--   0 root         (0) root         (0)     4211 2024-04-08 16:15:15.000000 xarg-python-1.4.4/xarg/logger.py
+-rw-r--r--   0 root         (0) root         (0)     8479 2024-03-31 14:51:50.000000 xarg-python-1.4.4/xarg/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-03-31 14:25:54.000000 xarg-python-1.4.4/xarg/safefile.py
+-rw-r--r--   0 root         (0) root         (0)     8482 2024-03-31 14:49:33.000000 xarg-python-1.4.4/xarg/scanner.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2024-03-31 15:00:43.000000 xarg-python-1.4.4/xarg/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:20:14.108264 xarg-python-1.4.4/xarg_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/zip-safe
```

### Comparing `xarg-python-1.4.3/LICENSE` & `xarg-python-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.3/PKG-INFO` & `xarg-python-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarg-python
-Version: 1.4.3
+Version: 1.4.4
 Summary: Simple command-line tool based on argparse.
 Home-page: https://github.com/bondbox/xarg-python/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/bondbox/xarg-python/
 Project-URL: Bug Tracker, https://github.com/bondbox/xarg-python/issues
```

### Comparing `xarg-python-1.4.3/README.md` & `xarg-python-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.3/setup.cfg` & `xarg-python-1.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.3/setup.py` & `xarg-python-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.3/xarg/actuator.py` & `xarg-python-1.4.4/xarg/actuator.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 from errno import ENOENT
 import logging
 from logging import Logger
 import sys
 from typing import Any
 from typing import Callable
 from typing import Dict
-from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 
 from .attribute import __prog_name__
 from .logger import log
-from .logger import once_filter as log_once_filter
 from .parser import argp
 from .util import singleton
 
 
 class add_command:
     '''Define a new command-line node.
 
@@ -281,27 +279,27 @@
 
     @property
     def main(self) -> run_command:
         return self.__main
 
 
 @singleton
-class commands:
+class commands(log):
     '''Singleton command-line tool based on argparse.
 
     Define and bind all callback functions before calling run() or parse().
 
     For example:
 
     >>> from typing import Optional\n
     >>> from typing import Sequence\n
 
     >>> from xarg import add_command\n
     >>> from xarg import argp\n
-    >>> from xarg import cmds\n
+    >>> from xarg import commands\n
     >>> from xarg import end_command\n
     >>> from xarg import pre_command\n
     >>> from xarg import run_command\n
 
     >>> @add_command("example")\n
     >>> def cmd(_arg: argp):\n
     >>>     argp.add_opt_on("-t", "--test")\n
@@ -315,29 +313,30 @@
     >>>     return 0\n
 
     >>> @end_command(run)\n
     >>> def end(cmds: commands) -> int:\n
     >>>     return 0\n
 
     >>> def main(argv: Optional[Sequence[str]] = None) -> int:\n
-    >>>     return cmds.run(\n
+    >>>     return commands().run(\n
     >>>         root=cmd,\n
     >>>         argv=argv,\n
     >>>         prog="xarg-example",\n
     >>>         description="Simple command-line tool based on argparse.")\n
     '''
 
     LOGGER_ARGUMENT_GROUP = "logger options"
 
     def __init__(self):
         self.__prog: str = __prog_name__
         self.__root: Optional[add_command] = None
         self.__args: Namespace = Namespace()
         self.__version: Optional[str] = None
-        self.__logging: log = log(True)
+        self.__enabled_logger: bool = True
+        super().__init__()
 
     @property
     def prog(self) -> str:
         return self.__prog
 
     @property
     def root(self) -> Optional[add_command]:
@@ -370,44 +369,28 @@
 
     @version.setter
     def version(self, value: str):
         assert isinstance(value, str)
         _version = value.strip()
         self.__version = _version
 
-    def initiate_logging(self, level: Optional[str] = None,
-                         handlers: Optional[Iterable[logging.Handler]] = None,
-                         filters: Optional[Iterable[logging.Filter]] = None):
-        assert self.logging.enabled is True
-        logger: logging.Logger = self.logger
-
-        if isinstance(level, str):
-            logger.setLevel(logging._nameToLevel[level.upper()])
-
-        if filters is None:
-            filters = [log_once_filter()]
-
-        for filter in filters:
-            logger.addFilter(filter)
-
-        if handlers is None:
-            handlers = [self.logging.new_stream_handler(stream=sys.stdout)]
-
-        for handler in handlers:
-            logger.addHandler(handler)
-
     @property
-    def logging(self) -> log:
-        return self.__logging
+    def enabled_logger(self) -> bool:
+        return self.__enabled_logger
+
+    @enabled_logger.setter
+    def enabled_logger(self, value: bool):
+        assert isinstance(value, bool)
+        self.__enabled_logger = value
 
     @property
     def logger(self) -> Logger:
         '''Logger.
         '''
-        return self.logging.get_logger(self.prog)
+        return self.get_logger(self.prog)
 
     def stdout(self, context: Any):
         '''Output string to sys.stdout.
         '''
         sys.stdout.write(f"{context}\n")
         sys.stdout.flush()
 
@@ -443,21 +426,21 @@
 
             option_level = filter_optional_name("--level", "--log-level")
             if isinstance(option_level, str):
                 group_level.add_argument(
                     option_level,
                     type=str,
                     nargs="?",
-                    const="info",
-                    default="info",
-                    choices=self.logging.ALLOWED_LOG_LEVELS,
+                    const=self.LOG_LEVEL_INFO.lower(),
+                    default=self.LOG_LEVEL_INFO.lower(),
+                    choices=self.ALLOWED_LOG_LEVELS,
                     dest="_log_level_str_",
                     help="Logger output level, default info.")
 
-            for level in self.logging.ALLOWED_LOG_LEVELS:
+            for level in self.ALLOWED_LOG_LEVELS:
                 options = []
                 if isinstance(filter_optional_name(f"-{level[0]}"), str):
                     options.append(f"-{level[0]}")
                 if isinstance(filter_optional_name(f"--{level}"), str):
                     options.append(f"--{level}")
                 elif isinstance(filter_optional_name(f"--{level}-level"), str):
                     options.append(f"--{level}-level")
@@ -496,15 +479,15 @@
                 " %(message)s"
 
             group = argp.argument_group(self.LOGGER_ARGUMENT_GROUP)
             group.add_argument(option,
                                type=str,
                                nargs="?",
                                const=DEFAULT_LOG_FMT,
-                               default=self.logging.DEFAULT_LOG_FORMAT,
+                               default=self.DEFAULT_LOG_FORMAT,
                                metavar="STRING",
                                dest="_log_format_",
                                help="Logger output format.")
 
         def add_optional_console():
             group = argp.argument_group(self.LOGGER_ARGUMENT_GROUP)
             group_std = group.add_mutually_exclusive_group()
@@ -521,22 +504,22 @@
             if isinstance(option, str):
                 group_std.add_argument(option,
                                        const=sys.stderr,
                                        action="store_const",
                                        dest="_log_console_",
                                        help="Logger output to stderr.")
 
-        if self.logging.enabled:
+        if self.enabled_logger:
             add_optional_level()
             add_optional_stream()
             add_optional_format()
             add_optional_console()
 
     def __parse_logger(self, args: Namespace):
-        if not self.logging.enabled:
+        if not self.enabled_logger:
             return
 
         level_name: Optional[str] = args._log_level_str_.upper() if hasattr(
             args, "_log_level_str_") and isinstance(
             args._log_level_str_, str) else None
         fmt: Optional[str] = args._log_format_ if hasattr(
             args, "_log_format_") and isinstance(
@@ -546,16 +529,15 @@
         if hasattr(args, "_log_console_") and args._log_console_ is not None:
             handlers.append(
                 log.new_stream_handler(stream=args._log_console_, fmt=fmt))
         if hasattr(args, "_log_files_"):
             for filename in args._log_files_:
                 handlers.append(
                     log.new_file_handler(filename=filename, fmt=fmt))
-
-        self.initiate_logging(level=level_name, handlers=handlers)
+        self.initiate_logger(self.logger, level=level_name, handlers=handlers)
 
     def __add_parser(self, _map: Dict[add_command, argp],
                      arg_root: argp, cmd_root: add_command, **kwargs):
         assert isinstance(cmd_root, add_command)
         assert cmd_root not in _map
         _map[cmd_root] = arg_root
```

### Comparing `xarg-python-1.4.3/xarg/colorful.py` & `xarg-python-1.4.4/xarg/colorful.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.3/xarg/complete.py` & `xarg-python-1.4.4/xarg/complete.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.3/xarg/parser.py` & `xarg-python-1.4.4/xarg/parser.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.3/xarg/safefile.py` & `xarg-python-1.4.4/xarg/safefile.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.3/xarg/scanner.py` & `xarg-python-1.4.4/xarg/scanner.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.3/xarg/util.py` & `xarg-python-1.4.4/xarg/util.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.3/xarg_python.egg-info/PKG-INFO` & `xarg-python-1.4.4/xarg_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarg-python
-Version: 1.4.3
+Version: 1.4.4
 Summary: Simple command-line tool based on argparse.
 Home-page: https://github.com/bondbox/xarg-python/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/bondbox/xarg-python/
 Project-URL: Bug Tracker, https://github.com/bondbox/xarg-python/issues
```

