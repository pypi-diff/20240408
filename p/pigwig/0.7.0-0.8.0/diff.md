# Comparing `tmp/pigwig-0.7.0.tar.gz` & `tmp/pigwig-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigwig-0.7.0.tar", last modified: Wed Dec 30 22:28:25 2020, max compression
+gzip compressed data, was "pigwig-0.8.0.tar", last modified: Mon Apr  8 03:07:24 2024, max compression
```

## Comparing `pigwig-0.7.0.tar` & `pigwig-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 raylu     (1000) raylu     (1000)        0 2020-12-30 22:28:25.000000 pigwig-0.7.0/
--rw-r--r--   0 raylu     (1000) raylu     (1000)      329 2020-12-30 22:28:25.000000 pigwig-0.7.0/PKG-INFO
--rw-r--r--   0 raylu     (1000) raylu     (1000)     1647 2019-10-24 18:44:16.000000 pigwig-0.7.0/README.md
-drwxr-xr-x   0 raylu     (1000) raylu     (1000)        0 2020-12-30 22:28:25.000000 pigwig-0.7.0/pigwig/
--rw-r--r--   0 raylu     (1000) raylu     (1000)      134 2020-07-22 04:38:47.000000 pigwig-0.7.0/pigwig/__init__.py
--rw-r--r--   0 raylu     (1000) raylu     (1000)      441 2020-07-22 04:38:47.000000 pigwig-0.7.0/pigwig/exceptions.py
--rw-r--r--   0 raylu     (1000) raylu     (1000)     1692 2020-07-22 04:38:47.000000 pigwig-0.7.0/pigwig/inotify.py
--rw-r--r--   0 raylu     (1000) raylu     (1000)     2368 2020-07-22 04:38:47.000000 pigwig-0.7.0/pigwig/multipart.py
--rw-r--r--   0 raylu     (1000) raylu     (1000)     9487 2020-07-22 04:39:33.000000 pigwig-0.7.0/pigwig/pigwig.py
--rw-r--r--   0 raylu     (1000) raylu     (1000)      691 2020-07-22 04:39:00.000000 pigwig-0.7.0/pigwig/reloader_linux.py
--rw-r--r--   0 raylu     (1000) raylu     (1000)      512 2020-07-22 04:39:06.000000 pigwig-0.7.0/pigwig/reloader_osx.py
--rw-r--r--   0 raylu     (1000) raylu     (1000)     7893 2020-07-22 04:38:47.000000 pigwig-0.7.0/pigwig/request_response.py
--rw-r--r--   0 raylu     (1000) raylu     (1000)     2899 2020-07-22 04:38:47.000000 pigwig-0.7.0/pigwig/routes.py
--rw-r--r--   0 raylu     (1000) raylu     (1000)      468 2020-07-22 04:38:47.000000 pigwig-0.7.0/pigwig/templates_jinja.py
-drwxr-xr-x   0 raylu     (1000) raylu     (1000)        0 2020-12-30 22:28:25.000000 pigwig-0.7.0/pigwig.egg-info/
--rw-r--r--   0 raylu     (1000) raylu     (1000)      329 2020-12-30 22:28:25.000000 pigwig-0.7.0/pigwig.egg-info/PKG-INFO
--rw-r--r--   0 raylu     (1000) raylu     (1000)      351 2020-12-30 22:28:25.000000 pigwig-0.7.0/pigwig.egg-info/SOURCES.txt
--rw-r--r--   0 raylu     (1000) raylu     (1000)        1 2020-12-30 22:28:25.000000 pigwig-0.7.0/pigwig.egg-info/dependency_links.txt
--rw-r--r--   0 raylu     (1000) raylu     (1000)        7 2020-12-30 22:28:25.000000 pigwig-0.7.0/pigwig.egg-info/top_level.txt
--rw-r--r--   0 raylu     (1000) raylu     (1000)       38 2020-12-30 22:28:25.000000 pigwig-0.7.0/setup.cfg
--rwxr-xr-x   0 raylu     (1000) raylu     (1000)      482 2020-12-30 22:25:15.000000 pigwig-0.7.0/setup.py
+drwxr-xr-x   0 raylu     (1000) raylu     (1000)        0 2024-04-08 03:07:24.832442 pigwig-0.8.0/
+-rw-r--r--   0 raylu     (1000) raylu     (1000)       71 2023-06-15 03:36:28.000000 pigwig-0.8.0/LICENSE
+-rw-r--r--   0 raylu     (1000) raylu     (1000)     2050 2024-04-08 03:07:24.832442 pigwig-0.8.0/PKG-INFO
+-rw-r--r--   0 raylu     (1000) raylu     (1000)     1647 2024-04-08 01:15:08.000000 pigwig-0.8.0/README.md
+drwxr-xr-x   0 raylu     (1000) raylu     (1000)        0 2024-04-08 03:07:24.832442 pigwig-0.8.0/pigwig/
+-rw-r--r--   0 raylu     (1000) raylu     (1000)      247 2024-04-08 02:47:45.000000 pigwig-0.8.0/pigwig/__init__.py
+-rw-r--r--   0 raylu     (1000) raylu     (1000)      459 2024-04-07 19:54:37.000000 pigwig-0.8.0/pigwig/exceptions.py
+-rw-r--r--   0 raylu     (1000) raylu     (1000)     1809 2024-04-08 02:47:45.000000 pigwig-0.8.0/pigwig/inotify.py
+-rw-r--r--   0 raylu     (1000) raylu     (1000)     2686 2024-04-08 02:47:45.000000 pigwig-0.8.0/pigwig/multipart.py
+-rw-r--r--   0 raylu     (1000) raylu     (1000)    10668 2024-04-08 02:47:45.000000 pigwig-0.8.0/pigwig/pigwig.py
+-rw-r--r--   0 raylu     (1000) raylu     (1000)        0 2024-04-07 16:50:06.000000 pigwig-0.8.0/pigwig/py.typed
+-rw-r--r--   0 raylu     (1000) raylu     (1000)      935 2024-04-08 02:47:45.000000 pigwig-0.8.0/pigwig/reloader_linux.py
+-rw-r--r--   0 raylu     (1000) raylu     (1000)      681 2024-04-08 02:47:45.000000 pigwig-0.8.0/pigwig/reloader_osx.py
+-rw-r--r--   0 raylu     (1000) raylu     (1000)     8728 2024-04-08 02:47:45.000000 pigwig-0.8.0/pigwig/request_response.py
+-rw-r--r--   0 raylu     (1000) raylu     (1000)     3400 2024-04-08 02:47:45.000000 pigwig-0.8.0/pigwig/routes.py
+-rw-r--r--   0 raylu     (1000) raylu     (1000)      623 2024-04-08 02:47:45.000000 pigwig-0.8.0/pigwig/templates_jinja.py
+drwxr-xr-x   0 raylu     (1000) raylu     (1000)        0 2024-04-08 03:07:24.832442 pigwig-0.8.0/pigwig.egg-info/
+-rw-r--r--   0 raylu     (1000) raylu     (1000)     2050 2024-04-08 03:07:24.000000 pigwig-0.8.0/pigwig.egg-info/PKG-INFO
+-rw-r--r--   0 raylu     (1000) raylu     (1000)      381 2024-04-08 03:07:24.000000 pigwig-0.8.0/pigwig.egg-info/SOURCES.txt
+-rw-r--r--   0 raylu     (1000) raylu     (1000)        1 2024-04-08 03:07:24.000000 pigwig-0.8.0/pigwig.egg-info/dependency_links.txt
+-rw-r--r--   0 raylu     (1000) raylu     (1000)        7 2024-04-08 03:07:24.000000 pigwig-0.8.0/pigwig.egg-info/top_level.txt
+-rw-r--r--   0 raylu     (1000) raylu     (1000)     1304 2024-04-08 03:06:44.000000 pigwig-0.8.0/pyproject.toml
+-rw-r--r--   0 raylu     (1000) raylu     (1000)       38 2024-04-08 03:07:24.832442 pigwig-0.8.0/setup.cfg
```

### Comparing `pigwig-0.7.0/README.md` & `pigwig-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pigwig-0.7.0/pigwig/inotify.py` & `pigwig-0.8.0/pigwig/inotify.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-from collections import namedtuple
 import ctypes
 import ctypes.util
