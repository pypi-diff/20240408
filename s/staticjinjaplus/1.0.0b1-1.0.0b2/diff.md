# Comparing `tmp/staticjinjaplus-1.0.0b1.tar.gz` & `tmp/staticjinjaplus-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staticjinjaplus-1.0.0b1.tar", last modified: Fri Apr  5 09:33:52 2024, max compression
+gzip compressed data, was "staticjinjaplus-1.0.0b2.tar", last modified: Mon Apr  8 15:59:03 2024, max compression
```

## Comparing `staticjinjaplus-1.0.0b1.tar` & `staticjinjaplus-1.0.0b2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 09:33:52.777515 staticjinjaplus-1.0.0b1/
--rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-1.0.0b1/LICENSE.md
--rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-1.0.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0     3684 2024-04-05 09:33:52.776515 staticjinjaplus-1.0.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     2315 2024-04-05 07:32:59.000000 staticjinjaplus-1.0.0b1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 09:33:52.777515 staticjinjaplus-1.0.0b1/setup.cfg
--rw-rw-rw-   0        0        0     3557 2024-04-05 09:28:32.000000 staticjinjaplus-1.0.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:33:52.765515 staticjinjaplus-1.0.0b1/staticjinjaplus/
--rw-rw-rw-   0        0        0     5705 2024-04-05 09:06:54.000000 staticjinjaplus-1.0.0b1/staticjinjaplus/__init__.py
--rw-rw-rw-   0        0        0       23 2024-04-04 21:46:33.000000 staticjinjaplus-1.0.0b1/staticjinjaplus/__version__.py
--rw-rw-rw-   0        0        0     1253 2024-04-05 08:59:20.000000 staticjinjaplus-1.0.0b1/staticjinjaplus/cli.py
--rw-rw-rw-   0        0        0     1988 2024-04-05 08:38:21.000000 staticjinjaplus-1.0.0b1/staticjinjaplus/helpers.py
--rw-rw-rw-   0        0        0     1966 2024-04-05 08:45:25.000000 staticjinjaplus-1.0.0b1/staticjinjaplus/http.py
--rw-rw-rw-   0        0        0        0 2024-04-05 08:17:36.000000 staticjinjaplus-1.0.0b1/staticjinjaplus/jinja.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:33:52.775515 staticjinjaplus-1.0.0b1/staticjinjaplus.egg-info/
--rw-rw-rw-   0        0        0     3684 2024-04-05 09:33:52.000000 staticjinjaplus-1.0.0b1/staticjinjaplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2024-04-05 09:33:52.000000 staticjinjaplus-1.0.0b1/staticjinjaplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 09:33:52.000000 staticjinjaplus-1.0.0b1/staticjinjaplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-05 09:33:52.000000 staticjinjaplus-1.0.0b1/staticjinjaplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      100 2024-04-05 09:33:52.000000 staticjinjaplus-1.0.0b1/staticjinjaplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-05 09:33:52.000000 staticjinjaplus-1.0.0b1/staticjinjaplus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 15:59:03.204876 staticjinjaplus-1.0.0b2/
+-rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-1.0.0b2/LICENSE.md
+-rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-1.0.0b2/MANIFEST.in
+-rw-rw-rw-   0        0        0    12082 2024-04-08 15:59:03.203875 staticjinjaplus-1.0.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0    10664 2024-04-08 15:54:17.000000 staticjinjaplus-1.0.0b2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 15:59:03.204876 staticjinjaplus-1.0.0b2/setup.cfg
+-rw-rw-rw-   0        0        0     3598 2024-04-08 11:58:14.000000 staticjinjaplus-1.0.0b2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:59:03.188876 staticjinjaplus-1.0.0b2/staticjinjaplus/
+-rw-rw-rw-   0        0        0     5778 2024-04-08 14:35:27.000000 staticjinjaplus-1.0.0b2/staticjinjaplus/__init__.py
+-rw-rw-rw-   0        0        0       23 2024-04-07 14:10:44.000000 staticjinjaplus-1.0.0b2/staticjinjaplus/__version__.py
+-rw-rw-rw-   0        0        0     1280 2024-04-07 14:43:00.000000 staticjinjaplus-1.0.0b2/staticjinjaplus/cli.py
+-rw-rw-rw-   0        0        0     2407 2024-04-07 14:45:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus/http.py
+-rw-rw-rw-   0        0        0     1290 2024-04-07 14:40:43.000000 staticjinjaplus-1.0.0b2/staticjinjaplus/jinja_helpers.py
+-rw-rw-rw-   0        0        0      712 2024-04-07 14:40:31.000000 staticjinjaplus-1.0.0b2/staticjinjaplus/staticjinja_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:59:03.202876 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/
+-rw-rw-rw-   0        0        0    12082 2024-04-08 15:59:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2024-04-08 15:59:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 15:59:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-08 15:59:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      115 2024-04-08 15:59:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-08 15:59:03.000000 staticjinjaplus-1.0.0b2/staticjinjaplus.egg-info/top_level.txt
```

### Comparing `staticjinjaplus-1.0.0b1/LICENSE.md` & `staticjinjaplus-1.0.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b1/setup.py` & `staticjinjaplus-1.0.0b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 REQUIRED = [
     'staticjinja~=5.0',
     'webassets~=2.0',
     'htmlmin~=0.1',
     'cssutils~=2.10',
     'jsmin~=3.0',
+    'environs~=11.0',
 ]
 
 EXTRAS = {
     'dev': {
         'build~=1.2',
         'twine~=5.0',
     }
@@ -37,15 +38,15 @@
     'Topic :: Text Processing :: Markup :: HTML',
     'Topic :: Text Processing :: Markup :: Markdown',
     'Programming Language :: Python :: 3.12',
     'Intended Audience :: Developers',
 ]
 
 PROJECT_URLS = {
-    'Documentation': 'https://github.com/EpocDotFr/staticjinjaplus#readme',
+    'Documentation': 'https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#usage',
     'Source': 'https://github.com/EpocDotFr/staticjinjaplus',
     'Tracker': 'https://github.com/EpocDotFr/staticjinjaplus/issues',
     'Changelog': 'https://github.com/EpocDotFr/staticjinjaplus/releases',
 }
 
 here = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `staticjinjaplus-1.0.0b1/staticjinjaplus/__init__.py` & `staticjinjaplus-1.0.0b2/staticjinjaplus/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,53 @@
+from staticjinjaplus.http import ThreadingHTTPServerWithConfig, SimpleEnhancedHTTPRequestHandler
 from webassets import Environment as AssetsEnvironment
-from staticjinjaplus.http import make_handler
+from staticjinjaplus import staticjinja_helpers
 from importlib import util as importlib_util
-from http.server import ThreadingHTTPServer
-import staticjinjaplus.helpers as helpers
+from staticjinjaplus import jinja_helpers
+from shutil import copytree, rmtree
+from os import makedirs, path
 from staticjinja import Site
-from copy import deepcopy
+from subprocess import call
+from environs import Env
 from typing import Dict
 import locale
-import shutil
 import sys
-import os
-
-
-DEFAULT_CONFIG = {
-    'LOCALE': None,
-    'SERVE_PORT': 8080,
-    'BASE_URL': 'http://localhost:8080/',
-    'MINIFY_XML': False,
-    'MINIFY_JSON': False,
-    'TEMPLATES_DIR': 'templates',
-    'OUTPUT_DIR': 'output',
-    'STATIC_DIR': 'static',
-    'STATIC_FILES_TO_COPY': [],
-    'STATIC_DIRECTORIES_TO_COPY': [],
-    'ASSETS_DIR': 'assets',
-    'ASSETS_BUNDLES': [],
-    'CONTEXTS': [],
-}
 
 
 def load_config() -> Dict:
     """Load configuration from both `config.py` in the directory where staticjinjaplus is executed and environment
-    variables, returning a dict representation of this configuration. Only uppercase variables are taken into account"""
-    config = deepcopy(DEFAULT_CONFIG)
+    variables, returning a dict representation of this configuration. Only uppercase variables are loaded"""
 
+    # Set default config values
+    config = {
+        'LOCALE': None,
+        'SERVE_PORT': 8080,
+        'BASE_URL': 'http://localhost:8080/',
+        'MINIFY_XML': False,
+        'MINIFY_JSON': False,
+        'TEMPLATES_DIR': 'templates',
+        'OUTPUT_DIR': 'output',
+        'STATIC_DIR': 'static',
+        'ASSETS_DIR': 'assets',
+        'ASSETS_BUNDLES': [],
+        'CONTEXTS': [],
+    }
+
+    # Load and erase default config values from config.py, if the file exists
     try:
         spec = importlib_util.spec_from_file_location('config', 'config.py')
         actual_config = importlib_util.module_from_spec(spec)
         spec.loader.exec_module(actual_config)
 
         config.update({
             k: v for k, v in vars(actual_config).items() if k.isupper()
         })
     except FileNotFoundError:
         pass
 
-    config.update({
-        'BASE_URL': os.environ.get('BASE_URL', config['BASE_URL']),
-        'MINIFY_XML': os.environ.get('MINIFY_XML', config['MINIFY_XML']) in (True, 'True'),
-        'MINIFY_JSON': os.environ.get('MINIFY_JSON', config['MINIFY_JSON']) in (True, 'True'),
-        'SSH_USER': os.environ.get('SSH_USER'),
-        'SSH_HOST': os.environ.get('SSH_HOST'),
-        'SSH_PORT': int(os.environ.get('SSH_PORT', 22)),
-        'SSH_PATH': os.environ.get('SSH_PATH'),
-    })
-
     return config
 
 
 def set_locale(config: Dict) -> None:
     """Set the system locale based on the LOCALE config"""
     if not config['LOCALE']:
         return
@@ -81,94 +70,113 @@
         print('Unable to set system locale', file=sys.stderr)
 
 
 def build(config: Dict, watch: bool = False) -> None:
     """Build the site"""
     set_locale(config)
 
-    os.makedirs(config['STATIC_DIR'], exist_ok=True)
-    os.makedirs(config['OUTPUT_DIR'], exist_ok=True)
-    os.makedirs(config['ASSETS_DIR'], exist_ok=True)
+    webassets_cache = path.join(config['ASSETS_DIR'], '.webassets-cache')
 
-    print('Copying static files from "{STATIC_DIR}" to "{OUTPUT_DIR}"...'.format(**config))
-
-    for file in config['STATIC_FILES_TO_COPY']:
-        dir_name = os.path.dirname(file)
+    makedirs(webassets_cache, exist_ok=True)
+    makedirs(config['STATIC_DIR'], exist_ok=True)
+    makedirs(config['OUTPUT_DIR'], exist_ok=True)
+    makedirs(config['ASSETS_DIR'], exist_ok=True)
 
-        if dir_name:
-            os.makedirs(dir_name, exist_ok=True)
-
-        shutil.copy2(str(os.path.join(config['STATIC_DIR'], file)), config['OUTPUT_DIR'])
+    print('Copying static files from "{STATIC_DIR}" to "{OUTPUT_DIR}"...'.format(**config))
 
-    for directory in config['STATIC_DIRECTORIES_TO_COPY']:
-        shutil.copytree(str(os.path.join(config['STATIC_DIR'], directory)), str(os.path.join(config['OUTPUT_DIR'], directory)), dirs_exist_ok=True)
+    copytree(
+        config['STATIC_DIR'],
+        config['OUTPUT_DIR'],
+        dirs_exist_ok=True
+    )
 
     print('Building from "{TEMPLATES_DIR}" to "{OUTPUT_DIR}"...'.format(**config))
 
     site = Site.make_site(
         searchpath=config['TEMPLATES_DIR'],
         outpath=config['OUTPUT_DIR'],
         mergecontexts=True,
         env_globals={
             'config': config,
-            'url': helpers.jinja_url(config),
-            'icon': helpers.jinja_icon(config),
+            'url': jinja_helpers.url(config),
+            'icon': jinja_helpers.icon(config),
         },
         filters={
-            'tojsonm': helpers.jinja_tojsonm(config),
-            'dictmerge': helpers.jinja_dictmerge,
+            'tojsonm': jinja_helpers.tojsonm(config),
+            'dictmerge': jinja_helpers.dictmerge,
         },
         contexts=config['CONTEXTS'] or None,
         rules=[
-            (r'.*\.(html|xml)', helpers.minify_xml_template)
+            (r'.*\.(html|xml)', staticjinja_helpers.minify_xml_template)
         ] if config['MINIFY_XML'] else None,
         extensions=['webassets.ext.jinja2.AssetsExtension'],
         env_kwargs={
             'trim_blocks': True,
             'lstrip_blocks': True,
         }
     )
 
     site.env.assets_environment = AssetsEnvironment(
         directory=config['OUTPUT_DIR'],
         url='/',
-        cache=os.path.join(config['ASSETS_DIR'], '.webassets-cache')
+        cache=webassets_cache
     )
 
     site.env.assets_environment.append_path(config['ASSETS_DIR'])
 
     for name, args, kwargs in config['ASSETS_BUNDLES']:
         site.env.assets_environment.register(name, *args, **kwargs)
 
     site.render(watch)
 
 
 def clean(config: Dict) -> None:
     """Delete and recreate the output directory"""
     print('Deleting and recreating "{OUTPUT_DIR}"...'.format(**config))
 
-    if os.path.isdir(config['OUTPUT_DIR']):
-        shutil.rmtree(config['OUTPUT_DIR'])
+    if path.isdir(config['OUTPUT_DIR']):
+        rmtree(config['OUTPUT_DIR'])
 
-    os.makedirs(config['OUTPUT_DIR'], exist_ok=True)
+    makedirs(config['OUTPUT_DIR'], exist_ok=True)
 
 
 def publish(config: Dict) -> None:
     """Publish the site (using `rsync` through SSH)"""
-    os.system(''.join([
-        'rsync --delete --exclude ".DS_Store" -pthrvz -c ',
-        '-e "ssh -p {SSH_PORT}" ',
+    print('Overriding some configuration values from environment variables...')
+
+    env = Env()
+
+    try:
+        config.update({
+            'BASE_URL': env.str('BASE_URL'),
+            'MINIFY_XML': env.bool('MINIFY_XML', config['MINIFY_XML']),
+            'MINIFY_JSON': env.bool('MINIFY_JSON', config['MINIFY_JSON']),
+            'SSH_USER': env.str('SSH_USER'),
+            'SSH_HOST': env.str('SSH_HOST'),
+            'SSH_PORT': env.int('SSH_PORT', default=22),
+            'SSH_PATH': env.str('SSH_PATH'),
+        })
+    except ValueError as e:
+        print(e, file=sys.stderr)
+
+    exit(call(
+        'rsync --delete --exclude ".DS_Store" -pthrvz -c '
+        '-e "ssh -p {SSH_PORT}" '
         '{} {SSH_USER}@{SSH_HOST}:{SSH_PATH}'.format(
             config['OUTPUT_DIR'].rstrip('/') + '/', **config
         )
-    ]))
+    ))
 
 
 def serve(config: Dict) -> None:
     """Serve the rendered site directory through HTTP"""
     print('Serving "{OUTPUT_DIR}" on http://localhost:{SERVE_PORT}/'.format(**config))
 
-    with ThreadingHTTPServer(('127.0.0.1', config['SERVE_PORT']), make_handler(config)) as server:
+    with ThreadingHTTPServerWithConfig(
+            ('127.0.0.1', config['SERVE_PORT']),
+            SimpleEnhancedHTTPRequestHandler,
+            directory=config['OUTPUT_DIR']
+    ) as server:
         try:
             server.serve_forever()
         except KeyboardInterrupt:
             pass
```

