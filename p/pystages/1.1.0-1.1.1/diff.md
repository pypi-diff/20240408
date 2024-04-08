# Comparing `tmp/pystages-1.1.tar.gz` & `tmp/pystages-1.1.1.tar.gz`

## Comparing `pystages-1.1.tar` & `pystages-1.1.1.tar`

### file list

```diff
@@ -1,35 +1,42 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pystages-1.1.0/.readthedocs.yml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pystages-1.1.0/requirements.txt
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pystages-1.1.0/.github/workflows/black.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/Makefile
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/api.rst
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/api_cnc.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/api_corvus.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/api_m3fs.rst
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/api_smc100.rst
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/api_tic.rst
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/autofocus.rst
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/conf.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/index.rst
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/logo.png
--rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/logo.svg
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/make.bat
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/troubleshooting.rst
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pystages-1.1.0/docs/vectors.rst
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 pystages-1.1.0/pystages/__init__.py
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 pystages-1.1.0/pystages/autofocus.py
--rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 pystages-1.1.0/pystages/cncrouter.py
--rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 pystages-1.1.0/pystages/corvus.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pystages-1.1.0/pystages/exceptions.py
--rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 pystages-1.1.0/pystages/grbl.py
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 pystages-1.1.0/pystages/m3fs.py
--rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 pystages-1.1.0/pystages/smc100.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pystages-1.1.0/pystages/stage.py
--rw-r--r--   0        0        0     7778 2020-02-02 00:00:00.000000 pystages-1.1.0/pystages/tic.py
--rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 pystages-1.1.0/pystages/vector.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pystages-1.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pystages-1.1.0/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 pystages-1.1.0/COPYING.LESSER
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pystages-1.1.0/README.md
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 pystages-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pystages-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pystages-1.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pystages-1.1.1/requirements.txt
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pystages-1.1.1/.github/workflows/black.yml
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pystages-1.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/api.rst
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/api_cnc.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/api_corvus.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/api_m3fs.rst
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/api_smc100.rst
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/api_tic.rst
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/autofocus.rst
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/conf.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/gui.md
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/index.rst
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/logo.png
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/logo.svg
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/make.bat
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/troubleshooting.rst
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pystages-1.1.1/docs/vectors.rst
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/__init__.py
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/autofocus.py
+-rw-r--r--   0        0        0    12280 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/cncrouter.py
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/corvus.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/exceptions.py
+-rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/grbl.py
+-rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/m3fs.py
+-rw-r--r--   0        0        0    15678 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/smc100.py
+-rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/stage.py
+-rw-r--r--   0        0        0     8234 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/tic.py
+-rw-r--r--   0        0        0     9289 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/vector.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/gui/__init__.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/gui/__main__.py
+-rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/gui/gui.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pystages-1.1.1/pystages/gui/util.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pystages-1.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pystages-1.1.1/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 pystages-1.1.1/COPYING.LESSER
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 pystages-1.1.1/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pystages-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 pystages-1.1.1/PKG-INFO
```

### Comparing `pystages-1.1.0/docs/Makefile` & `pystages-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pystages-1.1.0/docs/autofocus.rst` & `pystages-1.1.1/docs/autofocus.rst`

 * *Files identical despite different names*

### Comparing `pystages-1.1.0/docs/conf.py` & `pystages-1.1.1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,35 +6,38 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
-# import os
-# import sys
-# sys.path.insert(0, os.path.abspath('.'))
+
+import sys
+import os
+
+# Add path for autodoc
+sys.path.insert(0, os.path.abspath(".."))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "pystages"
-copyright = "2022, Olivier Hériveaux, Manuel San Pedro, Michaël Mouchous"
+copyright = "2024, Olivier Hériveaux, Manuel San Pedro, Michaël Mouchous"
 author = "Olivier Hériveaux, Manuel San Pedro, Michaël Mouchous"
 
 # The full version, including alpha/beta/rc tags
-release = "1.1"
+release = "1.1.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ["sphinx.ext.autodoc"]
+extensions = ["sphinx.ext.autodoc", "myst_parser"]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
@@ -50,7 +53,12 @@
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = []
 
 html_logo = "logo.png"
