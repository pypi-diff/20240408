# Comparing `tmp/casioplot-3.1.7.tar.gz` & `tmp/casioplot-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casioplot-3.1.7.tar", last modified: Thu Apr  4 07:05:10 2024, max compression
+gzip compressed data, was "casioplot-3.2.0.tar", last modified: Mon Apr  8 13:56:11 2024, max compression
```

## Comparing `casioplot-3.1.7.tar` & `casioplot-3.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:10.903474 casioplot-3.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 07:04:59.000000 casioplot-3.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 07:04:59.000000 casioplot-3.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-04 07:05:10.903474 casioplot-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-04 07:04:59.000000 casioplot-3.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-04 07:04:59.000000 casioplot-3.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:05:10.903474 casioplot-3.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:10.899474 casioplot-3.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:10.899474 casioplot-3.1.7/src/casioplot/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 07:04:59.000000 casioplot-3.1.7/src/casioplot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:10.903474 casioplot-3.1.7/src/casioplot/bg_images/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 07:04:59.000000 casioplot-3.1.7/src/casioplot/bg_images/blanck.png
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-04 07:04:59.000000 casioplot-3.1.7/src/casioplot/bg_images/calculator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-04-04 07:04:59.000000 casioplot-3.1.7/src/casioplot/casioplot.py
--rw-r--r--   0 runner    (1001) docker     (127)   127297 2024-04-04 07:04:59.000000 casioplot-3.1.7/src/casioplot/characters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:10.903474 casioplot-3.1.7/src/casioplot/presets/
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-04 07:04:59.000000 casioplot-3.1.7/src/casioplot/presets/default.toml
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-04 07:04:59.000000 casioplot-3.1.7/src/casioplot/presets/fx-CG50.toml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 07:04:59.000000 casioplot-3.1.7/src/casioplot/presets/fx-CG50_AU.toml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 07:04:59.000000 casioplot-3.1.7/src/casioplot/presets/graph_90+e.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-04 07:04:59.000000 casioplot-3.1.7/src/casioplot/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-04 07:04:59.000000 casioplot-3.1.7/src/casioplot/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:10.903474 casioplot-3.1.7/src/casioplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-04 07:05:10.000000 casioplot-3.1.7/src/casioplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-04 07:05:10.000000 casioplot-3.1.7/src/casioplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:05:10.000000 casioplot-3.1.7/src/casioplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 07:05:10.000000 casioplot-3.1.7/src/casioplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 07:05:10.000000 casioplot-3.1.7/src/casioplot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:56:11.547819 casioplot-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 13:56:05.000000 casioplot-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 13:56:05.000000 casioplot-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-08 13:56:11.547819 casioplot-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-08 13:56:05.000000 casioplot-3.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-08 13:56:05.000000 casioplot-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:56:11.547819 casioplot-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:56:11.543819 casioplot-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:56:11.543819 casioplot-3.2.0/src/casioplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:56:11.547819 casioplot-3.2.0/src/casioplot/bg_images/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/bg_images/blanck.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/bg_images/calculator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/casioplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127342 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/characters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:56:11.547819 casioplot-3.2.0/src/casioplot/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/presets/default.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/presets/fx-CG50.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/presets/fx-CG50_AU.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/presets/graph_90+e.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:56:11.547819 casioplot-3.2.0/src/casioplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-08 13:56:11.000000 casioplot-3.2.0/src/casioplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-08 13:56:11.000000 casioplot-3.2.0/src/casioplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:56:11.000000 casioplot-3.2.0/src/casioplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 13:56:11.000000 casioplot-3.2.0/src/casioplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 13:56:11.000000 casioplot-3.2.0/src/casioplot.egg-info/top_level.txt
```

### Comparing `casioplot-3.1.7/LICENSE` & `casioplot-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casioplot-3.1.7/PKG-INFO` & `casioplot-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casioplot
-Version: 3.1.7
+Version: 3.2.0
 Summary: Use casioplot module on a computer
 Author-email: Uniwix <uniwixu@gmail.com>, Miguel Torrinha Pereira <miguel.torrinha.pereira+pypi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Uniwix
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -124,8 +124,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 3.1.7 - Uniwix - MiguelTorrinhaPereira
+v 3.2.0 - Uniwix - MiguelTorrinhaPereira
```

### Comparing `casioplot-3.1.7/README.rst` & `casioplot-3.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -83,8 +83,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 3.1.7 - Uniwix - MiguelTorrinhaPereira
+v 3.2.0 - Uniwix - MiguelTorrinhaPereira
```

### Comparing `casioplot-3.1.7/pyproject.toml` & `casioplot-3.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "Pillow"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "casioplot"
-version = "3.1.7"
+version = "3.2.0"
 description = "Use casioplot module on a computer"
 readme = "README.rst"
 authors = [
     { name = "Uniwix", email = "uniwixu@gmail.com" },
     { name = "Miguel Torrinha Pereira", email = "miguel.torrinha.pereira+pypi@gmail.com" }
 ]
 license = { file = "LICENSE" }
