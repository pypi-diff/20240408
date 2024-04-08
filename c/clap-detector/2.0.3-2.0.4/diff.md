# Comparing `tmp/clap-detector-2.0.3.tar.gz` & `tmp/clap-detector-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clap-detector-2.0.3.tar", last modified: Wed Apr  3 04:38:16 2024, max compression
+gzip compressed data, was "clap-detector-2.0.4.tar", last modified: Mon Apr  8 01:37:20 2024, max compression
```

## Comparing `clap-detector-2.0.3.tar` & `clap-detector-2.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 04:38:16.044336 clap-detector-2.0.3/
--rw-rw-rw-   0        0        0     1090 2024-04-03 02:43:53.000000 clap-detector-2.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3327 2024-04-03 04:38:16.041357 clap-detector-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2850 2024-04-03 04:06:50.000000 clap-detector-2.0.3/README.md
--rw-rw-rw-   0        0        0      138 2024-04-03 03:43:06.000000 clap-detector-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 04:38:16.044336 clap-detector-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      771 2024-04-03 04:37:54.000000 clap-detector-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 04:38:15.994794 clap-detector-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 04:38:16.011785 clap-detector-2.0.3/src/clapDetector/
--rw-rw-rw-   0        0        0       38 2024-04-03 04:29:52.000000 clap-detector-2.0.3/src/clapDetector/__init__.py
--rw-rw-rw-   0        0        0    17669 2024-04-03 03:05:31.000000 clap-detector-2.0.3/src/clapDetector/clapDetector.py
-drwxrwxrwx   0        0        0        0 2024-04-03 04:38:16.038361 clap-detector-2.0.3/src/clap_detector.egg-info/
--rw-rw-rw-   0        0        0     3327 2024-04-03 04:38:15.000000 clap-detector-2.0.3/src/clap_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-04-03 04:38:15.000000 clap-detector-2.0.3/src/clap_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 04:38:15.000000 clap-detector-2.0.3/src/clap_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-03 04:38:15.000000 clap-detector-2.0.3/src/clap_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 01:37:20.536554 clap-detector-2.0.4/
+-rw-rw-rw-   0        0        0     1090 2024-04-03 02:43:53.000000 clap-detector-2.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3409 2024-04-08 01:37:20.533555 clap-detector-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2864 2024-04-03 14:15:32.000000 clap-detector-2.0.4/README.md
+-rw-rw-rw-   0        0        0      138 2024-04-03 03:43:06.000000 clap-detector-2.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 01:37:20.536554 clap-detector-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      858 2024-04-08 01:35:55.000000 clap-detector-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:37:20.482556 clap-detector-2.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 01:37:20.502556 clap-detector-2.0.4/src/clapDetector/
+-rw-rw-rw-   0        0        0       38 2024-04-03 04:29:52.000000 clap-detector-2.0.4/src/clapDetector/__init__.py
+-rw-rw-rw-   0        0        0    17669 2024-04-03 03:05:31.000000 clap-detector-2.0.4/src/clapDetector/clapDetector.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:37:20.531556 clap-detector-2.0.4/src/clap_detector.egg-info/
+-rw-rw-rw-   0        0        0     3409 2024-04-08 01:37:20.000000 clap-detector-2.0.4/src/clap_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2024-04-08 01:37:20.000000 clap-detector-2.0.4/src/clap_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 01:37:20.000000 clap-detector-2.0.4/src/clap_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-08 01:37:20.000000 clap-detector-2.0.4/src/clap_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-08 01:37:20.000000 clap-detector-2.0.4/src/clap_detector.egg-info/top_level.txt
```

### Comparing `clap-detector-2.0.3/LICENSE.txt` & `clap-detector-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clap-detector-2.0.3/PKG-INFO` & `clap-detector-2.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: clap-detector
-Version: 2.0.3
+Version: 2.0.4
 Summary: A clap detector that can detect claps in patterns of single, double, etc.
 Home-page: https://github.com/TzurSoffer/clapDetection
 Author: Tzur Soffer
 Author-email: tzur.soffer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pyaudio
 
 # Clap Detection System
 
 ## Overview
 