-from enum import IntEnum
 import errno
 import os
 import struct
+import typing
+from collections import namedtuple
+from enum import IntEnum
 
-libc = ctypes.cdll.LoadLibrary(ctypes.util.find_library('c'))
+libc = ctypes.cdll.LoadLibrary(typing.cast(str, ctypes.util.find_library('c')))
 libc.__errno_location.restype = ctypes.POINTER(ctypes.c_int)
 
 Event = namedtuple('Event', ['wd', 'mask', 'cookie', 'name'])
 
-def geterr():
+def geterr() -> str:
 	return errno.errorcode[libc.__errno_location().contents.value]
 
-def init():
+def init() -> int:
 	fd = libc.inotify_init()
 	if fd == -1:
 		raise OSError('inotify_init error', geterr())
 	return fd
 
-def add_watch(fd, path, mask):
+def add_watch(fd: int, path: str, mask: int) -> int:
 	wd = libc.inotify_add_watch(fd, path.encode(), mask)
 	if wd == -1:
 		raise OSError('inotify_add_watch error', geterr())
 	return wd
 
-def rm_watch(fd, wd):
+def rm_watch(fd: int, wd: int) -> None:
 	result = libc.inotify_rm_watch(fd, wd)
 	if result == -1:
 		raise OSError('inotify_rm_watch', geterr())
 
-def get_events(fd):
+def get_events(fd: int) -> typing.Iterator[Event]:
 	buf = b''
 	while True:
 		data = os.read(fd, 4096)
 		buf += data
 		if len(data) < 4096:
 			break
 	pos = end = 0
 	while pos < len(buf):
 		end += 16
 		wd, mask, cookie, name_len = struct.unpack('iIII', buf[pos:end])
 		pos = end
 		end = end + name_len
