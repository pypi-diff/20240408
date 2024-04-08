# Comparing `tmp/twikit-1.4.4.tar.gz` & `tmp/twikit-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.4.4.tar", last modified: Sat Apr  6 04:32:09 2024, max compression
+gzip compressed data, was "twikit-1.4.5.tar", last modified: Mon Apr  8 13:30:34 2024, max compression
```

## Comparing `twikit-1.4.4.tar` & `twikit-1.4.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 04:32:09.805292 twikit-1.4.4/
--rw-rw-rw-   0        0        0     1079 2024-03-23 06:08:25.000000 twikit-1.4.4/LICENSE
--rw-rw-rw-   0        0        0     3534 2024-04-06 04:32:09.802303 twikit-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     3264 2024-03-23 06:08:25.000000 twikit-1.4.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 04:32:09.805292 twikit-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      693 2024-03-28 12:25:18.000000 twikit-1.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 04:32:09.731489 twikit-1.4.4/twikit/
--rw-rw-rw-   0        0        0      601 2024-04-06 04:32:07.000000 twikit-1.4.4/twikit/__init__.py
--rw-rw-rw-   0        0        0   107913 2024-04-05 18:02:49.000000 twikit-1.4.4/twikit/client.py
--rw-rw-rw-   0        0        0     2380 2024-04-06 04:29:07.000000 twikit-1.4.4/twikit/errors.py
--rw-rw-rw-   0        0        0     6983 2024-04-02 02:28:49.000000 twikit-1.4.4/twikit/group.py
--rw-rw-rw-   0        0        0     1913 2024-04-06 04:28:27.000000 twikit-1.4.4/twikit/http.py
--rw-rw-rw-   0        0        0     7399 2024-04-02 02:28:12.000000 twikit-1.4.4/twikit/list.py
--rw-rw-rw-   0        0        0     3800 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/message.py
--rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/notification.py
--rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/trend.py
--rw-rw-rw-   0        0        0    16644 2024-04-02 02:26:56.000000 twikit-1.4.4/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-06 04:32:09.798312 twikit-1.4.4/twikit/twikit_async/
--rw-rw-rw-   0        0        0      553 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0   111344 2024-04-05 01:04:43.000000 twikit-1.4.4/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0      875 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7177 2024-04-02 02:30:57.000000 twikit-1.4.4/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     1955 2024-04-06 04:28:33.000000 twikit-1.4.4/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7562 2024-04-02 02:30:39.000000 twikit-1.4.4/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3866 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    16751 2024-04-02 02:29:48.000000 twikit-1.4.4/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14128 2024-04-02 02:29:20.000000 twikit-1.4.4/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3354 2024-04-02 05:30:54.000000 twikit-1.4.4/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    13905 2024-04-02 02:27:48.000000 twikit-1.4.4/twikit/user.py
--rw-rw-rw-   0        0        0    20911 2024-04-05 01:12:40.000000 twikit-1.4.4/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 04:32:09.749442 twikit-1.4.4/twikit.egg-info/
--rw-rw-rw-   0        0        0     3534 2024-04-06 04:32:09.000000 twikit-1.4.4/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2024-04-06 04:32:09.000000 twikit-1.4.4/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 04:32:09.000000 twikit-1.4.4/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-06 04:32:09.000000 twikit-1.4.4/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-06 04:32:09.000000 twikit-1.4.4/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 13:30:34.266087 twikit-1.4.5/
+-rw-rw-rw-   0        0        0     1079 2024-04-06 11:03:16.000000 twikit-1.4.5/LICENSE
+-rw-rw-rw-   0        0        0     3873 2024-04-08 13:30:34.263094 twikit-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3600 2024-04-08 12:57:20.000000 twikit-1.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 13:30:34.266087 twikit-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-04-08 07:44:57.000000 twikit-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:30:34.189291 twikit-1.4.5/twikit/
+-rw-rw-rw-   0        0        0      454 2024-04-08 08:23:50.000000 twikit-1.4.5/twikit/__init__.py
+-rw-rw-rw-   0        0        0   109445 2024-04-08 13:06:22.000000 twikit-1.4.5/twikit/client.py
+-rw-rw-rw-   0        0        0     2380 2024-04-06 04:29:07.000000 twikit-1.4.5/twikit/errors.py
+-rw-rw-rw-   0        0        0     7199 2024-04-08 13:02:51.000000 twikit-1.4.5/twikit/group.py
+-rw-rw-rw-   0        0        0     1913 2024-04-06 04:28:27.000000 twikit-1.4.5/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-04-08 13:03:12.000000 twikit-1.4.5/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-04-06 13:37:31.000000 twikit-1.4.5/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-06 13:37:50.000000 twikit-1.4.5/twikit/notification.py
+-rw-rw-rw-   0        0        0     1070 2024-04-08 13:03:49.000000 twikit-1.4.5/twikit/trend.py
+-rw-rw-rw-   0        0        0    17146 2024-04-08 13:04:49.000000 twikit-1.4.5/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:30:34.259106 twikit-1.4.5/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      406 2024-04-08 08:23:59.000000 twikit-1.4.5/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0   111424 2024-04-08 13:07:33.000000 twikit-1.4.5/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0      875 2024-03-23 06:08:25.000000 twikit-1.4.5/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7402 2024-04-08 13:08:15.000000 twikit-1.4.5/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     1955 2024-04-06 04:28:33.000000 twikit-1.4.5/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-04-08 13:08:52.000000 twikit-1.4.5/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-04-06 13:49:04.000000 twikit-1.4.5/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-06 13:49:28.000000 twikit-1.4.5/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1079 2024-04-06 13:49:39.000000 twikit-1.4.5/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    17253 2024-04-08 13:09:53.000000 twikit-1.4.5/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14677 2024-04-08 13:10:20.000000 twikit-1.4.5/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-04-06 13:55:17.000000 twikit-1.4.5/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14454 2024-04-08 13:05:19.000000 twikit-1.4.5/twikit/user.py
+-rw-rw-rw-   0        0        0    21210 2024-04-08 07:34:42.000000 twikit-1.4.5/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:30:34.210236 twikit-1.4.5/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3873 2024-04-08 13:30:33.000000 twikit-1.4.5/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2024-04-08 13:30:34.000000 twikit-1.4.5/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 13:30:33.000000 twikit-1.4.5/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-08 13:30:33.000000 twikit-1.4.5/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-08 13:30:33.000000 twikit-1.4.5/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.4.4/LICENSE` & `twikit-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.4.4/PKG-INFO` & `twikit-1.4.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,150 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.4
+Version: 1.4.5
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img src="https://i.imgur.com/iJe6rsZ.png" width="500">
+<img  src="https://i.imgur.com/iJe6rsZ.png"  width="500">
+
+
 
 ![Number of GitHub stars](https://img.shields.io/github/stars/d60/twikit)
+
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/d60/twikit)
+
 ![Version](https://img.shields.io/pypi/v/twikit?label=PyPI)
+
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Create%20your%20own%20Twitter%20bot%20for%20free%20with%20%22Twikit%22!%20%23python%20%23twitter%20%23twikit%20%23programming%20%23github%20%23bot&url=https%3A%2F%2Fgithub.com%2Fd60%2Ftwikit)
+
 [![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/nCrByrr8cX)
+
 [![BuyMeACoffee](https://img.shields.io/badge/-buy_me_a%C2%A0coffee-gray?logo=buy-me-a-coffee)](https://www.buymeacoffee.com/d60py)
 
 
-# Twikit <img height="35" src="https://i.imgur.com/9HSdIl4.png" valign="bottom">
+# Twikit <img height="35"  src="https://i.imgur.com/9HSdIl4.png"  valign="bottom">
+
 simple API wrapper to interact with twitter's unofficial API.
+
 You can log in to Twitter using your account username, email address and password and use most features on Twitter, such as posting and retrieving tweets, liking and following users.
+
 - [Documentation (English)](https://twikit.readthedocs.io/en/latest/twikit.html)
+
 - [Async Documentation](https://twikit.readthedocs.io/en/latest/twikit.twikit_async.html)
 
+
+
 If you have any questions, please ask on [Discord](https://discord.gg/nCrByrr8cX).
 
+
+
 ## Features
+
 ### No API Key Required
-The library uses an unofficial API and therefore does **not require an API key**.
+
+This library uses the unofficial API, therefore does **not require an API key**.
+
 ### Completely Free
-The service is entirely free to use.
+
+This library is completely free to use.
+
 ### Both Synchronous and Asynchronous Support
+
 Whether you prefer **synchronous** or **asynchronous** programming,
+
 Twikit supports both, providing flexibility for different use cases.
 
+
 ## Functionality
+
 This library allows you to perform various Twitter-related actions, including:
-- **Create tweets**
-- **Search tweets**
-- **Retrieve trending topics**
+
+-  **Create tweets**
+
+-  **Search tweets**
+
+-  **Retrieve trending topics**
+
 - etc...
 
+
+
 ## Installing
- ```back
- pip install twikit
- ```
+
+```bash
+
+pip install twikit
+
+```
+
+
 
 ## Quick Example
+
 **Define a client and log in to the account.**
+
 ```python
 from twikit import Client
 
 USERNAME = 'example_user'
 EMAIL = 'email@example.com'
 PASSWORD = 'password0000'
 
 # Initialize client
 client = Client('en-US')
+
 # Login to the service with provided user credentials
 client.login(
     auth_info_1=USERNAME ,
     auth_info_2=EMAIL,
     password=PASSWORD
 )
 ```
+
 **Create a tweet with media attached.**
+
 ```python
 # Upload media files and obtain media_ids
 media_ids = [
     client.upload_media('media1.jpg'),
     client.upload_media('media2.jpg')
 ]
+
 # Create a tweet with the provided text and attached media
 client.create_tweet(
     text='Example Tweet',
     media_ids=media_ids
 )
+
 ```
 
+**Search the latest tweets based on a keywords**
+```python
+tweets = client.search_tweet('python', 'Latest')
+
+for tweet in tweets:
+    print(
+        tweet.user.name,
+        tweet.text,
+        tweet.created_at
+    )
+```
+
+
 More Examples: [examples](https://github.com/d60/twikit/tree/main/examples) <br>
 
+
+
 ## Contributing
+
 I would like to hear your thoughts and suggestions.
+
 If you have any features you'd like to see added or encounter any issues,
+
 please let me know in the [issues](https://github.com/d60/twikit/issues) section.
 
+
 Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library⭐! Thank you very much!
```

### Comparing `twikit-1.4.4/README.md` & `twikit-1.4.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,140 @@
-<img src="https://i.imgur.com/iJe6rsZ.png" width="500">
+<img  src="https://i.imgur.com/iJe6rsZ.png"  width="500">
+
+
 
 ![Number of GitHub stars](https://img.shields.io/github/stars/d60/twikit)
+
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/d60/twikit)
+
 ![Version](https://img.shields.io/pypi/v/twikit?label=PyPI)
+
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Create%20your%20own%20Twitter%20bot%20for%20free%20with%20%22Twikit%22!%20%23python%20%23twitter%20%23twikit%20%23programming%20%23github%20%23bot&url=https%3A%2F%2Fgithub.com%2Fd60%2Ftwikit)
+
 [![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/nCrByrr8cX)
+
 [![BuyMeACoffee](https://img.shields.io/badge/-buy_me_a%C2%A0coffee-gray?logo=buy-me-a-coffee)](https://www.buymeacoffee.com/d60py)
 
 
-# Twikit <img height="35" src="https://i.imgur.com/9HSdIl4.png" valign="bottom">
+# Twikit <img height="35"  src="https://i.imgur.com/9HSdIl4.png"  valign="bottom">
+
 simple API wrapper to interact with twitter's unofficial API.
+
 You can log in to Twitter using your account username, email address and password and use most features on Twitter, such as posting and retrieving tweets, liking and following users.
+
 - [Documentation (English)](https://twikit.readthedocs.io/en/latest/twikit.html)
+
 - [Async Documentation](https://twikit.readthedocs.io/en/latest/twikit.twikit_async.html)
 
+
+
 If you have any questions, please ask on [Discord](https://discord.gg/nCrByrr8cX).
 
+
+
 ## Features
+
 ### No API Key Required
-The library uses an unofficial API and therefore does **not require an API key**.
+
+This library uses the unofficial API, therefore does **not require an API key**.
+
 ### Completely Free
-The service is entirely free to use.
+
+This library is completely free to use.
+
 ### Both Synchronous and Asynchronous Support
+
 Whether you prefer **synchronous** or **asynchronous** programming,
+
 Twikit supports both, providing flexibility for different use cases.
 
+
 ## Functionality
+
 This library allows you to perform various Twitter-related actions, including:
-- **Create tweets**
-- **Search tweets**
-- **Retrieve trending topics**
+
+-  **Create tweets**
+
+-  **Search tweets**
+
+-  **Retrieve trending topics**
+
 - etc...
 
+
+
 ## Installing
- ```back
- pip install twikit
- ```
+
+```bash
+
+pip install twikit
+
+```
+
+
 
 ## Quick Example
+
 **Define a client and log in to the account.**
+
 ```python
 from twikit import Client
 
 USERNAME = 'example_user'
 EMAIL = 'email@example.com'
 PASSWORD = 'password0000'
 
 # Initialize client
 client = Client('en-US')
+
 # Login to the service with provided user credentials
 client.login(
     auth_info_1=USERNAME ,
     auth_info_2=EMAIL,
     password=PASSWORD
 )
 ```
+
 **Create a tweet with media attached.**
+
 ```python
 # Upload media files and obtain media_ids
 media_ids = [
     client.upload_media('media1.jpg'),
     client.upload_media('media2.jpg')
 ]
+
 # Create a tweet with the provided text and attached media
 client.create_tweet(
     text='Example Tweet',
     media_ids=media_ids
 )
+
 ```
 
+**Search the latest tweets based on a keywords**
+```python
+tweets = client.search_tweet('python', 'Latest')
+
+for tweet in tweets:
+    print(
+        tweet.user.name,
+        tweet.text,
+        tweet.created_at
+    )
+```
+
+
 More Examples: [examples](https://github.com/d60/twikit/tree/main/examples) <br>
 
+
+
 ## Contributing
+
 I would like to hear your thoughts and suggestions.
+
 If you have any features you'd like to see added or encounter any issues,
+
 please let me know in the [issues](https://github.com/d60/twikit/issues) section.
 
-Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library⭐! Thank you very much!
+
+Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library⭐! Thank you very much!
```

### Comparing `twikit-1.4.4/setup.py` & `twikit-1.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     name='twikit',
     version=version,
     install_requires=[
         'httpx',
         'fake_useragent',
         'filetype'
     ],
-    python_requires='>=3.9',
+    python_requires='>=3.10',
     description='Twitter API wrapper for python with **no API key required**.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/d60/twikit',
     package_data={'twikit': ['py.typed']}
 )
```

### Comparing `twikit-1.4.4/twikit/client.py` & `twikit-1.4.5/twikit/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import io
 import json
 import time
+from functools import partial
 from typing import Literal
 
 import filetype
 from fake_useragent import UserAgent
 from httpx import Response
 
 from .errors import (
@@ -32,14 +33,15 @@
     USER_FEATURES,
     Endpoint,
     Flow,
     Result,
     build_tweet_data,
     build_user_data,
     find_dict,
+    flatten_params,
     get_query_id,
     urlencode
 )
 
 
 class Client:
     """
@@ -127,22 +129,22 @@
         `auth_info_2` is optional and can be omitted, but it is
         recommended to provide if available.
         The order in which you specify authentication information
         (auth_info_1 and auth_info_2) is flexible.
 
         Parameters
         ----------
-        auth_info_1 : str
+        auth_info_1 : :class:`str`
             The first piece of authentication information,
             which can be a username, email address, or phone number.
-        auth_info_2 : str, default=None
+        auth_info_2 : :class:`str`, default=None
             The second piece of authentication information,
             which is optional but recommended to provide.
             It can be a username, email address, or phone number.
-        password : str
+        password : :class:`str`
             The password associated with the account.
 
         Examples
         --------
         >>> client.login(
         ...     auth_info_1='example_user',
         ...     auth_info_2='email@example.com',
@@ -280,15 +282,15 @@
         """
         Save cookies to file in json format.
         You can skip the login procedure by loading the saved cookies
         using the :func:`load_cookies` method.
 
         Parameters
         ----------
-        path : str
+        path : :class:`str`
             The path to the file where the cookie will be stored.
 
         Examples
         --------
         >>> client.save_cookies('cookies.json')
 
         See Also
@@ -303,15 +305,15 @@
     def set_cookies(self, cookies: dict, clear_cookies: bool = False) -> None:
         """
         Sets cookies.
         You can skip the login procedure by loading a saved cookies.
 
         Parameters
         ----------
-        cookies : dict
+        cookies : :class:`dict`
             The cookies to be set as key value pair.
 
         Examples
         --------
         >>> with open('cookies.json', 'r', encoding='utf-8') as f:
         ...     client.set_cookies(json.load(f))
 
@@ -328,15 +330,15 @@
     def load_cookies(self, path: str) -> None:
         """
         Loads cookies from a file.
         You can skip the login procedure by loading a saved cookies.
 
         Parameters
         ----------
-        path : str
+        path : :class:`str`
             Path to the file where the cookie is stored.
 
         Examples
         --------
         >>> client.load_cookies('cookies.json')
 
         See Also
@@ -350,15 +352,15 @@
 
     def set_delegate_account(self, user_id: str | None) -> None:
         """
         Sets the account to act as.
 
         Parameters
         ----------
-        user_id : str | None
+        user_id : :class:`str` | None
             The user ID of the account to act as.
             Set to None to clear the delegated account.
         """
         self._act_as = user_id
 
     def _search(
         self,
@@ -374,18 +376,18 @@
             'rawQuery': query,
             'count': count,
             'querySource': 'typed_query',
             'product': product
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         response = self.http.get(
             Endpoint.SEARCH_TIMELINE,
             params=params,
             headers=self._base_headers
         ).json()
 
         return response
@@ -399,26 +401,26 @@
     ) -> Result[Tweet]:
         """
         Searches for tweets based on the specified query and
         product type.
 
         Parameters
         ----------
-        query : str
+        query : :class:`str`
             The search query.
         product : {'Top', 'Latest', 'Media'}
             The type of tweets to retrieve.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of tweets to retrieve, between 1 and 20.
-        cursor : str, default=20
+        cursor : :class:`str`, default=20
             Token to retrieve more tweets.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             An instance of the `Result` class containing the
             search results.
 
         Examples
         --------
         >>> tweets = client.search_tweet('query', 'Top')
         >>> for tweet in tweets:
@@ -483,41 +485,41 @@
                 previous_cursor = entries[-2]['content']['value']
             else:
                 next_cursor = instructions[-1]['entry']['content']['value']
                 previous_cursor = instructions[-2]['entry']['content']['value']
 
         return Result(
             results,
-            lambda:self.search_tweet(query, product, count, next_cursor),
+            partial(self.search_tweet, query, product, count, next_cursor),
             next_cursor,
-            lambda:self.search_tweet(query, product, count, previous_cursor),
+            partial(self.search_tweet, query, product, count, previous_cursor),
             previous_cursor
         )
 
     def search_user(
         self,
         query: str,
         count: int = 20,
         cursor: str | None = None
     ) -> Result[User]:
         """
         Searches for users based on the provided query.
 
         Parameters
         ----------
-        query : str
+        query : :class:`str`
             The search query for finding users.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of users to retrieve in each request.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             Token to retrieve more users.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             An instance of the `Result` class containing the
             search results.
 
         Examples
         --------
         >>> result = client.search_user('query')
         >>> for user in result:
@@ -544,15 +546,15 @@
             if 'itemContent' not in item['content']:
                 continue
             user_info = find_dict(item, 'result')[0]
             results.append(User(self, user_info))
 
         return Result(
             results,
-            lambda:self.search_user(query, count, next_cursor),
+            partial(self.search_user, query, count, next_cursor),
             next_cursor
         )
 
     def upload_media(
         self,
         source: str | bytes,
         wait_for_completion: bool = False,
@@ -561,31 +563,31 @@
         media_category: str | None = None
     ) -> str:
         """
         Uploads media to twitter.
 
         Parameters
         ----------
-        source : str | bytes
+        source : :class:`str` | :class:`bytes`
             The source of the media to be uploaded.
             It can be either a file path or bytes of the media content.
-        wait_for_completion : bool, default=False
+        wait_for_completion : :class:`bool`, default=False
             Whether to wait for the completion of the media upload process.
-        status_check_interval : float, default=1.0
+        status_check_interval : :class:`float`, default=1.0
             The interval (in seconds) to check the status of the
             media upload process.
-        media_type : str, default=None
+        media_type : :class:`str`, default=None
             The MIME type of the media.
             If not specified, it will be guessed from the source.
-        media_category : str, default=None
+        media_category : :class:`str`, default=None
             The media category.
 
         Returns
         -------
-        str
+        :class:`str`
             The media ID of the uploaded media.
 
         Examples
         --------
         Videos, images and gifs can be uploaded.
 
         >>> media_id_1 = client.upload_media(
@@ -703,20 +705,20 @@
 
     def check_media_status(self, media_id: str) -> dict:
         """
         Check the status of uploaded media.
 
         Parameters
         ----------
-        media_id : str
+        media_id : :class:`str`
             The media ID of the uploaded media.
 
         Returns
         -------
-        dict
+        :class:`dict`
             A dictionary containing information about the status of
             the uploaded media.
         """
         params = {
             'command': 'STATUS',
             'media_id': media_id
         }
@@ -733,22 +735,22 @@
         duration_minutes: int
     ) -> str:
         """
         Creates a poll and returns card-uri.
 
         Parameters
         ----------
-        choices : list[str]
+        choices : list[:class:`str`]
             A list of choices for the poll. Maximum of 4 choices.
-        duration_minutes : int
+        duration_minutes : :class:`int`
             The duration of the poll in minutes.
 
         Returns
         -------
-        str
+        :class:`str`
             The URI of the created poll card.
 
         Examples
         --------
         Create a poll with three choices lasting for 60 minutes:
 
         >>> choices = ['Option A', 'Option B', 'Option C']
@@ -788,26 +790,26 @@
         card_name: str
     ) -> Poll:
         """
         Vote on a poll with the selected choice.
 
         Parameters
         ----------
-        selected_choice : str
+        selected_choice : :class:`str`
             The label of the selected choice for the vote.
-        card_uri : str
+        card_uri : :class:`str`
             The URI of the poll card.
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the original tweet containing the poll.
-        card_name : str
+        card_name : :class:`str`
             The name of the poll card.
 
         Returns
         -------
-        Poll
+        :class:`Poll`
             The Poll object representing the updated poll after voting.
         """
         data = urlencode({
             'twitter:string:card_uri': card_uri,
             'twitter:long:original_tweet_id': tweet_id,
             'twitter:string:response_card_name': card_name,
             'twitter:string:cards_platform': 'Web-12',
@@ -840,39 +842,39 @@
     ) -> Tweet:
         """
         Creates a new tweet on Twitter with the specified
         text, media, and poll.
 
         Parameters
         ----------
-        text : str, default=''
+        text : :class:`str`, default=''
             The text content of the tweet.
-        media_ids : list[str], default=None
+        media_ids : list[:class:`str`], default=None
             A list of media IDs or URIs to attach to the tweet.
             media IDs can be obtained by using the `upload_media` method.
-        poll_uri : str, default=None
+        poll_uri : :class:`str`, default=None
             The URI of a Twitter poll card to attach to the tweet.
             Poll URIs can be obtained by using the `create_poll` method.
-        reply_to : str, default=None
+        reply_to : :class:`str`, default=None
             The ID of the tweet to which this tweet is a reply.
         conversation_control : {'followers', 'verified', 'mentioned'}
             The type of conversation control for the tweet:
             - 'followers': Limits replies to followers only.
             - 'verified': Limits replies to verified accounts only.
             - 'mentioned': Limits replies to mentioned accounts only.
-        attachment_url : str
+        attachment_url : :class:`str`
             URL of the tweet to be quoted.
 
         Raises
         ------
-        DuplicateTweet : If the tweet is a duplicate of another tweet.
+        :exc:`DuplicateTweet` : If the tweet is a duplicate of another tweet.
 
         Returns
         -------
-        Tweet
+        :class:`Tweet`
             The Created Tweet.
 
         Examples
         --------
         Create a tweet with media:
 
         >>> tweet_text = 'Example text'
@@ -941,15 +943,15 @@
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_TWEET),
             'features': FEATURES,
         }
         response = self.http.post(
             Endpoint.CREATE_TWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers,
         ).json()
 
         _result = find_dict(response, 'result')
         if not _result:
             raise_exceptions_from_response(response['errors'])
             raise CouldNotTweet(
@@ -969,24 +971,24 @@
         media_ids: list[str] | None = None,
     ) -> str:
         """
         Schedules a tweet to be posted at a specified timestamp.
 
         Parameters
         ----------
-        scheduled_at : int
+        scheduled_at : :class:`int`
             The timestamp when the tweet should be scheduled for posting.
-        text : str, default=''
+        text : :class:`str`, default=''
             The text content of the tweet, by default an empty string.
-        media_ids : list[str], default=None
+        media_ids : list[:class:`str`], default=None
             A list of media IDs to be attached to the tweet, by default None.
 
         Returns
         -------
-        str
+        :class:`str`
             The ID of the scheduled tweet.
 
         Examples
         --------
         Create a tweet with media:
 
         >>> scheduled_time = int(time.time()) + 3600  # One hour from now
@@ -1012,30 +1014,30 @@
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_SCHEDULED_TWEET),
         }
         response = self.http.post(
             Endpoint.CREATE_SCHEDULED_TWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers,
         ).json()
         return response['data']['tweet']['rest_id']
 
     def delete_tweet(self, tweet_id: str) -> Response:
         """Deletes a tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             ID of the tweet to be deleted.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '0000000000'
         >>> delete_tweet(tweet_id)
         """
@@ -1044,50 +1046,50 @@
                 'tweet_id': tweet_id,
                 'dark_request': False
             },
             'queryId': get_query_id(Endpoint.DELETE_TWEET)
         }
         response = self.http.post(
             Endpoint.DELETE_TWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def get_user_by_screen_name(self, screen_name: str) -> User:
         """
         Fetches a user by screen name.
 
         Parameter
         ---------
-        screen_name : str
+        screen_name : :class:`str`
             The screen name of the Twitter user.
 
         Returns
         -------
-        User
+        :class:`User`
             An instance of the User class representing the
             Twitter user.
 
         Examples
         --------
         >>> target_screen_name = 'example_user'
         >>> user = client.get_user_by_name(target_screen_name)
         >>> print(user)
         <User id="...">
         """
         variables = {
             'screen_name': screen_name,
             'withSafetyModeUserFields': False
         }
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(USER_FEATURES),
-            'fieldToggles': json.dumps({'withAuxiliaryUserLabels': False})
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': USER_FEATURES,
+            'fieldToggles': {'withAuxiliaryUserLabels': False}
+        })
         response = self.http.get(
             Endpoint.USER_BY_SCREEN_NAME,
             params=params,
             headers=self._base_headers
         ).json()
 
         if 'user' not in response['data']:
@@ -1100,38 +1102,38 @@
 
     def get_user_by_id(self, user_id: str) -> User:
         """
         Fetches a user by ID
 
         Parameter
         ---------
-        user_id : str
+        user_id : :class:`str`
             The ID of the Twitter user.
 
         Returns
         -------
-        User
+        :class:`User`
             An instance of the User class representing the
             Twitter user.
 
         Examples
         --------
         >>> target_screen_name = '000000000'
         >>> user = client.get_user_by_id(target_screen_name)
         >>> print(user)
         <User id="000000000">
         """
         variables = {
             'userId': user_id,
             'withSafetyModeUserFields': True
         }
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(USER_FEATURES),
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': USER_FEATURES
+        })
         response = self.http.get(
             Endpoint.USER_BY_REST_ID,
             params=params,
             headers=self._base_headers
         ).json()
         if 'result' not in response['data']['user']:
             raise TwitterException(f'Invalid user id: {user_id}')
@@ -1147,19 +1149,19 @@
             'withQuickPromoteEligibilityTweetFields': True,
             'withBirdwatchNotes': True,
             'withVoice': True,
             'withV2Timeline': True
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES),
-            'fieldToggles': json.dumps({'withAuxiliaryUserLabels': False})
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES,
+            'fieldToggles': {'withAuxiliaryUserLabels': False}
+        })
         response = self.http.get(
             Endpoint.TWEET_DETAIL,
             params=params,
             headers=self._base_headers
         ).json()
         return response
 
@@ -1168,23 +1170,25 @@
         entries = find_dict(response, 'entries')[0]
 
         results = []
         for entry in entries:
             if entry['entryId'].startswith('cursor'):
                 continue
             tweet_info = find_dict(entry, 'result')[0]
+            if tweet_info['__typename'] == 'TweetTombstone':
+                continue
             if tweet_info['__typename'] == 'TweetWithVisibilityResults':
                 tweet_info = tweet_info['tweet']
             user_info = tweet_info['core']['user_results']['result']
             results.append(Tweet(self, tweet_info, User(self, user_info)))
 
         if entries[-1]['entryId'].startswith('cursor'):
             next_cursor = entries[-1]['content']['itemContent']['value']
-            def _fetch_next_result():
-                return self._get_more_replies(tweet_id, next_cursor)
+            _fetch_next_result = partial(self._get_more_replies,
+                                         tweet_id, next_cursor)
         else:
             next_cursor = None
             _fetch_next_result = None
 
         return Result(
             results,
             _fetch_next_result,
@@ -1195,20 +1199,20 @@
         self, tweet_id: str, cursor: str | None = None
     ) -> Tweet:
         """
         Fetches a tweet by tweet ID.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet.
 
         Returns
         -------
-        Tweet
+        :class:`Tweet`
             A Tweet object representing the fetched tweet.
 
         Examples
         --------
         >>> target_tweet_id = '...'
         >>> tweet = client.get_tweet_by_id(target_tweet_id)
         >>> print(tweet)
@@ -1253,16 +1257,16 @@
                     reply_to.append(tweet_object)
                 else:
                     replies_list.append(tweet_object)
 
         if entries[-1]['entryId'].startswith('cursor'):
             # if has more replies
             reply_next_cursor = entries[-1]['content']['itemContent']['value']
-            def _fetch_more_replies():
-                return self._get_more_replies(tweet_id, reply_next_cursor)
+            _fetch_more_replies = partial(self._get_more_replies,
+                                          tweet_id, reply_next_cursor)
         else:
             reply_next_cursor = None
             _fetch_more_replies = None
 
         tweet.replies = Result(
             replies_list,
             _fetch_more_replies,
@@ -1275,51 +1279,51 @@
 
     def get_scheduled_tweets(self) -> list[ScheduledTweet]:
         """
         Retrieves scheduled tweets.
 
         Returns
         -------
-        list[ScheduledTweet]
+        list[:class:`ScheduledTweet`]
             List of ScheduledTweet objects representing the scheduled tweets.
         """
-        params = {
-            'variables': json.dumps({'ascending': True})
-        }
+        params = flatten_params({
+            'variables': {'ascending': True}
+        })
         response = self.http.get(
             Endpoint.FETCH_SCHEDULED_TWEETS,
             params=params,
             headers=self._base_headers
         ).json()
         tweets = find_dict(response, 'scheduled_tweet_list')[0]
         return [ScheduledTweet(self, tweet) for tweet in tweets]
 
     def delete_scheduled_tweet(self, tweet_id: str) -> Response:
         """
         Delete a scheduled tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the scheduled tweet to delete.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
         data = {
             'variables': {
                 'scheduled_tweet_id': tweet_id
             },
             'queryId': get_query_id(Endpoint.DELETE_SCHEDULED_TWEET)
         }
         response = self.http.post(
             Endpoint.DELETE_SCHEDULED_TWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def _get_tweet_engagements(
         self, tweet_id: str, count: int, cursor: str, endpoint: str,
     ) -> Result[User]:
@@ -1329,18 +1333,18 @@
         variables = {
             'tweetId': tweet_id,
             'count': count,
             'includePromotedContent': True
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         response = self.http.get(
             endpoint,
             params=params,
             headers=self._base_headers
         ).json()
         items_ = find_dict(response, 'entries')
         if not items_:
@@ -1357,40 +1361,40 @@
             if not user_info_:
                 continue
             user_info = user_info_[0]
             results.append(User(self, user_info))
 
         return Result(
             results,
-            lambda:self._get_tweet_engagements(
-                tweet_id, count, next_cursor, endpoint),
+            partial(self._get_tweet_engagements,
+                    tweet_id, count, next_cursor, endpoint),
             next_cursor,
-            lambda:self._get_tweet_engagements(
-                tweet_id, count, previous_cursor, endpoint),
+            partial(self._get_tweet_engagements,
+                    tweet_id, count, previous_cursor, endpoint),
             previous_cursor
         )
 
     def get_retweeters(
         self, tweet_id: str, count: int = 40, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieve users who retweeted a specific tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet.
-        count : int, default=40
+        count : :class:`int`, default=40
             The maximum number of users to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A string indicating the position of the cursor for pagination.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of users who retweeted the tweet.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> retweeters = client.get_retweeters(tweet_id)
         >>> print(retweeters)
@@ -1408,24 +1412,24 @@
         self, tweet_id: str, count: int = 40, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieve users who favorited a specific tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet.
         count : int, default=40
             The maximum number of users to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A string indicating the position of the cursor for pagination.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of users who favorited the tweet.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> favoriters = client.get_favoriters(tweet_id)
         >>> print(favoriters)
@@ -1447,28 +1451,28 @@
         cursor: str | None = None
     ) -> Result[Tweet]:
         """
         Fetches tweets from a specific user's timeline.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the Twitter user whose tweets to retrieve.
             To get the user id from the screen name, you can use
             `get_user_by_screen_name` method.
         tweet_type : {'Tweets', 'Replies', 'Media', 'Likes'}
             The type of tweets to retrieve.
-        count : int, default=40
+        count : :class:`int`, default=40
             The number of tweets to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             The cursor for fetching the next set of results.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing a list of `Tweet` objects.
 
         Examples
         --------
         >>> user_id = '...'
 
         If you only have the screen name, you can get the user id as follows:
@@ -1507,18 +1511,18 @@
             'includePromotedContent': True,
             'withQuickPromoteEligibilityTweetFields': True,
             'withVoice': True,
             'withV2Timeline': True
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES),
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         endpoint = {
             'Tweets': Endpoint.USER_TWEETS,
             'Replies': Endpoint.USER_TWEETS_AND_REPLIES,
             'Media': Endpoint.USER_MEDIA,
             'Likes': Endpoint.USER_LIKES,
         }[tweet_type]
 
@@ -1576,19 +1580,19 @@
             tweet = Tweet(self, tweet_info, User(self, user_info))
             tweet.replies = replies
 
             results.append(tweet)
 
         return Result(
             results,
-            lambda:self.get_user_tweets(
-                user_id, tweet_type, count, next_cursor),
+            partial(self.get_user_tweets,
+                    user_id, tweet_type, count, next_cursor),
             next_cursor,
-            lambda:self.get_user_tweets(
-                user_id, tweet_type, count, previous_cursor),
+            partial(self.get_user_tweets,
+                    user_id, tweet_type, count, previous_cursor),
             previous_cursor
         )
 
     def get_timeline(
         self,
         count: int = 20,
         seen_tweet_ids: list[str] | None = None,
@@ -1598,22 +1602,22 @@
         Retrieves the timeline.
         Retrieves tweets from Home -> For You.
 
         Parameters
         ----------
         count : int, default=20
             The number of tweets to retrieve.
-        seen_tweet_ids : list[str], default=None
+        seen_tweet_ids : list[:class:`str`], default=None
             A list of tweet IDs that have been seen.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A cursor for pagination.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing a list of Tweet objects.
 
         Example
         -------
         >>> tweets = client.get_timeline()
         >>> for tweet in tweets:
         ...     print(tweet)
@@ -1643,15 +1647,15 @@
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.HOME_TIMELINE),
             'features': FEATURES,
         }
         response = self.http.post(
             Endpoint.HOME_TIMELINE,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         ).json()
 
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
         results = []
 
@@ -1662,15 +1666,15 @@
             if tweet_info['__typename'] == 'TweetWithVisibilityResults':
                 tweet_info = tweet_info['tweet']
             user_info = tweet_info['core']['user_results']['result']
             results.append(Tweet(self, tweet_info, user_info))
 
         return Result(
             results,
-            lambda:self.get_timeline(count, seen_tweet_ids, next_cursor),
+            partial(self.get_timeline, count, seen_tweet_ids, next_cursor),
             next_cursor
         )
 
     def get_latest_timeline(
         self,
         count: int = 20,
         seen_tweet_ids: list[str] | None = None,
@@ -1680,22 +1684,22 @@
         Retrieves the timeline.
         Retrieves tweets from Home -> Following.
 
         Parameters
         ----------
         count : int, default=20
             The number of tweets to retrieve.
-        seen_tweet_ids : list[str], default=None
+        seen_tweet_ids : list[:class:`str`], default=None
             A list of tweet IDs that have been seen.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A cursor for pagination.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing a list of Tweet objects.
 
         Example
         -------
         >>> tweets = client.get_latest_timeline()
         >>> for tweet in tweets:
         ...     print(tweet)
@@ -1725,15 +1729,15 @@
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.HOME_LATEST_TIMELINE),
             'features': FEATURES,
         }
         response = self.http.post(
             Endpoint.HOME_LATEST_TIMELINE,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         ).json()
 
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
         results = []
 
@@ -1744,31 +1748,31 @@
             if tweet_info['__typename'] == 'TweetWithVisibilityResults':
                 tweet_info = tweet_info['tweet']
             user_info = tweet_info['core']['user_results']['result']
             results.append(Tweet(self, tweet_info, user_info))
 
         return Result(
             results,
-            lambda: self.get_latest_timeline(
-                count, seen_tweet_ids, next_cursor),
+            partial(self.get_latest_timeline,
+                    count, seen_tweet_ids, next_cursor),
             next_cursor
         )
 
     def favorite_tweet(self, tweet_id: str) -> Response:
         """
         Favorites a tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet to be liked.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> client.favorite_tweet(tweet_id)
 
@@ -1778,31 +1782,31 @@
         """
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.FAVORITE_TWEET)
         }
         response = self.http.post(
             Endpoint.FAVORITE_TWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def unfavorite_tweet(self, tweet_id: str) -> Response:
         """
         Unfavorites a tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet to be unliked.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> client.unfavorite_tweet(tweet_id)
 
@@ -1812,31 +1816,31 @@
         """
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.UNFAVORITE_TWEET)
         }
         response = self.http.post(
             Endpoint.UNFAVORITE_TWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def retweet(self, tweet_id: str) -> Response:
         """
         Retweets a tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet to be retweeted.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> client.retweet(tweet_id)
 
@@ -1846,31 +1850,31 @@
         """
         data = {
             'variables': {'tweet_id': tweet_id, 'dark_request': False},
             'queryId': get_query_id(Endpoint.CREATE_RETWEET)
         }
         response = self.http.post(
             Endpoint.CREATE_RETWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def delete_retweet(self, tweet_id: str) -> Response:
         """
         Deletes the retweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the retweeted tweet to be unretweeted.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> client.delete_retweet(tweet_id)
 
@@ -1880,31 +1884,31 @@
         """
         data = {
             'variables': {'source_tweet_id': tweet_id,'dark_request': False},
             'queryId': get_query_id(Endpoint.DELETE_RETWEET)
         }
         response = self.http.post(
             Endpoint.DELETE_RETWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def bookmark_tweet(self, tweet_id: str) -> Response:
         """
         Adds the tweet to bookmarks.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet to be bookmarked.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> client.bookmark_tweet(tweet_id)
 
@@ -1915,31 +1919,31 @@
 
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.CREATE_BOOKMARK)
         }
         response = self.http.post(
             Endpoint.CREATE_BOOKMARK,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def delete_bookmark(self, tweet_id: str) -> Response:
         """
         Removes the tweet from bookmarks.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet to be removed from bookmarks.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> client.delete_bookmark(tweet_id)
 
@@ -1949,35 +1953,35 @@
         """
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.DELETE_BOOKMARK)
         }
         response = self.http.post(
             Endpoint.DELETE_BOOKMARK,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def get_bookmarks(
         self, count: int = 20, cursor: str | None = None
     ) -> Result[Tweet]:
         """
         Retrieves bookmarks from the authenticated user's Twitter account.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of bookmarks to retrieve (default is 20).
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A cursor to paginate through the bookmarks (default is None).
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing a list of Tweet objects
             representing bookmarks.
 
         Example
         -------
         >>> bookmarks = client.get_bookmarks()
         >>> for bookmark in bookmarks:
@@ -1996,18 +2000,18 @@
             'includePromotedContent': True
         }
         if cursor is not None:
             variables['cursor'] = cursor
         features = FEATURES | {
             'graphql_timeline_v2_bookmark_timeline': True
         }
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(features)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': features
+        })
         response = self.http.get(
             Endpoint.BOOKMARKS,
             params=params,
             headers=self._base_headers
         ).json()
 
         items_ = find_dict(response, 'entries')
@@ -2023,56 +2027,56 @@
                 continue
             tweet_info = find_dict(item, 'tweet_results')[0]['result']
             user_info = tweet_info['core']['user_results']['result']
             results.append(Tweet(self, tweet_info, User(self, user_info)))
 
         return Result(
             results,
-            lambda:self.get_bookmarks(count, next_cursor),
+            partial(self.get_bookmarks, count, next_cursor),
             next_cursor,
-            lambda:self.get_bookmarks(count, previous_cursor),
+            partial(self.get_bookmarks, count, previous_cursor),
             previous_cursor
         )
 
     def delete_all_bookmarks(self) -> Response:
         """
         Deleted all bookmarks.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> client.delete_all_bookmarks()
         """
         data = {
             'variables': {},
             'queryId': get_query_id(Endpoint.BOOKMARKS_ALL_DELETE)
         }
         response = self.http.post(
             Endpoint.BOOKMARKS_ALL_DELETE,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def follow_user(self, user_id: str) -> Response:
         """
         Follows a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to follow.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response:class:`
             Response returned from twitter api.
 
         Examples
         --------
         >>> user_id = '...'
         >>> client.follow_user(user_id)
 
@@ -2107,20 +2111,20 @@
 
     def unfollow_user(self, user_id: str) -> Response:
         """
         Unfollows a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to unfollow.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> user_id = '...'
         >>> client.unfollow_user(user_id)
 
@@ -2155,20 +2159,20 @@
 
     def block_user(self, user_id: str) -> Response:
         """
         Blocks a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to block.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .unblock_user
         """
         data = urlencode({'user_id': user_id})
@@ -2183,20 +2187,20 @@
 
     def unblock_user(self, user_id: str) -> Response:
         """
         Unblocks a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to unblock.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .block_user
         """
         data = urlencode({'user_id': user_id})
@@ -2211,20 +2215,20 @@
 
     def mute_user(self, user_id: str) -> Response:
         """
         Mutes a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to mute.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .unmute_user
         """
         data = urlencode({'user_id': user_id})
@@ -2239,20 +2243,20 @@
 
     def unmute_user(self, user_id: str) -> Response:
         """
         Unmutes a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to unmute.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .mute_user
         """
         data = urlencode({'user_id': user_id})
@@ -2280,20 +2284,20 @@
         category : {'trending', 'for-you', 'news', 'sports', 'entertainment'}
             The category of trends to retrieve. Valid options include:
             - 'trending': General trending topics.
             - 'for-you': Trends personalized for the user.
             - 'news': News-related trends.
             - 'sports': Sports-related trends.
             - 'entertainment': Entertainment-related trends.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of trends to retrieve.
 
         Returns
         -------
-        list[Trend]
+        list[:class:`Trend`]
             A list of Trend objects representing the retrieved trends.
 
         Examples
         --------
         >>> trends = client.get_trends('trending')
         >>> for trend in trends:
         ...     print(trend)
@@ -2348,18 +2352,18 @@
         variables = {
             'userId': user_id,
             'count': count,
             'includePromotedContent': False
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         response = self.http.get(
             endpoint,
             params=params,
             headers=self._base_headers
         ).json()
 
         items = find_dict(response, 'entries')[0]
@@ -2370,35 +2374,35 @@
                 user_info = find_dict(item, 'result')[0]
                 results.append(User(self, user_info))
             elif entry_id.startswith('cursor-bottom'):
                 next_cursor = item['content']['value']
 
         return Result(
             results,
-            lambda: self._get_user_friendship(
-                user_id, count, endpoint, next_cursor),
+            partial(self._get_user_friendship,
+                    user_id, count, endpoint, next_cursor),
             next_cursor
         )
 
     def get_user_followers(
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of followers for a given user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user for whom to retrieve followers.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of followers to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the followers.
         """
         return self._get_user_friendship(
             user_id,
             count,
             Endpoint.FOLLOWERS,
             cursor
@@ -2408,22 +2412,22 @@
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of verified followers for a given user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user for whom to retrieve verified followers.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of verified followers to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the verified followers.
         """
         return self._get_user_friendship(
             user_id,
             count,
             Endpoint.BLUE_VERIFIED_FOLLOWERS,
             cursor
@@ -2433,22 +2437,22 @@
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of common followers.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user for whom to retrieve followers you might know.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of followers you might know to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the followers you might know.
         """
         return self._get_user_friendship(
             user_id,
             count,
             Endpoint.FOLLOWERS_YOU_KNOW,
             cursor
@@ -2458,22 +2462,22 @@
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of users whom the given user is following.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user for whom to retrieve the following users.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of following users to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the users being followed.
         """
         return self._get_user_friendship(
             user_id,
             count,
             Endpoint.FOLLOWING,
             cursor
@@ -2483,22 +2487,22 @@
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of users to which the specified user is subscribed.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user for whom to retrieve subscriptions.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of subscriptions to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the subscribed users.
         """
         return self._get_user_friendship(
             user_id,
             count,
             Endpoint.SUBSCRIPTIONS,
             cursor
@@ -2526,15 +2530,15 @@
         if media_id is not None:
             data['media_id'] = media_id
         if reply_to is not None:
             data['reply_to_dm_id'] = reply_to
 
         return self.http.post(
             Endpoint.SEND_DM,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         ).json()
 
     def _get_dm_history(
         self,
         conversation_id: str,
         max_id: str | None = None
@@ -2562,28 +2566,28 @@
         reply_to: str | None = None
     ) -> Message:
         """
         Send a direct message to a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to whom the direct message will be sent.
-        text : str
+        text : :class:`str`
             The text content of the direct message.
-        media_id : str, default=None
+        media_id : :class:`str`, default=None
             The media ID associated with any media content
             to be included in the message.
             Media ID can be received by using the :func:`.upload_media` method.
-        reply_to : str, default=None
+        reply_to : :class:`str`, default=None
             Message ID to reply to.
 
         Returns
         -------
-        Message
+        :class:`Message`
             `Message` object containing information about the message sent.
 
         Examples
         --------
         >>> # send DM with media
         >>> user_id = '000000000'
         >>> media_id = client.upload_media('image.png')
@@ -2602,36 +2606,36 @@
 
         message_data = find_dict(response, 'message_data')[0]
         users = list(response['users'].values())
         return Message(
             self,
             message_data,
             users[0]['id_str'],
-            users[1]['id_str']
+            users[1]['id_str'] if len(users) == 2 else users[0]['id_str']
         )
 
     def add_reaction_to_message(
         self, message_id: str, conversation_id: str, emoji: str
     ) -> Response:
         """
         Adds a reaction emoji to a specific message in a conversation.
 
         Parameters
         ----------
-        message_id : str
+        message_id : :class:`str`
             The ID of the message to which the reaction emoji will be added.
             Group ID ('00000000') or partner_ID-your_ID ('00000000-00000001')
-        conversation_id : str
+        conversation_id : :class:`str`
             The ID of the conversation containing the message.
-        emoji : str
+        emoji : :class:`str`
             The emoji to be added as a reaction.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> message_id = '00000000'
         >>> conversation_id = f'00000001-{client.user_id()}'
         >>> client.add_reaction_to_message(
@@ -2646,38 +2650,38 @@
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.MESSAGE_ADD_REACTION)
         }
         response = self.http.post(
             Endpoint.MESSAGE_ADD_REACTION,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def remove_reaction_from_message(
         self, message_id: str, conversation_id: str, emoji: str
     ) -> Response:
         """
         Remove a reaction from a message.
 
         Parameters
         ----------
-        message_id : str
+        message_id : :class:`str`
             The ID of the message from which to remove the reaction.
-        conversation_id : str
+        conversation_id : :class:`str`
             The ID of the conversation where the message is located.
             Group ID ('00000000') or partner_ID-your_ID ('00000000-00000001')
-        emoji : str
+        emoji : :class:`str`
             The emoji to remove as a reaction.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> message_id = '00000000'
         >>> conversation_id = f'00000001-{client.user_id()}'
         >>> client.remove_reaction_from_message(
@@ -2692,31 +2696,31 @@
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.MESSAGE_REMOVE_REACTION)
         }
         response = self.http.post(
             Endpoint.MESSAGE_REMOVE_REACTION,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def delete_dm(self, message_id: str) -> Response:
         """
         Deletes a direct message with the specified message ID.
 
         Parameters
         ----------
-        message_id : str
+        message_id : :class:`str`
             The ID of the direct message to be deleted.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> client.delete_dm('0000000000')
         """
 
@@ -2724,38 +2728,38 @@
             'variables': {
                 'messageId': message_id
             },
             'queryId': get_query_id(Endpoint.DELETE_DM)
         }
         response = self.http.post(
             Endpoint.DELETE_DM,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def get_dm_history(
         self,
         user_id: str,
         max_id: str | None = None
     ) -> Result[Message]:
         """
         Retrieves the DM conversation history with a specific user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user with whom the DM conversation
             history will be retrieved.
-        max_id : str, default=None
+        max_id : :class:`str`, default=None
             If specified, retrieves messages older than the specified max_id.
 
         Returns
         -------
-        Result[Message]
+        Result[:class:`Message`]
             A Result object containing a list of Message objects representing
             the DM conversation history.
 
         Examples
         --------
         >>> messages = client.get_dm_history('0000000000')
         >>> for message in messages:
@@ -2783,15 +2787,15 @@
                 self,
                 message_info,
                 message_info['sender_id'],
                 message_info['recipient_id']
             ))
         return Result(
             messages,
-            lambda:self.get_dm_history(user_id, messages[-1].id),
+            partial(self.get_dm_history, user_id, messages[-1].id),
             messages[-1].id
         )
 
     def send_dm_to_group(
         self,
         group_id: str,
         text: str,
@@ -2799,28 +2803,28 @@
         reply_to: str | None = None
     ) -> GroupMessage:
         """
         Sends a message to a group.
 
         Parameters
         ----------
-        group_id : str
+        group_id : :class:`str`
             The ID of the group in which the direct message will be sent.
-        text : str
+        text : :class:`str`
             The text content of the direct message.
-        media_id : str, default=None
+        media_id : :class:`str`, default=None
             The media ID associated with any media content
             to be included in the message.
             Media ID can be received by using the :func:`.upload_media` method.
-        reply_to : str, default=None
+        reply_to : :class:`str`, default=None
             Message ID to reply to.
 
         Returns
         -------
-        GroupMessage
+        :class:`GroupMessage`
             `GroupMessage` object containing information about
             the message sent.
 
         Examples
         --------
         >>> # send DM with media
         >>> group_id = '000000000'
@@ -2853,23 +2857,23 @@
         max_id: str | None = None
     ) -> Result[GroupMessage]:
         """
         Retrieves the DM conversation history in a group.
 
         Parameters
         ----------
-        group_id : str
+        group_id : :class:`str`
             The ID of the group in which the DM conversation
             history will be retrieved.
-        max_id : str, default=None
+        max_id : :class:`str`, default=None
             If specified, retrieves messages older than the specified max_id.
 
         Returns
         -------
-        Result[GroupMessage]
+        Result[:class:`GroupMessage`]
             A Result object containing a list of GroupMessage objects
             representing the DM conversation history.
 
         Examples
         --------
         >>> messages = client.get_group_dm_history('0000000000')
         >>> for message in messages:
@@ -2899,30 +2903,30 @@
                 self,
                 message_info,
                 message_info['sender_id'],
                 group_id
             ))
         return Result(
             messages,
-            lambda:self.get_group_dm_history(group_id, messages[-1].id),
+            partial(self.get_group_dm_history, group_id, messages[-1].id),
             messages[-1].id
         )
 
     def get_group(self, group_id: str) -> Group:
         """
         Fetches a guild by ID.
 
         Parameters
         ----------
-        group_id : str
+        group_id : :class:`str`
             The ID of the group to retrieve information for.
 
         Returns
         -------
-        Group
+        :class:`Group`
             An object representing the retrieved group.
         """
         params = {
             'context': 'FETCH_DM_CONVERSATION_HISTORY',
             'include_conversation_info': True,
         }
         response = self.http.get(
@@ -2935,22 +2939,22 @@
     def add_members_to_group(
         self, group_id: str, user_ids: list[str]
     ) -> Response:
         """Adds members to a group.
 
         Parameters
         ----------
-        group_id : str
+        group_id : :class:`str`
             ID of the group to which the member is to be added.
-        user_ids : list[str]
+        user_ids : list[:class:`str`]
             List of IDs of users to be added.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> group_id = '...'
         >>> members = ['...']
         >>> client.add_members_to_group(group_id, members)
@@ -2960,32 +2964,32 @@
                 'addedParticipants': user_ids,
                 'conversationId': group_id
             },
             'queryId': get_query_id(Endpoint.ADD_MEMBER_TO_GROUP)
         }
         response = self.http.post(
             Endpoint.ADD_MEMBER_TO_GROUP,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def change_group_name(self, group_id: str, name: str) -> Response:
         """Changes group name
 
         Parameters
         ----------
-        group_id : str
+        group_id : :class:`str`
             ID of the group to be renamed.
-        name : str
+        name : :class:`str`
             New name.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
         data = urlencode({
             'name': name
         })
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
@@ -3000,24 +3004,24 @@
         self, name: str, description: str = '', is_private: bool = False
     ) -> List:
         """
         Creates a list.
 
         Parameters
         ----------
-        name : str
+        name : :class:`str`
             The name of the list.
-        description : str, default=''
+        description : :class:`str`, default=''
             The description of the list.
-        is_private : bool, default=False
+        is_private : :class:`bool`, default=False
             Indicates whether the list is private (True) or public (False).
 
         Returns
         -------
-        List
+        list
             The created list.
 
         Examples
         --------
         >>> list = client.create_list(
         ...     'list name',
         ...     'list description',
@@ -3034,34 +3038,34 @@
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.CREATE_LIST)
         }
         response = self.http.post(
             Endpoint.CREATE_LIST,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         ).json()
         list_info = find_dict(response, 'list')[0]
         return List(self, list_info)
 
     def edit_list_banner(self, list_id: str, media_id: str) -> Response:
         """
         Edit the banner image of a list.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             The ID of the list.
-        media_id : str
+        media_id : :class:`str`
             The ID of the media to use as the new banner image.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> list_id = '...'
         >>> media_id = client.upload_media('image.png')
         >>> client.edit_list_banner(list_id, media_id)
@@ -3073,42 +3077,42 @@
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.EDIT_LIST_BANNER)
         }
         response = self.http.post(
             Endpoint.EDIT_LIST_BANNER,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def delete_list_banner(self, list_id: str) -> Response:
         """Deletes list banner.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             ID of the list from which the banner is to be removed.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
         data = {
             'variables': {
                 'listId': list_id
             },
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.DELETE_LIST_BANNER)
         }
         response = self.http.post(
             Endpoint.DELETE_LIST_BANNER,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def edit_list(
         self,
         list_id: str,
@@ -3117,27 +3121,27 @@
         is_private: bool | None = None
     ) -> List:
         """
         Edits list information.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             The ID of the list to edit.
-        name : str, default=None
+        name : :class:`str`, default=None
             The new name for the list.
-        description : str, default=None
+        description : :class:`str`, default=None
             The new description for the list.
-        is_private : bool, default=None
+        is_private : :class:`bool`, default=None
             Indicates whether the list should be private
             (True) or public (False).
 
         Returns
         -------
-        List
+        list
             The updated Twitter list.
 
         Examples
         --------
         >>> client.edit_list(
         ...     'new name', 'new description', True
         ... )
@@ -3154,34 +3158,34 @@
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.UPDATE_LIST)
         }
         response = self.http.post(
             Endpoint.UPDATE_LIST,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         ).json()
         list_info = find_dict(response, 'list')[0]
         return List(self, list_info)
 
     def add_list_member(self, list_id: str, user_id: str) -> Response:
         """
         Adds a user to a list.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             The ID of the list.
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to add to the list.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> client.add_list_member('list id', 'user id')
         """
         variables = {
@@ -3191,33 +3195,33 @@
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.LIST_ADD_MEMBER)
         }
         response = self.http.post(
             Endpoint.LIST_ADD_MEMBER,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def remove_list_member(self, list_id: str, user_id: str) -> Response:
         """
         Removes a user from a list.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             The ID of the list.
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to remove from the list.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> client.remove_list_member('list id', 'user id')
         """
         variables = {
@@ -3227,33 +3231,33 @@
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.LIST_REMOVE_MEMBER)
         }
         response = self.http.post(
             Endpoint.LIST_REMOVE_MEMBER,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     def get_lists(
         self, count: int = 100, cursor: str = None
     ) -> Result[List]:
         """
         Retrieves a list of user lists.
 
         Parameters
         ----------
-        count : int
+        count : :class:`int`
             The number of lists to retrieve.
 
         Returns
         -------
-        Result[List]
+        Result[:class:`List`]
             Retrieved lists.
 
         Examples
         --------
         >>> lists = client.get_lists()
         >>> for list_ in lists:
         ...     print(list_)
@@ -3264,18 +3268,18 @@
         >>> more_lists = lists.next()  # Retrieve more lists
         """
         variables = {
             'count': count
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         response = self.http.get(
             Endpoint.LIST_MANAGEMENT,
             params=params,
             headers=self._base_headers
         ).json()
 
         entries = find_dict(response, 'entries')[0]
@@ -3290,36 +3294,36 @@
                 List(self, list['item']['itemContent']['list'])
             )
 
         next_cursor = entries[-1]['content']['value']
 
         return Result(
             lists,
-            lambda: self.get_lists(count, next_cursor),
+            partial(self.get_lists, count, next_cursor),
             next_cursor
         )
 
     def get_list(self, list_id: str) -> List:
         """
         Retrieve list by ID.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             The ID of the list to retrieve.
 
         Returns
         -------
-        List
+        :class:`List`
             List object.
         """
-        params = {
-            'variables': json.dumps({'listId': list_id}),
-            'features': json.dumps(LIST_FEATURES)
-        }
+        params = flatten_params({
+            'variables': {'listId': list_id},
+            'features': LIST_FEATURES
+        })
         response = self.http.get(
             Endpoint.LIST_BY_REST_ID,
             params=params,
             headers=self._base_headers
         ).json()
         list_info = find_dict(response, 'list')[0]
         return List(self, list_info)
@@ -3328,24 +3332,24 @@
         self, list_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[Tweet]:
         """
         Retrieves tweets from a list.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             The ID of the list to retrieve tweets from.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of tweets to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             The cursor for pagination.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing the retrieved tweets.
 
         Examples
         --------
         >>> tweets = client.get_list_tweets('list id')
         >>> for tweet in tweets:
         ...    print(tweet)
@@ -3364,18 +3368,18 @@
         """
         variables = {
             'listId': list_id,
             'count': count
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         response = self.http.get(
             Endpoint.LIST_LATEST_TWEETS,
             params=params,
             headers=self._base_headers
         ).json()
 
         items = find_dict(response, 'entries')[0]
@@ -3389,15 +3393,15 @@
             if tweet_info['__typename'] == 'TweetWithVisibilityResults':
                 tweet_info = tweet_info['tweet']
             user_info = find_dict(tweet_info, 'result')[0]
             results.append(Tweet(self, tweet_info, User(self, user_info)))
 
         return Result(
             results,
-            lambda: self.get_list_tweets(list_id, count, next_cursor),
+            partial(self.get_list_tweets, list_id, count, next_cursor),
             next_cursor
         )
 
     def _get_list_users(
         self, endpoint: str, list_id: str, count: int, cursor: str
     ) -> Result[User]:
         """
@@ -3405,18 +3409,18 @@
         """
         variables = {
             'listId': list_id,
             'count': count,
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         response = self.http.get(
             endpoint,
             params=params,
             headers=self._base_headers
         ).json()
 
         items = find_dict(response, 'entries')[0]
@@ -3428,34 +3432,34 @@
                 results.append(User(self, user_info))
             elif entry_id.startswith('cursor-bottom'):
                 next_cursor = item['content']['value']
                 break
 
         return Result(
             results,
-            lambda: self._get_list_users(
-                endpoint, list_id, count, next_cursor),
+            partial(self._get_list_users,
+                    endpoint, list_id, count, next_cursor),
             next_cursor
         )
 
     def get_list_members(
         self, list_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """Retrieves members of a list.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             List ID.
-        count : int, default=20
+        count : :class:`int`, default=20
             Number of members to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             Members of a list
 
         Examples
         --------
         >>> members = client.get_list_members(123456789)
         >>> for member in members:
         ...     print(member)
@@ -3475,22 +3479,22 @@
     def get_list_subscribers(
         self, list_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """Retrieves subscribers of a list.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             List ID.
-        count : int, default=20
+        count : :class:`int`, default=20
             Number of subscribers to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             Subscribers of a list
 
         Examples
         --------
         >>> members = client.get_list_subscribers(123456789)
         >>> for subscriber in subscribers:
         ...     print(subscriber)
@@ -3516,24 +3520,23 @@
         """
         Retrieve notifications based on the provided type.
 
         Parameters
         ----------
         type : {'All', 'Verified', 'Mentions'}
             Type of notifications to retrieve.
-
             All: All notifications
             Verified: Notifications relating to authenticated users
             Mentions: Notifications with mentions
-        count : int, default=40
+        count : :class:`int`, default=40
             Number of notifications to retrieve.
 
         Returns
         -------
-        Result[Notification]
+        Result[:class:`Notification`]
             List of retrieved notifications.
 
         Examples
         --------
         >>> notifications = client.get_notifications('All')
         >>> for notification in notifications:
         ...     print(notification)
@@ -3606,10 +3609,10 @@
         if cursor_bottom_entry:
             next_cursor = find_dict(cursor_bottom_entry[0], 'value')[0]
         else:
             next_cursor = None
 
         return Result(
             notifications,
-            lambda: self.get_notifications(type, count, next_cursor),
+            partial(self.get_notifications, type, count, next_cursor),
             next_cursor
         )
```

### Comparing `twikit-1.4.4/twikit/errors.py` & `twikit-1.4.5/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.4/twikit/group.py` & `twikit-1.4.5/twikit/twikit_async/group.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
 class Group:
     """
     Represents a group.
 
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The ID of the group.
-    name : str | None
+    name : :class:`str` | None
         The name of the group.
-    members : list[str]
+    members : list[:class:`str`]
         Member IDs
     """
     def __init__(self, client: Client, group_id: str, data: dict) -> None:
         self._client = client
         self.id = group_id
 
         entries = data['conversation_timeline']['entries']
@@ -37,218 +37,224 @@
             name_update_log['conversation_name_update']['conversation_name']
             if name_update_log else None
         )
 
         members = data['conversation_timeline']['users'].values()
         self.members: list[str] = [i['id_str'] for i in members]
 
-    def get_history(self, max_id: str | None = None) -> Result[GroupMessage]:
+    async def get_history(
+        self, max_id: str | None = None
+    ) -> Result[GroupMessage]:
         """
         Retrieves the DM conversation history in the group.
 
         Parameters
         ----------
-        max_id : str, default=None
+        max_id : :class:`str`, default=None
             If specified, retrieves messages older than the specified max_id.
 
         Returns
         -------
-        Result[GroupMessage]
+        Result[:class:`GroupMessage`]
             A Result object containing a list of GroupMessage objects
             representing the DM conversation history.
 
         Examples
         --------
-        >>> messages = group.get_history()
+        >>> messages = await group.get_history()
         >>> for message in messages:
         >>>     print(message)
         <GroupMessage id="...">
         <GroupMessage id="...">
         ...
         ...
 
-        >>> more_messages = messages.next()  # Retrieve more messages
+        >>> more_messages = await messages.next()  # Retrieve more messages
         >>> for message in more_messages:
         >>>     print(message)
         <GroupMessage id="...">
         <GroupMessage id="...">
         ...
         ...
         """
-        return self._client.get_group_dm_history(self.id, max_id)
+        return await self._client.get_group_dm_history(self.id, max_id)
 
-    def add_members(self, user_ids: list[str]) -> Response:
+    async def add_members(self, user_ids: list[str]) -> Response:
         """Adds members to the group.
 
         Parameters
         ----------
-        user_ids : list[str]
+        user_ids : list[:class:`str`]
             List of IDs of users to be added.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> members = ['...']
-        >>> group.add_members(members)
+        >>> await group.add_members(members)
         """
-        return self._client.add_members_to_group(self.id, user_ids)
+        return await self._client.add_members_to_group(self.id, user_ids)
 
-    def change_name(self, name: str) -> Response:
+    async def change_name(self, name: str) -> Response:
         """Changes group name
 
         Parameters
         ----------
-        name : str
+        name : :class:`str`
             New name.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
-        return self._client.change_group_name(self.id, name)
+        return await self._client.change_group_name(self.id, name)
 
-    def send_message(
+    async def send_message(
         self,
         text: str,
         media_id: str | None = None,
         reply_to: str | None = None
     ) -> GroupMessage:
         """
         Sends a message to the group.
 
         Parameters
         ----------
-        text : str
+        text : :class:`str`
             The text content of the direct message.
-        media_id : str, default=None
+        media_id : :class:`str`, default=None
             The media ID associated with any media content
             to be included in the message.
             Media ID can be received by using the :func:`.upload_media` method.
-        reply_to : str, default=None
+        reply_to : :class:`str`, default=None
             Message ID to reply to.
 
         Returns
         -------
-        GroupMessage
+        :class:`GroupMessage`
             `Message` object containing information about the message sent.
 
         Examples
         --------
         >>> # send DM with media
         >>> group_id = '000000000'
-        >>> media_id = client.upload_media('image.png')
-        >>> message = group.send_message('text', media_id)
+        >>> media_id = await client.upload_media('image.png')
+        >>> message = await group.send_message('text', media_id)
         >>> print(message)
         <GroupMessage id='...'>
         """
-        return self._client.send_dm_to_group(self.id, text, media_id, reply_to)
+        return await self._client.send_dm_to_group(
+            self.id, text, media_id, reply_to
+        )
 
-    def update(self) -> None:
-        new = self._client.get_group(self.id)
+    async def update(self) -> None:
+        new = await self._client.get_group(self.id)
         self.__dict__.update(new.__dict__)
 
     def __repr__(self) -> str:
         return f'<Group id="{self.id}">'
 
 
 class GroupMessage(Message):
     """
     Represents a direct message.
 
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The ID of the message.
-    time : str
+    time : :class:`str`
         The timestamp of the message.
-    text : str
+    text : :class:`str`
         The text content of the message.
-    attachment : str
+    attachment : :class:`str`
         The media URL associated with any attachment in the message.
-    group_id : str
+    group_id : :class:`str`
         The ID of the group.
     """
     def __init__(
         self,
         client: Client,
         data: dict,
         sender_id: str,
         group_id: str
     ) -> None:
         super().__init__(client, data, sender_id, None)
         self.group_id = group_id
 
-    def group(self) -> Group:
+    async def group(self) -> Group:
         """
         Gets the group to which the message was sent.
         """
-        return self._client.get_group(self.group_id)
+        return await self._client.get_group(self.group_id)
 
-    def reply(self, text: str, media_id: str | None = None) -> GroupMessage:
+    async def reply(
+        self, text: str, media_id: str | None = None
+    ) -> GroupMessage:
         """Replies to the message.
 
         Parameters
         ----------
-        text : str
+        text : :class:`str`
             The text content of the direct message.
-        media_id : str, default=None
+        media_id : :class:`str`, default=None
             The media ID associated with any media content
             to be included in the message.
             Media ID can be received by using the :func:`.upload_media` method.
 
         Returns
         -------
-        Message
+        :class:`Message`
             `GroupMessage` object containing information about
             the message sent.
 
         See Also
         --------
         Client.send_dm_to_group
         """
-        return self._client.send_dm_to_group(
+        return await self._client.send_dm_to_group(
             self.group_id, text, media_id, self.id
         )
 
-    def add_reaction(self, emoji: str) -> Response:
+    async def add_reaction(self, emoji: str) -> Response:
         """
         Adds a reaction to the message.
 
         Parameters
         ----------
-        emoji : str
+        emoji : :class:`str`
             The emoji to be added as a reaction.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
-        return self._client.add_reaction_to_message(
+        return await self._client.add_reaction_to_message(
             self.id, self.group_id, emoji
         )
 
-    def remove_reaction(self, emoji: str) -> Response:
+    async def remove_reaction(self, emoji: str) -> Response:
         """
         Removes a reaction from the message.
 
         Parameters
         ----------
-        emoji : str
+        emoji : :class:`str`
             The emoji to be removed.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
-        return self._client.remove_reaction_from_message(
+        return await self._client.remove_reaction_from_message(
             self.id, self.group_id, emoji
         )
 
     def __repr__(self) -> str:
         return f'<GroupMessage id="{self.id}">'
```

### Comparing `twikit-1.4.4/twikit/http.py` & `twikit-1.4.5/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.4/twikit/list.py` & `twikit-1.4.5/twikit/twikit_async/list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import TYPE_CHECKING, Literal
 
-from .utils import timestamp_to_datetime
+from ..utils import timestamp_to_datetime
 
 if TYPE_CHECKING:
     from httpx import Response
 
     from .client import Client
     from .tweet import Tweet
     from .user import User
@@ -16,40 +16,40 @@
 
 class List:
     """
     Class representing a Twitter List.
 
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The unique identifier of the List.
-    created_at : int
+    created_at : :class:`int`
         The timestamp when the List was created.
-    default_banner : dict
+    default_banner : :class:`dict`
         Information about the default banner of the List.
-    banner : dict
+    banner : :class:`dict`
         Information about the banner of the List. If custom banner is not set,
         it defaults to the default banner.
-    description : str
+    description : :class:`str`
         The description of the List.
-    following : bool
+    following : :class:`bool`
         Indicates if the authenticated user is following the List.
-    is_member : bool
+    is_member : :class:`bool`
         Indicates if the authenticated user is a member of the List.
-    member_count : int
+    member_count : :class:`int`
         The number of members in the List.
-    mode : Literal['Private', 'Public']
+    mode : {'Private', 'Public'}
         The mode of the List, either 'Private' or 'Public'.
-    muting : bool
+    muting : :class:`bool`
         Indicates if the authenticated user is muting the List.
-    name : str
+    name : :class:`str`
         The name of the List.
-    pinning : bool
+    pinning : :class:`bool`
         Indicates if the List is pinned.
-    subscriber_count : int
+    subscriber_count : :class:`int`
         The number of subscribers to the List.
     """
     def __init__(self, client: Client, data: dict) -> None:
         self._client = client
 
         self.id: str = data['id_str']
         self.created_at: int = data['created_at']
@@ -70,181 +70,183 @@
         self.pinning: bool = data['pinning']
         self.subscriber_count: int = data['subscriber_count']
 
     @property
     def created_at_datetime(self) -> datetime:
         return timestamp_to_datetime(self.created_at)
 
-    def edit_banner(self, media_id: str) -> Response:
+    async def edit_banner(self, media_id: str) -> Response:
         """
         Edit the banner image of the list.
 
         Parameters
         ----------
-        media_id : str
+        media_id : :class:`str`
             The ID of the media to use as the new banner image.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
-        >>> media_id = client.upload_media('image.png')
-        >>> media.edit_banner(media_id)
+        >>> media_id = await client.upload_media('image.png')
+        >>> await media.edit_banner(media_id)
         """
-        return self._client.edit_list_banner(self.id, media_id)
+        return await self._client.edit_list_banner(self.id, media_id)
 
-    def delete_banner(self) -> Response:
+    async def delete_banner(self) -> Response:
         """
         Deletes the list banner.
         """
-        return self._client.delete_list_banner(self.id)
+        return await self._client.delete_list_banner(self.id)
 
-    def edit(
+    async def edit(
         self,
         name: str | None = None,
         description: str | None = None,
         is_private: bool | None = None
     ) -> List:
         """
         Edits list information.
 
         Parameters
         ----------
-        name : str, default=None
+        name : :class:`str`, default=None
             The new name for the list.
-        description : str, default=None
+        description : :class:`str`, default=None
             The new description for the list.
-        is_private : bool, default=None
+        is_private : :class:`bool`, default=None
             Indicates whether the list should be private
             (True) or public (False).
 
         Returns
         -------
-        List
+        :class:`List`
             The updated Twitter list.
 
         Examples
         --------
-        >>> list.edit(
+        >>> await list.edit(
         ...     'new name', 'new description', True
         ... )
         """
-        return self._client.edit_list(self.id, name, description, is_private)
+        return await self._client.edit_list(
+            self.id, name, description, is_private
+        )
 
-    def add_member(self, user_id: str) -> Response:
+    async def add_member(self, user_id: str) -> Response:
         """
         Adds a member to the list.
         """
-        return self._client.add_list_member(self.id, user_id)
+        return await self._client.add_list_member(self.id, user_id)
 
-    def remove_member(self, user_id: str) -> Response:
+    async def remove_member(self, user_id: str) -> Response:
         """
         Removes a member from the list.
         """
-        return self._client.remove_list_member(self.id, user_id)
+        return await self._client.remove_list_member(self.id, user_id)
 
-    def get_tweets(
+    async def get_tweets(
         self, count: int = 20, cursor: str | None = None
     ) -> Result[Tweet]:
         """
         Retrieves tweets from the list.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of tweets to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             The cursor for pagination.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing the retrieved tweets.
 
         Examples
         --------
-        >>> tweets = list.get_tweets()
+        >>> tweets = await list.get_tweets()
         >>> for tweet in tweets:
         ...    print(tweet)
         <Tweet id="...">
         <Tweet id="...">
         ...
         ...
 
-        >>> more_tweets = tweets.next()  # Retrieve more tweets
+        >>> more_tweets = await tweets.next()  # Retrieve more tweets
         >>> for tweet in more_tweets:
         ...     print(tweet)
         <Tweet id="...">
         <Tweet id="...">
         ...
         ...
         """
-        return self._client.get_list_tweets(self.id, count, cursor)
+        return await self._client.get_list_tweets(self.id, count, cursor)
 
-    def get_members(
+    async def get_members(
         self, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """Retrieves members of the list.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             Number of members to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             Members of the list
 
         Examples
         --------
         >>> members = list_.get_members()
         >>> for member in members:
         ...     print(member)
         <User id="...">
         <User id="...">
         ...
         ...
         >>> more_members = members.next()  # Retrieve more members
         """
-        return self._client.get_list_members(self.id, count, cursor)
+        return await self._client.get_list_members(self.id, count, cursor)
 
-    def get_subscribers(
+    async def get_subscribers(
         self, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """Retrieves subscribers of the list.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             Number of subscribers to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             Subscribers of the list
 
         Examples
         --------
         >>> subscribers = list_.get_subscribers()
         >>> for subscriber in subscribers:
         ...     print(subscriber)
         <User id="...">
         <User id="...">
         ...
         ...
         >>> more_subscribers = subscribers.next()  # Retrieve more subscribers
         """
-        return self._client.get_list_subscribers(self.id, count, cursor)
+        return await self._client.get_list_subscribers(self.id, count, cursor)
 
-    def update(self) -> None:
-        new = self._client.get_list(self.id)
+    async def update(self) -> None:
+        new = await self._client.get_list(self.id)
         self.__dict__.update(new.__dict__)
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, List) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
         return not self == __value
```

### Comparing `twikit-1.4.4/twikit/message.py` & `twikit-1.4.5/twikit/twikit_async/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 class Message:
     """
     Represents a direct message.
 
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The ID of the message.
-    time : str
+    time : :class:`str`
         The timestamp of the message.
-    text : str
+    text : :class:`str`
         The text content of the message.
-    attachment : dict
+    attachment : :class:`dict`
         Attachment Information.
     """
     def __init__(
         self,
         client: Client,
         data: dict,
         sender_id: str,
@@ -35,107 +35,107 @@
         self.recipient_id = recipient_id
 
         self.id: str = data['id']
         self.time: str = data['time']
         self.text: str = data['text']
         self.attachment: dict | None = data.get('attachment')
 
-    def reply(self, text: str, media_id: str | None = None) -> Message:
+    async def reply(self, text: str, media_id: str | None = None) -> Message:
         """Replies to the message.
 
         Parameters
         ----------
-        text : str
+        text : :class:`str`
             The text content of the direct message.
-        media_id : str, default=None
+        media_id : :class:`str`, default=None
             The media ID associated with any media content
             to be included in the message.
             Media ID can be received by using the :func:`.upload_media` method.
 
         Returns
         -------
-        Message
+        :class:`Message`
             `Message` object containing information about the message sent.
 
         See Also
         --------
         Client.send_dm
         """
-        user_id = self._client.user_id()
+        user_id = await self._client.user_id()
         send_to = (
             self.recipient_id
             if user_id == self.sender_id else
             self.sender_id
         )
-        return self._client.send_dm(send_to, text, media_id, self.id)
+        return await self._client.send_dm(send_to, text, media_id, self.id)
 
-    def add_reaction(self, emoji: str) -> Response:
+    async def add_reaction(self, emoji: str) -> Response:
         """
         Adds a reaction to the message.
 
         Parameters
         ----------
-        emoji : str
+        emoji : :class:`str`
             The emoji to be added as a reaction.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
-        user_id = self._client.user_id()
+        user_id = await self._client.user_id()
         partner_id = (
             self.recipient_id
             if user_id == self.sender_id else
             self.sender_id
         )
         conversation_id = f'{partner_id}-{user_id}'
-        return self._client.add_reaction_to_message(
+        return await self._client.add_reaction_to_message(
             self.id, conversation_id, emoji
         )
 
-    def remove_reaction(self, emoji: str) -> Response:
+    async def remove_reaction(self, emoji: str) -> Response:
         """
         Removes a reaction from the message.
 
         Parameters
         ----------
-        emoji : str
+        emoji : :class:`str`
             The emoji to be removed.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
-        user_id = self._client.user_id()
+        user_id = await self._client.user_id()
         partner_id = (
             self.recipient_id
             if user_id == self.sender_id else
             self.sender_id
         )
         conversation_id = f'{partner_id}-{user_id}'
-        return self._client.remove_reaction_from_message(
+        return await self._client.remove_reaction_from_message(
             self.id, conversation_id, emoji
         )
 
-    def delete(self) -> Response:
+    async def delete(self) -> Response:
         """
         Deletes the message.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.delete_dm
         """
-        return self._client.delete_dm(self.id)
+        return await self._client.delete_dm(self.id)
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, Message) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
         return not self == __value
```

### Comparing `twikit-1.4.4/twikit/notification.py` & `twikit-1.4.5/twikit/notification.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,25 @@
     from .user import User
 
 
 class Notification:
     """
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The unique identifier of the notification.
-    timestamp_ms : int
+    timestamp_ms : :class:`int`
         The timestamp of the notification in milliseconds.
-    icon : dict
+    icon : :class:`dict`
         Dictionary containing icon data for the notification.
-    message : str
+    message : :class:`str`
         The message text of the notification.
-    tweet : Tweet
+    tweet : :class:`Tweet`
         The tweet associated with the notification.
-    from_user : User
+    from_user : :class:`User`
         The user who triggered the notification.
     """
     def __init__(
         self, client: Client, data: dict, tweet: Tweet, from_user: User
     ) -> None:
         self._client = client
         self.tweet = tweet
```

### Comparing `twikit-1.4.4/twikit/trend.py` & `twikit-1.4.5/twikit/trend.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     from .client import Client
 
 
 class Trend:
     """
     Attributes
     ----------
-    name : str
+    name : :class:`str`
         The name of the trending topic.
-    tweets_count : int
+    tweets_count : :class:`int`
         The count of tweets associated with the trend.
-    domain_context : str
+    domain_context : :class:`str`
         The context or domain associated with the trend.
-    grouped_trends : list[str]
+    grouped_trends : list[:class:`str`]
         A list of trend names grouped under the main trend.
     """
 
     def __init__(self, client: Client, data: dict) -> None:
         self._client = client
 
         metadata: dict = data['trendMetadata']
```

### Comparing `twikit-1.4.4/twikit/tweet.py` & `twikit-1.4.5/twikit/twikit_async/tweet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,83 @@
 from __future__ import annotations
 
 import re
 from datetime import datetime
 from typing import TYPE_CHECKING
 
+from ..utils import find_dict, timestamp_to_datetime
 from .user import User
-from .utils import find_dict, timestamp_to_datetime
 
 if TYPE_CHECKING:
     from httpx import Response
 
     from .client import Client
     from .utils import Result
 
 
 class Tweet:
     """
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The unique identifier of the tweet.
-    created_at : str
+    created_at : :class:`str`
         The date and time when the tweet was created.
-    created_at_datetime : datetime
+    created_at_datetime : :class:`datetime`
         The created_at converted to datetime.
-    user: User
+    user: :class:`User`
         Author of the tweet.
-    text : str
+    text : :class:`str`
         The full text of the tweet.
-    lang : str
+    lang : :class:`str`
         The language of the tweet.
-    in_reply_to : str
+    in_reply_to : :class:`str`
         The tweet ID this tweet is in reply to, if any
-    is_quote_status : bool
+    is_quote_status : :class:`bool`
         Indicates if the tweet is a quote status.
-    quote : Tweet
+    quote : :class:`Tweet`
         The Tweet being quoted (if any)
-    retweeted : bool
+    retweeted : :class:`bool`
         Whether the tweet is a retweet
-    possibly_sensitive : bool
+    possibly_sensitive : :class:`bool`
         Indicates if the tweet content may be sensitive.
-    possibly_sensitive_editable : bool
+    possibly_sensitive_editable : :class:`bool`
         Indicates if the tweet's sensitivity can be edited.
-    quote_count : int
+    quote_count : :class:`int`
         The count of quotes for the tweet.
-    media : list
+    media : :class:`list`
         A list of media entities associated with the tweet.
-    reply_count : int
+    reply_count : :class:`int`
         The count of replies to the tweet.
-    favorite_count : int
+    favorite_count : :class:`int`
         The count of favorites or likes for the tweet.
-    favorited : bool
+    favorited : :class:`bool`
         Indicates if the tweet is favorited.
-    view_count: int
+    view_count: :class:`int`
         The count of views.
-    retweet_count : int
+    retweet_count : :class:`int`
         The count of retweets for the tweet.
-    editable_until_msecs : int
+    editable_until_msecs : :class:`int`
         The timestamp until which the tweet is editable.
-    is_translatable : bool
+    is_translatable : :class:`bool`
         Indicates if the tweet is translatable.
-    is_edit_eligible : bool
+    is_edit_eligible : :class:`bool`
         Indicates if the tweet is eligible for editing.
-    edits_remaining : int
+    edits_remaining : :class:`int`
         The remaining number of edits allowed for the tweet.
-    state : str
+    state : :class:`str`
         The state of the tweet views.
-    replies: Result[Tweet] | None
+    replies: Result[:class:`Tweet`] | None
         Replies to the tweet.
-    reply_to: list[Tweet] | None
+    reply_to: list[:class:`Tweet`] | None
         A list of Tweet objects representing the tweets to which to reply.
-    related_tweets : list[Tweet] | None
+    related_tweets : list[:class:`Tweet`] | None
         Related tweets.
-    hashtags: list[str]
+    hashtags: list[:class:`str`]
         Hashtags included in the tweet text.
-    poll : Poll
-        Poll attached to the tweet.
     """
 
     def __init__(self, client: Client, data: dict, user: User = None) -> None:
         self._client = client
         self._data = data
         self.user = user
 
@@ -174,226 +172,226 @@
     def created_at_datetime(self) -> datetime:
         return timestamp_to_datetime(self.created_at)
 
     @property
     def poll(self) -> Poll:
         return self._poll_data and Poll(self._client, self._poll_data, self)
 
-    def delete(self) -> Response:
+    async def delete(self) -> Response:
         """Deletes the tweet.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
-        >>> tweet.delete()
+        >>> await tweet.delete()
         """
-        return self._client.delete_tweet(self.id)
+        return await self._client.delete_tweet(self.id)
 
-    def favorite(self) -> Response:
+    async def favorite(self) -> Response:
         """
         Favorites the tweet.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.favorite_tweet
         """
-        return self._client.favorite_tweet(self.id)
+        return await self._client.favorite_tweet(self.id)
 
-    def unfavorite(self) -> Response:
+    async def unfavorite(self) -> Response:
         """
         Favorites the tweet.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.unfavorite_tweet
         """
-        return self._client.unfavorite_tweet(self.id)
+        return await self._client.unfavorite_tweet(self.id)
 
-    def retweet(self) -> Response:
+    async def retweet(self) -> Response:
         """
         Retweets the tweet.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.retweet
         """
-        return self._client.retweet(self.id)
+        return await self._client.retweet(self.id)
 
-    def delete_retweet(self) -> Response:
+    async def delete_retweet(self) -> Response:
         """
         Deletes the retweet.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.delete_retweet
         """
-        return self._client.delete_retweet(self.id)
+        return await self._client.delete_retweet(self.id)
 
-    def bookmark(self) -> Response:
+    async def bookmark(self) -> Response:
         """
         Adds the tweet to bookmarks.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.bookmark_tweet
         """
-        return self._client.bookmark_tweet(self.id)
+        return await self._client.bookmark_tweet(self.id)
 
-    def delete_bookmark(self) -> Response:
+    async def delete_bookmark(self) -> Response:
         """
         Removes the tweet from bookmarks.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.delete_bookmark
         """
-        return self._client.delete_bookmark(self.id)
+        return await self._client.delete_bookmark(self.id)
 
-    def reply(
+    async def reply(
         self,
         text: str = '',
         media_ids: list[str] | None = None,
         **kwargs
     ) -> Tweet:
         """
         Replies to the tweet.
 
         Parameters
         ----------
-        text : str, default=''
+        text : :class:`str`, default=''
             The text content of the reply.
-        media_ids : list[str], default=None
+        media_ids : list[:class:`str`], default=None
             A list of media IDs or URIs to attach to the reply.
             Media IDs can be obtained by using the `upload_media` method.
 
         Returns
         -------
-        Tweet
+        :class:`Tweet`
             The created tweet.
 
         Examples
         --------
         >>> tweet_text = 'Example text'
         >>> media_ids = [
         ...     client.upload_media('image1.png'),
         ...     client.upload_media('image2.png')
         ... ]
-        >>> tweet.reply(
+        >>> await tweet.reply(
         ...     tweet_text,
         ...     media_ids=media_ids
         ... )
 
         See Also
         --------
         `Client.upload_media`
         """
-        return self._client.create_tweet(
+        return await self._client.create_tweet(
             text, media_ids, reply_to=self.id, **kwargs
         )
 
-    def get_retweeters(
+    async def get_retweeters(
         self, count: str = 40, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieve users who retweeted the tweet.
 
         Parameters
         ----------
-        count : int, default=40
+        count : :class:`int`, default=40
             The maximum number of users to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A string indicating the position of the cursor for pagination.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of users who retweeted the tweet.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> retweeters = tweet.get_retweeters()
         >>> print(retweeters)
         [<User id="...">, <User id="...">, ..., <User id="...">]
 
         >>> more_retweeters = retweeters.next()  # Retrieve more retweeters.
         >>> print(more_retweeters)
         [<User id="...">, <User id="...">, ..., <User id="...">]
         """
-        return self._client.get_retweeters(self.id, count, cursor)
+        return await self._client.get_retweeters(self.id, count, cursor)
 
-    def get_favoriters(
+    async def get_favoriters(
         self, count: str = 40, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieve users who favorited a specific tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet.
-        count : int, default=40
+        count : :class:`int`, default=40
             The maximum number of users to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A string indicating the position of the cursor for pagination.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of users who favorited the tweet.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> favoriters = tweet.get_favoriters()
         >>> print(favoriters)
         [<User id="...">, <User id="...">, ..., <User id="...">]
 
         >>> more_favoriters = favoriters.next()  # Retrieve more favoriters.
         >>> print(more_favoriters)
         [<User id="...">, <User id="...">, ..., <User id="...">]
         """
-        return self._client.get_favoriters(self.id, count, cursor)
+        return await self._client.get_favoriters(self.id, count, cursor)
 
-    def update(self) -> None:
-        new = self._client.get_tweet_by_id(self.id)
+    async def update(self) -> None:
+        new = await self._client.get_tweet_by_id(self.id)
         self.__dict__.update(new.__dict__)
 
     def __repr__(self) -> str:
         return f'<Tweet id="{self.id}">'
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, Tweet) and self.id == __value.id
@@ -409,51 +407,50 @@
         self.id = data['rest_id']
         self.execute_at: int = data['scheduling_info']['execute_at']
         self.state: str = data['scheduling_info']['state']
         self.type: str = data['tweet_create_request']['type']
         self.text: str = data['tweet_create_request']['status']
         self.media = [i['media_info'] for i in data.get('media_entities', [])]
 
-    def delete(self) -> Response:
+    async def delete(self) -> Response:
         """
         Delete the scheduled tweet.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
-        return self._client.delete_scheduled_tweet(self.id)
+        return await self._client.delete_scheduled_tweet(self.id)
 
     def __repr__(self) -> str:
         return f'<ScheduledTweet id="{self.id}">'
 
 
 class Poll:
     """Represents a poll associated with a tweet.
-
     Attributes
     ----------
-    tweet : Tweet
+    tweet : :class:`Tweet`
         The tweet associated with the poll.
-    id : str
+    id : :class:`str`
         The unique identifier of the poll.
-    name : str
+    name : :class:`str`
         The name of the poll.
-    choices : list of dict
+    choices : list[:class:`dict`]
         A list containing dictionaries representing poll choices.
         Each dictionary contains 'label' and 'count' keys
         for choice label and count.
-    duration_minutes : int
+    duration_minutes : :class:`int`
         The duration of the poll in minutes.
-    end_datetime_utc : str
+    end_datetime_utc : :class:`str`
         The end date and time of the poll in UTC format.
-    last_updated_datetime_utc : str
+    last_updated_datetime_utc : :class:`str`
         The last updated date and time of the poll in UTC format.
-    selected_choice : str | None
+    selected_choice : :class:`str` | None
         Number of the selected choice.
     """
 
     def __init__(
         self, client: Client, data: dict, tweet: Tweet | None = None
     ) -> None:
         self._client = client
@@ -500,36 +497,34 @@
 
         if 'selected_choice' in binding_values:
             selected_choice = binding_values['selected_choice']['string_value']
             self.selected_choice: str = selected_choice
         else:
             self.selected_choice = None
 
-    def vote(self, selected_choice: str) -> Poll:
+    async def vote(self, selected_choice: str) -> Poll:
         """
         Vote on the poll with the specified selected choice.
-
         Parameters
         ----------
-        selected_choice : str
+        selected_choice : :class:`str`
             The label of the selected choice for the vote.
-
         Returns
         -------
-        Poll
+        :class:`Poll`
             The Poll object representing the updated poll after voting.
         """
-        return self._client.vote(
+        return await self._client.vote(
             selected_choice,
             self.id,
             self.tweet.id,
             self.name
         )
 
     def __repr__(self) -> str:
         return f'<Poll id="{self.id}">'
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, Poll) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
-        return not self == __value
+        return not self == __value
```

### Comparing `twikit-1.4.4/twikit/twikit_async/client.py` & `twikit-1.4.5/twikit/twikit_async/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import io
 import json
+from functools import partial
 from typing import Literal
 
 import filetype
 from fake_useragent import UserAgent
 from httpx import Response
 
 from ..errors import (
@@ -22,14 +23,15 @@
     LIST_FEATURES,
     TOKEN,
     USER_FEATURES,
     Endpoint,
     build_tweet_data,
     build_user_data,
     find_dict,
+    flatten_params,
     get_query_id,
     urlencode
 )
 from .group import Group, GroupMessage
 from .http import HTTPClient
 from .list import List
 from .message import Message
@@ -105,15 +107,15 @@
     def _get_csrf_token(self) -> str:
         """
         Retrieves the Cross-Site Request Forgery (CSRF) token from the
         current session's cookies.
 
         Returns
         -------
-        str
+        :class:`str`
             The CSRF token as a string.
         """
         return self.http.client.cookies.get('ct0')
 
     async def login(
         self,
         *,
@@ -127,22 +129,22 @@
         `auth_info_2` is optional and can be omitted, but it is
         recommended to provide if available.
         The order in which you specify authentication information
         (auth_info_1 and auth_info_2) is flexible.
 
         Parameters
         ----------
-        auth_info_1 : str
+        auth_info_1 : :class:`str`
             The first piece of authentication information,
             which can be a username, email address, or phone number.
-        auth_info_2 : str, default=None
+        auth_info_2 : :class:`str`, default=None
             The second piece of authentication information,
             which is optional but recommended to provide.
             It can be a username, email address, or phone number.
-        password : str
+        password : :class:`str`
             The password associated with the account.
 
         Examples
         --------
         >>> await client.login(
         ...     auth_info_1='example_user',
         ...     auth_info_2='email@example.com',
@@ -280,15 +282,15 @@
         """
         Save cookies to file in json format.
         You can skip the login procedure by loading the saved cookies
         using the :func:`load_cookies` method.
 
         Parameters
         ----------
-        path : str
+        path : :class:`str`
             The path to the file where the cookie will be stored.
 
         Examples
         --------
         >>> client.save_cookies('cookies.json')
 
         See Also
@@ -303,15 +305,15 @@
     def set_cookies(self, cookies: dict, clear_cookies: bool = False) -> None:
         """
         Sets cookies.
         You can skip the login procedure by loading a saved cookies.
 
         Parameters
         ----------
-        cookies : dict
+        cookies : :class:`dict`
             The cookies to be set as key value pair.
 
         Examples
         --------
         >>> with open('cookies.json', 'r', encoding='utf-8') as f:
         ...     client.set_cookies(json.load(f))
 
@@ -328,15 +330,15 @@
     def load_cookies(self, path: str) -> None:
         """
         Loads cookies from a file.
         You can skip the login procedure by loading a saved cookies.
 
         Parameters
         ----------
-        path : str
+        path : :class:`str`
             Path to the file where the cookie is stored.
 
         Examples
         --------
         >>> client.load_cookies('cookies.json')
 
         See Also
@@ -350,15 +352,15 @@
 
     def set_delegate_account(self, user_id: str | None) -> None:
         """
         Sets the account to act as.
 
         Parameters
         ----------
-        user_id : str | None
+        user_id : :class:`str` | None
             The user ID of the account to act as.
             Set to None to clear the delegated account.
         """
         self._act_as = user_id
 
     async def _search(
         self,
@@ -374,18 +376,18 @@
             'rawQuery': query,
             'count': count,
             'querySource': 'typed_query',
             'product': product
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         response = (await self.http.get(
             Endpoint.SEARCH_TIMELINE,
             params=params,
             headers=self._base_headers
         )).json()
 
         return response
@@ -399,26 +401,26 @@
     ) -> Result[Tweet]:
         """
         Searches for tweets based on the specified query and
         product type.
 
         Parameters
         ----------
-        query : str
+        query : :class:`str`
             The search query.
         product : {'Top', 'Latest', 'Media'}
             The type of tweets to retrieve.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of tweets to retrieve, between 1 and 20.
-        cursor : str, default=20
+        cursor : :class:`str`, default=20
             Token to retrieve more tweets.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             An instance of the `Result` class containing the
             search results.
 
         Examples
         --------
         >>> tweets = await client.search_tweet('query', 'Top')
         >>> for tweet in tweets:
@@ -482,51 +484,43 @@
                 )[0]
                 next_cursor = entries[-1]['content']['value']
                 previous_cursor = entries[-2]['content']['value']
             else:
                 next_cursor = instructions[-1]['entry']['content']['value']
                 previous_cursor = instructions[-2]['entry']['content']['value']
 
-        async def _fetch_next_result():
-            return await self.search_tweet(query, product, count, next_cursor)
-
-        async def _fetch_previous_result():
-            return await self.search_tweet(
-                query, product, count, previous_cursor
-            )
-
         return Result(
             results,
-            _fetch_next_result,
+            partial(self.search_tweet, query, product, count, next_cursor),
             next_cursor,
-            _fetch_previous_result,
+            partial(self.search_tweet, query, product, count, previous_cursor),
             previous_cursor
         )
 
     async def search_user(
         self,
         query: str,
         count: int = 20,
         cursor: str | None = None
     ) -> Result[User]:
         """
         Searches for users based on the provided query.
 
         Parameters
         ----------
-        query : str
+        query : :class:`str`
             The search query for finding users.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of users to retrieve in each request.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             Token to retrieve more users.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             An instance of the `Result` class containing the
             search results.
 
         Examples
         --------
         >>> result = await client.search_user('query')
         >>> for user in result:
@@ -551,20 +545,18 @@
         results = []
         for item in items:
             if 'itemContent' not in item['content']:
                 continue
             user_info = find_dict(item, 'result')[0]
             results.append(User(self, user_info))
 
-        async def _fetch_next_result():
-            return await self.search_user(query, count, next_cursor)
-
         return Result(
             results,
-            _fetch_next_result,
+            partial(self.search_user,
+                    query, count, next_cursor),
             next_cursor
         )
 
     async def upload_media(
         self,
         source: str | bytes,
         wait_for_completion: bool = False,
@@ -573,31 +565,31 @@
         media_category: str | None = None
     ) -> str:
         """
         Uploads media to twitter.
 
         Parameters
         ----------
-        source : str | bytes
+        source : :class:`str` | :class:`bytes`
             The source of the media to be uploaded.
             It can be either a file path or bytes of the media content.
-        wait_for_completion : bool, default=False
+        wait_for_completion : :class:`bool`, default=False
             Whether to wait for the completion of the media upload process.
-        status_check_interval : float, default=1.0
+        status_check_interval : :class:`float`, default=1.0
             The interval (in seconds) to check the status of the
             media upload process.
-        media_type : str, default=None
+        media_type : :class:`str`, default=None
             The MIME type of the media.
             If not specified, it will be guessed from the source.
-        media_category : str, default=None
+        media_category : :class:`str`, default=None
             The media category.
 
         Returns
         -------
-        str
+        :class:`str`
             The media ID of the uploaded media.
 
         Examples
         --------
         Videos, images and gifs can be uploaded.
 
         >>> media_id_1 = await client.upload_media(
@@ -726,15 +718,15 @@
 
     async def check_media_status(self, media_id: str) -> dict:
         """
         Check the status of uploaded media.
 
         Parameters
         ----------
-        media_id : str
+        media_id : :class:`str`
             The media ID of the uploaded media.
 
         Returns
         -------
         dict
             A dictionary containing information about the status of
             the uploaded media.
@@ -756,22 +748,22 @@
         duration_minutes: int
     ) -> str:
         """
         Creates a poll and returns card-uri.
 
         Parameters
         ----------
-        choices : list[str]
+        choices : list[:class:`str`]
             A list of choices for the poll. Maximum of 4 choices.
-        duration_minutes : int
+        duration_minutes : :class:`int`
             The duration of the poll in minutes.
 
         Returns
         -------
-        str
+        :class:`str`
             The URI of the created poll card.
 
         Examples
         --------
         Create a poll with three choices lasting for 60 minutes:
 
         >>> choices = ['Option A', 'Option B', 'Option C']
@@ -810,25 +802,25 @@
         tweet_id: str,
         card_name: str
     ) -> Poll:
         """
         Vote on a poll with the selected choice.
         Parameters
         ----------
-        selected_choice : str
+        selected_choice : :class:`str`
             The label of the selected choice for the vote.
-        card_uri : str
+        card_uri : :class:`str`
             The URI of the poll card.
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the original tweet containing the poll.
-        card_name : str
+        card_name : :class:`str`
             The name of the poll card.
         Returns
         -------
-        Poll
+        :class:`Poll`
             The Poll object representing the updated poll after voting.
         """
         data = urlencode({
             'twitter:string:card_uri': card_uri,
             'twitter:long:original_tweet_id': tweet_id,
             'twitter:string:response_card_name': card_name,
             'twitter:string:cards_platform': 'Web-12',
@@ -861,35 +853,39 @@
     ) -> Tweet:
         """
         Creates a new tweet on Twitter with the specified
         text, media, and poll.
 
         Parameters
         ----------
-        text : str, default=''
+        text : :class:`str`, default=''
             The text content of the tweet.
-        media_ids : list[str], default=None
+        media_ids : list[:class:`str`], default=None
             A list of media IDs or URIs to attach to the tweet.
             media IDs can be obtained by using the `upload_media` method.
-        poll_uri : str, default=None
+        poll_uri : :class:`str`, default=None
             The URI of a Twitter poll card to attach to the tweet.
             Poll URIs can be obtained by using the `create_poll` method.
-        reply_to : str, default=None
+        reply_to : :class:`str`, default=None
             The ID of the tweet to which this tweet is a reply.
         conversation_control : {'followers', 'verified', 'mentioned'}
             The type of conversation control for the tweet:
             - 'followers': Limits replies to followers only.
             - 'verified': Limits replies to verified accounts only.
             - 'mentioned': Limits replies to mentioned accounts only.
-        attachment_url : str
+        attachment_url : :class:`str`
             URL of the tweet to be quoted.
 
+        Raises
+        ------
+        :exc:`DuplicateTweet` : If the tweet is a duplicate of another tweet.
+
         Returns
         -------
-        Tweet
+        :class:`Tweet`
             The Created Tweet.
 
         Examples
         --------
         Create a tweet with media:
 
         >>> tweet_text = 'Example text'
@@ -958,15 +954,15 @@
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_TWEET),
             'features': FEATURES,
         }
         response = (await self.http.post(
             Endpoint.CREATE_TWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers,
         )).json()
 
         _result = find_dict(response, 'result')
         if not _result:
             raise_exceptions_from_response(response['errors'])
             raise CouldNotTweet(
@@ -986,24 +982,24 @@
         media_ids: list[str] | None = None,
     ) -> str:
         """
         Schedules a tweet to be posted at a specified timestamp.
 
         Parameters
         ----------
-        scheduled_at : int
+        scheduled_at : :class:`int`
             The timestamp when the tweet should be scheduled for posting.
-        text : str, default=''
+        text : :class:`str`, default=''
             The text content of the tweet, by default an empty string.
-        media_ids : list[str], default=None
+        media_ids : list[:class:`str`], default=None
             A list of media IDs to be attached to the tweet, by default None.
 
         Returns
         -------
-        str
+        :class:`str`
             The ID of the scheduled tweet.
 
         Examples
         --------
         Create a tweet with media:
 
         >>> scheduled_time = int(time.time()) + 3600  # One hour from now
@@ -1029,30 +1025,30 @@
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_SCHEDULED_TWEET),
         }
         response = (await self.http.post(
             Endpoint.CREATE_SCHEDULED_TWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers,
         )).json()
         return response['data']['tweet']['rest_id']
 
     async def delete_tweet(self, tweet_id: str) -> Response:
         """Deletes a tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             ID of the tweet to be deleted.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '0000000000'
         >>> await delete_tweet(tweet_id)
         """
@@ -1061,50 +1057,50 @@
                 'tweet_id': tweet_id,
                 'dark_request': False
             },
             'queryId': get_query_id(Endpoint.DELETE_TWEET)
         }
         response = await self.http.post(
             Endpoint.DELETE_TWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def get_user_by_screen_name(self, screen_name: str) -> User:
         """
         Fetches a user by screen name.
 
         Parameter
         ---------
-        screen_name : str
+        screen_name : :class:`str`
             The screen name of the Twitter user.
 
         Returns
         -------
-        User
+        :class:`User`
             An instance of the User class representing the
             Twitter user.
 
         Examples
         --------
         >>> target_screen_name = 'example_user'
         >>> user = await client.get_user_by_name(target_screen_name)
         >>> print(user)
         <User id="...">
         """
         variables = {
             'screen_name': screen_name,
             'withSafetyModeUserFields': False
         }
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(USER_FEATURES),
-            'fieldToggles': json.dumps({'withAuxiliaryUserLabels': False})
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': USER_FEATURES,
+            'fieldToggles': {'withAuxiliaryUserLabels': False}
+        })
         response = (await self.http.get(
             Endpoint.USER_BY_SCREEN_NAME,
             params=params,
             headers=self._base_headers
         )).json()
 
         if 'user' not in response['data']:
@@ -1117,38 +1113,38 @@
 
     async def get_user_by_id(self, user_id: str) -> User:
         """
         Fetches a user by ID
 
         Parameter
         ---------
-        user_id : str
+        user_id : :class:`str`
             The ID of the Twitter user.
 
         Returns
         -------
-        User
+        :class:`User`
             An instance of the User class representing the
             Twitter user.
 
         Examples
         --------
         >>> target_screen_name = '000000000'
         >>> user = await client.get_user_by_id(target_screen_name)
         >>> print(user)
         <User id="000000000">
         """
         variables = {
             'userId': user_id,
             'withSafetyModeUserFields': True
         }
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(USER_FEATURES),
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': USER_FEATURES
+        })
         response = (await self.http.get(
             Endpoint.USER_BY_REST_ID,
             params=params,
             headers=self._base_headers
         )).json()
         if 'result' not in response['data']['user']:
             raise TwitterException(f'Invalid user id: {user_id}')
@@ -1164,46 +1160,48 @@
             'withQuickPromoteEligibilityTweetFields': True,
             'withBirdwatchNotes': True,
             'withVoice': True,
             'withV2Timeline': True
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES),
-            'fieldToggles': json.dumps({'withAuxiliaryUserLabels': False})
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES,
+            'fieldToggles': {'withAuxiliaryUserLabels': False}
+        })
         response = (await self.http.get(
             Endpoint.TWEET_DETAIL,
             params=params,
             headers=self._base_headers
         )).json()
         return response
 
     async def _get_more_replies(
         self, tweet_id: str, cursor: str
     ) -> Result[Tweet]:
-        response =await self._get_tweet_detail(tweet_id, cursor)
+        response = await self._get_tweet_detail(tweet_id, cursor)
         entries = find_dict(response, 'entries')[0]
 
         results = []
         for entry in entries:
             if entry['entryId'].startswith('cursor'):
                 continue
             tweet_info = find_dict(entry, 'result')[0]
+            if tweet_info['__typename'] == 'TweetTombstone':
+                continue
             if tweet_info['__typename'] == 'TweetWithVisibilityResults':
                 tweet_info = tweet_info['tweet']
             user_info = tweet_info['core']['user_results']['result']
             results.append(Tweet(self, tweet_info, User(self, user_info)))
 
         if entries[-1]['entryId'].startswith('cursor'):
             next_cursor = entries[-1]['content']['itemContent']['value']
-            async def _fetch_next_result():
-                return await self._get_more_replies(tweet_id, next_cursor)
+            _fetch_next_result = partial(self._get_more_replies,
+                                         tweet_id, next_cursor)
         else:
             next_cursor = None
             _fetch_next_result = None
 
         return Result(
             results,
             _fetch_next_result,
@@ -1214,20 +1212,20 @@
         self, tweet_id: str, cursor: str | None = None
     ) -> Tweet:
         """
         Fetches a tweet by tweet ID.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet.
 
         Returns
         -------
-        Tweet
+        :class:`Tweet`
             A Tweet object representing the fetched tweet.
 
         Examples
         --------
         >>> target_tweet_id = '...'
         >>> tweet = client.get_tweet_by_id(target_tweet_id)
         >>> print(tweet)
@@ -1272,18 +1270,16 @@
                     reply_to.append(tweet_object)
                 else:
                     replies_list.append(tweet_object)
 
         if entries[-1]['entryId'].startswith('cursor'):
             # if has more replies
             reply_next_cursor = entries[-1]['content']['itemContent']['value']
-            async def _fetch_more_replies():
-                return await self._get_more_replies(
-                    tweet_id, reply_next_cursor
-                )
+            _fetch_more_replies = partial(self._get_more_replies,
+                                          tweet_id, reply_next_cursor)
         else:
             reply_next_cursor = None
             _fetch_more_replies = None
 
         tweet.replies = Result(
             replies_list,
             _fetch_more_replies,
@@ -1296,52 +1292,52 @@
 
     async def get_scheduled_tweets(self) -> list[ScheduledTweet]:
         """
         Retrieves scheduled tweets.
 
         Returns
         -------
-        list[ScheduledTweet]
+        list[:class:`ScheduledTweet`]
             List of ScheduledTweet objects representing the scheduled tweets.
         """
 
-        params = {
-            'variables': json.dumps({'ascending': True})
-        }
+        params = flatten_params({
+            'variables': {'ascending': True}
+        })
         response = (await self.http.get(
             Endpoint.FETCH_SCHEDULED_TWEETS,
             params=params,
             headers=self._base_headers
         )).json()
         tweets = find_dict(response, 'scheduled_tweet_list')[0]
         return [ScheduledTweet(self, tweet) for tweet in tweets]
 
     async def delete_scheduled_tweet(self, tweet_id: str) -> Response:
         """
         Delete a scheduled tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the scheduled tweet to delete.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
         data = {
             'variables': {
                 'scheduled_tweet_id': tweet_id
             },
             'queryId': get_query_id(Endpoint.DELETE_SCHEDULED_TWEET)
         }
         response = await self.http.post(
             Endpoint.DELETE_SCHEDULED_TWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def _get_tweet_engagements(
         self, tweet_id: str, count: int, cursor: str, endpoint: str,
     ) -> Result[User]:
@@ -1351,18 +1347,18 @@
         variables = {
             'tweetId': tweet_id,
             'count': count,
             'includePromotedContent': True
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         response = (await self.http.get(
             endpoint,
             params=params,
             headers=self._base_headers
         )).json()
         items_ = find_dict(response, 'entries')
         if not items_:
@@ -1377,50 +1373,42 @@
                 continue
             user_info_ = find_dict(item, 'result')
             if not user_info_:
                 continue
             user_info = user_info_[0]
             results.append(User(self, user_info))
 
-        async def _fetch_next_result():
-            return await self._get_tweet_engagements(
-                tweet_id, count, next_cursor, endpoint
-            )
-
-        async def _fetch_previous_result():
-            return await self._get_tweet_engagements(
-                tweet_id, count, previous_cursor, endpoint
-            )
-
         return Result(
             results,
-            _fetch_next_result,
+            partial(self._get_tweet_engagements,
+                    tweet_id, count, next_cursor, endpoint),
             next_cursor,
-            _fetch_previous_result,
+            partial(self._get_tweet_engagements,
+                    tweet_id, count, previous_cursor, endpoint),
             previous_cursor
         )
 
     async def get_retweeters(
         self, tweet_id: str, count: int = 40, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieve users who retweeted a specific tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet.
         count : int, default=40
             The maximum number of users to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A string indicating the position of the cursor for pagination.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of users who retweeted the tweet.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> retweeters = await client.get_retweeters(tweet_id)
         >>> print(retweeters)
@@ -1439,24 +1427,24 @@
         self, tweet_id: str, count: int = 40, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieve users who favorited a specific tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet.
         count : int, default=40
             The maximum number of users to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A string indicating the position of the cursor for pagination.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of users who favorited the tweet.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> favoriters = await client.get_favoriters(tweet_id)
         >>> print(favoriters)
@@ -1479,28 +1467,28 @@
         cursor: str | None = None
     ) -> Result[Tweet]:
         """
         Fetches tweets from a specific user's timeline.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the Twitter user whose tweets to retrieve.
             To get the user id from the screen name, you can use
             `get_user_by_screen_name` method.
         tweet_type : {'Tweets', 'Replies', 'Media', 'Likes'}
             The type of tweets to retrieve.
-        count : int, default=40
+        count : :class:`int`, default=40
             The number of tweets to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             The cursor for fetching the next set of results.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing a list of `Tweet` objects.
 
         Examples
         --------
         >>> user_id = '...'
 
         If you only have the screen name, you can get the user id as follows:
@@ -1540,18 +1528,18 @@
             'includePromotedContent': True,
             'withQuickPromoteEligibilityTweetFields': True,
             'withVoice': True,
             'withV2Timeline': True
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES),
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         endpoint = {
             'Tweets': Endpoint.USER_TWEETS,
             'Replies': Endpoint.USER_TWEETS_AND_REPLIES,
             'Media': Endpoint.USER_MEDIA,
             'Likes': Endpoint.USER_LIKES,
         }[tweet_type]
 
@@ -1607,29 +1595,21 @@
                 tweet_info = tweet_info['tweet']
             user_info = find_dict(tweet_info, 'result')[0]
             tweet = Tweet(self, tweet_info, User(self, user_info))
             tweet.replies = replies
 
             results.append(tweet)
 
-        async def _fetch_next_result():
-            return await self.get_user_tweets(
-                user_id, tweet_type, count, next_cursor
-            )
-
-        async def _fetch_previous_result():
-            return await self.get_user_tweets(
-                user_id, tweet_type, count, previous_cursor
-            )
-
         return Result(
             results,
-            _fetch_next_result,
+            partial(self.get_user_tweets,
+                    user_id, tweet_type, count, next_cursor),
             next_cursor,
-            _fetch_previous_result,
+            partial(self.get_user_tweets,
+                    user_id, tweet_type, count, previous_cursor),
             previous_cursor
         )
 
     async def get_timeline(
         self,
         count: int = 20,
         seen_tweet_ids: list[str] | None = None,
@@ -1637,24 +1617,24 @@
     ) -> Result[Tweet]:
         """
         Retrieves the timeline.
         Retrieves tweets from Home -> For You.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of tweets to retrieve.
-        seen_tweet_ids : list[str], default=None
+        seen_tweet_ids : list[:class:`str`], default=None
             A list of tweet IDs that have been seen.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A cursor for pagination.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing a list of Tweet objects.
 
         Example
         -------
         >>> tweets = await client.get_timeline()
         >>> for tweet in tweets:
         ...     print(tweet)
@@ -1684,15 +1664,15 @@
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.HOME_TIMELINE),
             'features': FEATURES,
         }
         response = (await self.http.post(
             Endpoint.HOME_TIMELINE,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )).json()
 
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
         results = []
 
@@ -1701,20 +1681,17 @@
                 continue
             tweet_info = find_dict(item, 'result')[0]
             if tweet_info['__typename'] == 'TweetWithVisibilityResults':
                 tweet_info = tweet_info['tweet']
             user_info = tweet_info['core']['user_results']['result']
             results.append(Tweet(self, tweet_info, user_info))
 
-        async def _fetch_next_result():
-            return await self.get_timeline(count, seen_tweet_ids, next_cursor)
-
         return Result(
             results,
-            _fetch_next_result,
+            partial(self.get_timeline, count, seen_tweet_ids, next_cursor),
             next_cursor
         )
 
     async def get_latest_timeline(
         self,
         count: int = 20,
         seen_tweet_ids: list[str] | None = None,
@@ -1722,24 +1699,24 @@
     ) -> Result[Tweet]:
         """
         Retrieves the timeline.
         Retrieves tweets from Home -> Following.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of tweets to retrieve.
-        seen_tweet_ids : list[str], default=None
+        seen_tweet_ids : list[:class:`str`], default=None
             A list of tweet IDs that have been seen.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A cursor for pagination.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing a list of Tweet objects.
 
         Example
         -------
         >>> tweets = await client.get_latest_timeline()
         >>> for tweet in tweets:
         ...     print(tweet)
@@ -1769,15 +1746,15 @@
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.HOME_LATEST_TIMELINE),
             'features': FEATURES,
         }
         response = (await self.http.post(
             Endpoint.HOME_LATEST_TIMELINE,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )).json()
 
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
         results = []
 
@@ -1786,37 +1763,33 @@
                 continue
             tweet_info = find_dict(item, 'result')[0]
             if tweet_info['__typename'] == 'TweetWithVisibilityResults':
                 tweet_info = tweet_info['tweet']
             user_info = tweet_info['core']['user_results']['result']
             results.append(Tweet(self, tweet_info, user_info))
 
-        async def _fetch_next_result():
-            return await self.get_latest_timeline(
-                count, seen_tweet_ids, next_cursor
-            )
-
         return Result(
             results,
-            _fetch_next_result,
+            partial(self.get_latest_timeline,
+                    count, seen_tweet_ids, next_cursor),
             next_cursor
         )
 
     async def favorite_tweet(self, tweet_id: str) -> Response:
         """
         Favorites a tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet to be liked.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> await client.favorite_tweet(tweet_id)
 
@@ -1826,31 +1799,31 @@
         """
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.FAVORITE_TWEET)
         }
         response = await self.http.post(
             Endpoint.FAVORITE_TWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def unfavorite_tweet(self, tweet_id: str) -> Response:
         """
         Unfavorites a tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet to be unliked.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> await client.unfavorite_tweet(tweet_id)
 
@@ -1860,31 +1833,31 @@
         """
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.UNFAVORITE_TWEET)
         }
         response = await self.http.post(
             Endpoint.UNFAVORITE_TWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def retweet(self, tweet_id: str) -> Response:
         """
         Retweets a tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet to be retweeted.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> await client.retweet(tweet_id)
 
@@ -1894,31 +1867,31 @@
         """
         data = {
             'variables': {'tweet_id': tweet_id, 'dark_request': False},
             'queryId': get_query_id(Endpoint.CREATE_RETWEET)
         }
         response = await self.http.post(
             Endpoint.CREATE_RETWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def delete_retweet(self, tweet_id: str) -> Response:
         """
         Deletes the retweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the retweeted tweet to be unretweeted.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> await client.delete_retweet(tweet_id)
 
@@ -1928,31 +1901,31 @@
         """
         data = {
             'variables': {'source_tweet_id': tweet_id,'dark_request': False},
             'queryId': get_query_id(Endpoint.DELETE_RETWEET)
         }
         response = await self.http.post(
             Endpoint.DELETE_RETWEET,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def bookmark_tweet(self, tweet_id: str) -> Response:
         """
         Adds the tweet to bookmarks.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet to be bookmarked.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> await client.bookmark_tweet(tweet_id)
 
@@ -1963,31 +1936,31 @@
 
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.CREATE_BOOKMARK)
         }
         response = await self.http.post(
             Endpoint.CREATE_BOOKMARK,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def delete_bookmark(self, tweet_id: str) -> Response:
         """
         Removes the tweet from bookmarks.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet to be removed from bookmarks.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> await client.delete_bookmark(tweet_id)
 
@@ -1997,35 +1970,35 @@
         """
         data = {
             'variables': {'tweet_id': tweet_id},
             'queryId': get_query_id(Endpoint.DELETE_BOOKMARK)
         }
         response = await self.http.post(
             Endpoint.DELETE_BOOKMARK,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def get_bookmarks(
         self, count: int = 20, cursor: str | None = None
     ) -> Result[Tweet]:
         """
         Retrieves bookmarks from the authenticated user's Twitter account.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of bookmarks to retrieve (default is 20).
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A cursor to paginate through the bookmarks (default is None).
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing a list of Tweet objects
             representing bookmarks.
 
         Example
         -------
         >>> bookmarks = await client.get_bookmarks()
         >>> for bookmark in bookmarks:
@@ -2045,18 +2018,18 @@
             'includePromotedContent': True
         }
         if cursor is not None:
             variables['cursor'] = cursor
         features = FEATURES | {
             'graphql_timeline_v2_bookmark_timeline': True
         }
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(features)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': features
+        })
         response = (await self.http.get(
             Endpoint.BOOKMARKS,
             params=params,
             headers=self._base_headers
         )).json()
 
         items_ = find_dict(response, 'entries')
@@ -2070,64 +2043,58 @@
         for item in items:
             if not item['entryId'].startswith('tweet'):
                 continue
             tweet_info = find_dict(item, 'tweet_results')[0]['result']
             user_info = tweet_info['core']['user_results']['result']
             results.append(Tweet(self, tweet_info, User(self, user_info)))
 
-        async def _fetch_next_result():
-            return await self.get_bookmarks(count, next_cursor)
-
-        async def _fetch_previous_result():
-            return await self.get_bookmarks(count, previous_cursor)
-
         return Result(
             results,
-            _fetch_next_result,
+            partial(self.get_bookmarks, count, next_cursor),
             next_cursor,
-            _fetch_previous_result,
+            partial(self.get_bookmarks, count, previous_cursor),
             previous_cursor
         )
 
     async def delete_all_bookmarks(self) -> Response:
         """
         Deleted all bookmarks.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> await client.delete_all_bookmarks()
         """
         data = {
             'variables': {},
             'queryId': get_query_id(Endpoint.BOOKMARKS_ALL_DELETE)
         }
         response = await self.http.post(
             Endpoint.BOOKMARKS_ALL_DELETE,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def follow_user(self, user_id: str) -> Response:
         """
         Follows a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to follow.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> user_id = '...'
         >>> await client.follow_user(user_id)
 
@@ -2162,20 +2129,20 @@
 
     async def unfollow_user(self, user_id: str) -> Response:
         """
         Unfollows a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to unfollow.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> user_id = '...'
         >>> await client.unfollow_user(user_id)
 
@@ -2210,20 +2177,20 @@
 
     async def block_user(self, user_id: str) -> Response:
         """
         Blocks a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to block.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .unblock_user
         """
         data = urlencode({'user_id': user_id})
@@ -2238,20 +2205,20 @@
 
     async def unblock_user(self, user_id: str) -> Response:
         """
         Unblocks a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to unblock.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .block_user
         """
         data = urlencode({'user_id': user_id})
@@ -2266,20 +2233,20 @@
 
     async def mute_user(self, user_id: str) -> Response:
         """
         Mutes a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to mute.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .unmute_user
         """
         data = urlencode({'user_id': user_id})
@@ -2294,20 +2261,20 @@
 
     async def unmute_user(self, user_id: str) -> Response:
         """
         Unmutes a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to unmute.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .mute_user
         """
         data = urlencode({'user_id': user_id})
@@ -2335,20 +2302,20 @@
         category : {'trending', 'for-you', 'news', 'sports', 'entertainment'}
             The category of trends to retrieve. Valid options include:
             - 'trending': General trending topics.
             - 'for-you': Trends personalized for the user.
             - 'news': News-related trends.
             - 'sports': Sports-related trends.
             - 'entertainment': Entertainment-related trends.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of trends to retrieve.
 
         Returns
         -------
-        list[Trend]
+        list[:class:`Trend`]
             A list of Trend objects representing the retrieved trends.
 
         Examples
         --------
         >>> trends = await client.get_trends('trending')
         >>> for trend in trends:
         ...     print(trend)
@@ -2403,18 +2370,18 @@
         variables = {
             'userId': user_id,
             'count': count,
             'includePromotedContent': False
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         response = (await self.http.get(
             endpoint,
             params=params,
             headers=self._base_headers
         )).json()
 
         items = find_dict(response, 'entries')[0]
@@ -2423,41 +2390,37 @@
             entry_id = item['entryId']
             if entry_id.startswith('user'):
                 user_info = find_dict(item, 'result')[0]
                 results.append(User(self, user_info))
             elif entry_id.startswith('cursor-bottom'):
                 next_cursor = item['content']['value']
 
-        async def _fetch_next_result():
-            return self._get_user_friendship(
-                user_id, count, endpoint, next_cursor
-            )
-
         return Result(
             results,
-            _fetch_next_result,
+            partial(self._get_user_friendship,
+                    user_id, count, endpoint, next_cursor),
             next_cursor
         )
 
     def get_user_followers(
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of followers for a given user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user for whom to retrieve followers.
         count : int, default=20
             The number of followers to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the followers.
         """
         return self._get_user_friendship(
             user_id,
             count,
             Endpoint.FOLLOWERS,
             cursor
@@ -2467,22 +2430,22 @@
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of verified followers for a given user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user for whom to retrieve verified followers.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of verified followers to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the verified followers.
         """
         return self._get_user_friendship(
             user_id,
             count,
             Endpoint.BLUE_VERIFIED_FOLLOWERS,
             cursor
@@ -2492,22 +2455,22 @@
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of common followers.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user for whom to retrieve followers you might know.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of followers you might know to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the followers you might know.
         """
         return self._get_user_friendship(
             user_id,
             count,
             Endpoint.FOLLOWERS_YOU_KNOW,
             cursor
@@ -2517,22 +2480,22 @@
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of users whom the given user is following.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user for whom to retrieve the following users.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of following users to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the users being followed.
         """
         return self._get_user_friendship(
             user_id,
             count,
             Endpoint.FOLLOWING,
             cursor
@@ -2542,22 +2505,22 @@
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of users to which the specified user is subscribed.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user for whom to retrieve subscriptions.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of subscriptions to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the subscribed users.
         """
         return self._get_user_friendship(
             user_id,
             count,
             Endpoint.SUBSCRIPTIONS,
             cursor
@@ -2585,15 +2548,15 @@
         if media_id is not None:
             data['media_id'] = media_id
         if reply_to is not None:
             data['reply_to_dm_id'] = reply_to
 
         return (await self.http.post(
             Endpoint.SEND_DM,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )).json()
 
     async def _get_dm_history(
         self,
         conversation_id: str,
         max_id: str | None = None
@@ -2621,28 +2584,28 @@
         reply_to: str | None = None
     ) -> Message:
         """
         Send a direct message to a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to whom the direct message will be sent.
-        text : str
+        text : :class:`str`
             The text content of the direct message.
-        media_id : str, default=None
+        media_id : :class:`str`, default=None
             The media ID associated with any media content
             to be included in the message.
             Media ID can be received by using the :func:`.upload_media` method.
-        reply_to : str, default=None
+        reply_to : :class:`str`, default=None
             Message ID to reply to.
 
         Returns
         -------
-        Message
+        :class:`Message`
             `Message` object containing information about the message sent.
 
         Examples
         --------
         >>> # send DM with media
         >>> user_id = '000000000'
         >>> media_id = await client.upload_media('image.png')
@@ -2661,36 +2624,36 @@
 
         message_data = find_dict(response, 'message_data')[0]
         users = list(response['users'].values())
         return Message(
             self,
             message_data,
             users[0]['id_str'],
-            users[1]['id_str']
+            users[1]['id_str'] if len(users) == 2 else users[0]['id_str']
         )
 
     async def add_reaction_to_message(
         self, message_id: str, conversation_id: str, emoji: str
     ) -> Response:
         """
         Adds a reaction emoji to a specific message in a conversation.
 
         Parameters
         ----------
-        message_id : str
+        message_id : :class:`str`
             The ID of the message to which the reaction emoji will be added.
             Group ID ('00000000') or partner_ID-your_ID ('00000000-00000001')
-        conversation_id : str
+        conversation_id : :class:`str`
             The ID of the conversation containing the message.
-        emoji : str
+        emoji : :class:`str`
             The emoji to be added as a reaction.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> message_id = '00000000'
         >>> conversation_id = f'00000001-{await client.user_id()}'
         >>> await client.add_reaction_to_message(
@@ -2705,38 +2668,38 @@
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.MESSAGE_ADD_REACTION)
         }
         response = await self.http.post(
             Endpoint.MESSAGE_ADD_REACTION,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def remove_reaction_from_message(
         self, message_id: str, conversation_id: str, emoji: str
     ) -> Response:
         """
         Remove a reaction from a message.
 
         Parameters
         ----------
-        message_id : str
+        message_id : :class:`str`
             The ID of the message from which to remove the reaction.
-        conversation_id : str
+        conversation_id : :class:`str`
             The ID of the conversation where the message is located.
             Group ID ('00000000') or partner_ID-your_ID ('00000000-00000001')
-        emoji : str
+        emoji : :class:`str`
             The emoji to remove as a reaction.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> message_id = '00000000'
         >>> conversation_id = f'00000001-{await client.user_id()}'
         >>> await client.remove_reaction_from_message(
@@ -2751,31 +2714,31 @@
         }
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.MESSAGE_REMOVE_REACTION)
         }
         response = await self.http.post(
             Endpoint.MESSAGE_REMOVE_REACTION,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def delete_dm(self, message_id: str) -> Response:
         """
         Deletes a direct message with the specified message ID.
 
         Parameters
         ----------
-        message_id : str
+        message_id : :class:`str`
             The ID of the direct message to be deleted.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> await client.delete_dm('0000000000')
         """
 
@@ -2783,38 +2746,38 @@
             'variables': {
                 'messageId': message_id
             },
             'queryId': get_query_id(Endpoint.DELETE_DM)
         }
         response = await self.http.post(
             Endpoint.DELETE_DM,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def get_dm_history(
         self,
         user_id: str,
         max_id: str | None = None
     ) -> Result[Message]:
         """
         Retrieves the DM conversation history with a specific user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user with whom the DM conversation
             history will be retrieved.
-        max_id : str, default=None
+        max_id : :class:`str`, default=None
             If specified, retrieves messages older than the specified max_id.
 
         Returns
         -------
-        Result[Message]
+        Result[:class:`Message`]
             A Result object containing a list of Message objects representing
             the DM conversation history.
 
         Examples
         --------
         >>> messages = await client.get_dm_history('0000000000')
         >>> for message in messages:
@@ -2843,20 +2806,17 @@
             messages.append(Message(
                 self,
                 message_info,
                 message_info['sender_id'],
                 message_info['recipient_id']
             ))
 
-        async def _fetch_next_result():
-            return await self.get_dm_history(user_id, messages[-1].id)
-
         return Result(
             messages,
-            _fetch_next_result,
+            partial(self.get_dm_history, user_id, messages[-1].id),
             messages[-1].id
         )
 
     async def send_dm_to_group(
         self,
         group_id: str,
         text: str,
@@ -2864,28 +2824,28 @@
         reply_to: str | None = None
     ) -> GroupMessage:
         """
         Sends a message to a group.
 
         Parameters
         ----------
-        group_id : str
+        group_id : :class:`str`
             The ID of the group in which the direct message will be sent.
-        text : str
+        text : :class:`str`
             The text content of the direct message.
-        media_id : str, default=None
+        media_id : :class:`str`, default=None
             The media ID associated with any media content
             to be included in the message.
             Media ID can be received by using the :func:`.upload_media` method.
-        reply_to : str, default=None
+        reply_to : :class:`str`, default=None
             Message ID to reply to.
 
         Returns
         -------
-        GroupMessage
+        :class:`GroupMessage`
             `GroupMessage` object containing information about
             the message sent.
 
         Examples
         --------
         >>> # send DM with media
         >>> group_id = '000000000'
@@ -2918,23 +2878,23 @@
         max_id: str | None = None
     ) -> Result[GroupMessage]:
         """
         Retrieves the DM conversation history in a group.
 
         Parameters
         ----------
-        group_id : str
+        group_id : :class:`str`
             The ID of the group in which the DM conversation
             history will be retrieved.
-        max_id : str, default=None
+        max_id : :class:`str`, default=None
             If specified, retrieves messages older than the specified max_id.
 
         Returns
         -------
-        Result[GroupMessage]
+        Result[:class:`GroupMessage`]
             A Result object containing a list of GroupMessage objects
             representing the DM conversation history.
 
         Examples
         --------
         >>> messages = await client.get_group_dm_history('0000000000')
         >>> for message in messages:
@@ -2963,35 +2923,32 @@
             messages.append(GroupMessage(
                 self,
                 message_info,
                 message_info['sender_id'],
                 group_id
             ))
 
-        async def _fetch_next_result():
-            return await self.get_group_dm_history(group_id, messages[-1].id)
-
         return Result(
             messages,
-            _fetch_next_result,
+            partial(self.get_group_dm_history, group_id, messages[-1].id),
             messages[-1].id
         )
 
     async def get_group(self, group_id: str) -> Group:
         """
         Fetches a guild by ID.
 
         Parameters
         ----------
-        group_id : str
+        group_id : :class:`str`
             The ID of the group to retrieve information for.
 
         Returns
         -------
-        Group
+        :class:`Group`
             An object representing the retrieved group.
         """
         params = {
             'context': 'FETCH_DM_CONVERSATION_HISTORY',
             'include_conversation_info': True,
         }
         response = (await self.http.get(
@@ -3004,22 +2961,22 @@
     async def add_members_to_group(
         self, group_id: str, user_ids: list[str]
     ) -> Response:
         """Adds members to a group.
 
         Parameters
         ----------
-        group_id : str
+        group_id : :class:`str`
             ID of the group to which the member is to be added.
-        user_ids : list[str]
+        user_ids : list[:class:`str`]
             List of IDs of users to be added.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> group_id = '...'
         >>> members = ['...']
         >>> await client.add_members_to_group(group_id, members)
@@ -3029,32 +2986,32 @@
                 'addedParticipants': user_ids,
                 'conversationId': group_id
             },
             'queryId': get_query_id(Endpoint.ADD_MEMBER_TO_GROUP)
         }
         response = await self.http.post(
             Endpoint.ADD_MEMBER_TO_GROUP,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def change_group_name(self, group_id: str, name: str) -> Response:
         """Changes group name
 
         Parameters
         ----------
-        group_id : str
+        group_id : :class:`str`
             ID of the group to be renamed.
-        name : str
+        name : :class:`str`
             New name.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
         data = urlencode({
             'name': name
         })
         headers = self._base_headers
         headers['content-type'] = 'application/x-www-form-urlencoded'
@@ -3069,24 +3026,24 @@
         self, name: str, description: str = '', is_private: bool = False
     ) -> List:
         """
         Creates a list.
 
         Parameters
         ----------
-        name : str
+        name : :class:`str`
             The name of the list.
-        description : str, default=''
+        description : :class:`str`, default=''
             The description of the list.
-        is_private : bool, default=False
+        is_private : :class:`bool`, default=False
             Indicates whether the list is private (True) or public (False).
 
         Returns
         -------
-        List
+        :class:`List`
             The created list.
 
         Examples
         --------
         >>> list = await client.create_list(
         ...     'list name',
         ...     'list description',
@@ -3103,34 +3060,34 @@
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.CREATE_LIST)
         }
         response = (await self.http.post(
             Endpoint.CREATE_LIST,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )).json()
         list_info = find_dict(response, 'list')[0]
         return List(self, list_info)
 
     async def edit_list_banner(self, list_id: str, media_id: str) -> Response:
         """
         Edit the banner image of a list.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             The ID of the list.
-        media_id : str
+        media_id : :class:`str`
             The ID of the media to use as the new banner image.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> list_id = '...'
         >>> media_id = await client.upload_media('image.png')
         >>> await client.edit_list_banner(list_id, media_id)
@@ -3142,42 +3099,42 @@
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.EDIT_LIST_BANNER)
         }
         response = await self.http.post(
             Endpoint.EDIT_LIST_BANNER,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def delete_list_banner(self, list_id: str) -> Response:
         """Deletes list banner.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             ID of the list from which the banner is to be removed.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
         data = {
             'variables': {
                 'listId': list_id
             },
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.DELETE_LIST_BANNER)
         }
         response = await self.http.post(
             Endpoint.DELETE_LIST_BANNER,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def edit_list(
         self,
         list_id: str,
@@ -3186,27 +3143,27 @@
         is_private: bool | None = None
     ) -> List:
         """
         Edits list information.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             The ID of the list to edit.
-        name : str, default=None
+        name : :class:`str`, default=None
             The new name for the list.
-        description : str, default=None
+        description : :class:`str`, default=None
             The new description for the list.
-        is_private : bool, default=None
+        is_private : :class:`bool`, default=None
             Indicates whether the list should be private
             (True) or public (False).
 
         Returns
         -------
-        List
+        :class:`List`
             The updated Twitter list.
 
         Examples
         --------
         >>> await client.edit_list(
         ...     'new name', 'new description', True
         ... )
@@ -3223,34 +3180,34 @@
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.UPDATE_LIST)
         }
         response = (await self.http.post(
             Endpoint.UPDATE_LIST,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )).json()
         list_info = find_dict(response, 'list')[0]
         return List(self, list_info)
 
     async def add_list_member(self, list_id: str, user_id: str) -> Response:
         """
         Adds a user to a list.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             The ID of the list.
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to add to the list.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> await client.add_list_member('list id', 'user id')
         """
         variables = {
@@ -3260,33 +3217,33 @@
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.LIST_ADD_MEMBER)
         }
         response = await self.http.post(
             Endpoint.LIST_ADD_MEMBER,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def remove_list_member(self, list_id: str, user_id: str) -> Response:
         """
         Removes a user from a list.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             The ID of the list.
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to remove from the list.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> await client.remove_list_member('list id', 'user id')
         """
         variables = {
@@ -3296,33 +3253,33 @@
         data = {
             'variables': variables,
             'features': LIST_FEATURES,
             'queryId': get_query_id(Endpoint.LIST_REMOVE_MEMBER)
         }
         response = await self.http.post(
             Endpoint.LIST_REMOVE_MEMBER,
-            data=json.dumps(data),
+            json=data,
             headers=self._base_headers
         )
         return response
 
     async def get_lists(
         self, count: int = 100, cursor: str = None
     ) -> Result[List]:
         """
         Retrieves a list of user lists.
 
         Parameters
         ----------
-        count : int
+        count : :class:`int`
             The number of lists to retrieve.
 
         Returns
         -------
-        Result[List]
+        Result[:class:`List`]
             Retrieved lists.
 
         Examples
         --------
         >>> lists = client.get_lists()
         >>> for list_ in lists:
         ...     print(list_)
@@ -3333,18 +3290,18 @@
         >>> more_lists = lists.next()  # Retrieve more lists
         """
         variables = {
             'count': count
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         response = (await self.http.get(
             Endpoint.LIST_MANAGEMENT,
             params=params,
             headers=self._base_headers
         )).json()
 
         entries = find_dict(response, 'entries')[0]
@@ -3357,41 +3314,38 @@
         for list in items[1]:
             lists.append(
                 List(self, list['item']['itemContent']['list'])
             )
 
         next_cursor = entries[-1]['content']['value']
 
-        async def _fetch_next_result():
-            return await self.get_lists(count, next_cursor)
-
         return Result(
             lists,
-            _fetch_next_result,
+            partial(self.get_lists, count, next_cursor),
             next_cursor
         )
 
     async def get_list(self, list_id: str) -> List:
         """
         Retrieve list by ID.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             The ID of the list to retrieve.
 
         Returns
         -------
-        List
+        :class:`List`
             List object.
         """
-        params = {
-            'variables': json.dumps({'listId': list_id}),
-            'features': json.dumps(LIST_FEATURES)
-        }
+        params = flatten_params({
+            'variables': {'listId': list_id},
+            'features': LIST_FEATURES
+        })
         response = (await self.http.get(
             Endpoint.LIST_BY_REST_ID,
             params=params,
             headers=self._base_headers
         )).json()
         list_info = find_dict(response, 'list')[0]
         return List(self, list_info)
@@ -3400,24 +3354,24 @@
         self, list_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[Tweet]:
         """
         Retrieves tweets from a list.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             The ID of the list to retrieve tweets from.
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of tweets to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             The cursor for pagination.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing the retrieved tweets.
 
         Examples
         --------
         >>> tweets = await client.get_list_tweets('list id')
         >>> for tweet in tweets:
         ...    print(tweet)
@@ -3436,18 +3390,18 @@
         """
         variables = {
             'listId': list_id,
             'count': count
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         response = (await self.http.get(
             Endpoint.LIST_LATEST_TWEETS,
             params=params,
             headers=self._base_headers
         )).json()
 
         items = find_dict(response, 'entries')[0]
@@ -3459,20 +3413,17 @@
                 continue
             tweet_info = find_dict(item, 'result')[0]
             if tweet_info['__typename'] == 'TweetWithVisibilityResults':
                 tweet_info = tweet_info['tweet']
             user_info = find_dict(tweet_info, 'result')[0]
             results.append(Tweet(self, tweet_info, User(self, user_info)))
 
-        async def _fetch_next_result():
-            return await self.get_list_tweets(list_id, count, next_cursor)
-
         return Result(
             results,
-            _fetch_next_result,
+            partial(self.get_list_tweets, list_id, count, next_cursor),
             next_cursor
         )
 
     async def _get_list_users(
         self, endpoint: str, list_id: str, count: int, cursor: str
     ) -> Result[User]:
         """
@@ -3480,18 +3431,18 @@
         """
         variables = {
             'listId': list_id,
             'count': count,
         }
         if cursor is not None:
             variables['cursor'] = cursor
-        params = {
-            'variables': json.dumps(variables),
-            'features': json.dumps(FEATURES)
-        }
+        params = flatten_params({
+            'variables': variables,
+            'features': FEATURES
+        })
         response = (await self.http.get(
             endpoint,
             params=params,
             headers=self._base_headers
         )).json()
 
         items = find_dict(response, 'entries')[0]
@@ -3519,22 +3470,22 @@
     async def get_list_members(
         self, list_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """Retrieves members of a list.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             List ID.
         count : int, default=20
             Number of members to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             Members of a list
 
         Examples
         --------
         >>> members = client.get_list_members(123456789)
         >>> for member in members:
         ...     print(member)
@@ -3554,22 +3505,22 @@
     async def get_list_subscribers(
         self, list_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """Retrieves subscribers of a list.
 
         Parameters
         ----------
-        list_id : str
+        list_id : :class:`str`
             List ID.
-        count : int, default=20
+        count : :class:`int`, default=20
             Number of subscribers to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             Subscribers of a list
 
         Examples
         --------
         >>> members = client.get_list_subscribers(123456789)
         >>> for subscriber in subscribers:
         ...     print(subscriber)
@@ -3595,24 +3546,23 @@
         """
         Retrieve notifications based on the provided type.
 
         Parameters
         ----------
         type : {'All', 'Verified', 'Mentions'}
             Type of notifications to retrieve.
-
             All: All notifications
             Verified: Notifications relating to authenticated users
             Mentions: Notifications with mentions
-        count : int, default=40
+        count : :class:`int`, default=40
             Number of notifications to retrieve.
 
         Returns
         -------
-        Result[Notification]
+        Result[:class:`Notification`]
             List of retrieved notifications.
 
         Examples
         --------
         >>> notifications = await client.get_notifications('All')
         >>> for notification in notifications:
         ...     print(notification)
@@ -3683,15 +3633,12 @@
             if i['entryId'].startswith('cursor-bottom')
         ]
         if cursor_bottom_entry:
             next_cursor = find_dict(cursor_bottom_entry[0], 'value')[0]
         else:
             next_cursor = None
 
-        async def _fetch_next_result():
-            return await self.get_notifications(type, count, next_cursor)
-
         return Result(
             notifications,
-            _fetch_next_result,
+            partial(self.get_notifications, type, count, next_cursor),
             next_cursor
         )
```

### Comparing `twikit-1.4.4/twikit/twikit_async/errors.py` & `twikit-1.4.5/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.4/twikit/twikit_async/group.py` & `twikit-1.4.5/twikit/group.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
 class Group:
     """
     Represents a group.
 
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The ID of the group.
-    name : str | None
+    name : :class:`str` | None
         The name of the group.
-    members : list[str]
+    members : list[:class:`str`]
         Member IDs
     """
     def __init__(self, client: Client, group_id: str, data: dict) -> None:
         self._client = client
         self.id = group_id
 
         entries = data['conversation_timeline']['entries']
@@ -37,224 +37,218 @@
             name_update_log['conversation_name_update']['conversation_name']
             if name_update_log else None
         )
 
         members = data['conversation_timeline']['users'].values()
         self.members: list[str] = [i['id_str'] for i in members]
 
-    async def get_history(
-        self, max_id: str | None = None
-    ) -> Result[GroupMessage]:
+    def get_history(self, max_id: str | None = None) -> Result[GroupMessage]:
         """
         Retrieves the DM conversation history in the group.
 
         Parameters
         ----------
-        max_id : str, default=None
+        max_id : :class:`str`, default=None
             If specified, retrieves messages older than the specified max_id.
 
         Returns
         -------
-        Result[GroupMessage]
+        Result[:class:`GroupMessage`]
             A Result object containing a list of GroupMessage objects
             representing the DM conversation history.
 
         Examples
         --------
-        >>> messages = await group.get_history()
+        >>> messages = group.get_history()
         >>> for message in messages:
         >>>     print(message)
         <GroupMessage id="...">
         <GroupMessage id="...">
         ...
         ...
 
-        >>> more_messages = await messages.next()  # Retrieve more messages
+        >>> more_messages = messages.next()  # Retrieve more messages
         >>> for message in more_messages:
         >>>     print(message)
         <GroupMessage id="...">
         <GroupMessage id="...">
         ...
         ...
         """
-        return await self._client.get_group_dm_history(self.id, max_id)
+        return self._client.get_group_dm_history(self.id, max_id)
 
-    async def add_members(self, user_ids: list[str]) -> Response:
+    def add_members(self, user_ids: list[str]) -> Response:
         """Adds members to the group.
 
         Parameters
         ----------
-        user_ids : list[str]
+        user_ids : list[:class:`str`]
             List of IDs of users to be added.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
         >>> members = ['...']
-        >>> await group.add_members(members)
+        >>> group.add_members(members)
         """
-        return await self._client.add_members_to_group(self.id, user_ids)
+        return self._client.add_members_to_group(self.id, user_ids)
 
-    async def change_name(self, name: str) -> Response:
+    def change_name(self, name: str) -> Response:
         """Changes group name
 
         Parameters
         ----------
-        name : str
+        name : :class:`str`
             New name.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
-        return await self._client.change_group_name(self.id, name)
+        return self._client.change_group_name(self.id, name)
 
-    async def send_message(
+    def send_message(
         self,
         text: str,
         media_id: str | None = None,
         reply_to: str | None = None
     ) -> GroupMessage:
         """
         Sends a message to the group.
 
         Parameters
         ----------
-        text : str
+        text : :class:`str`
             The text content of the direct message.
-        media_id : str, default=None
+        media_id : :class:`str`, default=None
             The media ID associated with any media content
             to be included in the message.
             Media ID can be received by using the :func:`.upload_media` method.
-        reply_to : str, default=None
+        reply_to : :class:`str`, default=None
             Message ID to reply to.
 
         Returns
         -------
-        GroupMessage
+        :class:`GroupMessage`
             `Message` object containing information about the message sent.
 
         Examples
         --------
         >>> # send DM with media
         >>> group_id = '000000000'
-        >>> media_id = await client.upload_media('image.png')
-        >>> message = await group.send_message('text', media_id)
+        >>> media_id = client.upload_media('image.png')
+        >>> message = group.send_message('text', media_id)
         >>> print(message)
         <GroupMessage id='...'>
         """
-        return await self._client.send_dm_to_group(
-            self.id, text, media_id, reply_to
-        )
+        return self._client.send_dm_to_group(self.id, text, media_id, reply_to)
 
-    async def update(self) -> None:
-        new = await self._client.get_group(self.id)
+    def update(self) -> None:
+        new = self._client.get_group(self.id)
         self.__dict__.update(new.__dict__)
 
     def __repr__(self) -> str:
         return f'<Group id="{self.id}">'
 
 
 class GroupMessage(Message):
     """
     Represents a direct message.
 
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The ID of the message.
-    time : str
+    time : :class:`str`
         The timestamp of the message.
-    text : str
+    text : :class:`str`
         The text content of the message.
-    attachment : str
+    attachment : :class:`str`
         The media URL associated with any attachment in the message.
-    group_id : str
+    group_id : :class:`str`
         The ID of the group.
     """
     def __init__(
         self,
         client: Client,
         data: dict,
         sender_id: str,
         group_id: str
     ) -> None:
         super().__init__(client, data, sender_id, None)
         self.group_id = group_id
 
-    async def group(self) -> Group:
+    def group(self) -> Group:
         """
         Gets the group to which the message was sent.
         """
-        return await self._client.get_group(self.group_id)
+        return self._client.get_group(self.group_id)
 
-    async def reply(
-        self, text: str, media_id: str | None = None
-    ) -> GroupMessage:
+    def reply(self, text: str, media_id: str | None = None) -> GroupMessage:
         """Replies to the message.
 
         Parameters
         ----------
-        text : str
+        text : :class:`str`
             The text content of the direct message.
-        media_id : str, default=None
+        media_id : :class:`str`, default=None
             The media ID associated with any media content
             to be included in the message.
             Media ID can be received by using the :func:`.upload_media` method.
 
         Returns
         -------
-        Message
+        :class:`Message`
             `GroupMessage` object containing information about
             the message sent.
 
         See Also
         --------
         Client.send_dm_to_group
         """
-        return await self._client.send_dm_to_group(
+        return self._client.send_dm_to_group(
             self.group_id, text, media_id, self.id
         )
 
-    async def add_reaction(self, emoji: str) -> Response:
+    def add_reaction(self, emoji: str) -> Response:
         """
         Adds a reaction to the message.
 
         Parameters
         ----------
-        emoji : str
+        emoji : :class:`str`
             The emoji to be added as a reaction.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
-        return await self._client.add_reaction_to_message(
+        return self._client.add_reaction_to_message(
             self.id, self.group_id, emoji
         )
 
-    async def remove_reaction(self, emoji: str) -> Response:
+    def remove_reaction(self, emoji: str) -> Response:
         """
         Removes a reaction from the message.
 
         Parameters
         ----------
-        emoji : str
+        emoji : :class:`str`
             The emoji to be removed.
 
         Returns
         -------
         httpx.Response
             Response returned from twitter api.
         """
-        return await self._client.remove_reaction_from_message(
+        return self._client.remove_reaction_from_message(
             self.id, self.group_id, emoji
         )
 
     def __repr__(self) -> str:
         return f'<GroupMessage id="{self.id}">'
```

### Comparing `twikit-1.4.4/twikit/twikit_async/http.py` & `twikit-1.4.5/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.4/twikit/twikit_async/list.py` & `twikit-1.4.5/twikit/list.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import TYPE_CHECKING, Literal
 
-from ..utils import timestamp_to_datetime
+from .utils import timestamp_to_datetime
 
 if TYPE_CHECKING:
     from httpx import Response
 
     from .client import Client
     from .tweet import Tweet
     from .user import User
@@ -16,40 +16,40 @@
 
 class List:
     """
     Class representing a Twitter List.
 
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The unique identifier of the List.
-    created_at : int
+    created_at : :class:`int`
         The timestamp when the List was created.
-    default_banner : dict
+    default_banner : :class:`dict`
         Information about the default banner of the List.
-    banner : dict
+    banner : :class:`dict`
         Information about the banner of the List. If custom banner is not set,
         it defaults to the default banner.
-    description : str
+    description : :class:`str`
         The description of the List.
-    following : bool
+    following : :class:`bool`
         Indicates if the authenticated user is following the List.
-    is_member : bool
+    is_member : :class:`bool`
         Indicates if the authenticated user is a member of the List.
-    member_count : int
+    member_count : :class:`int`
         The number of members in the List.
-    mode : Literal['Private', 'Public']
+    mode : {'Private', 'Public'}
         The mode of the List, either 'Private' or 'Public'.
-    muting : bool
+    muting : :class:`bool`
         Indicates if the authenticated user is muting the List.
-    name : str
+    name : :class:`str`
         The name of the List.
-    pinning : bool
+    pinning : :class:`bool`
         Indicates if the List is pinned.
-    subscriber_count : int
+    subscriber_count : :class:`int`
         The number of subscribers to the List.
     """
     def __init__(self, client: Client, data: dict) -> None:
         self._client = client
 
         self.id: str = data['id_str']
         self.created_at: int = data['created_at']
@@ -70,183 +70,181 @@
         self.pinning: bool = data['pinning']
         self.subscriber_count: int = data['subscriber_count']
 
     @property
     def created_at_datetime(self) -> datetime:
         return timestamp_to_datetime(self.created_at)
 
-    async def edit_banner(self, media_id: str) -> Response:
+    def edit_banner(self, media_id: str) -> Response:
         """
         Edit the banner image of the list.
 
         Parameters
         ----------
-        media_id : str
+        media_id : :class:`str`
             The ID of the media to use as the new banner image.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
-        >>> media_id = await client.upload_media('image.png')
-        >>> await media.edit_banner(media_id)
+        >>> media_id = client.upload_media('image.png')
+        >>> media.edit_banner(media_id)
         """
-        return await self._client.edit_list_banner(self.id, media_id)
+        return self._client.edit_list_banner(self.id, media_id)
 
-    async def delete_banner(self) -> Response:
+    def delete_banner(self) -> Response:
         """
         Deletes the list banner.
         """
-        return await self._client.delete_list_banner(self.id)
+        return self._client.delete_list_banner(self.id)
 
-    async def edit(
+    def edit(
         self,
         name: str | None = None,
         description: str | None = None,
         is_private: bool | None = None
     ) -> List:
         """
         Edits list information.
 
         Parameters
         ----------
-        name : str, default=None
+        name : :class:`str`, default=None
             The new name for the list.
-        description : str, default=None
+        description : :class:`str`, default=None
             The new description for the list.
-        is_private : bool, default=None
+        is_private : :class:`bool`, default=None
             Indicates whether the list should be private
             (True) or public (False).
 
         Returns
         -------
-        List
+        :class:`List`
             The updated Twitter list.
 
         Examples
         --------
-        >>> await list.edit(
+        >>> list.edit(
         ...     'new name', 'new description', True
         ... )
         """
-        return await self._client.edit_list(
-            self.id, name, description, is_private
-        )
+        return self._client.edit_list(self.id, name, description, is_private)
 
-    async def add_member(self, user_id: str) -> Response:
+    def add_member(self, user_id: str) -> Response:
         """
         Adds a member to the list.
         """
-        return await self._client.add_list_member(self.id, user_id)
+        return self._client.add_list_member(self.id, user_id)
 
-    async def remove_member(self, user_id: str) -> Response:
+    def remove_member(self, user_id: str) -> Response:
         """
         Removes a member from the list.
         """
-        return await self._client.remove_list_member(self.id, user_id)
+        return self._client.remove_list_member(self.id, user_id)
 
-    async def get_tweets(
+    def get_tweets(
         self, count: int = 20, cursor: str | None = None
     ) -> Result[Tweet]:
         """
         Retrieves tweets from the list.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of tweets to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             The cursor for pagination.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing the retrieved tweets.
 
         Examples
         --------
-        >>> tweets = await list.get_tweets()
+        >>> tweets = list.get_tweets()
         >>> for tweet in tweets:
         ...    print(tweet)
         <Tweet id="...">
         <Tweet id="...">
         ...
         ...
 
-        >>> more_tweets = await tweets.next()  # Retrieve more tweets
+        >>> more_tweets = tweets.next()  # Retrieve more tweets
         >>> for tweet in more_tweets:
         ...     print(tweet)
         <Tweet id="...">
         <Tweet id="...">
         ...
         ...
         """
-        return await self._client.get_list_tweets(self.id, count, cursor)
+        return self._client.get_list_tweets(self.id, count, cursor)
 
-    async def get_members(
+    def get_members(
         self, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """Retrieves members of the list.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             Number of members to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             Members of the list
 
         Examples
         --------
         >>> members = list_.get_members()
         >>> for member in members:
         ...     print(member)
         <User id="...">
         <User id="...">
         ...
         ...
         >>> more_members = members.next()  # Retrieve more members
         """
-        return await self._client.get_list_members(self.id, count, cursor)
+        return self._client.get_list_members(self.id, count, cursor)
 
-    async def get_subscribers(
+    def get_subscribers(
         self, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """Retrieves subscribers of the list.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             Number of subscribers to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             Subscribers of the list
 
         Examples
         --------
         >>> subscribers = list_.get_subscribers()
         >>> for subscriber in subscribers:
         ...     print(subscriber)
         <User id="...">
         <User id="...">
         ...
         ...
         >>> more_subscribers = subscribers.next()  # Retrieve more subscribers
         """
-        return await self._client.get_list_subscribers(self.id, count, cursor)
+        return self._client.get_list_subscribers(self.id, count, cursor)
 
-    async def update(self) -> None:
-        new = await self._client.get_list(self.id)
+    def update(self) -> None:
+        new = self._client.get_list(self.id)
         self.__dict__.update(new.__dict__)
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, List) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
         return not self == __value
```

### Comparing `twikit-1.4.4/twikit/twikit_async/notification.py` & `twikit-1.4.5/twikit/twikit_async/notification.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,25 @@
     from .user import User
 
 
 class Notification:
     """
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The unique identifier of the notification.
-    timestamp_ms : int
+    timestamp_ms : :class:`int`
         The timestamp of the notification in milliseconds.
-    icon : dict
+    icon : :class:`dict`
         Dictionary containing icon data for the notification.
-    message : str
+    message : :class:`str`
         The message text of the notification.
-    tweet : Tweet
+    tweet : :class:`Tweet`
         The tweet associated with the notification.
-    from_user : User
+    from_user : :class:`User`
         The user who triggered the notification.
     """
     def __init__(
         self, client: Client, data: dict, tweet: Tweet, from_user: User
     ) -> None:
         self._client = client
         self.tweet = tweet
```

### Comparing `twikit-1.4.4/twikit/twikit_async/trend.py` & `twikit-1.4.5/twikit/twikit_async/trend.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     from .client import Client
 
 
 class Trend:
     """
     Attributes
     ----------
-    name : str
+    name : :class:`str`
         The name of the trending topic.
-    tweets_count : int
+    tweets_count : :class:`int`
         The count of tweets associated with the trend.
-    domain_context : str
+    domain_context : :class:`str`
         The context or domain associated with the trend.
-    grouped_trends : list[str]
+    grouped_trends : :class:`list`[:class:`str`]
         A list of trend names grouped under the main trend.
     """
 
     def __init__(self, client: Client, data: dict) -> None:
         self._client = client
 
         metadata: dict = data['trendMetadata']
```

### Comparing `twikit-1.4.4/twikit/twikit_async/tweet.py` & `twikit-1.4.5/twikit/tweet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,85 @@
 from __future__ import annotations
 
 import re
 from datetime import datetime
 from typing import TYPE_CHECKING
 
-from ..utils import find_dict, timestamp_to_datetime
 from .user import User
+from .utils import find_dict, timestamp_to_datetime
 
 if TYPE_CHECKING:
     from httpx import Response
 
     from .client import Client
     from .utils import Result
 
 
 class Tweet:
     """
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The unique identifier of the tweet.
-    created_at : str
+    created_at : :class:`str`
         The date and time when the tweet was created.
-    created_at_datetime : datetime
+    created_at_datetime : :class:`datetime`
         The created_at converted to datetime.
-    user: User
+    user: :class:`User`
         Author of the tweet.
-    text : str
+    text : :class:`str`
         The full text of the tweet.
-    lang : str
+    lang : :class:`str`
         The language of the tweet.
-    in_reply_to : str
+    in_reply_to : :class:`str`
         The tweet ID this tweet is in reply to, if any
-    is_quote_status : bool
+    is_quote_status : :class:`bool`
         Indicates if the tweet is a quote status.
-    quote : Tweet
+    quote : :class:`Tweet`
         The Tweet being quoted (if any)
-    retweeted : bool
+    retweeted : :class:`bool`
         Whether the tweet is a retweet
-    possibly_sensitive : bool
+    possibly_sensitive : :class:`bool`
         Indicates if the tweet content may be sensitive.
-    possibly_sensitive_editable : bool
+    possibly_sensitive_editable : :class:`bool`
         Indicates if the tweet's sensitivity can be edited.
-    quote_count : int
+    quote_count : :class:`int`
         The count of quotes for the tweet.
-    media : list
+    media : :class:`list`
         A list of media entities associated with the tweet.
-    reply_count : int
+    reply_count : :class:`int`
         The count of replies to the tweet.
-    favorite_count : int
+    favorite_count : :class:`int`
         The count of favorites or likes for the tweet.
-    favorited : bool
+    favorited : :class:`bool`
         Indicates if the tweet is favorited.
-    view_count: int
+    view_count: :class:`int`
         The count of views.
-    retweet_count : int
+    retweet_count : :class:`int`
         The count of retweets for the tweet.
-    editable_until_msecs : int
+    editable_until_msecs : :class:`int`
         The timestamp until which the tweet is editable.
-    is_translatable : bool
+    is_translatable : :class:`bool`
         Indicates if the tweet is translatable.
-    is_edit_eligible : bool
+    is_edit_eligible : :class:`bool`
         Indicates if the tweet is eligible for editing.
-    edits_remaining : int
+    edits_remaining : :class:`int`
         The remaining number of edits allowed for the tweet.
-    state : str
+    state : :class:`str`
         The state of the tweet views.
-    replies: Result[Tweet] | None
+    replies: Result[:class:`Tweet`] | None
         Replies to the tweet.
-    reply_to: list[Tweet] | None
+    reply_to: list[:class:`Tweet`] | None
         A list of Tweet objects representing the tweets to which to reply.
-    related_tweets : list[Tweet] | None
+    related_tweets : list[:class:`Tweet`] | None
         Related tweets.
-    hashtags: list[str]
+    hashtags: list[:class:`str`]
         Hashtags included in the tweet text.
+    poll : :class:`Poll`
+        Poll attached to the tweet.
     """
 
     def __init__(self, client: Client, data: dict, user: User = None) -> None:
         self._client = client
         self._data = data
         self.user = user
 
@@ -172,226 +174,226 @@
     def created_at_datetime(self) -> datetime:
         return timestamp_to_datetime(self.created_at)
 
     @property
     def poll(self) -> Poll:
         return self._poll_data and Poll(self._client, self._poll_data, self)
 
-    async def delete(self) -> Response:
+    def delete(self) -> Response:
         """Deletes the tweet.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         Examples
         --------
-        >>> await tweet.delete()
+        >>> tweet.delete()
         """
-        return await self._client.delete_tweet(self.id)
+        return self._client.delete_tweet(self.id)
 
-    async def favorite(self) -> Response:
+    def favorite(self) -> Response:
         """
         Favorites the tweet.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.favorite_tweet
         """
-        return await self._client.favorite_tweet(self.id)
+        return self._client.favorite_tweet(self.id)
 
-    async def unfavorite(self) -> Response:
+    def unfavorite(self) -> Response:
         """
         Favorites the tweet.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.unfavorite_tweet
         """
-        return await self._client.unfavorite_tweet(self.id)
+        return self._client.unfavorite_tweet(self.id)
 
-    async def retweet(self) -> Response:
+    def retweet(self) -> Response:
         """
         Retweets the tweet.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.retweet
         """
-        return await self._client.retweet(self.id)
+        return self._client.retweet(self.id)
 
-    async def delete_retweet(self) -> Response:
+    def delete_retweet(self) -> Response:
         """
         Deletes the retweet.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.delete_retweet
         """
-        return await self._client.delete_retweet(self.id)
+        return self._client.delete_retweet(self.id)
 
-    async def bookmark(self) -> Response:
+    def bookmark(self) -> Response:
         """
         Adds the tweet to bookmarks.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.bookmark_tweet
         """
-        return await self._client.bookmark_tweet(self.id)
+        return self._client.bookmark_tweet(self.id)
 
-    async def delete_bookmark(self) -> Response:
+    def delete_bookmark(self) -> Response:
         """
         Removes the tweet from bookmarks.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.delete_bookmark
         """
-        return await self._client.delete_bookmark(self.id)
+        return self._client.delete_bookmark(self.id)
 
-    async def reply(
+    def reply(
         self,
         text: str = '',
         media_ids: list[str] | None = None,
         **kwargs
     ) -> Tweet:
         """
         Replies to the tweet.
 
         Parameters
         ----------
-        text : str, default=''
+        text : :class:`str`, default=''
             The text content of the reply.
-        media_ids : list[str], default=None
+        media_ids : list[:class:`str`], default=None
             A list of media IDs or URIs to attach to the reply.
             Media IDs can be obtained by using the `upload_media` method.
 
         Returns
         -------
-        Tweet
+        :class:`Tweet`
             The created tweet.
 
         Examples
         --------
         >>> tweet_text = 'Example text'
         >>> media_ids = [
         ...     client.upload_media('image1.png'),
         ...     client.upload_media('image2.png')
         ... ]
-        >>> await tweet.reply(
+        >>> tweet.reply(
         ...     tweet_text,
         ...     media_ids=media_ids
         ... )
 
         See Also
         --------
         `Client.upload_media`
         """
-        return await self._client.create_tweet(
+        return self._client.create_tweet(
             text, media_ids, reply_to=self.id, **kwargs
         )
 
-    async def get_retweeters(
+    def get_retweeters(
         self, count: str = 40, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieve users who retweeted the tweet.
 
         Parameters
         ----------
-        count : int, default=40
+        count : :class:`int`, default=40
             The maximum number of users to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A string indicating the position of the cursor for pagination.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of users who retweeted the tweet.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> retweeters = tweet.get_retweeters()
         >>> print(retweeters)
         [<User id="...">, <User id="...">, ..., <User id="...">]
 
         >>> more_retweeters = retweeters.next()  # Retrieve more retweeters.
         >>> print(more_retweeters)
         [<User id="...">, <User id="...">, ..., <User id="...">]
         """
-        return await self._client.get_retweeters(self.id, count, cursor)
+        return self._client.get_retweeters(self.id, count, cursor)
 
-    async def get_favoriters(
+    def get_favoriters(
         self, count: str = 40, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieve users who favorited a specific tweet.
 
         Parameters
         ----------
-        tweet_id : str
+        tweet_id : :class:`str`
             The ID of the tweet.
         count : int, default=40
             The maximum number of users to retrieve.
-        cursor : str, default=None
+        cursor : :class:`str`, default=None
             A string indicating the position of the cursor for pagination.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of users who favorited the tweet.
 
         Examples
         --------
         >>> tweet_id = '...'
         >>> favoriters = tweet.get_favoriters()
         >>> print(favoriters)
         [<User id="...">, <User id="...">, ..., <User id="...">]
 
         >>> more_favoriters = favoriters.next()  # Retrieve more favoriters.
         >>> print(more_favoriters)
         [<User id="...">, <User id="...">, ..., <User id="...">]
         """
-        return await self._client.get_favoriters(self.id, count, cursor)
+        return self._client.get_favoriters(self.id, count, cursor)
 
-    async def update(self) -> None:
-        new = await self._client.get_tweet_by_id(self.id)
+    def update(self) -> None:
+        new = self._client.get_tweet_by_id(self.id)
         self.__dict__.update(new.__dict__)
 
     def __repr__(self) -> str:
         return f'<Tweet id="{self.id}">'
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, Tweet) and self.id == __value.id
@@ -407,50 +409,51 @@
         self.id = data['rest_id']
         self.execute_at: int = data['scheduling_info']['execute_at']
         self.state: str = data['scheduling_info']['state']
         self.type: str = data['tweet_create_request']['type']
         self.text: str = data['tweet_create_request']['status']
         self.media = [i['media_info'] for i in data.get('media_entities', [])]
 
-    async def delete(self) -> Response:
+    def delete(self) -> Response:
         """
         Delete the scheduled tweet.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
         """
-        return await self._client.delete_scheduled_tweet(self.id)
+        return self._client.delete_scheduled_tweet(self.id)
 
     def __repr__(self) -> str:
         return f'<ScheduledTweet id="{self.id}">'
 
 
 class Poll:
     """Represents a poll associated with a tweet.
+
     Attributes
     ----------
-    tweet : Tweet
+    tweet : :class:`Tweet`
         The tweet associated with the poll.
-    id : str
+    id : :class:`str`
         The unique identifier of the poll.
-    name : str
+    name : :class:`str`
         The name of the poll.
-    choices : list of dict
+    choices : list[:class:`dict`]
         A list containing dictionaries representing poll choices.
         Each dictionary contains 'label' and 'count' keys
         for choice label and count.
-    duration_minutes : int
+    duration_minutes : :class:`int`
         The duration of the poll in minutes.
-    end_datetime_utc : str
+    end_datetime_utc : :class:`str`
         The end date and time of the poll in UTC format.
-    last_updated_datetime_utc : str
+    last_updated_datetime_utc : :class:`str`
         The last updated date and time of the poll in UTC format.
-    selected_choice : str | None
+    selected_choice : :class:`str` | None
         Number of the selected choice.
     """
 
     def __init__(
         self, client: Client, data: dict, tweet: Tweet | None = None
     ) -> None:
         self._client = client
@@ -497,34 +500,36 @@
 
         if 'selected_choice' in binding_values:
             selected_choice = binding_values['selected_choice']['string_value']
             self.selected_choice: str = selected_choice
         else:
             self.selected_choice = None
 
-    async def vote(self, selected_choice: str) -> Poll:
+    def vote(self, selected_choice: str) -> Poll:
         """
         Vote on the poll with the specified selected choice.
+
         Parameters
         ----------
-        selected_choice : str
+        selected_choice : :class:`str`
             The label of the selected choice for the vote.
+
         Returns
         -------
-        Poll
+        :class:`Poll`
             The Poll object representing the updated poll after voting.
         """
-        return await self._client.vote(
+        return self._client.vote(
             selected_choice,
             self.id,
             self.tweet.id,
             self.name
         )
 
     def __repr__(self) -> str:
         return f'<Poll id="{self.id}">'
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, Poll) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
-        return not self == __value
+        return not self == __value
```

### Comparing `twikit-1.4.4/twikit/twikit_async/user.py` & `twikit-1.4.5/twikit/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import TYPE_CHECKING, Literal
 
-from ..utils import timestamp_to_datetime
+from .utils import timestamp_to_datetime
 
 if TYPE_CHECKING:
     from httpx import Response
 
     from .client import Client
     from .message import Message
     from .tweet import Tweet
     from .utils import Result
 
 
 class User:
     """
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The unique identifier of the user.
-    created_at : str
+    created_at : :class:`str`
         The date and time when the user account was created.
-    name : str
+    name : :class:`str`
         The user's name.
-    screen_name : str
+    screen_name : :class:`str`
         The user's screen name.
-    profile_image_url : str
+    profile_image_url : :class:`str`
         The URL of the user's profile image (HTTPS version).
-    profile_banner_url : str
+    profile_banner_url : :class:`str`
         The URL of the user's profile banner.
-    url : str
+    url : :class:`str`
         The user's URL.
-    location : str
+    location : :class:`str`
         The user's location information.
-    description : str
+    description : :class:`str`
         The user's profile description.
-    description_urls : list
+    description_urls : :class:`list`
         URLs found in the user's profile description.
-    urls : list
+    urls : :class:`list`
         URLs associated with the user.
-    pinned_tweet_ids : str
+    pinned_tweet_ids : :class:`str`
         The IDs of tweets that the user has pinned to their profile.
-    is_blue_verified : bool
+    is_blue_verified : :class:`bool`
         Indicates if the user is verified with a blue checkmark.
-    verified : bool
+    verified : :class:`bool`
         Indicates if the user is verified.
-    possibly_sensitive : bool
+    possibly_sensitive : :class:`bool`
         Indicates if the user's content may be sensitive.
-    can_dm : bool
+    can_dm : :class:`bool`
         Indicates whether the user can receive direct messages.
-    can_media_tag : bool
+    can_media_tag : :class:`bool`
         Indicates whether the user can be tagged in media.
-    want_retweets : bool
+    want_retweets : :class:`bool`
         Indicates if the user wants retweets.
-    default_profile : bool
+    default_profile : :class:`bool`
         Indicates if the user has the default profile.
-    default_profile_image : bool
+    default_profile_image : :class:`bool`
         Indicates if the user has the default profile image.
-    has_custom_timelines : bool
+    has_custom_timelines : :class:`bool`
         Indicates if the user has custom timelines.
-    followers_count : int
+    followers_count : :class:`int`
         The count of followers.
-    fast_followers_count : int
+    fast_followers_count : :class:`int`
         The count of fast followers.
-    normal_followers_count : int
+    normal_followers_count : :class:`int`
         The count of normal followers.
-    following_count : int
+    following_count : :class:`int`
         The count of users the user is following.
-    favourites_count : int
+    favourites_count : :class:`int`
         The count of favorites or likes.
-    listed_count : int
+    listed_count : :class:`int`
         The count of lists the user is a member of.
-    media_count : int
+    media_count : :class:`int`
         The count of media items associated with the user.
-    statuses_count : int
+    statuses_count : :class:`int`
         The count of tweets.
-    is_translator : bool
+    is_translator : :class:`bool`
         Indicates if the user is a translator.
-    translator_type : str
+    translator_type : :class:`str`
         The type of translator.
-    profile_interstitial_type : str
+    profile_interstitial_type : :class:`str`
         The type of profile interstitial.
-    withheld_in_countries : list[str]
+    withheld_in_countries : list[:class:`str`]
         Countries where the user's content is withheld.
     """
 
     def __init__(self, client: Client, data: dict) -> None:
         self._client = client
         legacy = data['legacy']
 
@@ -123,339 +123,339 @@
         self.translator_type: str = legacy['translator_type']
         self.withheld_in_countries: list[str] = legacy['withheld_in_countries']
 
     @property
     def created_at_datetime(self) -> datetime:
         return timestamp_to_datetime(self.created_at)
 
-    async def get_tweets(
+    def get_tweets(
         self,
         tweet_type: Literal['Tweets', 'Replies', 'Media', 'Likes'],
         count: int = 40,
     ) -> Result[Tweet]:
         """
         Retrieves the user's tweets.
 
         Parameters
         ----------
         tweet_type : {'Tweets', 'Replies', 'Media', 'Likes'}
             The type of tweets to retrieve.
-        count : int, default=40
+        count : :class:`int`, default=40
             The number of tweets to retrieve.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing a list of `Tweet` objects.
 
         Examples
         --------
-        >>> user = await client.get_user_by_screen_name('example_user')
-        >>> tweets = await user.get_tweets('Tweets', count=20)
+        >>> user = client.get_user_by_screen_name('example_user')
+        >>> tweets = user.get_tweets('Tweets', count=20)
         >>> for tweet in tweets:
         ...    print(tweet)
         <Tweet id="...">
         <Tweet id="...">
         ...
         ...
 
-        >>> more_tweets = await tweets.next()  # Retrieve more tweets
+        >>> more_tweets = tweets.next()  # Retrieve more tweets
         >>> for tweet in more_tweets:
         ...     print(tweet)
         <Tweet id="...">
         <Tweet id="...">
         ...
         ...
         """
-        return await self._client.get_user_tweets(self.id, tweet_type, count)
+        return self._client.get_user_tweets(self.id, tweet_type, count)
 
-    async def follow(self) -> Response:
+    def follow(self) -> Response:
         """
         Follows the user.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.follow_user
         """
-        return await self._client.follow_user(self.id)
+        return self._client.follow_user(self.id)
 
-    async def unfollow(self) -> Response:
+    def unfollow(self) -> Response:
         """
         Unfollows the user.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.unfollow_user
         """
-        return await self._client.unfollow_user(self.id)
+        return self._client.unfollow_user(self.id)
 
-    async def block(self) -> Response:
+    def block(self) -> Response:
         """
         Blocks a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to block.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .unblock
         """
-        return await self._client.block_user(self.id)
+        return self._client.block_user(self.id)
 
-    async def unblock(self) -> Response:
+    def unblock(self) -> Response:
         """
         Unblocks a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to unblock.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .block
         """
-        return await self._client.unblock_user(self.id)
+        return self._client.unblock_user(self.id)
 
-    async def mute(self) -> Response:
+    def mute(self) -> Response:
         """
         Mutes a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to mute.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .unmute
         """
-        return await self._client.mute_user(self.id)
+        return self._client.mute_user(self.id)
 
-    async def unmute(self) -> Response:
+    def unmute(self) -> Response:
         """
         Unmutes a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to unmute.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .mute
         """
-        return await self._client.unmute_user(self.id)
+        return self._client.unmute_user(self.id)
 
-    async def get_followers(self, count: int = 20) -> Result[User]:
+    def get_followers(self, count: int = 20) -> Result[User]:
         """
         Retrieves a list of followers for the user.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of followers to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the followers.
 
         See Also
         --------
         Client.get_user_followers
         """
-        return await self._client.get_user_followers(self.id, count)
+        return self._client.get_user_followers(self.id, count)
 
-    async def get_verified_followers(self, count: int = 20) -> Result[User]:
+    def get_verified_followers(self, count: int = 20) -> Result[User]:
         """
         Retrieves a list of verified followers for the user.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of verified followers to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the verified followers.
 
         See Also
         --------
         Client.get_user_verified_followers
         """
-        return await self._client.get_user_verified_followers(self.id, count)
+        return self._client.get_user_verified_followers(self.id, count)
 
-    async def get_followers_you_know(self, count: int = 20) -> Result[User]:
+    def get_followers_you_know(self, count: int = 20) -> Result[User]:
         """
         Retrieves a list of followers whom the user might know.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of followers you might know to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the followers you might know.
 
         See Also
         --------
         Client.get_user_followers_you_know
         """
-        return await self._client.get_user_followers_you_know(self.id, count)
+        return self._client.get_user_followers_you_know(self.id, count)
 
-    async def get_following(self, count: int = 20) -> Result[User]:
+    def get_following(self, count: int = 20) -> Result[User]:
         """
         Retrieves a list of users whom the user is following.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of following users to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the users being followed.
 
         See Also
         --------
         Client.get_user_following
         """
-        return await self._client.get_user_following(self.id, count)
+        return self._client.get_user_following(self.id, count)
 
-    async def get_subscriptions(self, count: int = 20) -> Result[User]:
+    def get_subscriptions(self, count: int = 20) -> Result[User]:
         """
         Retrieves a list of users whom the user is subscribed to.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of subscriptions to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the subscribed users.
 
         See Also
         --------
         Client.get_user_subscriptions
         """
-        return await self._client.get_user_subscriptions(self.id, count)
+        return self._client.get_user_subscriptions(self.id, count)
 
-    async def send_dm(
+    def send_dm(
         self, text: str, media_id: str = None, reply_to = None
     ) -> Message:
         """
         Send a direct message to the user.
 
         Parameters
         ----------
-        text : str
+        text : :class:`str`
             The text content of the direct message.
-        media_id : str, default=None
+        media_id : :class:`str`, default=None
             The media ID associated with any media content
             to be included in the message.
             Media ID can be received by using the :func:`.upload_media` method.
-        reply_to : str, default=None
+        reply_to : :class:`str`, default=None
             Message ID to reply to.
 
         Returns
         -------
-        Message
+        :class:`Message`
             `Message` object containing information about the message sent.
 
         Examples
         --------
         >>> # send DM with media
-        >>> media_id = await client.upload_media('image.png')
-        >>> message = await user.send_dm('text', media_id)
+        >>> media_id = client.upload_media('image.png')
+        >>> message = user.send_dm('text', media_id)
         >>> print(message)
-        <Message id="...">
+        <Message id='...'>
 
         See Also
         --------
         Client.upload_media
         Client.send_dm
         """
-        return await self._client.send_dm(self.id, text, media_id, reply_to)
+        return self._client.send_dm(self.id, text, media_id, reply_to)
 
-    async def get_dm_history(self, max_id: str = None) -> Result[Message]:
+    def get_dm_history(self, max_id: str = None) -> Result[Message]:
         """
         Retrieves the DM conversation history with the user.
 
         Parameters
         ----------
-        max_id : str, default=None
+        max_id : :class:`str`, default=None
             If specified, retrieves messages older than the specified max_id.
 
         Returns
         -------
-        Result[Message]
+        Result[:class:`Message`]
             A Result object containing a list of Message objects representing
             the DM conversation history.
 
         Examples
         --------
-        >>> messages = await user.get_dm_history()
+        >>> messages = user.get_dm_history()
         >>> for message in messages:
         >>>     print(message)
         <Message id="...">
         <Message id="...">
         ...
         ...
 
-        >>> more_messages = await messages.next()  # Retrieve more messages
+        >>> more_messages = messages.next()  # Retrieve more messages
         >>> for message in more_messages:
         >>>     print(message)
         <Message id="...">
         <Message id="...">
         ...
         ...
         """
-        return await self._client.get_dm_history(self.id, max_id)
+        return self._client.get_dm_history(self.id, max_id)
 
-    async def update(self) -> None:
-        new = await self._client.get_user_by_id(self.id)
+    def update(self) -> None:
+        new = self._client.get_user_by_id(self.id)
         self.__dict__.update(new.__dict__)
 
     def __repr__(self) -> str:
         return f'<User id="{self.id}">'
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, User) and self.id == __value.id
```

### Comparing `twikit-1.4.4/twikit/twikit_async/utils.py` & `twikit-1.4.5/twikit/twikit_async/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,21 +14,21 @@
     This class is for storing multiple results.
     The `next` method can be used to retrieve further results.
     As with a regular list, you can access elements by
     specifying indexes and iterate over elements using a for loop.
 
     Attributes
     ----------
-    next_cursor : str
+    next_cursor : :class:`str`
         Cursor used to obtain the next result.
-    previous_cursor : str
+    previous_cursor : :class:`str`
         Cursor used to obtain the previous result.
-    token : str
+    token : :class:`str`
         Alias of `next_cursor`.
-    cursor : str
+    cursor : :class:`str`
         Alias of `next_cursor`.
     """
 
     def __init__(
         self,
         results: list[T],
         fetch_next_result: Awaitable | None = None,
```

### Comparing `twikit-1.4.4/twikit/user.py` & `twikit-1.4.5/twikit/twikit_async/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import TYPE_CHECKING, Literal
 
-from .utils import timestamp_to_datetime
+from ..utils import timestamp_to_datetime
 
 if TYPE_CHECKING:
     from httpx import Response
 
     from .client import Client
     from .message import Message
     from .tweet import Tweet
     from .utils import Result
 
 
 class User:
     """
     Attributes
     ----------
-    id : str
+    id : :class:`str`
         The unique identifier of the user.
-    created_at : str
+    created_at : :class:`str`
         The date and time when the user account was created.
-    name : str
+    name : :class:`str`
         The user's name.
-    screen_name : str
+    screen_name : :class:`str`
         The user's screen name.
-    profile_image_url : str
+    profile_image_url : :class:`str`
         The URL of the user's profile image (HTTPS version).
-    profile_banner_url : str
+    profile_banner_url : :class:`str`
         The URL of the user's profile banner.
-    url : str
+    url : :class:`str`
         The user's URL.
-    location : str
+    location : :class:`str`
         The user's location information.
-    description : str
+    description : :class:`str`
         The user's profile description.
-    description_urls : list
+    description_urls : :class:`list`
         URLs found in the user's profile description.
-    urls : list
+    urls : :class:`list`
         URLs associated with the user.
-    pinned_tweet_ids : str
+    pinned_tweet_ids : :class:`str`
         The IDs of tweets that the user has pinned to their profile.
-    is_blue_verified : bool
+    is_blue_verified : :class:`bool`
         Indicates if the user is verified with a blue checkmark.
-    verified : bool
+    verified : :class:`bool`
         Indicates if the user is verified.
-    possibly_sensitive : bool
+    possibly_sensitive : :class:`bool`
         Indicates if the user's content may be sensitive.
-    can_dm : bool
+    can_dm : :class:`bool`
         Indicates whether the user can receive direct messages.
-    can_media_tag : bool
+    can_media_tag : :class:`bool`
         Indicates whether the user can be tagged in media.
-    want_retweets : bool
+    want_retweets : :class:`bool`
         Indicates if the user wants retweets.
-    default_profile : bool
+    default_profile : :class:`bool`
         Indicates if the user has the default profile.
-    default_profile_image : bool
+    default_profile_image : :class:`bool`
         Indicates if the user has the default profile image.
-    has_custom_timelines : bool
+    has_custom_timelines : :class:`bool`
         Indicates if the user has custom timelines.
-    followers_count : int
+    followers_count : :class:`int`
         The count of followers.
-    fast_followers_count : int
+    fast_followers_count : :class:`int`
         The count of fast followers.
-    normal_followers_count : int
+    normal_followers_count : :class:`int`
         The count of normal followers.
-    following_count : int
+    following_count : :class:`int`
         The count of users the user is following.
-    favourites_count : int
+    favourites_count : :class:`int`
         The count of favorites or likes.
-    listed_count : int
+    listed_count : :class:`int`
         The count of lists the user is a member of.
-    media_count : int
+    media_count : :class:`int`
         The count of media items associated with the user.
-    statuses_count : int
+    statuses_count : :class:`int`
         The count of tweets.
-    is_translator : bool
+    is_translator : :class:`bool`
         Indicates if the user is a translator.
-    translator_type : str
+    translator_type : :class:`str`
         The type of translator.
-    profile_interstitial_type : str
+    profile_interstitial_type : :class:`str`
         The type of profile interstitial.
-    withheld_in_countries : list[str]
+    withheld_in_countries : list[:class:`str`]
         Countries where the user's content is withheld.
     """
 
     def __init__(self, client: Client, data: dict) -> None:
         self._client = client
         legacy = data['legacy']
 
@@ -123,339 +123,339 @@
         self.translator_type: str = legacy['translator_type']
         self.withheld_in_countries: list[str] = legacy['withheld_in_countries']
 
     @property
     def created_at_datetime(self) -> datetime:
         return timestamp_to_datetime(self.created_at)
 
-    def get_tweets(
+    async def get_tweets(
         self,
         tweet_type: Literal['Tweets', 'Replies', 'Media', 'Likes'],
         count: int = 40,
     ) -> Result[Tweet]:
         """
         Retrieves the user's tweets.
 
         Parameters
         ----------
         tweet_type : {'Tweets', 'Replies', 'Media', 'Likes'}
             The type of tweets to retrieve.
-        count : int, default=40
+        count : :class:`int`, default=40
             The number of tweets to retrieve.
 
         Returns
         -------
-        Result[Tweet]
+        Result[:class:`Tweet`]
             A Result object containing a list of `Tweet` objects.
 
         Examples
         --------
-        >>> user = client.get_user_by_screen_name('example_user')
-        >>> tweets = user.get_tweets('Tweets', count=20)
+        >>> user = await client.get_user_by_screen_name('example_user')
+        >>> tweets = await user.get_tweets('Tweets', count=20)
         >>> for tweet in tweets:
         ...    print(tweet)
         <Tweet id="...">
         <Tweet id="...">
         ...
         ...
 
-        >>> more_tweets = tweets.next()  # Retrieve more tweets
+        >>> more_tweets = await tweets.next()  # Retrieve more tweets
         >>> for tweet in more_tweets:
         ...     print(tweet)
         <Tweet id="...">
         <Tweet id="...">
         ...
         ...
         """
-        return self._client.get_user_tweets(self.id, tweet_type, count)
+        return await self._client.get_user_tweets(self.id, tweet_type, count)
 
-    def follow(self) -> Response:
+    async def follow(self) -> Response:
         """
         Follows the user.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.follow_user
         """
-        return self._client.follow_user(self.id)
+        return await self._client.follow_user(self.id)
 
-    def unfollow(self) -> Response:
+    async def unfollow(self) -> Response:
         """
         Unfollows the user.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         Client.unfollow_user
         """
-        return self._client.unfollow_user(self.id)
+        return await self._client.unfollow_user(self.id)
 
-    def block(self) -> Response:
+    async def block(self) -> Response:
         """
         Blocks a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to block.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .unblock
         """
-        return self._client.block_user(self.id)
+        return await self._client.block_user(self.id)
 
-    def unblock(self) -> Response:
+    async def unblock(self) -> Response:
         """
         Unblocks a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to unblock.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .block
         """
-        return self._client.unblock_user(self.id)
+        return await self._client.unblock_user(self.id)
 
-    def mute(self) -> Response:
+    async def mute(self) -> Response:
         """
         Mutes a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to mute.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .unmute
         """
-        return self._client.mute_user(self.id)
+        return await self._client.mute_user(self.id)
 
-    def unmute(self) -> Response:
+    async def unmute(self) -> Response:
         """
         Unmutes a user.
 
         Parameters
         ----------
-        user_id : str
+        user_id : :class:`str`
             The ID of the user to unmute.
 
         Returns
         -------
-        httpx.Response
+        :class:`httpx.Response`
             Response returned from twitter api.
 
         See Also
         --------
         .mute
         """
-        return self._client.unmute_user(self.id)
+        return await self._client.unmute_user(self.id)
 
-    def get_followers(self, count: int = 20) -> Result[User]:
+    async def get_followers(self, count: int = 20) -> Result[User]:
         """
         Retrieves a list of followers for the user.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of followers to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the followers.
 
         See Also
         --------
         Client.get_user_followers
         """
-        return self._client.get_user_followers(self.id, count)
+        return await self._client.get_user_followers(self.id, count)
 
-    def get_verified_followers(self, count: int = 20) -> Result[User]:
+    async def get_verified_followers(self, count: int = 20) -> Result[User]:
         """
         Retrieves a list of verified followers for the user.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of verified followers to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the verified followers.
 
         See Also
         --------
         Client.get_user_verified_followers
         """
-        return self._client.get_user_verified_followers(self.id, count)
+        return await self._client.get_user_verified_followers(self.id, count)
 
-    def get_followers_you_know(self, count: int = 20) -> Result[User]:
+    async def get_followers_you_know(self, count: int = 20) -> Result[User]:
         """
         Retrieves a list of followers whom the user might know.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of followers you might know to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the followers you might know.
 
         See Also
         --------
         Client.get_user_followers_you_know
         """
-        return self._client.get_user_followers_you_know(self.id, count)
+        return await self._client.get_user_followers_you_know(self.id, count)
 
-    def get_following(self, count: int = 20) -> Result[User]:
+    async def get_following(self, count: int = 20) -> Result[User]:
         """
         Retrieves a list of users whom the user is following.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of following users to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the users being followed.
 
         See Also
         --------
         Client.get_user_following
         """
-        return self._client.get_user_following(self.id, count)
+        return await self._client.get_user_following(self.id, count)
 
-    def get_subscriptions(self, count: int = 20) -> Result[User]:
+    async def get_subscriptions(self, count: int = 20) -> Result[User]:
         """
         Retrieves a list of users whom the user is subscribed to.
 
         Parameters
         ----------
-        count : int, default=20
+        count : :class:`int`, default=20
             The number of subscriptions to retrieve.
 
         Returns
         -------
-        Result[User]
+        Result[:class:`User`]
             A list of User objects representing the subscribed users.
 
         See Also
         --------
         Client.get_user_subscriptions
         """
-        return self._client.get_user_subscriptions(self.id, count)
+        return await self._client.get_user_subscriptions(self.id, count)
 
-    def send_dm(
+    async def send_dm(
         self, text: str, media_id: str = None, reply_to = None
     ) -> Message:
         """
         Send a direct message to the user.
 
         Parameters
         ----------
-        text : str
+        text : :class:`str`
             The text content of the direct message.
-        media_id : str, default=None
+        media_id : :class:`str`, default=None
             The media ID associated with any media content
             to be included in the message.
             Media ID can be received by using the :func:`.upload_media` method.
-        reply_to : str, default=None
+        reply_to : :class:`str`, default=None
             Message ID to reply to.
 
         Returns
         -------
-        Message
+        :class:`Message`
             `Message` object containing information about the message sent.
 
         Examples
         --------
         >>> # send DM with media
-        >>> media_id = client.upload_media('image.png')
-        >>> message = user.send_dm('text', media_id)
+        >>> media_id = await client.upload_media('image.png')
+        >>> message = await user.send_dm('text', media_id)
         >>> print(message)
-        <Message id='...'>
+        <Message id="...">
 
         See Also
         --------
         Client.upload_media
         Client.send_dm
         """
-        return self._client.send_dm(self.id, text, media_id, reply_to)
+        return await self._client.send_dm(self.id, text, media_id, reply_to)
 
-    def get_dm_history(self, max_id: str = None) -> Result[Message]:
+    async def get_dm_history(self, max_id: str = None) -> Result[Message]:
         """
         Retrieves the DM conversation history with the user.
 
         Parameters
         ----------
-        max_id : str, default=None
+        max_id : :class:`str`, default=None
             If specified, retrieves messages older than the specified max_id.
 
         Returns
         -------
-        Result[Message]
+        Result[:class:`Message`]
             A Result object containing a list of Message objects representing
             the DM conversation history.
 
         Examples
         --------
-        >>> messages = user.get_dm_history()
+        >>> messages = await user.get_dm_history()
         >>> for message in messages:
         >>>     print(message)
         <Message id="...">
         <Message id="...">
         ...
         ...
 
-        >>> more_messages = messages.next()  # Retrieve more messages
+        >>> more_messages = await messages.next()  # Retrieve more messages
         >>> for message in more_messages:
         >>>     print(message)
         <Message id="...">
         <Message id="...">
         ...
         ...
         """
-        return self._client.get_dm_history(self.id, max_id)
+        return await self._client.get_dm_history(self.id, max_id)
 
-    def update(self) -> None:
-        new = self._client.get_user_by_id(self.id)
+    async def update(self) -> None:
+        new = await self._client.get_user_by_id(self.id)
         self.__dict__.update(new.__dict__)
 
     def __repr__(self) -> str:
         return f'<User id="{self.id}">'
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, User) and self.id == __value.id
```

### Comparing `twikit-1.4.4/twikit/utils.py` & `twikit-1.4.5/twikit/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,21 +148,21 @@
     This class is for storing multiple results.
     The `next` method can be used to retrieve further results.
     As with a regular list, you can access elements by
     specifying indexes and iterate over elements using a for loop.
 
     Attributes
     ----------
-    next_cursor : str
+    next_cursor : :class:`str`
         Cursor used to obtain the next result.
-    previous_cursor : str
+    previous_cursor : :class:`str`
         Cursor used to obtain the previous result.
-    token : str
+    token : :class:`str`
         Alias of `next_cursor`.
-    cursor : str
+    cursor : :class:`str`
         Alias of `next_cursor`.
     """
 
     def __init__(
         self,
         results: list[T],
         fetch_next_result: Callable | None = None,
@@ -354,14 +354,22 @@
             'withheld_in_countries': raw_data.get('withheld_in_countries'),
             'url': raw_data.get('url'),
             'profile_banner_url': raw_data.get('profile_banner_url')
         }
     }
 
 
+def flatten_params(params: dict) -> dict:
+    flattened_params = {}
+    for key, value in params.items():
+        if isinstance(value, (list, dict)):
+            value = json.dumps(value)
+        flattened_params[key] = value
+    return flattened_params
+
 FILTERS = Literal[
     'media',
     'retweets',
     'native_video',
     'periscope',
     'vine',
     'images',
```

### Comparing `twikit-1.4.4/twikit.egg-info/PKG-INFO` & `twikit-1.4.5/twikit.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,150 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.4
+Version: 1.4.5
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img src="https://i.imgur.com/iJe6rsZ.png" width="500">
+<img  src="https://i.imgur.com/iJe6rsZ.png"  width="500">
+
+
 
 ![Number of GitHub stars](https://img.shields.io/github/stars/d60/twikit)
+
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/d60/twikit)
+
 ![Version](https://img.shields.io/pypi/v/twikit?label=PyPI)
+
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Create%20your%20own%20Twitter%20bot%20for%20free%20with%20%22Twikit%22!%20%23python%20%23twitter%20%23twikit%20%23programming%20%23github%20%23bot&url=https%3A%2F%2Fgithub.com%2Fd60%2Ftwikit)
+
 [![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/nCrByrr8cX)
+
 [![BuyMeACoffee](https://img.shields.io/badge/-buy_me_a%C2%A0coffee-gray?logo=buy-me-a-coffee)](https://www.buymeacoffee.com/d60py)
 
 
-# Twikit <img height="35" src="https://i.imgur.com/9HSdIl4.png" valign="bottom">
+# Twikit <img height="35"  src="https://i.imgur.com/9HSdIl4.png"  valign="bottom">
+
 simple API wrapper to interact with twitter's unofficial API.
+
 You can log in to Twitter using your account username, email address and password and use most features on Twitter, such as posting and retrieving tweets, liking and following users.
+
 - [Documentation (English)](https://twikit.readthedocs.io/en/latest/twikit.html)
+
 - [Async Documentation](https://twikit.readthedocs.io/en/latest/twikit.twikit_async.html)
 
+
+
 If you have any questions, please ask on [Discord](https://discord.gg/nCrByrr8cX).
 
+
+
 ## Features
+
 ### No API Key Required
-The library uses an unofficial API and therefore does **not require an API key**.
+
+This library uses the unofficial API, therefore does **not require an API key**.
+
 ### Completely Free
-The service is entirely free to use.
+
+This library is completely free to use.
+
 ### Both Synchronous and Asynchronous Support
+
 Whether you prefer **synchronous** or **asynchronous** programming,
+
 Twikit supports both, providing flexibility for different use cases.
 
+
 ## Functionality
+
 This library allows you to perform various Twitter-related actions, including:
-- **Create tweets**
-- **Search tweets**
-- **Retrieve trending topics**
+
+-  **Create tweets**
+
+-  **Search tweets**
+
+-  **Retrieve trending topics**
+
 - etc...
 
+
+
 ## Installing
- ```back
- pip install twikit
- ```
+
+```bash
+
+pip install twikit
+
+```
+
+
 
 ## Quick Example
+
 **Define a client and log in to the account.**
+
 ```python
 from twikit import Client
 
 USERNAME = 'example_user'
 EMAIL = 'email@example.com'
 PASSWORD = 'password0000'
 
 # Initialize client
 client = Client('en-US')
+
 # Login to the service with provided user credentials
 client.login(
     auth_info_1=USERNAME ,
     auth_info_2=EMAIL,
     password=PASSWORD
 )
 ```
+
 **Create a tweet with media attached.**
+
 ```python
 # Upload media files and obtain media_ids
 media_ids = [
     client.upload_media('media1.jpg'),
     client.upload_media('media2.jpg')
 ]
+
 # Create a tweet with the provided text and attached media
 client.create_tweet(
     text='Example Tweet',
     media_ids=media_ids
 )
+
 ```
 
+**Search the latest tweets based on a keywords**
+```python
+tweets = client.search_tweet('python', 'Latest')
+
+for tweet in tweets:
+    print(
+        tweet.user.name,
+        tweet.text,
+        tweet.created_at
+    )
+```
+
+
 More Examples: [examples](https://github.com/d60/twikit/tree/main/examples) <br>
 
+
+
 ## Contributing
+
 I would like to hear your thoughts and suggestions.
+
 If you have any features you'd like to see added or encounter any issues,
+
 please let me know in the [issues](https://github.com/d60/twikit/issues) section.
 
+
 Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library⭐! Thank you very much!
```

### Comparing `twikit-1.4.4/twikit.egg-info/SOURCES.txt` & `twikit-1.4.5/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

