# Comparing `tmp/qaml-0.0.4.tar.gz` & `tmp/qaml-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.4.tar", last modified: Fri Apr  5 17:33:13 2024, max compression
+gzip compressed data, was "qaml-0.0.5.tar", last modified: Mon Apr  8 19:51:41 2024, max compression
```

## Comparing `qaml-0.0.4.tar` & `qaml-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-05 17:33:13.287952 qaml-0.0.4/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.4/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-05 17:33:13.287789 qaml-0.0.4/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       74 2024-04-02 18:28:00.000000 qaml-0.0.4/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-05 17:33:08.000000 qaml-0.0.4/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-05 17:33:13.286951 qaml-0.0.4/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.4/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      780 2024-04-02 21:57:41.000000 qaml-0.0.4/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     8160 2024-04-04 15:32:11.000000 qaml-0.0.4/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-05 17:33:13.287623 qaml-0.0.4/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-05 17:33:13.000000 qaml-0.0.4/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-05 17:33:13.000000 qaml-0.0.4/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-05 17:33:13.000000 qaml-0.0.4/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-05 17:33:13.000000 qaml-0.0.4/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-05 17:33:13.000000 qaml-0.0.4/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-05 17:33:13.000000 qaml-0.0.4/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-05 17:33:13.287987 qaml-0.0.4/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-08 19:51:41.820960 qaml-0.0.5/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.5/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-08 19:51:41.820815 qaml-0.0.5/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       74 2024-04-02 18:28:00.000000 qaml-0.0.5/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-08 19:46:35.000000 qaml-0.0.5/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-08 19:51:41.819912 qaml-0.0.5/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.5/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      852 2024-04-08 19:47:07.000000 qaml-0.0.5/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     8465 2024-04-08 19:50:04.000000 qaml-0.0.5/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-08 19:51:41.820668 qaml-0.0.5/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-08 19:51:41.000000 qaml-0.0.5/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-08 19:51:41.000000 qaml-0.0.5/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-08 19:51:41.000000 qaml-0.0.5/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-08 19:51:41.000000 qaml-0.0.5/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-08 19:51:41.000000 qaml-0.0.5/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-08 19:51:41.000000 qaml-0.0.5/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-08 19:51:41.820990 qaml-0.0.5/setup.cfg
```

### Comparing `qaml-0.0.4/LICENSE` & `qaml-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.4/PKG-INFO` & `qaml-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.4
+Version: 0.0.5
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.4/pyproject.toml` & `qaml-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.4/qaml/__main__.py` & `qaml-0.0.5/qaml/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         while True:
             try:
                 command = input("Enter a command: ")
                 client.execute(command)
             except EOFError:
                 print("")
                 break
+            except Exception as e:
+                print(f"Error: {e}")
     else:
         args_str = " ".join(sys.argv[1:])
         print(f"Running command: {args_str}")
         client.execute(args_str)
 
 if __name__ == "__main__":
     main()
```

### Comparing `qaml-0.0.4/qaml/client.py` & `qaml-0.0.5/qaml/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import base64
 import subprocess
 import json
 from PIL import Image
 from io import BytesIO
 import requests
 
+class QAMLExecException(Exception):
+    pass
+
 class BaseClient:
     def __init__(self, api_key):
         self.api_key = api_key
         self.driver = None
         self.platform = None
         self.screen_size = None
 
@@ -35,14 +38,17 @@
 
     def type_text(self, text):
         raise NotImplementedError
 
     def sleep(self, duration):
         time.sleep(duration)
 
+    def report_error(self, reason):
+        raise QAMLExecException(reason)
+
     def execute(self, script):
         screenshot = self.driver.get_screenshot_as_base64()
         PIL_image = Image.open(BytesIO(base64.b64decode(screenshot)))
         longer_side = max(PIL_image.size)
         aspect_ratio = PIL_image.size[0] / PIL_image.size[1]
         new_size = (960, int(960 / aspect_ratio)) if PIL_image.size[0] == longer_side else (int(960 * aspect_ratio), 960)
         PIL_image = PIL_image.resize(new_size)
@@ -55,15 +61,17 @@
         actions = response.json()
         available_functions = {
             "tap": self.tap_coordinates,
             "drag": self.drag,
             "swipe": self.swipe,
             "scroll": self.scroll,
             "type_text": self.type_text,
-            "sleep": self.sleep
+            "sleep": self.sleep,
+            "report_error": self.report_error,
+            "switch_to_app": self.switch_to_app,
         }
         for action in actions:
             function = available_functions[action["name"]]
             arguments = json.loads(action["arguments"])
             function(**arguments)
 
 class AndroidClient(BaseClient):
@@ -157,14 +165,17 @@
     def scroll(self, direction):
         direction_map = {"up": "down", "down": "up", "left": "right", "right": "left"}
         self.driver.execute_script("mobile: swipe", {"direction": direction_map[direction]})
 
     def type_text(self, text):
         self.driver.find_element(AppiumBy.IOS_PREDICATE, "type == 'XCUIElementTypeApplication'").send_keys(text)
 
+    def switch_to_app(self, bundle_id):
+        self.driver.activate_app(bundle_id)
+
 def Client(api_key, driver=None):
     def get_ios_udid():
         system_profiler_output = subprocess.run(["system_profiler", "SPUSBDataType"], capture_output=True, text=True).stdout
         serial_numbers = re.findall(r'(iPhone|iPad).*?Serial Number: *([^\n]+)', system_profiler_output, re.DOTALL)
 
         if serial_numbers:
             first_serial_number = serial_numbers[0][1].strip()
```

### Comparing `qaml-0.0.4/qaml.egg-info/PKG-INFO` & `qaml-0.0.5/qaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.4
+Version: 0.0.5
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