```

### Comparing `casioplot-3.1.7/src/casioplot/bg_images/calculator.png` & `casioplot-3.2.0/src/casioplot/bg_images/calculator.png`

 * *Files identical despite different names*

### Comparing `casioplot-3.1.7/src/casioplot/casioplot.py` & `casioplot-3.2.0/src/casioplot/casioplot.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,21 @@
   - :py:func:`set_pixel`
   - :py:func:`get_pixel`
   - :py:func:`draw_string`
 
 Contains the original functions from the :py:mod:`casioplot` calculator module
 and the code needed to emulate the screen.
 """
-
+import atexit
 import tkinter as tk
-from typing import Literal
 
 from PIL import Image, ImageTk  # used to save the screen
 from casioplot.characters import _get_char
 from casioplot.settings import _settings
-from casioplot.types import Color
+from casioplot.types import Color, Text_size
 
 # some frequently used colors
 _WHITE: Color = (255, 255, 255)
 """RGB white"""
 
 _BLACK: Color = (0, 0, 0)
 """RGB black"""
@@ -78,26 +77,22 @@
     These modes are independent and can work at the same time
     """
 
     if _settings["show_screen"] is True:
         # the virtual screen is already updated, the tkinter window just needs to update what it is showing
         _window.update()
 
-    if _settings["save_screen"] is True:
-        if _settings["save_multiple"] is True:
-            global _save_screen_counter, _current_image_number
-            if _save_screen_counter == _settings["save_rate"]:
-                _save_screen(str(_current_image_number))
-                _current_image_number += 1
-                _save_screen_counter = 1
-            else:
-                _save_screen_counter += 1
+    if _settings["save_screen"] is True and _settings["save_multiple"] is True:
+        global _save_screen_counter, _current_image_number
+        if _save_screen_counter == _settings["save_rate"]:
+            _save_screen(str(_current_image_number))
+            _current_image_number += 1
+            _save_screen_counter = 1
         else:
