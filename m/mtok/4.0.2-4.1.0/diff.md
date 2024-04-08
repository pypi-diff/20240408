# Comparing `tmp/mtok-4.0.2.tar.gz` & `tmp/mtok-4.1.0.tar.gz`

## Comparing `mtok-4.0.2.tar` & `mtok-4.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mtok-4.0.2/.github/workflows/publish-on-pip.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mtok-4.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mtok-4.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mtok-4.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mtok-4.0.2/.idea/mtok.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mtok-4.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 mtok-4.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mtok-4.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-4.0.2/src/mtok/__init__.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 mtok-4.0.2/src/mtok/helpers.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 mtok-4.0.2/src/mtok/mtok.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 mtok-4.0.2/.gitignore
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mtok-4.0.2/README.md
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mtok-4.0.2/pyproject.toml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mtok-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mtok-4.1.0/.github/workflows/publish-on-pip.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mtok-4.1.0/.idea/.gitignore
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mtok-4.1.0/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mtok-4.1.0/.idea/modules.xml
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mtok-4.1.0/.idea/mtok.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mtok-4.1.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 mtok-4.1.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mtok-4.1.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-4.1.0/src/mtok/__init__.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 mtok-4.1.0/src/mtok/helpers.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 mtok-4.1.0/src/mtok/mtok.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 mtok-4.1.0/.gitignore
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mtok-4.1.0/README.md
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mtok-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mtok-4.1.0/PKG-INFO
```

### Comparing `mtok-4.0.2/.github/workflows/publish-on-pip.yml` & `mtok-4.1.0/.github/workflows/publish-on-pip.yml`

 * *Files identical despite different names*

### Comparing `mtok-4.0.2/.idea/inspectionProfiles/Project_Default.xml` & `mtok-4.1.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `mtok-4.0.2/src/mtok/helpers.py` & `mtok-4.1.0/src/mtok/helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from os import environ
 from pathlib import Path
 
 import requests
 
 class Const :
     # local GitHub token absolute filepath $HOME/.gt.json, I assume it is in the home directory
@@ -21,18 +22,14 @@
     tok = get_gt()
 
     trg_repo = 'tokens'
     br = 'main'
     fn = 'main.json'
     url = ret_github_url_for_private_access_to_file(tok , trg_repo , br , fn)
 
-    _hdr = {
-            'User-Agent' : 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
-            }
-
-    r = requests.get(url , headers = _hdr)
-    j = r.json()
+    r = requests.get(url)
+    j = json.loads(r.text)
 
     return j
 
 def ret_github_url_for_private_access_to_file(tok , trg_repo , brnch , fn) :
     return f'https://{c.gu}:{tok}@raw.githubusercontent.com/{c.gu}/{trg_repo}/{brnch}/{fn}'
```

### Comparing `mtok-4.0.2/src/mtok/mtok.py` & `mtok-4.1.0/src/mtok/mtok.py`

 * *Files identical despite different names*

### Comparing `mtok-4.0.2/.gitignore` & `mtok-4.1.0/.gitignore`

 * *Files identical despite different names*