-This project implements a clap detection system using an a mic or raw audio data as input. It can detect calp patterns including single and double claps.
+This project implements a clap detection system using an a mic or raw audio data as input. It can detect clap patterns including single and double claps.
 
 ## Features
 
 - Clap pattern detection.
 - Dynamic threshold adjustment for robust clap detection.
 - Bandpass filtering to focus on clap frequencies.
 - Audio recording and saving capabilities.
@@ -46,15 +49,15 @@
    pip install pyaudio numpy scipy
    ```
 
 2. Clone the repository:
 
    ```bash
    git clone https://github.com/TzurSoffer/clapDetection/
-   cd clapDetection/src
+   cd clapDetection/src/clapDetector
    ```
 
 3. Run the clap detection script:
 
    ```bash
    python clapDetector.py
    ```
@@ -63,42 +66,44 @@
 
 - Adjust parameters in the `ClapDetector` class constructor to fine-tune the clap detection system.
 
 ## Usage
 
 1. Create a script that uses this library 
    ```python
-    pyaudio.PyAudio()
-    thresholdBias = 6000
-    lowcut=200               #< increase this to make claps detection more strict
-    highcut=3200             #< decrease this to make claps detection more strict
-    clapDetector = ClapDetector(logLevel=logging.DEBUG, inputDeviceIndex="USB Audio Device")
-    clapDetector.printDeviceInfo()
-    print("""
-          -----------------------------
-          These are the audio devices, find the one you are using and change the variable "inputDeviceIndex" to the the name or index of your audio device. Then restart the program and it should properly get audio data.
-          -----------------------------
-          """)
-    clapDetector.initAudio()
-
-    try:
-        while True:
-            audioData = clapDetector.getAudio()
-
-            result = clapDetector.run(thresholdBias=thresholdBias, lowcut=lowcut, highcut=highcut, audioData=audioData)
-            resultLength = len(result)
-            if resultLength == 2:
-                message = f"Double clap detected! bias {thresholdBias}, lowcut {lowcut}, and highcut {highcut}"
-                clapDetector.saveAudio(folder="./")
-
-    except KeyboardInterrupt:
-        print("Exited gracefully")
-    except Exception as e:
-        print(f"error: {e}")
-        clapDetector.stop()
+   import logging
+   from clapDetector import ClapDetector
+
+   thresholdBias = 6000
+   lowcut=200               #< increase this to make claps detection more strict
+   highcut=3200             #< decrease this to make claps detection more strict
+   clapDetector = ClapDetector(logLevel=logging.DEBUG, inputDeviceIndex="USB Audio Device")
+   clapDetector.printDeviceInfo()
+   print("""
+         -----------------------------
+         These are the audio devices, find the one you are using and change the variable "inputDeviceIndex" to the the name or index of your audio device. Then restart the program and it should properly get audio data.
+         -----------------------------
+         """)
+   clapDetector.initAudio()
+
+   try:
+      while True:
+         audioData = clapDetector.getAudio()
+
+         result = clapDetector.run(thresholdBias=thresholdBias, lowcut=lowcut, highcut=highcut, audioData=audioData)
+         resultLength = len(result)
+         if resultLength == 2:
+               print(f"Double clap detected! bias {thresholdBias}, lowcut {lowcut}, and highcut {highcut}")
+               clapDetector.saveAudio(folder="./")
+
+   except KeyboardInterrupt:
+      print("Exited gracefully")
+   except Exception as e:
+      print(f"error: {e}")
+      clapDetector.stop()
    ```
 
 2. The system will continuously monitor audio input and detect claps.
 
 ## Troubleshooting
 
 - If there are issues with audio input, check the device index in the `ClapDetector` constructor.
```

### Comparing `clap-detector-2.0.3/README.md` & `clap-detector-2.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Clap Detection System
 
 ## Overview
 
-This project implements a clap detection system using an a mic or raw audio data as input. It can detect calp patterns including single and double claps.
+This project implements a clap detection system using an a mic or raw audio data as input. It can detect clap patterns including single and double claps.
 
 ## Features
 
 - Clap pattern detection.
 - Dynamic threshold adjustment for robust clap detection.
 - Bandpass filtering to focus on clap frequencies.
 - Audio recording and saving capabilities.
