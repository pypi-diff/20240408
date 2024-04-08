# Comparing `tmp/pybud-gui-0.9.5.tar.gz` & `tmp/pybud-gui-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybud-gui-0.9.5.tar", last modified: Sat Apr  6 18:49:37 2024, max compression
+gzip compressed data, was "pybud-gui-0.9.6.tar", last modified: Mon Apr  8 16:25:45 2024, max compression
```

## Comparing `pybud-gui-0.9.5.tar` & `pybud-gui-0.9.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 18:49:37.964254 pybud-gui-0.9.5/
--rw-rw-rw-   0        0        0     4162 2024-04-06 18:49:37.963254 pybud-gui-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     3728 2024-04-06 18:44:39.000000 pybud-gui-0.9.5/README.md
--rw-rw-rw-   0        0        0      566 2024-04-06 18:49:27.000000 pybud-gui-0.9.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 18:49:37.965254 pybud-gui-0.9.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-06 18:49:37.941821 pybud-gui-0.9.5/src/
--rw-rw-rw-   0        0        0     2352 2024-03-28 12:56:03.000000 pybud-gui-0.9.5/src/example1.py
--rw-rw-rw-   0        0        0     3579 2024-03-28 19:49:41.000000 pybud-gui-0.9.5/src/example2.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:49:37.943821 pybud-gui-0.9.5/src/pybud/
--rw-rw-rw-   0        0        0     5407 2024-03-28 12:00:12.000000 pybud-gui-0.9.5/src/pybud/ansi.py
--rw-rw-rw-   0        0        0    18794 2024-03-28 13:09:35.000000 pybud-gui-0.9.5/src/pybud/drawer.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:49:37.946821 pybud-gui-0.9.5/src/pybud/gui/
--rw-rw-rw-   0        0        0     7466 2024-03-28 13:18:01.000000 pybud-gui-0.9.5/src/pybud/gui/gui.py
--rw-rw-rw-   0        0        0     1908 2024-03-28 09:48:29.000000 pybud-gui-0.9.5/src/pybud/gui/utils.py
--rw-rw-rw-   0        0        0    10030 2024-03-28 19:30:17.000000 pybud-gui-0.9.5/src/pybud/gui/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:49:37.962253 pybud-gui-0.9.5/src/pybud_gui.egg-info/
--rw-rw-rw-   0        0        0     4162 2024-04-06 18:49:37.000000 pybud-gui-0.9.5/src/pybud_gui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-06 18:49:37.000000 pybud-gui-0.9.5/src/pybud_gui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 18:49:37.000000 pybud-gui-0.9.5/src/pybud_gui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-06 18:49:37.000000 pybud-gui-0.9.5/src/pybud_gui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-06 18:49:37.000000 pybud-gui-0.9.5/src/pybud_gui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 16:25:45.328108 pybud-gui-0.9.6/
+-rw-rw-rw-   0        0        0     4160 2024-04-08 16:25:45.326603 pybud-gui-0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3728 2024-04-06 18:44:39.000000 pybud-gui-0.9.6/README.md
+-rw-rw-rw-   0        0        0      564 2024-04-08 16:25:36.000000 pybud-gui-0.9.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 16:25:45.328108 pybud-gui-0.9.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 16:25:45.297587 pybud-gui-0.9.6/src/
+-rw-rw-rw-   0        0        0     2324 2024-04-08 15:08:08.000000 pybud-gui-0.9.6/src/example1.py
+-rw-rw-rw-   0        0        0     3548 2024-04-08 16:20:34.000000 pybud-gui-0.9.6/src/example2.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:25:45.301587 pybud-gui-0.9.6/src/pybud/
+-rw-rw-rw-   0        0        0     5789 2024-04-08 16:24:06.000000 pybud-gui-0.9.6/src/pybud/ansi.py
+-rw-rw-rw-   0        0        0     1912 2024-04-08 14:53:41.000000 pybud-gui-0.9.6/src/pybud/deftypes.py
+-rw-rw-rw-   0        0        0    20291 2024-04-08 16:15:46.000000 pybud-gui-0.9.6/src/pybud/drawer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:25:45.303588 pybud-gui-0.9.6/src/pybud/gui/
+-rw-rw-rw-   0        0        0     7852 2024-04-08 15:10:27.000000 pybud-gui-0.9.6/src/pybud/gui/dialog.py
+-rw-rw-rw-   0        0        0    10653 2024-04-08 16:23:39.000000 pybud-gui-0.9.6/src/pybud/gui/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:25:45.325606 pybud-gui-0.9.6/src/pybud_gui.egg-info/
+-rw-rw-rw-   0        0        0     4160 2024-04-08 16:25:45.000000 pybud-gui-0.9.6/src/pybud_gui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-04-08 16:25:45.000000 pybud-gui-0.9.6/src/pybud_gui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 16:25:45.000000 pybud-gui-0.9.6/src/pybud_gui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-08 16:25:45.000000 pybud-gui-0.9.6/src/pybud_gui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-08 16:25:45.000000 pybud-gui-0.9.6/src/pybud_gui.egg-info/top_level.txt
```

### Comparing `pybud-gui-0.9.5/PKG-INFO` & `pybud-gui-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pybud-gui
-Version: 0.9.5
-Summary: Create beautiful console GUIs in python, using Widgets, Dialouges, and more!
+Version: 0.9.6
+Summary: Create beautiful console GUIs in python, using Widgets, Dialogs, and more!
 Author-email: Amirali Mollaei <aam.products.mail@gmail.com>
 License: BSD 4-clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: readchar==4.0.5
```

### Comparing `pybud-gui-0.9.5/README.md` & `pybud-gui-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `pybud-gui-0.9.5/pyproject.toml` & `pybud-gui-0.9.6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pybud-gui"
-version = "0.9.5"
+version = "0.9.6"
 dependencies = [
   "readchar==4.0.5",
 ]
 requires-python = ">= 3.10"
 authors = [
   {name = "Amirali Mollaei", email = "aam.products.mail@gmail.com"},
 ]
-description = "Create beautiful console GUIs in python, using Widgets, Dialouges, and more!"
+description = "Create beautiful console GUIs in python, using Widgets, Dialogs, and more!"
 license = {text = "BSD 4-clause License"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 readme = "README.md"
```

### Comparing `pybud-gui-0.9.5/src/example1.py` & `pybud-gui-0.9.6/src/example1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pybud
 import pybud.ansi as ansi
 from pybud.drawer import ColoredString as CStr
 from pybud.ansi import ColorType
-from pybud.gui.gui import AutoDialouge
-from pybud.gui.utils import Size, Point
+from pybud.gui.dialog import AutoDialog
+from pybud.deftypes import Size, Point
 from pybud.gui.widgets import WidgetInput, WidgetLabel, WidgetOptions
 
 
-def main_dialouge(WIDTH = 70):
-    """ the main dialouge """
+def main_dialog(WIDTH = 70):
+    """ the main dialog """
 
     def briliant_option(self):
         ansi.write("Briliant!        \r")
         ansi.flush()
         return "Briliant!"
 
     def verycool_option(self):
@@ -23,56 +23,56 @@
     def nice_option(self):
         ansi.write("Nice!             \r")
         ansi.flush()
         return "Nice!"
 
     title = CStr("[") + CStr(" " + "PyBUD: GUI Beauty" +
                              " ", forecolor=(255, 0, 0)) + CStr("]")
-    caption = "A python library for creating beautiful GUIs in console, with tons of diffrent components, such as Dialouges, Widgets, Drawables, optimized colored strings, and more!"
+    caption = "A python library for creating beautiful GUIs in console, with tons of diffrent components, such as Dialogs, Widgets, Drawables, optimized colored strings, and more!"
     options = [
         ("Nice!", nice_option),
         ("Very Cool!", verycool_option),
         ("Briliant!", briliant_option),
     ]
     default = 2
