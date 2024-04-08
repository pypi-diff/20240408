# Comparing `tmp/iamlistening-5.1.5.tar.gz` & `tmp/iamlistening-5.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-5.1.5.tar", max compression
+gzip compressed data, was "iamlistening-5.1.6.tar", max compression
```

## Comparing `iamlistening-5.1.5.tar` & `iamlistening-5.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2024-03-31 05:52:51.974350 iamlistening-5.1.5/LICENSE
--rw-r--r--   0        0        0     2467 2024-03-31 05:52:51.974350 iamlistening-5.1.5/README.md
--rw-r--r--   0        0        0      113 2024-03-31 05:53:27.162656 iamlistening-5.1.5/iamlistening/__init__.py
--rw-r--r--   0        0        0      443 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/config.py
--rw-r--r--   0        0        0     1824 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/default_settings.toml
--rw-r--r--   0        0        0      548 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/handler/__init__.py
--rw-r--r--   0        0        0     3438 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/handler/client.py
--rw-r--r--   0        0        0      790 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/handler/discord.py
--rw-r--r--   0        0        0      668 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/handler/guilded.py
--rw-r--r--   0        0        0      834 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/handler/lemmy.py
--rw-r--r--   0        0        0     1281 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/handler/mastodon.py
--rw-r--r--   0        0        0     1413 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/handler/matrix.py
--rw-r--r--   0        0        0      698 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/handler/revolt.py
--rw-r--r--   0        0        0      899 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/handler/telegram.py
--rw-r--r--   0        0        0      761 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/handler/twitch.py
--rw-r--r--   0        0        0     6600 2024-03-31 05:52:51.978350 iamlistening-5.1.5/iamlistening/main.py
--rw-r--r--   0        0        0     4021 2024-03-31 05:53:27.158656 iamlistening-5.1.5/pyproject.toml
--rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 iamlistening-5.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-08 09:21:27.264958 iamlistening-5.1.6/LICENSE
+-rw-r--r--   0        0        0     2467 2024-04-08 09:21:27.264958 iamlistening-5.1.6/README.md
+-rw-r--r--   0        0        0      113 2024-04-08 09:22:02.636500 iamlistening-5.1.6/iamlistening/__init__.py
+-rw-r--r--   0        0        0      443 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/config.py
+-rw-r--r--   0        0        0     1824 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0      548 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/handler/__init__.py
+-rw-r--r--   0        0        0     3439 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/handler/client.py
+-rw-r--r--   0        0        0      790 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/handler/discord.py
+-rw-r--r--   0        0        0      668 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/handler/guilded.py
+-rw-r--r--   0        0        0      834 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/handler/lemmy.py
+-rw-r--r--   0        0        0     1281 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/handler/mastodon.py
+-rw-r--r--   0        0        0     1413 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/handler/matrix.py
+-rw-r--r--   0        0        0      698 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/handler/revolt.py
+-rw-r--r--   0        0        0      899 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/handler/telegram.py
+-rw-r--r--   0        0        0      761 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/handler/twitch.py
+-rw-r--r--   0        0        0     6600 2024-04-08 09:21:27.268958 iamlistening-5.1.6/iamlistening/main.py
+-rw-r--r--   0        0        0     4023 2024-04-08 09:22:02.636500 iamlistening-5.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 iamlistening-5.1.6/PKG-INFO
```

### Comparing `iamlistening-5.1.5/LICENSE` & `iamlistening-5.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/README.md` & `iamlistening-5.1.6/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/iamlistening/default_settings.toml` & `iamlistening-5.1.6/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/iamlistening/handler/__init__.py` & `iamlistening-5.1.6/iamlistening/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/iamlistening/handler/client.py` & `iamlistening-5.1.6/iamlistening/handler/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
         Args:
             message_content (str): The content of the message.
         """
 
         if self.is_connected:
             self.latest_message = message_content
-            logger.debug("Frasier👂 on {}: {}", self.platform, message_content)
+            #logger.debug("Frasier👂 on {}: {}", self.platform, message_content)
             await self.handle_iteration_limit()
 
     async def handle_iteration_limit(self):
         """
         Handle the iteration limit logic.
 
         Returns:
```

### Comparing `iamlistening-5.1.5/iamlistening/handler/discord.py` & `iamlistening-5.1.6/iamlistening/handler/discord.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/iamlistening/handler/guilded.py` & `iamlistening-5.1.6/iamlistening/handler/guilded.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/iamlistening/handler/lemmy.py` & `iamlistening-5.1.6/iamlistening/handler/lemmy.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/iamlistening/handler/mastodon.py` & `iamlistening-5.1.6/iamlistening/handler/mastodon.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/iamlistening/handler/matrix.py` & `iamlistening-5.1.6/iamlistening/handler/matrix.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/iamlistening/handler/revolt.py` & `iamlistening-5.1.6/iamlistening/handler/revolt.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/iamlistening/handler/telegram.py` & `iamlistening-5.1.6/iamlistening/handler/telegram.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/iamlistening/handler/twitch.py` & `iamlistening-5.1.6/iamlistening/handler/twitch.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/iamlistening/main.py` & `iamlistening-5.1.6/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.5/pyproject.toml` & `iamlistening-5.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "5.1.5"
+version = "5.1.6"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix",
@@ -131,27 +131,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `iamlistening-5.1.5/PKG-INFO` & `iamlistening-5.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 5.1.5
+Version: 5.1.6
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 5.1.5 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 5.1.6 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: Mastodon.py (==1.8.1) Requires-Dist:
```

