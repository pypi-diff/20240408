# Comparing `tmp/atom-tools-0.5.2.tar.gz` & `tmp/atom-tools-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atom-tools-0.5.2.tar", last modified: Thu Apr  4 14:03:28 2024, max compression
+gzip compressed data, was "atom-tools-0.5.3.tar", last modified: Mon Apr  8 16:50:58 2024, max compression
```

## Comparing `atom-tools-0.5.2.tar` & `atom-tools-0.5.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.398151 atom-tools-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 14:03:19.000000 atom-tools-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-04 14:03:19.000000 atom-tools-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-04 14:03:28.398151 atom-tools-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-04-04 14:03:19.000000 atom-tools-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.394151 atom-tools-0.5.2/atom_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.394151 atom-tools-0.5.2/atom_tools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/command_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.394151 atom-tools-0.5.2/atom_tools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/commands/query_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/commands/validate_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/logging_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.398151 atom-tools-0.5.2/atom_tools/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28204 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/regex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.398151 atom-tools-0.5.2/atom_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-04 14:03:28.000000 atom-tools-0.5.2/atom_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-04 14:03:28.000000 atom-tools-0.5.2/atom_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:03:28.000000 atom-tools-0.5.2/atom_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 14:03:28.000000 atom-tools-0.5.2/atom_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-04 14:03:28.000000 atom-tools-0.5.2/atom_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 14:03:28.000000 atom-tools-0.5.2/atom_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-04 14:03:19.000000 atom-tools-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:03:28.398151 atom-tools-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.398151 atom-tools-0.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)   831738 2024-04-04 14:03:19.000000 atom-tools-0.5.2/test/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-04 14:03:19.000000 atom-tools-0.5.2/test/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 14:03:19.000000 atom-tools-0.5.2/test/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-04 14:03:19.000000 atom-tools-0.5.2/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.544552 atom-tools-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 16:50:36.000000 atom-tools-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-08 16:50:36.000000 atom-tools-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-08 16:50:58.544552 atom-tools-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-04-08 16:50:36.000000 atom-tools-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.540552 atom-tools-0.5.3/atom_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.540552 atom-tools-0.5.3/atom_tools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/command_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.540552 atom-tools-0.5.3/atom_tools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/commands/query_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/commands/validate_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/logging_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.544552 atom-tools-0.5.3/atom_tools/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28204 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/regex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25732 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.544552 atom-tools-0.5.3/atom_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-08 16:50:58.000000 atom-tools-0.5.3/atom_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-08 16:50:58.000000 atom-tools-0.5.3/atom_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:50:58.000000 atom-tools-0.5.3/atom_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 16:50:58.000000 atom-tools-0.5.3/atom_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 16:50:58.000000 atom-tools-0.5.3/atom_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 16:50:58.000000 atom-tools-0.5.3/atom_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-08 16:50:36.000000 atom-tools-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:50:58.544552 atom-tools-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.544552 atom-tools-0.5.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)   831738 2024-04-08 16:50:36.000000 atom-tools-0.5.3/test/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-08 16:50:36.000000 atom-tools-0.5.3/test/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-08 16:50:36.000000 atom-tools-0.5.3/test/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-08 16:50:36.000000 atom-tools-0.5.3/test/test_utils.py
```

### Comparing `atom-tools-0.5.2/LICENSE` & `atom-tools-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/PKG-INFO` & `atom-tools-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atom-tools
-Version: 0.5.2
+Version: 0.5.3
 Summary: Collection of tools for use with AppThreat/atom.
 Author-email: Caroline Russell <caroline@appthreat.dev>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/appthreat/atom-tools
 Project-URL: Bug Tracker, https://github.com/appthreat/atom-tools/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `atom-tools-0.5.2/README.md` & `atom-tools-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/atom_tools/cli/application.py` & `atom-tools-0.5.3/atom_tools/cli/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         command = event.command
         if not isinstance(command, Command):
             return
 
         io = event.io
 
         loggers = []