### Comparing `staticjinjaplus-1.0.0b1/staticjinjaplus/cli.py` & `staticjinjaplus-1.0.0b2/staticjinjaplus/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from argparse import ArgumentParser
 import staticjinjaplus
-import argparse
 
 
 def cli() -> None:
-    arg_parser = argparse.ArgumentParser(description='The staticjinjaplus CLI which should be your main and only entry point to staticjinjaplus.')
+    arg_parser = ArgumentParser(
+        description='The staticjinjaplus CLI which should be your main and only entry point to staticjinjaplus.'
+    )
 
     command_arg_parser = arg_parser.add_subparsers(dest='command', required=True)
 
     build_arg_parser = command_arg_parser.add_parser('build', help='Build the site')
     build_arg_parser.add_argument(
         '-w', '--watch',
         help='Automatically rebuild the site when templates are modified',
```

### Comparing `staticjinjaplus-1.0.0b1/staticjinjaplus/http.py` & `staticjinjaplus-1.0.0b2/staticjinjaplus/http.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,65 @@
-from http.server import SimpleHTTPRequestHandler
+from __future__ import annotations
+from http.server import ThreadingHTTPServer, SimpleHTTPRequestHandler
 from http import HTTPStatus
-from typing import Dict
-import os
+from os import fstat, path
 
 
-def make_handler(config: Dict):
-    class SimpleButEnhancedHTTPRequestHandler(SimpleHTTPRequestHandler):
-        """A simple HTTP server which is meant to serve the output directory, with some enhancements (emulates URL rewrite
-        for HTML files without .html extension; emulates custom 404 error page"""
-        protocol_version = 'HTTP/1.1'
+class ThreadingHTTPServerWithConfig(ThreadingHTTPServer):
+    """Same as ThreadingHTTPServer but the directory to be served may be passed to its constructor"""
+    allow_reuse_address = True
+    daemon_threads = True
+    directory: str
+    RequestHandlerClass: SimpleEnhancedHTTPRequestHandler
 
-        def __init__(self, *args, **kvargs):
-            try:
-                super().__init__(*args, **kvargs, directory=config['OUTPUT_DIR'])
-            except (ConnectionAbortedError, BrokenPipeError):
-                pass
+    def __init__(self, *args, directory: str, **kvargs):
+        super().__init__(*args, **kvargs)
+
+        self.directory = directory
 
-        def translate_path(self, path):
-            path = super().translate_path(path)
+    def finish_request(self, request, client_address) -> None:
+        self.RequestHandlerClass(request, client_address, self, directory=self.directory)
 
-            if not path.endswith(('\\', '/')):
-                _, extension = os.path.splitext(path)
 
-                if not extension:
-                    path += '.html'
+class SimpleEnhancedHTTPRequestHandler(SimpleHTTPRequestHandler):
+    """A simple HTTP server handler which is meant to serve the output directory, with some enhancements (emulates URL
+    rewrite for HTML files without .html extension; emulates custom 404 error page"""
+    protocol_version = 'HTTP/1.1'
+    server: ThreadingHTTPServerWithConfig
 
-            return path
+    def __init__(self, *args, **kvargs):
+        try:
+            super().__init__(*args, **kvargs)
+        except (ConnectionAbortedError, BrokenPipeError):
+            pass
 
-        def send_error(self, code, message=None, explain=None):
-            if self.command != 'HEAD' and code == HTTPStatus.NOT_FOUND:
-                try:
-                    f = open(os.path.join(self.directory, '404.html'), 'rb')
-                except OSError:
-                    return super().send_error(code, message=message, explain=explain)
+    def translate_path(self, p) -> str:
+        p = super().translate_path(p)
 
-                fs = os.fstat(f.fileno())
+        if not p.endswith(('\\', '/')):
+            _, extension = path.splitext(p)
 
-                self.log_error("code %d, message %s", code, message)
-                self.send_response(code, message)
-                self.send_header('Connection', 'close')
+            if not extension:
+                p += '.html'
 
-                self.send_header('Content-Type', self.error_content_type)
-                self.send_header('Content-Length', str(fs[6]))
-                self.end_headers()
+        return p
 
-                self.copyfile(f, self.wfile)
-            else:
+    def send_error(self, code, message=None, explain=None) -> None:
+        if self.command != 'HEAD' and code == HTTPStatus.NOT_FOUND:
+            try:
+                f = open(path.join(self.directory, '404.html'), 'rb')
+            except OSError:
                 return super().send_error(code, message=message, explain=explain)
 
-    return SimpleButEnhancedHTTPRequestHandler
+            fs = fstat(f.fileno())
+
+            self.log_error("code %d, message %s", code, message)
+            self.send_response(code, message)
+            self.send_header('Connection', 'close')
+
+            self.send_header('Content-Type', self.error_content_type)
+            self.send_header('Content-Length', str(fs[6]))
+            self.end_headers()
+
+            self.copyfile(f, self.wfile)
+        else:
+            return super().send_error(code, message=message, explain=explain)
```