-		name = struct.unpack('%ds' % name_len, buf[pos:end])
-		name = name[0].rstrip(b'\0')
+		(name,) = struct.unpack('%ds' % name_len, buf[pos:end])
+		name = name.rstrip(b'\0')
 		yield Event(wd, mask, cookie, name.decode())
 		pos = end
 
 class IN(IntEnum):
 	ACCESS = 0x00000001
 	MODIFY = 0x00000002
 	ATTRIB = 0x00000004
```

### Comparing `pigwig-0.7.0/pigwig/multipart.py` & `pigwig-0.8.0/pigwig/multipart.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+from __future__ import annotations
+
 import cgi
 import http.client
+import io
 
 maxlen = 1024 * 1024 * 1024 # 1 GB
 
-def parse_multipart(fp, pdict):
-	'''
+def parse_multipart(fp: io.BufferedIOBase, pdict: dict) -> dict[str, list[bytes | MultipartFile]]:
+	"""
 		most of this code is copied straight from
 		`cgi.parse_multipart <https://github.com/python/cpython/blob/ad76602f69d884e491b0913c641dd8e42902c36c/Lib/cgi.py#L201>`_.
 		the only difference is that it returns a :class:`.MultipartFile` for any part with a ``filename``
 		param in its content-disposition (instead of just the bytes).
-	'''
+	"""
 	boundary = pdict.get('boundary', b'')
-	if not cgi.valid_boundary(boundary):
+	if not cgi.valid_boundary(boundary): # type: ignore[attr-defined]
 		raise ValueError('Invalid boundary in multipart form: %r' % boundary)
 
 	nextpart = b'--' + boundary
 	lastpart = b'--' + boundary + b'--'
-	partdict = {}
+	partdict: dict[str, list[bytes | MultipartFile]] = {}
 	terminator = b''
 	while terminator != lastpart:
 		read = -1
-		data = None
+		data: bytes | MultipartFile | None = None
 		if terminator:
 			# At start of next part.  Read headers first.
 			headers = http.client.parse_headers(fp)
 			clength = headers.get('content-length')
 			if clength:
 				try:
 					read = int(clength)
@@ -57,40 +60,41 @@
 				line = lines[-1]
 				if line[-2:] == b'\r\n':
 					line = line[:-2]
 				elif line[-1:] == b'\n':
 					line = line[:-1]
 				lines[-1] = line
 				data = b''.join(lines)
-		line = headers['content-disposition']
-		if not line:
+		content_disposition = headers['content-disposition']
+		if not content_disposition:
 			continue
-		key, params = cgi.parse_header(line)
+		key, params = cgi.parse_header(content_disposition)
 		if key != 'form-data':
 			continue
 		if 'name' in params:
 			name = params['name']
 		else:
 			continue
 
 		if 'filename' in params:
+			assert isinstance(data, bytes)
 			data = MultipartFile(data, params['filename'])
 		if name in partdict:
 			partdict[name].append(data)
 		else:
 			partdict[name] = [data]
 
 	return partdict
 
 class MultipartFile:
-	'''
+	"""
 		instance attrs:
 
 		* ``data`` - a bytes
 		* ``filename`` - a str
-	'''
-	def __init__(self, data, filename):
+	"""
+	def __init__(self, data: bytes, filename: str) -> None:
 		self.data = data
 		self.filename = filename
 
-	def __repr__(self):
+	def __repr__(self) -> str:
 		return '%s(%r, %r)' % (self.__class__.__name__, self.data, self.filename)
```

### Comparing `pigwig-0.7.0/pigwig/pigwig.py` & `pigwig-0.8.0/pigwig/pigwig.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,47 @@
+from __future__ import annotations
+
 import cgi
 import copy
 import http.client
 import http.cookies
-from inspect import isgenerator
 import json
 import sys
 import textwrap
 import traceback
 import urllib.parse
 import wsgiref.simple_server
+from inspect import isgenerator
+from typing import TYPE_CHECKING, Any, Callable, Iterable, Mapping, MutableMapping, TextIO
 
 from . import exceptions, multipart
 from .request_response import HTTPHeaders, Request, Response
 from .routes import build_route_tree
 from .templates_jinja import JinjaTemplateEngine
 
-def default_http_exception_handler(e, errors, request, app):
+if TYPE_CHECKING:
+	import io
+
+	from .routes import RouteDefinition
+
+def default_http_exception_handler(e: exceptions.HTTPException, errors: TextIO, request: Request,
+		app: 'PigWig') -> Response:
 	errors.write(textwrap.indent(e.body, '\t') + '\n')
 	return Response(e.body.encode('utf-8', 'replace'), e.code)
 
-def default_exception_handler(e, errors, request, app):
+def default_exception_handler(e: Exception, errors: TextIO, request: Request, app: 'PigWig') -> Response:
 	tb = traceback.format_exc()
 	errors.write(tb)
 	return Response(tb.encode('utf-8', 'replace'), 500)
 
+HTTPExceptionHandler = Callable[[exceptions.HTTPException, TextIO, Request, 'PigWig'], Response]
+ExceptionHandler = Callable[[Exception, TextIO, Request, 'PigWig'], Response]
+
 class PigWig:
-	'''
+	"""
 		main WSGI entrypoint. this is a class but defines a :func:`.__call__` so instances of it can
 		be passed directly to WSGI servers.
 
 		:type routes: list or function
 		:param routes: a list of 3-tuples: ``(method, path, handler)`` or a function that returns
 		  such a list
 		    * ``method`` is the HTTP method/verb (``GET``, ``POST``, etc.)
@@ -76,92 +88,96 @@
 
 		* ``routes`` - an internal representation of the route tree - not the list passed to the
 		  constructor
 		* ``template_engine``
 		* ``cookie_secret``
 		* ``http_exception_handler``
 		* ``exception_handler``
-	'''
+	"""
 