-        loggers += command.loggers
+        loggers += command.loggers  # type: ignore
 
         handler = IOHandler(io)
         handler.setFormatter(IOFormatter())
 
         level = logging.WARNING
 
         if io.is_debug():
```

### Comparing `atom-tools-0.5.2/atom_tools/cli/command_loader.py` & `atom-tools-0.5.3/atom_tools/cli/command_loader.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/atom_tools/cli/commands/convert.py` & `atom-tools-0.5.3/atom_tools/cli/commands/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,16 @@
             's',
             'The server url to be included in the server object.',
             flag=False,
         )
     ]
     help = """The convert command converts an atom slice to a different format.
 Currently supports creating an OpenAPI 3.x document based on a usages slice."""
-    loggers = ['atom_tools.lib.converter', 'atom_tools.lib.regex_utils', 'atom_tools.lib.slices']
+    loggers = ['atom_tools.lib.converter', 'atom_tools.lib.regex_utils', 'atom_tools.lib.slices',
+               'atom_tools.lib.utils']
 
     def handle(self):
         """
         Executes the convert command and performs the conversion.
         """
         supported_types = {'java', 'jar', 'python', 'py', 'javascript', 'js', 'typescript', 'ts'}
         if self.option('type') not in supported_types:
```

### Comparing `atom-tools-0.5.2/atom_tools/cli/commands/filter.py` & `atom-tools-0.5.3/atom_tools/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/atom_tools/cli/commands/query_endpoints.py` & `atom-tools-0.5.3/atom_tools/cli/commands/query_endpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,16 +53,17 @@
         ),
         option(
             'sparse',
             's',
             'Only display names; do not include path and line numbers.',
         )
     ]
-    help = """The query command can be used to return results directly to the console. """
-    loggers = ['atom_tools.lib.converter', 'atom_tools.lib.regex_utils', 'atom_tools.lib.slices']
+    help = """The query command can be used to return endpoint results directly to the console. """
+    loggers = ['atom_tools.lib.converter', 'atom_tools.lib.regex_utils', 'atom_tools.lib.slices',
+               'atom_tools.lib.utils']
 
     def handle(self):
         """
         Executes the query command and performs the conversion.
         """
         supported_types = {'java', 'jar', 'python', 'py', 'javascript', 'js', 'typescript', 'ts'}
         if self.option('type') not in supported_types:
@@ -70,12 +71,14 @@
         converter = OpenAPI(
             'openapi3.1.0',
             self.option('type'),
             self.option('input-slice'),
         )
         if not (result := converter.endpoints_to_openapi('')):
             logging.warning('No results produced!')
-        line_filter = ()
-        if self.option('filter-lines'):
-            line_filter = get_ln_range(self.option('filter-lines'))
-        output = output_endpoints(result, self.option('sparse'), line_filter)
-        print(output)
+            print('')
+        else:
+            line_filter = ()
+            if self.option('filter-lines'):
+                line_filter = get_ln_range(self.option('filter-lines'))
+            output = output_endpoints(result, self.option('sparse'), line_filter)
+            print(output)
```

### Comparing `atom-tools-0.5.2/atom_tools/cli/commands/validate_lines.py` & `atom-tools-0.5.3/atom_tools/cli/commands/validate_lines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # pylint: disable=duplicate-code
 """
 Line validation command for the atom-tools CLI.
 """
+import logging
 import os
 import pathlib
 import sys
 
 from cleo.helpers import option
 
 from atom_tools.cli.commands.command import Command
 from atom_tools.lib.validator import LineValidator
 
 
