# Comparing `tmp/streamlit-ldap-authenticator-0.2.3.tar.gz` & `tmp/streamlit-ldap-authenticator-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-ldap-authenticator-0.2.3.tar", last modified: Thu Apr  4 00:21:21 2024, max compression
+gzip compressed data, was "streamlit-ldap-authenticator-0.2.4.tar", last modified: Mon Apr  8 11:32:28 2024, max compression
```

## Comparing `streamlit-ldap-authenticator-0.2.3.tar` & `streamlit-ldap-authenticator-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 00:21:21.680514 streamlit-ldap-authenticator-0.2.3/
--rw-rw-rw-   0        0        0     1089 2024-02-22 23:54:56.000000 streamlit-ldap-authenticator-0.2.3/LICENSE
--rw-rw-rw-   0        0        0    23576 2024-04-04 00:21:21.674682 streamlit-ldap-authenticator-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    22561 2024-04-04 00:18:12.000000 streamlit-ldap-authenticator-0.2.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 00:21:21.680844 streamlit-ldap-authenticator-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1505 2024-04-04 00:18:20.000000 streamlit-ldap-authenticator-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 00:21:21.639383 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/
--rw-rw-rw-   0        0        0      308 2024-03-23 04:43:04.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/__init__.py
--rw-rw-rw-   0        0        0    18464 2024-04-04 00:18:05.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/authenticate.py
--rw-rw-rw-   0        0        0    10523 2024-03-23 04:42:56.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/configs.py
--rw-rw-rw-   0        0        0      971 2024-02-22 10:48:27.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/exceptions.py
--rw-rw-rw-   0        0        0     7428 2024-04-04 00:17:59.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/ldap_authenticate.py
-drwxrwxrwx   0        0        0        0 2024-04-04 00:21:21.666118 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/
--rw-rw-rw-   0        0        0    23576 2024-04-04 00:21:21.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-04-04 00:21:21.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 00:21:21.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      231 2024-04-04 00:21:21.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-04 00:21:21.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 11:32:28.746775 streamlit-ldap-authenticator-0.2.4/
+-rw-rw-rw-   0        0        0     1089 2024-02-22 23:54:56.000000 streamlit-ldap-authenticator-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0    23668 2024-04-08 11:32:28.742824 streamlit-ldap-authenticator-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    22653 2024-04-08 11:31:49.000000 streamlit-ldap-authenticator-0.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 11:32:28.746775 streamlit-ldap-authenticator-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1505 2024-04-08 11:31:58.000000 streamlit-ldap-authenticator-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 11:32:28.716378 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/
+-rw-rw-rw-   0        0        0      308 2024-03-23 04:43:04.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/__init__.py
+-rw-rw-rw-   0        0        0    18464 2024-04-08 10:58:49.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/authenticate.py
+-rw-rw-rw-   0        0        0    10523 2024-03-23 04:42:56.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/configs.py
+-rw-rw-rw-   0        0        0      971 2024-02-22 10:48:27.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/exceptions.py
+-rw-rw-rw-   0        0        0     7428 2024-04-04 00:17:59.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/ldap_authenticate.py
+drwxrwxrwx   0        0        0        0 2024-04-08 11:32:28.737010 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/
+-rw-rw-rw-   0        0        0    23668 2024-04-08 11:32:28.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2024-04-08 11:32:28.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 11:32:28.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      231 2024-04-08 11:32:28.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-08 11:32:28.000000 streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/top_level.txt
```

### Comparing `streamlit-ldap-authenticator-0.2.3/LICENSE` & `streamlit-ldap-authenticator-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.3/PKG-INFO` & `streamlit-ldap-authenticator-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: streamlit-ldap-authenticator
-Version: 0.2.3
+Version: 0.2.4
 Summary: Authenticate using ldap
 Home-page: https://github.com/NathanChen198/streamlit-ldap-authenticator
 Author: Nathan Chen
 Author-email: nathan.chen.198@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit>=0.63
 Requires-Dist: ldap3>=2.9.1
 Requires-Dist: pyjwt>=2.8.0
 Requires-Dist: streamlit-cookies-controller>=0.0.3
-Requires-Dist: streamlit-rsa-auth-ui>=1.1.0
+Requires-Dist: streamlit-rsa-auth-ui>=1.1.1
 Provides-Extra: devel
 Requires-Dist: wheel; extra == "devel"
 Requires-Dist: pytest==7.4.0; extra == "devel"
 Requires-Dist: playwright==1.39.0; extra == "devel"
 Requires-Dist: requests==2.31.0; extra == "devel"
 Requires-Dist: pytest-playwright-snapshot==1.0; extra == "devel"
 Requires-Dist: pytest-rerunfailures==12.0; extra == "devel"
