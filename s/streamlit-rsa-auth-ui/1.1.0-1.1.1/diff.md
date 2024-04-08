# Comparing `tmp/streamlit-rsa-auth-ui-1.1.0.tar.gz` & `tmp/streamlit-rsa-auth-ui-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-rsa-auth-ui-1.1.0.tar", last modified: Fri Mar 22 21:10:18 2024, max compression
+gzip compressed data, was "streamlit-rsa-auth-ui-1.1.1.tar", last modified: Mon Apr  8 11:24:32 2024, max compression
```

## Comparing `streamlit-rsa-auth-ui-1.1.0.tar` & `streamlit-rsa-auth-ui-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 21:10:18.335149 streamlit-rsa-auth-ui-1.1.0/
--rw-rw-rw-   0        0        0     1089 2024-03-09 15:15:01.000000 streamlit-rsa-auth-ui-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       56 2024-03-13 13:27:26.000000 streamlit-rsa-auth-ui-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5881 2024-03-22 21:10:18.334148 streamlit-rsa-auth-ui-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5001 2024-03-22 21:09:00.000000 streamlit-rsa-auth-ui-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-22 21:10:18.336149 streamlit-rsa-auth-ui-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1376 2024-03-22 21:08:35.000000 streamlit-rsa-auth-ui-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-22 21:10:18.307150 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/
--rw-rw-rw-   0        0        0      558 2024-03-22 21:07:40.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/__init__.py
--rw-rw-rw-   0        0        0    12211 2024-03-22 20:52:42.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/configs.py
--rw-rw-rw-   0        0        0     1775 2024-03-13 13:27:26.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/encryption.py
--rw-rw-rw-   0        0        0     2039 2024-03-22 21:03:02.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/events.py
--rw-rw-rw-   0        0        0     5444 2024-03-22 21:06:54.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/form.py
-drwxrwxrwx   0        0        0        0 2024-03-22 21:10:18.291909 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/
-drwxrwxrwx   0        0        0        0 2024-03-22 21:10:18.319166 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-03-22 18:56:40.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0      543 2024-03-15 18:28:40.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/index.css
--rw-rw-rw-   0        0        0      477 2024-03-22 18:56:40.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-03-22 21:10:18.292910 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-03-22 21:10:18.324149 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/static/js/
--rw-rw-rw-   0        0        0   983718 2024-03-22 18:56:40.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/static/js/main.2243da37.js
--rw-rw-rw-   0        0        0     2027 2024-03-22 18:56:40.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/static/js/main.2243da37.js.LICENSE.txt
--rw-rw-rw-   0        0        0  4135400 2024-03-22 18:56:40.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/static/js/main.2243da37.js.map
-drwxrwxrwx   0        0        0        0 2024-03-22 21:10:18.315149 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui.egg-info/
--rw-rw-rw-   0        0        0     5881 2024-03-22 21:10:18.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2024-03-22 21:10:18.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 21:10:18.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      149 2024-03-22 21:10:18.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-03-22 21:10:18.000000 streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 11:24:32.220180 streamlit-rsa-auth-ui-1.1.1/
+-rw-rw-rw-   0        0        0     1089 2024-03-11 00:20:19.000000 streamlit-rsa-auth-ui-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       56 2024-03-12 11:42:33.000000 streamlit-rsa-auth-ui-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6001 2024-04-08 11:24:32.215374 streamlit-rsa-auth-ui-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5123 2024-04-08 11:23:34.000000 streamlit-rsa-auth-ui-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 11:24:32.221176 streamlit-rsa-auth-ui-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1376 2024-04-08 11:21:34.000000 streamlit-rsa-auth-ui-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 11:24:32.145631 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/
+-rw-rw-rw-   0        0        0      558 2024-03-23 03:49:35.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/__init__.py
+-rw-rw-rw-   0        0        0    12211 2024-03-23 03:49:35.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/configs.py
+-rw-rw-rw-   0        0        0     1775 2024-03-12 06:44:42.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/encryption.py
+-rw-rw-rw-   0        0        0     2189 2024-04-08 11:21:57.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/events.py
+-rw-rw-rw-   0        0        0     5444 2024-03-23 03:49:35.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/form.py
+drwxrwxrwx   0        0        0        0 2024-04-08 11:24:32.110796 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-08 11:24:32.181585 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-03-20 06:40:26.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0      543 2024-03-15 15:51:14.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/index.css
+-rw-rw-rw-   0        0        0      477 2024-03-20 06:40:26.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-08 11:24:32.110796 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-08 11:24:32.197610 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   983699 2024-03-20 06:40:26.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/static/js/main.3bc257bc.js
+-rw-rw-rw-   0        0        0     2027 2024-03-20 06:40:26.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/static/js/main.3bc257bc.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  4135496 2024-03-20 06:40:26.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/static/js/main.3bc257bc.js.map
+drwxrwxrwx   0        0        0        0 2024-04-08 11:24:32.169225 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui.egg-info/
+-rw-rw-rw-   0        0        0     6001 2024-04-08 11:24:31.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2024-04-08 11:24:32.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 11:24:31.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      149 2024-04-08 11:24:31.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-08 11:24:32.000000 streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui.egg-info/top_level.txt
```

### Comparing `streamlit-rsa-auth-ui-1.1.0/LICENSE` & `streamlit-rsa-auth-ui-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-rsa-auth-ui-1.1.0/PKG-INFO` & `streamlit-rsa-auth-ui-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-rsa-auth-ui
-Version: 1.1.0
+Version: 1.1.1
 Summary: Streamlit RSA Authenticator UI
 Home-page: https://github.com/NathanChen198/streamlit-rsa-auth-ui
 Author: Nathan Chen
 Author-email: nathan.chen.198@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,63 +29,73 @@
 [![GitHub license][license_badge]][license_link]
 [![GitHub issues][issue_badge]][issue_link]
 [![GitHub pull requests][pull_badge]][pull_link]
 
 Encryption on Authenticate widget data from client to server.
 
 ## What is Streamlit RSA Authenticator UI?
+
 ### What is Http protocol
