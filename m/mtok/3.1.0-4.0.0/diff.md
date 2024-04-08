# Comparing `tmp/mtok-3.1.0.tar.gz` & `tmp/mtok-4.0.0.tar.gz`

## Comparing `mtok-3.1.0.tar` & `mtok-4.0.0.tar`

### file list

```diff
@@ -1,8 +1,15 @@
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mtok-3.1.0/.github/workflows/publish-on-pip.yml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-3.1.0/src/mtok/__init__.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 mtok-3.1.0/src/mtok/helpers.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 mtok-3.1.0/src/mtok/mtok.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 mtok-3.1.0/.gitignore
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mtok-3.1.0/README.md
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mtok-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mtok-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mtok-4.0.0/.github/workflows/publish-on-pip.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mtok-4.0.0/.idea/.gitignore
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mtok-4.0.0/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mtok-4.0.0/.idea/modules.xml
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mtok-4.0.0/.idea/mtok.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mtok-4.0.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 mtok-4.0.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mtok-4.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mtok-4.0.0/src/mtok/__init__.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 mtok-4.0.0/src/mtok/helpers.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 mtok-4.0.0/src/mtok/mtok.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 mtok-4.0.0/.gitignore
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mtok-4.0.0/README.md
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mtok-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mtok-4.0.0/PKG-INFO
```

### Comparing `mtok-3.1.0/.github/workflows/publish-on-pip.yml` & `mtok-4.0.0/.github/workflows/publish-on-pip.yml`

 * *Files identical despite different names*

### Comparing `mtok-3.1.0/src/mtok/mtok.py` & `mtok-4.0.0/src/mtok/mtok.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .helpers import c
-from .helpers import get_all_tokens_fr_tokens_repo
-from .helpers import get_gt
+from mtok.helpers import c
+from mtok.helpers import get_all_tokens_fr_tokens_repo
+from mtok.helpers import get_gt
 
 def get_token(key = None) :
     """ Gets the token by a key from the private tokens repo on my GitHub """
 
     if not c.lg.exists() :
         raise ValueError(f'GitHub Token Not Found.')
```

### Comparing `mtok-3.1.0/.gitignore` & `mtok-4.0.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-## Manually add by me
 venv
-.idea
 
 # General
 .DS_Store
 **/.DS_Store
 .AppleDouble
 .LSOverride
```