-	def __init__(self, routes, template_dir=None, template_engine=JinjaTemplateEngine,
-			cookie_secret=None, http_exception_handler=default_http_exception_handler,
-			exception_handler=default_exception_handler, response_done_handler=None):
+	def __init__(self, routes: RouteDefinition | Callable[[], RouteDefinition], template_dir: str | None=None,
+			template_engine: type=JinjaTemplateEngine, cookie_secret: bytes | None=None,
+			http_exception_handler: HTTPExceptionHandler=default_http_exception_handler,
+			exception_handler: ExceptionHandler=default_exception_handler,
+			response_done_handler: Callable[[Request, Response], Any] | None=None) -> None:
 		if callable(routes):
 			routes = routes()
 		self.routes = build_route_tree(routes)
 
 		if template_dir:
 			self.template_engine = template_engine(template_dir)
 		else:
 			self.template_engine = None
 
 		self.cookie_secret = cookie_secret
 		self.http_exception_handler = http_exception_handler
 		self.exception_handler = exception_handler
 		self.response_done_handler = response_done_handler
 
-	def __call__(self, environ, start_response):
-		''' main WSGI entrypoint '''
+	def __call__(self, environ: dict, start_response: Callable) -> Iterable[bytes]:
+		""" main WSGI entrypoint """
 		errors = environ.get('wsgi.errors', sys.stderr)
 		try:
 			if environ['REQUEST_METHOD'] == 'OPTIONS':
 				start_response('200 OK', copy.copy(Response.DEFAULT_HEADERS))
 				return []
 
 			request, err = self.build_request(environ)
 			try:
 				try:
 					if err:
-						raise err # pylint: disable=raising-bad-type
+						raise err
 
 					handler, kwargs = self.routes.route(request.method, request.path)
 					response = handler(request, **kwargs)
 				except exceptions.HTTPException as e:
 					response = self.http_exception_handler(e, errors, request, self)
 			except Exception as e: # something went wrong in handler or http_exception_handler
 				response = self.exception_handler(e, errors, request, self)
 
 			if isinstance(response.body, str):
-				response.body = [response.body.encode('utf-8')] # pylint: disable=no-member
+				response.body = [response.body.encode('utf-8')]
 			elif isinstance(response.body, bytes):
 				response.body = [response.body]
 			elif response.body is None:
 				response.body = []
 			elif not isgenerator(response.body):
 				raise Exception('unhandled view response type: %s' % type(response.body))
 
 			status_line = '%d %s' % (response.code, http.client.responses[response.code])
 			start_response(status_line, response.headers)
 			if self.response_done_handler:
 				self.response_done_handler(request, response)
 			return response.body
-		except: # something went very wrong handling OPTIONS, in error handling, or in sending the response
+		except Exception: # something went very wrong handling OPTIONS, in error handling, or in sending the response
 			errors.write(traceback.format_exc())
 			start_response('500 Internal Server Error', [])
 			return [b'internal server error']
 
-	def build_request(self, environ):
-		''' builds :class:`.Response` objects. for internal use. '''
+	def build_request(self, environ: dict) -> tuple[Request, Exception | None]:
+		""" builds :class:`.Response` objects. for internal use. """
 		method = environ['REQUEST_METHOD']
 		path = environ['PATH_INFO']
-		query = {}
+		query: Mapping[str, list[str] | str] = {}
 		headers = HTTPHeaders()
 		cookies = http.cookies.SimpleCookie()
-		body = err = None
+		body = {}
+		err = None
 
 		try:
 			qs = environ.get('QUERY_STRING')
 			if qs:
 				query = parse_qs(qs)
 
