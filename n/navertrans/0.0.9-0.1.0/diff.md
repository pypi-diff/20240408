# Comparing `tmp/navertrans-0.0.9.tar.gz` & `tmp/navertrans-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navertrans-0.0.9.tar", last modified: Tue Mar 26 09:06:24 2024, max compression
+gzip compressed data, was "navertrans-0.1.0.tar", last modified: Mon Apr  8 07:01:47 2024, max compression
```

## Comparing `navertrans-0.0.9.tar` & `navertrans-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 seongrok.kim   (501) staff       (20)        0 2024-03-26 09:06:24.876457 navertrans-0.0.9/
--rw-r--r--   0 seongrok.kim   (501) staff       (20)    17528 2023-10-27 06:04:22.000000 navertrans-0.0.9/LICENSE
--rw-r--r--   0 seongrok.kim   (501) staff       (20)     3418 2024-03-26 09:06:24.876391 navertrans-0.0.9/PKG-INFO
--rw-r--r--   0 seongrok.kim   (501) staff       (20)     2504 2023-11-06 06:00:48.000000 navertrans-0.0.9/README.md
-drwxr-xr-x   0 seongrok.kim   (501) staff       (20)        0 2024-03-26 09:06:24.875504 navertrans-0.0.9/navertrans/
--rw-r--r--   0 seongrok.kim   (501) staff       (20)       21 2024-03-26 09:05:23.000000 navertrans-0.0.9/navertrans/__init__.py
--rw-r--r--   0 seongrok.kim   (501) staff       (20)       78 2024-01-23 01:42:23.000000 navertrans-0.0.9/navertrans/constants.py
--rw-r--r--   0 seongrok.kim   (501) staff       (20)     5588 2024-03-26 08:55:06.000000 navertrans-0.0.9/navertrans/navertrans.py
--rw-r--r--   0 seongrok.kim   (501) staff       (20)      984 2023-10-25 15:00:56.000000 navertrans-0.0.9/navertrans/response.py
-drwxr-xr-x   0 seongrok.kim   (501) staff       (20)        0 2024-03-26 09:06:24.876129 navertrans-0.0.9/navertrans.egg-info/
--rw-r--r--   0 seongrok.kim   (501) staff       (20)     3418 2024-03-26 09:06:24.000000 navertrans-0.0.9/navertrans.egg-info/PKG-INFO
--rw-r--r--   0 seongrok.kim   (501) staff       (20)      300 2024-03-26 09:06:24.000000 navertrans-0.0.9/navertrans.egg-info/SOURCES.txt
--rw-r--r--   0 seongrok.kim   (501) staff       (20)        1 2024-03-26 09:06:24.000000 navertrans-0.0.9/navertrans.egg-info/dependency_links.txt
--rw-r--r--   0 seongrok.kim   (501) staff       (20)       20 2024-03-26 09:06:24.000000 navertrans-0.0.9/navertrans.egg-info/requires.txt
--rw-r--r--   0 seongrok.kim   (501) staff       (20)       11 2024-03-26 09:06:24.000000 navertrans-0.0.9/navertrans.egg-info/top_level.txt
--rw-r--r--   0 seongrok.kim   (501) staff       (20)       79 2024-03-26 09:06:24.876684 navertrans-0.0.9/setup.cfg
--rw-r--r--   0 seongrok.kim   (501) staff       (20)     2769 2023-10-27 06:37:10.000000 navertrans-0.0.9/setup.py
+drwxr-xr-x   0 seongrok.kim   (501) staff       (20)        0 2024-04-08 07:01:47.051192 navertrans-0.1.0/
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)    17528 2023-10-27 06:04:22.000000 navertrans-0.1.0/LICENSE
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)     3418 2024-04-08 07:01:47.051129 navertrans-0.1.0/PKG-INFO
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)     2504 2023-11-06 06:00:48.000000 navertrans-0.1.0/README.md
+drwxr-xr-x   0 seongrok.kim   (501) staff       (20)        0 2024-04-08 07:01:47.050332 navertrans-0.1.0/navertrans/
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)       21 2024-04-08 07:01:18.000000 navertrans-0.1.0/navertrans/__init__.py
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)       78 2024-01-23 01:42:23.000000 navertrans-0.1.0/navertrans/constants.py
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)     5516 2024-04-08 06:59:17.000000 navertrans-0.1.0/navertrans/navertrans.py
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)      984 2023-10-25 15:00:56.000000 navertrans-0.1.0/navertrans/response.py
+drwxr-xr-x   0 seongrok.kim   (501) staff       (20)        0 2024-04-08 07:01:47.050907 navertrans-0.1.0/navertrans.egg-info/
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)     3418 2024-04-08 07:01:47.000000 navertrans-0.1.0/navertrans.egg-info/PKG-INFO
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)      300 2024-04-08 07:01:47.000000 navertrans-0.1.0/navertrans.egg-info/SOURCES.txt
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)        1 2024-04-08 07:01:47.000000 navertrans-0.1.0/navertrans.egg-info/dependency_links.txt
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)       20 2024-04-08 07:01:47.000000 navertrans-0.1.0/navertrans.egg-info/requires.txt
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)       11 2024-04-08 07:01:47.000000 navertrans-0.1.0/navertrans.egg-info/top_level.txt
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)       79 2024-04-08 07:01:47.051377 navertrans-0.1.0/setup.cfg
+-rw-r--r--   0 seongrok.kim   (501) staff       (20)     2769 2023-10-27 06:37:10.000000 navertrans-0.1.0/setup.py
```

### Comparing `navertrans-0.0.9/LICENSE` & `navertrans-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `navertrans-0.0.9/PKG-INFO` & `navertrans-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navertrans
-Version: 0.0.9
+Version: 0.1.0
 Summary: Thanks for NAVER
 Home-page: https://github.com/LearningnRunning/NaverTrans.git
 Author: learningnRunning
 Author-email: max_sungrok@naver.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `navertrans-0.0.9/README.md` & `navertrans-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `navertrans-0.0.9/navertrans/navertrans.py` & `navertrans-0.1.0/navertrans/navertrans.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,37 +15,29 @@
 from . import __version__
 from .response import Checked
 from .constants import base_url
 
 _agent = requests.Session()
 PY3 = sys.version_info[0] == 3
 cache = TTLCache(maxsize = 10, ttl = 3600)
-
 def read_token():
     try:
         TOKEN = cache.get('PASSPORT_TOKEN')
         return TOKEN
     except KeyError:
         return None
 
 def update_token(agent):
     html = agent.get(url='https://search.naver.com/search.naver?where=nexearch&sm=top_hty&fbm=1&ie=utf8&query=번역기') 
-    try:
-        match = re.search('passportKey=([a-zA-Z0-9]+)', html.text)
-        if match is not None:
-            TOKEN = parse.unquote(match.group(1))
-            cache['PASSPORT_TOKEN'] = TOKEN
-        return TOKEN
-    except UnboundLocalError as e:
-        time.sleep(2)
-        match = re.search('passportKey=([a-zA-Z0-9]+)', html.text)
-        if match is not None:
-            TOKEN = parse.unquote(match.group(1))
-            cache['PASSPORT_TOKEN'] = TOKEN
-        return TOKEN
+
+    match = re.search('passportKey=([a-zA-Z0-9]+)', html.text)
+    if match is not None:
+        TOKEN = parse.unquote(match.group(1))
+        cache['PASSPORT_TOKEN'] = TOKEN
+    return TOKEN
 
 def get_response(TOKEN, text, src_lan, tar_lan):
     
     if TOKEN is None:
         TOKEN = update_token(_agent)
     
     payload = {
@@ -129,23 +121,27 @@
         elif src_lan == "th": # Thai separator
             split_str = "ครับ"
         else:
             split_str = "."
             
         split_txt = src_txt.split(split_str)  # Split the text using 'split_str' as a delimiter
         
+        if len(split_txt) == 1:
+            # Split the text into chunks of 350 characters each
+            split_txt = [src_txt[i:i+300] for i in range(0, len(src_txt), 300)]
+        
+        print('len(split_txt)', len(split_txt))
         # Remove empty strings from the list
         split_txt = [item for item in split_txt if item]
         
         for idx, sentence in enumerate(split_txt):
             # print(sentence)
             if len(current_segment) + len(sentence) < limited_len:
                 current_segment += sentence + split_str
             else:
-      
                 src_txt_list.append(current_segment)
                 current_segment = ""
                 current_segment = sentence + split_str
 
                 if (idx+1) == len(split_txt):
                     src_txt_list.append(current_segment)
```

### Comparing `navertrans-0.0.9/navertrans/response.py` & `navertrans-0.1.0/navertrans/response.py`

 * *Files identical despite different names*

### Comparing `navertrans-0.0.9/navertrans.egg-info/PKG-INFO` & `navertrans-0.1.0/navertrans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navertrans
-Version: 0.0.9
+Version: 0.1.0
 Summary: Thanks for NAVER
 Home-page: https://github.com/LearningnRunning/NaverTrans.git
 Author: learningnRunning
 Author-email: max_sungrok@naver.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `navertrans-0.0.9/setup.py` & `navertrans-0.1.0/setup.py`

 * *Files identical despite different names*

