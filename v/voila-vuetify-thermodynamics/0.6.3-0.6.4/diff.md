# Comparing `tmp/voila-vuetify-thermodynamics-0.6.3.tar.gz` & `tmp/voila-vuetify-thermodynamics-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-vuetify-thermodynamics-0.6.3.tar", last modified: Sun Apr  7 18:36:43 2024, max compression
+gzip compressed data, was "voila-vuetify-thermodynamics-0.6.4.tar", last modified: Mon Apr  8 20:52:12 2024, max compression
```

## Comparing `voila-vuetify-thermodynamics-0.6.3.tar` & `voila-vuetify-thermodynamics-0.6.4.tar`

### file list

```diff
@@ -1,13 +1,30 @@
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-07 18:36:43.066551 voila-vuetify-thermodynamics-0.6.3/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1545 2024-04-07 17:10:33.000000 voila-vuetify-thermodynamics-0.6.3/LICENSE
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       16 2024-04-07 17:10:33.000000 voila-vuetify-thermodynamics-0.6.3/MANIFEST.in
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      322 2024-04-07 18:36:43.066452 voila-vuetify-thermodynamics-0.6.3/PKG-INFO
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1574 2024-04-07 17:10:33.000000 voila-vuetify-thermodynamics-0.6.3/README.md
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      101 2024-04-07 18:36:43.066876 voila-vuetify-thermodynamics-0.6.3/setup.cfg
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     3340 2024-04-07 18:36:10.000000 voila-vuetify-thermodynamics-0.6.3/setup.py
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-07 18:36:43.066136 voila-vuetify-thermodynamics-0.6.3/voila_vuetify_thermodynamics.egg-info/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      322 2024-04-07 18:36:43.000000 voila-vuetify-thermodynamics-0.6.3/voila_vuetify_thermodynamics.egg-info/PKG-INFO
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      307 2024-04-07 18:36:43.000000 voila-vuetify-thermodynamics-0.6.3/voila_vuetify_thermodynamics.egg-info/SOURCES.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)        1 2024-04-07 18:36:43.000000 voila-vuetify-thermodynamics-0.6.3/voila_vuetify_thermodynamics.egg-info/dependency_links.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       18 2024-04-07 18:36:43.000000 voila-vuetify-thermodynamics-0.6.3/voila_vuetify_thermodynamics.egg-info/requires.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)        8 2024-04-07 18:36:43.000000 voila-vuetify-thermodynamics-0.6.3/voila_vuetify_thermodynamics.egg-info/top_level.txt
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.735186 voila-vuetify-thermodynamics-0.6.4/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1545 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/LICENSE
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       68 2024-04-08 20:50:57.000000 voila-vuetify-thermodynamics-0.6.4/MANIFEST.in
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      297 2024-04-08 20:52:12.735090 voila-vuetify-thermodynamics-0.6.4/PKG-INFO
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1574 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/README.md
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      101 2024-04-08 20:52:12.735430 voila-vuetify-thermodynamics-0.6.4/setup.cfg
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     3458 2024-04-08 20:52:04.000000 voila-vuetify-thermodynamics-0.6.4/setup.py
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.729774 voila-vuetify-thermodynamics-0.6.4/share/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.730122 voila-vuetify-thermodynamics-0.6.4/share/jupyter/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.729889 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.730032 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.733272 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     7797 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/ansi.js
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1434 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/app.html
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       25 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/conf.json
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     3179 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/index.html.j2
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     7280 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-base/util.js
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.733832 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-default/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     6381 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-default/app.html
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       33 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/nbconvert/templates/vuetify-default/conf.json
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.730182 voila-vuetify-thermodynamics-0.6.4/share/jupyter/voila/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.730244 voila-vuetify-thermodynamics-0.6.4/share/jupyter/voila/templates/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.734029 voila-vuetify-thermodynamics-0.6.4/share/jupyter/voila/templates/vuetify-base/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1757 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.4/share/jupyter/voila/templates/vuetify-base/index.html.j2
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-08 20:52:12.734855 voila-vuetify-thermodynamics-0.6.4/voila_vuetify_thermodynamics.egg-info/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      297 2024-04-08 20:52:12.000000 voila-vuetify-thermodynamics-0.6.4/voila_vuetify_thermodynamics.egg-info/PKG-INFO
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      767 2024-04-08 20:52:12.000000 voila-vuetify-thermodynamics-0.6.4/voila_vuetify_thermodynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)        1 2024-04-08 20:52:12.000000 voila-vuetify-thermodynamics-0.6.4/voila_vuetify_thermodynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       31 2024-04-08 20:52:12.000000 voila-vuetify-thermodynamics-0.6.4/voila_vuetify_thermodynamics.egg-info/requires.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)        6 2024-04-08 20:52:12.000000 voila-vuetify-thermodynamics-0.6.4/voila_vuetify_thermodynamics.egg-info/top_level.txt
```

### Comparing `voila-vuetify-thermodynamics-0.6.3/LICENSE` & `voila-vuetify-thermodynamics-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.3/README.md` & `voila-vuetify-thermodynamics-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.3/setup.py` & `voila-vuetify-thermodynamics-0.6.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 import sys
 import os
 from setuptools import setup
 from setuptools.command.develop import develop
 import contextlib
