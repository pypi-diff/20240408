# Comparing `tmp/protonmail-api-client-1.3.3.tar.gz` & `tmp/protonmail-api-client-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protonmail-api-client-1.3.3.tar", last modified: Sat Mar 23 18:25:12 2024, max compression
+gzip compressed data, was "protonmail-api-client-1.3.4.tar", last modified: Sun Apr  7 23:52:27 2024, max compression
```

## Comparing `protonmail-api-client-1.3.3.tar` & `protonmail-api-client-1.3.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 18:25:12.077073 protonmail-api-client-1.3.3/
--rw-rw-rw-   0        0        0    35823 2023-08-07 00:41:20.000000 protonmail-api-client-1.3.3/LICENSE
--rw-rw-rw-   0        0        0       85 2023-09-09 18:01:44.000000 protonmail-api-client-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0    45914 2024-03-23 18:25:12.077073 protonmail-api-client-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3839 2023-11-23 22:47:44.000000 protonmail-api-client-1.3.3/README.md
--rw-rw-rw-   0        0        0      952 2024-03-23 18:19:33.000000 protonmail-api-client-1.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-23 18:25:12.078044 protonmail-api-client-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-09-09 16:25:43.000000 protonmail-api-client-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-23 18:25:12.053905 protonmail-api-client-1.3.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-23 18:25:12.066904 protonmail-api-client-1.3.3/src/protonmail/
--rw-rw-rw-   0        0        0       32 2023-09-09 17:48:47.000000 protonmail-api-client-1.3.3/src/protonmail/__init__.py
--rw-rw-rw-   0        0        0    37531 2024-03-23 18:11:55.000000 protonmail-api-client-1.3.3/src/protonmail/client.py
--rw-rw-rw-   0        0        0     1176 2023-08-13 15:48:03.000000 protonmail-api-client-1.3.3/src/protonmail/constants.py
--rw-rw-rw-   0        0        0      199 2024-03-23 18:06:55.000000 protonmail-api-client-1.3.3/src/protonmail/exceptions.py
--rw-rw-rw-   0        0        0     1186 2023-08-13 15:46:48.000000 protonmail-api-client-1.3.3/src/protonmail/logger.py
--rw-rw-rw-   0        0        0     2816 2024-03-10 11:50:55.000000 protonmail-api-client-1.3.3/src/protonmail/models.py
--rw-rw-rw-   0        0        0     5442 2023-09-09 13:05:03.000000 protonmail-api-client-1.3.3/src/protonmail/pgp.py
-drwxrwxrwx   0        0        0        0 2024-03-23 18:25:12.070907 protonmail-api-client-1.3.3/src/protonmail/utils/
--rw-rw-rw-   0        0        0        0 2023-08-06 23:59:40.000000 protonmail-api-client-1.3.3/src/protonmail/utils/__init__.py
--rw-rw-rw-   0        0        0      220 2023-08-13 15:27:53.000000 protonmail-api-client-1.3.3/src/protonmail/utils/openpgp.html
--rw-rw-rw-   0        0        0     5681 2023-09-09 17:09:37.000000 protonmail-api-client-1.3.3/src/protonmail/utils/pysrp.py
--rw-rw-rw-   0        0        0     2077 2024-03-10 11:56:42.000000 protonmail-api-client-1.3.3/src/protonmail/utils/script.js
--rw-rw-rw-   0        0        0     2304 2023-09-09 17:11:10.000000 protonmail-api-client-1.3.3/src/protonmail/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-23 18:25:12.075043 protonmail-api-client-1.3.3/src/protonmail_api_client.egg-info/
--rw-rw-rw-   0        0        0    45914 2024-03-23 18:25:12.000000 protonmail-api-client-1.3.3/src/protonmail_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      646 2024-03-23 18:25:12.000000 protonmail-api-client-1.3.3/src/protonmail_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 18:25:12.000000 protonmail-api-client-1.3.3/src/protonmail_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-03-23 18:25:12.000000 protonmail-api-client-1.3.3/src/protonmail_api_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-23 18:25:12.000000 protonmail-api-client-1.3.3/src/protonmail_api_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 23:52:27.262902 protonmail-api-client-1.3.4/
+-rw-rw-rw-   0        0        0    35823 2023-08-07 00:41:20.000000 protonmail-api-client-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-09-09 18:01:44.000000 protonmail-api-client-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    45914 2024-04-07 23:52:27.262902 protonmail-api-client-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3839 2023-11-23 22:47:44.000000 protonmail-api-client-1.3.4/README.md
+-rw-rw-rw-   0        0        0      952 2024-04-07 23:52:02.000000 protonmail-api-client-1.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 23:52:27.263902 protonmail-api-client-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-09-09 16:25:43.000000 protonmail-api-client-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 23:52:27.239918 protonmail-api-client-1.3.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 23:52:27.251903 protonmail-api-client-1.3.4/src/protonmail/
+-rw-rw-rw-   0        0        0       32 2023-09-09 17:48:47.000000 protonmail-api-client-1.3.4/src/protonmail/__init__.py
+-rw-rw-rw-   0        0        0    37631 2024-04-07 23:52:02.000000 protonmail-api-client-1.3.4/src/protonmail/client.py
+-rw-rw-rw-   0        0        0     1176 2023-08-13 15:48:03.000000 protonmail-api-client-1.3.4/src/protonmail/constants.py
+-rw-rw-rw-   0        0        0      199 2024-03-23 18:30:56.000000 protonmail-api-client-1.3.4/src/protonmail/exceptions.py
+-rw-rw-rw-   0        0        0     1186 2023-08-13 15:46:48.000000 protonmail-api-client-1.3.4/src/protonmail/logger.py
+-rw-rw-rw-   0        0        0     2816 2024-03-10 11:50:55.000000 protonmail-api-client-1.3.4/src/protonmail/models.py
+-rw-rw-rw-   0        0        0     5442 2023-09-09 13:05:03.000000 protonmail-api-client-1.3.4/src/protonmail/pgp.py
+drwxrwxrwx   0        0        0        0 2024-04-07 23:52:27.256902 protonmail-api-client-1.3.4/src/protonmail/utils/
+-rw-rw-rw-   0        0        0        0 2023-08-06 23:59:40.000000 protonmail-api-client-1.3.4/src/protonmail/utils/__init__.py
+-rw-rw-rw-   0        0        0      220 2023-08-13 15:27:53.000000 protonmail-api-client-1.3.4/src/protonmail/utils/openpgp.html
+-rw-rw-rw-   0        0        0     5681 2023-09-09 17:09:37.000000 protonmail-api-client-1.3.4/src/protonmail/utils/pysrp.py
+-rw-rw-rw-   0        0        0     2077 2024-03-10 11:56:42.000000 protonmail-api-client-1.3.4/src/protonmail/utils/script.js
+-rw-rw-rw-   0        0        0     2304 2023-09-09 17:11:10.000000 protonmail-api-client-1.3.4/src/protonmail/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 23:52:27.261901 protonmail-api-client-1.3.4/src/protonmail_api_client.egg-info/
+-rw-rw-rw-   0        0        0    45914 2024-04-07 23:52:27.000000 protonmail-api-client-1.3.4/src/protonmail_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      646 2024-04-07 23:52:27.000000 protonmail-api-client-1.3.4/src/protonmail_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 23:52:27.000000 protonmail-api-client-1.3.4/src/protonmail_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-04-07 23:52:27.000000 protonmail-api-client-1.3.4/src/protonmail_api_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 23:52:27.000000 protonmail-api-client-1.3.4/src/protonmail_api_client.egg-info/top_level.txt
```

### Comparing `protonmail-api-client-1.3.3/LICENSE` & `protonmail-api-client-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `protonmail-api-client-1.3.3/PKG-INFO` & `protonmail-api-client-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protonmail-api-client
-Version: 1.3.3
+Version: 1.3.4
 Summary: This is not an official python ProtonMail API client. it allows you to read, send and delete messages in protonmail, as well as render a ready-made template with embedded images.
 Author-email: opulentfox-29 <3acqw2bx@duck.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `protonmail-api-client-1.3.3/README.md` & `protonmail-api-client-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `protonmail-api-client-1.3.3/pyproject.toml` & `protonmail-api-client-1.3.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "protonmail-api-client"
-version = "1.3.3"
+version = "1.3.4"
 description = "This is not an official python ProtonMail API client. it allows you to read, send and delete messages in protonmail, as well as render a ready-made template with embedded images."
 readme = "README.md"
 authors = [{ name = "opulentfox-29", email = "3acqw2bx@duck.com" }]
 license = { file = "LICENSE" }
 keywords = ["protonmail", "api", "client", "proton", "proton-mail", "send", "read", "mail", "email"]
 dependencies = [
 	"aiohttp",
```