-			content_length = environ.get('CONTENT_LENGTH')
-			if content_length:
-				headers['Content-Length'] = content_length
-				content_length = int(content_length)
-			body = (environ['wsgi.input'], content_length)
+			content_length_str: str | None = environ.get('CONTENT_LENGTH')
+			if content_length_str:
+				headers['Content-Length'] = content_length_str
+				content_length = int(content_length_str)
+			else:
+				content_length = None
 			content_type = environ.get('CONTENT_TYPE')
 			if content_type:
 				headers['Content-Type'] = content_type
 				media_type, params = cgi.parse_header(content_type)
 				handler = self.content_handlers.get(media_type)
 				if handler:
 					body = handler(environ['wsgi.input'], content_length, params)
@@ -174,27 +190,27 @@
 				if key.startswith('HTTP_'):
 					headers[key[5:].replace('_', '-')] = environ[key]
 		except Exception as e:
 			err = e
 
 		return Request(self, method, path, query, headers, body, cookies, environ), err
 
-	def main(self, host='0.0.0.0', port=None):
-		'''
+	def main(self, host: str='0.0.0.0', port: int | None=None) -> None:
+		"""
 		sets up the autoreloader and runs a
 		`wsgiref.simple_server <https://docs.python.org/3/library/wsgiref.html#module-wsgiref.simple_server>`_.
 		useful for development.
-		'''
+		"""
 
 		have_reloader = True
 		if sys.platform == 'linux':
-			from . import reloader_linux as reloader # pylint: disable=import-outside-toplevel
+			from . import reloader_linux as reloader
 		elif sys.platform == 'darwin':
 			try:
-				from . import reloader_osx as reloader # pylint: disable=import-outside-toplevel
+				from . import reloader_osx as reloader
 			except ImportError as e:
 				have_reloader = False
 				print('install', e.name, 'for auto-reloading')
 		else:
 			have_reloader = False
 			print('no reloader available for', sys.platform)
 		if have_reloader:
@@ -208,43 +224,52 @@
 			if len(sys.argv) == 2:
 				port = int(sys.argv[1])
 		server = wsgiref.simple_server.make_server(host, port, self)
 		print('listening on', port)
 		server.serve_forever()
 
 	@staticmethod
-	def handle_urlencoded(body, length, params):
+	def handle_urlencoded(body: io.BufferedIOBase, length: int | None,
+			params: dict[str, str]) -> Mapping[str, str | list[str]]:
+		if length is None:
+			length = -1
 		charset = params.get('charset', 'utf-8')
 		return parse_qs(body.read(length).decode(charset))
 
 	@staticmethod
-	def handle_json(body, length, params):
+	def handle_json(body: io.BufferedIOBase, length: int | None, params: dict[str, str]) -> Any:
+		if length is None:
+			length = -1
 		charset = params.get('charset', 'utf-8')
 		return json.loads(body.read(length).decode(charset))
 
 	@staticmethod
-	def handle_multipart(body, length, params):
+	def handle_multipart(body: io.BufferedIOBase,
+				length: int | None, params: dict[str, Any]) -> dict[str, list[bytes | multipart.MultipartFile]]:
 		params['boundary'] = params['boundary'].encode()
 		form = multipart.parse_multipart(body, params)
 		for k, v in form.items():
 			if len(v) == 1:
-				form[k] = v[0]
+				form[k] = v[0] # type: ignore[assignment]
 		return form
 
+	content_handlers: dict[str, Callable[[io.BufferedIOBase, int | None, dict[str, str]], Any]]
+
 PigWig.content_handlers = {
 	'application/json': PigWig.handle_json,
 	'application/x-www-form-urlencoded': PigWig.handle_urlencoded,
 	'multipart/form-data': PigWig.handle_multipart,
 }
 
-def parse_qs(qs):
+def parse_qs(qs: str) -> Mapping[str, str | list[str]]:
 	if not qs:
 		return {}
 	try:
-		parsed = urllib.parse.parse_qs(qs, keep_blank_values=True, strict_parsing=True, errors='strict')
+		parsed: MutableMapping[str, Any] = urllib.parse.parse_qs(qs,
+				keep_blank_values=True, strict_parsing=True, errors='strict')
 	except UnicodeDecodeError as e:
 		qs_trunc = qs
 		if len(qs_trunc) > 24:
 			qs_trunc = qs_trunc[:24] + '...'
 		raise exceptions.HTTPException(400, '%s\n%r' % (e, qs_trunc)) # "'utf-8' codec can't decode byte ..."
 	except ValueError as e:
 		raise exceptions.HTTPException(400, e.args[0]) # "bad query field: ..."
```

### Comparing `pigwig-0.7.0/pigwig/reloader_linux.py` & `pigwig-0.8.0/pigwig/reloader_linux.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,40 @@
+from __future__ import annotations
+
+import _thread  # noqa: F401
 import os
 import sys
-import _thread
+import typing
 
 from . import inotify
 
-def init():
+def init() -> None:
 	fd = inotify.init()
 	wds = {}
 	for module in sys.modules.values():
 		try:
 			pathname = module.__file__
 		except AttributeError:
 			continue
 		if pathname is None:
 			continue
 		wd = inotify.add_watch(fd, pathname, inotify.IN.CLOSE_WRITE)
 		wds[wd] = pathname
 
+	try:
+		import eventlet
+	except ImportError:
+		pass
+	else:
+		_thread = eventlet.patcher.original('_thread')
 	_thread.start_new_thread(_reloader, (fd, wds))
 
-def _reloader(fd, wds):
+def _reloader(fd: int, wds: dict[int, str]) -> typing.NoReturn:
 	events = inotify.get_events(fd)
 	for event in events:
 		print(wds[event.wd], 'changed, reloading...')
 	do_reload(fd)
 
-def do_reload(fd):
+def do_reload(fd: int) -> typing.NoReturn:
 	os.close(fd)
 	os.closerange(sys.stderr.fileno()+1, os.sysconf('SC_OPEN_MAX')) # close keep-alive client sockets
 	os.execv(sys.argv[0], sys.argv)
```

### Comparing `pigwig-0.7.0/pigwig/request_response.py` & `pigwig-0.8.0/pigwig/request_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,78 @@
-from collections import UserDict
-import copy
+from __future__ import annotations
+
+import datetime
 import hashlib
 import hmac
 import http.cookies
 import json as jsonlib
 import time
+import typing
+from collections import UserDict
 
 from . import exceptions
 
+if typing.TYPE_CHECKING:
+	from .pigwig import PigWig
+
 class Request:
-	'''
+	"""
 	an instance of this class is passed to every route handler. has the following instance attrs:
 
 	* ``app`` - an instance of :class:`.PigWig`
 	* ``method`` - the request method/verb (``GET``, ``POST``, etc.)
 	* ``path`` - WSGI environ ``PATH_INFO`` (``/foo/bar``)
 	* ``query`` - dict of parsed query string. duplicate keys appear as lists
 	* ``headers`` - :class:`.HTTPHeaders` of the headers
 	* ``body`` - dict of parsed body content. see :attr:`PigWig.content_handlers` for a list
 	  of supported content types
 	* ``cookies`` - an instance of
 	  `http.cookies.SimpleCookie <https://docs.python.org/3/library/http.cookies.html#http.cookies.SimpleCookie>`_
 	* ``wsgi_environ`` - the raw `WSGI environ <https://www.python.org/dev/peps/pep-0333/#environ-variables>`_
 	  handed down from the server
