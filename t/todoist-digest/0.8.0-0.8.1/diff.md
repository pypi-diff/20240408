# Comparing `tmp/todoist_digest-0.8.0.tar.gz` & `tmp/todoist_digest-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todoist_digest-0.8.0.tar", max compression
+gzip compressed data, was "todoist_digest-0.8.1.tar", max compression
```

## Comparing `todoist_digest-0.8.0.tar` & `todoist_digest-0.8.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3001 2024-03-23 17:50:56.778671 todoist_digest-0.8.0/README.md
--rw-r--r--   0        0        0     1005 2024-03-23 17:51:26.586587 todoist_digest-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    14398 2024-03-23 17:50:56.778671 todoist_digest-0.8.0/todoist_digest/__init__.py
--rw-r--r--   0        0        0     1960 2024-03-23 17:50:56.778671 todoist_digest-0.8.0/todoist_digest/email.py
--rw-r--r--   0        0        0     1178 2024-03-23 17:50:56.778671 todoist_digest-0.8.0/todoist_digest/patch.py
--rw-r--r--   0        0        0     1661 2024-03-23 17:50:56.778671 todoist_digest-0.8.0/todoist_digest/todoist.py
--rw-r--r--   0        0        0     4033 1970-01-01 00:00:00.000000 todoist_digest-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     3592 2024-04-08 15:28:23.263448 todoist_digest-0.8.1/README.md
+-rw-r--r--   0        0        0     1006 2024-04-08 15:28:50.219475 todoist_digest-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    14398 2024-04-08 15:28:23.263448 todoist_digest-0.8.1/todoist_digest/__init__.py
+-rw-r--r--   0        0        0     1964 2024-04-08 15:28:23.263448 todoist_digest-0.8.1/todoist_digest/email.py
+-rw-r--r--   0        0        0     1411 2024-04-08 15:28:23.263448 todoist_digest-0.8.1/todoist_digest/patch.py
+-rw-r--r--   0        0        0     1661 2024-04-08 15:28:23.263448 todoist_digest-0.8.1/todoist_digest/todoist.py
+-rw-r--r--   0        0        0     4625 1970-01-01 00:00:00.000000 todoist_digest-0.8.1/PKG-INFO
```

### Comparing `todoist_digest-0.8.0/README.md` & `todoist_digest-0.8.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![Release Notes](https://img.shields.io/github/release/iloveitaly/todoist-digest)](https://github.com/iloveitaly/todoist-digest/releases) [![Downloads](https://static.pepy.tech/badge/todoist-digest/month)](https://pepy.tech/project/todoist-digest) [![Python Versions](https://img.shields.io/pypi/pyversions/todoist-digest)](https://pypi.org/project/todoist-digest) ![GitHub CI Status](https://github.com/iloveitaly/todoist-digest/actions/workflows/build_and_publish.yml/badge.svg) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 # Todoist Project Digest
 
 [Todoist](https://mikebian.co/todoist) doesn't have a way to generate a digest of all recent comments in a project created by a specific user. This makes it challenging to see what changed and what requires your action if you are collaborating with someone on a project.
 
 This is a simple project which generates a digest of all comments by a particular user on a particular project.
 
 This project was also a good excuse to play around and test some functional programming/data manipulation tooling I've been messing with ([funcy](https://github.com/Suor/funcy), [funcy-pipe](https://github.com/iloveitaly/funcy-pipe), and [whatever](https://github.com/Suor/whatever)).
```

### Comparing `todoist_digest-0.8.0/pyproject.toml` & `todoist_digest-0.8.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "todoist-digest"
-version = "0.8.0"
+version = "0.8.1"
 description = "Generate a digest of comments that occured since the last checked in date. Useful for including in an email."
 authors = ["Michael Bianco <mike@mikebian.co>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["todoist", "digest", "task", "management"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 todoist-api-python = "^2.1.3"
 click = "^8.1.7"
 pyjson5 = "^1.6.6"
-funcy-pipe = "^0.9.2"
+funcy-pipe = "^0.11.0"
 # funcy-pipe = { develop = true, path = "../../python/funcy-pipe" }
 python-dateutil = "^2.9.0.post0"
 backoff = "^2.2.1"
 markdown2 = "^2.4.13"
 whatever = "^0.7"
 apscheduler = "^3.10.4"
-css-inline = "^0.13.0"
+css-inline = "^0.14.0"
 jinja2 = "^3.1.3"
 
 [tool.poetry.group.dev.dependencies]
 isort = "5.11.5"
 black = "^24.3.0"
 pylint = "^3.1.0"
-pyright = "^1.1.355"
+pyright = "^1.1.357"
 mypy = "^1.9.0"
 
 [tool.isort]
 profile = "black"
 float_to_top = true
 
 [build-system]
```

### Comparing `todoist_digest-0.8.0/todoist_digest/__init__.py` & `todoist_digest-0.8.1/todoist_digest/__init__.py`

 * *Files identical despite different names*

### Comparing `todoist_digest-0.8.0/todoist_digest/email.py` & `todoist_digest-0.8.1/todoist_digest/email.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     msg = MIMEMultipart()
     msg["From"] = os.environ.get("EMAIL_FROM", parsed_url.username)
     msg["To"] = to_addresses
     msg["Subject"] = subject
 
     logger.info(
-        "creating email for %s, from %s, content length %i",
+        "creating email for '%s', from '%s', content length %i",
         to_addresses,
         parsed_url.username,
         len(markdown_content),
     )
 
     # this caused the html version to be ignored...
     # msg.attach(MIMEText(markdown_content, "plain"))
```

### Comparing `todoist_digest-0.8.0/todoist_digest/patch.py` & `todoist_digest-0.8.1/todoist_digest/patch.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,20 +17,24 @@
 
         setattr(
             todoist_api_python.http_requests,
             f"original_{target}",
             original_function,
         )
 
-        # raw response on 429
-        # b'{"error":"Too many requests. Limits reached. Try again later","error_code":35,"error_extra":{"event_id":"07c3fb965eaa4ec6a42e977c3e035c6b","retry_after":66},"error_tag":"LIMITS_REACHED","http_code":429}'
+        # raw response on 429:
+        #   b'{"error":"Too many requests. Limits reached. Try again later","error_code":35,"error_extra":{"event_id":"07c3fb965eaa4ec6a42e977c3e035c6b","retry_after":66},"error_tag":"LIMITS_REACHED","http_code":429}'
 
         # TODO pretty sure authorization errors are retried :/
         patched_function = backoff.on_exception(
-            backoff.expo, requests.exceptions.HTTPError, max_tries=30
+            backoff.expo,
+            # RequestException superclass is IOError, which is a low-level py error
+            # tried using HTTPError as the retry, but at scale the Todoist API has lots of interesting failures
+            (requests.exceptions.RequestException),
+            max_tries=30,
         )(original_function)
 
         setattr(
             todoist_api_python.http_requests,
             target,
             patched_function,
         )
```

### Comparing `todoist_digest-0.8.0/todoist_digest/todoist.py` & `todoist_digest-0.8.1/todoist_digest/todoist.py`

 * *Files identical despite different names*

### Comparing `todoist_digest-0.8.0/PKG-INFO` & `todoist_digest-0.8.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: todoist-digest
-Version: 0.8.0
+Version: 0.8.1
 Summary: Generate a digest of comments that occured since the last checked in date. Useful for including in an email.
 License: MIT
 Keywords: todoist,digest,task,management
 Author: Michael Bianco
 Author-email: mike@mikebian.co
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: apscheduler (>=3.10.4,<4.0.0)
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: css-inline (>=0.13.0,<0.14.0)
-Requires-Dist: funcy-pipe (>=0.9.2,<0.10.0)
+Requires-Dist: css-inline (>=0.14.0,<0.15.0)
+Requires-Dist: funcy-pipe (>=0.11.0,<0.12.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: markdown2 (>=2.4.13,<3.0.0)
 Requires-Dist: pyjson5 (>=1.6.6,<2.0.0)
 Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
 Requires-Dist: todoist-api-python (>=2.1.3,<3.0.0)
 Requires-Dist: whatever (>=0.7,<0.8)
 Description-Content-Type: text/markdown
 
+[![Release Notes](https://img.shields.io/github/release/iloveitaly/todoist-digest)](https://github.com/iloveitaly/todoist-digest/releases) [![Downloads](https://static.pepy.tech/badge/todoist-digest/month)](https://pepy.tech/project/todoist-digest) [![Python Versions](https://img.shields.io/pypi/pyversions/todoist-digest)](https://pypi.org/project/todoist-digest) ![GitHub CI Status](https://github.com/iloveitaly/todoist-digest/actions/workflows/build_and_publish.yml/badge.svg) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 # Todoist Project Digest
 
 [Todoist](https://mikebian.co/todoist) doesn't have a way to generate a digest of all recent comments in a project created by a specific user. This makes it challenging to see what changed and what requires your action if you are collaborating with someone on a project.
 
 This is a simple project which generates a digest of all comments by a particular user on a particular project.
 
 This project was also a good excuse to play around and test some functional programming/data manipulation tooling I've been messing with ([funcy](https://github.com/Suor/funcy), [funcy-pipe](https://github.com/iloveitaly/funcy-pipe), and [whatever](https://github.com/Suor/whatever)).
```