+
 Http is the information transfer protocol between networked devices. However, all the requests and responses are in plaintext, which means that anyone can read them.
 
 If you want to deploy streamlit server using http protocol (not https protocol) and you add the user authentication, user password can be read by anyone in the network as it is the plaintext for http protocol.
 
 `streamlit-rsa-auth-ui` correct it by encrypting user information including password at the client browser before transmit to streamlit server using [RSA algorithm](https://www.techtarget.com/searchsecurity/definition/RSA)
 
 ### What is RSA algorithm
+
 It is [asymmetric cryptography](https://www.techtarget.com/searchsecurity/definition/asymmetric-cryptography), uses two different but mathematically linked [keys](https://www.techtarget.com/searchsecurity/definition/key)
+
 - [Public key](https://www.techtarget.com/searchsecurity/definition/public-key) that can be share with everyone
 - [Private key](https://www.techtarget.com/searchsecurity/definition/private-key) must be kept secret
 
 ## Installation
+
 Open a terminal and run:
 
-``` terminal
+```terminal
 pip install streamlit-rsa-auth-ui
 ```
 
-
 ## Quickstart
+
 ### Gnerate RSA Key Pair
+
 Create a new file generateKeys.py
 
-``` python
+```python
 from streamlit_rsa_auth_ui import Encryptor
 
 encryptor = Encryptor.generateNew(2048)
 encryptor.save('rsa', 'authkey')
 ```
 
 Run `generateKeys.py` python script
-``` terminal
+
+```terminal
 python generateKeys.py
 ```
 
 this will create a private key and public key pair
+
 - private key with the file name `authkey`
 - public key with the file name `authkey.pub`
 
-``` md
+```md
 ├── rsa
-│   ├── authkey
-│   │   authkey.pub
+│ ├── authkey
+│ │ authkey.pub
 ```
 
 ### Create streamlit page
+
 Create a new file example.py
-``` python
+
+```python
 import streamlit as st
 from streamlit_rsa_auth_ui import Encryptor, authUI, SigninEvent, SigninFormConfig, getEvent
 ss = st.session_state
 
 encryptor = Encryptor.load('rsa', 'authkey')
 ui = authUI('login_ui_result', encryptor.publicKeyPem)
 
@@ -117,42 +127,56 @@
 
 st.title('Streamlit Rsa Auth UI Test')
 button = st.button('test')
 button
 ```
 
 Run the streamlit app
-``` terminal
+
+```terminal
 streamlit run example.py
 ```
 
-
 ## Change Log
+
 ### Version 0.0.1
+
 - Initial release
+
 ### Version 0.0.2
+
 - Fix missing frontend issue
+
 ### Version 0.0.3
+
 - Optional 'cancel' button to signoutform
 - Minor bug fixed
 - Remove bootstrap.min.css warning
+
 ### Version 0.0.4
+
 - Remove location setting(seem redundunt as if you want to add to any container/sidebar you can call with syntax)
 - Add in classname to frontend so that easier to add in custom styling if needed
 - Remove off the unnecessary excess height of streamlit
+
 ### Version 1.0.0
+
 - More customizable UI
 - Add inline mode
 - Add ChangePassword UI
+
 ### Version 1.1.0
+
 - Add id property in event if no public key is provided
 - Add AuthUI class
 - Add Configs class
 
+### Version 1.1.1
 
+- Fix 'no remember in signinevent' when remember option is disabled
 
 [pypi_badge]: https://img.shields.io/pypi/v/streamlit-rsa-auth-ui.svg
 [pypi_link]: https://pypi.org/project/streamlit-rsa-auth-ui
 [pypi_download_badge]: https://static.pepy.tech/badge/streamlit-rsa-auth-ui
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-rsa-auth-ui
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
```

### Comparing `streamlit-rsa-auth-ui-1.1.0/README.md` & `streamlit-rsa-auth-ui-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,63 +6,73 @@
 [![GitHub license][license_badge]][license_link]
 [![GitHub issues][issue_badge]][issue_link]
 [![GitHub pull requests][pull_badge]][pull_link]
 
 Encryption on Authenticate widget data from client to server.
 
 ## What is Streamlit RSA Authenticator UI?
+
 ### What is Http protocol
+
 Http is the information transfer protocol between networked devices. However, all the requests and responses are in plaintext, which means that anyone can read them.
 
 If you want to deploy streamlit server using http protocol (not https protocol) and you add the user authentication, user password can be read by anyone in the network as it is the plaintext for http protocol.
 
 `streamlit-rsa-auth-ui` correct it by encrypting user information including password at the client browser before transmit to streamlit server using [RSA algorithm](https://www.techtarget.com/searchsecurity/definition/RSA)
 
 ### What is RSA algorithm
+
 It is [asymmetric cryptography](https://www.techtarget.com/searchsecurity/definition/asymmetric-cryptography), uses two different but mathematically linked [keys](https://www.techtarget.com/searchsecurity/definition/key)
+
 - [Public key](https://www.techtarget.com/searchsecurity/definition/public-key) that can be share with everyone
 - [Private key](https://www.techtarget.com/searchsecurity/definition/private-key) must be kept secret
 
 ## Installation
+
 Open a terminal and run:
 
-``` terminal
+```terminal
 pip install streamlit-rsa-auth-ui
 ```
 
-
 ## Quickstart
+
 ### Gnerate RSA Key Pair
+
 Create a new file generateKeys.py
 
-``` python
+```python
 from streamlit_rsa_auth_ui import Encryptor
 
 encryptor = Encryptor.generateNew(2048)
 encryptor.save('rsa', 'authkey')
 ```
 
 Run `generateKeys.py` python script
-``` terminal
+
+```terminal
 python generateKeys.py
 ```
 
 this will create a private key and public key pair
+
 - private key with the file name `authkey`
 - public key with the file name `authkey.pub`
 
-``` md
+```md
 ├── rsa
-│   ├── authkey
-│   │   authkey.pub
+│ ├── authkey
+│ │ authkey.pub
 ```
 
 ### Create streamlit page
+
 Create a new file example.py
-``` python
+
+```python
 import streamlit as st
 from streamlit_rsa_auth_ui import Encryptor, authUI, SigninEvent, SigninFormConfig, getEvent
 ss = st.session_state
 
 encryptor = Encryptor.load('rsa', 'authkey')
 ui = authUI('login_ui_result', encryptor.publicKeyPem)
 
@@ -94,47 +104,61 @@
 
 st.title('Streamlit Rsa Auth UI Test')
 button = st.button('test')
 button
 ```
 
 Run the streamlit app
-``` terminal
+
+```terminal
 streamlit run example.py
 ```
 
-
 ## Change Log
+
 ### Version 0.0.1
+
 - Initial release
+
 ### Version 0.0.2
+
 - Fix missing frontend issue
+
 ### Version 0.0.3
+
 - Optional 'cancel' button to signoutform
 - Minor bug fixed
 - Remove bootstrap.min.css warning
+
 ### Version 0.0.4
+
 - Remove location setting(seem redundunt as if you want to add to any container/sidebar you can call with syntax)
 - Add in classname to frontend so that easier to add in custom styling if needed
 - Remove off the unnecessary excess height of streamlit
+
 ### Version 1.0.0
+
 - More customizable UI
 - Add inline mode
 - Add ChangePassword UI
+
 ### Version 1.1.0
+
 - Add id property in event if no public key is provided
 - Add AuthUI class
 - Add Configs class
 
+### Version 1.1.1
 
+- Fix 'no remember in signinevent' when remember option is disabled
 
 [pypi_badge]: https://img.shields.io/pypi/v/streamlit-rsa-auth-ui.svg
 [pypi_link]: https://pypi.org/project/streamlit-rsa-auth-ui
 [pypi_download_badge]: https://static.pepy.tech/badge/streamlit-rsa-auth-ui
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-rsa-auth-ui
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
 [license_link]: https://github.com/NathanChen198/streamlit-rsa-auth-ui/blob/main/LICENSE
 [issue_badge]: https://img.shields.io/github/issues/NathanChen198/streamlit-rsa-auth-ui
 [issue_link]: https://github.com/NathanChen198/streamlit-rsa-auth-ui/issues
 [pull_badge]: https://img.shields.io/github/issues-pr/NathanChen198/streamlit-rsa-auth-ui
-[pull_link]: https://github.com/NathanChen198/streamlit-rsa-auth-ui/pulls
+[pull_link]: https://github.com/NathanChen198/streamlit-rsa-auth-ui/pulls
```

### Comparing `streamlit-rsa-auth-ui-1.1.0/setup.py` & `streamlit-rsa-auth-ui-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Author   : Nathan Chen
-# Date     : 23-Mar-2024
+# Date     : 08-Apr-2024
 
 
 from pathlib import Path
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='UTF-8')
 
 setup(
     name='streamlit-rsa-auth-ui',
-    version='1.1.0',
+    version='1.1.1',
     author='Nathan Chen',
     author_email='nathan.chen.198@gmail.com',
     description='Streamlit RSA Authenticator UI',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/NathanChen198/streamlit-rsa-auth-ui',
     packages=find_packages(),
```

### Comparing `streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/__init__.py` & `streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/configs.py` & `streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/configs.py`

 * *Files identical despite different names*

### Comparing `streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/encryption.py` & `streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/encryption.py`

 * *Files identical despite different names*

### Comparing `streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/events.py` & `streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/events.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 # Author    : Nathan Chen
-# Date      : 20-Mar-2024
+# Date      : 08-Apr-2024
 
 
-from typing import Literal
+from typing import Literal, Dict
 
 
 EventInfo = Literal['signin', 'cancelSignin', 'signout', 'cancelSignout', 'changePassword', 'cancelChangePassword']
 
 
 class Event:
     event: EventInfo
 
     def __init__(self, event: EventInfo) -> None:
         self.event = event
 
+    def setattr(self, dict: Dict):
+        for key, val in dict.items():
+            self.__setattr__(key, val)
+
 
 class SigninEvent(Event):
     event: EventInfo = 'signin'
     username: str
     password: str
     remember: bool
 
     def __init__(self) -> None:
         super().__init__('signin')
+        self.remember = False
 
 class CancelSigninEvent(Event):
     event: EventInfo = 'cancelSignin'
 
     def __init__(self) -> None:
         super().__init__('cancelSignin')
 
@@ -58,23 +63,23 @@
 
 
 def getEvent(value):
     if type(value) is not dict: return None
     info: EventInfo = value.get('event', None)
     if info == SigninEvent.event:
         event = SigninEvent()
-        event.__dict__ = value
+        event.setattr(value)
     elif info == CancelSigninEvent.event:
         event = CancelSignoutEvent()
     elif info == SignoutEvent.event:
         event = SignoutEvent()
     elif info == CancelSignoutEvent.event:
         event = CancelSignoutEvent()
     elif info == ChangePasswordEvent.event:
         event = ChangePasswordEvent()
-        event.__dict__ = value
+        event.setattr(value)
     elif info == CancelChangePasswordEvent.event:
         event = CancelChangePasswordEvent()
     else:
         event = None
 
     return event
```

### Comparing `streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/form.py` & `streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/form.py`

 * *Files identical despite different names*

### Comparing `streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/index.css` & `streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/index.css`

 * *Files identical despite different names*

### Comparing `streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/static/js/main.2243da37.js` & `streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/static/js/main.3bc257bc.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.2243da37.js.LICENSE.txt */
+/*! For license information please see main.3bc257bc.js.LICENSE.txt */
 (() => {
     var e = {
             5270: (e, t, n) => {
                 "use strict";
                 var r = n(139),
                     i = {
                         "text/plain": "Text",
@@ -40160,15 +40160,15 @@
                 })
             }
             setComponentValue(e) {
                 if (this.publicKey) {
                     const t = JSON.stringify(e);
                     let n = this.publicKey.encrypt(t);
                     n = lE().util.encode64(n), rE.setComponentValue(n)
-                } else e.id = Math.random(), rE.setComponentValue(e)
+                } else rE.setComponentValue(e)
             }
             render() {
                 var e, t, n, r, i;
                 return (0, fE.jsx)("div", {
                     children: (0, fE.jsx)(ty, {
                         theme: {
                             token: {
@@ -40850,8 +40850,8 @@
             })),
             RE = document.getElementById("root");
         (0, r.H)(RE).render((0, fE.jsx)(e.StrictMode, {
             children: (0, fE.jsx)(NE, {})
         }))
     })()
 })();
-//# sourceMappingURL=main.2243da37.js.map
+//# sourceMappingURL=main.3bc257bc.js.map
```

### Comparing `streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/static/js/main.2243da37.js.LICENSE.txt` & `streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/static/js/main.3bc257bc.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui/frontend/build/static/js/main.2243da37.js.map` & `streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui/frontend/build/static/js/main.3bc257bc.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8566166798210997%*

 * *Differences: {"'file'": "'static/js/main.3bc257bc.js'",*

 * * "'mappings'": "';yCAEA,IAAIA,EAAkBC,EAAQ,KAE1BC,EAA4B,CAC9B,aAAc,OACd,YAAa,MACb,QAAW,QA2GbC,EAAOC,QAjGP,SAAcC,EAAMC,GAClB,IAAIC,EACFC,EACAC,EACAC,EACAC,EACAC,EACAC,GAAU,EACPP,IACHA,EAAU,CAAC,GAEbC,EAAQD,EAAQC,QAAS,EACzB,IAkDE,GAjDAE,EAAmBT,IAEnBU,EAAQI,SAASC,cACjBJ,EAAYG,SAASE,gBAErBJ,EAAOE,SAASG,cAAc,SACzBC,YAAcb,EAEnBO,EAAKO,WAAa,OAElBP,EAAKQ,MAAMC,IAAM,QAEjBT,EAAKQ,MAAME,SAAW,QACtBV,EAAKQ,MAAMG,IAAM,EACjBX,EAAKQ,MAAMI,KAAO,mBAElBZ,EAAKQ,MAAMK,WAAa,MAExBb,EAAKQ, […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.2243da37.js",
+    "file": "static/js/main.3bc257bc.js",
     "names": [
         "deselectCurrent",
         "require",
         "clipboardToIE11Formatting",
         "module",
         "exports",
         "text",
@@ -9622,16 +9622,16 @@
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport { Data } from '../data.js';\nimport { Table } from '../table.js';\nimport { MAGIC } from './message.js';\nimport { Vector } from '../vector.js';\nimport { DataType, TypeMap } from '../type.js';\nimport { Schema, Field } from '../schema.js';\nimport { Message } from './metadata/message.js';\nimport * as metadata from './metadata/message.js';\nimport { FileBlock, Footer } from './metadata/file.js';\nimport { MessageHeader, MetadataVersion } from '../enum.js';\nimport { compareSchemas } from '../visitor/typecomparator.js';\nimport { WritableSink, AsyncByteQueue } from '../io/stream.js';\nimport { VectorAssembler } from '../visitor/vectorassembler.js';\nimport { JSONTypeAssembler } from '../visitor/jsontypeassembler.js';\nimport { JSONVectorAssembler } from '../visitor/jsonvectorassembler.js';\nimport { ArrayBufferViewInput, toUint8Array } from '../util/buffer.js';\nimport { RecordBatch, _InternalEmptyPlaceholderRecordBatch } from '../recordbatch.js';\nimport { Writable, ReadableInterop, ReadableDOMStreamOptions } from '../io/interfaces.js';\nimport { isPromise, isAsyncIterable, isWritableDOMStream, isWritableNodeStream, isIterable, isObject } from '../util/compat.js';\n\nexport interface RecordBatchStreamWriterOptions {\n    /**\n     *\n     */\n    autoDestroy?: boolean;\n    /**\n     * A flag indicating whether the RecordBatchWriter should construct pre-0.15.0\n     * encapsulated IPC Messages, which reserves  4 bytes for the Message metadata\n     * length instead of 8.\n     * @see https://issues.apache.org/jira/browse/ARROW-6313\n     */\n    writeLegacyIpcFormat?: boolean;\n}\n\nexport class RecordBatchWriter<T extends TypeMap = any> extends ReadableInterop<Uint8Array> implements Writable<RecordBatch<T>> {\n\n    /** @nocollapse */\n    // @ts-ignore\n    public static throughNode(options?: import('stream').DuplexOptions & { autoDestroy: boolean }): import('stream').Duplex {\n        throw new Error(`\"throughNode\" not available in this environment`);\n    }\n    /** @nocollapse */\n    public static throughDOM<T extends TypeMap>(\n        // @ts-ignore\n        writableStrategy?: QueuingStrategy<RecordBatch<T>> & { autoDestroy: boolean },\n        // @ts-ignore\n        readableStrategy?: { highWaterMark?: number; size?: any }\n    ): { writable: WritableStream<Table<T> | RecordBatch<T>>; readable: ReadableStream<Uint8Array> } {\n        throw new Error(`\"throughDOM\" not available in this environment`);\n    }\n\n    constructor(options?: RecordBatchStreamWriterOptions) {\n        super();\n        isObject(options) || (options = { autoDestroy: true, writeLegacyIpcFormat: false });\n        this._autoDestroy = (typeof options.autoDestroy === 'boolean') ? options.autoDestroy : true;\n        this._writeLegacyIpcFormat = (typeof options.writeLegacyIpcFormat === 'boolean') ? options.writeLegacyIpcFormat : false;\n    }\n\n    protected _position = 0;\n    protected _started = false;\n    protected _autoDestroy: boolean;\n    protected _writeLegacyIpcFormat: boolean;\n    // @ts-ignore\n    protected _sink = new AsyncByteQueue();\n    protected _schema: Schema | null = null;\n    protected _dictionaryBlocks: FileBlock[] = [];\n    protected _recordBatchBlocks: FileBlock[] = [];\n    protected _dictionaryDeltaOffsets = new Map<number, number>();\n\n    public toString(sync: true): string;\n    public toString(sync?: false): Promise<string>;\n    public toString(sync: any = false) {\n        return this._sink.toString(sync) as Promise<string> | string;\n    }\n    public toUint8Array(sync: true): Uint8Array;\n    public toUint8Array(sync?: false): Promise<Uint8Array>;\n    public toUint8Array(sync: any = false) {\n        return this._sink.toUint8Array(sync) as Promise<Uint8Array> | Uint8Array;\n    }\n\n    public writeAll(input: Table<T> | Iterable<RecordBatch<T>>): this;\n    public writeAll(input: AsyncIterable<RecordBatch<T>>): Promise<this>;\n    public writeAll(input: PromiseLike<AsyncIterable<RecordBatch<T>>>): Promise<this>;\n    public writeAll(input: PromiseLike<Table<T> | Iterable<RecordBatch<T>>>): Promise<this>;\n    public writeAll(input: PromiseLike<any> | Table<T> | Iterable<RecordBatch<T>> | AsyncIterable<RecordBatch<T>>) {\n        if (isPromise<any>(input)) {\n            return input.then((x) => this.writeAll(x));\n        } else if (isAsyncIterable<RecordBatch<T>>(input)) {\n            return writeAllAsync(this, input);\n        }\n        return writeAll(this, <any>input);\n    }\n\n    public get closed() { return this._sink.closed; }\n    public [Symbol.asyncIterator]() { return this._sink[Symbol.asyncIterator](); }\n    public toDOMStream(options?: ReadableDOMStreamOptions) { return this._sink.toDOMStream(options); }\n    public toNodeStream(options?: import('stream').ReadableOptions) { return this._sink.toNodeStream(options); }\n\n    public close() {\n        return this.reset()._sink.close();\n    }\n    public abort(reason?: any) {\n        return this.reset()._sink.abort(reason);\n    }\n    public finish() {\n        this._autoDestroy ? this.close() : this.reset(this._sink, this._schema);\n        return this;\n    }\n    public reset(sink: WritableSink<ArrayBufferViewInput> = this._sink, schema: Schema<T> | null = null) {\n        if ((sink === this._sink) || (sink instanceof AsyncByteQueue)) {\n            this._sink = sink as AsyncByteQueue;\n        } else {\n            this._sink = new AsyncByteQueue();\n            if (sink && isWritableDOMStream(sink)) {\n                this.toDOMStream({ type: 'bytes' }).pipeTo(sink);\n            } else if (sink && isWritableNodeStream(sink)) {\n                this.toNodeStream({ objectMode: false }).pipe(sink);\n            }\n        }\n\n        if (this._started && this._schema) {\n            this._writeFooter(this._schema);\n        }\n\n        this._started = false;\n        this._dictionaryBlocks = [];\n        this._recordBatchBlocks = [];\n        this._dictionaryDeltaOffsets = new Map();\n\n        if (!schema || !(compareSchemas(schema, this._schema))) {\n            if (schema == null) {\n                this._position = 0;\n                this._schema = null;\n            } else {\n                this._started = true;\n                this._schema = schema;\n                this._writeSchema(schema);\n            }\n        }\n\n        return this;\n    }\n\n    public write(payload?: Table<T> | RecordBatch<T> | Iterable<RecordBatch<T>> | null) {\n        let schema: Schema<T> | null = null;\n\n        if (!this._sink) {\n            throw new Error(`RecordBatchWriter is closed`);\n        } else if (payload == null) {\n            return this.finish() && undefined;\n        } else if (payload instanceof Table && !(schema = payload.schema)) {\n            return this.finish() && undefined;\n        } else if (payload instanceof RecordBatch && !(schema = payload.schema)) {\n            return this.finish() && undefined;\n        }\n\n        if (schema && !compareSchemas(schema, this._schema)) {\n            if (this._started && this._autoDestroy) {\n                return this.close();\n            }\n            this.reset(this._sink, schema);\n        }\n\n        if (payload instanceof RecordBatch) {\n            if (!(payload instanceof _InternalEmptyPlaceholderRecordBatch)) {\n                this._writeRecordBatch(payload);\n            }\n        } else if (payload instanceof Table) {\n            this.writeAll(payload.batches);\n        } else if (isIterable(payload)) {\n            this.writeAll(payload);\n        }\n    }\n\n    protected _writeMessage<T extends MessageHeader>(message: Message<T>, alignment = 8) {\n        const a = alignment - 1;\n        const buffer = Message.encode(message);\n        const flatbufferSize = buffer.byteLength;\n        const prefixSize = !this._writeLegacyIpcFormat ? 8 : 4;\n        const alignedSize = (flatbufferSize + prefixSize + a) & ~a;\n        const nPaddingBytes = alignedSize - flatbufferSize - prefixSize;\n\n        if (message.headerType === MessageHeader.RecordBatch) {\n            this._recordBatchBlocks.push(new FileBlock(alignedSize, message.bodyLength, this._position));\n        } else if (message.headerType === MessageHeader.DictionaryBatch) {\n            this._dictionaryBlocks.push(new FileBlock(alignedSize, message.bodyLength, this._position));\n        }\n\n        // If not in legacy pre-0.15.0 mode, write the stream continuation indicator\n        if (!this._writeLegacyIpcFormat) {\n            this._write(Int32Array.of(-1));\n        }\n        // Write the flatbuffer size prefix including padding\n        this._write(Int32Array.of(alignedSize - prefixSize));\n        // Write the flatbuffer\n        if (flatbufferSize > 0) { this._write(buffer); }\n        // Write any padding\n        return this._writePadding(nPaddingBytes);\n    }\n\n    protected _write(chunk: ArrayBufferViewInput) {\n        if (this._started) {\n            const buffer = toUint8Array(chunk);\n            if (buffer && buffer.byteLength > 0) {\n                this._sink.write(buffer);\n                this._position += buffer.byteLength;\n            }\n        }\n        return this;\n    }\n\n    protected _writeSchema(schema: Schema<T>) {\n        return this._writeMessage(Message.from(schema));\n    }\n\n    // @ts-ignore\n    protected _writeFooter(schema: Schema<T>) {\n        // eos bytes\n        return this._writeLegacyIpcFormat\n            ? this._write(Int32Array.of(0))\n            : this._write(Int32Array.of(-1, 0));\n    }\n\n    protected _writeMagic() {\n        return this._write(MAGIC);\n    }\n\n    protected _writePadding(nBytes: number) {\n        return nBytes > 0 ? this._write(new Uint8Array(nBytes)) : this;\n    }\n\n    protected _writeRecordBatch(batch: RecordBatch<T>) {\n        const { byteLength, nodes, bufferRegions, buffers } = VectorAssembler.assemble(batch);\n        const recordBatch = new metadata.RecordBatch(batch.numRows, nodes, bufferRegions);\n        const message = Message.from(recordBatch, byteLength);\n        return this\n            ._writeDictionaries(batch)\n            ._writeMessage(message)\n            ._writeBodyBuffers(buffers);\n    }\n\n    protected _writeDictionaryBatch(dictionary: Data, id: number, isDelta = false) {\n        this._dictionaryDeltaOffsets.set(id, dictionary.length + (this._dictionaryDeltaOffsets.get(id) || 0));\n        const { byteLength, nodes, bufferRegions, buffers } = VectorAssembler.assemble(new Vector([dictionary]));\n        const recordBatch = new metadata.RecordBatch(dictionary.length, nodes, bufferRegions);\n        const dictionaryBatch = new metadata.DictionaryBatch(recordBatch, id, isDelta);\n        const message = Message.from(dictionaryBatch, byteLength);\n        return this\n            ._writeMessage(message)\n            ._writeBodyBuffers(buffers);\n    }\n\n    protected _writeBodyBuffers(buffers: ArrayBufferView[]) {\n        let buffer: ArrayBufferView;\n        let size: number, padding: number;\n        for (let i = -1, n = buffers.length; ++i < n;) {\n            if ((buffer = buffers[i]) && (size = buffer.byteLength) > 0) {\n                this._write(buffer);\n                if ((padding = ((size + 7) & ~7) - size) > 0) {\n                    this._writePadding(padding);\n                }\n            }\n        }\n        return this;\n    }\n\n    protected _writeDictionaries(batch: RecordBatch<T>) {\n        for (let [id, dictionary] of batch.dictionaries) {\n            let offset = this._dictionaryDeltaOffsets.get(id) || 0;\n            if (offset === 0 || (dictionary = dictionary?.slice(offset)).length > 0) {\n                for (const data of dictionary.data) {\n                    this._writeDictionaryBatch(data, id, offset > 0);\n                    offset += data.length;\n                }\n            }\n        }\n        return this;\n    }\n}\n\n/** @ignore */\nexport class RecordBatchStreamWriter<T extends TypeMap = any> extends RecordBatchWriter<T> {\n    public static writeAll<T extends TypeMap = any>(input: Table<T> | Iterable<RecordBatch<T>>, options?: RecordBatchStreamWriterOptions): RecordBatchStreamWriter<T>;\n    public static writeAll<T extends TypeMap = any>(input: AsyncIterable<RecordBatch<T>>, options?: RecordBatchStreamWriterOptions): Promise<RecordBatchStreamWriter<T>>;\n    public static writeAll<T extends TypeMap = any>(input: PromiseLike<AsyncIterable<RecordBatch<T>>>, options?: RecordBatchStreamWriterOptions): Promise<RecordBatchStreamWriter<T>>;\n    public static writeAll<T extends TypeMap = any>(input: PromiseLike<Table<T> | Iterable<RecordBatch<T>>>, options?: RecordBatchStreamWriterOptions): Promise<RecordBatchStreamWriter<T>>;\n    /** @nocollapse */\n    public static writeAll<T extends TypeMap = any>(input: any, options?: RecordBatchStreamWriterOptions) {\n        const writer = new RecordBatchStreamWriter<T>(options);\n        if (isPromise<any>(input)) {\n            return input.then((x) => writer.writeAll(x));\n        } else if (isAsyncIterable<RecordBatch<T>>(input)) {\n            return writeAllAsync(writer, input);\n        }\n        return writeAll(writer, input);\n    }\n}\n\n/** @ignore */\nexport class RecordBatchFileWriter<T extends TypeMap = any> extends RecordBatchWriter<T> {\n    public static writeAll<T extends TypeMap = any>(input: Table<T> | Iterable<RecordBatch<T>>): RecordBatchFileWriter<T>;\n    public static writeAll<T extends TypeMap = any>(input: AsyncIterable<RecordBatch<T>>): Promise<RecordBatchFileWriter<T>>;\n    public static writeAll<T extends TypeMap = any>(input: PromiseLike<AsyncIterable<RecordBatch<T>>>): Promise<RecordBatchFileWriter<T>>;\n    public static writeAll<T extends TypeMap = any>(input: PromiseLike<Table<T> | Iterable<RecordBatch<T>>>): Promise<RecordBatchFileWriter<T>>;\n    /** @nocollapse */\n    public static writeAll<T extends TypeMap = any>(input: any) {\n        const writer = new RecordBatchFileWriter<T>();\n        if (isPromise<any>(input)) {\n            return input.then((x) => writer.writeAll(x));\n        } else if (isAsyncIterable<RecordBatch<T>>(input)) {\n            return writeAllAsync(writer, input);\n        }\n        return writeAll(writer, input);\n    }\n\n    constructor() {\n        super();\n        this._autoDestroy = true;\n    }\n\n    // @ts-ignore\n    protected _writeSchema(schema: Schema<T>) {\n        return this._writeMagic()._writePadding(2);\n    }\n\n    protected _writeFooter(schema: Schema<T>) {\n        const buffer = Footer.encode(new Footer(\n            schema, MetadataVersion.V4,\n            this._recordBatchBlocks, this._dictionaryBlocks\n        ));\n        return super\n            ._writeFooter(schema) // EOS bytes for sequential readers\n            ._write(buffer) // Write the flatbuffer\n            ._write(Int32Array.of(buffer.byteLength)) // then the footer size suffix\n            ._writeMagic(); // then the magic suffix\n    }\n}\n\n/** @ignore */\nexport class RecordBatchJSONWriter<T extends TypeMap = any> extends RecordBatchWriter<T> {\n\n    public static writeAll<T extends TypeMap = any>(this: typeof RecordBatchWriter, input: Table<T> | Iterable<RecordBatch<T>>): RecordBatchJSONWriter<T>;\n    // @ts-ignore\n    public static writeAll<T extends TypeMap = any>(this: typeof RecordBatchWriter, input: AsyncIterable<RecordBatch<T>>): Promise<RecordBatchJSONWriter<T>>;\n    public static writeAll<T extends TypeMap = any>(this: typeof RecordBatchWriter, input: PromiseLike<AsyncIterable<RecordBatch<T>>>): Promise<RecordBatchJSONWriter<T>>;\n    public static writeAll<T extends TypeMap = any>(this: typeof RecordBatchWriter, input: PromiseLike<Table<T> | Iterable<RecordBatch<T>>>): Promise<RecordBatchJSONWriter<T>>;\n    /** @nocollapse */\n    public static writeAll<T extends TypeMap = any>(this: typeof RecordBatchWriter, input: any) {\n        return new RecordBatchJSONWriter<T>().writeAll(input as any);\n    }\n\n    private _recordBatches: RecordBatch[];\n    private _dictionaries: RecordBatch[];\n\n    constructor() {\n        super();\n        this._autoDestroy = true;\n        this._recordBatches = [];\n        this._dictionaries = [];\n    }\n\n    protected _writeMessage() { return this; }\n    // @ts-ignore\n    protected _writeFooter(schema: Schema<T>) { return this; }\n    protected _writeSchema(schema: Schema<T>) {\n        return this._write(`{\\n  \"schema\": ${JSON.stringify({ fields: schema.fields.map(field => fieldToJSON(field)) }, null, 2)}`);\n    }\n    protected _writeDictionaries(batch: RecordBatch<T>) {\n        if (batch.dictionaries.size > 0) {\n            this._dictionaries.push(batch);\n        }\n        return this;\n    }\n    protected _writeDictionaryBatch(dictionary: Data, id: number, isDelta = false) {\n        this._dictionaryDeltaOffsets.set(id, dictionary.length + (this._dictionaryDeltaOffsets.get(id) || 0));\n        this._write(this._dictionaryBlocks.length === 0 ? `    ` : `,\\n    `);\n        this._write(`${dictionaryBatchToJSON(dictionary, id, isDelta)}`);\n        this._dictionaryBlocks.push(new FileBlock(0, 0, 0));\n        return this;\n    }\n    protected _writeRecordBatch(batch: RecordBatch<T>) {\n        this._writeDictionaries(batch);\n        this._recordBatches.push(batch);\n        return this;\n    }\n    public close() {\n\n        if (this._dictionaries.length > 0) {\n            this._write(`,\\n  \"dictionaries\": [\\n`);\n            for (const batch of this._dictionaries) {\n                super._writeDictionaries(batch);\n            }\n            this._write(`\\n  ]`);\n        }\n\n        if (this._recordBatches.length > 0) {\n            for (let i = -1, n = this._recordBatches.length; ++i < n;) {\n                this._write(i === 0 ? `,\\n  \"batches\": [\\n    ` : `,\\n    `);\n                this._write(`${recordBatchToJSON(this._recordBatches[i])}`);\n                this._recordBatchBlocks.push(new FileBlock(0, 0, 0));\n            }\n            this._write(`\\n  ]`);\n        }\n\n        if (this._schema) {\n            this._write(`\\n}`);\n        }\n\n        this._dictionaries = [];\n        this._recordBatches = [];\n\n        return super.close();\n    }\n}\n\n/** @ignore */\nfunction writeAll<T extends TypeMap = any>(writer: RecordBatchWriter<T>, input: Table<T> | Iterable<RecordBatch<T>>) {\n    let chunks = input as Iterable<RecordBatch<T>>;\n    if (input instanceof Table) {\n        chunks = input.batches;\n        writer.reset(undefined, input.schema);\n    }\n    for (const batch of chunks) {\n        writer.write(batch);\n    }\n    return writer.finish();\n}\n\n/** @ignore */\nasync function writeAllAsync<T extends TypeMap = any>(writer: RecordBatchWriter<T>, batches: AsyncIterable<RecordBatch<T>>) {\n    for await (const batch of batches) {\n        writer.write(batch);\n    }\n    return writer.finish();\n}\n\n/** @ignore */\nfunction fieldToJSON({ name, type, nullable }: Field): Record<string, unknown> {\n    const assembler = new JSONTypeAssembler();\n    return {\n        'name': name, 'nullable': nullable,\n        'type': assembler.visit(type),\n        'children': (type.children || []).map((field: any) => fieldToJSON(field)),\n        'dictionary': !DataType.isDictionary(type) ? undefined : {\n            'id': type.id,\n            'isOrdered': type.isOrdered,\n            'indexType': assembler.visit(type.indices)\n        }\n    };\n}\n\n/** @ignore */\nfunction dictionaryBatchToJSON(dictionary: Data, id: number, isDelta = false) {\n    const [columns] = JSONVectorAssembler.assemble(new RecordBatch({ [id]: dictionary }));\n    return JSON.stringify({\n        'id': id,\n        'isDelta': isDelta,\n        'data': {\n            'count': dictionary.length,\n            'columns': columns\n        }\n    }, null, 2);\n}\n\n/** @ignore */\nfunction recordBatchToJSON(records: RecordBatch) {\n    const [columns] = JSONVectorAssembler.assemble(records);\n    return JSON.stringify({\n        'count': records.numRows,\n        'columns': columns\n    }, null, 2);\n}\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport { Table } from '../table.js';\nimport { TypeMap } from '../type.js';\nimport { isPromise } from '../util/compat.js';\nimport {\n    FromArg0, FromArg1, FromArg2, FromArg3, FromArg4, FromArg5,\n    RecordBatchReader,\n    RecordBatchFileReader, RecordBatchStreamReader,\n    AsyncRecordBatchFileReader, AsyncRecordBatchStreamReader\n} from './reader.js';\nimport { RecordBatchFileWriter, RecordBatchStreamWriter } from './writer.js';\n\ntype RecordBatchReaders<T extends TypeMap = any> = RecordBatchFileReader<T> | RecordBatchStreamReader<T>;\ntype AsyncRecordBatchReaders<T extends TypeMap = any> = AsyncRecordBatchFileReader<T> | AsyncRecordBatchStreamReader<T>;\n\n/**\n * Deserialize the IPC format into a {@link Table}. This function is a\n * convenience wrapper for {@link RecordBatchReader}. Opposite of {@link tableToIPC}.\n */\nexport function tableFromIPC<T extends TypeMap = any>(source: FromArg0 | FromArg2): Table<T>;\nexport function tableFromIPC<T extends TypeMap = any>(source: FromArg1): Promise<Table<T>>;\nexport function tableFromIPC<T extends TypeMap = any>(source: FromArg3 | FromArg4 | FromArg5): Promise<Table<T>>;\nexport function tableFromIPC<T extends TypeMap = any>(source: RecordBatchReaders<T>): Table<T>;\nexport function tableFromIPC<T extends TypeMap = any>(source: AsyncRecordBatchReaders<T>): Promise<Table<T>>;\nexport function tableFromIPC<T extends TypeMap = any>(source: RecordBatchReader<T>): Table<T> | Promise<Table<T>>;\nexport function tableFromIPC<T extends TypeMap = any>(input: any): Table<T> | Promise<Table<T>> {\n    const reader = RecordBatchReader.from<T>(input) as RecordBatchReader<T> | Promise<RecordBatchReader<T>>;\n    if (isPromise<RecordBatchReader<T>>(reader)) {\n        return reader.then((reader) => tableFromIPC(reader)) as Promise<Table<T>>;\n    }\n    if (reader.isAsync()) {\n        return (reader as AsyncRecordBatchReaders<T>).readAll().then((xs) => new Table(xs));\n    }\n    return new Table((reader as RecordBatchReaders<T>).readAll());\n}\n\n/**\n * Serialize a {@link Table} to the IPC format. This function is a convenience\n * wrapper for {@link RecordBatchStreamWriter} and {@link RecordBatchFileWriter}.\n * Opposite of {@link tableFromIPC}.\n *\n * @param table The Table to serialize.\n * @param type Whether to serialize the Table as a file or a stream.\n */\nexport function tableToIPC<T extends TypeMap = any>(table: Table, type: 'file' | 'stream' = 'stream'): Uint8Array {\n    return (type === 'stream' ? RecordBatchStreamWriter : RecordBatchFileWriter)\n        .writeAll<T>(table)\n        .toUint8Array(true);\n}\n",
         "/**\n * Copyright (c) Streamlit Inc. (2018-2022) Snowflake Inc. (2022)\n *\n * Licensed under the Apache License, Version 2.0 (the \"License\");\n * you may not use this file except in compliance with the License.\n * You may obtain a copy of the License at\n *\n *     http://www.apache.org/licenses/LICENSE-2.0\n *\n * Unless required by applicable law or agreed to in writing, software\n * distributed under the License is distributed on an \"AS IS\" BASIS,\n * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n * See the License for the specific language governing permissions and\n * limitations under the License.\n */\nimport { tableToIPC, tableFromIPC, Type } from \"apache-arrow\";\nvar ArrowTable = /** @class */ (function () {\n    function ArrowTable(dataBuffer, indexBuffer, columnsBuffer, styler) {\n        var _this = this;\n        this.getCell = function (rowIndex, columnIndex) {\n            var isBlankCell = rowIndex < _this.headerRows && columnIndex < _this.headerColumns;\n            var isIndexCell = rowIndex >= _this.headerRows && columnIndex < _this.headerColumns;\n            var isColumnsCell = rowIndex < _this.headerRows && columnIndex >= _this.headerColumns;\n            if (isBlankCell) {\n                var classNames = [\"blank\"];\n                if (columnIndex > 0) {\n                    classNames.push(\"level\" + rowIndex);\n                }\n                return {\n                    type: \"blank\",\n                    classNames: classNames.join(\" \"),\n                    content: \"\"\n                };\n            }\n            else if (isColumnsCell) {\n                var dataColumnIndex = columnIndex - _this.headerColumns;\n                var classNames = [\n                    \"col_heading\",\n                    \"level\" + rowIndex,\n                    \"col\" + dataColumnIndex\n                ];\n                return {\n                    type: \"columns\",\n                    classNames: classNames.join(\" \"),\n                    content: _this.getContent(_this.columnsTable, dataColumnIndex, rowIndex)\n                };\n            }\n            else if (isIndexCell) {\n                var dataRowIndex = rowIndex - _this.headerRows;\n                var classNames = [\n                    \"row_heading\",\n                    \"level\" + columnIndex,\n                    \"row\" + dataRowIndex\n                ];\n                return {\n                    type: \"index\",\n                    id: \"T_\".concat(_this.uuid, \"level\").concat(columnIndex, \"_row\").concat(dataRowIndex),\n                    classNames: classNames.join(\" \"),\n                    content: _this.getContent(_this.indexTable, dataRowIndex, columnIndex)\n                };\n            }\n            else {\n                var dataRowIndex = rowIndex - _this.headerRows;\n                var dataColumnIndex = columnIndex - _this.headerColumns;\n                var classNames = [\n                    \"data\",\n                    \"row\" + dataRowIndex,\n                    \"col\" + dataColumnIndex\n                ];\n                var content = _this.styler\n                    ? _this.getContent(_this.styler.displayValuesTable, dataRowIndex, dataColumnIndex)\n                    : _this.getContent(_this.dataTable, dataRowIndex, dataColumnIndex);\n                return {\n                    type: \"data\",\n                    id: \"T_\".concat(_this.uuid, \"row\").concat(dataRowIndex, \"_col\").concat(dataColumnIndex),\n                    classNames: classNames.join(\" \"),\n                    content: content\n                };\n            }\n        };\n        this.getContent = function (table, rowIndex, columnIndex) {\n            var column = table.getChildAt(columnIndex);\n            if (column === null) {\n                return \"\";\n            }\n            var columnTypeId = _this.getColumnTypeId(table, columnIndex);\n            switch (columnTypeId) {\n                case Type.Timestamp: {\n                    return _this.nanosToDate(column.get(rowIndex));\n                }\n                default: {\n                    return column.get(rowIndex);\n                }\n            }\n        };\n        this.dataTable = tableFromIPC(dataBuffer);\n        this.indexTable = tableFromIPC(indexBuffer);\n        this.columnsTable = tableFromIPC(columnsBuffer);\n        this.styler = styler\n            ? {\n                caption: styler.caption,\n                displayValuesTable: tableFromIPC(styler.displayValues),\n                styles: styler.styles,\n                uuid: styler.uuid\n            }\n            : undefined;\n    }\n    Object.defineProperty(ArrowTable.prototype, \"rows\", {\n        get: function () {\n            return this.indexTable.numRows + this.columnsTable.numCols;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"columns\", {\n        get: function () {\n            return this.indexTable.numCols + this.columnsTable.numRows;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"headerRows\", {\n        get: function () {\n            return this.rows - this.dataRows;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"headerColumns\", {\n        get: function () {\n            return this.columns - this.dataColumns;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"dataRows\", {\n        get: function () {\n            return this.dataTable.numRows;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"dataColumns\", {\n        get: function () {\n            return this.dataTable.numCols;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"uuid\", {\n        get: function () {\n            return this.styler && this.styler.uuid;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"caption\", {\n        get: function () {\n            return this.styler && this.styler.caption;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"styles\", {\n        get: function () {\n            return this.styler && this.styler.styles;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"table\", {\n        get: function () {\n            return this.dataTable;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"index\", {\n        get: function () {\n            return this.indexTable;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    Object.defineProperty(ArrowTable.prototype, \"columnTable\", {\n        get: function () {\n            return this.columnsTable;\n        },\n        enumerable: false,\n        configurable: true\n    });\n    /**\n     * Serialize arrow table.\n     */\n    ArrowTable.prototype.serialize = function () {\n        return {\n            data: tableToIPC(this.dataTable),\n            index: tableToIPC(this.indexTable),\n            columns: tableToIPC(this.columnsTable)\n        };\n    };\n    /**\n     * Returns apache-arrow specific typeId of column.\n     */\n    ArrowTable.prototype.getColumnTypeId = function (table, columnIndex) {\n        return table.schema.fields[columnIndex].type.typeId;\n    };\n    ArrowTable.prototype.nanosToDate = function (nanos) {\n        return new Date(nanos / 1e6);\n    };\n    return ArrowTable;\n}());\nexport { ArrowTable };\n",
         "/**\n * Copyright (c) Streamlit Inc. (2018-2022) Snowflake Inc. (2022)\n *\n * Licensed under the Apache License, Version 2.0 (the \"License\");\n * you may not use this file except in compliance with the License.\n * You may obtain a copy of the License at\n *\n *     http://www.apache.org/licenses/LICENSE-2.0\n *\n * Unless required by applicable law or agreed to in writing, software\n * distributed under the License is distributed on an \"AS IS\" BASIS,\n * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n * See the License for the specific language governing permissions and\n * limitations under the License.\n */\nvar __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\n// Safari doesn't support the EventTarget class, so we use a shim.\nimport { ArrowTable } from \"./ArrowTable\";\n/** Messages from Component -> Streamlit */\nvar ComponentMessageType;\n(function (ComponentMessageType) {\n    // A component sends this message when it's ready to receive messages\n    // from Streamlit. Streamlit won't send any messages until it gets this.\n    // Data: { apiVersion: number }\n    ComponentMessageType[\"COMPONENT_READY\"] = \"streamlit:componentReady\";\n    // The component has a new widget value. Send it back to Streamlit, which\n    // will then re-run the app.\n    // Data: { value: any }\n    ComponentMessageType[\"SET_COMPONENT_VALUE\"] = \"streamlit:setComponentValue\";\n    // The component has a new height for its iframe.\n    // Data: { height: number }\n    ComponentMessageType[\"SET_FRAME_HEIGHT\"] = \"streamlit:setFrameHeight\";\n})(ComponentMessageType || (ComponentMessageType = {}));\n/**\n * Streamlit communication API.\n *\n * Components can send data to Streamlit via the functions defined here,\n * and receive data from Streamlit via the `events` property.\n */\nexport var Streamlit = /** @class */ (function () {\n    function Streamlit() {\n    }\n    /**\n     * The Streamlit component API version we're targeting.\n     * There's currently only 1!\n     */\n    Streamlit.API_VERSION = 1;\n    Streamlit.RENDER_EVENT = \"streamlit:render\";\n    /** Dispatches events received from Streamlit. */\n    Streamlit.events = new EventTarget();\n    Streamlit.registeredMessageListener = false;\n    /**\n     * Tell Streamlit that the component is ready to start receiving data.\n     * Streamlit will defer emitting RENDER events until it receives the\n     * COMPONENT_READY message.\n     */\n    Streamlit.setComponentReady = function () {\n        if (!Streamlit.registeredMessageListener) {\n            // Register for message events if we haven't already\n            window.addEventListener(\"message\", Streamlit.onMessageEvent);\n            Streamlit.registeredMessageListener = true;\n        }\n        Streamlit.sendBackMsg(ComponentMessageType.COMPONENT_READY, {\n            apiVersion: Streamlit.API_VERSION\n        });\n    };\n    /**\n     * Report the component's height to Streamlit.\n     * This should be called every time the component changes its DOM - that is,\n     * when it's first loaded, and any time it updates.\n     */\n    Streamlit.setFrameHeight = function (height) {\n        if (height === undefined) {\n            // `height` is optional. If undefined, it defaults to scrollHeight,\n            // which is the entire height of the element minus its border,\n            // scrollbar, and margin.\n            height = document.body.scrollHeight;\n        }\n        if (height === Streamlit.lastFrameHeight) {\n            // Don't bother updating if our height hasn't changed.\n            return;\n        }\n        Streamlit.lastFrameHeight = height;\n        Streamlit.sendBackMsg(ComponentMessageType.SET_FRAME_HEIGHT, { height: height });\n    };\n    /**\n     * Set the component's value. This value will be returned to the Python\n     * script, and the script will be re-run.\n     *\n     * For example:\n     *\n     * JavaScript:\n     * Streamlit.setComponentValue(\"ahoy!\")\n     *\n     * Python:\n     * value = st.my_component(...)\n     * st.write(value) # -> \"ahoy!\"\n     *\n     * The value must be an ArrowTable, a typed array, an ArrayBuffer, or be\n     * serializable to JSON.\n     */\n    Streamlit.setComponentValue = function (value) {\n        var dataType;\n        if (value instanceof ArrowTable) {\n            dataType = \"dataframe\";\n            value = value.serialize();\n        }\n        else if (isTypedArray(value)) {\n            // All typed arrays get sent as Uint8Array, because that's what our\n            // protobuf library uses for the \"bytes\" field type.\n            dataType = \"bytes\";\n            value = new Uint8Array(value.buffer);\n        }\n        else if (value instanceof ArrayBuffer) {\n            dataType = \"bytes\";\n            value = new Uint8Array(value);\n        }\n        else {\n            dataType = \"json\";\n        }\n        Streamlit.sendBackMsg(ComponentMessageType.SET_COMPONENT_VALUE, {\n            value: value,\n            dataType: dataType\n        });\n    };\n    /** Receive a ForwardMsg from the Streamlit app */\n    Streamlit.onMessageEvent = function (event) {\n        var type = event.data[\"type\"];\n        switch (type) {\n            case Streamlit.RENDER_EVENT:\n                Streamlit.onRenderMessage(event.data);\n                break;\n        }\n    };\n    /**\n     * Handle an untyped Streamlit render event and redispatch it as a\n     * StreamlitRenderEvent.\n     */\n    Streamlit.onRenderMessage = function (data) {\n        var args = data[\"args\"];\n        if (args == null) {\n            console.error(\"Got null args in onRenderMessage. This should never happen\");\n            args = {};\n        }\n        // Parse our dataframe arguments with arrow, and merge them into our args dict\n        var dataframeArgs = data[\"dfs\"] && data[\"dfs\"].length > 0\n            ? Streamlit.argsDataframeToObject(data[\"dfs\"])\n            : {};\n        args = __assign(__assign({}, args), dataframeArgs);\n        var disabled = Boolean(data[\"disabled\"]);\n        var theme = data[\"theme\"];\n        if (theme) {\n            _injectTheme(theme);\n        }\n        // Dispatch a render event!\n        var eventData = { disabled: disabled, args: args, theme: theme };\n        var event = new CustomEvent(Streamlit.RENDER_EVENT, {\n            detail: eventData\n        });\n        Streamlit.events.dispatchEvent(event);\n    };\n    Streamlit.argsDataframeToObject = function (argsDataframe) {\n        var argsDataframeArrow = argsDataframe.map(function (_a) {\n            var key = _a.key, value = _a.value;\n            return [key, Streamlit.toArrowTable(value)];\n        });\n        return Object.fromEntries(argsDataframeArrow);\n    };\n    Streamlit.toArrowTable = function (df) {\n        var _a;\n        var data = (_a = df.data, _a.data), index = _a.index, columns = _a.columns, styler = _a.styler;\n        return new ArrowTable(data, index, columns, styler);\n    };\n    /** Post a message to the Streamlit app. */\n    Streamlit.sendBackMsg = function (type, data) {\n        window.parent.postMessage(__assign({ isStreamlitMessage: true, type: type }, data), \"*\");\n    };\n    return Streamlit;\n}());\nvar _injectTheme = function (theme) {\n    var style = document.createElement(\"style\");\n    document.head.appendChild(style);\n    style.innerHTML = \"\\n    :root {\\n      --primary-color: \".concat(theme.primaryColor, \";\\n      --background-color: \").concat(theme.backgroundColor, \";\\n      --secondary-background-color: \").concat(theme.secondaryBackgroundColor, \";\\n      --text-color: \").concat(theme.textColor, \";\\n      --font: \").concat(theme.font, \";\\n    }\\n\\n    body {\\n      background-color: var(--background-color);\\n      color: var(--text-color);\\n    }\\n  \");\n};\n/** True if the value is a TypedArray. */\nfunction isTypedArray(value) {\n    var isBigIntArray = false;\n    try {\n        isBigIntArray =\n            value instanceof BigInt64Array || value instanceof BigUint64Array;\n    }\n    catch (e) {\n        // Ignore cause Safari does not support this\n        // https://caniuse.com/mdn-javascript_builtins_bigint64array\n    }\n    return (value instanceof Int8Array ||\n        value instanceof Uint8Array ||\n        value instanceof Uint8ClampedArray ||\n        value instanceof Int16Array ||\n        value instanceof Uint16Array ||\n        value instanceof Int32Array ||\n        value instanceof Uint32Array ||\n        value instanceof Float32Array ||\n        value instanceof Float64Array ||\n        isBigIntArray);\n}\n",
         "/**\n * Copyright (c) Streamlit Inc. (2018-2022) Snowflake Inc. (2022)\n *\n * Licensed under the Apache License, Version 2.0 (the \"License\");\n * you may not use this file except in compliance with the License.\n * You may obtain a copy of the License at\n *\n *     http://www.apache.org/licenses/LICENSE-2.0\n *\n * Unless required by applicable law or agreed to in writing, software\n * distributed under the License is distributed on an \"AS IS\" BASIS,\n * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n * See the License for the specific language governing permissions and\n * limitations under the License.\n */\nvar __extends = (this && this.__extends) || (function () {\n    var extendStatics = function (d, b) {\n        extendStatics = Object.setPrototypeOf ||\n            ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\n            function (d, b) { for (var p in b) if (Object.prototype.hasOwnProperty.call(b, p)) d[p] = b[p]; };\n        return extendStatics(d, b);\n    };\n    return function (d, b) {\n        if (typeof b !== \"function\" && b !== null)\n            throw new TypeError(\"Class extends value \" + String(b) + \" is not a constructor or null\");\n        extendStatics(d, b);\n        function __() { this.constructor = d; }\n        d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\n    };\n})();\nimport hoistNonReactStatics from \"hoist-non-react-statics\";\nimport React from \"react\";\nimport { Streamlit } from \"./streamlit\";\n/**\n * Optional Streamlit React-based component base class.\n *\n * You are not required to extend this base class to create a Streamlit\n * component. If you decide not to extend it, you should implement the\n * `componentDidMount` and `componentDidUpdate` functions in your own class,\n * so that your plugin properly resizes.\n */\nvar StreamlitComponentBase = /** @class */ (function (_super) {\n    __extends(StreamlitComponentBase, _super);\n    function StreamlitComponentBase() {\n        return _super !== null && _super.apply(this, arguments) || this;\n    }\n    StreamlitComponentBase.prototype.componentDidMount = function () {\n        // After we're rendered for the first time, tell Streamlit that our height\n        // has changed.\n        Streamlit.setFrameHeight();\n    };\n    StreamlitComponentBase.prototype.componentDidUpdate = function () {\n        // After we're updated, tell Streamlit that our height may have changed.\n        Streamlit.setFrameHeight();\n    };\n    return StreamlitComponentBase;\n}(React.PureComponent));\nexport { StreamlitComponentBase };\n/**\n * Wrapper for React-based Streamlit components.\n *\n * Bootstraps the communication interface between Streamlit and the component.\n */\nexport function withStreamlitConnection(WrappedComponent) {\n    var ComponentWrapper = /** @class */ (function (_super) {\n        __extends(ComponentWrapper, _super);\n        function ComponentWrapper(props) {\n            var _this = _super.call(this, props) || this;\n            _this.componentDidMount = function () {\n                // Set up event listeners, and signal to Streamlit that we're ready.\n                // We won't render the component until we receive the first RENDER_EVENT.\n                Streamlit.events.addEventListener(Streamlit.RENDER_EVENT, _this.onRenderEvent);\n                Streamlit.setComponentReady();\n            };\n            _this.componentDidUpdate = function () {\n                // If our child threw an error, we display it in render(). In this\n                // case, the child won't be mounted and therefore won't call\n                // `setFrameHeight` on its own. We do it here so that the rendered\n                // error will be visible.\n                if (_this.state.componentError != null) {\n                    Streamlit.setFrameHeight();\n                }\n            };\n            _this.componentWillUnmount = function () {\n                Streamlit.events.removeEventListener(Streamlit.RENDER_EVENT, _this.onRenderEvent);\n            };\n            /**\n             * Streamlit is telling this component to redraw.\n             * We save the render data in State, so that it can be passed to the\n             * component in our own render() function.\n             */\n            _this.onRenderEvent = function (event) {\n                // Update our state with the newest render data\n                _this.setState({ renderData: event.detail });\n            };\n            _this.state = {\n                renderData: undefined,\n                componentError: undefined\n            };\n            return _this;\n        }\n        ComponentWrapper.prototype.render = function () {\n            // If our wrapped component threw an error, display it.\n            if (this.state.componentError != null) {\n                return (React.createElement(\"div\", null,\n                    React.createElement(\"h1\", null, \"Component Error\"),\n                    React.createElement(\"span\", null, this.state.componentError.message)));\n            }\n            // Don't render until we've gotten our first RENDER_EVENT from Streamlit.\n            if (this.state.renderData == null) {\n                return null;\n            }\n            return (React.createElement(WrappedComponent, { width: window.innerWidth, disabled: this.state.renderData.disabled, args: this.state.renderData.args, theme: this.state.renderData.theme }));\n        };\n        /**\n         * Error boundary function. This will be called if our wrapped\n         * component throws an error. We store the caught error in our state,\n         * and display it in the next render().\n         */\n        ComponentWrapper.getDerivedStateFromError = function (error) {\n            return { componentError: error };\n        };\n        return ComponentWrapper;\n    }(React.PureComponent));\n    return hoistNonReactStatics(ComponentWrapper, WrappedComponent);\n}\n",
         "// This icon file is generated automatically.\nvar CloseOutlined = { \"icon\": { \"tag\": \"svg\", \"attrs\": { \"fill-rule\": \"evenodd\", \"viewBox\": \"64 64 896 896\", \"focusable\": \"false\" }, \"children\": [{ \"tag\": \"path\", \"attrs\": { \"d\": \"M799.86 166.31c.02 0 .04.02.08.06l57.69 57.7c.04.03.05.05.06.08a.12.12 0 010 .06c0 .03-.02.05-.06.09L569.93 512l287.7 287.7c.04.04.05.06.06.09a.12.12 0 010 .07c0 .02-.02.04-.06.08l-57.7 57.69c-.03.04-.05.05-.07.06a.12.12 0 01-.07 0c-.03 0-.05-.02-.09-.06L512 569.93l-287.7 287.7c-.04.04-.06.05-.09.06a.12.12 0 01-.07 0c-.02 0-.04-.02-.08-.06l-57.69-57.7c-.04-.03-.05-.05-.06-.07a.12.12 0 010-.07c0-.03.02-.05.06-.09L454.07 512l-287.7-287.7c-.04-.04-.05-.06-.06-.09a.12.12 0 010-.07c0-.02.02-.04.06-.08l57.7-57.69c.03-.04.05-.05.07-.06a.12.12 0 01.07 0c.03 0 .05.02.09.06L512 454.07l287.7-287.7c.04-.04.06-.05.09-.06a.12.12 0 01.07 0z\" } }] }, \"name\": \"close\", \"theme\": \"outlined\" };\nexport default CloseOutlined;\n",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\n// GENERATE BY ./scripts/generate.ts\n// DON NOT EDIT IT MANUALLY\n\nimport * as React from 'react';\nimport CloseOutlinedSvg from \"@ant-design/icons-svg/es/asn/CloseOutlined\";\nimport AntdIcon from \"../components/AntdIcon\";\nvar CloseOutlined = function CloseOutlined(props, ref) {\n  return /*#__PURE__*/React.createElement(AntdIcon, _extends({}, props, {\n    ref: ref,\n    icon: CloseOutlinedSvg\n  }));\n};\nif (process.env.NODE_ENV !== 'production') {\n  CloseOutlined.displayName = 'CloseOutlined';\n}\nexport default /*#__PURE__*/React.forwardRef(CloseOutlined);",
-        "/*\r\nauthor: Nathan Chen\r\ndate  : 23-Mar-2024\r\n*/\r\n\r\n\r\nimport { ConfigProvider, FormProps, Typography } from \"antd\";\r\nimport React, { ComponentProps, ReactNode } from \"react\";\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\";\r\nimport forge from 'node-forge'\r\nimport { ButtonConfig, TitleConfig } from \"./configs\";\r\nimport { CloseOutlined } from \"@ant-design/icons\";\r\n\r\nconst { Title } = Typography\r\n\r\nexport default abstract class BaseForm extends StreamlitComponentBase{\r\n  private publicKey: forge.pki.rsa.PublicKey | undefined\r\n\r\n  constructor(props: ComponentProps<any>){\r\n    super(props);\r\n    const pem = props.args['publicKey']\r\n    if(pem) this.publicKey = forge.pki.publicKeyFromPem(pem)\r\n  }\r\n\r\n  abstract getForm(): ReactNode;\r\n  abstract onCancel: FormProps['onClick'];\r\n\r\n  protected getHeader(title: TitleConfig | undefined, cancel: ButtonConfig | undefined): ReactNode | undefined {\r\n    return (title || cancel) &&\r\n    <div className=\"form-header\" style={title?.headerStyle}>\r\n      {\r\n        title &&\r\n        <Title className=\"form-title\" {...title.props}\r\n        >{title.text}</Title>\r\n      }\r\n      {\r\n        cancel &&\r\n        <CloseOutlined className=\"form-cancel\" onClick={this.onCancel}/>\r\n      }\r\n    </div>\r\n  }\r\n\r\n  protected setComponentValue(value: any){\r\n    if (!this.publicKey){\r\n      value.id = Math.random()\r\n      Streamlit.setComponentValue(value)\r\n    }\r\n    else{\r\n      const json = JSON.stringify(value)\r\n      let encrypted = this.publicKey.encrypt(json)\r\n      encrypted = forge.util.encode64(encrypted)\r\n      Streamlit.setComponentValue(encrypted)\r\n    }\r\n  }\r\n\r\n  render(): ReactNode {\r\n    return <div>\r\n      <ConfigProvider\r\n        theme={{\r\n          token: {\r\n            colorText: this.props.theme?.textColor,\r\n            colorTextPlaceholder: this.props.theme?.font,\r\n            colorPrimary: this.props.theme?.primaryColor,\r\n            colorPrimaryBg: this.props.theme?.primaryColor,\r\n            colorBgBase: this.props.theme?.secondaryBackgroundColor\r\n          }\r\n        }}\r\n      >\r\n        {this.getForm()}\r\n      </ConfigProvider>\r\n    </div>\r\n  }\r\n}",
-        "/*\r\nauthor: Nathan Chen\r\ndate  : 23-Mar-2024\r\n*/\r\n\r\n\r\nexport enum FormType{\r\n  default = 'default',\r\n  inline = 'inline',\r\n}\r\n\r\nexport enum HorizontalAlignment{\r\n  left = 'left',\r\n  right = 'right',\r\n  center = 'center'\r\n}\r\nexport const getTextAlign = (align: any, defaultAlign: HorizontalAlignment = HorizontalAlignment.left) : HorizontalAlignment =>\r\n  (typeof align === 'string') ? HorizontalAlignment[align as keyof typeof HorizontalAlignment] : defaultAlign\r\n\r\nexport enum TitleSize{\r\n  smaller = 5,\r\n  small = 4,\r\n  medium = 3,\r\n  large = 2,\r\n  extraLarge = 1\r\n}\r\nexport const getTitleSize = (size: any, defaultSize: TitleSize = TitleSize.medium) : TitleSize => {\r\n  if(typeof size === 'string')\r\n    return TitleSize[size as keyof typeof TitleSize]\r\n  else if(typeof size === 'number')\r\n    return size\r\n  else\r\n    return defaultSize\r\n}\r\n",
+        "/*\r\nauthor: Nathan Chen\r\ndate  : 20-Mar-2024\r\n*/\r\n\r\n\r\nimport { ConfigProvider, FormProps, Typography } from \"antd\";\r\nimport React, { ComponentProps, ReactNode } from \"react\";\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\";\r\nimport forge from 'node-forge'\r\nimport { ButtonConfig, TitleConfig } from \"./configs\";\r\nimport { CloseOutlined } from \"@ant-design/icons\";\r\n\r\nconst { Title } = Typography\r\n\r\nexport default abstract class BaseForm extends StreamlitComponentBase{\r\n  private publicKey: forge.pki.rsa.PublicKey | undefined\r\n\r\n  constructor(props: ComponentProps<any>){\r\n    super(props);\r\n    const pem = props.args['publicKey']\r\n    if(pem) this.publicKey = forge.pki.publicKeyFromPem(pem)\r\n  }\r\n\r\n  abstract getForm(): ReactNode;\r\n  abstract onCancel: FormProps['onClick'];\r\n\r\n  protected getHeader(title: TitleConfig | undefined, cancel: ButtonConfig | undefined): ReactNode | undefined {\r\n    return (title || cancel) &&\r\n    <div className=\"form-header\" style={title?.headerStyle}>\r\n      {\r\n        title &&\r\n        <Title className=\"form-title\" {...title.props}\r\n        >{title.text}</Title>\r\n      }\r\n      {\r\n        cancel &&\r\n        <CloseOutlined className=\"form-cancel\" onClick={this.onCancel}/>\r\n      }\r\n    </div>\r\n  }\r\n\r\n  protected setComponentValue(value: any){\r\n    if (!this.publicKey){\r\n      Streamlit.setComponentValue(value)\r\n    }\r\n    else{\r\n      const json = JSON.stringify(value)\r\n      let encrypted = this.publicKey.encrypt(json)\r\n      encrypted = forge.util.encode64(encrypted)\r\n      Streamlit.setComponentValue(encrypted)\r\n    }\r\n  }\r\n\r\n  render(): ReactNode {\r\n    return <div>\r\n      <ConfigProvider\r\n        theme={{\r\n          token: {\r\n            colorText: this.props.theme?.textColor,\r\n            colorTextPlaceholder: this.props.theme?.font,\r\n            colorPrimary: this.props.theme?.primaryColor,\r\n            colorPrimaryBg: this.props.theme?.primaryColor,\r\n            colorBgBase: this.props.theme?.secondaryBackgroundColor\r\n          }\r\n        }}\r\n      >\r\n        {this.getForm()}\r\n      </ConfigProvider>\r\n    </div>\r\n  }\r\n}",
+        "/*\r\nauthor: Nathan Chen\r\ndate  : 20-Mar-2024\r\n*/\r\n\r\n\r\nexport enum FormType{\r\n  default = 'default',\r\n  inline = 'inline',\r\n}\r\n\r\nexport enum HorizontalAlignment{\r\n  left = 'left',\r\n  right = 'right',\r\n  center = 'center'\r\n}\r\n\r\nexport enum TextAlign{\r\n  left = 'left',\r\n  right = 'right',\r\n  center = 'center',\r\n  justify = 'justify',\r\n  matchParent = 'match-parent'\r\n}\r\nexport const getTextAlign = (align: any, defaultAlign: HorizontalAlignment = HorizontalAlignment.left) : HorizontalAlignment =>\r\n  (typeof align === 'string') ? HorizontalAlignment[align as keyof typeof HorizontalAlignment] : defaultAlign\r\n\r\nexport enum TitleSize{\r\n  smaller = 5,\r\n  small = 4,\r\n  medium = 3,\r\n  large = 2,\r\n  extraLarge = 1\r\n}\r\nexport const getTitleSize = (size: any, defaultSize: TitleSize = TitleSize.medium) : TitleSize => {\r\n  if(typeof size === 'string')\r\n    return TitleSize[size as keyof typeof TitleSize]\r\n  else if(typeof size === 'number')\r\n    return size\r\n  else\r\n    return defaultSize\r\n}\r\n",
         "/*\r\n  author: Nathan Chen\r\n  date  : 20-Mar-2024\r\n*/\r\n\r\n\r\nimport { IconBaseProps } from \"@ant-design/icons/lib/components/Icon\"\r\nimport\r\n{\r\n  FormType,\r\n  HorizontalAlignment, TitleSize,\r\n  getTextAlign, getTitleSize,\r\n} from \"./types\"\r\nimport {\r\n  FormProps, FormItemProps,\r\n  InputProps, InputNumberProps, CheckboxProps, ButtonProps\r\n} from \"antd\"\r\nimport { \r\n  TitleProps\r\n} from \"antd/es/typography/Title\"\r\nimport React from \"react\"\r\n\r\nexport const getConfig = (config: any): any => (typeof config === 'object') ? config : {}\r\nconst getString = (text: any, defaultText: string): string => (typeof text === 'string') ? text : defaultText\r\n\r\n\r\nexport interface TitleConfig{\r\n  text: string\r\n  headerStyle?: React.CSSProperties\r\n  props: TitleProps\r\n}\r\nexport const getTitleConfig = (config: any, _default: any) : TitleConfig => {\r\n  config = getConfig(config)\r\n  let {text, size, align, title, cancel, submit, ...rest} = config\r\n\r\n  text = getString(text, _default?.text)\r\n  size = getTitleSize(size, _default?.size || TitleSize.medium)\r\n  align = getTextAlign(align, _default?.align || HorizontalAlignment.left)\r\n  const headerStyle: React.CSSProperties = {textAlign: align}\r\n  const props: TitleProps = {level: size, ...rest}\r\n\r\n  return {text, headerStyle, props}\r\n}\r\n\r\nexport interface FormItemRule {\r\n  message?: string\r\n  warningOnly?: boolean\r\n}\r\nexport interface FormItemRequired extends FormItemRule {\r\n  required: boolean\r\n}\r\nexport interface FormItemPattern extends FormItemRule {\r\n  pattern: string\r\n}\r\n\r\ninterface FormItemConfig{\r\n  formItemProps: FormItemProps\r\n}\r\nexport const getFormItemRules = (_required?: any, patterns?: any) => {\r\n  const rules: FormItemProps['rules'] = []\r\n  if (_required){\r\n    const {required, ...rest} = _required\r\n    rules.push({required, ...rest})\r\n  }\r\n  if (Array.isArray(patterns)){\r\n    patterns.forEach(value => {\r\n      const {pattern, ...rest} = value\r\n      rules.push({pattern:  RegExp(pattern), ...rest})\r\n    })\r\n  }\r\n  return rules\r\n}\r\nexport const getFormItemProps = (config: any, _default?: any) : [props: FormItemProps, rest: any] => {\r\n  config = getConfig(config)\r\n  _default = getConfig(_default)\r\n  let {label, width, required, patterns, ...rest} = config\r\n\r\n  label = label || _default?.label\r\n  width = width || _default?.width\r\n  \r\n  required = required || _default?.required\r\n  const rules = getFormItemRules(required, patterns)\r\n\r\n  return [{label, style: {width}, rules}, rest]\r\n}\r\n\r\nexport interface InputConfig extends FormItemConfig {\r\n  props: InputProps\r\n}\r\nexport const getInputConfig = (config: any, _default?: any) : InputConfig => {\r\n  const [formItemProps, props] = getFormItemProps(config, _default);\r\n  props.placeholder = props.placeholder || ((!formItemProps.label && !props.placeholder) ? _default?.placeholder : undefined)\r\n  return{formItemProps, props}\r\n}\r\n\r\nexport interface InputNumberConfig extends FormItemConfig {\r\n  props: InputNumberProps\r\n}\r\nexport const getInputNumberConfig = (config: any, _default?: any): InputNumberConfig => {\r\n  const [formItemProps, props] = getFormItemProps(config, _default)\r\n  props.placeholder = props.placeholder || ((!config.label && !props.placeholder) ? _default.placeholder : undefined)\r\n  props.style ??= {}\r\n  props.style.width ??= '100%'\r\n  return{formItemProps, props}\r\n}\r\n\r\nexport interface CheckboxConfig extends FormItemConfig {\r\n  text: string\r\n  props: CheckboxProps\r\n}\r\nexport const getCheckboxConfig = (config: any, _default?: any) : CheckboxConfig => {\r\n  config = getConfig(config)\r\n  let {label, ..._config} = config\r\n  label ||= _default?.label\r\n  const [formItemProps, props] = getFormItemProps(_config, _default)\r\n  formItemProps.valuePropName = 'checked'\r\n  return{text: label, formItemProps, props}\r\n}\r\n\r\nexport interface ButtonConfig {\r\n  text: string\r\n  props: ButtonProps\r\n}\r\nexport const getButtonConfig = (config: any, _default?: any) : ButtonConfig => {\r\n  config = getConfig(config)\r\n  let {label, width, style, ...props} = config\r\n  style = {\r\n    width: width || _default?.width,\r\n    ...style\r\n  }\r\n  props.style = style\r\n  return {\r\n    text: label || _default?.label || 'Submit',\r\n    props\r\n  }\r\n}\r\n\r\nexport interface IconConfig {\r\n  props: IconBaseProps\r\n}\r\nexport const getIconConfig = (config: any, _default?: any): IconConfig => {\r\n  config = getConfig(config)\r\n  return {props: config}\r\n}\r\n\r\nexport interface FormConfig {\r\n  type: FormType\r\n  props: FormProps\r\n  title?: TitleConfig\r\n  cancel?: ButtonConfig\r\n  submit: ButtonConfig\r\n}\r\nexport const getFormConfig = (config: any, _default?: any): FormConfig => {\r\n  config = getConfig(config)\r\n  _default = getConfig(_default)\r\n\r\n  let {type, labelSpan, wrapperSpan, maxWidth, align, title, cancel, submit, ...rest} = config\r\n  type = type || _default.type || FormType.default\r\n  maxWidth = maxWidth || _default.maxWidth\r\n  maxWidth = (!maxWidth && type === FormType.default) ? 300 : maxWidth\r\n  align = align || _default.align\r\n  const marginLeft = (align === HorizontalAlignment.center || align === HorizontalAlignment.right) ? 'auto' : undefined\r\n  const marginRIght = (align === HorizontalAlignment.center || align === HorizontalAlignment.left) ? 'auto' : undefined\r\n\r\n  const props = rest as FormProps\r\n  props.labelCol = {span: labelSpan || _default.labelSpan}\r\n  props.wrapperCol = {span: wrapperSpan || _default.wrapperSpan}\r\n  props.style = {\r\n    maxWidth,\r\n    marginLeft: marginLeft,\r\n    marginRight: marginRIght,\r\n    ...props.style\r\n  }\r\n\r\n  if (type === FormType.default){\r\n    _default.submit ??= {}\r\n    _default.submit.width ||= '100%'\r\n  }\r\n\r\n  return {type, props,\r\n    title: title && getTitleConfig(title, _default.title),\r\n    cancel: cancel && getIconConfig(cancel, _default.cancel),\r\n    submit: getButtonConfig(submit, _default.submit)\r\n  }\r\n}",
         "/*\r\nauthor: Nathan Chen\r\ndate  : 20-Mar-2024\r\n*/\r\n\r\n\r\nimport React, { ComponentProps, ReactNode } from \"react\";\r\nimport {\r\n  Form, Input, Checkbox, Button,\r\n  FormProps, Flex,\r\n} from \"antd\";\r\nimport {\r\n  UserOutlined, LockOutlined\r\n} from \"@ant-design/icons\"\r\nimport BaseForm from \"./base_form\";\r\nimport {\r\n  FormType\r\n} from \"./types\"\r\nimport {\r\n  FormConfig, InputConfig, CheckboxConfig, ButtonConfig,\r\n  getConfig, getFormConfig, getInputConfig, getCheckboxConfig, getButtonConfig\r\n} from \"./configs\";\r\n\r\n\r\ntype FieldType = {\r\n  username: string;\r\n  password: string;\r\n  remember: boolean;\r\n};\r\n\r\ninterface Configs extends FormConfig{\r\n  username: InputConfig\r\n  password: InputConfig\r\n  remember: CheckboxConfig | undefined\r\n  forgot: ButtonConfig | undefined\r\n}\r\nconst getConfigs = (configs: any): Configs => {\r\n  configs = getConfig(configs)\r\n  const {username, password, remember, forgot, ...form} = {...configs} as Configs\r\n\r\n  const formConfigs = getFormConfig(form, {\r\n    type: FormType.default,\r\n    title: {text: 'Login'},\r\n    submit: {label: '\ud83d\udd11 Sign In'}\r\n  })\r\n  return{\r\n    username: getInputConfig(username, {\r\n      placeholder: 'Username',\r\n      width: '100%',\r\n      required: { required: true }\r\n    }),\r\n    password: getInputConfig(password, {\r\n      placeholder: 'Password',\r\n      width: '100%',\r\n      required: { required: true }\r\n    }),\r\n    remember: remember && getCheckboxConfig(remember, {label: 'Remember me'}),\r\n    forgot: forgot && getButtonConfig(forgot, {label: 'Forgot password'}),\r\n    ...formConfigs\r\n  }\r\n}\r\n\r\nexport default class SigninForm extends BaseForm{\r\n  private configs: Configs\r\n  private default: FieldType\r\n\r\n  constructor(props: ComponentProps<any>){\r\n    super(props)\r\n    const args = props.args\r\n    \r\n    this.default = args['default'] || {}\r\n    this.default.remember = this.default.remember === false ? false : true\r\n\r\n    this.configs = getConfigs(args['configs'])\r\n  }\r\n\r\n  private onFinish: FormProps<FieldType>[\"onFinish\"] = (values) => {\r\n    const event = {event: 'signin', ...values}\r\n    this.setComponentValue(event)\r\n  }\r\n\r\n  onCancel = () => {\r\n    const event = {event: 'cancelSignin'}\r\n    this.setComponentValue(event)\r\n  }\r\n\r\n  private onForgot = () => {\r\n    const event = {'event': 'forgotPasswrod'}\r\n    this.setComponentValue(event)\r\n  }\r\n\r\n  private getAddon(remember: CheckboxConfig | undefined, forgot: ButtonConfig | undefined): ReactNode{\r\n    return <div className=\"signin-addon\">\r\n      {\r\n        remember &&\r\n        <Form.Item<FieldType> className=\"signin-remember\" name=\"remember\" valuePropName=\"checked\" noStyle {...remember.formItemProps}>\r\n          <Checkbox className=\"signin-remember\" {...remember.props}>{remember.text}</Checkbox>\r\n        </Form.Item>\r\n      }\r\n      {\r\n        forgot &&\r\n        <a className=\"signin-forgot\" onClick={this.onForgot} {...forgot.props}>{forgot.text}</a>\r\n      }\r\n    </div>\r\n  }\r\n\r\n  private getDefaultBody(username: InputConfig,\r\n  password: InputConfig,\r\n  remember: CheckboxConfig | undefined,\r\n  forgot: ButtonConfig | undefined,\r\n  submit: ButtonConfig) : ReactNode {\r\n    return <div className=\"signin-body\">\r\n      <Form.Item<FieldType> className=\"signin-username\" name=\"username\" {...username.formItemProps}>\r\n        <Input className=\"signin-username\" prefix={<UserOutlined />} {...username.props} />\r\n      </Form.Item>\r\n\r\n      <Form.Item<FieldType> className=\"signin-password\" name=\"password\" {...password.formItemProps}>\r\n        <Input.Password className=\"signin-password\" prefix={<LockOutlined />} {...password.props} />\r\n      </Form.Item>\r\n\r\n      { this.getAddon(remember, forgot) }\r\n\r\n      <Button className=\"signin-submit\" type=\"primary\" htmlType=\"submit\" {...submit.props}\r\n      >{submit.text}</Button>\r\n    </div>\r\n  }\r\n\r\n  private getInlineBody(username: InputConfig, password: InputConfig, submit: ButtonConfig) : ReactNode {\r\n    return <div className=\"signin-body\">\r\n      <Flex className=\"signin-body\" gap='small' align='start'>\r\n        <Form.Item<FieldType> className=\"signin-username\" name=\"username\" {...username.formItemProps}>\r\n          <Input className=\"signin-username\" prefix={<UserOutlined />} {...username.props} />\r\n        </Form.Item>\r\n\r\n        <Form.Item<FieldType> className=\"signin-password\" name=\"password\" {...password.formItemProps}>\r\n          <Input.Password className=\"signin-password\" prefix={<LockOutlined />} {...password.props} />\r\n        </Form.Item>\r\n\r\n        <Button className=\"signin-submit\" type=\"primary\" htmlType=\"submit\" {...submit.props}\r\n        >{submit.text}</Button>\r\n      </Flex>\r\n    </div>\r\n  }\r\n\r\n  private getDefaultForm(): ReactNode {\r\n    const {title, cancel, username, password, remember, forgot, submit, ...form} = this.configs\r\n\r\n    return(\r\n      <Form className=\"signin-form\" name=\"signin\" initialValues={ this.default } onFinish={this.onFinish} {...form.props}>\r\n        { this.getHeader(title, cancel) }\r\n        { this.getDefaultBody(username, password, remember, forgot, submit) }\r\n      </Form>\r\n    )\r\n  }\r\n  \r\n  private getInlineForm(): ReactNode {\r\n    const {title, cancel, username, password, remember, forgot, submit, ...form} = this.configs\r\n\r\n    return(\r\n      <Form className=\"signin-form\" name=\"signin\" initialValues={this.default} onFinish={this.onFinish} {...form.props}>\r\n        {this.getHeader(title, cancel)}\r\n        {this.getInlineBody(username, password, submit)}\r\n        {this.getAddon(remember, forgot)}\r\n      </Form>\r\n    )\r\n  }\r\n\r\n  getForm(): ReactNode {\r\n    const {type} = this.configs\r\n    if (type === FormType.inline) return this.getInlineForm()\r\n    else return this.getDefaultForm()\r\n  }\r\n}",
         "/*\r\nauthor: Nathan Chen\r\ndate  : 20-Mar-2024\r\n*/\r\n\r\n\r\nimport React, { ComponentProps, ReactNode } from \"react\";\r\nimport {\r\n  Form, Button,\r\n  type FormProps,\r\n} from \"antd\";\r\nimport BaseForm from \"./base_form\";\r\nimport {\r\n  FormConfig,\r\n  getConfig, getFormConfig,\r\n} from \"./configs\";\r\nimport { FormType } from \"./types\";\r\n\r\nconst getConfigs = (configs: any): FormConfig => {\r\n  configs = getConfig(configs)\r\n  const {...form} = {...configs} as FormConfig\r\n\r\n  const formConfigs = getFormConfig(form, {\r\n    type: FormType.default,\r\n    title: {text: \"Welcome\"},\r\n    submit: {label: '\ud83d\udd10 Sign Out'},\r\n  })\r\n  return formConfigs\r\n}\r\n\r\nexport default class SignoutForm extends BaseForm{\r\n  private configs: FormConfig\r\n\r\n  constructor(props: ComponentProps<any>){\r\n    super(props)\r\n    this.configs = getConfigs(props.args['configs'])\r\n  }\r\n\r\n  private onFinish: FormProps['onFinish'] = () => {\r\n    const event = {'event': 'signout'}\r\n    this.setComponentValue(event)\r\n  }\r\n\r\n  onCancel = () => {\r\n    const event = {'event': 'cancelSignout'}\r\n    this.setComponentValue(event)\r\n  }\r\n  getForm(): ReactNode {\r\n    const {submit, cancel, title, ...form} = this.configs\r\n    return(\r\n      <Form className=\"signout-form\" name='signout' onFinish={this.onFinish} {...form.props}>\r\n        { this.getHeader(title, cancel) }\r\n        <Button className=\"signout-submit\" type='primary' htmlType='submit' {...submit.props}>\r\n          {submit.text}\r\n        </Button>\r\n      </Form>\r\n    )\r\n  }\r\n}",
         "// This icon file is generated automatically.\nvar UnlockOutlined = { \"icon\": { \"tag\": \"svg\", \"attrs\": { \"viewBox\": \"64 64 896 896\", \"focusable\": \"false\" }, \"children\": [{ \"tag\": \"path\", \"attrs\": { \"d\": \"M832 464H332V240c0-30.9 25.1-56 56-56h248c30.9 0 56 25.1 56 56v68c0 4.4 3.6 8 8 8h56c4.4 0 8-3.6 8-8v-68c0-70.7-57.3-128-128-128H388c-70.7 0-128 57.3-128 128v224h-68c-17.7 0-32 14.3-32 32v384c0 17.7 14.3 32 32 32h640c17.7 0 32-14.3 32-32V496c0-17.7-14.3-32-32-32zm-40 376H232V536h560v304zM484 701v53c0 4.4 3.6 8 8 8h40c4.4 0 8-3.6 8-8v-53a48.01 48.01 0 10-56 0z\" } }] }, \"name\": \"unlock\", \"theme\": \"outlined\" };\nexport default UnlockOutlined;\n",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\n// GENERATE BY ./scripts/generate.ts\n// DON NOT EDIT IT MANUALLY\n\nimport * as React from 'react';\nimport UnlockOutlinedSvg from \"@ant-design/icons-svg/es/asn/UnlockOutlined\";\nimport AntdIcon from \"../components/AntdIcon\";\nvar UnlockOutlined = function UnlockOutlined(props, ref) {\n  return /*#__PURE__*/React.createElement(AntdIcon, _extends({}, props, {\n    ref: ref,\n    icon: UnlockOutlinedSvg\n  }));\n};\nif (process.env.NODE_ENV !== 'production') {\n  UnlockOutlined.displayName = 'UnlockOutlined';\n}\nexport default /*#__PURE__*/React.forwardRef(UnlockOutlined);",
         "/*\r\nauthor: Nathan Chen\r\ndate  : 20-Mar-2024\r\n*/\r\n\r\n\r\nimport React, { ComponentProps, ReactNode } from \"react\";\r\nimport {\r\n  Form, Input, Button,\r\n  FormProps, Flex,\r\n} from \"antd\";\r\nimport {\r\n  LockOutlined, UnlockOutlined\r\n} from \"@ant-design/icons\"\r\nimport BaseForm from \"./base_form\";\r\nimport {\r\n  FormType\r\n} from \"./types\"\r\nimport {\r\n  FormConfig, InputConfig, ButtonConfig,\r\n  getConfig, getFormConfig, getInputConfig,\r\n} from \"./configs\";\r\n\r\n\r\ntype FieldType = {\r\n  current: string;\r\n  new: string;\r\n  confirm: string;\r\n};\r\n\r\n\r\ninterface Configs extends FormConfig{\r\n  current: InputConfig\r\n  newPass: InputConfig\r\n  confirm: InputConfig\r\n  submit: ButtonConfig\r\n}\r\nconst getConfigs = (configs: any): Configs => {\r\n  configs = getConfig(configs)\r\n  const {current, newPass, confirm, submit, ...form} = {...configs} as Configs\r\n\r\n  const formConfigs = getFormConfig(form, {\r\n    title: {text: 'Change Password'},\r\n    submit: {label: '\ud83d\udd0f Change'}\r\n  })\r\n  return {\r\n    current: getInputConfig(current, {\r\n      placeholder: 'Current password',\r\n      width: '100%',\r\n      required: { required: true }\r\n    }),\r\n    newPass: getInputConfig(newPass, {\r\n      placeholder: 'New password',\r\n      width: '100%',\r\n      required: { required: true }\r\n    }),\r\n    confirm: getInputConfig(confirm, {\r\n      placeholder: 'Confirm password',\r\n      width: '100%',\r\n      required: { required: true }\r\n    }),\r\n    ...formConfigs\r\n  }\r\n}\r\n\r\n\r\nexport default class ChangePasswordForm extends BaseForm{\r\n  private configs: Configs\r\n  private default: FieldType\r\n\r\n  constructor(props: ComponentProps<any>){\r\n    super(props)\r\n    const args = props.args\r\n\r\n    this.default = args['default'] || {}\r\n    this.configs = getConfigs(args['configs'])\r\n  }\r\n\r\n  onCancel = () => {\r\n    const event = {event: 'cancelChangePassword'}\r\n    this.setComponentValue(event)\r\n  };\r\n\r\n  private getDefaultBody(current: InputConfig,\r\n  newPass: InputConfig,\r\n  confirm: InputConfig | undefined,\r\n  submit: ButtonConfig) : ReactNode {\r\n    return <div className=\"change-password-body\">\r\n      <Form.Item<FieldType> className=\"change-password-current\" name=\"current\" {...current.formItemProps}>\r\n        <Input.Password className=\"change-password-current\" prefix={<LockOutlined />} {...current.props} />\r\n      </Form.Item>\r\n\r\n      <Form.Item<FieldType> className=\"change-password-new\" name=\"new\" {...newPass.formItemProps}>\r\n        <Input.Password className=\"change-password-new\" prefix={<UnlockOutlined />} {...newPass.props} />\r\n      </Form.Item>\r\n\r\n      {\r\n        confirm &&\r\n        <Form.Item<FieldType> className=\"change-password-confirm\" name=\"confirm\" {...confirm.formItemProps}>\r\n          <Input.Password className=\"change-password-confirm\" prefix={<UnlockOutlined />} {...confirm.props} />\r\n        </Form.Item>\r\n      }\r\n\r\n      <Button className=\"change-password-submit\" type=\"primary\" htmlType=\"submit\" {...submit.props}>\r\n        {submit.text}\r\n      </Button>\r\n    </div>\r\n  }\r\n\r\n  private getInlineBody(current: InputConfig, newPass: InputConfig, confirm: InputConfig, submit: ButtonConfig) : ReactNode {\r\n    return <div className=\"change-password-body\">\r\n      <Flex className=\"change-password-body\" gap='small' align='start'>\r\n        <Form.Item<FieldType> className=\"change-password-current\" name=\"current\" {...current.formItemProps}>\r\n          <Input.Password className=\"change-password-current\" prefix={<LockOutlined />} {...current.props} />\r\n        </Form.Item>\r\n\r\n        <Form.Item<FieldType> className=\"change-password-new\" name=\"new\" {...newPass.formItemProps}>\r\n          <Input.Password className=\"change-password-password\" prefix={<UnlockOutlined />} {...newPass.props} />\r\n        </Form.Item>\r\n\r\n        {\r\n          confirm &&\r\n          <Form.Item<FieldType> className=\"change-password-confirm\" name=\"confirm\" {...confirm.formItemProps}>\r\n            <Input.Password className=\"change-password-password\" prefix={<UnlockOutlined />} {...confirm.props} />\r\n          </Form.Item>\r\n        }\r\n\r\n        <Button className=\"change-password-submit\" type=\"primary\" htmlType=\"submit\" {...submit.props}>\r\n          {submit.text}\r\n        </Button>\r\n      </Flex>\r\n    </div>\r\n  }\r\n\r\n  private getDefaultForm(): ReactNode {\r\n    const {title, cancel, current, newPass, confirm, submit, ...form} = this.configs\r\n\r\n    return(\r\n      <Form className=\"change-password-form\" name=\"change-password\" initialValues={ this.default } onFinish={this.onFinish} {...form.props}>\r\n        { this.getHeader(title, cancel) }\r\n        { this.getDefaultBody(current, newPass, confirm, submit) }\r\n      </Form>\r\n    )\r\n  }\r\n  \r\n  private getInlineForm(): ReactNode {\r\n    const {title, cancel, current, newPass, confirm, submit, ...form} = this.configs\r\n\r\n    return(\r\n      <Form className=\"change-password-form\" name=\"change-password\" initialValues={this.default} onFinish={this.onFinish} {...form.props}>\r\n        { this.getHeader(title, cancel) }\r\n        { this.getInlineBody(current, newPass, confirm, submit) }\r\n      </Form>\r\n    )\r\n  }\r\n\r\n  private onFinish: FormProps['onFinish'] = (values) => {\r\n    const event = {event: 'changePassword', ...values}\r\n    this.setComponentValue(event)\r\n  }\r\n\r\n  getForm(): ReactNode {\r\n    const {type} = this.configs\r\n    if (type === FormType.inline) return this.getInlineForm()\r\n    else return this.getDefaultForm()\r\n  }\r\n}\r\n  ",
         "/*\r\nauthor: Nathan Chen\r\ndate  : 20-Mar-2024\r\n*/\r\n\r\n\r\nimport React from \"react\";\r\nimport { createRoot } from \"react-dom/client\";\r\nimport SigninForm from \"./signin_form\";\r\nimport { ComponentProps, withStreamlitConnection } from \"streamlit-component-lib\";\r\nimport SignoutForm from \"./signout_form\";\r\nimport ChangePasswordForm from \"./change_password_form\";\r\n\r\n\r\nconst getComponent = (props: ComponentProps) => {\r\n    const id = props.args['id']\r\n    switch (id){\r\n        case 'signin': return (<SigninForm {...props} />)\r\n        case 'signout': return (<SignoutForm {...props} />)\r\n        case 'changePassword': return(<ChangePasswordForm {...props} />)\r\n        default: return (<div />)\r\n    }\r\n}\r\n\r\n\r\nconst StreamlitComponent = withStreamlitConnection(getComponent)\r\n\r\n\r\nconst container = document.getElementById('root');\r\nconst root = createRoot(container!);\r\n\r\nroot.render(\r\n    <React.StrictMode>\r\n        <StreamlitComponent />\r\n    </React.StrictMode>\r\n);"
```

### Comparing `streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui.egg-info/PKG-INFO` & `streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-rsa-auth-ui
-Version: 1.1.0
+Version: 1.1.1
 Summary: Streamlit RSA Authenticator UI
 Home-page: https://github.com/NathanChen198/streamlit-rsa-auth-ui
 Author: Nathan Chen
 Author-email: nathan.chen.198@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,63 +29,73 @@
 [![GitHub license][license_badge]][license_link]
 [![GitHub issues][issue_badge]][issue_link]
 [![GitHub pull requests][pull_badge]][pull_link]
 
 Encryption on Authenticate widget data from client to server.
 
 ## What is Streamlit RSA Authenticator UI?
+
 ### What is Http protocol
+
 Http is the information transfer protocol between networked devices. However, all the requests and responses are in plaintext, which means that anyone can read them.
 
 If you want to deploy streamlit server using http protocol (not https protocol) and you add the user authentication, user password can be read by anyone in the network as it is the plaintext for http protocol.
 
 `streamlit-rsa-auth-ui` correct it by encrypting user information including password at the client browser before transmit to streamlit server using [RSA algorithm](https://www.techtarget.com/searchsecurity/definition/RSA)
 
 ### What is RSA algorithm
+
 It is [asymmetric cryptography](https://www.techtarget.com/searchsecurity/definition/asymmetric-cryptography), uses two different but mathematically linked [keys](https://www.techtarget.com/searchsecurity/definition/key)
+
 - [Public key](https://www.techtarget.com/searchsecurity/definition/public-key) that can be share with everyone
 - [Private key](https://www.techtarget.com/searchsecurity/definition/private-key) must be kept secret
 
 ## Installation
+
 Open a terminal and run:
 
-``` terminal
+```terminal
 pip install streamlit-rsa-auth-ui
 ```
 
-
 ## Quickstart
+
 ### Gnerate RSA Key Pair
+
 Create a new file generateKeys.py
 
-``` python
+```python
 from streamlit_rsa_auth_ui import Encryptor
 
 encryptor = Encryptor.generateNew(2048)
 encryptor.save('rsa', 'authkey')
 ```
 
 Run `generateKeys.py` python script
-``` terminal
+
+```terminal
 python generateKeys.py
 ```
 
 this will create a private key and public key pair
+
 - private key with the file name `authkey`
 - public key with the file name `authkey.pub`
 
-``` md
+```md
 ├── rsa
-│   ├── authkey
-│   │   authkey.pub
+│ ├── authkey
+│ │ authkey.pub
 ```
 
 ### Create streamlit page
+
 Create a new file example.py
-``` python
+
+```python
 import streamlit as st
 from streamlit_rsa_auth_ui import Encryptor, authUI, SigninEvent, SigninFormConfig, getEvent
 ss = st.session_state
 
 encryptor = Encryptor.load('rsa', 'authkey')
 ui = authUI('login_ui_result', encryptor.publicKeyPem)
 
@@ -117,42 +127,56 @@
 
 st.title('Streamlit Rsa Auth UI Test')
 button = st.button('test')
 button
 ```
 
 Run the streamlit app
-``` terminal
+
+```terminal
 streamlit run example.py
 ```
 
-
 ## Change Log
+
 ### Version 0.0.1
+
 - Initial release
+
 ### Version 0.0.2
+
 - Fix missing frontend issue
+
 ### Version 0.0.3
+
 - Optional 'cancel' button to signoutform
 - Minor bug fixed
 - Remove bootstrap.min.css warning
+
 ### Version 0.0.4
+
 - Remove location setting(seem redundunt as if you want to add to any container/sidebar you can call with syntax)
 - Add in classname to frontend so that easier to add in custom styling if needed
 - Remove off the unnecessary excess height of streamlit
+
 ### Version 1.0.0
+
 - More customizable UI
 - Add inline mode
 - Add ChangePassword UI
+
 ### Version 1.1.0
+
 - Add id property in event if no public key is provided
 - Add AuthUI class
 - Add Configs class
 
+### Version 1.1.1
 
+- Fix 'no remember in signinevent' when remember option is disabled
 
 [pypi_badge]: https://img.shields.io/pypi/v/streamlit-rsa-auth-ui.svg
 [pypi_link]: https://pypi.org/project/streamlit-rsa-auth-ui
 [pypi_download_badge]: https://static.pepy.tech/badge/streamlit-rsa-auth-ui
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-rsa-auth-ui
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
```

### Comparing `streamlit-rsa-auth-ui-1.1.0/streamlit_rsa_auth_ui.egg-info/SOURCES.txt` & `streamlit-rsa-auth-ui-1.1.1/streamlit_rsa_auth_ui.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 streamlit_rsa_auth_ui.egg-info/SOURCES.txt
 streamlit_rsa_auth_ui.egg-info/dependency_links.txt
 streamlit_rsa_auth_ui.egg-info/requires.txt
 streamlit_rsa_auth_ui.egg-info/top_level.txt
 streamlit_rsa_auth_ui/frontend/build/asset-manifest.json
 streamlit_rsa_auth_ui/frontend/build/index.css
 streamlit_rsa_auth_ui/frontend/build/index.html
-streamlit_rsa_auth_ui/frontend/build/static/js/main.2243da37.js
-streamlit_rsa_auth_ui/frontend/build/static/js/main.2243da37.js.LICENSE.txt
-streamlit_rsa_auth_ui/frontend/build/static/js/main.2243da37.js.map
+streamlit_rsa_auth_ui/frontend/build/static/js/main.3bc257bc.js
+streamlit_rsa_auth_ui/frontend/build/static/js/main.3bc257bc.js.LICENSE.txt
+streamlit_rsa_auth_ui/frontend/build/static/js/main.3bc257bc.js.map
```