@@ -33,15 +33,15 @@
    pip install pyaudio numpy scipy
    ```
 
 2. Clone the repository:
 
    ```bash
    git clone https://github.com/TzurSoffer/clapDetection/
-   cd clapDetection/src
+   cd clapDetection/src/clapDetector
    ```
 
 3. Run the clap detection script:
 
    ```bash
    python clapDetector.py
    ```
@@ -50,42 +50,44 @@
 
 - Adjust parameters in the `ClapDetector` class constructor to fine-tune the clap detection system.
 
 ## Usage
 
 1. Create a script that uses this library 
    ```python
-    pyaudio.PyAudio()
-    thresholdBias = 6000
-    lowcut=200               #< increase this to make claps detection more strict
-    highcut=3200             #< decrease this to make claps detection more strict
-    clapDetector = ClapDetector(logLevel=logging.DEBUG, inputDeviceIndex="USB Audio Device")
-    clapDetector.printDeviceInfo()
-    print("""
-          -----------------------------
-          These are the audio devices, find the one you are using and change the variable "inputDeviceIndex" to the the name or index of your audio device. Then restart the program and it should properly get audio data.
-          -----------------------------
-          """)
-    clapDetector.initAudio()
-
-    try:
-        while True:
-            audioData = clapDetector.getAudio()
-
-            result = clapDetector.run(thresholdBias=thresholdBias, lowcut=lowcut, highcut=highcut, audioData=audioData)
-            resultLength = len(result)
-            if resultLength == 2:
-                message = f"Double clap detected! bias {thresholdBias}, lowcut {lowcut}, and highcut {highcut}"
-                clapDetector.saveAudio(folder="./")
-
-    except KeyboardInterrupt:
-        print("Exited gracefully")
-    except Exception as e:
-        print(f"error: {e}")
-        clapDetector.stop()
+   import logging
+   from clapDetector import ClapDetector
+
+   thresholdBias = 6000
+   lowcut=200               #< increase this to make claps detection more strict
+   highcut=3200             #< decrease this to make claps detection more strict
+   clapDetector = ClapDetector(logLevel=logging.DEBUG, inputDeviceIndex="USB Audio Device")
+   clapDetector.printDeviceInfo()
+   print("""
+         -----------------------------
+         These are the audio devices, find the one you are using and change the variable "inputDeviceIndex" to the the name or index of your audio device. Then restart the program and it should properly get audio data.
+         -----------------------------
+         """)
+   clapDetector.initAudio()
+
+   try:
+      while True:
+         audioData = clapDetector.getAudio()
+
+         result = clapDetector.run(thresholdBias=thresholdBias, lowcut=lowcut, highcut=highcut, audioData=audioData)
+         resultLength = len(result)
+         if resultLength == 2:
+               print(f"Double clap detected! bias {thresholdBias}, lowcut {lowcut}, and highcut {highcut}")
+               clapDetector.saveAudio(folder="./")
+
+   except KeyboardInterrupt:
+      print("Exited gracefully")
+   except Exception as e:
+      print(f"error: {e}")
+      clapDetector.stop()
    ```
 
 2. The system will continuously monitor audio input and detect claps.
 
 ## Troubleshooting
 
 - If there are issues with audio input, check the device index in the `ClapDetector` constructor.
```

### Comparing `clap-detector-2.0.3/setup.py` & `clap-detector-2.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "clap-detector",
-    version = "2.0.3",
+    version = "2.0.4",
     author = "Tzur Soffer",
     author_email = "tzur.soffer@gmail.com",
     description = "A clap detector that can detect claps in patterns of single, double, etc.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/TzurSoffer/clapDetection",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    install_requires=[
+        "numpy",
+        "scipy",
+        "pyaudio"
+    ],
     package_dir = {"": "src"},
     packages = setuptools.find_packages(where="src")
 )