+
+source_suffix = {
+    ".rst": "restructuredtext",
+    ".md": "markdown",
+}
```

### Comparing `pystages-1.1.0/docs/index.rst` & `pystages-1.1.1/docs/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-.. pystages documentation master file, created by
-   sphinx-quickstart on Tue Jul  7 15:03:18 2020.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
-
 Welcome to pystages's documentation!
 ====================================
 
 PyStages is a Python 3 library for controlling motorized stages which have a
 motion controller. It has been designed for microscopy test benches automation.
 
 The following motion controllers are currently supported (only the main
@@ -20,21 +15,22 @@
   (:class:`pystages.cncrouter.CNCRouter`)
 
 The library also provides helper classes for basic vector manipulation
 (:class:`pystages.Vector`) and autofocus calculation
 (:class:`pystages.Autofocus`).
 
 .. toctree::
-   :maxdepth: 2
-   :caption: Contents:
+  :maxdepth: 2
+  :caption: Contents:
 
-   Vectors <vectors.rst>
-   Autofocus <autofocus.rst>
-   Python API <api.rst>
-   Troubleshooting <troubleshooting.rst>
+  Vectors <vectors.rst>
+  Autofocus <autofocus.rst>
+  Python API <api.rst>
+  GUI <gui.md>
+  Troubleshooting <troubleshooting.rst>
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `pystages-1.1.0/docs/logo.png` & `pystages-1.1.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `pystages-1.1.0/docs/logo.svg` & `pystages-1.1.1/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `pystages-1.1.0/docs/make.bat` & `pystages-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pystages-1.1.0/docs/vectors.rst` & `pystages-1.1.1/docs/vectors.rst`

 * *Files identical despite different names*

### Comparing `pystages-1.1.0/pystages/autofocus.py` & `pystages-1.1.1/pystages/autofocus.py`

 * *Files identical despite different names*

### Comparing `pystages-1.1.0/pystages/cncrouter.py` & `pystages-1.1.1/pystages/cncrouter.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,76 +3,91 @@
 # pystages is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# along with this program. If not, see <https://www.gnu.org/licenses/>.
 #
 # Values and descriptions of commands and error codes has been taken from GRBL Github repository
 # https://github.com/grbl/grbl
 # and the instruction manual of the CNC 3018 PRO
 # https://drive.google.com/file/d/1yQH9gtO8lWbE-K0dff8g9zq_1xOB57x7
 #
-# Copyright 2018-2022 Ledger SAS, written by Michaël Mouchous
+# Copyright 2018-2023 Ledger SAS, written by Michaël Mouchous
 
-import serial
+import serial.serialutil
 import time
 from typing import Optional, Tuple, List, Union
 from .exceptions import ConnectionFailure
 from .vector import Vector
 from enum import Enum
 from .grbl import GRBLSetting, InvertMask, StatusReportMask
 from .stage import Stage
 
 
-class CNCStatus(Enum):
+class CNCStatus(str, Enum):
+    """
+    Possible statuses that the CNC can report.
+    """
+
     IDLE = "Idle"
     RUN = "Run"
     HOLD = "Hold"
     DOOR = "Door"
     HOME = "Home"
     ALARM = "Alarm"
     CHECK = "Check"
 
 
+class CNCError(Exception):
+    """Exception raised when a specific error is detected by the CNC"""
+
+    def __init__(self, message: str, cncstatus: CNCStatus):
+        super().__init__(message)
+        self.cncstatus = cncstatus
+
+
 class CNCRouter(Stage):
     """
     Class to command CNC routers.
     """
 
-    def __init__(self, dev: str, reset_wait_time=2.0):
+    def __init__(self, dev: Optional[str] = None, reset_wait_time=2.0):
         """
         Open serial device to connect to the CNC routers. Raise a
         ConnectionFailure exception if the serial device could not be open.
 
-        :param dev: Serial device. For instance `'/dev/ttyUSB0'`.
+        :param dev: Serial device. For instance `'/dev/ttyUSB0'`. If not provided, try
+            to discover a suitable device according to device vendor and product IDs
         :param reset_wait_time: Depending on the state of the stage, it can take some time for
-         GRBL to reset. This parameter makes the wait time to be tuned, by giving a time in seconds.
+            GRBL to reset. This parameter makes the wait time to be tuned, by giving a time in seconds.
         """
+
         super().__init__(num_axis=3)
         self.reset_wait_time = reset_wait_time
         try:
+            dev = dev or self.find_device(pid=0x7523, vid=0x1A86)
             self.serial = serial.Serial(dev, 115200, timeout=1)
         except serial.serialutil.SerialException as e:
             raise ConnectionFailure() from e
         self.reset_grbl()
 
     def reset_grbl(self, wait_time: Optional[float] = None) -> bool:
         """
         Sends a CTRL+X control to reset the GRBL
 
         :return: True if the GRBL sent the correct prompt at the end of the reset
         :param wait_time: Depending on the state of the stage, it can take some time for GRBL to
-         reset. This parameter makes the wait time to be tuned, by giving a time in seconds.
+            reset. This parameter makes the wait time to be tuned, by giving a time in seconds.
         """
         if wait_time is None:
             wait_time = self.reset_wait_time
         self.serial.flush()
         self.send("\030", eol="")
         time.sleep(wait_time)
         self.send("")
@@ -159,29 +174,42 @@
 
     def get_current_status(self) -> Optional[Tuple[CNCStatus, dict]]:
         """
         Sending '?' character permits to get the status of the CNC
         router
 
         :return: A tuple containing the status and a dictionary of all other parameters in the
-         output of the command.
+            output of the command.
         """
+
         self.send("?", eol="")
         status = self.receive()
 
+        # Retry, sometimes it does not respond
+        if status == "":
+            self.send("?", eol="")
+            status = self.receive()
+
         # Sometimes, the CNC returns 'ok' and the actual response is following.
         while status == "ok":
             status = self.receive()
 
         # In the case there has been a communication error
         if status is None:
             return None
 
-        # The output
+        # The possible outputs
         # '<Idle|MPos:1.000,3.000,4.000|FS:0,0|WCO:0.000,0.000,0.000>'
+        # 'ALARM:1'
+
+        if status.startswith("ALARM:1"):
+            # The ALARM message is followed by something like
+            # '[MSG:Reset to continue]'
+            next = self.receive()
+            raise CNCError(next, CNCStatus.ALARM)
 
         # Discard any unwanted format
         if not (status.startswith("<") and status.endswith(">")):
             print(f"Response to '?' is unexpected: {status}")
             return None
 
         # Remove the chevrons and split all pipes.
@@ -215,33 +243,40 @@
 
     def receive_lines(self, until: str = "ok") -> List[str]:
         """
         Receive multiple lines until getting as specific value.
 
         :param until: The expected response indicating the end of received lines.
         :return: The list of all received lines. Note that the expected line is not included in the
-         list.
+            list.
         """
         lines = []
-        while (l := self.serial.readline().strip().decode()) != until:
-            if len(l):
-                lines.append(l)
+        while (line := self.serial.readline().strip().decode()) != until:
+            if len(line):
+                lines.append(line)
         return lines
 
     def receive(self) -> str:
         """
         Read input serial buffer to get a response. Blocks until a response is
         available.
 
         :return: Received response string, CR-LF removed.
         """
+        tries = 10
         # Read at least 2 bytes for CR-LF.
         response = self.serial.read(2)
         while response[-2:] != b"\r\n":
-            response += self.serial.read(1)
+            part = self.serial.read(1)
+            response += part
+            # Give a chance to get out of this
+            if part == b"":
+                tries -= 1
+            if tries == 0:
+                return ""
         # Remove CR-LF and return as string
         return response[:-2].decode()
 
     def send_receive(self, command: str) -> str:
         """
         Send a command, wait and return the response.
 
@@ -270,35 +305,48 @@
         wco = Vector(*tuple(float(x) for x in extra_dict["WCO"]))
 
         return mpos - wco
 
     @position.setter
     def position(self, value: Vector):
         # To check dimension and range of the given value
-        super(__class__, self.__class__).position.fset(self, value)
+        pos_setter = Stage.position.fset
+        assert pos_setter is not None
+        pos_setter(self, value)
 
         command = f"G0 X{value.x}"
         if len(value) > 1:
             command += f" Y{value.y}"
         if len(value) > 2:
             command += f" Z{value.z}"
         self.send_receive(command)
 
     @property
     def is_moving(self) -> bool:
         """
         Queries the current status of the CNC in order to determine if the CNC is moving
 
         :return: True if the CNC reports that a cycle is running (Run) or
-         if it is in a middle of a homing cycle.
+            if it is in a middle of a homing cycle (Home).
         """
         while (status := self.get_current_status()) is None:
             pass
         return status[0] in [CNCStatus.RUN, CNCStatus.HOME]
 
     def set_origin(self) -> str:
         """
         Set current position as origin
 
         :return: The response of the CNC ('ok' if command has been submitted correctly).
         """
         return self.send_receive("G92 X0 Y0 Z0")
+
+    def home(self, wait=False):
+        """
+        Sends a `$H` command. The stage responds a message `[MSG:Sleeping]` after `ok`.
+        Take caution for collisions before calling this method !
+
+        :param wait: Optionally waits for move operation to be done.
+        """
+        self.send("$H")
+        if wait:
+            self.wait_move_finished()
```

### Comparing `pystages-1.1.0/pystages/corvus.py` & `pystages-1.1.1/pystages/corvus.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,35 +13,38 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 #
 # Copyright 2018-2022 Ledger SAS, written by Olivier Hériveaux
 
 
-import serial
+import serial.serialutil
 import time
 from .exceptions import ConnectionFailure
 from .vector import Vector
 from .stage import Stage
+from typing import Optional
 
 
 class Corvus(Stage):
     """
     Class to command Corvus Eco XYZ stage controller.
     """
 
-    def __init__(self, dev):
+    def __init__(self, dev: Optional[str] = None, serial_number: Optional[str] = None):
         """
         Open serial device to connect to the Corvus controller. Raise a
         ConnectionFailure exception if the serial device could not be open.
 
-        :param dev: Serial device. For instance '/dev/ttyUSB0'.
+        :param dev: Serial device path. For instance '/dev/ttyUSB0'.
+        :param serial_number: Device Serial Number. For instance 'A600AAAA'.
         """
         super().__init__(num_axis=3)
         try:
+            dev = dev or self.find_device(serial_number=serial_number)
             self.serial = serial.Serial(dev, 57600)
         except serial.serialutil.SerialException as e:
             raise ConnectionFailure() from e
         self.__init()
 
     def __init(self):
         """Initialize a few parameters."""
@@ -119,14 +122,26 @@
         self.send("cal")
         self.send("rm")
         # Wait until finished
         for i in range(3):
             while int(self.send_receive("{0} getcaldone".format(i + 1))) != 3:
                 time.sleep(0.1)
 
+    def home(self, wait=False):
+        """
+        Execute limit-switch move.
+        Take caution for collisions before calling this method !
+
+        :param wait: Optionally waits for move operation to be done.
+        """
+        # Call for calibration
+        self.send("cal")
+        if wait:
+            self.wait_move_finished()
+
     def move_relative(self, x, y, z):
         """
         Move stage relative to current position.
 
         :param x: Relative distance on X-axis, in micrometers.
         :param y: Relative distance on Y-axis, in micrometers.
         :param z: Relative distance on Z-axis, in micrometers.
@@ -162,15 +177,18 @@
         """
         res = self.send_receive("p").split()
         return Vector(*tuple(float(x) for x in res))
 
     @position.setter
     def position(self, value: Vector):
         # To check dimension and range of the given value
-        super(__class__, self.__class__).position.fset(self, value)
+        pos_setter = Stage.position.fset
+        assert pos_setter is not None
+        pos_setter(self, value)
+
         self.send("3 setdim")
         self.send("{0} {1} {2} move".format(value.x, value.y, value.z))
 
     @property
     def velocity(self):
         """
         Motors velocity setting, in µm/s.
```

### Comparing `pystages-1.1.0/pystages/exceptions.py` & `pystages-1.1.1/pystages/exceptions.py`

 * *Files identical despite different names*

### Comparing `pystages-1.1.0/pystages/grbl.py` & `pystages-1.1.1/pystages/grbl.py`

 * *Files identical despite different names*

### Comparing `pystages-1.1.0/pystages/m3fs.py` & `pystages-1.1.1/pystages/m3fs.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,37 +13,52 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 #
 # Copyright 2018-2020 Ledger SAS, written by Olivier Hériveaux
 
 
-import serial
+from typing import Optional
+import serial.serialutil
 from binascii import hexlify
 from .exceptions import ConnectionFailure, ProtocolError, VersionNotSupported
 from .stage import Stage
 from .vector import Vector
+from enum import Enum
+
+
+class M3FSCommand(Enum):
+    """
+    Command integer ID for New Scale Technologies M3-FS.
+    https://www.newscaletech.com/downloads/please-register/
+    """
+
+    READ_FIRM_VERSION = 1
+    MOVE_TO_TARGET = 8
+    VIEW_CLOSED_LOOP_STATUS_POS = 10
 
 
 class M3FS(Stage):
     """
     Class to command New Scale Technologies M3-FS focus modules in serial mode
     (VCP).
     If a M3-FS device is seen as a USBXpress chip, it may be used as a
     Virtual-Com-Port after a few cumbersome operations (custom driver with
     correct VID/DID).
     """
 
-    def __init__(self, dev, baudrate=250000):
+    def __init__(self, dev: Optional[str] = None, baudrate=250000):
         """
         Connect to the device. If the serial device cannot be opened, a
         ConnectionFailure exception is thrown. If the device version is not
         supported, a VersionNotSupported error is thrown.
 
-        :param dev: Serial device. For instance 'COM0'.
+        :param dev: Serial device. For instance `'/dev/ttyUSB0'`.
+            If not provided, a suitable device is searched according to
+            according to vendor and product IDs
         :param baudrate: Serial baudrate.
         """
         super().__init__()
         self.resolution_um = 0.5
         try:
             self.serial = serial.Serial(
                 dev, baudrate=baudrate, stopbits=serial.STOPBITS_TWO
@@ -51,33 +66,33 @@
         except serial.serialutil.SerialException as e:
             raise ConnectionFailure() from e
         # Test version string.
         # Currently, only one version has been tested. Some others may be added
         # in the future...
         self.serial.timeout = 1
         try:
-            res = self.command(1)
+            res = self.command(M3FSCommand.READ_FIRM_VERSION)
         except ProtocolError as e:
             raise ConnectionFailure() from e
         self.serial.timeout = None
         if res != "1 VER 4.7.3 M3-FS":
             raise VersionNotSupported(res)
 
-    def __send(self, command, data=None):
+    def __send(self, command: M3FSCommand, data: Optional[str] = None):
         """
         Send a command to the controller.
 
         :param command: Command integer ID.
         :param data: Extra data string.
         """
         if data is not None:
             assert ("<" not in data) and (">" not in data) and ("\r" not in data)
-        if command not in range(100):
+        if command.value not in range(100):
             raise ValueError("Invalid command ID.")
-        full_command = "<{0:02d}".format(command)
+        full_command = "<{0:02d}".format(command.value)
         if data is not None:
             full_command += " " + data
         full_command += ">\r"
         self.serial.write(full_command.encode())
 
     def __receive(self):
         """
@@ -108,65 +123,81 @@
         b = self.serial.read(1)
         if len(b) != 1:
             raise ProtocolError()
         if b[0] != ord("\r"):
             raise ProtocolError()
         return result.decode()
 
-    def command(self, command, data=None):
+    def command(self, command: M3FSCommand, data=None):
         """
         Send a command to the controller and get the response.
 
         :param command: Command integer ID.
         :param data: Extra data string.
         :return: Response data string.
         """
         self.__send(command, data)
         res = self.__receive()
         # Check that the command id in the response is the same as the command
         # id in the request.
-        if (len(res) < 2) or (int(res[0:2]) != command):
-            raise ProtocolError()
+        if (len(res) < 2) or (int(res[0:2]) != command.value):
+            raise ProtocolError(
+                f"Unexpected response after sending command {command}:", res
+            )
         if len(res) == 2:
             return None
         else:
             if res[2] != " ":
-                raise ProtocolError()
+                raise ProtocolError(
+                    f"Unexpected response after sending command {command}:", res
+                )
             return res[3:]
 
     def __get_closed_loop_status(self):
         """
         Query closed-loop status and position.
 
         :return: Tuple of 3 int.
         """
-        res = list(bytes.fromhex(x) for x in self.command(10).split(" "))
+        command = M3FSCommand.VIEW_CLOSED_LOOP_STATUS_POS
+        res = self.command(command)
+        if res is None:
+            raise ProtocolError(
+                f"Unexpected response after sending command {command}: Got response without data."
+            )
+        res = list(bytes.fromhex(x) for x in res.split(" "))
+        if len(res) != 3:
+            raise ProtocolError(
+                f"Unexpected response after sending command {command}: Expecting 3 values, got {res}."
+            )
         motor_status = int.from_bytes(res[0], "big", signed=False)
         position = int.from_bytes(res[1], "big", signed=True)
         error = int.from_bytes(res[2], "big", signed=True)
         return motor_status, position, error
 
     @property
     def position(self) -> Vector:
         """
         Stage position, in micrometers.
 
         :getter: Query and return current stage position.
         :setter: Move stage. Wait until position is reached.
         """
-        motor_status, position, error = self.__get_closed_loop_status()
+        _, position, _ = self.__get_closed_loop_status()
         return Vector(position * self.resolution_um)
 
     @position.setter
     def position(self, value: Vector):
         # To check dimension and range of the given value
-        super(__class__, self.__class__).position.fset(self, value)
+        pos_setter = Stage.position.fset
+        assert pos_setter is not None
+        pos_setter(self, value)
 
         val = round(value.x / self.resolution_um).to_bytes(4, "big", signed=True)
-        self.command(8, hexlify(val).decode())
+        self.command(M3FSCommand.MOVE_TO_TARGET, hexlify(val).decode())
         # Now wait until motor is not moving anymore
         while self.is_moving:
             pass
 
     @property
     def is_moving(self) -> bool:
         return bool(self.__get_closed_loop_status()[0] & 4)
```

### Comparing `pystages-1.1.0/pystages/smc100.py` & `pystages-1.1.1/pystages/smc100.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 #
 # Copyright 2018-2022 Ledger SAS,
 # written by Olivier Hériveaux, Manuel San Pedro and Michaël Mouchous
 
 
-import serial
+import serial.serialutil
 import time
 from .vector import Vector
 from .exceptions import ProtocolError, ConnectionFailure
-from enum import Enum, IntFlag
-from typing import Optional, List
+from enum import Enum, Flag
+from typing import Optional, List, Union
 from .stage import Stage
 
 
 class Link:
     """
     Class to control Newport SMC100 controllers. This uses a serial device to
     communicate with multiple controllers which may be configured in daisy-chain
@@ -38,17 +38,19 @@
     example, we can have two XY stages using four SMC100 controllers connected
     in daisy-chain configuration.
 
     As specified in SMC100 controllers documentation, the address of the first
     controller in the daisy chain is always zero.
     """
 
-    def __init__(self, dev: str):
+    def __init__(self, dev: Optional[str] = None):
         """
-        :param dev: Serial device. For instance '/dev/ttyUSB0' or 'COM0'.
+        :param dev: Serial device. For instance `'/dev/ttyUSB0'`.
+            If not provided, a suitable device is searched according to
+            according to vendor and product IDs
         """
         try:
             self.serial = serial.Serial(port=dev, baudrate=57600, xonxoff=True)
         except serial.serialutil.SerialException as e:
             raise ConnectionFailure() from e
 
     def send(self, address: Optional[int], command: str):
@@ -109,20 +111,20 @@
         check the header of the response.
 
         :param address: Controller address. int.
         :param command: Command string, without '?'.
         """
         query_string = f'{"" if address is None else address}{command}'
         res = self.receive()
-        if res[: len(query_string)] != query_string:
+        if res is None or res[: len(query_string)] != query_string:
             raise ProtocolError(query_string, res)
         return res[len(query_string) :]
 
 
-class State(Enum):
+class State(int, Enum):
     """
     Possible controller states.
     The values in this enumeration corresponds to the values returned by the
     controller.
     """
 
     NOT_REFERENCED_FROM_RESET = 0x0A
@@ -144,15 +146,15 @@
     DISABLE_FROM_READY = 0x3C
     DISABLE_FROM_MOVING = 0x3D
     DISABLE_FROM_JOGGING = 0x3E
     JOGGING_FROM_READY = 0x46
     JOGGING_FROM_DISABLE = 0x47
 
 
-class Error(IntFlag):
+class Error(int, Flag):
     """
     Information returned when querying positioner error.
     """
 
     OUTPUT_POWER_EXCEEDED = 1 << 9
     DC_VOLTAGE_TOO_LOW = 1 << 8
     WRONG_STAGE = 1 << 7
@@ -167,74 +169,74 @@
 
 
 class ErrorAndState:
     """
     Information returned when querying positioner error and controller state.
     """
 
-    state = None
-    error = None
+    state = State.NOT_REFERENCED_FROM_RESET
+    error = Error.NO_ERROR
 
     @property
     def is_referenced(self) -> bool:
         """
         :return: True if state is not one of the NOT_REFERENCED_x states.
         """
         if self.state is None:
             raise RuntimeError("state not available")
         else:
             return not (
-                (self.state.value >= State.NOT_REFERENCED_FROM_RESET.value)
-                and (self.state.value <= State.NOT_REFERENCED_FROM_JOGGING.value)
+                (self.state >= State.NOT_REFERENCED_FROM_RESET)
+                and (self.state <= State.NOT_REFERENCED_FROM_JOGGING)
             )
 
     @property
     def is_ready(self) -> bool:
         """:return: True if state is one of READY_x states."""
-        return (self.state.value >= State.READY_FROM_HOMING.value) and (
-            self.state.value <= State.READY_FROM_JOGGING.value
+        return (self.state >= State.READY_FROM_HOMING) and (
+            self.state <= State.READY_FROM_JOGGING
         )
 
     @property
     def is_moving(self) -> bool:
         """:return: True if state is MOVING."""
-        return self.state.value == State.MOVING.value
+        return self.state == State.MOVING
 
     @property
     def is_homing(self) -> bool:
         """:return: True if state is one of HOMING_x states."""
-        return (self.state.value >= State.HOMING_RS232.value) and (
-            self.state.value <= State.HOMING_SMCRC.value
-        )
+        return (self.state >= State.HOMING_RS232) and (self.state <= State.HOMING_SMCRC)
 
     @property
-    def is_jogging(self):
+    def is_jogging(self) -> bool:
         """:return: True if state is one of JOGGING_x states."""
-        return (self.state.value >= State.JOGGING_FROM_READY.value) and (
-            self.state.value <= State.JOGGING_FROM_DISABLE.value
+        return (self.state >= State.JOGGING_FROM_READY) and (
+            self.state <= State.JOGGING_FROM_DISABLE
         )
 
     @property
-    def is_disabled(self):
+    def is_disabled(self) -> bool:
         """:return: True if state is one of DISABLE_x states."""
-        return (self.state.value >= State.DISABLE_FROM_READY.value) and (
-            self.state.value <= State.DISABLE_FROM_JOGGING.value
+        return (self.state >= State.DISABLE_FROM_READY) and (
+            self.state <= State.DISABLE_FROM_JOGGING
         )
 
 
 class SMC100(Stage):
     """
     Class to command Newport SMC100 controllers.
     """
 
-    def __init__(self, dev, addresses: List[int]):
+    def __init__(self, dev: Optional[Union[str, Link, "SMC100"]], addresses: List[int]):
         """
-        :param dev: Serial device string (for instance '/dev/ttyUSB0' or
+        :param dev: Serial device string (for instance `'/dev/ttyUSB0'` or
             'COM0'), an instance of Link, or an instance of SMC100 sharing
             the same serial device.
+            If not provided, a suitable device is searched according to
+            according to vendor and product IDs
         :param addresses: An iterable of int controller addresses.
         """
         super().__init__(num_axis=len(addresses))
         if isinstance(dev, Link):
             self.link = dev
         elif isinstance(dev, SMC100):
             self.link = dev.link
@@ -257,31 +259,45 @@
         :getter: Query and return current stage position.
         :setter: Move stage.
         """
         result = Vector(dim=self.num_axis)
         # It is faster to send all the request and then get all the responses.
         # This reduces a lot the latency.
         for i, addr in enumerate(self.addresses):
-            r = self.link.query(addr, "TP", lazy_res=False)
-            val = float(r)
+            res = self.link.query(addr, "TP", lazy_res=False)
+            if res is None:
+                raise ProtocolError("TP")
+            val = float(res)
             result[i] = val
         return result
 
     @position.setter
     def position(self, value: Vector):
         # To check dimension and range of the given value
-        super(__class__, self.__class__).position.fset(self, value)
+        pos_setter = Stage.position.fset
+        assert pos_setter is not None
+        pos_setter(self, value)
 
         # Enable the motors
         self.is_disabled = False
         commands = []
-        for position, addr in zip(value, self.addresses):
+        for position, addr in zip(value.data, self.addresses):
             commands.append(f"{addr}PA{position:.5f}")
         self.link.send(None, "\r\n".join(commands))
 
+    def home(self, wait=False):
+        """
+        Perform home search.
+
+        :param wait: Optionally waits for move operation to be done.
+        """
+        self.home_search()
+        if wait:
+            self.wait_move_finished()
+
     def home_search(self):
         """
         Perform home search.
         Home search is performed even if the axes are already referenced.
         It may be better to use home_search_if_required.
         """
         for addr in self.addresses:
@@ -304,15 +320,15 @@
         Query current motion controller errors and state.
         Querying the error and state may clear error flags.
 
         :param addr: Address of the axis.
         :return: Current error and state, in a ErrorAndState instance.
         """
         res = self.link.query(addr, "TS")
-        if len(res) != 6:
+        if res is None or len(res) != 6:
             raise ProtocolError("TS", res)
         result = ErrorAndState()
         result.error = Error(int(res[:4], 16))
         result.state = State(int(res[4:], 16))
         return result
 
     def enter_configuration_state(self, addr: int):
@@ -326,15 +342,18 @@
         """
         self.link.send(addr, "PW0")
 
     def controller_address(self, addr: int):
         """
         Get controller's RS-485 address. int in [2, 31].
         """
-        return int(self.link.query(addr, "SA"))
+        res = self.link.query(addr, "SA")
+        if res is None:
+            raise ProtocolError("SA")
+        return int(res)
 
     def set_controller_address(self, addr: int, value: int):
         """
         Set controller's RS-485 address. int in [2, 31].
         Changing the address is only possible when the controller is in
         configuration state.
         """
@@ -388,14 +407,15 @@
             while error_and_state.is_moving:
                 time.sleep(0.1)
 
     @property
     def is_moving(self) -> bool:
         """
         Indicates if the stage is currently moving due to MOVE, HOME or JOG operation.
+
         :return: Moving state of the stage
         """
         for addr in self.addresses:
             state = self.get_error_and_state(addr=addr)
             if state.is_moving or state.is_homing or state.is_jogging:
                 return True
         return False
@@ -419,13 +439,13 @@
 
     def enter_leave_disable_state(self, addr: Optional[int], enter: bool = True):
         """
         Permits for a specified axis to enter or leave the DISABLE state.
         DISABLE state makes the motor not energized and opens the control loop.
 
         :param addr: address of the axis to operate.
-         If None is passed, it applies to all controllers
+            If None is passed, it applies to all controllers
         :param enter: True to enter, False to leave DISABLE state
         """
         # MM0 changes the controller’s state from READY to DISABLE (enter)
         # MM1 changes the controller’s state from DISABLE to READY (leave)
         self.link.send(addr, f"MM{0 if enter else 1}")
```

### Comparing `pystages-1.1.0/pystages/stage.py` & `pystages-1.1.1/pystages/stage.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,38 +13,70 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 #
 # Copyright 2018-2022 Ledger SAS, written by Michaël Mouchous
 
 from .vector import Vector
-from typing import Optional
+from typing import Optional, Callable
 from abc import ABC, abstractmethod
+from serial.tools.list_ports import comports
 
 
 class Stage(ABC):
     """
     Stage is an abstract class from which all stage implementation must inherit to get a consistent
     behavior and value checking for getting and setting position, setting software limits...
     """
 
     def __init__(self, num_axis=1):
         """
-        :param num_axis: The number of axis of the stage, can be updated or set after initialisation
-         of the object.
+        :param num_axis: The number of axis of the stage, can be updated or set after initialization
+            of the object.
         """
         self.num_axis = num_axis
         # The wait routine is a function that is called when the wait_move_finished is looping.
-        # It can be used to add some temporisation and/or UI updates.
-        self.wait_routine = None
+        # It can be used to add some temporization and/or UI updates.
+        self.wait_routine: Optional[Callable] = None
 
         # Minimum and maximum software limits
         self._minimums: Optional[Vector] = None
         self._maximums: Optional[Vector] = None
 
+    def find_device(
+        self,
+        pid: Optional[int] = None,
+        vid: Optional[int] = None,
+        serial_number: Optional[str] = None,
+    ) -> str:
+        """
+        Find automatically one device according to given information in parameters
+
+        :param pid: Product ID of the device. If None, not a limiting criteria.
+        :param vid: Vendor ID of the device. If None, not a limiting criterial.
+        :param serial_number: serial number of the device. If not None, the device
+            must have a serial number and matches the given value.
+        :return: The device path to the communication port.
+        """
+        possible_ports = []
+        for port in comports():
+            if serial_number is not None:
+                if port.serial_number == serial_number:
+                    possible_ports.append(port)
+                continue
+            if (port.pid, port.vid) == (pid, vid):
+                possible_ports.append(port)
+        if len(possible_ports) > 1:
+            raise RuntimeError("Multiple devices found! I don't know which one to use.")
+        elif len(possible_ports) == 1:
+            dev = possible_ports[0].device
+        else:
+            raise RuntimeError("No device found")
+        return dev
+
     @property
     @abstractmethod
     def position(self) -> Vector:
         """
         Current stage position. Vector.
 
         :getter: Query and return stage position.
@@ -147,7 +179,14 @@
         return self._maximums
 
     @maximums.setter
     def maximums(self, value: Optional[Vector]):
         if value is not None:
             self.check_dimension(value)
         self._maximums = value
+
+    def home(self, wait=False):
+        """Triggers a homing command.
+
+        :param wait: Optionally waits for move operation to be done.
+        """
+        self.move_to(Vector(dim=self.num_axis), wait=wait)
```

### Comparing `pystages-1.1.0/pystages/tic.py` & `pystages-1.1.1/pystages/tic.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 import usb.core
 import usb.util
 from enum import Enum
 from time import sleep
 from .stage import Stage
 from .vector import Vector
+from .exceptions import ConnectionFailure
 
 
 class TicVariable(Enum):
     """
     Variables which can be read using GET_VARIABLE command.
     https://www.pololu.com/docs/0J71/7
     """
@@ -69,15 +70,15 @@
     AGC_MODE = (0x56, 1, False)
     AGC_BOTTOM_CURRENT_LIMIT = (0x57, 1, False)
     AGC_CURRENT_BOOST_STEP = (0x58, 1, False)
     AGC_FREQUENCY_LIMIT = (0x59, 1, False)
     LAST_HP_DRIVER_ERRORS = (0xFF, 1, False)
 
 
-class TicCommand(Enum):
+class TicCommand(int, Enum):
     """
     Command codes for Polulu Tic Stepper Motor Controller.
     https://www.pololu.com/docs/0J71/8
     """
 
     SET_TARGET_POSITION = 0xE0
     SET_TARGET_VELOCITY = 0xE3
@@ -103,15 +104,15 @@
     GET_VARIABLE_AND_CLEAR_ERRORS_OCCURRED = 0xA2
     GET_SETTING = 0xA8
     SET_SETTING = 0x13
     REINITIALIZE = 0x10
     START_BOOTLOADER = 0xFF
 
 
-class TicDirection(Enum):
+class TicDirection(int, Enum):
     """Possible directions for homing"""
 
     REVERSE = 0
     FORWARD = 1
 
 
 class Tic(Stage):
@@ -120,85 +121,97 @@
 
     :ivar poll_interval: Interval between successive state polling for some
      long motor operations.
     """
 
     def __init__(self):
         super().__init__()
-        self.dev = usb.core.find(idVendor=0x1FFB, idProduct=0x00B5)
+        dev = usb.core.find(idVendor=0x1FFB, idProduct=0x00B5)
+        if isinstance(dev, usb.core.Device):
+            self.dev = dev
+        else:
+            raise ConnectionFailure("Tic stepper motor not found.")
         self.dev.set_configuration()
         self.energize()
         self.poll_interval = 0.1
 
     def quick(self, command: TicCommand):
         """
         Send a quick command with no data.
 
         :param command: Command.
         """
-        self.dev.ctrl_transfer(0x40, command.value, 0, 0, 0)
+        self.dev.ctrl_transfer(0x40, command, 0, 0, 0)
 
     def write_7(self, command: TicCommand, data: int):
         """
         Write 7 bits.
 
         :param command: Command.
         :param data: Value to be written.
         """
-        self.dev.ctrl_transfer(0x40, command.value, data, 0, 0)
+        self.dev.ctrl_transfer(0x40, command, data, 0, 0)
 
     def write_32(self, command: TicCommand, data: int):
         """
         Write 32 bits.
 
         :param command: Command code.
         :param data: Value to be written.
         """
-        self.dev.ctrl_transfer(0x40, command.value, data & 0xFFFF, data >> 16, 0)
+        self.dev.ctrl_transfer(0x40, command, data & 0xFFFF, data >> 16, 0)
 
     def block_read(self, command: TicCommand, offset, length) -> bytes:
         """
         Read data from the device.
 
         :param command: Command code.
         :param offset: Data offset.
         :param length: Data length.
         """
-        return bytes(self.dev.ctrl_transfer(0xC0, command.value, 0, offset, length))
+        return bytes(self.dev.ctrl_transfer(0xC0, command, 0, offset, length))
 
     def set_setting(self, command: TicCommand, data, offset):
         """
         Set setting data.
 
         :param command: Command code.
         :param data: Value to be written.
         :param offset: Write offset.
         """
-        self.dev.ctrl_transfer(0x40, command.value, data, offset, 0)
+        self.dev.ctrl_transfer(0x40, command, data, offset, 0)
 
     def energize(self):
         self.quick(TicCommand.ENERGIZE)
 
     def deenergize(self):
         self.quick(TicCommand.DEENERGIZE)
 
     def reset(self):
         self.quick(TicCommand.RESET)
 
     def exit_safe_start(self):
         self.quick(TicCommand.EXIT_SAFE_START)
 
+    def home(self, wait=False):
+        """Triggers a Home command.
+
+        :param wait: Optionally waits for move operation to be done."""
+        self.go_home(TicDirection.REVERSE, False)
+        if wait:
+            self.wait_move_finished()
+
     def go_home(self, direction: TicDirection, wait: bool = True):
         """
         Run the homing procedure.
         :param direction: Homing direction.
         :param wait: If True, wait for homing procedure end.
         """
         self.exit_safe_start()
-        self.write_7(TicCommand.GO_HOME, direction.value)
+        self.write_7(TicCommand.GO_HOME, direction)
         if wait:
             while self.get_variable(TicVariable.MISC_FLAGS) & (1 << 4):
                 self.exit_safe_start()
                 sleep(self.poll_interval)
 
     def set_target_position(self, pos: int):
         self.write_32(TicCommand.SET_TARGET_POSITION, pos)
@@ -223,15 +236,18 @@
         :setter: Set target position and wait until position is reached.
         """
         return Vector(self.get_variable(TicVariable.CURRENT_POSITION))
 
     @position.setter
     def position(self, value: Vector):
         # To check dimension and range of the given value
-        super(__class__, self.__class__).position.fset(self, value)
+        pos_setter = Stage.position.fset
+        assert pos_setter is not None
+        pos_setter(self, value)
+
         self.target_position = value.x
         while self.position.x != value.x:
             sleep(self.poll_interval)
             self.exit_safe_start()
 
     @property
     def target_position(self) -> int:
```

### Comparing `pystages-1.1.0/pystages/vector.py` & `pystages-1.1.1/pystages/vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Copyright 2018 Ledger SAS, written by Olivier Hériveaux and Manuel San Pedro
 
 
 import unittest
 from typing import Union
 
 
-class Vector:
+class Vector(object):
     """
     Some basic vector manipulation class for stages control.
     """
 
     def __init__(self, *args, dim=None):
         """
         :param args: Initial values of the vector.
@@ -159,25 +159,25 @@
             result = Vector(dim=dim)
             for i in range(dim):
                 result[i] = self[i] * other
             return result
 
         result = Vector(dim=dim)
         if len(other) != dim:
-            raise ValueError(f"Incorrect vector size")
+            raise ValueError("Incorrect vector size")
         for i in range(dim):
             result[i] = self[i] * other[i]
         return result
 
     def __truediv__(self, other):
         if isinstance(other, (int, float)):
             return self * (1.0 / other)
         else:
             raise TypeError(
-                f"Incorrect type for second operand. int or float is expected."
+                "Incorrect type for second operand. int or float is expected."
             )
 
 
 class TestVector(unittest.TestCase):
     def test_init(self):
         v = Vector(1)
         self.assertEqual(len(v), 1)
```

### Comparing `pystages-1.1.0/.gitignore` & `pystages-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pystages-1.1.0/COPYING` & `pystages-1.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `pystages-1.1.0/COPYING.LESSER` & `pystages-1.1.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pystages-1.1.0/README.md` & `pystages-1.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,41 @@
-[![Documentation Status](https://readthedocs.org/projects/pystages/badge/?version=latest)](https://pystages.readthedocs.io/en/latest/?badge=latest)
-
 # PyStages
 
+[![Documentation Status](https://readthedocs.org/projects/pystages/badge/?version=latest)](https://pystages.readthedocs.io/en/latest/?badge=latest)
+
 PyStages is a Python 3 library for controlling motorized stages which have a
 motion controller. It has been designed for microscopy test benches automation.
 
 The following motion controllers are currently supported (only the main features
 are implemented):
 
 - Micos Corvus Eco controller
 - New Scale Technologies M3-FS focus modules (serial only)
 - Newport SMC100 motion controllers
 - Tic Stepper Motor controller (USB only)
 - CNC Router with GRBL/GCode instructions (CNC 3018-PRO)
 
-The library also provides helper classes for basic vector manipulation and 
-autofocus calculation
+The library also provides helper classes for basic vector manipulation and
+autofocus computation.
 
 ## Documentation
 
 Documentation is available on [Read the Docs](https://pystages.readthedocs.io).
 
+## PyStages GUI
+
+A user interface has been implemented to control the stages.
+
+You can run it with the following command:
+
+```bash
+python -m pystages.gui
+```
+
 ## Requirements
 
 This library requires the following packages:
+
 - [pyserial](https://pypi.org/project/pyserial/)
 - [numpy](https://pypi.org/project/numpy/)
-- [pyusb](https://pypi.org/project/pyusb/)
+- [pyusb](https://pypi.org/project/pyusb/)
+- [PyQt6](https://pypi.org/project/PyQt6/)
```

### Comparing `pystages-1.1.0/pyproject.toml` & `pystages-1.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pystages"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Olivier Hérivaux", email="olivier.heriveaux@ledger.fr" },
   { name="Michaël Mouchous", email="michael.mouchous@ledger.fr" },
 ]
 description = "Motorized stage control library for scientific applications"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pyserial",
     "pyusb",
-    "numpy"
+    "numpy",
+    "pyqt6"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Ledger-Donjon/pystages"
 "Bug Tracker" = "https://github.com/Ledger-Donjon/pystages/issues"
-"Documentation" = "https://pystages.readthedocs.io/en/latest"
+"Documentation" = "https://pystages.readthedocs.io/en/latest"
```

### Comparing `pystages-1.1.0/PKG-INFO` & `pystages-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,61 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pystages
-Version: 1.1.0
+Version: 1.1.1
 Summary: Motorized stage control library for scientific applications
 Project-URL: Homepage, https://github.com/Ledger-Donjon/pystages
 Project-URL: Bug Tracker, https://github.com/Ledger-Donjon/pystages/issues
 Project-URL: Documentation, https://pystages.readthedocs.io/en/latest
 Author-email: Olivier Hérivaux <olivier.heriveaux@ledger.fr>, Michaël Mouchous <michael.mouchous@ledger.fr>
 License-File: COPYING
 License-File: COPYING.LESSER
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: numpy
+Requires-Dist: pyqt6
 Requires-Dist: pyserial
 Requires-Dist: pyusb
 Description-Content-Type: text/markdown
 
-[![Documentation Status](https://readthedocs.org/projects/pystages/badge/?version=latest)](https://pystages.readthedocs.io/en/latest/?badge=latest)
-
 # PyStages
 
+[![Documentation Status](https://readthedocs.org/projects/pystages/badge/?version=latest)](https://pystages.readthedocs.io/en/latest/?badge=latest)
+
 PyStages is a Python 3 library for controlling motorized stages which have a
 motion controller. It has been designed for microscopy test benches automation.
 
 The following motion controllers are currently supported (only the main features
 are implemented):
 
 - Micos Corvus Eco controller
 - New Scale Technologies M3-FS focus modules (serial only)
 - Newport SMC100 motion controllers
 - Tic Stepper Motor controller (USB only)
 - CNC Router with GRBL/GCode instructions (CNC 3018-PRO)
 
-The library also provides helper classes for basic vector manipulation and 
-autofocus calculation
+The library also provides helper classes for basic vector manipulation and
+autofocus computation.
 
 ## Documentation
 
 Documentation is available on [Read the Docs](https://pystages.readthedocs.io).
 
+## PyStages GUI
+
+A user interface has been implemented to control the stages.
+
+You can run it with the following command:
+
+```bash
+python -m pystages.gui
+```
+
 ## Requirements
 
 This library requires the following packages:
+
 - [pyserial](https://pypi.org/project/pyserial/)
 - [numpy](https://pypi.org/project/numpy/)
-- [pyusb](https://pypi.org/project/pyusb/)
+- [pyusb](https://pypi.org/project/pyusb/)
+- [PyQt6](https://pypi.org/project/PyQt6/)
```