-            # When the program ends, the saved image will show the screen as it was in the last call of show_screen
-            _save_screen()
+            _save_screen_counter += 1
 
 
 def clear_screen() -> None:
     """Clear the canvas, sets every pixel to white"""
     _canvas.put(
         "white",
         to=(0, 0, _settings["width"], _settings["height"])
@@ -138,15 +133,15 @@
 
 
 def draw_string(
         x: int,
         y: int,
         text: str,
         color: Color = _BLACK,
-        size: Literal["small", "medium", "large"] = "medium"
+        size: Text_size = "medium"
 ) -> None:
     """Draw a string on the canvas with the given RGB color and size.
 
     :param x: x coordinate (from the left)
     :param y: y coordinate (from the top)
     :param text: text that will be drawn
     :param color: The color of the text. A tuple that contain 3 integers from 0 to 255
@@ -189,40 +184,52 @@
     else:
         _window.withdraw()
 
     # screen
 
     _canvas = tk.PhotoImage(width=_settings["width"], height=_settings["height"])
     """The canvas that the user can interact with using the functions from this module
-    
+
     :meta hide-value:
     """
     clear_screen()  # ensures the pixels are set to white and not transparent
 
     if _settings["bg_image_is_set"] is True:
         _background = tk.PhotoImage(file=_settings["background_image"])
         """The background image that is shown behind the canvas
-        
+
         :meta hide-value:
         """
     else:
         bg_width, bg_height = _screen_dimensions()
         _background = tk.PhotoImage(width=bg_width, height=bg_height)
         _background.put(  # same as clear_screen but for the background image
             "white",
             to=(0, 0, bg_width, bg_height)
         )
 
     _background_display = tk.Label(master=_window, image=_background, border=0)
     """The tkinter label that shows the background image
-    
+
     :meta hide-value:
     """
     _background_display.place(x=0, y=0)
     _canvas_display = tk.Label(master=_window, image=_canvas, border=0)
     """The tkinter label that shows the canvas
-    
+
     :meta hide-value:
     """
     _canvas_display.place(x=_settings["left_margin"], y=_settings["top_margin"])
 except tk.TclError:
     print("The tkinter window couldn't be created. The screen won't be shown.")
+
+
+@atexit.register
+def run_at_exit() -> None:
+    """This function should be called at the end of the program to close the tkinter window"""
+    if _settings["save_screen"] is True:  # saves the thes screen as it was before the program ended
+        _save_screen()
+    if _settings["show_screen"] is True:  # keeps the tkinter window open after the program ends
+        if _settings["close_window"] is True:
+            _window.destroy()
+        else:
+            _window.mainloop()
```

### Comparing `casioplot-3.1.7/src/casioplot/characters.py` & `casioplot-3.2.0/src/casioplot/characters.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 Every size has it's one dictionary there is a key for every character
 and the values are tuples of strings that represent the character in
 a sort of character map, every string corresponds to a row. An X means that
 the pixel should be set and a space that the pixel should stay as it is.
 """
 
+from casioplot.types import Text_size
+
 # TODO: change how characters are drawn to be more efficient and faster
 
 
 large = {
     " ": (
         "                  ",
         "                  ",
@@ -5355,15 +5357,15 @@
 _size_to_dict = {"small": small, "medium": medium, "large": large}
 """A dictionary that maps the size of the font to the font dictionary
 
 :meta hide-value:
 """
 
 
-def _get_char(char: str, size: str = "medium") -> tuple:
+def _get_char(char: str, size: Text_size = "medium") -> tuple:
     """Gets the char_map of a character in a given size
 
     Gets the character from the dictionaries,
     serves as an interface for :file:`casioplot.py` to get the characters it needs
 
     :param char: The character
     :param size: The size of the character
```

### Comparing `casioplot-3.1.7/src/casioplot/presets/default.toml` & `casioplot-3.2.0/src/casioplot/presets/default.toml`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 bg_image_is_set = false
 # use this image if you don't want to have a background image and not use a default file
 background_image = "bg_images/blanck.png"
 
 # Show the screen with tkinter.
 [showing_screen]
 show_screen = true
+# Close the window at exit.
+close_window = true
 
 # Save the screen in the current directory.
 # If `save_multiple` is set to false, the screen will be saved at each
 # `show_screen` call, overwriting the previous save,
 # the file name will be `image_name` + '.' + `image_format`.
 # If `save_multiple` is set to true, the screen will be saved every time
 # `show_screen` is called `save_rate` times,
```

### Comparing `casioplot-3.1.7/src/casioplot/settings.py` & `casioplot-3.2.0/src/casioplot/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         ),
         "background": (
             "bg_image_is_set",
             "background_image"
         ),
         "showing_screen": (
             "show_screen",
+            "close_window"
         ),
         "saving_screen": (
             "save_screen",
             "image_name",
             "image_format",
             "save_multiple",
             "save_rate"
```

### Comparing `casioplot-3.1.7/src/casioplot/types.py` & `casioplot-3.2.0/src/casioplot/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""This file contains the type :py:class:`Configuration` and the type :py:class:`Color`"""
+"""This file contains the types :py:class:`Configuration`, :py:class:`Color` and :py:class:`Text_size`"""
 
-from typing import TypedDict
+from typing import TypedDict, Literal
 
 
-"""The type :py:class:`Configuration` makes it possible to representing all settings and configs in a dictionary but still
-have type annotations for every setting.
-The option :python:`total=False` makes it possible for a configuration to not have a value for all settings"""
 class Configuration(TypedDict, total=False):
+    """The type :py:class:`Configuration` makes it possible to representing all settings and configs in a dictionary but still
+    have type annotations for every setting.
+    The option :python:`total=False` makes it possible for a configuration to not have a value for all settings"""
+
     # canvas size
     width: int  # canvas width in pixels
     height: int  # canvas height in pixels
 
     # margins
     left_margin: int
     right_margin: int
@@ -19,21 +20,26 @@
 
     # background
     bg_image_is_set: bool  # if it is False the background_image will be ignored
     background_image: str  # some config files like `graph_90+e.toml`
     # have a special background image
 
     # showing_screen
-    show_screen: bool  # do not mistake for the function `show_screen` from `casioplot.py`
+    show_screen: bool  # do not mistake for the function `show_screen` from `casioplot.py
+    close_window: bool  # close the window at exit
 
     # saving_screen
     save_screen: bool  # Save the screen as an image
     image_name: str
     image_format: str  # should be one of the following image formats: jpeg, jpg, png, gif, bmp, tiff or tif
     save_multiple: bool  # save multiple images so that the user can examine better the virtual screen
     save_rate: int  # if `save_multiple is True a new image will be saved`
     # every `save_rate` times show_screen is called
 
 
 Color = tuple[int, int, int]
 """A color is represented as a tuple of three integers, each integer is in the range [0, 255] and represents the
 intensity of the color in the red, green and blue channels respectively."""
+
+
+Text_size = Literal["small", "medium", "large"]
+"""The three accpeted text sizes"""
```

### Comparing `casioplot-3.1.7/src/casioplot.egg-info/PKG-INFO` & `casioplot-3.2.0/src/casioplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casioplot
-Version: 3.1.7
+Version: 3.2.0
 Summary: Use casioplot module on a computer
 Author-email: Uniwix <uniwixu@gmail.com>, Miguel Torrinha Pereira <miguel.torrinha.pereira+pypi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Uniwix
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -124,8 +124,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 3.1.7 - Uniwix - MiguelTorrinhaPereira
+v 3.2.0 - Uniwix - MiguelTorrinhaPereira
```

### Comparing `casioplot-3.1.7/src/casioplot.egg-info/SOURCES.txt` & `casioplot-3.2.0/src/casioplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

