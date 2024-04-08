# Comparing `tmp/flask_social_oauth-1.0.0.tar.gz` & `tmp/flask_social_oauth-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_social_oauth-1.0.0.tar", last modified: Sun Mar 31 16:54:11 2024, max compression
+gzip compressed data, was "flask_social_oauth-1.1.0.tar", last modified: Mon Apr  8 08:29:05 2024, max compression
```

## Comparing `flask_social_oauth-1.0.0.tar` & `flask_social_oauth-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:54:11.862271 flask_social_oauth-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-03-31 16:54:11.862271 flask_social_oauth-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-03-31 16:54:07.000000 flask_social_oauth-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-31 16:54:07.000000 flask_social_oauth-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 16:54:11.862271 flask_social_oauth-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:54:11.858271 flask_social_oauth-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:54:11.862271 flask_social_oauth-1.0.0/src/flask_social_oauth/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-03-31 16:54:07.000000 flask_social_oauth-1.0.0/src/flask_social_oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-03-31 16:54:07.000000 flask_social_oauth-1.0.0/src/flask_social_oauth/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    20465 2024-03-31 16:54:07.000000 flask_social_oauth-1.0.0/src/flask_social_oauth/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-31 16:54:07.000000 flask_social_oauth-1.0.0/src/flask_social_oauth/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:54:11.862271 flask_social_oauth-1.0.0/src/flask_social_oauth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-03-31 16:54:11.000000 flask_social_oauth-1.0.0/src/flask_social_oauth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-31 16:54:11.000000 flask_social_oauth-1.0.0/src/flask_social_oauth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 16:54:11.000000 flask_social_oauth-1.0.0/src/flask_social_oauth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-31 16:54:11.000000 flask_social_oauth-1.0.0/src/flask_social_oauth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-31 16:54:11.000000 flask_social_oauth-1.0.0/src/flask_social_oauth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:29:05.655982 flask_social_oauth-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-08 08:29:05.655982 flask_social_oauth-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-08 08:28:57.000000 flask_social_oauth-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-08 08:28:57.000000 flask_social_oauth-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 08:29:05.655982 flask_social_oauth-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:29:05.655982 flask_social_oauth-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:29:05.655982 flask_social_oauth-1.1.0/src/flask_social_oauth/
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-08 08:28:57.000000 flask_social_oauth-1.1.0/src/flask_social_oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-08 08:28:57.000000 flask_social_oauth-1.1.0/src/flask_social_oauth/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20465 2024-04-08 08:28:57.000000 flask_social_oauth-1.1.0/src/flask_social_oauth/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-08 08:28:57.000000 flask_social_oauth-1.1.0/src/flask_social_oauth/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:29:05.655982 flask_social_oauth-1.1.0/src/flask_social_oauth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-08 08:29:05.000000 flask_social_oauth-1.1.0/src/flask_social_oauth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 08:29:05.000000 flask_social_oauth-1.1.0/src/flask_social_oauth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:29:05.000000 flask_social_oauth-1.1.0/src/flask_social_oauth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 08:29:05.000000 flask_social_oauth-1.1.0/src/flask_social_oauth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 08:29:05.000000 flask_social_oauth-1.1.0/src/flask_social_oauth.egg-info/top_level.txt
```

### Comparing `flask_social_oauth-1.0.0/PKG-INFO` & `flask_social_oauth-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_social_oauth
-Version: 1.0.0
+Version: 1.1.0
 Summary: Flask Social Login is a Python package that simplifies the integration of social login functionality into Flask web applications. With support for popular social authentication providers like Google, GitHub, and Discord, Flask Social Login streamlines the authentication process for users and enables seamless access to your web application.
 Author-email: Om Mishra <hello@om-mishra.com>
 Project-URL: Homepage, https://docs.om-mishra.com/flask-social-oauth
 Project-URL: Issues, https://github.com/om-mishra7/flask-social-oauth/issues
 Project-URL: Repository, https://github.com/om-mishra7/flask-social-oauth
 Keywords: flask,social,auth,login,oauth,google,github,discord
 Requires-Python: >=3.1
```

### Comparing `flask_social_oauth-1.0.0/README.md` & `flask_social_oauth-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `flask_social_oauth-1.0.0/pyproject.toml` & `flask_social_oauth-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flask_social_oauth"
-version = "1.0.0"
+version = "1.1.0"
 authors = [{ name = "Om Mishra", email = "hello@om-mishra.com" }]
 description = "Flask Social Login is a Python package that simplifies the integration of social login functionality into Flask web applications. With support for popular social authentication providers like Google, GitHub, and Discord, Flask Social Login streamlines the authentication process for users and enables seamless access to your web application."
 readme = "README.md"
 requires-python = ">=3.1"
 dependencies = [
   "flask",
   "urllib3",
```

### Comparing `flask_social_oauth-1.0.0/src/flask_social_oauth/__init__.py` & `flask_social_oauth-1.1.0/src/flask_social_oauth/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from flask_social_auth.config import Config
-from flask_social_auth.helpers import sanitize_provider_name, validate_auth_config
+from flask_social_oauth.config import Config
+from flask_social_oauth.helpers import sanitize_provider_name, validate_auth_config
 
 
 def initialize_social_login(session, app, config):
     """
     Initialize social login for the Flask app using the provided configuration settings
 
     :param app: The Flask app
```

### Comparing `flask_social_oauth-1.0.0/src/flask_social_oauth/config.py` & `flask_social_oauth-1.1.0/src/flask_social_oauth/config.py`

 * *Files identical despite different names*

### Comparing `flask_social_oauth-1.0.0/src/flask_social_oauth/handlers.py` & `flask_social_oauth-1.1.0/src/flask_social_oauth/handlers.py`

 * *Files identical despite different names*

### Comparing `flask_social_oauth-1.0.0/src/flask_social_oauth/helpers.py` & `flask_social_oauth-1.1.0/src/flask_social_oauth/helpers.py`

 * *Files identical despite different names*

### Comparing `flask_social_oauth-1.0.0/src/flask_social_oauth.egg-info/PKG-INFO` & `flask_social_oauth-1.1.0/src/flask_social_oauth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_social_oauth
-Version: 1.0.0
+Version: 1.1.0
 Summary: Flask Social Login is a Python package that simplifies the integration of social login functionality into Flask web applications. With support for popular social authentication providers like Google, GitHub, and Discord, Flask Social Login streamlines the authentication process for users and enables seamless access to your web application.
 Author-email: Om Mishra <hello@om-mishra.com>
 Project-URL: Homepage, https://docs.om-mishra.com/flask-social-oauth
 Project-URL: Issues, https://github.com/om-mishra7/flask-social-oauth/issues
 Project-URL: Repository, https://github.com/om-mishra7/flask-social-oauth
 Keywords: flask,social,auth,login,oauth,google,github,discord
 Requires-Python: >=3.1
```

