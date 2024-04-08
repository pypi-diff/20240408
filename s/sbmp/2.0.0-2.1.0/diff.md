# Comparing `tmp/sbmp-2.0.0.tar.gz` & `tmp/sbmp-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmp-2.0.0.tar", last modified: Thu Apr  4 19:33:47 2024, max compression
+gzip compressed data, was "sbmp-2.1.0.tar", last modified: Mon Apr  8 13:44:25 2024, max compression
```

## Comparing `sbmp-2.0.0.tar` & `sbmp-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-04 19:33:47.962381 sbmp-2.0.0/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)     1075 2024-01-08 11:37:56.000000 sbmp-2.0.0/LICENSE
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      487 2024-04-04 19:33:47.962199 sbmp-2.0.0/PKG-INFO
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        6 2024-01-08 11:39:16.000000 sbmp-2.0.0/README.txt
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-04 19:33:47.961325 sbmp-2.0.0/sbmp/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)       18 2024-01-08 11:36:04.000000 sbmp-2.0.0/sbmp/__init__.py
--rw-------   0 jainambarbhaya   (501) staff       (20)    14742 2024-04-04 18:56:13.000000 sbmp-2.0.0/sbmp/iss.py
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-04 19:33:47.962041 sbmp-2.0.0/sbmp.egg-info/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      487 2024-04-04 19:33:47.000000 sbmp-2.0.0/sbmp.egg-info/PKG-INFO
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      168 2024-04-04 19:33:47.000000 sbmp-2.0.0/sbmp.egg-info/SOURCES.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        1 2024-04-04 19:33:47.000000 sbmp-2.0.0/sbmp.egg-info/dependency_links.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        5 2024-04-04 19:33:47.000000 sbmp-2.0.0/sbmp.egg-info/top_level.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)       38 2024-04-04 19:33:47.962426 sbmp-2.0.0/setup.cfg
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      627 2024-04-04 19:30:57.000000 sbmp-2.0.0/setup.py
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-08 13:44:25.264203 sbmp-2.1.0/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)     1075 2024-01-08 11:37:56.000000 sbmp-2.1.0/LICENSE
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      487 2024-04-08 13:44:25.264006 sbmp-2.1.0/PKG-INFO
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        6 2024-01-08 11:39:16.000000 sbmp-2.1.0/README.txt
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-08 13:44:25.263092 sbmp-2.1.0/sbmp/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)       18 2024-01-08 11:36:04.000000 sbmp-2.1.0/sbmp/__init__.py
+-rw-------   0 jainambarbhaya   (501) staff       (20)    14745 2024-04-08 13:42:39.000000 sbmp-2.1.0/sbmp/iss.py
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-08 13:44:25.263808 sbmp-2.1.0/sbmp.egg-info/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      487 2024-04-08 13:44:25.000000 sbmp-2.1.0/sbmp.egg-info/PKG-INFO
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      168 2024-04-08 13:44:25.000000 sbmp-2.1.0/sbmp.egg-info/SOURCES.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        1 2024-04-08 13:44:25.000000 sbmp-2.1.0/sbmp.egg-info/dependency_links.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        5 2024-04-08 13:44:25.000000 sbmp-2.1.0/sbmp.egg-info/top_level.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)       38 2024-04-08 13:44:25.264240 sbmp-2.1.0/setup.cfg
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      627 2024-04-08 13:44:08.000000 sbmp-2.1.0/setup.py
```

### Comparing `sbmp-2.0.0/LICENSE` & `sbmp-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sbmp-2.0.0/sbmp/iss.py` & `sbmp-2.1.0/sbmp/iss.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,13 +611,13 @@
     "diffie_hellman.cpp": diffie_hellman,
     "rsa.cpp": rsa,
     'des.cpp': des,
     'keylogger.cpp': keylogger,
     'rainbow_table.cpp': rainbow_table
 }
 
-def iss_():
+def codes__():
     for file,code in iss_codes.items():
         print(file)
     filename = input("Enter filename: ")
     with open(filename, 'w') as f:
         f.write(iss_codes[filename])
```

### Comparing `sbmp-2.0.0/setup.py` & `sbmp-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='sbmp',
-  version='2.0.0',
+  version='2.1.0',
   description='SBMP',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Jainam Barbhaya',
   author_email='jainambarbhaya1509@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