```

### Comparing `clap-detector-2.0.3/src/clapDetector/clapDetector.py` & `clap-detector-2.0.4/src/clapDetector/clapDetector.py`

 * *Files identical despite different names*

### Comparing `clap-detector-2.0.3/src/clap_detector.egg-info/PKG-INFO` & `clap-detector-2.0.4/src/clap_detector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: clap-detector
-Version: 2.0.3
+Version: 2.0.4
 Summary: A clap detector that can detect claps in patterns of single, double, etc.
 Home-page: https://github.com/TzurSoffer/clapDetection
 Author: Tzur Soffer
 Author-email: tzur.soffer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pyaudio
 
 # Clap Detection System
 
 ## Overview
 
-This project implements a clap detection system using an a mic or raw audio data as input. It can detect calp patterns including single and double claps.
+This project implements a clap detection system using an a mic or raw audio data as input. It can detect clap patterns including single and double claps.
 
 ## Features
 
 - Clap pattern detection.
 - Dynamic threshold adjustment for robust clap detection.
 - Bandpass filtering to focus on clap frequencies.
 - Audio recording and saving capabilities.
@@ -46,15 +49,15 @@
    pip install pyaudio numpy scipy
    ```
 
 2. Clone the repository:
 
    ```bash
    git clone https://github.com/TzurSoffer/clapDetection/
-   cd clapDetection/src
+   cd clapDetection/src/clapDetector
    ```
 
 3. Run the clap detection script:
 
    ```bash
    python clapDetector.py
    ```
@@ -63,42 +66,44 @@
 
 - Adjust parameters in the `ClapDetector` class constructor to fine-tune the clap detection system.
 
 ## Usage
 
 1. Create a script that uses this library 
    ```python
-    pyaudio.PyAudio()
-    thresholdBias = 6000
-    lowcut=200               #< increase this to make claps detection more strict
-    highcut=3200             #< decrease this to make claps detection more strict
-    clapDetector = ClapDetector(logLevel=logging.DEBUG, inputDeviceIndex="USB Audio Device")
-    clapDetector.printDeviceInfo()
-    print("""
-          -----------------------------
-          These are the audio devices, find the one you are using and change the variable "inputDeviceIndex" to the the name or index of your audio device. Then restart the program and it should properly get audio data.
-          -----------------------------
-          """)
-    clapDetector.initAudio()
-
-    try:
-        while True:
-            audioData = clapDetector.getAudio()
-
-            result = clapDetector.run(thresholdBias=thresholdBias, lowcut=lowcut, highcut=highcut, audioData=audioData)
-            resultLength = len(result)
-            if resultLength == 2:
-                message = f"Double clap detected! bias {thresholdBias}, lowcut {lowcut}, and highcut {highcut}"
-                clapDetector.saveAudio(folder="./")
-
-    except KeyboardInterrupt:
-        print("Exited gracefully")
-    except Exception as e:
-        print(f"error: {e}")
-        clapDetector.stop()
+   import logging
+   from clapDetector import ClapDetector
+
+   thresholdBias = 6000
+   lowcut=200               #< increase this to make claps detection more strict
+   highcut=3200             #< decrease this to make claps detection more strict
+   clapDetector = ClapDetector(logLevel=logging.DEBUG, inputDeviceIndex="USB Audio Device")
+   clapDetector.printDeviceInfo()
+   print("""
+         -----------------------------
+         These are the audio devices, find the one you are using and change the variable "inputDeviceIndex" to the the name or index of your audio device. Then restart the program and it should properly get audio data.
+         -----------------------------
+         """)
+   clapDetector.initAudio()
+
+   try:
+      while True:
+         audioData = clapDetector.getAudio()
+
+         result = clapDetector.run(thresholdBias=thresholdBias, lowcut=lowcut, highcut=highcut, audioData=audioData)
+         resultLength = len(result)
+         if resultLength == 2:
+               print(f"Double clap detected! bias {thresholdBias}, lowcut {lowcut}, and highcut {highcut}")
+               clapDetector.saveAudio(folder="./")
+
+   except KeyboardInterrupt:
+      print("Exited gracefully")
+   except Exception as e:
+      print(f"error: {e}")
+      clapDetector.stop()
    ```
 
 2. The system will continuously monitor audio input and detect claps.
 
 ## Troubleshooting
 
 - If there are issues with audio input, check the device index in the `ClapDetector` constructor.
```