-	'''
+	"""
 
-	def __init__(self, app, method, path, query, headers, body, cookies, wsgi_environ):
+	def __init__(self, app: PigWig, method: str, path: str, query: typing.Mapping[str, str |  list[str]],
+				headers: HTTPHeaders, body: dict, cookies: http.cookies.BaseCookie,
+				wsgi_environ: dict[str, typing.Any]) -> None:
 		self.app = app
 		self.method = method
 		self.path = path
 		self.query = query
 		self.headers = headers
 		self.body = body
 		self.cookies = cookies
 		self.wsgi_environ = wsgi_environ
 
-	def get_secure_cookie(self, key, max_time):
-		'''
+	def get_secure_cookie(self, key: str, max_time: datetime.timedelta) -> str | None:
+		"""
 		decode and verify a cookie set with :func:`Response.set_secure_cookie`
 
 		:param key: ``key`` passed to ``set_secure_cookie``
 		:type max_time: `datetime.timedelta <https://docs.python.org/3/library/datetime.html#timedelta-objects>`_
 		  or None
 		:param max_time: amount of time since cookie was set that it should be considered valid for.
 		  this is normally equal to the ``max_age`` passed to ``set_secure_cookie``. longer times mean
 		  larger windows during which a replay attack is valid. this can be None, in which case no
 		  expiry check is performed
 		:rtype: str or None
-		'''
+		"""
+		assert self.app.cookie_secret is not None
 		try:
 			cookie = self.cookies[key].value
 		except KeyError:
 			return None
 		try:
-			value, ts, signature = cookie.rsplit('|', 2)
-			ts = int(ts)
+			value, ts_str, signature = cookie.rsplit('|', 2)
+			ts_int = int(ts_str)
 		except ValueError:
 			raise exceptions.HTTPException(400, 'invalid %s cookie: %s' % (key, cookie))
-		value_ts = '%s|%d' % (value, int(ts))
+		value_ts = '%s|%d' % (value, ts_int)
 		if hmac.compare_digest(signature, _hash(key + '|' + value_ts, self.app.cookie_secret)):
-			if max_time is not None and ts + max_time.total_seconds() < time.time(): # cookie has expired
+			if max_time is not None and ts_int + max_time.total_seconds() < time.time(): # cookie has expired
 				return None
 			return value
 		else:
 			return None
 
 class Response:
 	'''
@@ -84,127 +93,131 @@
 	has the following instance attrs:
 
 	* ``code``
 	* ``body``
 	* ``headers`` - a list of 2-tuples
 	'''
 
-	DEFAULT_HEADERS = [
+	DEFAULT_HEADERS: typing.Sequence[tuple[str, str]] = (
 		('Access-Control-Allow-Origin', '*'),
 		('Access-Control-Allow-Headers', 'Authorization, X-Requested-With, X-Request'),
-	]
+	)
 
 	json_encoder = jsonlib.JSONEncoder(indent='\t')
 	simple_cookie = http.cookies.SimpleCookie()
 
