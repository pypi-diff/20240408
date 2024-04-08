# Comparing `tmp/robocorp_browser-2.3.2.tar.gz` & `tmp/robocorp_browser-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_browser-2.3.2.tar", max compression
+gzip compressed data, was "robocorp_browser-2.3.3.tar", max compression
```

## Comparing `robocorp_browser-2.3.2.tar` & `robocorp_browser-2.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     2927 2024-03-27 14:55:22.073294 robocorp_browser-2.3.2/README.md
--rw-r--r--   0        0        0      684 2024-03-27 14:55:22.073294 robocorp_browser-2.3.2/pyproject.toml
--rw-r--r--   0        0        0    10581 2024-03-27 14:55:22.073294 robocorp_browser-2.3.2/src/robocorp/browser/__init__.py
--rw-r--r--   0        0        0       81 2024-03-27 14:55:22.073294 robocorp_browser-2.3.2/src/robocorp/browser/__main__.py
--rw-r--r--   0        0        0     4849 2024-03-27 14:55:22.073294 robocorp_browser-2.3.2/src/robocorp/browser/_config.py
--rw-r--r--   0        0        0     8585 2024-03-27 14:55:22.073294 robocorp_browser-2.3.2/src/robocorp/browser/_context.py
--rw-r--r--   0        0        0     5308 2024-03-27 14:55:22.073294 robocorp_browser-2.3.2/src/robocorp/browser/_engines.py
--rw-r--r--   0        0        0      530 2024-03-27 14:55:22.073294 robocorp_browser-2.3.2/src/robocorp/browser/_types.py
--rw-r--r--   0        0        0     1538 2024-03-27 14:55:22.073294 robocorp_browser-2.3.2/src/robocorp/browser/cli.py
--rw-r--r--   0        0        0        0 2024-03-27 14:55:22.073294 robocorp_browser-2.3.2/src/robocorp/browser/py.typed
--rw-r--r--   0        0        0     3681 1970-01-01 00:00:00.000000 robocorp_browser-2.3.2/PKG-INFO
+-rwxr-xr-x   0        0        0     3122 2024-04-08 10:13:31.151422 robocorp_browser-2.3.3/README.md
+-rw-r--r--   0        0        0      719 2024-04-08 10:13:31.151422 robocorp_browser-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0    10570 2024-04-08 10:13:31.151422 robocorp_browser-2.3.3/src/robocorp/browser/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-08 10:13:31.151422 robocorp_browser-2.3.3/src/robocorp/browser/__main__.py
+-rw-r--r--   0        0        0     4849 2024-04-08 10:13:31.151422 robocorp_browser-2.3.3/src/robocorp/browser/_config.py
+-rw-r--r--   0        0        0     8585 2024-04-08 10:13:31.151422 robocorp_browser-2.3.3/src/robocorp/browser/_context.py
+-rw-r--r--   0        0        0     5308 2024-04-08 10:13:31.151422 robocorp_browser-2.3.3/src/robocorp/browser/_engines.py
+-rw-r--r--   0        0        0      530 2024-04-08 10:13:31.151422 robocorp_browser-2.3.3/src/robocorp/browser/_types.py
+-rw-r--r--   0        0        0     1538 2024-04-08 10:13:31.151422 robocorp_browser-2.3.3/src/robocorp/browser/cli.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:13:31.151422 robocorp_browser-2.3.3/src/robocorp/browser/py.typed
+-rw-r--r--   0        0        0     3876 1970-01-01 00:00:00.000000 robocorp_browser-2.3.3/PKG-INFO
```

### Comparing `robocorp_browser-2.3.2/README.md` & `robocorp_browser-2.3.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,71 @@
 # robocorp-browser
 
