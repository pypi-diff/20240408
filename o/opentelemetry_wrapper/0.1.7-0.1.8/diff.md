# Comparing `tmp/opentelemetry_wrapper-0.1.7.tar.gz` & `tmp/opentelemetry_wrapper-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_wrapper-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "opentelemetry_wrapper-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `opentelemetry_wrapper-0.1.7.tar` & `opentelemetry_wrapper-0.1.8.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0     2311 2022-12-13 07:19:54.176205 opentelemetry_wrapper-0.1.7/.gitignore
--rw-r--r--   0        0        0     9229 2022-12-13 07:19:54.177203 opentelemetry_wrapper-0.1.7/LICENSE
--rw-r--r--   0        0        0     6716 2024-03-13 01:20:38.192223 opentelemetry_wrapper-0.1.7/README.md
--rw-r--r--   0        0        0     3172 2024-03-13 07:50:04.007289 opentelemetry_wrapper-0.1.7/TODO.md
--rw-r--r--   0        0        0       60 2022-12-13 07:19:54.179199 opentelemetry_wrapper-0.1.7/aaaa/bbbb.py
--rw-r--r--   0        0        0     3197 2022-12-14 03:19:01.348649 opentelemetry_wrapper-0.1.7/experiment_otel_logging.py
--rw-r--r--   0        0        0     2487 2023-10-03 05:22:38.975631 opentelemetry_wrapper-0.1.7/fastapi_main.py
--rw-r--r--   0        0        0      320 2024-03-13 07:03:46.314493 opentelemetry_wrapper-0.1.7/log_weird_things.py
--rw-r--r--   0        0        0     1870 2024-03-13 08:56:32.415136 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/__init__.py
--rw-r--r--   0        0        0     3652 2023-06-05 02:58:25.364476 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/config/otel_exporter_otlp.py
--rw-r--r--   0        0        0     1260 2023-10-02 06:53:40.662583 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/config/otel_header_attributes.py
--rw-r--r--   0        0        0     2230 2022-12-15 07:50:47.979391 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/config/otel_headers.py
--rw-r--r--   0        0        0     1359 2022-12-13 07:19:54.183188 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/config/otel_log_level.py
--rw-r--r--   0        0        0     6154 2022-12-14 06:49:31.121402 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/config/otel_service_name.py
--rw-r--r--   0        0        0      270 2024-03-13 02:40:51.157859 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/fastapi/fastapi_typedef.py
--rw-r--r--   0        0        0     1262 2024-03-13 02:40:51.171798 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/fastapi/starlette_request_hook.py
--rw-r--r--   0        0        0     1310 2022-12-14 06:03:08.846216 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/instrument_dataclasses.py
--rw-r--r--   0        0        0     9376 2023-11-07 03:21:05.873899 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/instrument_decorator.py
--rw-r--r--   0        0        0     1844 2024-03-13 02:40:51.148884 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/instrument_fastapi.py
--rw-r--r--   0        0        0     6658 2024-03-13 08:52:59.572819 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/instrument_logging.py
--rw-r--r--   0        0        0      638 2022-12-14 06:03:08.959063 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/instrument_requests.py
--rw-r--r--   0        0        0     3388 2023-02-09 01:34:22.212343 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/instrument_sqlalchemy.py
--rw-r--r--   0        0        0      153 2022-12-14 03:26:52.894387 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/resource_detector.py
--rw-r--r--   0        0        0     2906 2024-03-13 08:55:59.891836 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/tracers.py
--rw-r--r--   0        0        0     1026 2024-03-13 02:40:51.165811 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/sqlalchemy/engine_typedef.py
--rw-r--r--   0        0        0     5371 2024-03-13 02:32:14.739659 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/utils/extract_json_header.py
--rw-r--r--   0        0        0    14882 2022-12-14 03:46:12.795251 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/utils/introspect.py
--rw-r--r--   0        0        0     4476 2022-12-14 03:09:31.646597 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/utils/json_encoder.py
--rw-r--r--   0        0        0     6575 2024-03-13 07:02:29.960397 opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/utils/logging_json_formatter.py
--rw-r--r--   0        0        0      931 2023-01-16 02:06:31.195899 opentelemetry_wrapper-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      364 2023-01-16 02:06:31.172959 opentelemetry_wrapper-0.1.7/requirements.txt
--rw-r--r--   0        0        0     1514 2022-12-15 09:33:55.784575 opentelemetry_wrapper-0.1.7/setup_otel_logging.py
--rw-r--r--   0        0        0     1016 2024-03-13 01:24:02.712219 opentelemetry_wrapper-0.1.7/sqlalchemy_example.py
--rw-r--r--   0        0        0     7523 1970-01-01 00:00:00.000000 opentelemetry_wrapper-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2311 2022-12-13 07:19:54.176205 opentelemetry_wrapper-0.1.8/.gitignore
+-rw-r--r--   0        0        0     9229 2022-12-13 07:19:54.177203 opentelemetry_wrapper-0.1.8/LICENSE
+-rw-r--r--   0        0        0     9233 2024-04-08 08:23:00.044355 opentelemetry_wrapper-0.1.8/README.md
+-rw-r--r--   0        0        0     3868 2024-04-08 10:04:05.057403 opentelemetry_wrapper-0.1.8/TODO.md
+-rw-r--r--   0        0        0       60 2022-12-13 07:19:54.179199 opentelemetry_wrapper-0.1.8/aaaa/bbbb.py
+-rw-r--r--   0        0        0     3264 2024-04-08 01:44:30.035164 opentelemetry_wrapper-0.1.8/experiment_otel_logging.py
+-rw-r--r--   0        0        0     2834 2024-04-08 10:31:54.524507 opentelemetry_wrapper-0.1.8/fastapi_main.py
+-rw-r--r--   0        0        0     1181 2024-04-05 09:25:30.071466 opentelemetry_wrapper-0.1.8/log_weird_things.py
+-rw-r--r--   0        0        0     2646 2024-04-05 08:52:10.474665 opentelemetry_wrapper-0.1.8/next_version_intended_usage.py
+-rw-r--r--   0        0        0     2093 2024-04-08 10:34:21.599201 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/__init__.py
+-rw-r--r--   0        0        0     3652 2023-06-05 02:58:25.364476 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_exporter_otlp.py
+-rw-r--r--   0        0        0     1260 2023-10-02 06:53:40.662583 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_header_attributes.py
+-rw-r--r--   0        0        0     2397 2024-04-08 10:00:58.967436 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_headers.py
+-rw-r--r--   0        0        0     1359 2022-12-13 07:19:54.183188 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_log_level.py
+-rw-r--r--   0        0        0     6154 2022-12-14 06:49:31.121402 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_service_name.py
+-rw-r--r--   0        0        0      507 2024-04-08 10:01:06.853687 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_wrapper_prometheus_exporter.py
+-rw-r--r--   0        0        0      270 2024-03-13 02:40:51.157859 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/fastapi/fastapi_typedef.py
+-rw-r--r--   0        0        0     1275 2024-04-08 10:12:38.034849 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/fastapi/starlette_request_hook.py
+-rw-r--r--   0        0        0     1310 2022-12-14 06:03:08.846216 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_dataclasses.py
+-rw-r--r--   0        0        0     9850 2024-04-05 10:17:45.422050 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_decorator.py
+-rw-r--r--   0        0        0     1908 2024-04-08 10:00:04.336638 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_fastapi.py
+-rw-r--r--   0        0        0     6271 2024-04-08 01:55:33.344141 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_logging.py
+-rw-r--r--   0        0        0      784 2024-03-13 09:44:08.327016 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_requests.py
+-rw-r--r--   0        0        0     3534 2024-03-13 09:44:08.280147 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_sqlalchemy.py
+-rw-r--r--   0        0        0     1811 2024-04-08 09:24:04.758627 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_system_metrics.py
+-rw-r--r--   0        0        0     6805 2024-04-08 10:23:45.979425 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/otel_providers.py
+-rw-r--r--   0        0        0      153 2022-12-14 03:26:52.894387 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/resource_detector.py
+-rw-r--r--   0        0        0     1031 2024-04-08 10:17:28.804459 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/sqlalchemy/engine_typedef.py
+-rw-r--r--   0        0        0     5363 2024-04-08 10:25:31.283954 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/extract_json_header.py
+-rw-r--r--   0        0        0    15005 2024-04-05 10:18:28.473240 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/introspect.py
+-rw-r--r--   0        0        0     5184 2024-04-08 10:28:14.050060 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/json_encoder.py
+-rw-r--r--   0        0        0     6575 2024-03-13 07:02:29.960397 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/logging_json_formatter.py
+-rw-r--r--   0        0        0     1069 2024-04-08 08:34:14.802204 opentelemetry_wrapper-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      445 2024-04-08 08:34:14.829047 opentelemetry_wrapper-0.1.8/requirements.txt
+-rw-r--r--   0        0        0     1639 2024-04-04 06:59:50.663250 opentelemetry_wrapper-0.1.8/setup_otel_logging.py
+-rw-r--r--   0        0        0     1016 2024-03-13 01:24:02.712219 opentelemetry_wrapper-0.1.8/sqlalchemy_example.py
+-rw-r--r--   0        0        0    10162 1970-01-01 00:00:00.000000 opentelemetry_wrapper-0.1.8/PKG-INFO
```

### Comparing `opentelemetry_wrapper-0.1.7/.gitignore` & `opentelemetry_wrapper-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.7/LICENSE` & `opentelemetry_wrapper-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.7/TODO.md` & `opentelemetry_wrapper-0.1.8/TODO.md`

 * *Files 12% similar despite different names*

```diff
@@ -35,36 +35,46 @@
     * `flit publish`
 * check that it can be downloaded/installed
     * `cd tmp`
     * `pip download opentelemetry_wrapper==X.Y.Z` <- replace with latest `__version__`
 
 ## todo
 