-	def __init__(self, body=None, code=200, content_type='text/plain', location=None, extra_headers=None):
+	def __init__(self, body: str | bytes | typing.Iterator[bytes] | None=None, code: int=200,
+				content_type: str='text/plain', location: str | None=None,
+				extra_headers: list[tuple[str, str]] | None=None) -> None:
 		self.body = body
 		self.code = code
 
-		headers = copy.copy(self.DEFAULT_HEADERS)
+		headers = list(self.DEFAULT_HEADERS)
 		headers.append(('Content-Type', content_type))
 		if location:
 			headers.append(('Location', location))
 		if extra_headers:
 			headers.extend(extra_headers)
 		self.headers = headers
 
-	def set_cookie(self, key, value, domain=None, path='/', expires=None, max_age=None, secure=False, http_only=False):
-		'''
+	def set_cookie(self, key: str, value: typing.Any, domain: str | None=None, path: str='/',
+			expires: datetime.datetime | None=None, max_age: datetime.timedelta | None=None, secure: bool=False,
+			http_only: bool=False) -> None:
+		"""
 		adds a Set-Cookie header
 
 		:type expires: datetime.datetime
 		:param expires: if set to a value in the past, the cookie is deleted. if this and ``max_age`` are
 		  not set, the cookie becomes a session cookie.
 		:type max_age: datetime.timedelta
 		:param max_age: according to the spec, has precedence over expires. if you specify both, both are sent.
 		:param secure: controls when the browser sends the cookie back - unrelated to :func:`set_secure_cookie`
 
 		see `the docs <https://tools.ietf.org/html/rfc6265#section-4.1>`_ for an explanation of the other params
-		'''
+		"""
 		cookie = '%s=%s' % (key, self.simple_cookie.value_encode(value)[1])
 		if domain:
 			cookie += '; Domain=%s' % domain
 		if path:
 			cookie += '; Path=%s' % path
 		if expires:
-			expires = expires.strftime('%a, %d %b %Y %H:%M:%S GMT')
-			cookie += '; Expires=%s' % expires
+			cookie += '; Expires=%s' % expires.strftime('%a, %d %b %Y %H:%M:%S GMT')
 		if max_age is not None:
 			cookie += '; Max-Age=%d' % max_age.total_seconds()
 		if secure:
 			cookie += '; Secure'
 		if http_only:
 			cookie += '; HttpOnly'
 		self.headers.append(('Set-Cookie', cookie))
 
-	def set_secure_cookie(self, request, key, value, **kwargs):
-		'''
+	def set_secure_cookie(self, request: Request, key: str, value: typing.Any, **kwargs: typing.Any) -> None:
+		"""
 		this function accepts the same keyword arguments as :func:`.set_cookie` but stores a
 		timestamp and a signature based on ``request.app.cookie_secret``. decode with
 		:func:`Request.get_secure_cookie`.
 
 		the signature is a SHA-256 `hmac <https://docs.python.org/3/library/hmac.html>`_ of the
 		key, value, and timestamp. the value is *not* encrypted and is readable by the user, but is
 		signed and tamper-proof (assuming the ``cookie_secret`` is secure). because we store the
 		signing time, expiry is checked with ``get_secure_cookie``. you generally will want to pass
 		this function a ``max_age`` equal to ``max_time`` used when reading the cookie.
-		'''
+		"""
+		assert request.app.cookie_secret is not None
 		ts = int(time.time())
 		value_ts = '%s|%s' % (value, ts)
 		signature = _hash(key + '|' + value_ts, request.app.cookie_secret)
 		value_signed = '%s|%s' % (value_ts, signature)
 		self.set_cookie(key, value_signed, **kwargs)
 
 	@classmethod
-	def json(cls, obj):
-		'''
+	def json(cls, obj: typing.Any) -> Response:
+		"""
 		generate a streaming :class:`.Response` object from an object with an ``application/json``
 		content type. the default :attr:`.json_encoder` indents with tabs - override if you want
 		different indentation or need special encoding.
-		'''
+		"""
 		body = cls._gen_json(obj)
 		return Response(body, content_type='application/json; charset=utf-8')
 
 	@classmethod
-	def _gen_json(cls, obj):
-		'''
+	def _gen_json(cls, obj: typing.Any) -> typing.Iterator[bytes]:
+		"""
 		internal use generator for converting
 		`json.JSONEncoder.iterencode <https://docs.python.org/3/library/json.html#json.JSONEncoder.iterencode>`_
 		output to bytes
-		'''
+		"""
 		for chunk in cls.json_encoder.iterencode(obj):
 			yield chunk.encode('utf-8')
 
 	@classmethod
-	def render(cls, request, template, context):
-		'''
+	def render(cls, request: Request, template: str, context: dict[str, typing.Any]) -> 'Response':
+		"""
 		generate a streaming :class:`.Response` object from a template and a context with a
 		``text/html`` content type.
 
 		:type request: :class:`.Request`
 		:param request: the request to generate the response for
 		:type template: str
 		:param template: the template name to render, relative to ``request.app.template_dir``
 		:param context: if you used the default jinja2 template engine, this is a dict
 
