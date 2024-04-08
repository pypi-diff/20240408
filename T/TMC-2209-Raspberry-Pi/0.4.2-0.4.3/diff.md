# Comparing `tmp/TMC_2209_Raspberry_Pi-0.4.2.tar.gz` & `tmp/TMC_2209_Raspberry_Pi-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMC_2209_Raspberry_Pi-0.4.2.tar", last modified: Mon Jan 15 18:18:49 2024, max compression
+gzip compressed data, was "TMC_2209_Raspberry_Pi-0.4.3.tar", last modified: Mon Apr  8 18:32:13 2024, max compression
```

## Comparing `TMC_2209_Raspberry_Pi-0.4.2.tar` & `TMC_2209_Raspberry_Pi-0.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:18:49.488268 TMC_2209_Raspberry_Pi-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35305 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-01-15 18:18:49.488268 TMC_2209_Raspberry_Pi-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-15 18:18:49.488268 TMC_2209_Raspberry_Pi-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:18:49.484268 TMC_2209_Raspberry_Pi-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:18:49.488268 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/
--rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/TMC_2209_StepperDriver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_GPIO_board.py
--rw-r--r--   0 runner    (1001) docker     (127)    22093 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_uart.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:18:49.488268 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209_Raspberry_Pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-01-15 18:18:49.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-15 18:18:49.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 18:18:49.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209_Raspberry_Pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-15 18:18:49.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209_Raspberry_Pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-15 18:18:49.000000 TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209_Raspberry_Pi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:18:49.488268 TMC_2209_Raspberry_Pi-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/tests/test_TMC_2209_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/tests/test_TMC_2209_move.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-01-15 18:18:41.000000 TMC_2209_Raspberry_Pi-0.4.2/tests/test_TMC_2209_uart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:13.027114 TMC_2209_Raspberry_Pi-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35305 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-04-08 18:32:13.027114 TMC_2209_Raspberry_Pi-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-08 18:32:13.027114 TMC_2209_Raspberry_Pi-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:13.019114 TMC_2209_Raspberry_Pi-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:13.023114 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/
+-rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/TMC_2209_StepperDriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_GPIO_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22221 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_uart.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:13.027114 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-04-08 18:32:13.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 18:32:13.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:32:13.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 18:32:13.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 18:32:13.000000 TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:13.023114 TMC_2209_Raspberry_Pi-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/tests/test_TMC_2209_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/tests/test_TMC_2209_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-08 18:32:03.000000 TMC_2209_Raspberry_Pi-0.4.3/tests/test_TMC_2209_uart.py
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/LICENSE` & `TMC_2209_Raspberry_Pi-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/PKG-INFO` & `TMC_2209_Raspberry_Pi-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMC_2209_Raspberry_Pi
-Version: 0.4.2
+Version: 0.4.3
 Summary: this is a Python libary to drive a stepper motor with a Trinamic TMC2209 stepper driver and a Raspberry Pi
 Home-page: https://github.com/Chr157i4n/TMC2209_Raspberry_Pi
 Author: Christian Köhlke
 Author-email: christian@koehlke.de
 Project-URL: Bug Tracker, https://github.com/Chr157i4n/TMC2209_Raspberry_Pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/README.md` & `TMC_2209_Raspberry_Pi-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/setup.cfg` & `TMC_2209_Raspberry_Pi-0.4.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TMC_2209_Raspberry_Pi
-version = 0.4.2
+version = 0.4.3
 author = Christian Köhlke
 author_email = christian@koehlke.de
 description = this is a Python libary to drive a stepper motor with a Trinamic TMC2209 stepper driver and a Raspberry Pi
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Chr157i4n/TMC2209_Raspberry_Pi
 project_urls =
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/TMC_2209_StepperDriver.py` & `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/TMC_2209_StepperDriver.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_GPIO_board.py` & `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_GPIO_board.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_comm.py` & `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_comm.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,14 +513,15 @@
     msresdezimal = chopconf & (tmc_reg.msres0 | tmc_reg.msres1 |
                                 tmc_reg.msres2 | tmc_reg.msres3)
 
     msresdezimal = msresdezimal >> 24
     msresdezimal = 8 - msresdezimal
 
     self._msres = int(math.pow(2, msresdezimal))
+    self._steps_per_rev = self._fullsteps_per_rev * self._msres
 
     return self._msres
 
 
 
 def get_microstepping_resolution(self):
     """returns the current native microstep resolution (1-256)
@@ -548,14 +549,15 @@
     chopconf = int(chopconf) & int(4043309055)
     chopconf = chopconf | msresdezimal <<24
 
     self.tmc_logger.log(f"writing {msres} microstep setting", Loglevel.INFO)
     self.tmc_uart.write_reg_check(tmc_reg.CHOPCONF, chopconf)
 
     self._msres = msres
+    self._steps_per_rev = self._fullsteps_per_rev * self._msres
 
     self.set_mstep_resolution_reg_select(True)
 
     return True
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_logger.py` & `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_logger.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_math.py` & `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_math.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_move.py` & `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_move.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_reg.py` & `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_reg.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_test.py` & `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_test.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209/_TMC_2209_uart.py` & `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209/_TMC_2209_uart.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO` & `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMC_2209_Raspberry_Pi
-Version: 0.4.2
+Version: 0.4.3
 Summary: this is a Python libary to drive a stepper motor with a Trinamic TMC2209 stepper driver and a Raspberry Pi
 Home-page: https://github.com/Chr157i4n/TMC2209_Raspberry_Pi
 Author: Christian Köhlke
 Author-email: christian@koehlke.de
 Project-URL: Bug Tracker, https://github.com/Chr157i4n/TMC2209_Raspberry_Pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt` & `TMC_2209_Raspberry_Pi-0.4.3/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/tests/test_TMC_2209_math.py` & `TMC_2209_Raspberry_Pi-0.4.3/tests/test_TMC_2209_math.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/tests/test_TMC_2209_move.py` & `TMC_2209_Raspberry_Pi-0.4.3/tests/test_TMC_2209_move.py`

 * *Files identical despite different names*

### Comparing `TMC_2209_Raspberry_Pi-0.4.2/tests/test_TMC_2209_uart.py` & `TMC_2209_Raspberry_Pi-0.4.3/tests/test_TMC_2209_uart.py`

 * *Files identical despite different names*