+* why is the fastapi instrumentor not outputting metrics? does it need to call observable metrics?
+  * consider doing whatever `prometheus-fastapi-instrumentator` is doing instead
 * documentation pls, including design decisions
+* rename `OTEL_EXPORTER_*` to `OTEL_COLLECTOR_*`
+  * and have separate metric, log, and trace collectors
+  * separate for http and grpc exporters too
+* env var to enable/disable console printing for logs, metrics (off by default), and traces
 * set `__tracebackhide__=True` (pytest) and `__traceback_hide__=True` (a few others like sentry) in the functions
 * update [introspect.py](./opentelemetry_wrapper/utils/introspect.py) for pep 626
     * The f_lineno attribute of frame objects will always contain the expected line number.
     * The co_lnotab attribute of code objects is deprecated and will be removed in 3.12.
     * Code that needs to convert from offset to line number should use the new co_lines() method instead.
 * `OTEL_HEADER_ATTRIBUTES` behaves too much like `OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_SERVER_REQUEST`
     * consider removing it?
 * `with ...` instrumentation for non-callable code (e.g. settings, semi-hardcoded config)
+  * see [next_version_intended_usage.py](./next_version_intended_usage.py)
 * type-checking decorator, with warning on unmatched types
     * https://github.com/prechelt/typecheck-decorator/blob/master/README.md
     * https://stackoverflow.com/questions/36879932/python-type-checking-decorator
     * https://towardsdatascience.com/the-power-of-decorators-fef4dc97020e
     * https://typeguard.readthedocs.io/en/latest/userguide.html
+    * or use `pydantic.TypeAdaptor` to manually check
 * correctly handle generators and context managers (and async versions of them)
 * instrument pydantic?
-* support metrics somehow
+* validate support for metrics
     * the asgi/fastapi already supports some metrics
     * https://github.com/instana/python-sensor/blob/master/instana/autoprofile/samplers
         * memory profiling
         * reading frames to make a statistical guess how much time is spent in each function
     * https://psutil.readthedocs.io/en/latest/
     * Request Error Duration metrics can be calculated from spans