@@ -514,14 +514,18 @@
 
 - Fix misleading error message of "Wrong username or password" when there is an exception occured during ldap connection
 
 ### Version 0.2.3
 
 - Enhance security by clearing password from Connection object after bind.
 
+### Version 0.2.4
+
+- Fix 'no attribute in signinevent' when cookie option is disabled.
+
 [pypi_badge]: https://img.shields.io/pypi/v/streamlit-ldap-authenticator.svg
 [pypi_link]: https://pypi.org/project/streamlit-ldap-authenticator
 [pypi_download_badge]: https://static.pepy.tech/badge/streamlit-ldap-authenticator
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
 [license_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator/blob/main/LICENSE
```

### Comparing `streamlit-ldap-authenticator-0.2.3/README.md` & `streamlit-ldap-authenticator-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -488,14 +488,18 @@
 
 - Fix misleading error message of "Wrong username or password" when there is an exception occured during ldap connection
 
 ### Version 0.2.3
 
 - Enhance security by clearing password from Connection object after bind.
 
+### Version 0.2.4
+
+- Fix 'no attribute in signinevent' when cookie option is disabled.
+
 [pypi_badge]: https://img.shields.io/pypi/v/streamlit-ldap-authenticator.svg
 [pypi_link]: https://pypi.org/project/streamlit-ldap-authenticator
 [pypi_download_badge]: https://static.pepy.tech/badge/streamlit-ldap-authenticator
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
 [license_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator/blob/main/LICENSE
```

### Comparing `streamlit-ldap-authenticator-0.2.3/setup.py` & `streamlit-ldap-authenticator-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Author   : Nathan Chen
-# Date     : 04-Apr-2024
+# Date     : 08-Apr-2024
 
 
 from pathlib import Path
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='UTF-8')
 
 setup(
     name='streamlit-ldap-authenticator',
-    version='0.2.3',
+    version='0.2.4',
     author='Nathan Chen',
     author_email='nathan.chen.198@gmail.com',
     description='Authenticate using ldap',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/NathanChen198/streamlit-ldap-authenticator',
     packages=find_packages(),
@@ -29,15 +29,15 @@
         # By definition, a Custom Component depends on Streamlit.
         # If your component has other Python dependencies, list
         # them here.
         "streamlit >= 0.63",
         "ldap3 >= 2.9.1",
         "pyjwt>=2.8.0",
         "streamlit-cookies-controller >= 0.0.3",
-        "streamlit-rsa-auth-ui >= 1.1.0"
+        "streamlit-rsa-auth-ui >= 1.1.1"
     ],
     extras_require={
         "devel": [
             "wheel",
             "pytest==7.4.0",
             "playwright==1.39.0",
             "requests==2.31.0",
```

### Comparing `streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/authenticate.py` & `streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/authenticate.py`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/configs.py` & `streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/configs.py`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/exceptions.py` & `streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/ldap_authenticate.py` & `streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator/ldap_authenticate.py`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/PKG-INFO` & `streamlit-ldap-authenticator-0.2.4/streamlit_ldap_authenticator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: streamlit-ldap-authenticator
-Version: 0.2.3
+Version: 0.2.4
 Summary: Authenticate using ldap
 Home-page: https://github.com/NathanChen198/streamlit-ldap-authenticator
 Author: Nathan Chen
 Author-email: nathan.chen.198@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit>=0.63
 Requires-Dist: ldap3>=2.9.1
 Requires-Dist: pyjwt>=2.8.0
 Requires-Dist: streamlit-cookies-controller>=0.0.3
-Requires-Dist: streamlit-rsa-auth-ui>=1.1.0
+Requires-Dist: streamlit-rsa-auth-ui>=1.1.1
 Provides-Extra: devel
 Requires-Dist: wheel; extra == "devel"
 Requires-Dist: pytest==7.4.0; extra == "devel"
 Requires-Dist: playwright==1.39.0; extra == "devel"
 Requires-Dist: requests==2.31.0; extra == "devel"
 Requires-Dist: pytest-playwright-snapshot==1.0; extra == "devel"
 Requires-Dist: pytest-rerunfailures==12.0; extra == "devel"
@@ -514,14 +514,18 @@
 
 - Fix misleading error message of "Wrong username or password" when there is an exception occured during ldap connection
 
 ### Version 0.2.3
 
 - Enhance security by clearing password from Connection object after bind.
 
+### Version 0.2.4
+
+- Fix 'no attribute in signinevent' when cookie option is disabled.
+
 [pypi_badge]: https://img.shields.io/pypi/v/streamlit-ldap-authenticator.svg
 [pypi_link]: https://pypi.org/project/streamlit-ldap-authenticator
 [pypi_download_badge]: https://static.pepy.tech/badge/streamlit-ldap-authenticator
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
 [license_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator/blob/main/LICENSE
```

