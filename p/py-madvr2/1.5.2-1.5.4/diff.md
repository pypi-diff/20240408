# Comparing `tmp/py_madvr2-1.5.2.tar.gz` & `tmp/py_madvr2-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr2-1.5.2.tar", last modified: Sun Mar 17 01:05:20 2024, max compression
+gzip compressed data, was "py_madvr2-1.5.4.tar", last modified: Sun Apr  7 23:30:55 2024, max compression
```

## Comparing `py_madvr2-1.5.2.tar` & `py_madvr2-1.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-03-17 01:05:20.675053 py_madvr2-1.5.2/
--rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-01-10 23:29:29.000000 py_madvr2-1.5.2/LICENSE
--rw-r--r--   0 ilan       (501) staff       (20)      870 2024-03-17 01:05:20.674833 py_madvr2-1.5.2/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      472 2023-05-14 18:58:32.000000 py_madvr2-1.5.2/README.md
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-03-17 01:05:20.667042 py_madvr2-1.5.2/madvr/
--rw-r--r--   0 ilan       (501) staff       (20)      230 2023-01-10 23:29:29.000000 py_madvr2-1.5.2/madvr/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     3566 2023-07-02 16:13:13.000000 py_madvr2-1.5.2/madvr/commands.py
--rw-r--r--   0 ilan       (501) staff       (20)      242 2023-01-14 01:34:27.000000 py_madvr2-1.5.2/madvr/errors.py
--rw-r--r--   0 ilan       (501) staff       (20)    18423 2024-03-17 01:05:04.000000 py_madvr2-1.5.2/madvr/madvr.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-03-17 01:05:20.674586 py_madvr2-1.5.2/py_madvr2.egg-info/
--rw-r--r--   0 ilan       (501) staff       (20)      870 2024-03-17 01:05:20.000000 py_madvr2-1.5.2/py_madvr2.egg-info/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      262 2024-03-17 01:05:20.000000 py_madvr2-1.5.2/py_madvr2.egg-info/SOURCES.txt
--rw-r--r--   0 ilan       (501) staff       (20)        1 2024-03-17 01:05:20.000000 py_madvr2-1.5.2/py_madvr2.egg-info/dependency_links.txt
--rw-r--r--   0 ilan       (501) staff       (20)       12 2024-03-17 01:05:20.000000 py_madvr2-1.5.2/py_madvr2.egg-info/top_level.txt
--rw-r--r--   0 ilan       (501) staff       (20)       38 2024-03-17 01:05:20.675121 py_madvr2-1.5.2/setup.cfg
--rw-r--r--   0 ilan       (501) staff       (20)      601 2024-03-17 01:05:13.000000 py_madvr2-1.5.2/setup.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-03-17 01:05:20.670119 py_madvr2-1.5.2/tests/
--rw-r--r--   0 ilan       (501) staff       (20)        0 2023-01-10 23:29:29.000000 py_madvr2-1.5.2/tests/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     2159 2024-03-09 17:25:48.000000 py_madvr2-1.5.2/tests/testMadVR.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:30:55.655390 py_madvr2-1.5.4/
+-rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-01-10 23:29:29.000000 py_madvr2-1.5.4/LICENSE
+-rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-07 23:30:55.655198 py_madvr2-1.5.4/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      472 2023-05-14 18:58:32.000000 py_madvr2-1.5.4/README.md
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:30:55.653784 py_madvr2-1.5.4/madvr/
+-rw-r--r--   0 ilan       (501) staff       (20)      230 2023-01-10 23:29:29.000000 py_madvr2-1.5.4/madvr/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     3566 2023-07-02 16:13:13.000000 py_madvr2-1.5.4/madvr/commands.py
+-rw-r--r--   0 ilan       (501) staff       (20)      242 2023-01-14 01:34:27.000000 py_madvr2-1.5.4/madvr/errors.py
+-rw-r--r--   0 ilan       (501) staff       (20)    18430 2024-04-07 23:25:31.000000 py_madvr2-1.5.4/madvr/madvr.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:30:55.655002 py_madvr2-1.5.4/py_madvr2.egg-info/
+-rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-07 23:30:55.000000 py_madvr2-1.5.4/py_madvr2.egg-info/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      262 2024-04-07 23:30:55.000000 py_madvr2-1.5.4/py_madvr2.egg-info/SOURCES.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-07 23:30:55.000000 py_madvr2-1.5.4/py_madvr2.egg-info/dependency_links.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       12 2024-04-07 23:30:55.000000 py_madvr2-1.5.4/py_madvr2.egg-info/top_level.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-07 23:30:55.655432 py_madvr2-1.5.4/setup.cfg
+-rw-r--r--   0 ilan       (501) staff       (20)      601 2024-04-07 22:48:41.000000 py_madvr2-1.5.4/setup.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:30:55.654742 py_madvr2-1.5.4/tests/
+-rw-r--r--   0 ilan       (501) staff       (20)        0 2023-01-10 23:29:29.000000 py_madvr2-1.5.4/tests/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     2159 2024-03-09 17:25:48.000000 py_madvr2-1.5.4/tests/testMadVR.py
```

### Comparing `py_madvr2-1.5.2/LICENSE` & `py_madvr2-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr2-1.5.2/PKG-INFO` & `py_madvr2-1.5.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr2
-Version: 1.5.2
+Version: 1.5.4
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr2-1.5.2/madvr/commands.py` & `py_madvr2-1.5.4/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr2-1.5.2/madvr/madvr.py` & `py_madvr2-1.5.4/madvr/madvr.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,22 +149,22 @@
                 )
                 await asyncio.sleep(2)
                 continue
 
             # includes conn refused
             # backoff to not spam HA
             except asyncio.TimeoutError:
-                self.logger.warning("Connecting timeout, retrying in %s seconds", 2)
+                self.logger.debug("Connecting timeout, retrying in %s seconds", 2)
                 await asyncio.sleep(2)
                 continue
 
             # includes conn refused
             # backoff to not spam HA
             except OSError as err:
-                self.logger.warning("Connecting failed, retrying in %s seconds", 2)
+                self.logger.warning("Connecting failed, retrying in %s seconds: %s", 2, err)
                 self.logger.debug(err)
                 await asyncio.sleep(2)
                 continue
 
     async def send_heartbeat(self, once=False) -> None:
         """
         Send a heartbeat to keep connection open
```

### Comparing `py_madvr2-1.5.2/py_madvr2.egg-info/PKG-INFO` & `py_madvr2-1.5.4/py_madvr2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr2
-Version: 1.5.2
+Version: 1.5.4
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr2-1.5.2/setup.py` & `py_madvr2-1.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr2",
-    version="1.5.2",
+    version="1.5.4",
     author="iloveicedgreentea2",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr2-1.5.2/tests/testMadVR.py` & `py_madvr2-1.5.4/tests/testMadVR.py`

 * *Files identical despite different names*