+logger = logging.getLogger(__name__)
+
+
 class ValidateLinesCommand(Command):
     """
     This command handles the conversion of an atom slice to a specified
     destination format.
 
     Attributes:
         name (str): The name of the command.
@@ -68,15 +72,16 @@
             'j',
             'JSON report file to store invalid lines. Include valid lines as well using -v flag.',
             flag=False,
         )
 
     ]
     help = """Validate source file line numbers in an atom usages or reachables slice."""
-    loggers = ['atom_tools.lib.validator', 'atom_tools.lib.regex_utils', 'atom_tools.lib.slices']
+    loggers = ['atom_tools.lib.validator', 'atom_tools.lib.regex_utils', 'atom_tools.lib.slices',
+               'atom_tools.lib.utils']
 
     def handle(self):
         """
         Executes the line validation and outputs the results.
         """
         if not os.path.isfile(self.option('input-slice')):
             self.line(f'Could not locate {self.option("input-slice")}.')
```

### Comparing `atom-tools-0.5.2/atom_tools/cli/logging_config.py` & `atom-tools-0.5.3/atom_tools/cli/logging_config.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/atom_tools/lib/converter.py` & `atom-tools-0.5.3/atom_tools/lib/converter.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/atom_tools/lib/filtering.py` & `atom-tools-0.5.3/atom_tools/lib/filtering.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/atom_tools/lib/regex_utils.py` & `atom-tools-0.5.3/atom_tools/lib/regex_utils.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/atom_tools/lib/slices.py` & `atom-tools-0.5.3/atom_tools/lib/slices.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,17 +93,17 @@
         with open(filename, 'r', encoding='utf-8') as f:
             raw_content = f.read().replace(r'\\', '/')
             if 'flask' in raw_content:
                 custom_attr = 'flask'
             elif 'django' in raw_content:
                 custom_attr = 'django'
             content = json.loads(raw_content)
-        if content.get('objectSlices'):
+        if 'objectSlices' in content:
             slice_type = 'usages'
-        if content.get('reachables'):
+        elif 'reachables' in content:
             slice_type = 'reachables'
     except (json.decoder.JSONDecodeError, UnicodeDecodeError):
         logger.warning(
             f'Failed to load usages slice: {filename}\nPlease check that you specified a valid'
             f' json file.'
         )
     except FileNotFoundError:
```

### Comparing `atom-tools-0.5.2/atom_tools/lib/utils.py` & `atom-tools-0.5.3/atom_tools/lib/utils.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/atom_tools/lib/validator.py` & `atom-tools-0.5.3/atom_tools/lib/validator.py`

 * *Files identical despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import jmespath
 
 from atom_tools.lib.slices import AtomSlice
 from atom_tools.lib.regex_utils import ValidationRegexCollection
 from atom_tools.lib.utils import export_json, remove_duplicates_list
 
+
 logger = logging.getLogger(__name__)
 regex: ValidationRegexCollection = ValidationRegexCollection()
 operator_map: Dict[str, List[str]] = {
     '<operator>.addition': ['+'],
     '<operator>.minus': ['-'],
     '<operator>.multiplication': ['*'],
     '<operator>.division': ['/'],
```

### Comparing `atom-tools-0.5.2/atom_tools.egg-info/PKG-INFO` & `atom-tools-0.5.3/atom_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atom-tools
-Version: 0.5.2
+Version: 0.5.3
 Summary: Collection of tools for use with AppThreat/atom.
 Author-email: Caroline Russell <caroline@appthreat.dev>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/appthreat/atom-tools
 Project-URL: Bug Tracker, https://github.com/appthreat/atom-tools/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `atom-tools-0.5.2/atom_tools.egg-info/SOURCES.txt` & `atom-tools-0.5.3/atom_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/pyproject.toml` & `atom-tools-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atom-tools"
-version = "0.5.2"
+version = "0.5.3"
 description = "Collection of tools for use with AppThreat/atom."
 authors = [
   { name = "Caroline Russell", email = "caroline@appthreat.dev" },
 ]
 dependencies = ["cleo>=1.0.0", "jmespath>=1.0.0", "thefuzz>=0.22.1", "json-flatten>=0.3"]
 license = { text = "Apache-2.0" }
 readme = "README.md"
```

### Comparing `atom-tools-0.5.2/test/test_converter.py` & `atom-tools-0.5.3/test/test_converter.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/test/test_filtering.py` & `atom-tools-0.5.3/test/test_filtering.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/test/test_slices.py` & `atom-tools-0.5.3/test/test_slices.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.2/test/test_utils.py` & `atom-tools-0.5.3/test/test_utils.py`

 * *Files identical despite different names*