### Comparing `protonmail-api-client-1.3.3/src/protonmail/client.py` & `protonmail-api-client-1.3.4/src/protonmail/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -687,27 +687,28 @@
             extra=response,
         )
         return conversation
 
     @staticmethod
     def _prepare_message(data: str) -> str:
         """Converting an unencrypted message into a multipart mime."""
-        data_base64 = b64encode(data.encode())
+        data_base64 = b64encode(data.encode()).decode()
+        data_base64 = '\n'.join([data_base64[i:i+76] for i in range(0, len(data_base64), 76)])
 
         msg_mixed = MIMEMultipart('mixed')
         msg_alt = MIMEMultipart('alternative')
         msg_plain = MIMEText('', _subtype='plain')
         msg_related = MIMEMultipart('related')
         msg_base = MIMEText('', _subtype='html')
 
         msg_base.replace_header('Content-Transfer-Encoding', 'base64')
         msg_base.set_payload(data_base64, 'utf-8')
 
         msg_plain.replace_header('Content-Transfer-Encoding', 'quoted-printable')
-        msg_plain.set_payload('hello', 'utf-8')
+        msg_plain.set_payload('', 'utf-8')
 
         msg_alt.attach(msg_plain)
         msg_related.attach(msg_base)
         msg_alt.attach(msg_related)
 
         msg_mixed.attach(msg_alt)
         message = msg_mixed.as_string().replace('MIME-Version: 1.0\n', '')