-    mydialouge = AutoDialouge(width=WIDTH, ctype=ColorType.LEGACY)
-    mydialouge.add_widget(WidgetLabel(
+    mydialog = AutoDialog(width=WIDTH, ctype=ColorType.LEGACY)
+    mydialog.add_widget(WidgetLabel(
         title,
         size=Size(WIDTH, 0),  # height will be owerwritten in WidgetLabel
         pos=Point(0, 1),
     ))
-    mydialouge.add_widget(WidgetLabel(
+    mydialog.add_widget(WidgetLabel(
         text = caption,
         centered=False,
         size=Size(WIDTH, 0),  # height will be owerwritten in WidgetLabel
         pos=Point(4, 2),
     ))
 
-    mydialouge.add_widget(WidgetOptions(
+    mydialog.add_widget(WidgetOptions(
         options,
         default_option=default,
         size=Size(WIDTH-4, 0),  # height will be owerwritten in WidgetOptions
         pos=Point(2, 6),
     ))
 
-    return mydialouge
+    return mydialog
 
 if __name__ == "__main__":
     ansi.InitAnsi()
 
     DEBUG = False
 
     if DEBUG:
         f = open("output.ansi", "w", encoding="utf-8")
         ansi.write = lambda x: f.write(x)
         ansi.writeln = lambda x: f.write(x + "\n")
         ansi.flush = lambda: f.flush()
 
-    mydialouge = main_dialouge()
+    mydialog = main_dialog()
     try:
-        # mydialouge.show()
-        text = mydialouge.show()
+        # mydialog.show()
+        text = mydialog.show()
 
         print(f"result: \"{text}\"")
         
     except KeyboardInterrupt:
-        mydialouge.close()
+        mydialog.close()
```

### Comparing `pybud-gui-0.9.5/src/example2.py` & `pybud-gui-0.9.6/src/example2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 import pybud
 import pybud.ansi as ansi
 from pybud.ansi import ColorType
 from pybud.drawer import ColoredString as CStr
-from pybud.gui.gui import AutoDialouge
-from pybud.gui.utils import Point, Size
+import pybud.gui.dialog 
+from pybud.gui.dialog import AutoDialog
+from pybud.deftypes import Point, Size
 from pybud.gui.widgets import WidgetInput, WidgetLabel, WidgetOptions
 
 
-def input_dialouge(WIDTH=76):
-    """ the main dialouge """
+def input_dialog(WIDTH=76):
+    """ the main dialog """
 
     title = CStr("[") + CStr(" " + "PyBUD: GUI Beauty" +
                              " ", forecolor=(255, 0, 0)) + CStr("]")
-    caption = "A python library for creating beautiful GUIs in console, with tons of diffrent components, such as Dialouges, Widgets, Drawables, color optimization, and more!"
-    mydialouge = AutoDialouge(width=WIDTH, ctype=ColorType.LEGACY)
+    caption = "A python library for creating beautiful GUIs in console, with tons of diffrent components, such as Dialogs, Widgets, Drawables, color optimization, and more!"
+    mydialog = AutoDialog(width=WIDTH, ctype=ColorType.LEGACY, background_color = (90, 90, 255))
 
-    mydialouge.add_widget(WidgetLabel(
+    mydialog.add_widget(WidgetLabel(
         title,
         size=Size(WIDTH),  # height will be owerwritten in WidgetLabel
         pos=Point(0, 1),
     ))
 
-    mydialouge.add_widget(WidgetLabel(
+    mydialog.add_widget(WidgetLabel(
         caption,
         centered=True,
         size=Size(WIDTH),  # height will be owerwritten in WidgetLabel
         pos=Point(0, 2),
     ))
 
-    mydialouge.add_widget(WidgetInput(
+    mydialog.add_widget(WidgetInput(
         "text input: ",
         size=Size(WIDTH//2 - 4),  # height will be owerwritten in WidgetLabel
         pos=Point(2, 6),
     ))
-    mydialouge.add_widget(WidgetInput(
+    mydialog.add_widget(WidgetInput(
         "another text input: ",
         size=Size(WIDTH//2 - 4),  # height will be owerwritten in WidgetLabel
         pos=Point(WIDTH//2 + 2, 6),
     ))
 
     def briliant_option(self):
         ansi.write("Briliant!        \r")
@@ -61,49 +62,47 @@
     # the text and callback function for each option
     options = [
         ("Nice!", nice_option),
         ("Very Cool!", verycool_option),
         ("Awesome!", awesome_option),
         ("Briliant!", briliant_option),
     ]
-    mydialouge.add_widget(WidgetOptions(
+    mydialog.add_widget(WidgetOptions(
         options,
         size=Size(WIDTH-4),  # height will be owerwritten in WidgetOptions
         pos=Point(2, 8),
     ))
-    mydialouge.add_widget(WidgetLabel(
+    mydialog.add_widget(WidgetLabel(
         CStr("Tip: ", forecolor=(220, 220, 0)) +
         CStr("you can use TAB or arrow keys to switch between selectable Widgets! and use ") + CStr("Ctrl + C", forecolor=(220, 220, 0)) +
         CStr(" or press enter on (InputWidget)s to exit!"),
         centered=True,
         size=Size(WIDTH - 24),  # height will be owerwritten in WidgetLabel
         pos=Point(22, 9),
+        name = "LastLabel"
     ))
-    return mydialouge
+    return mydialog
 
 
 if __name__ == "__main__":
     ansi.InitAnsi()
-    DEBUG = False
 
-    if DEBUG:
-        f = open("output.ansi", "w", encoding="utf-8")
-        ansi.write = lambda x: f.write(x)
-        ansi.writeln = lambda x: f.write(x + "\n")
-        ansi.flush = lambda: f.flush()
+    mydialog = input_dialog()
 
-    mydialouge = input_dialouge()
+    # print dialog summery
+    # print(mydialog)
 
-    # mydialouge.show()
-    text = mydialouge.show()
+    # mydialog.show()
+    text = mydialog.show()
 
     print(f"result (last callback return): \"{text}\"")
 
     print(f"individual outputs:")
-    for i, w in enumerate(mydialouge.widgets):
+    for i, w in enumerate(mydialog.widgets):
+        print(w.name + ":")
         if isinstance(w, WidgetInput):
             print(f"text written in textbox ({w.text}): ", w.input)
-        if isinstance(w, WidgetOptions):
-            print("selected option id:", w.selected, "selected option text:", w.options[w.selected])
-
-
-
+        elif isinstance(w, WidgetOptions):
+            print("selected option id:", w.selected)
+            print("selected option text:", w.options[w.selected])
+        else:
+            print("no output")
```

### Comparing `pybud-gui-0.9.5/src/pybud/ansi.py` & `pybud-gui-0.9.6/src/pybud/ansi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 
 import os
 import re
 import string
 from enum import Enum
-from sys import stdin, stdout
+from sys import platform, stdin, stdout
 
 ansi_escape = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')
 
 def InitAnsi():
     # call os.system("") to active ansi colors on the windows terminal
     os.system("")
 
 # write and flash on stdout
-
-f = stdout#open("output.ansi", "w", encoding="utf-8")
+f = stdout
 
 def write(data): f.write(data)
 def writeln(data): f.write(data+"\n")
 def read(): stdin.read()
 def readln(): stdin.readline()
 def flush(): f.flush()
-        
+
+DEBUG = False
+if DEBUG:
+    f = open("output.ansi", "w", encoding="utf-8")
+    write = lambda x: f.write(x)
+    writeln = lambda x: f.write(x + "\n")
+    flush = lambda: f.flush()
+
 # ansi colors
 class ForeColors():
     Black          = "\x1B[0;30m"
     Red            = "\x1B[0;31m"
     Green          = "\x1B[0;32m"
     Yellow         = "\x1B[0;33m"
     Blue           = "\x1B[0;34m"
@@ -78,26 +84,27 @@
 
 class AnsiColor():
     def __init__(self, rgb: tuple[int, int, int], foreground: bool = True):
         self.rgb = rgb
         self.foreground = foreground
 
     def __str__(self) -> str:
-        return self.rgb
+        return str(self.rgb)
 
     def __eq__(self, other) -> bool:
         if other is None:
             return False
         return (self.rgb == other.rgb) and self.foreground == other.foreground
 
     # def __add__(self, other) -> str:
     #    return self.__str__() + other.__str__()
 
     @staticmethod
     def get_c816color_from_rgb(rgb: tuple[int, int, int], foreground: bool) -> str:
+        # TODO: implement
         raise NotImplementedError()
 
     @staticmethod
     def get_legacycolor_from_rgb(rgb: tuple[int, int, int], foreground: bool) -> str:
         if foreground:
             return FRgbAnsi(*rgb)
         else:
@@ -120,87 +127,84 @@
             return self.get_legacycolor_from_rgb(self.rgb, self.foreground)
         elif ctype == ColorType.TRUECOLOR:
             return self.get_truecolor_from_rgb(self.rgb, self.foreground)
 
 def remove_ansi(text):
     return ansi_escape.sub('', text)
 
+def round_if_float(c):
+    return round(c) if isinstance(c, float) else c
+
 def FRgbAnsiTC(R: int, G: int, B: int) -> string:
+    R = round_if_float(R)
+    G = round_if_float(G)
+    B = round_if_float(B)
     return (f"\x1b[38;2;{R};{G};{B}m")
 
 def BRgbAnsiTC(R: int, G: int, B: int) -> string:
+    R = round_if_float(R)
+    G = round_if_float(G)
+    B = round_if_float(B)
     return (f"\x1b[48;2;{R};{G};{B}m")
 
-def FRgbAnsi(R: int, G: int, B: int) -> string:
-    r = round((R / 256) * 5)
-    g = round((G / 256) * 5)
-    b = round((B / 256) * 5)
+def calc_legacy_colorbit(c):
+    #legacy color ranges from about 48 - 236 (changes in different environments)
+    k = (1 / 188) * 5
+    r = int(max(0,(c-48)) * k)
+    return r
+
+def calc_legacy_colorcode(R: int, G: int, B: int) -> int:
+    r = calc_legacy_colorbit(R)
+    g = calc_legacy_colorbit(G)
+    b = calc_legacy_colorbit(B)
     color_code = r * 36 + g * 6 + b + 16
+    #print(color_code)
+    return color_code
+
+def FRgbAnsi(R: int, G: int, B: int) -> string:
+    color_code = calc_legacy_colorcode(R, G, B)
     return (f"\x1b[38;5;{color_code}m")
 
 def BRgbAnsi(R: int, G: int, B: int) -> string:
-    r = round((R / 255) * 5)
-    g = round((G / 255) * 5)
-    b = round((B / 255) * 5)
-    color_code = r * 36 + g * 6 + b + 16
+    color_code = calc_legacy_colorcode(R, G, B)
     return (f"\x1b[48;5;{color_code}m")
 
 def bold(text):
     return "\x1b[1m" + text + "\x1b[22m"
 
 
 def italic(text):
     return "\x1b[3m" + text + "\x1b[23m"
 
 
 def underline(text):
     return "\x1b[4m" + text + "\x1b[24m"
 
-
-def underline(text):
-    return "\x1b[4m" + text + "\x1b[24m"
-
-
+# might not be supprted in some environments
 def blinking(text):
     return "\x1b[5m" + text + "\x1b[25m"
 
 
 CR = "\x1b[0m"
 
 
 def go_up(n_lines: int) -> str:
     return write(f"\033[{n_lines}F")
 
-
-def go_up_() -> str:
-    return write(f"\033M")
+# Legacy go up
+def go_up_(n_lines: int = 1) -> str:
+    return write("\033M" * n_lines)
 
 # clear console
 
 
-def clear() -> int:
-    return os.system("cls")
-
+def clear():
+    if platform.startswith(("linux", "darwin", "freebsd", "openbsd", "cygwin")):
+        os.system("clear")
+    elif platform == "win32":
+        os.system("cls")
+    else:
+        raise NotImplementedError(f"The platform {platform} is not supported yet.")
 
 # get terminal size
 def get_size() -> os.terminal_size:
-    return os.get_terminal_size()
-
-# formatting
-
-def center(text: str, max_len: int, fill: str = " "):
-    text_len = len(remove_ansi(text))
-    pl = (max_len - text_len)//2
-    pr = max_len - pl - text_len
-    return (fill * pl) + text + (fill * pr)
-
-
-def rjust(text: str, max_len: int, fill: str = " "):
-    text_len = len(remove_ansi(text))
-    pl = max_len - text_len
-    return (fill * pl) + text
-
-
-def ljust(text: str, max_len: int, fill: str = " "):
-    text_len = len(remove_ansi(text))
-    pr = max_len - text_len
-    return text + (fill * pr)
+    return os.get_terminal_size()
```

### Comparing `pybud-gui-0.9.5/src/pybud/drawer.py` & `pybud-gui-0.9.6/src/pybud/drawer.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 # ansilen = lambda x: len(ansi.remove_ansi(x))
 
 
 def get_rgb_if_exists(color: AnsiColor = None):
     return color.rgb if color is not None else None
 
-
 class ColoredString():
     def __init__(self, string: str, forecolor: tuple[int, int, int] = None, backcolor: tuple[int, int, int] = None, ctype: ColorType = ColorType.LEGACY):
         self.forecolor = AnsiColor(
             rgb=forecolor) if forecolor is not None else None
         self.backcolor = AnsiColor(
             rgb=backcolor, foreground=False) if backcolor is not None else None
         self.str = string
@@ -92,91 +91,80 @@
             return ColoredString(
                 string=self.str[__p.start:__p.stop:__p.step],
                 forecolor=get_rgb_if_exists(self.forecolor),
                 backcolor=get_rgb_if_exists(self.backcolor)
             )
 
     @overload
-    def __setitem__(self, __i: SupportsIndex, __o: str): ...
+    def __setitem__(self, __p: SupportsIndex, __o): ...
+
+    @overload
+    def __setitem__(self, __p: slice, __o): ...
 
     # @overload
     def __setitem__(self, __p, __o):
         if isinstance(__p, SupportsIndex):
-            if len(__o.str) != 1:
-                raise ValueError(
-                    "Shape mismatch! can not set one character of ColoredString to multiple characters.")
-
             if isinstance(__o, str):
                 self.str[__p] = __o
             elif isinstance(__o, ColoredString):
-                if self.forecolor == __o.forecolor and self.backcolor == __o.backcolor:
-                    self.str[__p] = __o.str
-                elif len(self.str) == 1:
-                    self.str = __o.str
+                if len(__o.str) != 1:
+                    raise ValueError("Shape mismatch! can not set an index of ColoredString to multiple characters.")
                 else:
-                    raise NotImplementedError(
-                        "Setting a part of ColoredString to another color is not supported!")
+                    if self.forecolor == __o.forecolor and self.backcolor == __o.backcolor:
+                        self.str[__p] = __o.str
+                    elif len(self.str) == 1:
+                        self.str = __o.str
+                    else:
+                        raise NotImplementedError("Setting an index of a `ColoredString` to another color is not supported!")
         elif isinstance(__p, slice):
             # the code below is comented because if there's a shape mismatch, this
             # will raise a ValueError for setting self.str anyways...
             # if len(__o.str) != len(self.strp[__p.start:__p.stop:__p.step]):
             #    raise ValueError("Shape mismatch! make sure to set to correct lenght.")
 
             if isinstance(__o, str):
                 self.str[__p.start:__p.stop:__p.step] = __o
             elif isinstance(__o, ColoredString):
                 if self.forecolor == __o.forecolor and self.backcolor == __o.backcolor:
                     self.str[__p.start:__p.stop:__p.step] = __o
                 elif len(self.str) == len(__o.str):
                     self.str = __o.str
                 else:
-                    raise NotImplementedError(
-                        "Setting a part of ColoredString to another color is not supported!")
-
-    # @overload
-    def __setitem__(self, __s: slice, __o):
-        if self.forecolor == __o.forecolor and self.backcolor == __o.backcolor:
-            new_str = self.str
-            new_str[__s.start:__s.stop:__s.step] = __o.str
-            return ColoredString(
-                string=new_str,
-                forecolor=get_rgb_if_exists(self.forecolor),
-                backcolor=get_rgb_if_exists(self.backcolor)
-            )
-        else:
-            assert __s.step == 1, "step is not supported when differentiating color!"
-            if self.str[:__s.start] != "":
-                cstr_1 = ColoredString(
-                    string=self.str[:__s.start],
-                    forecolor=get_rgb_if_exists(self.forecolor),
-                    backcolor=get_rgb_if_exists(self.backcolor)
-                )
-            else:
-                cstr_1 = None
-            cstr_2 = ColoredString(
-                string=__o.str,
-                forecolor=get_rgb_if_exists(__o.forecolor),
-                backcolor=get_rgb_if_exists(__o.backcolor)
-            )
-            if self.str[__s.stop+len(__o.str):] != "":
-                cstr_3 = ColoredString(
-                    string=self.str[__s.stop+len(__o.str):],
-                    forecolor=get_rgb_if_exists(self.forecolor),
-                    backcolor=get_rgb_if_exists(self.backcolor)
-                )
-            else:
-                cstr_3 = None
-
-            if cstr_3 is None and cstr_1 is None:
-                return cstr_2
-            else:
-                if cstr_3 is None:
-                    return ColoredStringList([cstr_1, cstr_2])
-                elif cstr_1 is None:
-                    return ColoredStringList([cstr_2, cstr_3])
+                    assert __p.step == 1, "step is not supported when differentiating colors!"
+                    if self.str[:__p.start] != "":
+                        cstr_pre = ColoredString(
+                            string=self.str[:__p.start],
+                            forecolor=get_rgb_if_exists(self.forecolor),
+                            backcolor=get_rgb_if_exists(self.backcolor)
+                        )
+                    else:
+                        cstr_pre = None
+                    cstr_center = ColoredString(
+                        string=__o.str,
+                        forecolor=get_rgb_if_exists(__o.forecolor),
+                        backcolor=get_rgb_if_exists(__o.backcolor)
+                    )
+                    if self.str[__p.stop+len(__o.str):] != "":
+                        cstr_post = ColoredString(
+                            string=self.str[__p.stop+len(__o.str):],
+                            forecolor=get_rgb_if_exists(self.forecolor),
+                            backcolor=get_rgb_if_exists(self.backcolor)
+                        )
+                    else:
+                        cstr_post = None
+
+                    # return the simplest representation
+                    if cstr_post is None and cstr_pre is None:
+                        return cstr_center
+                    elif cstr_post is None:
+                        return ColoredStringList([cstr_pre, cstr_center])
+                    elif cstr_pre is None:
+                        return ColoredStringList([cstr_center, cstr_post])
+                    else:
+                        return ColoredStringList([cstr_pre, cstr_center, cstr_post])
 
     @overload
     def __delitem__(self, __i: SupportsIndex): ...
 
     @overload
     def __delitem__(self, __s: slice): ...
 
@@ -191,14 +179,27 @@
     #        return self.str + other
     #    else:
     #        other_ = ColoredString(string=self.str + other)
     #        return ColoredStringList([self, other_])
     def __iadd__(self, other) -> str:
         return self + other
 
+# modify built-in string class
+# from forbiddenfruit import curse
+
+# def curse_str():
+#    def __add__(self, other: ColoredString):
+#        if isinstance(other, ColoredString):
+#            return ColoredString(self) + other
+#        elif isinstance(other, ColoredStringList):
+#            return ColoredString(self) + other
+#        else:
+#            return super(str, self).__add__(other)
+#    curse(str, "__add__", __add__)
+# curse_str()
 
 class ColoredStringList():
     def __init__(self, strings: ColoredString, ctype: ColorType = ColorType.LEGACY):
         self.strs: list[ColoredString] = strings
         self.ctype = ctype
 
     def copy(self):
@@ -237,48 +238,61 @@
 
     @overload
     def __add__(self, other: 'ColoredStringList') -> 'ColoredStringList': ...
 
     @overload
     def __add__(self, other: ColoredString) -> 'ColoredStringList': ...
 
+    @overload
+    def __add__(self, other: str) -> 'ColoredStringList': ...
+
     def __add__(self, other) -> str:
         if isinstance(other, ColoredStringList):
             return ColoredStringList(self.strs + other.strs)
         elif isinstance(other, ColoredString):
-            return ColoredStringList(self.strs + [other])
+            # return ColoredStringList(self.strs + [other]) (is not optimized)
+
+            # if self.strs[-1] + other can be optimized to a single ColoredString object
+            # this will return a ColoredString, else it will return a ColoredStringList
+            # the value then will be added to self.strs[:-1]
+            new_last = self.strs[-1] + other
+            if isinstance(new_last, ColoredString):
+                return ColoredStringList(self.strs[:-1] + [new_last])
+            elif isinstance(new_last, ColoredStringList):
+                return ColoredStringList(self.strs[:-1] + new_last.strs)
         elif isinstance(other, str):
-            other_ = ColoredString(string=other)
-            return ColoredStringList(self.strs + [other_])
+            return self + ColoredString(string=other)
         else:
             raise NotImplementedError(
-                f"Only supports \"+\" operand between a ColoredString or a ColoredStringList, but got {type(other)}")
+                f"`ColoredStringList` Only supports to be added to a \"ColoredString\", \"ColoredStringList\" or \"str\", but got \"{type(other)}\"")
 
     def __iadd__(self, other) -> str:
         return self + other
 
     @overload
     def __getitem__(self, __p: SupportsIndex): ...
 
     @overload
     def __getitem__(self, __s: slice): ...
 
     def __getitem__(self, __p):
         if isinstance(__p, SupportsIndex):
             p = 0
             for cstr in self.strs:
-                if len(cstr) <= 0:
+                # if cstr is empty continue (this should never happen but we want to be optimized)
+                if len(cstr) == 0:
                     continue
                 if (__p - p - len(cstr)) < 0:
                     r = cstr[__p-p]
                     return r
                 else:
                     p += len(cstr)
-            return None
+            raise IndexError("Index out of range!")
         elif isinstance(__p, slice):
+            # TODO: optimize this
             st = 0 if __p.start is None else __p.start
             et = len(self) if __p.stop is None else __p.stop
             s = 1 if __p.step is None else __p.step
             r = ColoredString("")
             for i in range(st, et, s):
                 r += self[i]
             return r
@@ -475,21 +489,27 @@
             return
     
     def center_place_drawer(self, other_drawer: 'Drawer', ln_idx: int, borderless: bool = True):
         idx = (self.w - other_drawer.w)//2
         self.place_drawer(other_drawer, pos=(idx, ln_idx), borderless = borderless)
 
 if __name__ == "__main__":
+    #result = "test" + (ColoredString("will this work?") + ColoredString("will this work?", forecolor=(0, 255, 0)))
+    #print(result)
+
     # test = ColoredString("test ", forecolor=(0, 100, 200)) + ColoredString("for ", forecolor=(0, 100, 200)) + ColoredString("colors", forecolor=(0, 100, 200), backcolor=(200, 100, 200))
     tsize = ansi.get_size()
     screen = Drawer(size=(tsize.columns, tsize.lines))
     drawer = Drawer(size=(31, 5))
     drawer.write_text("Hello, World!", ((drawer.w-13)//2, 2))
     # painter.place(ColoredString("Hello, World!", forecolor=(200, 100, 0)), (8, 5))
     welcome_text = ColoredString("-"*((drawer.w-15)//2)+"[", forecolor=(0, 255, 0)) + ColoredString(
         "Welcome", forecolor=(255, 255, 0)) + ColoredString("]"+"-"*((drawer.w-15)//2), forecolor=(0, 255, 0))
+    test_text = ColoredString("-"*((drawer.w-15)//2)+"[", forecolor=(0, 255, 0)) + ColoredString(
+        "TEST", forecolor=(255, 255, 0)) + ColoredString("]"+"-"*((drawer.w-15)//2), forecolor=(0, 0, 0))
     drawer.center_place(welcome_text, ln_idx=1)
+    drawer.place(test_text, pos=(0, 1))
     # print(type(drawer))
     screen.center_place_drawer(drawer, 10, borderless = False)
     ansi.write(screen.tostring(ctype=ColorType.TRUECOLOR))
     ansi.flush()
-    ansi.read()
+    input()
```

### Comparing `pybud-gui-0.9.5/src/pybud/gui/gui.py` & `pybud-gui-0.9.6/src/pybud/gui/dialog.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,121 +10,121 @@
     print("Unable to find dependency module named 'readchar', install using 'pip install readchar'")
     exit(1)
 
 import pybud.ansi as ansi
 from pybud.drawer import ColoredString as CStr
 from pybud.drawer import ColorType, Drawer
 from .widgets import Widget
-from .utils import DEFAULT_BACKGROUND_COLOR
+from ..deftypes import DEFAULT_BACKGROUND_COLOR
 
 LAST_SHOWN_DRAWABLE = None
+# ticks per second
+TPS = 20
 
 class Drawable():
     def __init__(self, ctype: ColorType = None):
         self.ctype = ctype
         self.width = None
         self.height = None
         self.background_color = DEFAULT_BACKGROUND_COLOR
         self.is_disabled = False
         self.closed = True
+        self.drawer: Drawer = None
         self.drawing = False
-        #self.last_update = 0
-        
+        # self.last_update = 0
+        self.tickupdate_thread: Thread = None
         self.tickupdate_started = False
-    
+
     def onClose(self):
         self.close()
 
     def close(self):
         self.closed = True
         while self.tickupdate_thread.is_alive():
-            time.sleep(1/20)
+            time.sleep(0.01)
         self.tickupdate_started = False
         ansi.go_up(self.height)
         ansi.write(("\n" + " " * self.width) * (self.height))
         ansi.write(f"\033M" * self.height)
         ansi.write(f"\r" + " " * self.width)
         ansi.write(f"\033M\n")
-        
 
     def update(self, key: str):
-        # fix a race condition that breaks refreshing the drawable
-        
         if key == Key.CTRL_C:
             self.onClose()
         if key == Key.ESC:
             self.onClose()
         return key
 
     def doTickUpdates(self):
         t = time.time()
         while not self.closed:
-            time.sleep(max(0, 1/20 - (time.time() - t)))
+            time.sleep(max(0, 1/TPS - (time.time() - t)))
             self.update("UPDATE")
-            t = time.time() 
-            
-    
+            t = time.time()
+
     def doKeyUpdates(self):
         while not self.closed:
             try:
                 key = readkey()
             except KeyboardInterrupt:
                 key = Key.CTRL_C
             self.update(key)
-            
 
     def show(self):
         global LAST_SHOWN_DRAWABLE
         LAST_SHOWN_DRAWABLE = self
+
         self.closed = False
 
         ansi.write("\n" * self.height)
         self.draw()
-        
+
         if not self.tickupdate_started:
             self.tickupdate_thread = Thread(target=self.doTickUpdates)
             self.tickupdate_thread.start()
             self.tickupdate_started = True
         self.doKeyUpdates()
 
     def get_drawer(self):
-        self.drawing = True
         return Drawer(size=(self.width, self.height), background_color=self.background_color)
 
     def draw(self):
         if not self.closed:
+            self.drawing = True
             self.drawer = self.get_drawer()
 
-class AutoDialouge(Drawable):
-    def __init__(self, width: int, ctype: ColorType = None, mode:str = "v"):
+
+class DialogBase(Drawable):
+    def __init__(self, width: int, ctype: ColorType = None, background_color: ColorType = None):
         super().__init__(ctype)
         self.width = width
-        self.height = 3
+        self.background_color = background_color
         self.widgets: List[Widget] = []
         self.set_active_widget(0)
         self.result = None
         self.tick = 0
-        self.mode = mode
+        self.totw = 0
 
     def update_height(self):
         max_height = 0
         for w in self.widgets:
             widget_height = w.pos.getY() + w.size.getHeight()
             if widget_height > max_height:
                 max_height = widget_height
 
-        # set the height to one line more than the end of most buttom added dialouge
+        # set the height to one line more than the end of most buttom added dialog
         self.height = max_height + 1
 
     def add_widget(self, w: Widget):
-        w.parent = self
+        w.on_add(self)
         self.widgets.append(w)
         # self.height += w.size.getHeight()
         self.update_height()
-        
+        self.totw = self.get_total_selectable_widgets()
 
     def get_total_selectable_widgets(self):
         i = 0
         for w in self.widgets:
             if w.selectable:
                 i += 1
         return i
@@ -152,92 +152,116 @@
 
             if i == __i:
                 w.is_disabled = False
             else:
                 w.is_disabled = True
             i += 1
 
-    def on_enter(self):
-        return self.run_callbacks()
-
-    def run_callbacks(self):
-        w, active_i = self.get_active_widget(True)
-        if w is not None:
-            self.result = w.run_callbacks()
-
-    def update(self, key):
+    def update(self, key, draw=True):
         key = super().update(key)
-        if key == Key.ENTER:
-            self.on_enter()
-            return
 
         w, i = self.get_active_widget(True)
         if w is not None:
             key = w.update(key)
+            self.result = w.result
 
         if key == Key.TAB:
-            self.set_active_widget(
-                (i + 1) % self.get_total_selectable_widgets())
+            self.set_active_widget((i + 1) % self.totw)
+
+        if key == "UPDATE":
+            self.tick += 1
+
+        if draw:
+            self.draw()
+        else:
+            return key
+
+    def draw_widgets(self, drawer: Drawer):
+        active_w = self.get_active_widget()
+        for w in self.widgets:
+            border = w is active_w
+            w_render = w.get_render()
+            drawer.place_drawer(
+                w_render, (w.pos.getX(), w.pos.getY()), borderless=not border)
+        return drawer
+
+    def render(self):
+        self.drawer = self.draw_widgets(self.drawer)
+
+    def draw(self):
+        if self.closed or self.drawing:
+            return
+        super().draw()
+        self.render()
+        ansi.go_up(self.height)
+        ansi.write(self.drawer.tostring(self.ctype) + "\n")
+        ansi.flush()
+        # time.sleep(0.01)
+        self.drawing = False
+
+    def show(self):
+        super().show()
+        return self.result
+
+    def __str__(self):
+        s = "+ " + self.__class__.__name__ + ":\n"
+        for w in self.widgets:
+            s += "|   " + w.name + "\n"
+        return s
+
+
+class AutoDialog(DialogBase):
+    def __init__(self, width: int, ctype: ColorType = None, background_color: ColorType = None, mode: str = "v"):
+        super().__init__(width, ctype)
+        assert mode in ["v", "iv", "h", "ih"], f"Unknown mode \"{mode}\"!"
+        self.mode = mode.lower()
+        self.background_color = background_color
+
+    def update(self, key):
+        key = super().update(key, draw=False)
+        if key == None:
+            self.draw()
+            return
+
+        w, i = self.get_active_widget(True)
+        if w is None:
+            return
 
-        if self.mode.lower() == "v":
+        av = i
+        if self.mode == "v":
             if key == Key.UP:
-                self.set_active_widget(
-                    (i - 1) % self.get_total_selectable_widgets())
+                av = (i - 1) % self.totw 
             elif key == Key.DOWN:
-                self.set_active_widget(
-                    (i + 1) % self.get_total_selectable_widgets())
-        
-        if self.mode.lower() == "iv":
+                av = (i + 1) % self.totw
+        elif self.mode == "iv":
             if key == Key.DOWN:
-                self.set_active_widget(
-                    (i + 1) % self.get_total_selectable_widgets())
+                av = (i + 1) % self.totw
             elif key == Key.UP:
-                self.set_active_widget(
-                    (i + 1) % self.get_total_selectable_widgets())
-
-        if self.mode.lower() == "h":
+                av = (i + 1) % self.totw
+        elif self.mode == "h":
             if key == Key.LEFT:
-                self.set_active_widget(
-                    (i + 1) % self.get_total_selectable_widgets())
+                av = (i - 1) % self.totw
             elif key == Key.RIGHT:
-                self.set_active_widget(
-                    (i + 1) % self.get_total_selectable_widgets())
-        
-        if self.mode.lower() == "ih":
+                av = (i + 1) % self.totw
+        elif self.mode == "ih":
             if key == Key.RIGHT:
-                self.set_active_widget(
-                    (i + 1) % self.get_total_selectable_widgets())
+                av = (i + 1) % self.totw
             elif key == Key.LEFT:
-                self.set_active_widget(
-                    (i + 1) % self.get_total_selectable_widgets())
-        
-        if key == "UPDATE":
-            self.tick += 1
+                av = (i - 1) % self.totw
+        else:
+            raise ValueError(f"Unknown mode \"{self.mode}\"!")
         
+        self.set_active_widget(av)
         self.draw()
 
-    def draw(self):
-        if self.closed or self.drawing:
-            return
-        super().draw()
+    def render(self):
+        super().render()
         animation = "▁▂▃▄▅▆▆▅▄▃▂▁▂ "
-        def getadmination(tick, n = 3):
+
+        def get_admination(tick, n=3):
             rt = tick
             return animation[rt % (len(animation)-n):rt % (len(animation)-n)+n]
-        self.drawer.place(CStr(getadmination(self.tick)), pos = (1, 0))
-        w, active_i = self.get_active_widget(True)
-        ansi.go_up(self.height)
-        i = 0
-        for w in self.widgets:
-            border = w.selectable and i == active_i
-            if w.selectable:
-                i += 1
-            self.drawer.place_drawer(
-                w.get_render(), (w.pos.getX(), w.pos.getY()), borderless=not border)
-        ansi.write(self.drawer.tostring(self.ctype) + "\n")
-        ansi.flush()
-        #time.sleep(0.01)
-        self.drawing = False
+        self.drawer.place(CStr(get_admination(self.tick)), pos=(1, 0))
 
     def show(self):
         super().show()
         return self.result
```

### Comparing `pybud-gui-0.9.5/src/pybud/gui/utils.py` & `pybud-gui-0.9.6/src/pybud/deftypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-DEFAULT_BACKGROUND_COLOR =  None#(50, 120, 200)
+DEFAULT_BACKGROUND_COLOR = None  # (50, 120, 200)
+
 
 class Point:
     def __init__(self, x: int = 0, y: int = 0) -> None:
         assert x >= 0
         assert y >= 0
         self.x = x
         self.y = y
```

### Comparing `pybud-gui-0.9.5/src/pybud/gui/widgets.py` & `pybud-gui-0.9.6/src/pybud/gui/widgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,622 +6,661 @@
 00000050: 7765 7220 696d 706f 7274 2043 6f6c 6f72  wer import Color
 00000060: 6564 5374 7269 6e67 4c69 7374 2061 7320  edStringList as 
 00000070: 4353 7472 4c69 7374 0d0a 6672 6f6d 2070  CStrList..from p
 00000080: 7962 7564 2e64 7261 7765 7220 696d 706f  ybud.drawer impo
 00000090: 7274 2043 6f6c 6f72 5479 7065 2c20 4472  rt ColorType, Dr
 000000a0: 6177 6572 0d0a 6672 6f6d 2072 6561 6463  awer..from readc
 000000b0: 6861 7220 696d 706f 7274 206b 6579 2061  har import key a
-000000c0: 7320 4b65 790d 0a0d 0a66 726f 6d20 2e75  s Key....from .u
-000000d0: 7469 6c73 2069 6d70 6f72 7420 506f 696e  tils import Poin
-000000e0: 742c 2053 697a 652c 2044 4546 4155 4c54  t, Size, DEFAULT
-000000f0: 5f42 4143 4b47 524f 554e 445f 434f 4c4f  _BACKGROUND_COLO
-00000100: 520d 0a0d 0a0d 0a63 6c61 7373 2057 6964  R......class Wid
-00000110: 6765 7442 6173 6528 293a 0d0a 2020 2020  getBase():..    
-00000120: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00000130: 662c 2063 7479 7065 3a20 436f 6c6f 7254  f, ctype: ColorT
-00000140: 7970 6520 3d20 4e6f 6e65 2c20 7369 7a65  ype = None, size
-00000150: 3a20 5369 7a65 203d 204e 6f6e 652c 2070  : Size = None, p
-00000160: 6f73 3a20 506f 696e 7420 3d20 506f 696e  os: Point = Poin
-00000170: 7428 302c 2030 2929 3a0d 0a20 2020 2020  t(0, 0)):..     
-00000180: 2020 2023 2073 6574 2076 6172 6961 626c     # set variabl
-00000190: 6564 0d0a 2020 2020 2020 2020 7365 6c66  ed..        self
-000001a0: 2e63 7479 7065 203d 2063 7479 7065 0d0a  .ctype = ctype..
-000001b0: 2020 2020 2020 2020 7365 6c66 2e73 697a          self.siz
-000001c0: 6520 3d20 5369 7a65 2831 302c 2032 3029  e = Size(10, 20)
-000001d0: 2069 6620 7369 7a65 2069 7320 4e6f 6e65   if size is None
-000001e0: 2065 6c73 6520 7369 7a65 0d0a 2020 2020   else size..    
-000001f0: 2020 2020 7365 6c66 2e70 6f73 203d 2050      self.pos = P
-00000200: 6f69 6e74 2830 2c20 3029 2069 6620 706f  oint(0, 0) if po
-00000210: 7320 6973 204e 6f6e 6520 656c 7365 2070  s is None else p
-00000220: 6f73 0d0a 2020 2020 2020 2020 2320 6465  os..        # de
-00000230: 6661 756c 7473 0d0a 2020 2020 2020 2020  faults..        
-00000240: 7365 6c66 2e62 6163 6b67 726f 756e 645f  self.background_
-00000250: 636f 6c6f 7220 3d20 4445 4641 554c 545f  color = DEFAULT_
-00000260: 4241 434b 4752 4f55 4e44 5f43 4f4c 4f52  BACKGROUND_COLOR
-00000270: 0d0a 0d0a 2020 2020 6465 6620 6f6e 5f69  ....    def on_i
-00000280: 6e74 6572 7275 7074 2873 656c 6629 3a0d  nterrupt(self):.
-00000290: 0a20 2020 2020 2020 2070 6173 730d 0a0d  .        pass...
-000002a0: 0a20 2020 2064 6566 2067 6574 5f64 7261  .    def get_dra
-000002b0: 7765 7228 7365 6c66 293a 0d0a 2020 2020  wer(self):..    
-000002c0: 2020 2020 7265 7475 726e 2044 7261 7765      return Drawe
-000002d0: 7228 7369 7a65 3d28 7365 6c66 2e73 697a  r(size=(self.siz
-000002e0: 652e 6765 7457 6964 7468 2829 2c20 7365  e.getWidth(), se
-000002f0: 6c66 2e73 697a 652e 6765 7448 6569 6768  lf.size.getHeigh
-00000300: 7428 2929 2c20 6261 636b 6772 6f75 6e64  t()), background
-00000310: 5f63 6f6c 6f72 3d73 656c 662e 6261 636b  _color=self.back
-00000320: 6772 6f75 6e64 5f63 6f6c 6f72 290d 0a0d  ground_color)...
-00000330: 0a20 2020 2064 6566 2072 656e 6465 7228  .    def render(
-00000340: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00000350: 7061 7373 0d0a 0d0a 2020 2020 6465 6620  pass....    def 
-00000360: 6765 745f 7265 6e64 6572 2873 656c 6629  get_render(self)
-00000370: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-00000380: 6472 6177 6572 203d 2073 656c 662e 6765  drawer = self.ge
-00000390: 745f 6472 6177 6572 2829 0d0a 2020 2020  t_drawer()..    
-000003a0: 2020 2020 7365 6c66 2e72 656e 6465 7228      self.render(
-000003b0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-000003c0: 6e20 7365 6c66 2e64 7261 7765 720d 0a0d  n self.drawer...
-000003d0: 0a20 2020 2064 6566 2075 7064 6174 6528  .    def update(
-000003e0: 7365 6c66 2c20 6b65 7929 3a0d 0a20 2020  self, key):..   
-000003f0: 2020 2020 2072 6574 7572 6e20 6b65 790d       return key.
-00000400: 0a0d 0a0d 0a63 6c61 7373 2057 6964 6765  .....class Widge
-00000410: 7428 5769 6467 6574 4261 7365 293a 0d0a  t(WidgetBase):..
-00000420: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00000430: 2873 656c 662c 2063 7479 7065 3a20 436f  (self, ctype: Co
-00000440: 6c6f 7254 7970 6520 3d20 4e6f 6e65 2c20  lorType = None, 
-00000450: 7369 7a65 3a20 5369 7a65 203d 204e 6f6e  size: Size = Non
-00000460: 652c 2070 6f73 3a20 506f 696e 7420 3d20  e, pos: Point = 
-00000470: 506f 696e 7428 302c 2030 2929 3a0d 0a20  Point(0, 0)):.. 
-00000480: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
-00000490: 5f69 6e69 745f 5f28 6374 7970 652c 2073  _init__(ctype, s
-000004a0: 697a 652c 2070 6f73 290d 0a20 2020 2020  ize, pos)..     
-000004b0: 2020 2023 2064 6566 6175 6c74 730d 0a20     # defaults.. 
-000004c0: 2020 2020 2020 2073 656c 662e 6973 5f64         self.is_d
-000004d0: 6973 6162 6c65 6420 3d20 4661 6c73 650d  isabled = False.
-000004e0: 0a20 2020 2020 2020 2073 656c 662e 6973  .        self.is
-000004f0: 5f73 656c 6563 7465 6420 3d20 4661 6c73  _selected = Fals
-00000500: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00000510: 7365 6c65 6374 6162 6c65 203d 2054 7275  selectable = Tru
-00000520: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00000530: 7061 7265 6e74 203d 204e 6f6e 650d 0a0d  parent = None...
-00000540: 0a20 2020 2064 6566 2072 756e 5f63 616c  .    def run_cal
-00000550: 6c62 6163 6b73 2873 656c 6629 3a0d 0a20  lbacks(self):.. 
-00000560: 2020 2020 2020 2070 6173 730d 0a0d 0a20         pass.... 
-00000570: 2020 2064 6566 206f 6e5f 656e 7465 7228     def on_enter(
-00000580: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00000590: 7265 7475 726e 2073 656c 662e 7275 6e5f  return self.run_
-000005a0: 6361 6c6c 6261 636b 7328 290d 0a0d 0a20  callbacks().... 
-000005b0: 2020 2064 6566 206f 6e5f 696e 7465 7272     def on_interr
-000005c0: 7570 7428 7365 6c66 293a 0d0a 2020 2020  upt(self):..    
-000005d0: 2020 2020 7375 7065 7228 292e 6f6e 5f69      super().on_i
-000005e0: 6e74 6572 7275 7074 2829 0d0a 2020 2020  nterrupt()..    
-000005f0: 2020 2020 7365 6c66 2e69 735f 6469 7361      self.is_disa
-00000600: 626c 6564 203d 2054 7275 650d 0a0d 0a20  bled = True.... 
-00000610: 2020 2064 6566 2075 7064 6174 6528 7365     def update(se
-00000620: 6c66 2c20 6b65 7929 3a0d 0a20 2020 2020  lf, key):..     
-00000630: 2020 206b 6579 203d 2073 7570 6572 2829     key = super()
-00000640: 2e75 7064 6174 6528 6b65 7929 0d0a 2020  .update(key)..  
-00000650: 2020 2020 2020 6966 206b 6579 203d 3d20        if key == 
-00000660: 4b65 792e 454e 5445 523a 0d0a 2020 2020  Key.ENTER:..    
-00000670: 2020 2020 2020 2020 7365 6c66 2e6f 6e5f          self.on_
-00000680: 656e 7465 7228 290d 0a20 2020 2020 2020  enter()..       
-00000690: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-000006a0: 2020 2020 2072 6574 7572 6e20 6b65 790d       return key.
-000006b0: 0a0d 0a0d 0a63 6c61 7373 2055 6e73 656c  .....class Unsel
-000006c0: 6563 7461 626c 6557 6964 6765 7428 5769  ectableWidget(Wi
-000006d0: 6467 6574 4261 7365 293a 0d0a 2020 2020  dgetBase):..    
-000006e0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-000006f0: 662c 2063 7479 7065 3a20 436f 6c6f 7254  f, ctype: ColorT
-00000700: 7970 6520 3d20 4e6f 6e65 2c20 7369 7a65  ype = None, size
-00000710: 3a20 5369 7a65 203d 204e 6f6e 652c 2070  : Size = None, p
-00000720: 6f73 3a20 506f 696e 7420 3d20 506f 696e  os: Point = Poin
-00000730: 7428 302c 2030 2929 3a0d 0a20 2020 2020  t(0, 0)):..     
-00000740: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-00000750: 745f 5f28 6374 7970 652c 2073 697a 652c  t__(ctype, size,
-00000760: 2070 6f73 290d 0a20 2020 2020 2020 2073   pos)..        s
-00000770: 656c 662e 7365 6c65 6374 6162 6c65 203d  elf.selectable =
-00000780: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00000790: 7365 6c66 2e69 735f 7365 6c65 6374 6564  self.is_selected
-000007a0: 203d 2046 616c 7365 0d0a 0d0a 0d0a 636c   = False......cl
-000007b0: 6173 7320 5769 6467 6574 4c61 6265 6c28  ass WidgetLabel(
-000007c0: 556e 7365 6c65 6374 6162 6c65 5769 6467  UnselectableWidg
-000007d0: 6574 293a 0d0a 2020 2020 6465 6620 5f5f  et):..    def __
-000007e0: 696e 6974 5f5f 2873 656c 662c 0d0a 2020  init__(self,..  
-000007f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00000800: 6578 742c 0d0a 2020 2020 2020 2020 2020  ext,..          
-00000810: 2020 2020 2020 2063 656e 7465 7265 643a         centered:
-00000820: 2062 6f6f 6c20 3d20 5472 7565 2c0d 0a20   bool = True,.. 
-00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000840: 776f 7264 7772 6170 3a20 626f 6f6c 203d  wordwrap: bool =
-00000850: 2054 7275 652c 0d0a 2020 2020 2020 2020   True,..        
-00000860: 2020 2020 2020 2020 2073 697a 653a 2053           size: S
-00000870: 697a 6520 3d20 4e6f 6e65 2c0d 0a20 2020  ize = None,..   
-00000880: 2020 2020 2020 2020 2020 2020 2020 706f                po
-00000890: 733a 2050 6f69 6e74 203d 2050 6f69 6e74  s: Point = Point
-000008a0: 2830 2c20 3029 2c0d 0a20 2020 2020 2020  (0, 0),..       
-000008b0: 2020 2020 2020 2020 2020 6374 7970 653a            ctype:
-000008c0: 2043 6f6c 6f72 5479 7065 203d 204e 6f6e   ColorType = Non
-000008d0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-000008e0: 2020 2020 293a 0d0a 0d0a 2020 2020 2020      ):....      
-000008f0: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-00000900: 5f5f 2863 7479 7065 2c20 7369 7a65 2c20  __(ctype, size, 
-00000910: 706f 7329 0d0a 0d0a 2020 2020 2020 2020  pos)....        
-00000920: 6966 2069 7369 6e73 7461 6e63 6528 7465  if isinstance(te
-00000930: 7874 2c20 7374 7229 3a0d 0a20 2020 2020  xt, str):..     
-00000940: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
-00000950: 203d 2043 5374 7228 7465 7874 2c20 666f   = CStr(text, fo
-00000960: 7265 636f 6c6f 723d 2832 3230 2c20 3232  recolor=(220, 22
-00000970: 302c 2032 3230 2929 0d0a 2020 2020 2020  0, 220))..      
-00000980: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00000990: 6528 7465 7874 2c20 4353 7472 2920 6f72  e(text, CStr) or
-000009a0: 2069 7369 6e73 7461 6e63 6528 7465 7874   isinstance(text
-000009b0: 2c20 4353 7472 4c69 7374 293a 0d0a 2020  , CStrList):..  
-000009c0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-000009d0: 6578 7420 3d20 7465 7874 0d0a 2020 2020  ext = text..    
-000009e0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000009f0: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-00000a00: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-00000a10: 2829 0d0a 0d0a 2020 2020 2020 2020 7365  ()....        se
-00000a20: 6c66 2e73 697a 652e 6820 3d20 286c 656e  lf.size.h = (len
-00000a30: 2874 6578 7429 202f 2f20 2873 656c 662e  (text) // (self.
-00000a40: 7369 7a65 2e77 202d 2038 2929 202b 2031  size.w - 8)) + 1
-00000a50: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-00000a60: 656e 7465 7265 6420 3d20 6365 6e74 6572  entered = center
-00000a70: 6564 0d0a 2020 2020 2020 2020 7365 6c66  ed..        self
-00000a80: 2e77 6f72 6477 7261 7020 3d20 776f 7264  .wordwrap = word
-00000a90: 7772 6170 0d0a 0d0a 2020 2020 6465 6620  wrap....    def 
-00000aa0: 7275 6e5f 6361 6c6c 6261 636b 7328 7365  run_callbacks(se
-00000ab0: 6c66 293a 0d0a 2020 2020 2020 2020 7061  lf):..        pa
-00000ac0: 7373 0d0a 0d0a 2020 2020 6465 6620 5f70  ss....    def _p
-00000ad0: 6c61 6365 5f74 6578 7428 7365 6c66 2c20  lace_text(self, 
-00000ae0: 7465 7874 2c20 6c6e 5f69 6478 293a 0d0a  text, ln_idx):..
-00000af0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00000b00: 6365 6e74 6572 6564 3a0d 0a20 2020 2020  centered:..     
-00000b10: 2020 2020 2020 2073 656c 662e 6472 6177         self.draw
-00000b20: 6572 2e63 656e 7465 725f 706c 6163 6528  er.center_place(
-00000b30: 7465 7874 2c20 6c6e 5f69 6478 3d6c 6e5f  text, ln_idx=ln_
-00000b40: 6964 7829 0d0a 2020 2020 2020 2020 656c  idx)..        el
-00000b50: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00000b60: 2073 656c 662e 6472 6177 6572 2e70 6c61   self.drawer.pla
-00000b70: 6365 2874 6578 742c 2070 6f73 3d28 302c  ce(text, pos=(0,
-00000b80: 206c 6e5f 6964 7829 290d 0a0d 0a20 2020   ln_idx))....   
-00000b90: 2064 6566 2070 6c61 6365 5f74 6578 7428   def place_text(
-00000ba0: 7365 6c66 2c20 742c 206c 6e5f 6964 7829  self, t, ln_idx)
-00000bb0: 3a0d 0a20 2020 2020 2020 2023 7072 696e  :..        #prin
-00000bc0: 7428 7429 0d0a 2020 2020 2020 2020 6966  t(t)..        if
-00000bd0: 206c 656e 2874 2920 3e20 2873 656c 662e   len(t) > (self.
-00000be0: 7369 7a65 2e67 6574 5769 6474 6828 2920  size.getWidth() 
-00000bf0: 2d20 3829 3a0d 0a20 2020 2020 2020 2020  - 8):..         
-00000c00: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00000c10: 6528 6c65 6e28 7429 293a 0d0a 2020 2020  e(len(t)):..    
-00000c20: 2020 2020 2020 2020 2020 2020 695f 203d              i_ =
-00000c30: 206c 656e 2874 2920 2d20 6920 2d20 310d   len(t) - i - 1.
-00000c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c50: 2069 6620 695f 203e 2028 7365 6c66 2e73   if i_ > (self.s
-00000c60: 697a 652e 6765 7457 6964 7468 2829 202d  ize.getWidth() -
-00000c70: 2038 293a 0d0a 2020 2020 2020 2020 2020   8):..          
-00000c80: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00000c90: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00000ca0: 2020 2020 6320 3d20 745b 695f 5d0d 0a20      c = t[i_].. 
-00000cb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00000cc0: 6620 6973 696e 7374 616e 6365 2863 2c20  f isinstance(c, 
-00000cd0: 7374 7229 2061 6e64 2063 203d 3d20 2220  str) and c == " 
-00000ce0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-00000cf0: 2020 2020 2020 2020 7365 6c66 2e5f 706c          self._pl
-00000d00: 6163 655f 7465 7874 2874 5b3a 695f 5d2c  ace_text(t[:i_],
-00000d10: 206c 6e5f 6964 7829 0d0a 2020 2020 2020   ln_idx)..      
-00000d20: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00000d30: 7475 726e 2073 656c 662e 706c 6163 655f  turn self.place_
-00000d40: 7465 7874 2874 5b69 5f2b 313a 5d2c 206c  text(t[i_+1:], l
-00000d50: 6e5f 6964 7820 2b20 3129 0d0a 2020 2020  n_idx + 1)..    
-00000d60: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00000d70: 7369 6e73 7461 6e63 6528 632c 2043 5374  sinstance(c, CSt
-00000d80: 7229 2061 6e64 2063 2e73 7472 203d 3d20  r) and c.str == 
-00000d90: 2220 223a 0d0a 2020 2020 2020 2020 2020  " ":..          
-00000da0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00000db0: 706c 6163 655f 7465 7874 2874 5b3a 695f  place_text(t[:i_
-00000dc0: 5d2c 206c 6e5f 6964 7829 0d0a 2020 2020  ], ln_idx)..    
-00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000de0: 7265 7475 726e 2073 656c 662e 706c 6163  return self.plac
-00000df0: 655f 7465 7874 2874 5b69 5f2b 313a 5d2c  e_text(t[i_+1:],
-00000e00: 206c 6e5f 6964 7820 2b20 3129 0d0a 2020   ln_idx + 1)..  
-00000e10: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00000e20: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
-00000e30: 6c61 6365 5f74 6578 7428 742c 206c 6e5f  lace_text(t, ln_
-00000e40: 6964 7829 0d0a 0d0a 2020 2020 6465 6620  idx)....    def 
-00000e50: 7265 6e64 6572 2873 656c 6629 3a0d 0a20  render(self):.. 
-00000e60: 2020 2020 2020 2073 656c 662e 706c 6163         self.plac
-00000e70: 655f 7465 7874 2873 656c 662e 7465 7874  e_text(self.text
-00000e80: 2c20 6c6e 5f69 6478 3d30 290d 0a0d 0a0d  , ln_idx=0).....
-00000e90: 0a63 6c61 7373 2057 6964 6765 744f 7074  .class WidgetOpt
-00000ea0: 696f 6e73 2857 6964 6765 7429 3a0d 0a20  ions(Widget):.. 
-00000eb0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00000ec0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-00000ed0: 2020 2020 2020 2020 6f70 7469 6f6e 733a          options:
-00000ee0: 206c 6973 745b 7475 706c 655b 7374 722c   list[tuple[str,
-00000ef0: 2074 7970 6573 2e46 756e 6374 696f 6e54   types.FunctionT
-00000f00: 7970 655d 5d2c 0d0a 2020 2020 2020 2020  ype]],..        
-00000f10: 2020 2020 2020 2020 2074 6578 743a 2073           text: s
-00000f20: 7472 203d 2022 4f70 7469 6f6e 733a 222c  tr = "Options:",
-00000f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000f40: 2020 2064 6566 6175 6c74 5f6f 7074 696f     default_optio
-00000f50: 6e3a 2069 6e74 203d 2030 2c0d 0a20 2020  n: int = 0,..   
-00000f60: 2020 2020 2020 2020 2020 2020 2020 7369                si
-00000f70: 7a65 3a20 5369 7a65 203d 204e 6f6e 652c  ze: Size = None,
-00000f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000f90: 2020 2070 6f73 3a20 506f 696e 7420 3d20     pos: Point = 
-00000fa0: 506f 696e 7428 302c 2030 292c 0d0a 2020  Point(0, 0),..  
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00000fc0: 7479 7065 3a20 436f 6c6f 7254 7970 6520  type: ColorType 
-00000fd0: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-00000fe0: 2020 2020 2020 2020 2029 3a0d 0a0d 0a20           ):.... 
-00000ff0: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
-00001000: 5f69 6e69 745f 5f28 6374 7970 652c 2073  _init__(ctype, s
-00001010: 697a 652c 2070 6f73 290d 0a20 2020 2020  ize, pos)..     
-00001020: 2020 2073 656c 662e 6e5f 6f70 7469 6f6e     self.n_option
-00001030: 7320 3d20 6c65 6e28 6f70 7469 6f6e 7329  s = len(options)
-00001040: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
-00001050: 7074 696f 6e73 203d 206c 6973 7428 6d61  ptions = list(ma
-00001060: 7028 6c61 6d62 6461 2078 3a20 785b 305d  p(lambda x: x[0]
-00001070: 2c20 6f70 7469 6f6e 7329 290d 0a20 2020  , options))..   
-00001080: 2020 2020 2073 656c 662e 7465 7874 203d       self.text =
-00001090: 2074 6578 740d 0a20 2020 2020 2020 2073   text..        s
-000010a0: 656c 662e 6361 6c6c 6261 636b 7320 3d20  elf.callbacks = 
-000010b0: 6c69 7374 286d 6170 286c 616d 6264 6120  list(map(lambda 
-000010c0: 783a 2078 5b31 5d2c 206f 7074 696f 6e73  x: x[1], options
-000010d0: 2929 0d0a 2020 2020 2020 2020 7365 6c66  ))..        self
-000010e0: 2e73 656c 6563 7465 6420 3d20 6465 6661  .selected = defa
-000010f0: 756c 745f 6f70 7469 6f6e 0d0a 2020 2020  ult_option..    
-00001100: 2020 2020 7365 6c66 2e73 697a 652e 6820      self.size.h 
-00001110: 3d20 3120 2b20 7365 6c66 2e6e 5f6f 7074  = 1 + self.n_opt
-00001120: 696f 6e73 0d0a 0d0a 2020 2020 6465 6620  ions....    def 
-00001130: 7275 6e5f 6361 6c6c 6261 636b 7328 7365  run_callbacks(se
-00001140: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-00001150: 7475 726e 2073 656c 662e 6361 6c6c 6261  turn self.callba
-00001160: 636b 735b 7365 6c66 2e73 656c 6563 7465  cks[self.selecte
-00001170: 645d 2873 656c 662e 7061 7265 6e74 290d  d](self.parent).
-00001180: 0a0d 0a20 2020 2064 6566 2075 7064 6174  ...    def updat
-00001190: 6528 7365 6c66 2c20 6b65 7929 3a0d 0a20  e(self, key):.. 
-000011a0: 2020 2020 2020 206b 6579 203d 2073 7570         key = sup
-000011b0: 6572 2829 2e75 7064 6174 6528 6b65 7929  er().update(key)
-000011c0: 0d0a 2020 2020 2020 2020 6966 206b 6579  ..        if key
-000011d0: 203d 3d20 4b65 792e 5550 3a0d 0a20 2020   == Key.UP:..   
-000011e0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000011f0: 6c65 6374 6564 203d 2028 7365 6c66 2e73  lected = (self.s
-00001200: 656c 6563 7465 6420 2d20 3129 2025 2073  elected - 1) % s
-00001210: 656c 662e 6e5f 6f70 7469 6f6e 730d 0a20  elf.n_options.. 
-00001220: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001230: 6e0d 0a20 2020 2020 2020 2069 6620 6b65  n..        if ke
-00001240: 7920 3d3d 204b 6579 2e44 4f57 4e3a 0d0a  y == Key.DOWN:..
-00001250: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001260: 2e73 656c 6563 7465 6420 3d20 2873 656c  .selected = (sel
-00001270: 662e 7365 6c65 6374 6564 202b 2031 2920  f.selected + 1) 
-00001280: 2520 7365 6c66 2e6e 5f6f 7074 696f 6e73  % self.n_options
-00001290: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000012a0: 7475 726e 0d0a 2020 2020 2020 2020 7265  turn..        re
-000012b0: 7475 726e 206b 6579 0d0a 0d0a 2020 2020  turn key....    
-000012c0: 6465 6620 7265 6e64 6572 2873 656c 6629  def render(self)
-000012d0: 3a0d 0a20 2020 2020 2020 2063 6170 7469  :..        capti
-000012e0: 6f6e 5f73 7461 7274 203d 2032 0d0a 2020  on_start = 2..  
-000012f0: 2020 2020 2020 5f5f 6f70 7469 6f6e 7320        __options 
-00001300: 3d20 7365 6c66 2e74 6578 742e 6c6a 7573  = self.text.ljus
-00001310: 7428 7365 6c66 2e73 697a 652e 6765 7457  t(self.size.getW
-00001320: 6964 7468 2829 2d63 6170 7469 6f6e 5f73  idth()-caption_s
-00001330: 7461 7274 290d 0a20 2020 2020 2020 2073  tart)..        s
-00001340: 656c 662e 6472 6177 6572 2e70 6c61 6365  elf.drawer.place
-00001350: 2843 5374 7228 5f5f 6f70 7469 6f6e 732c  (CStr(__options,
-00001360: 2066 6f72 6563 6f6c 6f72 3d28 0d0a 2020   forecolor=(..  
-00001370: 2020 2020 2020 2020 2020 3232 302c 2032            220, 2
-00001380: 3230 2c20 3232 3029 292c 2070 6f73 3d28  20, 220)), pos=(
-00001390: 6361 7074 696f 6e5f 7374 6172 742c 2030  caption_start, 0
-000013a0: 2929 0d0a 2020 2020 2020 2020 666f 7220  ))..        for 
-000013b0: 692c 206f 7074 696f 6e20 696e 2065 6e75  i, option in enu
-000013c0: 6d65 7261 7465 2873 656c 662e 6f70 7469  merate(self.opti
-000013d0: 6f6e 7329 3a0d 0a20 2020 2020 2020 2020  ons):..         
-000013e0: 2020 2069 6620 6920 3d3d 2073 656c 662e     if i == self.
-000013f0: 7365 6c65 6374 6564 3a0d 0a20 2020 2020  selected:..     
-00001400: 2020 2020 2020 2020 2020 206f 7074 696f             optio
-00001410: 6e5f 636f 6c6f 7220 3d20 2835 302c 2032  n_color = (50, 2
-00001420: 3230 2c20 3830 290d 0a20 2020 2020 2020  20, 80)..       
-00001430: 2020 2020 2020 2020 206f 7074 696f 6e5f           option_
-00001440: 696e 6469 6361 746f 7220 3d20 4353 7472  indicator = CStr
-00001450: 2822 3e20 222c 2066 6f72 6563 6f6c 6f72  ("> ", forecolor
-00001460: 3d28 3232 302c 2032 3230 2c20 3232 3029  =(220, 220, 220)
-00001470: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00001480: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00001490: 2020 2020 2020 6f70 7469 6f6e 5f63 6f6c        option_col
-000014a0: 6f72 203d 2028 3232 302c 2032 3230 2c20  or = (220, 220, 
-000014b0: 3232 3029 0d0a 2020 2020 2020 2020 2020  220)..          
-000014c0: 2020 2020 2020 6f70 7469 6f6e 5f69 6e64        option_ind
-000014d0: 6963 6174 6f72 203d 2043 5374 7228 2220  icator = CStr(" 
-000014e0: 2022 2c20 666f 7265 636f 6c6f 723d 2832   ", forecolor=(2
-000014f0: 3230 2c20 3232 302c 2032 3230 2929 0d0a  20, 220, 220))..
-00001500: 2020 2020 2020 2020 2020 2020 5f5f 6f70              __op
-00001510: 7469 6f6e 203d 2043 5374 7228 6f70 7469  tion = CStr(opti
-00001520: 6f6e 2c20 666f 7265 636f 6c6f 723d 6f70  on, forecolor=op
-00001530: 7469 6f6e 5f63 6f6c 6f72 290d 0a20 2020  tion_color)..   
-00001540: 2020 2020 2020 2020 2073 656c 662e 6472           self.dr
-00001550: 6177 6572 2e70 6c61 6365 286f 7074 696f  awer.place(optio
-00001560: 6e5f 696e 6469 6361 746f 7220 2b20 5f5f  n_indicator + __
-00001570: 6f70 7469 6f6e 2c0d 0a20 2020 2020 2020  option,..       
-00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001590: 2020 2020 2020 2070 6f73 3d28 6361 7074         pos=(capt
-000015a0: 696f 6e5f 7374 6172 742c 2031 202b 2069  ion_start, 1 + i
-000015b0: 2929 0d0a 0d0a 0d0a 636c 6173 7320 5769  ))......class Wi
-000015c0: 6467 6574 496e 7075 7428 5769 6467 6574  dgetInput(Widget
-000015d0: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
-000015e0: 6974 5f5f 2873 656c 662c 0d0a 2020 2020  it__(self,..    
-000015f0: 2020 2020 2020 2020 2020 2020 2074 6578               tex
-00001600: 743a 2073 7472 2c0d 0a20 2020 2020 2020  t: str,..       
-00001610: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-00001620: 5369 7a65 203d 204e 6f6e 652c 0d0a 2020  Size = None,..  
-00001630: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00001640: 6f73 3a20 506f 696e 7420 3d20 506f 696e  os: Point = Poin
-00001650: 7428 302c 2030 292c 0d0a 2020 2020 2020  t(0, 0),..      
-00001660: 2020 2020 2020 2020 2020 2063 7479 7065             ctype
-00001670: 3a20 436f 6c6f 7254 7970 6520 3d20 4e6f  : ColorType = No
-00001680: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-00001690: 2020 2020 2020 616c 6c6f 7765 645f 6368        allowed_ch
-000016a0: 6172 6163 7465 7273 3a20 7374 7220 3d20  aracters: str = 
-000016b0: 2220 6162 6364 6566 6768 696a 6b6c 6d6e  " abcdefghijklmn
-000016c0: 6f70 7172 7374 7576 7778 797a 3031 3233  opqrstuvwxyz0123
-000016d0: 3435 3637 3839 5f2d 2b2f 5c5c 2829 5b5d  456789_-+/\\()[]
-000016e0: 2e22 0d0a 2020 2020 2020 2020 2020 2020  ."..            
-000016f0: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
-00001700: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
-00001710: 5f28 6374 7970 652c 2073 697a 652c 2070  _(ctype, size, p
-00001720: 6f73 290d 0a20 2020 2020 2020 2023 2070  os)..        # p
-00001730: 203d 2031 0d0a 2020 2020 2020 2020 7365   = 1..        se
-00001740: 6c66 2e73 697a 652e 6820 3d20 310d 0a20  lf.size.h = 1.. 
-00001750: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
-00001760: 203d 2074 6578 740d 0a20 2020 2020 2020   = text..       
-00001770: 2073 656c 662e 6865 6967 6874 203d 2031   self.height = 1
-00001780: 0d0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
-00001790: 6e70 7574 203d 2022 220d 0a20 2020 2020  nput = ""..     
-000017a0: 2020 2073 656c 662e 706f 696e 7465 7220     self.pointer 
-000017b0: 3d20 300d 0a20 2020 2020 2020 2073 656c  = 0..        sel
-000017c0: 662e 7669 6577 203d 2030 0d0a 2020 2020  f.view = 0..    
-000017d0: 2020 2020 7365 6c66 2e73 686f 775f 706f      self.show_po
-000017e0: 696e 7465 7220 3d20 4661 6c73 650d 0a20  inter = False.. 
-000017f0: 2020 2020 2020 2023 2063 6861 7261 6374         # charact
-00001800: 6572 7320 7468 6174 2074 6869 7320 6469  ers that this di
-00001810: 616c 6f75 6765 2077 696c 6c20 6c69 7374  alouge will list
-00001820: 656e 2074 6f0d 0a20 2020 2020 2020 2073  en to..        s
-00001830: 656c 662e 616c 6c6f 7765 645f 6368 6172  elf.allowed_char
-00001840: 6163 7465 7273 203d 2061 6c6c 6f77 6564  acters = allowed
-00001850: 5f63 6861 7261 6374 6572 730d 0a20 2020  _characters..   
-00001860: 2020 2020 2073 656c 662e 7469 636b 203d       self.tick =
-00001870: 2030 0d0a 0d0a 2020 2020 6465 6620 7275   0....    def ru
-00001880: 6e5f 6361 6c6c 6261 636b 7328 7365 6c66  n_callbacks(self
-00001890: 293a 0d0a 2020 2020 2020 2020 7375 7065  ):..        supe
-000018a0: 7228 292e 7275 6e5f 6361 6c6c 6261 636b  r().run_callback
-000018b0: 7328 290d 0a20 2020 2020 2020 2073 656c  s()..        sel
-000018c0: 662e 7061 7265 6e74 2e63 6c6f 7365 2829  f.parent.close()
-000018d0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000018e0: 2073 656c 662e 696e 7075 740d 0a0d 0a20   self.input.... 
-000018f0: 2020 2064 6566 2072 6573 6574 2873 656c     def reset(sel
-00001900: 6629 3a0d 0a20 2020 2020 2020 2073 656c  f):..        sel
-00001910: 662e 696e 7075 7420 3d20 2222 0d0a 2020  f.input = ""..  
-00001920: 2020 2020 2020 7365 6c66 2e70 6f69 6e74        self.point
-00001930: 6572 203d 2030 0d0a 2020 2020 2020 2020  er = 0..        
-00001940: 7365 6c66 2e76 6965 7720 3d20 300d 0a0d  self.view = 0...
-00001950: 0a20 2020 2064 6566 2067 6574 6d61 786c  .    def getmaxl
-00001960: 656e 2873 656c 6629 3a0d 0a20 2020 2020  en(self):..     
-00001970: 2020 2070 203d 2032 0d0a 2020 2020 2020     p = 2..      
-00001980: 2020 6d61 785f 696e 7075 745f 6c65 6e20    max_input_len 
-00001990: 3d20 7365 6c66 2e73 697a 652e 6765 7457  = self.size.getW
-000019a0: 6964 7468 2829 2d28 7020 2a20 3229 2d6c  idth()-(p * 2)-l
-000019b0: 656e 2873 656c 662e 7465 7874 290d 0a20  en(self.text).. 
-000019c0: 2020 2020 2020 2072 6574 7572 6e20 6d61         return ma
-000019d0: 785f 696e 7075 745f 6c65 6e0d 0a0d 0a20  x_input_len.... 
-000019e0: 2020 2064 6566 2075 7064 6174 6528 7365     def update(se
-000019f0: 6c66 2c20 6b65 7929 3a0d 0a20 2020 2020  lf, key):..     
-00001a00: 2020 206b 6579 203d 2073 7570 6572 2829     key = super()
-00001a10: 2e75 7064 6174 6528 6b65 7929 0d0a 2020  .update(key)..  
-00001a20: 2020 2020 2020 6966 206b 6579 2069 7320        if key is 
-00001a30: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00001a40: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
-00001a50: 2020 206d 6178 5f69 6e70 7574 5f6c 656e     max_input_len
-00001a60: 203d 2073 656c 662e 6765 746d 6178 6c65   = self.getmaxle
-00001a70: 6e28 290d 0a20 2020 2020 2020 2023 2063  n()..        # c
-00001a80: 6170 7475 7265 2061 6e64 2070 6c61 6365  apture and place
-00001a90: 2063 6861 7261 6374 6572 730d 0a20 2020   characters..   
-00001aa0: 2020 2020 2069 6620 6b65 792e 6c6f 7765       if key.lowe
-00001ab0: 7228 2920 696e 2073 656c 662e 616c 6c6f  r() in self.allo
-00001ac0: 7765 645f 6368 6172 6163 7465 7273 3a0d  wed_characters:.
-00001ad0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00001ae0: 662e 696e 7075 7420 3d20 7365 6c66 2e69  f.input = self.i
-00001af0: 6e70 7574 5b3a 7365 6c66 2e70 6f69 6e74  nput[:self.point
-00001b00: 6572 5d20 2b20 5c0d 0a20 2020 2020 2020  er] + \..       
-00001b10: 2020 2020 2020 2020 206b 6579 202b 2073           key + s
-00001b20: 656c 662e 696e 7075 745b 7365 6c66 2e70  elf.input[self.p
-00001b30: 6f69 6e74 6572 3a5d 0d0a 2020 2020 2020  ointer:]..      
-00001b40: 2020 2020 2020 7365 6c66 2e70 6f69 6e74        self.point
-00001b50: 6572 202b 3d20 310d 0a20 2020 2020 2020  er += 1..       
-00001b60: 2020 2020 2069 6620 286c 656e 2873 656c       if (len(sel
-00001b70: 662e 696e 7075 7429 2d73 656c 662e 7669  f.input)-self.vi
-00001b80: 6577 2920 3e20 286d 6178 5f69 6e70 7574  ew) > (max_input
-00001b90: 5f6c 656e 2d31 293a 0d0a 2020 2020 2020  _len-1):..      
-00001ba0: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-00001bb0: 6965 7720 2b3d 2031 0d0a 2020 2020 2020  iew += 1..      
-00001bc0: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
-00001bd0: 2020 2020 2020 2020 2320 6261 636b 7370          # backsp
-00001be0: 6163 650d 0a20 2020 2020 2020 2069 6620  ace..        if 
-00001bf0: 6b65 7920 3d3d 204b 6579 2e42 4143 4b53  key == Key.BACKS
-00001c00: 5041 4345 3a0d 0a20 2020 2020 2020 2020  PACE:..         
-00001c10: 2020 2069 6620 7365 6c66 2e70 6f69 6e74     if self.point
-00001c20: 6572 2021 3d20 303a 0d0a 2020 2020 2020  er != 0:..      
-00001c30: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-00001c40: 6e70 7574 203d 2073 656c 662e 696e 7075  nput = self.inpu
-00001c50: 745b 3a73 656c 662e 706f 696e 7465 7220  t[:self.pointer 
-00001c60: 2d0d 0a20 2020 2020 2020 2020 2020 2020  -..             
-00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c80: 2020 2020 2020 2020 2020 2031 5d20 2b20             1] + 
-00001c90: 7365 6c66 2e69 6e70 7574 5b73 656c 662e  self.input[self.
-00001ca0: 706f 696e 7465 723a 5d0d 0a20 2020 2020  pointer:]..     
-00001cb0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001cd0: 6c66 2e69 6e70 7574 203d 2073 656c 662e  lf.input = self.
-00001ce0: 696e 7075 745b 7365 6c66 2e70 6f69 6e74  input[self.point
-00001cf0: 6572 3a5d 0d0a 2020 2020 2020 2020 2020  er:]..          
-00001d00: 2020 7365 6c66 2e70 6f69 6e74 6572 203d    self.pointer =
-00001d10: 206d 6178 2873 656c 662e 706f 696e 7465   max(self.pointe
-00001d20: 7220 2d20 312c 2030 290d 0a20 2020 2020  r - 1, 0)..     
-00001d30: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00001d40: 6f69 6e74 6572 2d73 656c 662e 7669 6577  ointer-self.view
-00001d50: 203c 2030 3a0d 0a20 2020 2020 2020 2020   < 0:..         
-00001d60: 2020 2020 2020 2073 656c 662e 7669 6577         self.view
-00001d70: 203d 206d 6178 2873 656c 662e 7669 6577   = max(self.view
-00001d80: 202d 206d 6178 5f69 6e70 7574 5f6c 656e   - max_input_len
-00001d90: 2c20 3029 0d0a 2020 2020 2020 2020 2020  , 0)..          
-00001da0: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
-00001db0: 2020 2020 2320 6465 6c65 7465 0d0a 2020      # delete..  
-00001dc0: 2020 2020 2020 6966 206b 6579 203d 3d20        if key == 
-00001dd0: 4b65 792e 4445 4c45 5445 3a0d 0a20 2020  Key.DELETE:..   
-00001de0: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
-00001df0: 7075 7420 3d20 7365 6c66 2e69 6e70 7574  put = self.input
-00001e00: 5b3a 7365 6c66 2e70 6f69 6e74 6572 5d20  [:self.pointer] 
-00001e10: 2b20 5c0d 0a20 2020 2020 2020 2020 2020  + \..           
-00001e20: 2020 2020 2073 656c 662e 696e 7075 745b       self.input[
-00001e30: 7365 6c66 2e70 6f69 6e74 6572 2b31 3a5d  self.pointer+1:]
-00001e40: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00001e50: 7365 6c66 2e70 6f69 6e74 6572 203d 206d  self.pointer = m
-00001e60: 6178 2873 656c 662e 706f 696e 7465 7220  ax(self.pointer 
-00001e70: 2d20 312c 2030 290d 0a20 2020 2020 2020  - 1, 0)..       
-00001e80: 2020 2020 2072 6574 7572 6e0d 0a0d 0a20       return.... 
-00001e90: 2020 2020 2020 2023 206c 6566 7420 6172         # left ar
-00001ea0: 726f 770d 0a20 2020 2020 2020 2069 6620  row..        if 
-00001eb0: 6b65 7920 3d3d 204b 6579 2e4c 4546 543a  key == Key.LEFT:
-00001ec0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00001ed0: 6c66 2e70 6f69 6e74 6572 203d 206d 6178  lf.pointer = max
-00001ee0: 2873 656c 662e 706f 696e 7465 7220 2d20  (self.pointer - 
-00001ef0: 312c 2030 290d 0a20 2020 2020 2020 2020  1, 0)..         
-00001f00: 2020 2069 6620 7365 6c66 2e70 6f69 6e74     if self.point
-00001f10: 6572 2d73 656c 662e 7669 6577 203c 2030  er-self.view < 0
-00001f20: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001f30: 2020 2073 656c 662e 7669 6577 203d 206d     self.view = m
-00001f40: 6178 2873 656c 662e 7669 6577 202d 2031  ax(self.view - 1
-00001f50: 2c20 3029 0d0a 2020 2020 2020 2020 2020  , 0)..          
-00001f60: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
-00001f70: 2020 2020 2320 7269 6768 7420 6172 726f      # right arro
-00001f80: 770d 0a20 2020 2020 2020 2069 6620 6b65  w..        if ke
-00001f90: 7920 3d3d 204b 6579 2e52 4947 4854 3a0d  y == Key.RIGHT:.
-00001fa0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00001fb0: 662e 706f 696e 7465 7220 3d20 6d69 6e28  f.pointer = min(
-00001fc0: 7365 6c66 2e70 6f69 6e74 6572 202b 2031  self.pointer + 1
-00001fd0: 2c20 6c65 6e28 7365 6c66 2e69 6e70 7574  , len(self.input
-00001fe0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00001ff0: 6966 2073 656c 662e 7669 6577 203d 3d20  if self.view == 
-00002000: 2873 656c 662e 706f 696e 7465 722d 6d61  (self.pointer-ma
-00002010: 785f 696e 7075 745f 6c65 6e29 3a0d 0a20  x_input_len):.. 
-00002020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002030: 656c 662e 7669 6577 203d 206d 696e 2873  elf.view = min(s
-00002040: 656c 662e 7669 6577 202b 2031 2c20 6c65  elf.view + 1, le
-00002050: 6e28 7365 6c66 2e69 6e70 7574 2929 0d0a  n(self.input))..
-00002060: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002070: 726e 0d0a 0d0a 2020 2020 2020 2020 6966  rn....        if
-00002080: 206b 6579 203d 3d20 2255 5044 4154 4522   key == "UPDATE"
-00002090: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000020a0: 656c 662e 7469 636b 202b 3d20 310d 0a20  elf.tick += 1.. 
-000020b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000020c0: 7368 6f77 5f70 6f69 6e74 6572 203d 2028  show_pointer = (
-000020d0: 7365 6c66 2e74 6963 6b20 2520 3132 2920  self.tick % 12) 
-000020e0: 3e3d 2036 0d0a 2020 2020 2020 2020 7265  >= 6..        re
-000020f0: 7475 726e 206b 6579 0d0a 0d0a 2020 2020  turn key....    
-00002100: 6465 6620 666f 726d 6174 5f74 6578 7462  def format_textb
-00002110: 6f78 2873 656c 6629 3a0d 0a20 2020 2020  ox(self):..     
-00002120: 2020 2074 6578 742c 2069 6e70 2c20 706f     text, inp, po
-00002130: 696e 7465 722c 2076 6965 7720 3d20 7365  inter, view = se
-00002140: 6c66 2e74 6578 742c 2073 656c 662e 696e  lf.text, self.in
-00002150: 7075 742c 2073 656c 662e 706f 696e 7465  put, self.pointe
-00002160: 722c 2073 656c 662e 7669 6577 0d0a 2020  r, self.view..  
-00002170: 2020 2020 2020 6d61 785f 696e 7075 745f        max_input_
-00002180: 6c65 6e20 3d20 7365 6c66 2e67 6574 6d61  len = self.getma
-00002190: 786c 656e 2829 0d0a 2020 2020 2020 2020  xlen()..        
-000021a0: 2320 6765 7420 7468 6520 696e 7075 7420  # get the input 
-000021b0: 7465 7874 2077 6974 6820 6669 7865 6420  text with fixed 
-000021c0: 6c65 6e67 7468 2070 6c75 7320 6f6e 6520  length plus one 
-000021d0: 6578 7472 6120 7370 6163 6520 666f 7220  extra space for 
-000021e0: 7468 6520 706f 696e 7465 720d 0a20 2020  the pointer..   
-000021f0: 2020 2020 2069 6620 7669 6577 2b6d 6178       if view+max
-00002200: 5f69 6e70 7574 5f6c 656e 2d31 203c 206c  _input_len-1 < l
-00002210: 656e 2869 6e70 293a 0d0a 2020 2020 2020  en(inp):..      
-00002220: 2020 2020 2020 696e 705f 203d 2069 6e70        inp_ = inp
-00002230: 5b76 6965 773a 7669 6577 2b6d 6178 5f69  [view:view+max_i
-00002240: 6e70 7574 5f6c 656e 5d0d 0a20 2020 2020  nput_len]..     
-00002250: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00002260: 2020 2020 2020 696e 705f 203d 2069 6e70        inp_ = inp
-00002270: 5b76 6965 773a 7669 6577 2b6d 6178 5f69  [view:view+max_i
-00002280: 6e70 7574 5f6c 656e 2d31 5d20 2b20 2220  nput_len-1] + " 
-00002290: 220d 0a0d 0a20 2020 2020 2020 2069 6620  "....        if 
-000022a0: 6e6f 7420 7365 6c66 2e69 735f 6469 7361  not self.is_disa
-000022b0: 626c 6564 2061 6e64 2073 656c 662e 7368  bled and self.sh
-000022c0: 6f77 5f70 6f69 6e74 6572 206f 7220 696e  ow_pointer or in
-000022d0: 705f 5b70 6f69 6e74 6572 2d76 6965 775d  p_[pointer-view]
-000022e0: 2021 3d20 2220 223a 0d0a 2020 2020 2020   != " ":..      
-000022f0: 2020 2020 2020 706f 696e 7465 725f 7374        pointer_st
-00002300: 7220 3d20 4353 7472 280d 0a20 2020 2020  r = CStr(..     
-00002310: 2020 2020 2020 2020 2020 2069 6e70 5f5b             inp_[
-00002320: 706f 696e 7465 722d 7669 6577 5d2c 2062  pointer-view], b
-00002330: 6163 6b63 6f6c 6f72 3d28 3232 302c 2032  ackcolor=(220, 2
-00002340: 3230 2c20 3232 3029 2c20 666f 7265 636f  20, 220), foreco
-00002350: 6c6f 723d 2832 302c 2032 302c 2032 3029  lor=(20, 20, 20)
-00002360: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-00002370: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
-00002380: 696e 7465 725f 7374 7220 3d20 4353 7472  inter_str = CStr
-00002390: 2869 6e70 5f5b 706f 696e 7465 722d 7669  (inp_[pointer-vi
-000023a0: 6577 5d29 0d0a 2020 2020 2020 2020 2320  ew])..        # 
-000023b0: 696e 7365 7274 2074 6865 2070 6f69 6e74  insert the point
-000023c0: 6572 2069 6e74 6f20 696e 7075 7420 7465  er into input te
-000023d0: 7874 2061 7420 7468 6520 636f 7272 6563  xt at the correc
-000023e0: 7420 706f 7369 7469 6f6e 0d0a 2020 2020  t position..    
-000023f0: 2020 2020 696e 7075 745f 706c 7573 5f70      input_plus_p
-00002400: 6f69 6e74 6572 203d 2043 5374 7228 0d0a  ointer = CStr(..
-00002410: 2020 2020 2020 2020 2020 2020 696e 705f              inp_
-00002420: 5b3a 706f 696e 7465 722d 7669 6577 5d29  [:pointer-view])
-00002430: 202b 2070 6f69 6e74 6572 5f73 7472 202b   + pointer_str +
-00002440: 2043 5374 7228 696e 705f 5b70 6f69 6e74   CStr(inp_[point
-00002450: 6572 2d76 6965 772b 313a 5d29 0d0a 0d0a  er-view+1:])....
-00002460: 2020 2020 2020 2020 7465 7874 5f63 203d          text_c =
-00002470: 2028 3530 2c20 3230 302c 2035 3029 0d0a   (50, 200, 50)..
-00002480: 0d0a 2020 2020 2020 2020 6673 7472 203d  ..        fstr =
-00002490: 2043 5374 7228 7465 7874 2c20 666f 7265   CStr(text, fore
-000024a0: 636f 6c6f 723d 7465 7874 5f63 290d 0a0d  color=text_c)...
-000024b0: 0a20 2020 2020 2020 2062 6163 6b5f 6578  .        back_ex
-000024c0: 6973 7473 203d 2043 5374 7228 223c 222c  ists = CStr("<",
-000024d0: 2066 6f72 6563 6f6c 6f72 3d74 6578 745f   forecolor=text_
-000024e0: 6329 0d0a 2020 2020 2020 2020 666f 7277  c)..        forw
-000024f0: 6172 645f 6578 6973 7473 203d 2043 5374  ard_exists = CSt
-00002500: 7228 223e 222c 2066 6f72 6563 6f6c 6f72  r(">", forecolor
-00002510: 3d74 6578 745f 6329 0d0a 0d0a 2020 2020  =text_c)....    
-00002520: 2020 2020 6673 7472 202b 3d20 2862 6163      fstr += (bac
-00002530: 6b5f 6578 6973 7473 2069 6620 7669 6577  k_exists if view
-00002540: 2021 3d20 3020 656c 7365 2022 2022 290d   != 0 else " ").
-00002550: 0a20 2020 2020 2020 2066 7374 7220 2b3d  .        fstr +=
-00002560: 2069 6e70 7574 5f70 6c75 735f 706f 696e   input_plus_poin
-00002570: 7465 7220 2b20 2220 2220 2a20 5c0d 0a20  ter + " " * \.. 
-00002580: 2020 2020 2020 2020 2020 2028 6d61 785f             (max_
-00002590: 696e 7075 745f 6c65 6e20 2d20 6c65 6e28  input_len - len(
-000025a0: 696e 7075 745f 706c 7573 5f70 6f69 6e74  input_plus_point
-000025b0: 6572 2929 0d0a 2020 2020 2020 2020 6673  er))..        fs
-000025c0: 7472 202b 3d20 2866 6f72 7761 7264 5f65  tr += (forward_e
-000025d0: 7869 7374 7320 6966 2076 6965 772b 6d61  xists if view+ma
-000025e0: 785f 696e 7075 745f 6c65 6e2d 3120 3c20  x_input_len-1 < 
-000025f0: 6c65 6e28 696e 7029 2065 6c73 6520 2220  len(inp) else " 
-00002600: 2229 0d0a 0d0a 2020 2020 2020 2020 7265  ")....        re
-00002610: 7475 726e 2066 7374 720d 0a0d 0a20 2020  turn fstr....   
-00002620: 2064 6566 2072 656e 6465 7228 7365 6c66   def render(self
-00002630: 293a 0d0a 2020 2020 2020 2020 7020 3d20  ):..        p = 
-00002640: 310d 0a20 2020 2020 2020 2023 2073 656c  1..        # sel
-00002650: 662e 6472 6177 6572 2e70 6c61 6365 2843  f.drawer.place(C
-00002660: 5374 7228 2220 2220 2a20 2873 656c 662e  Str(" " * (self.
-00002670: 7369 7a65 2e67 6574 5769 6474 6828 2920  size.getWidth() 
-00002680: 2d20 2870 202a 2032 2920 2d20 6c65 6e28  - (p * 2) - len(
-00002690: 7365 6c66 2e74 6578 7429 292c 0d0a 2020  self.text)),..  
-000026a0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-000026b0: 2020 2020 2020 2020 2062 6163 6b63 6f6c           backcol
-000026c0: 6f72 3d28 3230 2c20 3230 2c20 3230 2929  or=(20, 20, 20))
-000026d0: 2c20 706f 733d 2870 202b 206c 656e 2873  , pos=(p + len(s
-000026e0: 656c 662e 7465 7874 292c 2030 2929 0d0a  elf.text), 0))..
-000026f0: 2020 2020 2020 2020 7365 6c66 2e64 7261          self.dra
-00002700: 7765 722e 706c 6163 6528 7365 6c66 2e66  wer.place(self.f
-00002710: 6f72 6d61 745f 7465 7874 626f 7828 292c  ormat_textbox(),
-00002720: 2070 6f73 3d28 702c 2030 2929 0d0a        pos=(p, 0))..
+000000c0: 7320 4b65 790d 0a0d 0a66 726f 6d20 2e2e  s Key....from ..
+000000d0: 6465 6674 7970 6573 2069 6d70 6f72 7420  deftypes import 
+000000e0: 506f 696e 742c 2053 697a 652c 2044 4546  Point, Size, DEF
+000000f0: 4155 4c54 5f42 4143 4b47 524f 554e 445f  AULT_BACKGROUND_
+00000100: 434f 4c4f 520d 0a0d 0a64 6566 2064 6566  COLOR....def def
+00000110: 6175 6c74 2864 3a20 6469 6374 2c20 6b3a  ault(d: dict, k:
+00000120: 7374 722c 2064 6566 6175 6c74 293a 0d0a  str, default):..
+00000130: 2020 2020 6966 206b 2069 6e20 642e 6b65      if k in d.ke
+00000140: 7973 2829 3a0d 0a20 2020 2020 2020 2072  ys():..        r
+00000150: 6574 7572 6e20 645b 6b5d 0d0a 2020 2020  eturn d[k]..    
+00000160: 656c 7365 3a0d 0a20 2020 2020 2020 2072  else:..        r
+00000170: 6574 7572 6e20 6465 6661 756c 740d 0a0d  eturn default...
+00000180: 0a63 6c61 7373 2057 6964 6765 7442 6173  .class WidgetBas
+00000190: 6528 293a 0d0a 2020 2020 6465 6620 5f5f  e():..    def __
+000001a0: 696e 6974 5f5f 2873 656c 662c 2073 697a  init__(self, siz
+000001b0: 653a 2053 697a 6520 3d20 4e6f 6e65 2c20  e: Size = None, 
+000001c0: 706f 733a 2050 6f69 6e74 203d 2050 6f69  pos: Point = Poi
+000001d0: 6e74 2830 2c20 3029 2c20 2a2a 6b77 6172  nt(0, 0), **kwar
+000001e0: 6773 293a 0d0a 2020 2020 2020 2020 2320  gs):..        # 
+000001f0: 7365 7420 7661 7269 6162 6c65 640d 0a20  set variabled.. 
+00000200: 2020 2020 2020 2073 656c 662e 6374 7970         self.ctyp
+00000210: 6520 3d20 6465 6661 756c 7428 6b77 6172  e = default(kwar
+00000220: 6773 2c20 2263 7479 7065 222c 2043 6f6c  gs, "ctype", Col
+00000230: 6f72 5479 7065 2e4c 4547 4143 5929 0d0a  orType.LEGACY)..
+00000240: 2020 2020 2020 2020 7365 6c66 2e73 697a          self.siz
+00000250: 6520 3d20 5369 7a65 2831 302c 2032 3029  e = Size(10, 20)
+00000260: 2069 6620 7369 7a65 2069 7320 4e6f 6e65   if size is None
+00000270: 2065 6c73 6520 7369 7a65 0d0a 2020 2020   else size..    
+00000280: 2020 2020 7365 6c66 2e70 6f73 203d 2050      self.pos = P
+00000290: 6f69 6e74 2830 2c20 3029 2069 6620 706f  oint(0, 0) if po
+000002a0: 7320 6973 204e 6f6e 6520 656c 7365 2070  s is None else p
+000002b0: 6f73 0d0a 2020 2020 2020 2020 2320 6465  os..        # de
+000002c0: 6661 756c 7473 0d0a 2020 2020 2020 2020  faults..        
+000002d0: 7365 6c66 2e62 6163 6b67 726f 756e 645f  self.background_
+000002e0: 636f 6c6f 7220 3d20 4445 4641 554c 545f  color = DEFAULT_
+000002f0: 4241 434b 4752 4f55 4e44 5f43 4f4c 4f52  BACKGROUND_COLOR
+00000300: 0d0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
+00000310: 616d 6520 3d20 6465 6661 756c 7428 6b77  ame = default(kw
+00000320: 6172 6773 2c20 226e 616d 6522 2c20 225f  args, "name", "_
+00000330: 5f6e 616d 655f 5f22 290d 0a20 2020 2020  _name__")..     
+00000340: 2020 2073 656c 662e 7061 7265 6e74 203d     self.parent =
+00000350: 204e 6f6e 650d 0a20 2020 2020 2020 200d   None..        .
+00000360: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00000370: 7375 6c74 203d 204e 6f6e 650d 0a0d 0a20  sult = None.... 
+00000380: 2020 2064 6566 2067 6574 5f6e 616d 6528     def get_name(
+00000390: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000003a0: 6e61 6d65 203d 2020 7365 6c66 2e5f 5f63  name =  self.__c
+000003b0: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f0d  lass__.__name__.
+000003c0: 0a20 2020 2020 2020 2063 203d 2030 0d0a  .        c = 0..
+000003d0: 2020 2020 2020 2020 666f 7220 7720 696e          for w in
+000003e0: 2073 656c 662e 7061 7265 6e74 2e77 6964   self.parent.wid
+000003f0: 6765 7473 3a0d 0a20 2020 2020 2020 2020  gets:..         
+00000400: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00000410: 2877 2c20 7365 6c66 2e5f 5f63 6c61 7373  (w, self.__class
+00000420: 5f5f 293a 0d0a 2020 2020 2020 2020 2020  __):..          
+00000430: 2020 2020 2020 6320 2b3d 2031 0d0a 2020        c += 1..  
+00000440: 2020 2020 2020 7265 7475 726e 206e 616d        return nam
+00000450: 6520 2b20 225f 2220 2b20 7374 7228 632b  e + "_" + str(c+
+00000460: 3129 0d0a 0d0a 2020 2020 0d0a 2020 2020  1)....    ..    
+00000470: 6465 6620 6f6e 5f61 6464 2873 656c 662c  def on_add(self,
+00000480: 2070 6172 656e 7429 3a0d 0a20 2020 2020   parent):..     
+00000490: 2020 2073 656c 662e 7061 7265 6e74 203d     self.parent =
+000004a0: 2070 6172 656e 740d 0a20 2020 2020 2020   parent..       
+000004b0: 2069 6620 7365 6c66 2e6e 616d 6520 3d3d   if self.name ==
+000004c0: 2022 5f5f 6e61 6d65 5f5f 223a 0d0a 2020   "__name__":..  
+000004d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000004e0: 616d 6520 3d20 7365 6c66 2e67 6574 5f6e  ame = self.get_n
+000004f0: 616d 6528 290d 0a0d 0a20 2020 2064 6566  ame()....    def
+00000500: 206f 6e5f 696e 7465 7272 7570 7428 7365   on_interrupt(se
+00000510: 6c66 293a 0d0a 2020 2020 2020 2020 7061  lf):..        pa
+00000520: 7373 0d0a 0d0a 2020 2020 6465 6620 6765  ss....    def ge
+00000530: 745f 6472 6177 6572 2873 656c 6629 3a0d  t_drawer(self):.
+00000540: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000550: 4472 6177 6572 2873 697a 653d 2873 656c  Drawer(size=(sel
+00000560: 662e 7369 7a65 2e67 6574 5769 6474 6828  f.size.getWidth(
+00000570: 292c 2073 656c 662e 7369 7a65 2e67 6574  ), self.size.get
+00000580: 4865 6967 6874 2829 292c 2062 6163 6b67  Height()), backg
+00000590: 726f 756e 645f 636f 6c6f 723d 7365 6c66  round_color=self
+000005a0: 2e62 6163 6b67 726f 756e 645f 636f 6c6f  .background_colo
+000005b0: 7229 0d0a 0d0a 2020 2020 6465 6620 7265  r)....    def re
+000005c0: 6e64 6572 2873 656c 6629 3a0d 0a20 2020  nder(self):..   
+000005d0: 2020 2020 2070 6173 730d 0a0d 0a20 2020       pass....   
+000005e0: 2064 6566 2067 6574 5f72 656e 6465 7228   def get_render(
+000005f0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000600: 7365 6c66 2e64 7261 7765 7220 3d20 7365  self.drawer = se
+00000610: 6c66 2e67 6574 5f64 7261 7765 7228 290d  lf.get_drawer().
+00000620: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00000630: 6e64 6572 2829 0d0a 2020 2020 2020 2020  nder()..        
+00000640: 7265 7475 726e 2073 656c 662e 6472 6177  return self.draw
+00000650: 6572 0d0a 0d0a 2020 2020 6465 6620 7570  er....    def up
+00000660: 6461 7465 2873 656c 662c 206b 6579 293a  date(self, key):
+00000670: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000680: 206b 6579 0d0a 0d0a 0d0a 636c 6173 7320   key......class 
+00000690: 5769 6467 6574 2857 6964 6765 7442 6173  Widget(WidgetBas
+000006a0: 6529 3a0d 0a20 2020 2064 6566 205f 5f69  e):..    def __i
+000006b0: 6e69 745f 5f28 7365 6c66 2c20 7369 7a65  nit__(self, size
+000006c0: 3a20 5369 7a65 203d 204e 6f6e 652c 2070  : Size = None, p
+000006d0: 6f73 3a20 506f 696e 7420 3d20 506f 696e  os: Point = Poin
+000006e0: 7428 302c 2030 292c 202a 2a6b 7761 7267  t(0, 0), **kwarg
+000006f0: 7329 3a0d 0a20 2020 2020 2020 2073 7570  s):..        sup
+00000700: 6572 2829 2e5f 5f69 6e69 745f 5f28 7369  er().__init__(si
+00000710: 7a65 2c20 706f 732c 202a 2a6b 7761 7267  ze, pos, **kwarg
+00000720: 7329 0d0a 2020 2020 2020 2020 2320 6465  s)..        # de
+00000730: 6661 756c 7473 0d0a 2020 2020 2020 2020  faults..        
+00000740: 7365 6c66 2e69 735f 6469 7361 626c 6564  self.is_disabled
+00000750: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+00000760: 2020 7365 6c66 2e69 735f 7365 6c65 6374    self.is_select
+00000770: 6564 203d 2046 616c 7365 0d0a 2020 2020  ed = False..    
+00000780: 2020 2020 7365 6c66 2e73 656c 6563 7461      self.selecta
+00000790: 626c 6520 3d20 5472 7565 0d0a 0d0a 2020  ble = True....  
+000007a0: 2020 6465 6620 7275 6e5f 6361 6c6c 6261    def run_callba
+000007b0: 636b 7328 7365 6c66 293a 0d0a 2020 2020  cks(self):..    
+000007c0: 2020 2020 7061 7373 0d0a 0d0a 2020 2020      pass....    
+000007d0: 6465 6620 6f6e 5f65 6e74 6572 2873 656c  def on_enter(sel
+000007e0: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
+000007f0: 7572 6e20 7365 6c66 2e72 756e 5f63 616c  urn self.run_cal
+00000800: 6c62 6163 6b73 2829 0d0a 0d0a 2020 2020  lbacks()....    
+00000810: 6465 6620 6f6e 5f69 6e74 6572 7275 7074  def on_interrupt
+00000820: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00000830: 2073 7570 6572 2829 2e6f 6e5f 696e 7465   super().on_inte
+00000840: 7272 7570 7428 290d 0a20 2020 2020 2020  rrupt()..       
+00000850: 2073 656c 662e 6973 5f64 6973 6162 6c65   self.is_disable
+00000860: 6420 3d20 5472 7565 0d0a 0d0a 2020 2020  d = True....    
+00000870: 6465 6620 7570 6461 7465 2873 656c 662c  def update(self,
+00000880: 206b 6579 293a 0d0a 2020 2020 2020 2020   key):..        
+00000890: 6b65 7920 3d20 7375 7065 7228 292e 7570  key = super().up
+000008a0: 6461 7465 286b 6579 290d 0a20 2020 2020  date(key)..     
+000008b0: 2020 2069 6620 6b65 7920 3d3d 204b 6579     if key == Key
+000008c0: 2e45 4e54 4552 3a0d 0a20 2020 2020 2020  .ENTER:..       
+000008d0: 2020 2020 2073 656c 662e 6f6e 5f65 6e74       self.on_ent
+000008e0: 6572 2829 0d0a 2020 2020 2020 2020 2020  er()..          
+000008f0: 2020 7265 7475 726e 0d0a 2020 2020 2020    return..      
+00000900: 2020 7265 7475 726e 206b 6579 0d0a 0d0a    return key....
+00000910: 0d0a 636c 6173 7320 5769 6467 6574 4c61  ..class WidgetLa
+00000920: 6265 6c28 5769 6467 6574 293a 0d0a 2020  bel(Widget):..  
+00000930: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00000940: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
+00000950: 2020 2020 2020 2074 6578 742c 0d0a 2020         text,..  
+00000960: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00000970: 656e 7465 7265 643a 2062 6f6f 6c20 3d20  entered: bool = 
+00000980: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00000990: 2020 2020 2020 2020 776f 7264 7772 6170          wordwrap
+000009a0: 3a20 626f 6f6c 203d 2054 7275 652c 0d0a  : bool = True,..
+000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009c0: 2073 697a 653a 2053 697a 6520 3d20 4e6f   size: Size = No
+000009d0: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
+000009e0: 2020 2020 2020 706f 733a 2050 6f69 6e74        pos: Point
+000009f0: 203d 2050 6f69 6e74 2830 2c20 3029 2c0d   = Point(0, 0),.
+00000a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a10: 2020 2a2a 6b77 6172 6773 0d0a 2020 2020    **kwargs..    
+00000a20: 2020 2020 2020 2020 2020 2020 2029 3a0d               ):.
+00000a30: 0a0d 0a20 2020 2020 2020 2073 7570 6572  ...        super
+00000a40: 2829 2e5f 5f69 6e69 745f 5f28 7369 7a65  ().__init__(size
+00000a50: 2c20 706f 732c 202a 2a6b 7761 7267 7329  , pos, **kwargs)
+00000a60: 0d0a 0d0a 2020 2020 2020 2020 6966 2069  ....        if i
+00000a70: 7369 6e73 7461 6e63 6528 7465 7874 2c20  sinstance(text, 
+00000a80: 7374 7229 3a0d 0a20 2020 2020 2020 2020  str):..         
+00000a90: 2020 2073 656c 662e 7465 7874 203d 2043     self.text = C
+00000aa0: 5374 7228 7465 7874 2c20 666f 7265 636f  Str(text, foreco
+00000ab0: 6c6f 723d 2832 3230 2c20 3232 302c 2032  lor=(220, 220, 2
+00000ac0: 3230 2929 0d0a 2020 2020 2020 2020 656c  20))..        el
+00000ad0: 6966 2069 7369 6e73 7461 6e63 6528 7465  if isinstance(te
+00000ae0: 7874 2c20 4353 7472 2920 6f72 2069 7369  xt, CStr) or isi
+00000af0: 6e73 7461 6e63 6528 7465 7874 2c20 4353  nstance(text, CS
+00000b00: 7472 4c69 7374 293a 0d0a 2020 2020 2020  trList):..      
+00000b10: 2020 2020 2020 7365 6c66 2e74 6578 7420        self.text 
+00000b20: 3d20 7465 7874 0d0a 2020 2020 2020 2020  = text..        
+00000b30: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00000b40: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+00000b50: 656d 656e 7465 6445 7272 6f72 2829 0d0a  ementedError()..
+00000b60: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00000b70: 697a 652e 6820 3d20 286c 656e 2874 6578  ize.h = (len(tex
+00000b80: 7429 202f 2f20 2873 656c 662e 7369 7a65  t) // (self.size
+00000b90: 2e77 202d 2038 2929 202b 2031 0d0a 2020  .w - 8)) + 1..  
+00000ba0: 2020 2020 2020 7365 6c66 2e63 656e 7465        self.cente
+00000bb0: 7265 6420 3d20 6365 6e74 6572 6564 0d0a  red = centered..
+00000bc0: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
+00000bd0: 6477 7261 7020 3d20 776f 7264 7772 6170  dwrap = wordwrap
+00000be0: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00000bf0: 656c 6563 7461 626c 6520 3d20 4661 6c73  electable = Fals
+00000c00: 650d 0a0d 0a20 2020 2064 6566 2072 756e  e....    def run
+00000c10: 5f63 616c 6c62 6163 6b73 2873 656c 6629  _callbacks(self)
+00000c20: 3a0d 0a20 2020 2020 2020 2070 6173 730d  :..        pass.
+00000c30: 0a0d 0a20 2020 2064 6566 205f 706c 6163  ...    def _plac
+00000c40: 655f 7465 7874 2873 656c 662c 2074 6578  e_text(self, tex
+00000c50: 742c 206c 6e5f 6964 7829 3a0d 0a20 2020  t, ln_idx):..   
+00000c60: 2020 2020 2069 6620 7365 6c66 2e63 656e       if self.cen
+00000c70: 7465 7265 643a 0d0a 2020 2020 2020 2020  tered:..        
+00000c80: 2020 2020 7365 6c66 2e64 7261 7765 722e      self.drawer.
+00000c90: 6365 6e74 6572 5f70 6c61 6365 2874 6578  center_place(tex
+00000ca0: 742c 206c 6e5f 6964 783d 6c6e 5f69 6478  t, ln_idx=ln_idx
+00000cb0: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
+00000cc0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00000cd0: 6c66 2e64 7261 7765 722e 706c 6163 6528  lf.drawer.place(
+00000ce0: 7465 7874 2c20 706f 733d 2830 2c20 6c6e  text, pos=(0, ln
+00000cf0: 5f69 6478 2929 0d0a 0d0a 2020 2020 6465  _idx))....    de
+00000d00: 6620 706c 6163 655f 7465 7874 2873 656c  f place_text(sel
+00000d10: 662c 2074 2c20 6c6e 5f69 6478 293a 0d0a  f, t, ln_idx):..
+00000d20: 2020 2020 2020 2020 2370 7269 6e74 2874          #print(t
+00000d30: 290d 0a20 2020 2020 2020 2069 6620 6c65  )..        if le
+00000d40: 6e28 7429 203e 2028 7365 6c66 2e73 697a  n(t) > (self.siz
+00000d50: 652e 6765 7457 6964 7468 2829 202d 2038  e.getWidth() - 8
+00000d60: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00000d70: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+00000d80: 656e 2874 2929 3a0d 0a20 2020 2020 2020  en(t)):..       
+00000d90: 2020 2020 2020 2020 2069 5f20 3d20 6c65           i_ = le
+00000da0: 6e28 7429 202d 2069 202d 2031 0d0a 2020  n(t) - i - 1..  
+00000db0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00000dc0: 2069 5f20 3e20 2873 656c 662e 7369 7a65   i_ > (self.size
+00000dd0: 2e67 6574 5769 6474 6828 2920 2d20 3829  .getWidth() - 8)
+00000de0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000df0: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00000e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e10: 2063 203d 2074 5b69 5f5d 0d0a 2020 2020   c = t[i_]..    
+00000e20: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00000e30: 7369 6e73 7461 6e63 6528 632c 2073 7472  sinstance(c, str
+00000e40: 2920 616e 6420 6320 3d3d 2022 2022 3a0d  ) and c == " ":.
+00000e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e60: 2020 2020 2073 656c 662e 5f70 6c61 6365       self._place
+00000e70: 5f74 6578 7428 745b 3a69 5f5d 2c20 6c6e  _text(t[:i_], ln
+00000e80: 5f69 6478 290d 0a20 2020 2020 2020 2020  _idx)..         
+00000e90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000ea0: 6e20 7365 6c66 2e70 6c61 6365 5f74 6578  n self.place_tex
+00000eb0: 7428 745b 695f 2b31 3a5d 2c20 6c6e 5f69  t(t[i_+1:], ln_i
+00000ec0: 6478 202b 2031 290d 0a20 2020 2020 2020  dx + 1)..       
+00000ed0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+00000ee0: 7374 616e 6365 2863 2c20 4353 7472 2920  stance(c, CStr) 
+00000ef0: 616e 6420 632e 7374 7220 3d3d 2022 2022  and c.str == " "
+00000f00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000f10: 2020 2020 2020 2073 656c 662e 5f70 6c61         self._pla
+00000f20: 6365 5f74 6578 7428 745b 3a69 5f5d 2c20  ce_text(t[:i_], 
+00000f30: 6c6e 5f69 6478 290d 0a20 2020 2020 2020  ln_idx)..       
+00000f40: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00000f50: 7572 6e20 7365 6c66 2e70 6c61 6365 5f74  urn self.place_t
+00000f60: 6578 7428 745b 695f 2b31 3a5d 2c20 6c6e  ext(t[i_+1:], ln
+00000f70: 5f69 6478 202b 2031 290d 0a20 2020 2020  _idx + 1)..     
+00000f80: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000f90: 2020 2020 2020 7365 6c66 2e5f 706c 6163        self._plac
+00000fa0: 655f 7465 7874 2874 2c20 6c6e 5f69 6478  e_text(t, ln_idx
+00000fb0: 290d 0a0d 0a20 2020 2064 6566 2072 656e  )....    def ren
+00000fc0: 6465 7228 7365 6c66 293a 0d0a 2020 2020  der(self):..    
+00000fd0: 2020 2020 7365 6c66 2e70 6c61 6365 5f74      self.place_t
+00000fe0: 6578 7428 7365 6c66 2e74 6578 742c 206c  ext(self.text, l
+00000ff0: 6e5f 6964 783d 3029 0d0a 0d0a 0d0a 636c  n_idx=0)......cl
+00001000: 6173 7320 5769 6467 6574 4f70 7469 6f6e  ass WidgetOption
+00001010: 7328 5769 6467 6574 293a 0d0a 2020 2020  s(Widget):..    
+00001020: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00001030: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
+00001040: 2020 2020 206f 7074 696f 6e73 3a20 6c69       options: li
+00001050: 7374 5b74 7570 6c65 5b73 7472 2c20 7479  st[tuple[str, ty
+00001060: 7065 732e 4675 6e63 7469 6f6e 5479 7065  pes.FunctionType
+00001070: 5d5d 2c0d 0a20 2020 2020 2020 2020 2020  ]],..           
+00001080: 2020 2020 2020 7465 7874 3a20 7374 7220        text: str 
+00001090: 3d20 224f 7074 696f 6e73 3a22 2c0d 0a20  = "Options:",.. 
+000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010b0: 6465 6661 756c 745f 6f70 7469 6f6e 3a20  default_option: 
+000010c0: 696e 7420 3d20 302c 0d0a 2020 2020 2020  int = 0,..      
+000010d0: 2020 2020 2020 2020 2020 2073 697a 653a             size:
+000010e0: 2053 697a 6520 3d20 4e6f 6e65 2c0d 0a20   Size = None,.. 
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001100: 706f 733a 2050 6f69 6e74 203d 2050 6f69  pos: Point = Poi
+00001110: 6e74 2830 2c20 3029 2c0d 0a20 2020 2020  nt(0, 0),..     
+00001120: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
+00001130: 6172 6773 0d0a 2020 2020 2020 2020 2020  args..          
+00001140: 2020 2020 2020 2029 3a0d 0a0d 0a20 2020         ):....   
+00001150: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
+00001160: 6e69 745f 5f28 7369 7a65 2c20 706f 732c  nit__(size, pos,
+00001170: 202a 2a6b 7761 7267 7329 0d0a 2020 2020   **kwargs)..    
+00001180: 2020 2020 7365 6c66 2e6e 5f6f 7074 696f      self.n_optio
+00001190: 6e73 203d 206c 656e 286f 7074 696f 6e73  ns = len(options
+000011a0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000011b0: 6f70 7469 6f6e 7320 3d20 6c69 7374 286d  options = list(m
+000011c0: 6170 286c 616d 6264 6120 783a 2078 5b30  ap(lambda x: x[0
+000011d0: 5d2c 206f 7074 696f 6e73 2929 0d0a 2020  ], options))..  
+000011e0: 2020 2020 2020 7365 6c66 2e74 6578 7420        self.text 
+000011f0: 3d20 7465 7874 0d0a 2020 2020 2020 2020  = text..        
+00001200: 7365 6c66 2e63 616c 6c62 6163 6b73 203d  self.callbacks =
+00001210: 206c 6973 7428 6d61 7028 6c61 6d62 6461   list(map(lambda
+00001220: 2078 3a20 785b 315d 2c20 6f70 7469 6f6e   x: x[1], option
+00001230: 7329 290d 0a20 2020 2020 2020 2073 656c  s))..        sel
+00001240: 662e 7365 6c65 6374 6564 203d 2064 6566  f.selected = def
+00001250: 6175 6c74 5f6f 7074 696f 6e0d 0a20 2020  ault_option..   
+00001260: 2020 2020 2073 656c 662e 7369 7a65 2e68       self.size.h
+00001270: 203d 2031 202b 2073 656c 662e 6e5f 6f70   = 1 + self.n_op
+00001280: 7469 6f6e 730d 0a0d 0a20 2020 2064 6566  tions....    def
+00001290: 2072 756e 5f63 616c 6c62 6163 6b73 2873   run_callbacks(s
+000012a0: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
+000012b0: 656c 662e 7265 7375 6c74 203d 2073 656c  elf.result = sel
+000012c0: 662e 6361 6c6c 6261 636b 735b 7365 6c66  f.callbacks[self
+000012d0: 2e73 656c 6563 7465 645d 2873 656c 662e  .selected](self.
+000012e0: 7061 7265 6e74 290d 0a20 2020 2020 2020  parent)..       
+000012f0: 2072 6574 7572 6e20 7365 6c66 2e72 6573   return self.res
+00001300: 756c 740d 0a0d 0a20 2020 2064 6566 2075  ult....    def u
+00001310: 7064 6174 6528 7365 6c66 2c20 6b65 7929  pdate(self, key)
+00001320: 3a0d 0a20 2020 2020 2020 206b 6579 203d  :..        key =
+00001330: 2073 7570 6572 2829 2e75 7064 6174 6528   super().update(
+00001340: 6b65 7929 0d0a 2020 2020 2020 2020 6966  key)..        if
+00001350: 206b 6579 203d 3d20 4b65 792e 5550 3a0d   key == Key.UP:.
+00001360: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001370: 662e 7365 6c65 6374 6564 203d 2028 7365  f.selected = (se
+00001380: 6c66 2e73 656c 6563 7465 6420 2d20 3129  lf.selected - 1)
+00001390: 2025 2073 656c 662e 6e5f 6f70 7469 6f6e   % self.n_option
+000013a0: 730d 0a20 2020 2020 2020 2020 2020 2072  s..            r
+000013b0: 6574 7572 6e0d 0a20 2020 2020 2020 2069  eturn..        i
+000013c0: 6620 6b65 7920 3d3d 204b 6579 2e44 4f57  f key == Key.DOW
+000013d0: 4e3a 0d0a 2020 2020 2020 2020 2020 2020  N:..            
+000013e0: 7365 6c66 2e73 656c 6563 7465 6420 3d20  self.selected = 
+000013f0: 2873 656c 662e 7365 6c65 6374 6564 202b  (self.selected +
+00001400: 2031 2920 2520 7365 6c66 2e6e 5f6f 7074   1) % self.n_opt
+00001410: 696f 6e73 0d0a 2020 2020 2020 2020 2020  ions..          
+00001420: 2020 7265 7475 726e 0d0a 2020 2020 2020    return..      
+00001430: 2020 7265 7475 726e 206b 6579 0d0a 0d0a    return key....
+00001440: 2020 2020 6465 6620 7265 6e64 6572 2873      def render(s
+00001450: 656c 6629 3a0d 0a20 2020 2020 2020 2063  elf):..        c
+00001460: 6170 7469 6f6e 5f73 7461 7274 203d 2032  aption_start = 2
+00001470: 0d0a 2020 2020 2020 2020 5f5f 6f70 7469  ..        __opti
+00001480: 6f6e 7320 3d20 7365 6c66 2e74 6578 742e  ons = self.text.
+00001490: 6c6a 7573 7428 7365 6c66 2e73 697a 652e  ljust(self.size.
+000014a0: 6765 7457 6964 7468 2829 2d63 6170 7469  getWidth()-capti
+000014b0: 6f6e 5f73 7461 7274 290d 0a20 2020 2020  on_start)..     
+000014c0: 2020 2073 656c 662e 6472 6177 6572 2e70     self.drawer.p
+000014d0: 6c61 6365 2843 5374 7228 5f5f 6f70 7469  lace(CStr(__opti
+000014e0: 6f6e 732c 2066 6f72 6563 6f6c 6f72 3d28  ons, forecolor=(
+000014f0: 0d0a 2020 2020 2020 2020 2020 2020 3232  ..            22
+00001500: 302c 2032 3230 2c20 3232 3029 292c 2070  0, 220, 220)), p
+00001510: 6f73 3d28 6361 7074 696f 6e5f 7374 6172  os=(caption_star
+00001520: 742c 2030 2929 0d0a 2020 2020 2020 2020  t, 0))..        
+00001530: 666f 7220 692c 206f 7074 696f 6e20 696e  for i, option in
+00001540: 2065 6e75 6d65 7261 7465 2873 656c 662e   enumerate(self.
+00001550: 6f70 7469 6f6e 7329 3a0d 0a20 2020 2020  options):..     
+00001560: 2020 2020 2020 2069 6620 6920 3d3d 2073         if i == s
+00001570: 656c 662e 7365 6c65 6374 6564 3a0d 0a20  elf.selected:.. 
+00001580: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00001590: 7074 696f 6e5f 636f 6c6f 7220 3d20 2835  ption_color = (5
+000015a0: 302c 2032 3230 2c20 3830 290d 0a20 2020  0, 220, 80)..   
+000015b0: 2020 2020 2020 2020 2020 2020 206f 7074               opt
+000015c0: 696f 6e5f 696e 6469 6361 746f 7220 3d20  ion_indicator = 
+000015d0: 4353 7472 2822 3e20 222c 2066 6f72 6563  CStr("> ", forec
+000015e0: 6f6c 6f72 3d28 3232 302c 2032 3230 2c20  olor=(220, 220, 
+000015f0: 3232 3029 290d 0a20 2020 2020 2020 2020  220))..         
+00001600: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00001610: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
+00001620: 5f63 6f6c 6f72 203d 2028 3232 302c 2032  _color = (220, 2
+00001630: 3230 2c20 3232 3029 0d0a 2020 2020 2020  20, 220)..      
+00001640: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
+00001650: 5f69 6e64 6963 6174 6f72 203d 2043 5374  _indicator = CSt
+00001660: 7228 2220 2022 2c20 666f 7265 636f 6c6f  r("  ", forecolo
+00001670: 723d 2832 3230 2c20 3232 302c 2032 3230  r=(220, 220, 220
+00001680: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00001690: 5f5f 6f70 7469 6f6e 203d 2043 5374 7228  __option = CStr(
+000016a0: 6f70 7469 6f6e 2c20 666f 7265 636f 6c6f  option, forecolo
+000016b0: 723d 6f70 7469 6f6e 5f63 6f6c 6f72 290d  r=option_color).
+000016c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000016d0: 662e 6472 6177 6572 2e70 6c61 6365 286f  f.drawer.place(o
+000016e0: 7074 696f 6e5f 696e 6469 6361 746f 7220  ption_indicator 
+000016f0: 2b20 5f5f 6f70 7469 6f6e 2c0d 0a20 2020  + __option,..   
+00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001710: 2020 2020 2020 2020 2020 2070 6f73 3d28             pos=(
+00001720: 6361 7074 696f 6e5f 7374 6172 742c 2031  caption_start, 1
+00001730: 202b 2069 2929 0d0a 0d0a 0d0a 636c 6173   + i))......clas
+00001740: 7320 5769 6467 6574 496e 7075 7428 5769  s WidgetInput(Wi
+00001750: 6467 6574 293a 0d0a 2020 2020 6465 6620  dget):..    def 
+00001760: 5f5f 696e 6974 5f5f 2873 656c 662c 0d0a  __init__(self,..
+00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001780: 2074 6578 743a 2073 7472 2c0d 0a20 2020   text: str,..   
+00001790: 2020 2020 2020 2020 2020 2020 2020 7369                si
+000017a0: 7a65 3a20 5369 7a65 203d 204e 6f6e 652c  ze: Size = None,
+000017b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000017c0: 2020 2070 6f73 3a20 506f 696e 7420 3d20     pos: Point = 
+000017d0: 506f 696e 7428 302c 2030 292c 0d0a 2020  Point(0, 0),..  
+000017e0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000017f0: 6c6c 6f77 6564 5f63 6861 7261 6374 6572  llowed_character
+00001800: 733a 2073 7472 203d 2022 2061 6263 6465  s: str = " abcde
+00001810: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
+00001820: 7677 7879 7a30 3132 3334 3536 3738 395f  vwxyz0123456789_
+00001830: 2d2b 2f5c 5c28 295b 5d2e 222c 0d0a 2020  -+/\\()[].",..  
+00001840: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+00001850: 2a6b 7761 7267 730d 0a20 2020 2020 2020  *kwargs..       
+00001860: 2020 2020 2020 2020 2020 293a 0d0a 2020            ):..  
+00001870: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+00001880: 696e 6974 5f5f 2873 697a 652c 2070 6f73  init__(size, pos
+00001890: 2c20 2a2a 6b77 6172 6773 290d 0a20 2020  , **kwargs)..   
+000018a0: 2020 2020 2023 2070 203d 2031 0d0a 2020       # p = 1..  
+000018b0: 2020 2020 2020 7365 6c66 2e73 697a 652e        self.size.
+000018c0: 6820 3d20 310d 0a20 2020 2020 2020 2073  h = 1..        s
+000018d0: 656c 662e 7465 7874 203d 2074 6578 740d  elf.text = text.
+000018e0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+000018f0: 6967 6874 203d 2031 0d0a 2020 2020 2020  ight = 1..      
+00001900: 2020 7365 6c66 2e69 6e70 7574 203d 2022    self.input = "
+00001910: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
+00001920: 706f 696e 7465 7220 3d20 300d 0a20 2020  pointer = 0..   
+00001930: 2020 2020 2073 656c 662e 7669 6577 203d       self.view =
+00001940: 2030 0d0a 2020 2020 2020 2020 7365 6c66   0..        self
+00001950: 2e73 686f 775f 706f 696e 7465 7220 3d20  .show_pointer = 
+00001960: 4661 6c73 650d 0a20 2020 2020 2020 2023  False..        #
+00001970: 2063 6861 7261 6374 6572 7320 7468 6174   characters that
+00001980: 2074 6869 7320 6469 616c 6f75 6765 2077   this dialouge w
+00001990: 696c 6c20 6c69 7374 656e 2074 6f0d 0a20  ill listen to.. 
+000019a0: 2020 2020 2020 2073 656c 662e 616c 6c6f         self.allo
+000019b0: 7765 645f 6368 6172 6163 7465 7273 203d  wed_characters =
+000019c0: 2061 6c6c 6f77 6564 5f63 6861 7261 6374   allowed_charact
+000019d0: 6572 730d 0a20 2020 2020 2020 2073 656c  ers..        sel
+000019e0: 662e 7469 636b 203d 2030 0d0a 0d0a 2020  f.tick = 0....  
+000019f0: 2020 6465 6620 7275 6e5f 6361 6c6c 6261    def run_callba
+00001a00: 636b 7328 7365 6c66 293a 0d0a 2020 2020  cks(self):..    
+00001a10: 2020 2020 7375 7065 7228 292e 7275 6e5f      super().run_
+00001a20: 6361 6c6c 6261 636b 7328 290d 0a20 2020  callbacks()..   
+00001a30: 2020 2020 2073 656c 662e 7061 7265 6e74       self.parent
+00001a40: 2e63 6c6f 7365 2829 0d0a 2020 2020 2020  .close()..      
+00001a50: 2020 7365 6c66 2e72 6573 756c 7420 3d20    self.result = 
+00001a60: 7365 6c66 2e69 6e70 7574 0d0a 2020 2020  self.input..    
+00001a70: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00001a80: 7265 7375 6c74 0d0a 0d0a 2020 2020 6465  result....    de
+00001a90: 6620 7265 7365 7428 7365 6c66 293a 0d0a  f reset(self):..
+00001aa0: 2020 2020 2020 2020 7365 6c66 2e69 6e70          self.inp
+00001ab0: 7574 203d 2022 220d 0a20 2020 2020 2020  ut = ""..       
+00001ac0: 2073 656c 662e 706f 696e 7465 7220 3d20   self.pointer = 
+00001ad0: 300d 0a20 2020 2020 2020 2073 656c 662e  0..        self.
+00001ae0: 7669 6577 203d 2030 0d0a 0d0a 2020 2020  view = 0....    
+00001af0: 6465 6620 6765 745f 6d61 785f 6c65 6e67  def get_max_leng
+00001b00: 7468 2873 656c 6629 3a0d 0a20 2020 2020  th(self):..     
+00001b10: 2020 2070 203d 2032 0d0a 2020 2020 2020     p = 2..      
+00001b20: 2020 6d61 785f 696e 7075 745f 6c65 6e20    max_input_len 
+00001b30: 3d20 7365 6c66 2e73 697a 652e 6765 7457  = self.size.getW
+00001b40: 6964 7468 2829 2d28 7020 2a20 3229 2d6c  idth()-(p * 2)-l
+00001b50: 656e 2873 656c 662e 7465 7874 290d 0a20  en(self.text).. 
+00001b60: 2020 2020 2020 2072 6574 7572 6e20 6d61         return ma
+00001b70: 785f 696e 7075 745f 6c65 6e0d 0a0d 0a20  x_input_len.... 
+00001b80: 2020 2064 6566 2075 7064 6174 6528 7365     def update(se
+00001b90: 6c66 2c20 6b65 7929 3a0d 0a20 2020 2020  lf, key):..     
+00001ba0: 2020 206b 6579 203d 2073 7570 6572 2829     key = super()
+00001bb0: 2e75 7064 6174 6528 6b65 7929 0d0a 2020  .update(key)..  
+00001bc0: 2020 2020 2020 6966 206b 6579 2069 7320        if key is 
+00001bd0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00001be0: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
+00001bf0: 2020 206d 6178 5f69 6e70 7574 5f6c 656e     max_input_len
+00001c00: 203d 2073 656c 662e 6765 745f 6d61 785f   = self.get_max_
+00001c10: 6c65 6e67 7468 2829 0d0a 2020 2020 2020  length()..      
+00001c20: 2020 2320 6361 7074 7572 6520 616e 6420    # capture and 
+00001c30: 706c 6163 6520 6368 6172 6163 7465 7273  place characters
+00001c40: 0d0a 2020 2020 2020 2020 6966 206b 6579  ..        if key
+00001c50: 2e6c 6f77 6572 2829 2069 6e20 7365 6c66  .lower() in self
+00001c60: 2e61 6c6c 6f77 6564 5f63 6861 7261 6374  .allowed_charact
+00001c70: 6572 733a 0d0a 2020 2020 2020 2020 2020  ers:..          
+00001c80: 2020 7365 6c66 2e69 6e70 7574 203d 2073    self.input = s
+00001c90: 656c 662e 696e 7075 745b 3a73 656c 662e  elf.input[:self.
+00001ca0: 706f 696e 7465 725d 202b 205c 0d0a 2020  pointer] + \..  
+00001cb0: 2020 2020 2020 2020 2020 2020 2020 6b65                ke
+00001cc0: 7920 2b20 7365 6c66 2e69 6e70 7574 5b73  y + self.input[s
+00001cd0: 656c 662e 706f 696e 7465 723a 5d0d 0a20  elf.pointer:].. 
+00001ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001cf0: 706f 696e 7465 7220 2b3d 2031 0d0a 2020  pointer += 1..  
+00001d00: 2020 2020 2020 2020 2020 6966 2028 6c65            if (le
+00001d10: 6e28 7365 6c66 2e69 6e70 7574 292d 7365  n(self.input)-se
+00001d20: 6c66 2e76 6965 7729 203e 2028 6d61 785f  lf.view) > (max_
+00001d30: 696e 7075 745f 6c65 6e2d 3129 3a0d 0a20  input_len-1):.. 
+00001d40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001d50: 656c 662e 7669 6577 202b 3d20 310d 0a20  elf.view += 1.. 
+00001d60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001d70: 6e0d 0a0d 0a20 2020 2020 2020 2023 2062  n....        # b
+00001d80: 6163 6b73 7061 6365 0d0a 2020 2020 2020  ackspace..      
+00001d90: 2020 6966 206b 6579 203d 3d20 4b65 792e    if key == Key.
+00001da0: 4241 434b 5350 4143 453a 0d0a 2020 2020  BACKSPACE:..    
+00001db0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00001dc0: 706f 696e 7465 7220 213d 2030 3a0d 0a20  pointer != 0:.. 
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001de0: 656c 662e 696e 7075 7420 3d20 7365 6c66  elf.input = self
+00001df0: 2e69 6e70 7574 5b3a 7365 6c66 2e70 6f69  .input[:self.poi
+00001e00: 6e74 6572 202d 0d0a 2020 2020 2020 2020  nter -..        
+00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 315d 202b 2073 656c 662e 696e 7075 745b  1] + self.input[
+00001e40: 7365 6c66 2e70 6f69 6e74 6572 3a5d 0d0a  self.pointer:]..
+00001e50: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00001e60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001e70: 2020 2073 656c 662e 696e 7075 7420 3d20     self.input = 
+00001e80: 7365 6c66 2e69 6e70 7574 5b73 656c 662e  self.input[self.
+00001e90: 706f 696e 7465 723a 5d0d 0a20 2020 2020  pointer:]..     
+00001ea0: 2020 2020 2020 2073 656c 662e 706f 696e         self.poin
+00001eb0: 7465 7220 3d20 6d61 7828 7365 6c66 2e70  ter = max(self.p
+00001ec0: 6f69 6e74 6572 202d 2031 2c20 3029 0d0a  ointer - 1, 0)..
+00001ed0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00001ee0: 656c 662e 706f 696e 7465 722d 7365 6c66  elf.pointer-self
+00001ef0: 2e76 6965 7720 3c20 303a 0d0a 2020 2020  .view < 0:..    
+00001f00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001f10: 2e76 6965 7720 3d20 6d61 7828 7365 6c66  .view = max(self
+00001f20: 2e76 6965 7720 2d20 6d61 785f 696e 7075  .view - max_inpu
+00001f30: 745f 6c65 6e2c 2030 290d 0a20 2020 2020  t_len, 0)..     
+00001f40: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
+00001f50: 0a20 2020 2020 2020 2023 2064 656c 6574  .        # delet
+00001f60: 650d 0a20 2020 2020 2020 2069 6620 6b65  e..        if ke
+00001f70: 7920 3d3d 204b 6579 2e44 454c 4554 453a  y == Key.DELETE:
+00001f80: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00001f90: 6c66 2e69 6e70 7574 203d 2073 656c 662e  lf.input = self.
+00001fa0: 696e 7075 745b 3a73 656c 662e 706f 696e  input[:self.poin
+00001fb0: 7465 725d 202b 205c 0d0a 2020 2020 2020  ter] + \..      
+00001fc0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+00001fd0: 6e70 7574 5b73 656c 662e 706f 696e 7465  nput[self.pointe
+00001fe0: 722b 313a 5d0d 0a20 2020 2020 2020 2020  r+1:]..         
+00001ff0: 2020 2023 2073 656c 662e 706f 696e 7465     # self.pointe
+00002000: 7220 3d20 6d61 7828 7365 6c66 2e70 6f69  r = max(self.poi
+00002010: 6e74 6572 202d 2031 2c20 3029 0d0a 2020  nter - 1, 0)..  
+00002020: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002030: 0d0a 0d0a 2020 2020 2020 2020 2320 6c65  ....        # le
+00002040: 6674 2061 7272 6f77 0d0a 2020 2020 2020  ft arrow..      
+00002050: 2020 6966 206b 6579 203d 3d20 4b65 792e    if key == Key.
+00002060: 4c45 4654 3a0d 0a20 2020 2020 2020 2020  LEFT:..         
+00002070: 2020 2073 656c 662e 706f 696e 7465 7220     self.pointer 
+00002080: 3d20 6d61 7828 7365 6c66 2e70 6f69 6e74  = max(self.point
+00002090: 6572 202d 2031 2c20 3029 0d0a 2020 2020  er - 1, 0)..    
+000020a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000020b0: 706f 696e 7465 722d 7365 6c66 2e76 6965  pointer-self.vie
+000020c0: 7720 3c20 303a 0d0a 2020 2020 2020 2020  w < 0:..        
+000020d0: 2020 2020 2020 2020 7365 6c66 2e76 6965          self.vie
+000020e0: 7720 3d20 6d61 7828 7365 6c66 2e76 6965  w = max(self.vie
+000020f0: 7720 2d20 312c 2030 290d 0a20 2020 2020  w - 1, 0)..     
+00002100: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
+00002110: 0a20 2020 2020 2020 2023 2072 6967 6874  .        # right
+00002120: 2061 7272 6f77 0d0a 2020 2020 2020 2020   arrow..        
+00002130: 6966 206b 6579 203d 3d20 4b65 792e 5249  if key == Key.RI
+00002140: 4748 543a 0d0a 2020 2020 2020 2020 2020  GHT:..          
+00002150: 2020 7365 6c66 2e70 6f69 6e74 6572 203d    self.pointer =
+00002160: 206d 696e 2873 656c 662e 706f 696e 7465   min(self.pointe
+00002170: 7220 2b20 312c 206c 656e 2873 656c 662e  r + 1, len(self.
+00002180: 696e 7075 7429 290d 0a20 2020 2020 2020  input))..       
+00002190: 2020 2020 2069 6620 7365 6c66 2e76 6965       if self.vie
+000021a0: 7720 3d3d 2028 7365 6c66 2e70 6f69 6e74  w == (self.point
+000021b0: 6572 2d6d 6178 5f69 6e70 7574 5f6c 656e  er-max_input_len
+000021c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000021d0: 2020 2020 7365 6c66 2e76 6965 7720 3d20      self.view = 
+000021e0: 6d69 6e28 7365 6c66 2e76 6965 7720 2b20  min(self.view + 
+000021f0: 312c 206c 656e 2873 656c 662e 696e 7075  1, len(self.inpu
+00002200: 7429 290d 0a20 2020 2020 2020 2020 2020  t))..           
+00002210: 2072 6574 7572 6e0d 0a0d 0a20 2020 2020   return....     
+00002220: 2020 2069 6620 6b65 7920 3d3d 2022 5550     if key == "UP
+00002230: 4441 5445 223a 0d0a 2020 2020 2020 2020  DATE":..        
+00002240: 2020 2020 7365 6c66 2e74 6963 6b20 2b3d      self.tick +=
+00002250: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
+00002260: 7365 6c66 2e73 686f 775f 706f 696e 7465  self.show_pointe
+00002270: 7220 3d20 2873 656c 662e 7469 636b 2025  r = (self.tick %
+00002280: 2031 3229 203e 3d20 360d 0a20 2020 2020   12) >= 6..     
+00002290: 2020 2072 6574 7572 6e20 6b65 790d 0a0d     return key...
+000022a0: 0a20 2020 2064 6566 2066 6f72 6d61 745f  .    def format_
+000022b0: 7465 7874 626f 7828 7365 6c66 293a 0d0a  textbox(self):..
+000022c0: 2020 2020 2020 2020 7465 7874 2c20 696e          text, in
+000022d0: 702c 2070 6f69 6e74 6572 2c20 7669 6577  p, pointer, view
+000022e0: 203d 2073 656c 662e 7465 7874 2c20 7365   = self.text, se
+000022f0: 6c66 2e69 6e70 7574 2c20 7365 6c66 2e70  lf.input, self.p
+00002300: 6f69 6e74 6572 2c20 7365 6c66 2e76 6965  ointer, self.vie
+00002310: 770d 0a20 2020 2020 2020 206d 6178 5f69  w..        max_i
+00002320: 6e70 7574 5f6c 656e 203d 2073 656c 662e  nput_len = self.
+00002330: 6765 745f 6d61 785f 6c65 6e67 7468 2829  get_max_length()
+00002340: 0d0a 2020 2020 2020 2020 2320 6765 7420  ..        # get 
+00002350: 7468 6520 696e 7075 7420 7465 7874 2077  the input text w
+00002360: 6974 6820 6669 7865 6420 6c65 6e67 7468  ith fixed length
+00002370: 2070 6c75 7320 6f6e 6520 6578 7472 6120   plus one extra 
+00002380: 7370 6163 6520 666f 7220 7468 6520 706f  space for the po
+00002390: 696e 7465 720d 0a20 2020 2020 2020 2069  inter..        i
+000023a0: 6620 7669 6577 2b6d 6178 5f69 6e70 7574  f view+max_input
+000023b0: 5f6c 656e 2d31 203c 206c 656e 2869 6e70  _len-1 < len(inp
+000023c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000023d0: 696e 705f 203d 2069 6e70 5b76 6965 773a  inp_ = inp[view:
+000023e0: 7669 6577 2b6d 6178 5f69 6e70 7574 5f6c  view+max_input_l
+000023f0: 656e 5d0d 0a20 2020 2020 2020 2065 6c73  en]..        els
+00002400: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002410: 696e 705f 203d 2069 6e70 5b76 6965 773a  inp_ = inp[view:
+00002420: 7669 6577 2b6d 6178 5f69 6e70 7574 5f6c  view+max_input_l
+00002430: 656e 2d31 5d20 2b20 2220 220d 0a0d 0a20  en-1] + " ".... 
+00002440: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00002450: 6c66 2e69 735f 6469 7361 626c 6564 2061  lf.is_disabled a
+00002460: 6e64 2073 656c 662e 7368 6f77 5f70 6f69  nd self.show_poi
+00002470: 6e74 6572 206f 7220 696e 705f 5b70 6f69  nter or inp_[poi
+00002480: 6e74 6572 2d76 6965 775d 2021 3d20 2220  nter-view] != " 
+00002490: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+000024a0: 706f 696e 7465 725f 7374 7220 3d20 4353  pointer_str = CS
+000024b0: 7472 280d 0a20 2020 2020 2020 2020 2020  tr(..           
+000024c0: 2020 2020 2069 6e70 5f5b 706f 696e 7465       inp_[pointe
+000024d0: 722d 7669 6577 5d2c 2062 6163 6b63 6f6c  r-view], backcol
+000024e0: 6f72 3d28 3232 302c 2032 3230 2c20 3232  or=(220, 220, 22
+000024f0: 3029 2c20 666f 7265 636f 6c6f 723d 2832  0), forecolor=(2
+00002500: 302c 2032 302c 2032 3029 290d 0a20 2020  0, 20, 20))..   
+00002510: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00002520: 2020 2020 2020 2020 706f 696e 7465 725f          pointer_
+00002530: 7374 7220 3d20 4353 7472 2869 6e70 5f5b  str = CStr(inp_[
+00002540: 706f 696e 7465 722d 7669 6577 5d29 0d0a  pointer-view])..
+00002550: 2020 2020 2020 2020 2320 696e 7365 7274          # insert
+00002560: 2074 6865 2070 6f69 6e74 6572 2069 6e74   the pointer int
+00002570: 6f20 696e 7075 7420 7465 7874 2061 7420  o input text at 
+00002580: 7468 6520 636f 7272 6563 7420 706f 7369  the correct posi
+00002590: 7469 6f6e 0d0a 2020 2020 2020 2020 696e  tion..        in
+000025a0: 7075 745f 706c 7573 5f70 6f69 6e74 6572  put_plus_pointer
+000025b0: 203d 2043 5374 7228 0d0a 2020 2020 2020   = CStr(..      
+000025c0: 2020 2020 2020 696e 705f 5b3a 706f 696e        inp_[:poin
+000025d0: 7465 722d 7669 6577 5d29 202b 2070 6f69  ter-view]) + poi
+000025e0: 6e74 6572 5f73 7472 202b 2043 5374 7228  nter_str + CStr(
+000025f0: 696e 705f 5b70 6f69 6e74 6572 2d76 6965  inp_[pointer-vie
+00002600: 772b 313a 5d29 0d0a 0d0a 2020 2020 2020  w+1:])....      
+00002610: 2020 7465 7874 5f63 203d 2028 3530 2c20    text_c = (50, 
+00002620: 3230 302c 2035 3029 0d0a 0d0a 2020 2020  200, 50)....    
+00002630: 2020 2020 6673 7472 203d 2043 5374 7228      fstr = CStr(
+00002640: 7465 7874 2c20 666f 7265 636f 6c6f 723d  text, forecolor=
+00002650: 7465 7874 5f63 290d 0a0d 0a20 2020 2020  text_c)....     
+00002660: 2020 2062 6163 6b5f 6578 6973 7473 203d     back_exists =
+00002670: 2043 5374 7228 223c 222c 2066 6f72 6563   CStr("<", forec
+00002680: 6f6c 6f72 3d74 6578 745f 6329 0d0a 2020  olor=text_c)..  
+00002690: 2020 2020 2020 666f 7277 6172 645f 6578        forward_ex
+000026a0: 6973 7473 203d 2043 5374 7228 223e 222c  ists = CStr(">",
+000026b0: 2066 6f72 6563 6f6c 6f72 3d74 6578 745f   forecolor=text_
+000026c0: 6329 0d0a 0d0a 2020 2020 2020 2020 6673  c)....        fs
+000026d0: 7472 202b 3d20 2862 6163 6b5f 6578 6973  tr += (back_exis
+000026e0: 7473 2069 6620 7669 6577 2021 3d20 3020  ts if view != 0 
+000026f0: 656c 7365 2022 2022 290d 0a20 2020 2020  else " ")..     
+00002700: 2020 2066 7374 7220 2b3d 2069 6e70 7574     fstr += input
+00002710: 5f70 6c75 735f 706f 696e 7465 7220 2b20  _plus_pointer + 
+00002720: 2220 2220 2a20 5c0d 0a20 2020 2020 2020  " " * \..       
+00002730: 2020 2020 2028 6d61 785f 696e 7075 745f       (max_input_
+00002740: 6c65 6e20 2d20 6c65 6e28 696e 7075 745f  len - len(input_
+00002750: 706c 7573 5f70 6f69 6e74 6572 2929 0d0a  plus_pointer))..
+00002760: 2020 2020 2020 2020 6673 7472 202b 3d20          fstr += 
+00002770: 2866 6f72 7761 7264 5f65 7869 7374 7320  (forward_exists 
+00002780: 6966 2076 6965 772b 6d61 785f 696e 7075  if view+max_inpu
+00002790: 745f 6c65 6e2d 3120 3c20 6c65 6e28 696e  t_len-1 < len(in
+000027a0: 7029 2065 6c73 6520 2220 2229 0d0a 0d0a  p) else " ")....
+000027b0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+000027c0: 7374 720d 0a0d 0a20 2020 2064 6566 2072  str....    def r
+000027d0: 656e 6465 7228 7365 6c66 293a 0d0a 2020  ender(self):..  
+000027e0: 2020 2020 2020 7020 3d20 310d 0a20 2020        p = 1..   
+000027f0: 2020 2020 2069 6620 7365 6c66 2e70 6172       if self.par
+00002800: 656e 742e 6261 636b 6772 6f75 6e64 5f63  ent.background_c
+00002810: 6f6c 6f72 2069 7320 6e6f 7420 4e6f 6e65  olor is not None
+00002820: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
+00002830: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
+00002840: 745f 7368 6164 6f77 203d 2074 7570 6c65  t_shadow = tuple
+00002850: 286d 6170 286c 616d 6264 6120 783a 2078  (map(lambda x: x
+00002860: 202a 2030 2e38 2c20 6c69 7374 2873 656c   * 0.8, list(sel
+00002870: 662e 7061 7265 6e74 2e62 6163 6b67 726f  f.parent.backgro
+00002880: 756e 645f 636f 6c6f 7229 2929 0d0a 2020  und_color)))..  
+00002890: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+000028a0: 7261 7765 722e 706c 6163 6528 4353 7472  rawer.place(CStr
+000028b0: 2822 2022 202a 2028 7365 6c66 2e73 697a  (" " * (self.siz
+000028c0: 652e 6765 7457 6964 7468 2829 202d 2028  e.getWidth() - (
+000028d0: 7020 2a20 3229 202d 206c 656e 2873 656c  p * 2) - len(sel
+000028e0: 662e 7465 7874 2929 2c20 6261 636b 636f  f.text)), backco
+000028f0: 6c6f 723d 7465 7874 5f73 6861 646f 7729  lor=text_shadow)
+00002900: 2c20 706f 733d 2870 202b 206c 656e 2873  , pos=(p + len(s
+00002910: 656c 662e 7465 7874 292c 2030 2929 0d0a  elf.text), 0))..
+00002920: 2020 2020 2020 2020 7365 6c66 2e64 7261          self.dra
+00002930: 7765 722e 706c 6163 6528 7365 6c66 2e66  wer.place(self.f
+00002940: 6f72 6d61 745f 7465 7874 626f 7828 292c  ormat_textbox(),
+00002950: 2070 6f73 3d28 702c 2030 2929 0d0a 2020   pos=(p, 0))..  
+00002960: 2020 2020 2020 2373 656c 662e 6472 6177        #self.draw
+00002970: 6572 2e77 7269 7465 5f74 6578 7428 7374  er.write_text(st
+00002980: 7228 7465 7874 5f73 6861 646f 7729 2c20  r(text_shadow), 
+00002990: 706f 733d 2830 2c20 3029 290d 0a         pos=(0, 0))..
```

### Comparing `pybud-gui-0.9.5/src/pybud_gui.egg-info/PKG-INFO` & `pybud-gui-0.9.6/src/pybud_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pybud-gui
-Version: 0.9.5
-Summary: Create beautiful console GUIs in python, using Widgets, Dialouges, and more!
+Version: 0.9.6
+Summary: Create beautiful console GUIs in python, using Widgets, Dialogs, and more!
 Author-email: Amirali Mollaei <aam.products.mail@gmail.com>
 License: BSD 4-clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: readchar==4.0.5
```