-		'''
+		"""
 		body = request.app.template_engine.render(template, context)
 		response = cls(body, content_type='text/html; charset=utf-8')
 		return response
 
-def _hash(value_ts, cookie_secret):
+def _hash(value_ts: str, cookie_secret: bytes) -> str:
 	h = hmac.new(cookie_secret, value_ts.encode(), hashlib.sha256)
 	signature = h.hexdigest()
 	return signature
 
 class HTTPHeaders(UserDict): # inherit so that __init__ and fromkeys work (even though we never use them)
-	'''
+	"""
 	behaves like a regular :class:`dict` but
 	`casefolds <https://docs.python.org/3/library/stdtypes.html#str.casefold>`_ the keys
-	'''
+	"""
 
-	def __setitem__(self, key, value):
+	def __setitem__(self, key: str, value: str) -> None:
 		self.data[key.casefold()] = value
 
-	def __getitem__(self, key):
+	def __getitem__(self, key: str) -> str:
 		return self.data[key.casefold()]
```

### Comparing `pigwig-0.7.0/pigwig/routes.py` & `pigwig-0.8.0/pigwig/routes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-import textwrap
+from __future__ import annotations
+
 import re
+import textwrap
+from typing import Callable, Iterable, Sequence, Tuple
 
 from . import exceptions
 
 class RouteNode:
-	def __init__(self):
-		self.method_handlers = {}
-		self.static_children = {}
-		self.param_name = self.param_children = self.param_is_path = None
+	def __init__(self) -> None:
+		self.method_handlers: dict[str, Callable] = {}
+		self.static_children: dict[str, RouteNode] = {}
+		self.param_name: str | None = None
+		self.param_children: RouteNode | None = None
+		self.param_is_path: bool | None = None
 
 	param_re = re.compile(r'<([\w:]+)>')
-	def assign_route(self, path_elements, method, handler):
+	def assign_route(self, path_elements: Sequence[str], method: str, handler: Callable) -> None:
 		if not path_elements or path_elements[0] == '':
 			if len(path_elements) > 1:
 				raise Exception('cannot have consecutive / in routes')
 			if method in self.method_handlers:
 				raise exceptions.RouteConflict(method, handler)
 			self.method_handlers[method] = handler
 			return
@@ -30,23 +35,25 @@
 					self.param_is_path = True
 					self.param_name = self.param_name[5:]
 					remaining = []
 				else:
 					self.param_is_path = False
 			elif self.param_name != param.group(1):
 				raise exceptions.RouteConflict(method, handler)
+			else:
+				assert self.param_children is not None
 			child = self.param_children
 		else:
 			if element not in self.static_children:
 				self.static_children[element] = RouteNode()
 			child = self.static_children[element]
 
 		child.assign_route(remaining, method, handler)
 
-	def get_route(self, method, path_elements, params):
+	def get_route(self, method: str, path_elements: list[str], params: dict[str, str]) -> tuple[Callable, dict]:
 		if not path_elements or path_elements[0] == '':
 			handler = self.method_handlers.get(method)
 			if handler is not None:
 				return handler, params
 			elif self.method_handlers:
 				raise exceptions.HTTPException(405, 'method %s not allowed' % method)
 			else:
@@ -60,32 +67,35 @@
 				raise exceptions.HTTPException(404, 'route not found')
 			if self.param_is_path:
 				params[self.param_name] = '/'.join(path_elements)
 				remaining = []
 			else:
 				params[self.param_name] = element
 			child = self.param_children
+			assert child is not None
 		return child.get_route(method, remaining, params)
 
-	def route(self, method, path):
+	def route(self, method: str, path: str) -> tuple[Callable, dict]:
 		path_elements = path[1:].split('/')
 		return self.get_route(method, path_elements, {})
 
-	def __str__(self):
+	def __str__(self) -> str:
 		rval = []
 		for method, handler in self.method_handlers.items():
 			rval.append('%s: %s,' % (method, handler))
 		for element, node in self.static_children.items():
 			rval.append('%r: %s' % (element, node))
 		if self.param_name:
 			name = self.param_name
 			if self.param_is_path:
 				name += ' (path)'
 			rval.append('%s: %s' % (name, self.param_children))
 		return '{\n%s\n}' % textwrap.indent('\n'.join(rval), '\t')
 
-def build_route_tree(routes):
+RouteDefinition = Iterable[Tuple[str, str, Callable]]
+
+def build_route_tree(routes: RouteDefinition) -> RouteNode:
 	root_node = RouteNode()
 	for method, path, handler in routes:
 		path_elements = path[1:].split('/')
 		root_node.assign_route(path_elements, method, handler)
 	return root_node
```