```

### Comparing `protonmail-api-client-1.3.3/src/protonmail/constants.py` & `protonmail-api-client-1.3.4/src/protonmail/constants.py`

 * *Files identical despite different names*

### Comparing `protonmail-api-client-1.3.3/src/protonmail/logger.py` & `protonmail-api-client-1.3.4/src/protonmail/logger.py`

 * *Files identical despite different names*

### Comparing `protonmail-api-client-1.3.3/src/protonmail/models.py` & `protonmail-api-client-1.3.4/src/protonmail/models.py`

 * *Files identical despite different names*

### Comparing `protonmail-api-client-1.3.3/src/protonmail/pgp.py` & `protonmail-api-client-1.3.4/src/protonmail/pgp.py`

 * *Files identical despite different names*

### Comparing `protonmail-api-client-1.3.3/src/protonmail/utils/pysrp.py` & `protonmail-api-client-1.3.4/src/protonmail/utils/pysrp.py`

 * *Files identical despite different names*

### Comparing `protonmail-api-client-1.3.3/src/protonmail/utils/script.js` & `protonmail-api-client-1.3.4/src/protonmail/utils/script.js`

 * *Files identical despite different names*

### Comparing `protonmail-api-client-1.3.3/src/protonmail/utils/utils.py` & `protonmail-api-client-1.3.4/src/protonmail/utils/utils.py`

 * *Files identical despite different names*

### Comparing `protonmail-api-client-1.3.3/src/protonmail_api_client.egg-info/PKG-INFO` & `protonmail-api-client-1.3.4/src/protonmail_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protonmail-api-client
-Version: 1.3.3
+Version: 1.3.4
 Summary: This is not an official python ProtonMail API client. it allows you to read, send and delete messages in protonmail, as well as render a ready-made template with embedded images.
 Author-email: opulentfox-29 <3acqw2bx@duck.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `protonmail-api-client-1.3.3/src/protonmail_api_client.egg-info/SOURCES.txt` & `protonmail-api-client-1.3.4/src/protonmail_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

