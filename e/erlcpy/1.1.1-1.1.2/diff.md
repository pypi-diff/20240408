# Comparing `tmp/erlcpy-1.1.1.tar.gz` & `tmp/erlcpy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlcpy-1.1.1.tar", last modified: Mon Apr  8 19:45:43 2024, max compression
+gzip compressed data, was "erlcpy-1.1.2.tar", last modified: Mon Apr  8 20:28:14 2024, max compression
```

## Comparing `erlcpy-1.1.1.tar` & `erlcpy-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 19:45:43.921011 erlcpy-1.1.1/
--rw-rw-rw-   0        0        0     1085 2024-02-25 08:54:13.000000 erlcpy-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      363 2024-04-08 19:45:43.919759 erlcpy-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      666 2024-02-25 08:21:47.000000 erlcpy-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 19:45:43.902659 erlcpy-1.1.1/erlcpy/
--rw-rw-rw-   0        0        0      381 2024-04-08 19:44:43.000000 erlcpy-1.1.1/erlcpy/__init__.py
--rw-rw-rw-   0        0        0     2114 2024-04-08 19:44:29.000000 erlcpy-1.1.1/erlcpy/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 19:45:43.919759 erlcpy-1.1.1/erlcpy.egg-info/
--rw-rw-rw-   0        0        0      363 2024-04-08 19:45:43.000000 erlcpy-1.1.1/erlcpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-08 19:45:43.000000 erlcpy-1.1.1/erlcpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 19:45:43.000000 erlcpy-1.1.1/erlcpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-08 19:45:43.000000 erlcpy-1.1.1/erlcpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-08 19:45:43.000000 erlcpy-1.1.1/erlcpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 19:45:43.921011 erlcpy-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      469 2024-04-08 19:45:11.000000 erlcpy-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:28:14.220370 erlcpy-1.1.2/
+-rw-rw-rw-   0        0        0     1085 2024-02-25 08:54:13.000000 erlcpy-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      363 2024-04-08 20:28:14.219365 erlcpy-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2024-02-25 08:21:47.000000 erlcpy-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 20:28:14.185933 erlcpy-1.1.2/erlcpy/
+-rw-rw-rw-   0        0        0      381 2024-04-08 19:44:43.000000 erlcpy-1.1.2/erlcpy/__init__.py
+-rw-rw-rw-   0        0        0     2341 2024-04-08 20:27:44.000000 erlcpy-1.1.2/erlcpy/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:28:14.217986 erlcpy-1.1.2/erlcpy.egg-info/
+-rw-rw-rw-   0        0        0      363 2024-04-08 20:28:14.000000 erlcpy-1.1.2/erlcpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-08 20:28:14.000000 erlcpy-1.1.2/erlcpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 20:28:14.000000 erlcpy-1.1.2/erlcpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 20:28:14.000000 erlcpy-1.1.2/erlcpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-08 20:28:14.000000 erlcpy-1.1.2/erlcpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 20:28:14.220370 erlcpy-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      469 2024-04-08 20:28:04.000000 erlcpy-1.1.2/setup.py
```

### Comparing `erlcpy-1.1.1/LICENSE` & `erlcpy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `erlcpy-1.1.1/README.md` & `erlcpy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `erlcpy-1.1.1/erlcpy/main.py` & `erlcpy-1.1.2/erlcpy/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,31 @@
         self.headers = {
             'Authorization': f'Bearer {global_api_key}',
             'Server-Key': server_key
         }
 
     def _make_get_request(self, endpoint):
         url = f"{self.base_url}/{endpoint}"
-        response = requests.get(url, headers=self.headers)
-        response.raise_for_status()  # Raise exception for non-200 status codes
-        return response.json()
+        try:
+            response = requests.get(url, headers=self.headers)
+            response.raise_for_status()
+            return response.json()
+        except requests.exceptions.RequestException as e:
+            print(f"GET request failed: {e}")
+            return None
 
     def _make_post_request(self, endpoint, data):
         url = f"{self.base_url}/{endpoint}"
-        response = requests.post(url, json=data, headers=self.headers)
-        response.raise_for_status()  # Raise exception for non-200 status codes
-        return response.json()
+        try:
+            response = requests.post(url, json=data, headers=self.headers)
+            response.raise_for_status()
+            return response.json()
+        except requests.exceptions.RequestException as e:
+            print(f"POST request failed: {e}")
+            return None
 
 # Define the methods outside of the class
 def get_server_info(self):
     return self._make_get_request('server')
 
 def get_players(self):
     return self._make_get_request('server/players')
```

