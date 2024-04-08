# Comparing `tmp/mtok-4.1.1.tar.gz` & `tmp/mtok-4.1.2.tar.gz`

## Comparing `mtok-4.1.1.tar` & `mtok-4.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mtok-4.1.1/.github/workflows/publish-on-pip.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mtok-4.1.1/.idea/.gitignore
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mtok-4.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mtok-4.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mtok-4.1.1/.idea/mtok.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mtok-4.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 mtok-4.1.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mtok-4.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-4.1.1/src/mtok/__init__.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 mtok-4.1.1/src/mtok/helpers.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 mtok-4.1.1/src/mtok/mtok.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 mtok-4.1.1/.gitignore
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mtok-4.1.1/README.md
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mtok-4.1.1/pyproject.toml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mtok-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mtok-4.1.2/.github/workflows/publish-on-pip.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mtok-4.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mtok-4.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mtok-4.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mtok-4.1.2/.idea/mtok.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mtok-4.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 mtok-4.1.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mtok-4.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-4.1.2/src/mtok/__init__.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 mtok-4.1.2/src/mtok/helpers.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 mtok-4.1.2/src/mtok/mtok.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 mtok-4.1.2/.gitignore
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mtok-4.1.2/README.md
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mtok-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mtok-4.1.2/PKG-INFO
```

### Comparing `mtok-4.1.1/.github/workflows/publish-on-pip.yml` & `mtok-4.1.2/.github/workflows/publish-on-pip.yml`

 * *Files identical despite different names*

### Comparing `mtok-4.1.1/.idea/inspectionProfiles/Project_Default.xml` & `mtok-4.1.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `mtok-4.1.1/src/mtok/helpers.py` & `mtok-4.1.2/src/mtok/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,16 +22,18 @@
     tok = get_gt()
 
     trg_repo = 'tokens'
     br = 'main'
     fn = 'main.json'
     url = ret_github_url_for_private_access_to_file(tok , trg_repo , br , fn)
 
-    r = requests.get(url)
+    _hdr = {
+            'Accept' : 'application/vnd.github.v3+json'
+            }
+    r = requests.get(url , headers = _hdr)
     print(r.status_code)
-    print(r.text)
-    j = json.loads(r.text)
+    j = r.json()
 
     return j
 
 def ret_github_url_for_private_access_to_file(tok , trg_repo , brnch , fn) :
     return f'https://{c.gu}:{tok}@raw.githubusercontent.com/{c.gu}/{trg_repo}/{brnch}/{fn}'
```

### Comparing `mtok-4.1.1/src/mtok/mtok.py` & `mtok-4.1.2/src/mtok/mtok.py`

 * *Files identical despite different names*

### Comparing `mtok-4.1.1/.gitignore` & `mtok-4.1.2/.gitignore`

 * *Files identical despite different names*

