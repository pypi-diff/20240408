# Comparing `tmp/fr-3.0b7.tar.gz` & `tmp/fr-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fr-3.0b7.tar", last modified: Thu Jun 21 23:00:55 2018, max compression
+gzip compressed data, was "fr-3.1.tar", last modified: Fri Apr  5 18:38:00 2024, max compression
```

## Comparing `fr-3.0b7.tar` & `fr-3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2018-06-21 23:00:55.000000 fr-3.0b7/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       38 2018-06-21 23:00:55.000000 fr-3.0b7/setup.cfg
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2018-06-21 23:00:55.000000 fr-3.0b7/fr/
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     8441 2018-06-21 21:11:51.000000 fr-3.0b7/fr/ansi.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     6768 2018-06-21 21:17:17.000000 fr-3.0b7/fr/fr
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1638 2018-06-21 23:00:26.000000 fr-3.0b7/fr/meta.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     5956 2018-06-21 22:59:55.000000 fr-3.0b7/fr/darwin.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2218 2018-06-21 22:59:55.000000 fr-3.0b7/fr/utils.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     7933 2018-06-21 17:52:30.000000 fr-3.0b7/fr/linux.py
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     6312 2018-06-21 21:13:55.000000 fr-3.0b7/fr/windows.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    11920 2018-06-21 21:19:42.000000 fr-3.0b7/fr/__init__.py
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     1037 2018-06-20 20:30:25.000000 fr-3.0b7/setup.py
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2018-06-21 23:00:55.000000 fr-3.0b7/fr.egg-info/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        1 2018-06-21 23:00:55.000000 fr-3.0b7/fr.egg-info/dependency_links.txt
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       25 2018-06-21 23:00:55.000000 fr-3.0b7/fr.egg-info/requires.txt
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      238 2018-06-21 23:00:55.000000 fr-3.0b7/fr.egg-info/SOURCES.txt
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        3 2018-06-21 23:00:55.000000 fr-3.0b7/fr.egg-info/top_level.txt
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     6926 2018-06-21 23:00:55.000000 fr-3.0b7/fr.egg-info/PKG-INFO
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)      164 2013-01-18 22:58:26.000000 fr-3.0b7/fr.cmd
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     6926 2018-06-21 23:00:55.000000 fr-3.0b7/PKG-INFO
+drwxr-xr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2024-04-05 18:38:00.454963 fr-3.1/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    35147 2018-06-07 03:00:56.000000 fr-3.1/LICENSE
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     5467 2024-04-05 18:38:00.453963 fr-3.1/PKG-INFO
+drwxr-xr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2024-04-05 18:38:00.453963 fr-3.1/fr/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    12045 2024-04-05 17:37:04.000000 fr-3.1/fr/__init__.py
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     8441 2018-06-21 21:11:51.000000 fr-3.1/fr/ansi.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     5956 2018-06-21 22:59:55.000000 fr-3.1/fr/darwin.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     6768 2018-06-21 21:17:17.000000 fr-3.1/fr/fr
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     7945 2024-04-05 17:45:44.000000 fr-3.1/fr/linux.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1598 2024-04-05 17:46:42.000000 fr-3.1/fr/meta.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2218 2018-06-21 22:59:55.000000 fr-3.1/fr/utils.py
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     6312 2018-06-21 21:13:55.000000 fr-3.1/fr/windows.py
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)      160 2020-12-29 08:38:08.000000 fr-3.1/fr.cmd
+drwxr-xr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2024-04-05 18:38:00.453963 fr-3.1/fr.egg-info/
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     5467 2024-04-05 18:38:00.000000 fr-3.1/fr.egg-info/PKG-INFO
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      221 2024-04-05 18:38:00.000000 fr-3.1/fr.egg-info/SOURCES.txt
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        1 2024-04-05 18:38:00.000000 fr-3.1/fr.egg-info/dependency_links.txt
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        3 2024-04-05 18:38:00.000000 fr-3.1/fr.egg-info/top_level.txt
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)       38 2024-04-05 18:38:00.454963 fr-3.1/setup.cfg
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     1079 2024-04-05 18:36:59.000000 fr-3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fr-3.0b7/fr/ansi.py` & `fr-3.1/fr/ansi.py`

 * *Files identical despite different names*

### Comparing `fr-3.0b7/fr/fr` & `fr-3.1/fr/fr`

 * *Files identical despite different names*

### Comparing `fr-3.0b7/fr/meta.py` & `fr-3.1/fr/meta.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,29 +4,28 @@
     This module *should not* import anything from the project or third-party
     modules, to avoid dependencies in setup.py or circular import issues.
 '''
 from time import localtime as _localtime
 
 
 pkgname         = 'fr'
-__version__     = version = '3.00b07'
+__version__     = version = '3.01'
 __author__      = authors = ', '.join([
                                 'Mike Miller',
                                 #~ 'and contributors',
                             ])
 copyright       = '© 2005-%s' % _localtime().tm_year
 description     = 'A program to print resources in delicious flavors.'
 email           = ''
 license         = license = 'GPLv3'
 
 # online repo information
 repo_account    = 'mixmastamyk'
 repo_name       = 'fr'
 repo_provider   = 'github.com'
-#~ repo_provider   = 'bitbucket.org'
 repo_url        = 'https://%s/%s/%s' % (repo_provider, repo_account, repo_name)
 trove_classifiers = [
     'Development Status :: 4 - Beta',
     'Environment :: Console',
     'Intended Audience :: Developers',
     'Intended Audience :: System Administrators',
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
```

### Comparing `fr-3.0b7/fr/darwin.py` & `fr-3.1/fr/darwin.py`

 * *Files identical despite different names*

### Comparing `fr-3.0b7/fr/utils.py` & `fr-3.1/fr/utils.py`

 * *Files identical despite different names*

### Comparing `fr-3.0b7/fr/linux.py` & `fr-3.1/fr/linux.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
         disk = DiskInfo()
         dev = basename(device)          # short name
         disk.isnet  = ':' in device     # cheesy but works
         if local_only and disk.isnet:
             continue
         disk.isimg = is_img = dev.startswith('loop')  # could be better
-        is_tmpfs = (device == 'tmpfs')
+        is_tmpfs = device in ('tmpfs', 'devtmpfs')
 
         # lots of junk here, so we throw away most entries
         for selector in selectors:
             if selector in device:
                 if show_all:
                     if is_tmpfs:
                         disk.isram = True
```

### Comparing `fr-3.0b7/fr/windows.py` & `fr-3.1/fr/windows.py`

 * *Files identical despite different names*

### Comparing `fr-3.0b7/fr/__init__.py` & `fr-3.1/fr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,18 @@
     colwidth = opts.colwidth
     # get precision
     if precision is None:
         precision = opts.precision
     fmt = '%%.%sf' % precision
 
     # format with decimal mark, separators
-    result = locale.format(fmt, value, True)
+    try:
+        result = locale.format_string(fmt, value, True)  #  >= Py 3.7
+    except AttributeError:  # olden tymes
+        result = locale.format(fmt, value, True)
 
     if spacing:
         result = '%%%ss' % colwidth % result
 
     if trunc:
         if len(result) > colwidth:   # truncate w/ellipsis
             result = truncstr(result, colwidth)
```

### Comparing `fr-3.0b7/setup.py` & `fr-3.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,31 +10,31 @@
     with open('readme.rst', encoding='utf8') as f:
         long_desc = f.read()
 except IOError:
     long_desc = ''
 
 
 # install helper script for windows?
+extras_require    = {}
 scripts = [join(pkgname, pkgname)]
 if os.name == 'nt':
     scripts.append('fr.cmd')
+    extras_require['win'] = ['winstats', 'colorama']
 
 
 setup(
     name              = pkgname,
     version           = version,
     description       = description,
     author            = authors,
     author_email      = email,
     url               = repo_url,
     download_url      = '',
     license           = license,
     packages          = [pkgname],
     scripts           = scripts,
     python_requires   = '>3.6.0',
-    extras_require    = {
-        'win': ['winstats', 'colorama'],
-    },
+    extras_require    = extras_require,
 
     long_description  = long_desc,
     classifiers       = trove_classifiers,
 )
```