+* also add a prometheus endpoint for scraping?
 * builtin `tracemalloc` can be used locate the source file and line number of a function, if started early enough
     * check for the [`PYTHONTRACEMALLOC`](https://docs.python.org/3/using/cmdline.html#envvar-PYTHONTRACEMALLOC) var?
-* somehow mark function as do-not-instrument, for extremely spammy functions? or specify a sampling ratio?
+* somehow mark functions/endpoints as do-not-instrument, for extremely spammy functions? or specify a sampling ratio?
+  * the nearest sampling ratio should overwrite, but idk how to do that
 * add a (regex-based?) sanitizer to erase strings/patterns from log output
 * print config at startup? at least print the version?
     * or maybe print a json string with all the (non-sensitive) config?
```

### Comparing `opentelemetry_wrapper-0.1.7/experiment_otel_logging.py` & `opentelemetry_wrapper-0.1.8/experiment_otel_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import logging
 import time
+from functools import lru_cache
 
 from asgiref.sync import async_to_sync
 from asgiref.sync import sync_to_async
 
 from opentelemetry_wrapper import instrument_decorate
 from opentelemetry_wrapper import instrument_logging
 
@@ -30,14 +31,16 @@
         return x >> -shift_by
     else:
         logging.debug(f'bit-shifting {x=} by 0')
         return x
 
 
 @instrument_decorate
+@lru_cache
+@instrument_decorate
 async def multiply(multiplier: int, multiplicand: int):
     """
     very silly way to multiply things inspired by exponentiation-by-squaring
     constrained to only use the `bitshift` function and addition
     """
     await asyncio.sleep(0.01)
```

### Comparing `opentelemetry_wrapper-0.1.7/fastapi_main.py` & `opentelemetry_wrapper-0.1.8/fastapi_main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import datetime
 import inspect
 import logging
+import os
 from typing import Callable
 
 import requests
 import uvicorn
 from fastapi import FastAPI
 from fastapi import Request
 from fastapi import status
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.middleware.gzip import GZipMiddleware
 from fastapi.responses import RedirectResponse
 from starlette.middleware.sessions import SessionMiddleware
 
 from opentelemetry_wrapper import instrument_all
+from opentelemetry_wrapper.dependencies.opentelemetry.instrument_fastapi import instrument_fastapi_app
 
 instrument_all()
 
-app = FastAPI(title='My Super Project',
-              description='This is a very fancy project, with auto docs for the API and everything',
-              version='2.5.0',  # only semver makes sense here
-              )
+app = instrument_fastapi_app(FastAPI(title='My Super Project',
+                                     description='This is a very fancy project, with docs for the API and everything',
+                                     version='2.5.0',  # only semver makes sense here
+                                     ))
 
 app.add_middleware(GZipMiddleware, minimum_size=1000)
 app.add_middleware(SessionMiddleware, secret_key='config.settings.secret_key')
 app.add_middleware(CORSMiddleware,
                    allow_origins=['*'],
                    allow_credentials=True,
                    allow_methods=['*'],
@@ -62,16 +64,18 @@
     logging.info('called `hello-hello`')
     r = requests.get('http://localhost:8000/hello/hello')
     logging.info(f'`hello` returned {r.text}')
     return r.text
 
 
 if __name__ == '__main__':
+    os.environ['OTEL_EXPORTER_PROMETHEUS_PORT'] = '9464'
     uvicorn.run(f'{inspect.getmodulename(__file__)}:app',
                 host='localhost',
                 port=8000,
                 # reload=True,
                 access_log=True,
                 workers=2,  # not valid with reload=True
                 # proxy_headers=True,  # github.com/encode/uvicorn/blob/master/uvicorn/middleware/proxy_headers.py
                 limit_concurrency=128,
+                # log_config=None, # this tells uvicorn not to set up its own logger
                 )
```

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/__init__.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """
 a wrapper around `opentelemetry` and `opentelemetry-instrumentation-*` to make life a bit easier
 """
 
-__version__ = '0.1.7'
+__version__ = '0.1.8'
 
 from opentelemetry_wrapper.config.otel_headers import OTEL_WRAPPER_DISABLED
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_dataclasses import instrument_dataclasses
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_decorator import instrument_decorate
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_fastapi import instrument_fastapi
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_fastapi import instrument_fastapi_app
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_logging import instrument_logging
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_requests import instrument_requests
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_sqlalchemy import instrument_sqlalchemy
+from opentelemetry_wrapper.dependencies.opentelemetry.instrument_system_metrics import instrument_system_metrics
 
 
 @instrument_decorate
 def instrument_all(dataclasses: bool = True,
                    logging: bool = True,
                    fastapi: bool = True,
                    requests: bool = True,
                    sqlalchemy: bool = False,  # too noisy for a default
                    log_json: bool = True,
+                   system_metrics: bool = True
                    ):
     # no-op
     if OTEL_WRAPPER_DISABLED:
         return
 
     if dataclasses:
         instrument_dataclasses()
@@ -32,14 +34,16 @@
         instrument_logging(print_json=log_json)
     if fastapi:
         instrument_fastapi()
     if requests:
         instrument_requests()
     if sqlalchemy:
         instrument_sqlalchemy()
+    if system_metrics:
+        instrument_system_metrics()
 
 
 __all__ = (
     '__version__',
     'instrument_all',
     'instrument_decorate',
     'instrument_dataclasses',
```

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/config/otel_exporter_otlp.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_exporter_otlp.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/config/otel_header_attributes.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_header_attributes.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/config/otel_headers.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_headers.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from opentelemetry_wrapper.config.otel_exporter_otlp import getenv_otel_exporter_otlp_insecure
 from opentelemetry_wrapper.config.otel_header_attributes import get_header_attributes
 from opentelemetry_wrapper.config.otel_log_level import get_log_level
 from opentelemetry_wrapper.config.otel_service_name import get_default_service_name
 from opentelemetry_wrapper.config.otel_service_name import get_k8s_namespace
 from opentelemetry_wrapper.config.otel_service_name import getenv_otel_service_name
 from opentelemetry_wrapper.config.otel_service_name import getenv_otel_service_namespace
+from opentelemetry_wrapper.config.otel_wrapper_prometheus_exporter import get_prometheus_port
 
 # global flag to override opentelemetry and not do anything
 # because opentelemetry is too verbose in tests
 # naming / terminology based on:
 # https://opentelemetry.io/docs/reference/specification/sdk-environment-variables/#:~:text=OTEL_SDK_DISABLED
 OTEL_WRAPPER_DISABLED: bool = os.getenv('OTEL_WRAPPER_DISABLED', 'false').casefold().strip() == 'true'
 
@@ -32,7 +33,9 @@
 OTEL_EXPORTER_OTLP_ENDPOINT: str = getenv_otel_exporter_otlp_endpoint()
 OTEL_EXPORTER_OTLP_HEADER: Tuple[Tuple[str, str], ...] = getenv_otel_exporter_otlp_header()
 OTEL_EXPORTER_OTLP_INSECURE: Optional[bool] = getenv_otel_exporter_otlp_insecure()
 
 OTEL_LOG_LEVEL: int = get_log_level()
 
 OTEL_HEADER_ATTRIBUTES: List[str] = get_header_attributes()
+
+OTEL_EXPORTER_PROMETHEUS_PORT: Optional[int] = get_prometheus_port()
```

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/config/otel_log_level.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_log_level.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/config/otel_service_name.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_service_name.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/fastapi/starlette_request_hook.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/fastapi/starlette_request_hook.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,9 +24,9 @@
                     span.set_attribute(f'{header_name}.{k}', v)
                 continue
 
             # all other headers
             if isinstance(header_value, (bool, str, bytes, int, float)):
                 span.set_attribute(header_name, header_value)
 except ImportError:
-    def request_hook(_, __) -> None:
+    def request_hook(_: Span, __: Scope) -> None:
         return
```

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/instrument_dataclasses.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_dataclasses.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/instrument_decorator.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import Status
 from opentelemetry.trace import StatusCode
 
 from opentelemetry_wrapper import __version__  # don't worry, this does not create an infinite import loop
 from opentelemetry_wrapper.config.otel_headers import OTEL_WRAPPER_DISABLED
-from opentelemetry_wrapper.dependencies.opentelemetry.tracers import get_tracer
+from opentelemetry_wrapper.dependencies.opentelemetry.otel_providers import get_tracer
 from opentelemetry_wrapper.utils.introspect import CodeInfo
 
-_TRACER = get_tracer(__name__, __version__)
+_TRACER = get_tracer(__name__, __version__)  # TODO: move this somewhere else
 
 InstrumentableThing = TypeVar('InstrumentableThing', Callable, Coroutine, type)
 
 _CACHE_INSTRUMENTED: Dict[InstrumentableThing, Optional[InstrumentableThing]] = dict()  # type: ignore[valid-type]
 _CACHE_GETATTRIBUTE: Dict[InstrumentableThing, InstrumentableThing] = dict()  # type: ignore[valid-type]
 
 
@@ -63,14 +63,25 @@
             return ret
         return func
 
     # if not provided, try to find the function name
     code_info = CodeInfo(func)
     func_name = func_name or code_info.name
 
+    # avoid re-instrumenting functions with wrappers (e.g., lru_cache)
+    # note: this only works if the base function is instrumented
+    # todo: peel back one layer at a time and check if its instrumented
+    # noinspection PyBroadException
+    try:
+        # noinspection PyProtectedMember
+        if code_info._unwrapped_code_object in _CACHE_INSTRUMENTED:
+            return func
+    except Exception:
+        pass
+
     # build span attributes for this class / function / method / builtin / etc
     span_attributes: Dict[str, Union[str, None, int]] = dict()
     if code_info.function_name:
         span_attributes[SpanAttributes.CODE_FUNCTION] = code_info.function_name
     if code_info.module_name:
         span_attributes[SpanAttributes.CODE_NAMESPACE] = code_info.module_name
     if code_info.path:
```

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/instrument_fastapi.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_fastapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-from typing import TypeVar
-
 from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
 
 from opentelemetry_wrapper.config.otel_headers import OTEL_WRAPPER_DISABLED
 from opentelemetry_wrapper.dependencies.fastapi.fastapi_typedef import is_fastapi_app
 from opentelemetry_wrapper.dependencies.fastapi.starlette_request_hook import request_hook
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_decorator import instrument_decorate
-
-FastApiType = TypeVar('FastApiType', bound=type)
+from opentelemetry_wrapper.dependencies.opentelemetry.otel_providers import init_meter_provider
 
 
 @instrument_decorate
 def instrument_fastapi_app(app):
     """
     instrument a FastAPI app
     also instruments logging and requests (if `requests` exists)
@@ -26,14 +23,17 @@
     if not is_fastapi_app(app):
         return app
 
     # avoid double instrumentation
     if getattr(app, '_is_instrumented_by_opentelemetry', None):
         return app
 
+    # init metrics
+    init_meter_provider()
+
     # instrument the app
     FastAPIInstrumentor.instrument_app(app,
                                        server_request_hook=request_hook,
                                        client_request_hook=request_hook,
                                        )
     return app
```

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/instrument_logging.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_logging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,40 @@
 import logging
 import sys
 from functools import lru_cache
 from functools import update_wrapper
 from functools import wraps
 from pathlib import Path
+from typing import Dict
+from typing import List
 from typing import Optional
 from typing import Set
 from typing import TextIO
+from typing import Tuple
 
-from opentelemetry.exporter.otlp.proto.grpc._log_exporter import OTLPLogExporter
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
-from opentelemetry.sdk._logs import LoggerProvider
-from opentelemetry.sdk._logs import LoggingHandler
-from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
-from opentelemetry.sdk.resources import Resource
-from opentelemetry.sdk.resources import SERVICE_NAME
-from opentelemetry.sdk.resources import SERVICE_NAMESPACE
 
 from opentelemetry_wrapper.config.otel_headers import OTEL_EXPORTER_OTLP_ENDPOINT
-from opentelemetry_wrapper.config.otel_headers import OTEL_EXPORTER_OTLP_HEADER
-from opentelemetry_wrapper.config.otel_headers import OTEL_EXPORTER_OTLP_INSECURE
 from opentelemetry_wrapper.config.otel_headers import OTEL_LOG_LEVEL
-from opentelemetry_wrapper.config.otel_headers import OTEL_SERVICE_NAME
-from opentelemetry_wrapper.config.otel_headers import OTEL_SERVICE_NAMESPACE
 from opentelemetry_wrapper.config.otel_headers import OTEL_WRAPPER_DISABLED
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_decorator import instrument_decorate
+from opentelemetry_wrapper.dependencies.opentelemetry.otel_providers import get_otel_log_handler
 from opentelemetry_wrapper.utils.logging_json_formatter import JsonFormatter
 
-# write IDs as 0xBEEF instead of BEEF, so it matches the trace json exactly
 LOGGING_FORMAT_VERBOSE = (
     '%(asctime)s '
     '%(levelname)-8s '
     '[%(name)s] '
     '[%(filename)s:%(funcName)s:%(lineno)d] '
-    '[trace_id=0x%(otelTraceID)s span_id=0x%(otelSpanID)s resource.service.name=%(otelServiceName)s] '
+    '[trace_id=%(otelTraceID)s span_id=%(otelSpanID)s resource.service.name=%(otelServiceName)s] '
     '- %(message)s'
 )
 
-_CURRENT_ROOT_JSON_HANDLERS: Set[logging.Handler] = set()
-
-
-@lru_cache  # only run once
-def get_otel_log_handler(*,
-                         level: int = OTEL_LOG_LEVEL,
-                         ) -> LoggingHandler:
-    if OTEL_SERVICE_NAMESPACE:
-        lp = LoggerProvider(resource=Resource.create({SERVICE_NAME:      OTEL_SERVICE_NAME,
-                                                      SERVICE_NAMESPACE: OTEL_SERVICE_NAMESPACE}))
-    else:
-        lp = LoggerProvider(resource=Resource.create({SERVICE_NAME: OTEL_SERVICE_NAME}))
-
-    if OTEL_EXPORTER_OTLP_ENDPOINT:
-        lp.add_log_record_processor(BatchLogRecordProcessor(OTLPLogExporter(endpoint=OTEL_EXPORTER_OTLP_ENDPOINT,
-                                                                            headers=OTEL_EXPORTER_OTLP_HEADER,
-                                                                            insecure=OTEL_EXPORTER_OTLP_INSECURE)))
-
-    return LoggingHandler(level=level, logger_provider=lp)
+_OUR_ROOT_HANDLERS: Set[logging.Handler] = set()
+_CLOBBERED_ROOT_HANDLERS: Dict[str, Tuple[List[logging.Handler], bool]] = dict()
 
 
 @lru_cache  # avoid creating duplicate handlers
 def get_json_handler(*,
                      level: int = OTEL_LOG_LEVEL,
                      path: Optional[Path] = None,
                      stream: Optional[TextIO] = None,
@@ -76,88 +51,113 @@
         handler = logging.StreamHandler(stream=sys.stderr)
 
     handler.setFormatter(JsonFormatter())
     handler.setLevel(level)
     return handler
 
 
+def uninstrument_logging():
+    # un-instrument from OTEL
+    _instrumentor = LoggingInstrumentor()  # this is a singleton, so it'll return the same object
+    if _instrumentor.is_instrumented_by_opentelemetry:
+        _instrumentor.uninstrument()
+
+    # un-clobber the handlers
+    for logger_name, (handlers, propagate) in _CLOBBERED_ROOT_HANDLERS.items():
+        logging.getLogger(logger_name).handlers = handlers
+        logging.getLogger(logger_name).propagate = propagate
+    _CLOBBERED_ROOT_HANDLERS.clear()
+
+    # un-instrument logging root handler
+    while _OUR_ROOT_HANDLERS:
+        # noinspection PyBroadException
+        try:
+            logging.root.removeHandler(_OUR_ROOT_HANDLERS.pop())
+        except Exception:
+            continue
+
+
 @instrument_decorate
 def instrument_logging(*,
                        level: int = OTEL_LOG_LEVEL,
                        path: Optional[Path] = None,
                        stream: Optional[TextIO] = None,
                        print_json: bool = True,
+                       clobber_other_log_handlers: bool = False,
                        ) -> None:
     """
     this function is (by default) idempotent; calling it multiple times has no additional side effects
 
     :param level:
     :param path:
     :param stream:
     :param print_json:
+    :param clobber_other_log_handlers: drop all other log handlers created by anyone else
     :return:
     """
-    global _CURRENT_ROOT_JSON_HANDLERS
-
     # no-op
     if OTEL_WRAPPER_DISABLED:
         return
 
-    _instrumentor = LoggingInstrumentor()
-    if _instrumentor.is_instrumented_by_opentelemetry:
-        _instrumentor.uninstrument()
-    _instrumentor.instrument(set_logging_format=False)
+    uninstrument_logging()
+
+    LoggingInstrumentor().instrument(set_logging_format=False)
     old_factory = logging.getLogRecordFactory()
 
     # the instrumentor failed to use the @wraps decorator so let's do it for them
     # noinspection PyProtectedMember
     if LoggingInstrumentor._old_factory is not None:
         # noinspection PyProtectedMember
         update_wrapper(old_factory, LoggingInstrumentor._old_factory)
 
     @wraps(old_factory)
     def record_factory(*args, **kwargs):
         record = old_factory(*args, **kwargs)
 
-        # we want the trace-id and span-id in a log to match the span it was created in
-        # therefore we format it to match
+        # we want the trace-id and span-id in a log to match the span it was created in;
+        # therefore, we format it to match (span_id: `0x09f8e31e775ec22e` instead of `9f8e31e775ec22e`)
         # note that logs outside a span will be assigned an invalid trace-id and span-id (all zeroes)
+        # TODO: this could skip the int cast and instead just left-pad and lowercase
         record.otelTraceID = f'0x{int(record.otelTraceID, 16):032x}'
         record.otelSpanID = f'0x{int(record.otelSpanID, 16):016x}'
 
         return record
 
     logging.setLogRecordFactory(record_factory)
 
-    # un-instrument logging root handler
-    while _CURRENT_ROOT_JSON_HANDLERS:
-        logging.root.removeHandler(_CURRENT_ROOT_JSON_HANDLERS.pop())
-
     # output as json
     if print_json:
         if path is not None:
-            _CURRENT_ROOT_JSON_HANDLERS.add(get_json_handler(level=level, path=path))
+            _OUR_ROOT_HANDLERS.add(get_json_handler(level=level, path=path))
         if stream is not None or path is None:
-            _CURRENT_ROOT_JSON_HANDLERS.add(get_json_handler(level=level, stream=stream))
+            _OUR_ROOT_HANDLERS.add(get_json_handler(level=level, stream=stream))
 
     # output as text, using the templated logging string format
     else:
         # equivalent to logging.basicConfig(format=..., level=level)
         _formatter = logging.Formatter(fmt=LOGGING_FORMAT_VERBOSE)
 
         if path is not None:
             _file_handler = logging.FileHandler(path)
             _file_handler.setFormatter(_formatter)
-            _CURRENT_ROOT_JSON_HANDLERS.add(_file_handler)
+            _OUR_ROOT_HANDLERS.add(_file_handler)
         if stream is not None or path is None:
             _stream_handler = logging.StreamHandler(stream)
             _stream_handler.setFormatter(_formatter)
-            _CURRENT_ROOT_JSON_HANDLERS.add(_stream_handler)
+            _OUR_ROOT_HANDLERS.add(_stream_handler)
 
     # add an otel log exporter too
     if OTEL_EXPORTER_OTLP_ENDPOINT:
-        _CURRENT_ROOT_JSON_HANDLERS.add(get_otel_log_handler(level=level))
+        _OUR_ROOT_HANDLERS.add(get_otel_log_handler(level=level))
 
     # set root handlers
-    for _handler in _CURRENT_ROOT_JSON_HANDLERS:
+    for _handler in _OUR_ROOT_HANDLERS:
         logging.root.addHandler(_handler)
     logging.root.setLevel(level)
+
+    # clobber all other handlers
+    if clobber_other_log_handlers:
+        for logger_name, logger in logging.root.manager.loggerDict.items():
+            if not isinstance(logger, logging.PlaceHolder):
+                _CLOBBERED_ROOT_HANDLERS[logger_name] = (logger.handlers, logger.propagate)
+                logger.handlers = []
+                logger.propagate = True
```

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/opentelemetry/instrument_sqlalchemy.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_sqlalchemy.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TypeVar
 
 from opentelemetry.instrumentation.sqlalchemy import EngineTracer
 from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
 
 from opentelemetry_wrapper import instrument_decorate
 from opentelemetry_wrapper.config.otel_headers import OTEL_WRAPPER_DISABLED
+from opentelemetry_wrapper.dependencies.opentelemetry.otel_providers import init_meter_provider
 from opentelemetry_wrapper.dependencies.sqlalchemy.engine_typedef import is_sqlalchemy_async_engine
 from opentelemetry_wrapper.dependencies.sqlalchemy.engine_typedef import is_sqlalchemy_engine
 from opentelemetry_wrapper.dependencies.sqlalchemy.engine_typedef import is_sqlalchemy_sync_engine
 
 SqlAlchemyEngineType = TypeVar('SqlAlchemyEngineType', bound=type)
 
 _CACHE_INSTRUMENTED: Dict[int, EngineTracer] = dict()
@@ -76,10 +77,13 @@
     this function is idempotent; calling it multiple times has no additional side effects
     """
 
     # no-op
     if OTEL_WRAPPER_DISABLED:
         return
 
+    # init metrics
+    init_meter_provider()
+
     _instrumentor = SQLAlchemyInstrumentor()  # assume this is a singleton
     if not _instrumentor.is_instrumented_by_opentelemetry:
         _instrumentor.instrument()
```

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/dependencies/sqlalchemy/engine_typedef.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/sqlalchemy/engine_typedef.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def is_sqlalchemy_async_engine(item: Any) -> bool:  # noqa: E303
         # noinspection PyTypeHints
         return isinstance(item, AsyncEngine)
 
 except ImportError:
     # noinspection PyUnusedLocal
-    def is_sqlalchemy_engine(_) -> bool:
+    def is_sqlalchemy_engine(_: Any) -> bool:
         return False
 
 
     # noqa: E303
     LegacyEngine = Any  # type: ignore[assignment,misc]
     AsyncEngine = Any  # type: ignore[assignment,misc]
     FutureEngine = Any  # type: ignore[assignment,misc]
```

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/utils/extract_json_header.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/extract_json_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 
-def extract_json_header(header_value: str) -> Optional[Dict[str, Union[bool, str, bytes, int, float]]]:
+def extract_json_header(header_value: Optional[str]) -> Optional[Dict[str, Union[bool, str, int, float]]]:
     """
     extract JSON as a flat dict from a (possibly base64-encoded) string
 
     :param header_value:
     :return:
     """
     # does not extract keys where the value is None
@@ -46,15 +46,15 @@
         pass
 
     # didn't extract anything
     return None
 
 
 @lru_cache(maxsize=0x10000)
-def _extract_userinfo(header_value: str) -> Optional[Dict[str, Union[bool, str, bytes, int, float]]]:
+def _extract_userinfo(header_value: str) -> Optional[Dict[str, Union[bool, str, int, float]]]:
     """
     extract the oauth userinfo token into a flat dict
     if the provided value is not base64-encoded json, returns None
 
     this function is cached because the userinfo token (almost) never changes
     since the userinfo token is injected by the api gateway there shouldn't be cache-busting dos attacks
 
@@ -71,16 +71,16 @@
         return None
     except json.decoder.JSONDecodeError:
         return None
 
     return _flatten_json(_header_value)
 
 
-def _flatten_json(header_value: Union[Dict, List, bool, str, int, float],
-                  ) -> Optional[Dict[str, Union[bool, str, int, float]]]:
+def _flatten_json(header_value: Union[Dict, List, bool, str, int, float, None],
+                  ) -> Dict[str, Union[bool, str, int, float]]:
     """
         parses a json string and flattens it into an un-nested dictionary, dropping null values
         >>> _flatten_json({'a': {'aa': {'aaa': 'AAA'}, 'x': None}, 'b': [1, 2, 3]})
         {'a.aa.aaa': 'AAA', 'b.[0]': 1, 'b.[1]': 2, 'b.[2]': 3}
         >>> _flatten_json(['x', None, {1: 11, 2: 22}, 'y'])
         {'[0]': 'x', '[2].1': 11, '[2].2': 22, '[3]': 'y'}
```

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/utils/introspect.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/introspect.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 
 # noinspection PyBroadException
 @lru_cache(maxsize=None)
 @dataclass(unsafe_hash=True, frozen=True)
 class CodeInfo:
     code_object: Union[Coroutine, Callable,
-                       partial, partialmethod, singledispatchmethod, cached_property,
-                       asyncio.Task,
-                       type, property]
+    partial, partialmethod, singledispatchmethod, cached_property,
+    asyncio.Task,
+    type, property]
 
     unwrap_partial: bool = True
     unwrap_async: bool = True
 
     _maybe_unsafe__try_very_hard_to_find_class: bool = True
 
     __cached_cls: List[type] = field(default_factory=list, init=False, repr=False, hash=False, compare=False)
@@ -56,15 +56,15 @@
 
     @cached_property
     def is_class(self) -> bool:
         """
         is the unwrapped base object a class?
         """
         try:
-            return inspect.isclass(self.__unwrapped_code_object)
+            return inspect.isclass(self._unwrapped_code_object)
         except Exception:
             return False
 
     @cached_property
     def name(self) -> str:
         try:
             _prefixes = ' '.join(self.__unwrapped_prefixes) + ' ' if self.__unwrapped_prefixes else ''
@@ -86,36 +86,36 @@
             return f'{_prefixes}{_module_name}{_class_name}{_function_name}'
         except Exception:
             return '<unknown class>' if self.is_class else '<unknown function>'
 
     @cached_property
     def __code__(self):
         # get the code stuff
-        _code = getattr(self.__unwrapped_code_object, '__code__', None)
+        _code = getattr(self._unwrapped_code_object, '__code__', None)
 
         # asyncio.Task stores it here
         if _code is None:
-            _code = getattr(self.__unwrapped_code_object, 'cr_code', None)
+            _code = getattr(self._unwrapped_code_object, 'cr_code', None)
 
         # sometimes it's in __func__.__code__
         if _code is None:
-            _code = getattr(getattr(self.__unwrapped_code_object, '__func__', None), '__code__', None)
+            _code = getattr(getattr(self._unwrapped_code_object, '__func__', None), '__code__', None)
 
         return _code
 
     @cached_property
     def function_qualname(self) -> Optional[str]:
         try:
             # a class does not have a function name
             if self.is_class:
                 return None
 
             # use qualname instead of name if possible, but strip out the class name
-            if hasattr(self.__unwrapped_code_object, '__qualname__'):
-                return self.__unwrapped_code_object.__qualname__
+            if hasattr(self._unwrapped_code_object, '__qualname__'):
+                return self._unwrapped_code_object.__qualname__
         except Exception:
             pass
 
         return None
 
     @cached_property
     def function_name(self) -> Optional[str]:
@@ -131,30 +131,30 @@
                     if _function_name.startswith(f'{self.class_name}.'):
                         _function_name = _function_name[len(self.class_name) + 1:]
                     elif f'.{self.class_name}.' in _function_name:
                         _function_name = _function_name.split(f'.{self.class_name}.', 1)[1]
                 return _function_name
 
             # fallback to name
-            if getattr(self.__unwrapped_code_object, '__name__', None):
-                return self.__unwrapped_code_object.__name__
+            if getattr(self._unwrapped_code_object, '__name__', None):
+                return self._unwrapped_code_object.__name__
 
             # use the code name
             if self.__code__ is not None:
                 if getattr(self.__code__, 'co_name', None):
                     return self.__code__.co_name
         except Exception:
             pass
 
         return None
 
     @cached_property
     def module(self) -> Optional[ModuleType]:
         try:
-            return inspect.getmodule(self.__unwrapped_code_object)
+            return inspect.getmodule(self._unwrapped_code_object)
         except Exception:
             return None
 
     @cached_property
     def module_name(self) -> Optional[str]:
         try:
             if self.module is not None:
@@ -172,31 +172,31 @@
         return None
 
     @cached_property
     def cls(self) -> Optional[type]:
         try:
             # if we already are a class
             if self.is_class:
-                return self.__unwrapped_code_object
+                return self._unwrapped_code_object
 
             # get class of method
-            if inspect.ismethod(self.__unwrapped_code_object) or \
-                    (inspect.isbuiltin(self.__unwrapped_code_object) and
-                     hasattr(self.__unwrapped_code_object, '__self__')):
+            if inspect.ismethod(self._unwrapped_code_object) or \
+                    (inspect.isbuiltin(self._unwrapped_code_object) and
+                     hasattr(self._unwrapped_code_object, '__self__')):
                 for _attr_name in ('__class__', '__slots__'):
-                    _attr = getattr(self.__unwrapped_code_object.__self__, _attr_name, None)
+                    _attr = getattr(self._unwrapped_code_object.__self__, _attr_name, None)
                     if _attr is not None and hasattr(_attr, '__mro__'):
                         for _mro_cls in inspect.getmro(_attr):
                             if inspect.isclass(_mro_cls):
-                                if self.__unwrapped_code_object.__name__ in _mro_cls.__dict__:
+                                if self._unwrapped_code_object.__name__ in _mro_cls.__dict__:
                                     return _mro_cls
 
             # get class qualname
-            if hasattr(self.__unwrapped_code_object, '__qualname__'):
-                _cls_qualname = self.__unwrapped_code_object.__qualname__.split('.<locals>')[0]
+            if hasattr(self._unwrapped_code_object, '__qualname__'):
+                _cls_qualname = self._unwrapped_code_object.__qualname__.split('.<locals>')[0]
                 if '.' in _cls_qualname:
                     _cls_qualname = _cls_qualname.rsplit('.', 1)[0]
                 else:
                     _cls_qualname = ''
             else:
                 _cls_qualname = ''
 
@@ -210,15 +210,15 @@
                     _cls = getattr(_cls, _cls_name, None)
                 else:
                     if _cls is not None:
                         if inspect.isclass(_cls):
                             return _cls
 
             # one more place to try
-            _cls = getattr(self.__unwrapped_code_object, '__objclass__', None)
+            _cls = getattr(self._unwrapped_code_object, '__objclass__', None)
             if _cls is not None:
                 if inspect.isclass(_cls):
                     return _cls
 
             # try harder: load module from path and search inside it to find the class qualname
             if self._maybe_unsafe__try_very_hard_to_find_class and _cls_qualname and not self.module and self.path:
                 _temp_module_name = f'__introspected_file__.{self.path}'
@@ -255,15 +255,15 @@
 
         return None
 
     @cached_property
     def path(self) -> Optional[Path]:
         try:
             try:
-                _source_file = inspect.getsourcefile(self.__unwrapped_code_object)
+                _source_file = inspect.getsourcefile(self._unwrapped_code_object)
                 if _source_file:
                     return Path(_source_file)
             except TypeError:
                 pass
 
             if self.__code__ is not None:
                 if getattr(self.__code__, 'co_filename', None):
@@ -273,15 +273,15 @@
 
         return None
 
     @cached_property
     def lineno(self) -> Optional[int]:
         try:
             try:
-                _source_lines = inspect.getsourcelines(self.__unwrapped_code_object)
+                _source_lines = inspect.getsourcelines(self._unwrapped_code_object)
                 if _source_lines:
                     return _source_lines[1]
             except (TypeError, OSError):
                 pass
 
             if self.__code__ is not None:
                 if getattr(self.__code__, 'co_firstlineno', None):
@@ -300,14 +300,16 @@
         if isinstance(code_object, asyncio.Task):
             return True
 
         return False
 
     @cached_property
     def __unwrapped(self):
+        # todo: provide a way to get at all the layers, so that i can check whether any of them are instrumented
+        # this should probably be externalized and yield all the layers one at a time
         _code_object = self.code_object
         _prefixes = []
 
         # unwrap recursively
         while True:
 
             # handle wrappers from functools
@@ -374,13 +376,13 @@
         return _prefixes, _code_object
 
     @property
     def __unwrapped_prefixes(self) -> List[str]:
         return self.__unwrapped[0]
 
     @property
-    def __unwrapped_code_object(self):
+    def _unwrapped_code_object(self):
         """
         it is unsafe to expose this externally!
         the potential side effects (or lack thereof) of calling an unwrapped function are undefined
         """
         return self.__unwrapped[1]
```

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/utils/json_encoder.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/json_encoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,17 +24,26 @@
 try:
     fastapi_jsonable_encoder: Optional[Callable]
     from fastapi.encoders import jsonable_encoder as fastapi_jsonable_encoder
 except ImportError:
     fastapi_jsonable_encoder = None
 
 try:
+    pydantic_jsonable_encoder: Optional[Callable]
+    from pydantic.v1.json import pydantic_encoder as pydantic_jsonable_encoder
+except ImportError:
+    try:
+        from pydantic_core import to_jsonable_python as pydantic_jsonable_encoder
+    except ImportError:
+        pydantic_jsonable_encoder = None
+
+try:
     PYDANTIC_ENCODERS: Dict[Type, Callable]
     # noinspection PyProtectedMember
-    from pydantic.json import ENCODERS_BY_TYPE as PYDANTIC_ENCODERS
+    from pydantic.v1.json import ENCODERS_BY_TYPE as PYDANTIC_ENCODERS
 except ImportError:
     PYDANTIC_ENCODERS = dict()
 
 
 def parse_datetime(o: datetime.date) -> str:
     return o.isoformat()
 
@@ -44,15 +53,19 @@
 
 
 def parse_timedelta(o: datetime.timedelta) -> float:
     return o.total_seconds()
 
 
 def parse_decimal(o: Decimal) -> Union[int, float]:
-    return int(o) if o.as_tuple().exponent >= 0 else float(o)
+    _exp = o.as_tuple().exponent  # can be an int or Literal["n", "N", "F"]
+    if isinstance(_exp, int):
+        return int(o) if _exp >= 0 else float(o)
+    else:
+        return float(o)
 
 
 def parse_enum(o: Enum) -> Any:
     return o.value
 
 
 def parse_pattern(o: Pattern) -> str:
@@ -96,14 +109,22 @@
 
 
 def jsonable_encoder(obj: Any) -> Any:
     # hand off to the fastapi encoder if we have it
     if fastapi_jsonable_encoder is not None:
         return fastapi_jsonable_encoder(obj, custom_encoder=ENCODERS_BY_TYPE)
 
+    # hand off to the pydantic encoder if we have it
+    if pydantic_jsonable_encoder is not None:
+        # noinspection PyBroadException
+        try:
+            return pydantic_jsonable_encoder(obj)
+        except Exception:
+            pass
+
     # extremely simplified version of the fastapi jsonable_encoder
     if dataclasses.is_dataclass(obj):
         return dataclasses.asdict(obj)
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, PurePath):
         return str(obj)
```

### Comparing `opentelemetry_wrapper-0.1.7/opentelemetry_wrapper/utils/logging_json_formatter.py` & `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/logging_json_formatter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.7/pyproject.toml` & `opentelemetry_wrapper-0.1.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -14,20 +14,24 @@
 # NOTE: also update requirements.txt
 dependencies = [
     "asgiref",
     "fastapi",
     "itsdangerous",
     "opentelemetry-api",
     "opentelemetry-exporter-otlp",
+    "opentelemetry-exporter-prometheus",
     "opentelemetry-instrumentation-fastapi",
     "opentelemetry-instrumentation-logging",
     "opentelemetry-instrumentation-requests",
     "opentelemetry-instrumentation-sqlalchemy",
+    "opentelemetry-instrumentation-system-metrics",
     "opentelemetry-sdk",
+    "pydantic",
     "requests",
     "sqlalchemy",
+    "sqlalchemy2-stubs",
     "starlette",
     "uvicorn",
 ]
 
 [project.urls]
 Home = "https://github.com/averykhoo/opentelemetry_wrapper"
```

### Comparing `opentelemetry_wrapper-0.1.7/setup_otel_logging.py` & `opentelemetry_wrapper-0.1.8/setup_otel_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,7 +64,12 @@
     A().b()
     A().c()()
     A()()
     A().__class__
     A().e
     A().e
     A().x
+
+    a = instrument_decorate(A)()
+    a_c = instrument_decorate(a.c)
+    a_c_d = instrument_decorate(a_c())
+    a_c_d()
```

### Comparing `opentelemetry_wrapper-0.1.7/sqlalchemy_example.py` & `opentelemetry_wrapper-0.1.8/sqlalchemy_example.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.7/PKG-INFO` & `opentelemetry_wrapper-0.1.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,96 @@
 Metadata-Version: 2.1
 Name: opentelemetry_wrapper
-Version: 0.1.7
+Version: 0.1.8
 Summary: a wrapper around `opentelemetry` and `opentelemetry-instrumentation-*` to make life a bit easier
 Author-email: Avery Khoo <averykhoo@gmail.com>
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: asgiref
 Requires-Dist: fastapi
 Requires-Dist: itsdangerous
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-exporter-otlp
+Requires-Dist: opentelemetry-exporter-prometheus
 Requires-Dist: opentelemetry-instrumentation-fastapi
 Requires-Dist: opentelemetry-instrumentation-logging
 Requires-Dist: opentelemetry-instrumentation-requests
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy
+Requires-Dist: opentelemetry-instrumentation-system-metrics
 Requires-Dist: opentelemetry-sdk
+Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: sqlalchemy
+Requires-Dist: sqlalchemy2-stubs
 Requires-Dist: starlette
 Requires-Dist: uvicorn
 Project-URL: Home, https://github.com/averykhoo/opentelemetry_wrapper
 
 # opentelemetry_wrapper
 
 a wrapper around `opentelemetry` and `opentelemetry-instrumentation-*` to make life a bit easier
 
-## what this does (or is supposed to do)
+## design principles
 
-* Make instrumentation (more) idempotent
-* Make re-instrumentation of logging actually work with different format strings
-* Make `logging` print as a one-line JSON dict by default
-* Provide support for decorating functions and classes
-* Provide support for instrumentation of dataclasses
-    * Global instrumentation needs to be run *before* any dataclasses are initialized
-    * Otherwise, use the decorator on each class as usual (it's idempotent anyway)
-* Add global instrumentation of FastAPI
-    * sometimes works even after apps are created for some reason, likely due to how Uvicorn runs in a new process
-    * but somehow sometimes doesn't work in prod, for equally unknown reasons
-    * probably best to instrument each app instance
-* Logs (some) http headers received by fastapi as span attributes
-* Creates OTLP exporter if specific env vars (below) are set
+### safe
+
+* **never crash the application**
+    * fallback to non-`opentelemetry` if necessary
+    * ignore input over raising an exception
+    * possible exception: it may be better to fail at startup than to run with known bad config
+        * https://opentelemetry.io/docs/specs/otel/error-handling/#basic-error-handling-principles
+* **hard to get wrong**
+    * idempotent, even when you instrument the same thing in different ways from different places
+    * "be conservative in what you send, be liberal in what you accept"
+    * note: easy and simple mean different things
+
+### unsurprising
+
+* **simple, idiomatic, succinct, and pretty**
+    * decorators over wrappers
+    * wrappers over context managers
+    * context mangers over ~~manually managing spans~~ anything else *(note: this is still a todo)*
+* **reasonable documented defaults**
+    * magic may be hard to understand, but it's better than being irritating
+* **emits zero logs/spans (of its own) at runtime**
+    * fail silently over flailing noisily
+    * drowning out real logs can be worse than being useless (e.g., you could crash `fluentd` - ask me how I know)
+
+### helpful
+
+* **machine-readable first, human-readable a close second**
+    * no newlines in logs or spans
+    * no whitespace-delimited ambiguity
+    * json all the things (within reason)
+* **provide all available application context**
+    * we want to know all we can about what's going on and where
+    * code introspection and runtime analysis if we can make it fast enough
 
 ## usage
 
 > **TL;DR:** <br>
-> 1. call `instrument_all()` to instrument logging and requests
-> 2. instrument your FastAPI app using `instrument_fastapi_app(...)`
+> 1. call `instrument_all()` to instrument `logging` and `requests`
+> 2. instrument your FastAPI app using `instrument_fastapi_app(FastAPI(...))`
 > 3. use `@instrument_decorate` on any function or class you want to monitor
 > 4. set `OTEL_WRAPPER_DISABLED=true` in your CICD tests, especially if you're using `pytest`
 
 ### env vars
 
-| Variable Name                 | Description                                                                                                                                       | Default (if not set)                                                                        |
-|-------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
-| `OTEL_EXPORTER_OTLP_ENDPOINT` | Looks like `http://tempo.localhost:4317`.                                                                                                         | *NA* (traces are not exported to any OTLP endpoint)                                         |
-| `OTEL_EXPORTER_OTLP_HEADER`   | Looks like `Header-Name=header value`, where values can contain space ('\x20'). To insert multiple headers, delimit by any other whitespace char. | *NA* (no header sent to OTLP endpoint)                                                      |
-| `OTEL_EXPORTER_OTLP_INSECURE` | Set to `true` to disable SSL for OTLP trace exports, or `false` to always verify.                                                                 | *NA* (follows OpenTelemetry default, which is secure for https and insecure for http)       |
-| `OTEL_HEADER_ATTRIBUTES`      | List of HTTP headers to extract from incoming requests as span attributes, split by whitespace.                                                   | x-pf-number, x-client-id, x-preferred-username, x-resource-access                           |
-| `OTEL_LOG_LEVEL`              | Log level used by the logging instrumentor (case-insensitive).                                                                                    | `info`                                                                                      |
-| `OTEL_SERVICE_NAME`           | Sets the value of the `service.name` resource attribute.                                                                                          | f'{k8s namespace}/{k8s pod name}' or f'{username}@{hostname}.{domain}:<{filename of main}>' |
-| `OTEL_SERVICE_NAMESPACE`      | Sets the value of the `service.namespace` resource attribute.                                                                                     | f'{k8s namespace}' or None                                                                  |
-| `OTEL_WRAPPER_DISABLED`       | Set to `true` to disable tracing globally (e.g. when running pytest).                                                                             | `false` (tracing is enabled)                                                                |
+| Variable Name                   | Description                                                                                                                                       | Default (if not set)                                                                        |
+|---------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
+| `OTEL_EXPORTER_OTLP_ENDPOINT`   | Looks like `http://tempo.localhost:4317`.                                                                                                         | *NA* (traces are not exported to any OTLP endpoint)                                         |
+| `OTEL_EXPORTER_OTLP_HEADER`     | Looks like `Header-Name=header value`, where values can contain space ('\x20'). To insert multiple headers, delimit by any other whitespace char. | *NA* (no header sent to OTLP endpoint)                                                      |
+| `OTEL_EXPORTER_OTLP_INSECURE`   | Set to `true` to disable SSL for OTLP trace exports, or `false` to always verify.                                                                 | *NA* (follows OpenTelemetry default, which is secure for https and insecure for http)       |
+| `OTEL_EXPORTER_PROMETHEUS_PORT` | The port on which to expose methics for Prometheus. (E.g. `9464` to expose `http://localhost:9464/metrics`)                                       | *NA* (follows OpenTelemetry default, which is secure for https and insecure for http)       |
+| `OTEL_HEADER_ATTRIBUTES`        | List of HTTP headers to extract from incoming requests as span attributes, split by whitespace.                                                   | x-pf-number, x-client-id, x-preferred-username, x-resource-access                           |
+| `OTEL_LOG_LEVEL`                | Log level used by the logging instrumentor (case-insensitive).                                                                                    | `info`                                                                                      |
+| `OTEL_SERVICE_NAME`             | Sets the value of the `service.name` resource attribute.                                                                                          | f'{k8s namespace}/{k8s pod name}' or f'{username}@{hostname}.{domain}:<{filename of main}>' |
+| `OTEL_SERVICE_NAMESPACE`        | Sets the value of the `service.namespace` resource attribute.                                                                                     | f'{k8s namespace}' or None                                                                  |
+| `OTEL_WRAPPER_DISABLED`         | Set to `true` to disable tracing globally (e.g. when running pytest).                                                                             | `false` (tracing is enabled)                                                                |
 
 > **Note:** <br>
 > The `service.name` and `service.namespace` can also be set via `OTEL_RESOURCE_ATTRIBUTES`, but any settings there
 > will be overwritten by `OTEL_SERVICE_NAME` and `OTEL_SERVICE_NAMESPACE`. For more details, read the
 > original [OpenTelemetry docs](https://opentelemetry.io/docs)
 
 ### `@instrument_decorate` decorator for functions and classes
@@ -126,7 +151,30 @@
 
 ```python
 from fastapi import FastAPI
 from opentelemetry_wrapper import instrument_fastapi_app
 
 app = instrument_fastapi_app(FastAPI(...))
 ```
+
+## features
+
+* Make instrumentation (more) idempotent:
+    * you can call the instrument functions unlimited times from multiple places in your codebase, and it'll work the
+      same
+    * e.g., a class definition, a defined method of the class, a class instance, and a method from the instance
+* Make re-instrumentation of `logging` actually work when passing in a new format string
+* Make `logging` print as a one-line JSON dict by default, with a lot of magic to convert stuff to valid json
+* logs and spans contain info about which thread / process and which file / function / line of code it came from
+    * and the k8s namespace and pod, if applicable, otherwise the local pc name
+* Provide support for decorating functions and classes
+* Provide support for instrumentation of dataclasses
+    * NOTE: Global instrumentation needs to be run *before* any dataclasses are initialized
+    * Otherwise, use the decorator on each class as usual (since it is idempotent anyway)
+* Add global instrumentation of FastAPI
+    * sometimes works even after apps are created for some reason, likely due to how Uvicorn runs in a new process
+    * but somehow sometimes doesn't work in prod, for equally unknown reasons
+    * probably best to instrument each app instance
+* Logs OIDC http headers as span attributes for FastAPI
+* Creates OTLP exporters if specific env vars (below) are set
+    * Pushes logs, metrics, and traces to the OTEL endpoint, if configured
+    * Note: only logs and traces are printed to console, metrics are too noisy
```