-The `robocorp-browser` is a wrapper for the [Playwright](https://playwright.dev/python/)
-project, with quality-of-life improvements such as automatic lifecycle management
-for Playwright objects (meant to be used with `robocorp-tasks`).
+The **robocorp-browser** package is a light wrapper for the [Playwright](https://playwright.dev/python/) -project, with quality-of-life improvements, such as automatic lifecycle management for Playwright objects (meant to be used with **robocorp-tasks**).
 
 ## Usage
 
-![`robocorp-browser`](https://img.shields.io/pypi/v/robocorp-browser?label=robocorp-browser)
-
-> 👉 Check that you have added the dependency in your configuration, this library is not apart of the `robocorp` -package.
-> - _conda.yaml_ for an automation [Task Packages](https://robocorp.com/docs/robot-structure)
-> - _action-package.yaml_ for an automation Action Packages
-> - _requirements.txt_, _pyproject.toml_ etc. for the rest
+[![`robocorp-browser`](https://img.shields.io/pypi/v/robocorp-browser?label=robocorp-browser)](https://pypi.org/project/robocorp-browser/)
 
+> 👉 Check that you have added the dependency in your configuration; this library is not part of the [**robocorp**](https://pypi.org/project/robocorp/) bundle.
+> - _conda.yaml_ for automation [Task Packages](https://robocorp.com/docs/robot-structure)
+> - _package.yaml_ for automation Action Packages
+> - _requirements.txt_, _pyproject.toml_, _setup.py|cfg_ etc. for the rest
 
 ```python
+from robocorp import browser, vault
 from robocorp.tasks import task
-from robocorp import browser
-from robocorp import vault
 
 @task
-def browser_automate():
-    # Configure may be used to set the basic robocorp.browser settings.
-    # It must be called prior to calling APIs which create playwright objects.
+def automate_browser():
+    """Start a browser to login in the surfed page."""
+    # The configuration is used to set the basic `robocorp.browser` settings.
+    # It must be called before calling APIs that create Playwright objects.
     browser.configure(
-        # Note: screenshot="only-on-failure" is actually the default.
-        # If the browser_automate() function finishes with an exception it will
-        # make a screenshot and embed it into the logs.
+        # NOTE: `screenshot="only-on-failure"` is the default.
+        # If this function finishes with an exception, it will make a screenshot and
+        #  embed it into the logs.
         screenshot="only-on-failure",
-        
-        # By default headless is False unless running in a Linux container
-        # without a DISPLAY/WAYLAND_DISPLAY environment variable, but it
-        # can also be manually specified.
-        headless=True,
-        
-        # Interactions may be run in slow-motion (given in milliseconds).
+
+        # By default, `headless` is False, unless running in a Linux container
+        #  without a DISPLAY/WAYLAND_DISPLAY environment variable, but it
+        #  can also be manually overridden.
+        headless=True,  # won't display the browser window
+
+        # Interactions may be run in slow motion (given in milliseconds).
         slowmo=100,
     )
 
-    # browser.goto() may be used as a shortcut to get the current page and
-    # go to some url (it may create the browser if still not created).
+    # The `browser.goto()` call may be used as a shortcut to get the current page and
+    #  surf some URL (it may create the browser if not created already).
     browser.goto("https://example.com>")
 
-    login()
+    _login()  # call the login instructions
 
 
-def login():
-    # APIs in robocorp.browser return the same browser instance, which is
-    # automatically closed when the task finishes.
+def _login():
+    # APIs in `robocorp.browser` return the same browser instance, which is
+    #  automatically closed when the task finishes.
     page = browser.page()
 
-    # robocorp.vault is recommended for managing secrets.
+    # `robocorp.vault` is recommended for managing secrets.
     account = vault.get_secret("default-account")
 
-    # Use the playwright Browser api as usual.
+    # Use the Playwright Browser API as usual to interact with the web elements.
     page.fill('//input[@ng-reflect-name="password"]', account["password"])
     page.click("input:text('Submit')")
 ```
 
-🚀 You can also [get started with our template](https://robocorp.com/portal/robot/robocorp/template-python-browser)
-
+🚀 Get started with our [template](https://robocorp.com/portal/robot/robocorp/template-python-browser) now!
 
 ## Guides
 
 - [Browser configuration](https://github.com/robocorp/robocorp/blob/master/browser/docs/guides/00-configuration.md)
 - [Persistent Context](https://github.com/robocorp/robocorp/blob/master/browser/docs/guides/01-persistent-context.md)
 
 ## API Reference
 
-Information on specific functions or classes: [robocorp.browser](https://github.com/robocorp/robocorp/blob/master/browser/docs/api/robocorp.browser.md)
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/browser/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
 A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/browser/docs/CHANGELOG.md).
```

### Comparing `robocorp_browser-2.3.2/pyproject.toml` & `robocorp_browser-2.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-browser"
-version = "2.3.2"
+version = "2.3.3"
 description = "Robocorp browser automation library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Cosmin P. <cosmin@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
@@ -24,7 +24,10 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 mypy_path = "src:tests"
+
+[tool.lazydocs]
+validate = "true"
```

### Comparing `robocorp_browser-2.3.2/src/robocorp/browser/__init__.py` & `robocorp_browser-2.3.3/src/robocorp/browser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Locator,
     Page,
     Playwright,
 )
 
 from ._types import BrowserEngine, BrowserNotFound, InstallError
 
-__version__ = "2.3.2"
+__version__ = "2.3.3"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def configure(**kwargs) -> None:
     """Configures browser settings before any other method is called.
 
     This method is optional, and if not invoked, default configurations will be used.
@@ -102,15 +102,15 @@
     """
     from . import _context
 
     browser_context_kwargs = _context.browser_context_kwargs()
     browser_context_kwargs.update(kwargs)
 
 
-def page(ceva="true") -> Page:
+def page() -> Page:
     """Provides a managed instance of the browser page to interact with.
 
     Example:
         ```python
         page = browser.page()
         page.goto("https://robotsparebinindustries.com/#/robot-order")
         page.click("button:text('OK')")
```

### Comparing `robocorp_browser-2.3.2/src/robocorp/browser/_config.py` & `robocorp_browser-2.3.3/src/robocorp/browser/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_browser-2.3.2/src/robocorp/browser/_context.py` & `robocorp_browser-2.3.3/src/robocorp/browser/_context.py`

 * *Files identical despite different names*

### Comparing `robocorp_browser-2.3.2/src/robocorp/browser/_engines.py` & `robocorp_browser-2.3.3/src/robocorp/browser/_engines.py`

 * *Files identical despite different names*

### Comparing `robocorp_browser-2.3.2/src/robocorp/browser/_types.py` & `robocorp_browser-2.3.3/src/robocorp/browser/_types.py`

 * *Files identical despite different names*

### Comparing `robocorp_browser-2.3.2/src/robocorp/browser/cli.py` & `robocorp_browser-2.3.3/src/robocorp/browser/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_browser-2.3.2/PKG-INFO` & `robocorp_browser-2.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-browser
-Version: 2.3.2
+Version: 2.3.3
 Summary: Robocorp browser automation library
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,81 +16,77 @@
 Requires-Dist: playwright (>=1.32.1,<2.0.0)
 Requires-Dist: robocorp-tasks (>=1,<4)
 Project-URL: Repository, https://github.com/robocorp/robocorp/
 Description-Content-Type: text/markdown
 
 # robocorp-browser
 
-The `robocorp-browser` is a wrapper for the [Playwright](https://playwright.dev/python/)
-project, with quality-of-life improvements such as automatic lifecycle management
-for Playwright objects (meant to be used with `robocorp-tasks`).
+The **robocorp-browser** package is a light wrapper for the [Playwright](https://playwright.dev/python/) -project, with quality-of-life improvements, such as automatic lifecycle management for Playwright objects (meant to be used with **robocorp-tasks**).
 
 ## Usage
 
-![`robocorp-browser`](https://img.shields.io/pypi/v/robocorp-browser?label=robocorp-browser)
-
-> 👉 Check that you have added the dependency in your configuration, this library is not apart of the `robocorp` -package.
-> - _conda.yaml_ for an automation [Task Packages](https://robocorp.com/docs/robot-structure)
-> - _action-package.yaml_ for an automation Action Packages
-> - _requirements.txt_, _pyproject.toml_ etc. for the rest
+[![`robocorp-browser`](https://img.shields.io/pypi/v/robocorp-browser?label=robocorp-browser)](https://pypi.org/project/robocorp-browser/)
 
+> 👉 Check that you have added the dependency in your configuration; this library is not part of the [**robocorp**](https://pypi.org/project/robocorp/) bundle.
+> - _conda.yaml_ for automation [Task Packages](https://robocorp.com/docs/robot-structure)
+> - _package.yaml_ for automation Action Packages
+> - _requirements.txt_, _pyproject.toml_, _setup.py|cfg_ etc. for the rest
 
 ```python
+from robocorp import browser, vault
 from robocorp.tasks import task
-from robocorp import browser
-from robocorp import vault
 
 @task
-def browser_automate():
-    # Configure may be used to set the basic robocorp.browser settings.
-    # It must be called prior to calling APIs which create playwright objects.
+def automate_browser():
+    """Start a browser to login in the surfed page."""
+    # The configuration is used to set the basic `robocorp.browser` settings.
+    # It must be called before calling APIs that create Playwright objects.
     browser.configure(
-        # Note: screenshot="only-on-failure" is actually the default.
-        # If the browser_automate() function finishes with an exception it will
-        # make a screenshot and embed it into the logs.
+        # NOTE: `screenshot="only-on-failure"` is the default.
+        # If this function finishes with an exception, it will make a screenshot and
+        #  embed it into the logs.
         screenshot="only-on-failure",
-        
-        # By default headless is False unless running in a Linux container
-        # without a DISPLAY/WAYLAND_DISPLAY environment variable, but it
-        # can also be manually specified.
-        headless=True,
-        
-        # Interactions may be run in slow-motion (given in milliseconds).
+
+        # By default, `headless` is False, unless running in a Linux container
+        #  without a DISPLAY/WAYLAND_DISPLAY environment variable, but it
+        #  can also be manually overridden.
+        headless=True,  # won't display the browser window
+
+        # Interactions may be run in slow motion (given in milliseconds).
         slowmo=100,
     )
 
-    # browser.goto() may be used as a shortcut to get the current page and
-    # go to some url (it may create the browser if still not created).
+    # The `browser.goto()` call may be used as a shortcut to get the current page and
+    #  surf some URL (it may create the browser if not created already).
     browser.goto("https://example.com>")
 
-    login()
+    _login()  # call the login instructions
 
 
-def login():
-    # APIs in robocorp.browser return the same browser instance, which is
-    # automatically closed when the task finishes.
+def _login():
+    # APIs in `robocorp.browser` return the same browser instance, which is
+    #  automatically closed when the task finishes.
     page = browser.page()
 
-    # robocorp.vault is recommended for managing secrets.
+    # `robocorp.vault` is recommended for managing secrets.
     account = vault.get_secret("default-account")
 
-    # Use the playwright Browser api as usual.
+    # Use the Playwright Browser API as usual to interact with the web elements.
     page.fill('//input[@ng-reflect-name="password"]', account["password"])
     page.click("input:text('Submit')")
 ```
 
-🚀 You can also [get started with our template](https://robocorp.com/portal/robot/robocorp/template-python-browser)
-
+🚀 Get started with our [template](https://robocorp.com/portal/robot/robocorp/template-python-browser) now!
 
 ## Guides
 
 - [Browser configuration](https://github.com/robocorp/robocorp/blob/master/browser/docs/guides/00-configuration.md)
 - [Persistent Context](https://github.com/robocorp/robocorp/blob/master/browser/docs/guides/01-persistent-context.md)
 
 ## API Reference
 
-Information on specific functions or classes: [robocorp.browser](https://github.com/robocorp/robocorp/blob/master/browser/docs/api/robocorp.browser.md)
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/browser/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
 A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/browser/docs/CHANGELOG.md).
```