+#from jupyter_core.paths import get_home_dir
 
 pjoin = os.path.join
 
 
 # these are based on jupyter_core.paths
 def jupyter_config_dir():
     """Get the Jupyter config directory for this platform and user.
 
     Returns JUPYTER_CONFIG_DIR if defined, else ~/.jupyter
     """
 
     env = os.environ
     home_dir = get_home_dir()
 
+    stop = 0
+
     if env.get('JUPYTER_NO_CONFIG'):
         return _mkdtemp_once('jupyter-clean-cfg')
 
     if env.get('JUPYTER_CONFIG_DIR'):
         return env['JUPYTER_CONFIG_DIR']
 
     return pjoin(home_dir, '.jupyter')
 
 
+
+stop = 0
+
 def user_dir():
     homedir = os.path.expanduser('~')
     # Next line will make things work even when /home/ is a symlink to
     # /usr/home as it is on FreeBSD, for example
     homedir = os.path.realpath(homedir)
     if sys.platform == 'darwin':
         return os.path.join(homedir, 'Library', 'Jupyter')
@@ -45,18 +51,18 @@
         if not xdg:
             xdg = pjoin(home, '.local', 'share')
         return pjoin(xdg, 'jupyter')
 
 
 class DevelopCmd(develop):
     prefix_targets = [
-        ("nbconvert/templates", 'vuetify-base-thermodynamics'),
-        ("nbconvert/templates", 'vuetify-default-thermodynamics'),
-        ("voila/templates", 'vuetify-base-thermodynamics'),
-        ("voila/templates", 'vuetify-default-thermodynamics'),
+        ("nbconvert/templates", 'vuetify-base'),
+        ("nbconvert/templates", 'vuetify-default'),
+        ("voila/templates", 'vuetify-base'),
+        ("voila/templates", 'vuetify-default'),
     ]
     def run(self):
         target_dir = os.path.join(sys.prefix, 'share', 'jupyter')
         if '--user' in sys.prefix:  # TODO: is there a better way to find out?
             target_dir = user_dir()
         target_dir = os.path.join(target_dir)
 
@@ -69,38 +75,42 @@
             rel_source = os.path.relpath(os.path.abspath(source), os.path.abspath(target_subdir))
             try:
                 os.remove(target)
             except:
                 pass
             print(rel_source, '->', target)
             os.symlink(rel_source, target)
+            print(f"***** Creating symlink: {rel_source} -> {target}")
 
         super(DevelopCmd, self).run()
 
 
 # WARNING: all files generates during setup.py will not end up in the source distribution
 data_files = []
 # Add all the templates
 for (dirpath, dirnames, filenames) in os.walk('share/jupyter/'):
     if filenames:
         data_files.append((dirpath, [os.path.join(dirpath, filename) for filename in filenames]))
 
 
+print("Setup.py is being executed")
+
 setup(
     name='voila-vuetify-thermodynamics',
-    version="0.6.3",
+    version="0.6.4",
     description="A vuetify template for Voila",
     data_files=data_files,
-    install_requires=['voila>=0.2.0,<0.5'],
+    install_requires=['voila>=0.2.0,<0.5', 'jupyter_core'],
     include_package_data=True,
-    author='Lukas Bongartz',
-    url='https://github.com/lukasbongartz/voila-vuetify-thermodynamics',
+    author='Mario Buikhuizen, Maarten Breddels',
     keywords=[
         'ipython',
         'jupyter',
         'widgets',
         'voila'
     ],
     cmdclass={
          'develop': DevelopCmd,
    },
 )
+
+print("Setup.py execution finished")
```

