# Comparing `tmp/gerber_writer-0.4.2.19.tar.gz` & `tmp/gerber_writer-0.4.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerber_writer-0.4.2.19.tar", last modified: Wed Dec  6 19:19:56 2023, max compression
+gzip compressed data, was "gerber_writer-0.4.2.20.tar", last modified: Mon Apr  8 09:42:33 2024, max compression
```

## Comparing `gerber_writer-0.4.2.19.tar` & `gerber_writer-0.4.2.20.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2023-12-06 19:19:56.049621 gerber_writer-0.4.2.19/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    11357 2023-12-04 16:10:40.000000 gerber_writer-0.4.2.19/LICENSE
--rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2745 2023-12-06 19:19:56.049621 gerber_writer-0.4.2.19/PKG-INFO
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1983 2023-12-04 16:10:40.000000 gerber_writer-0.4.2.19/README.rst
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1148 2023-12-06 19:14:14.000000 gerber_writer-0.4.2.19/pyproject.toml
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       38 2023-12-06 19:19:56.049621 gerber_writer-0.4.2.19/setup.cfg
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2023-12-06 19:19:56.049621 gerber_writer-0.4.2.19/src/
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2023-12-06 19:19:56.049621 gerber_writer-0.4.2.19/src/gerber_writer/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       78 2023-12-06 19:14:36.000000 gerber_writer-0.4.2.19/src/gerber_writer/__init__.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      168 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.19/src/gerber_writer/lutils.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2133 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.19/src/gerber_writer/macros.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    10964 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.19/src/gerber_writer/padmasters.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    56389 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.19/src/gerber_writer/writer.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    20619 2023-12-04 16:51:31.000000 gerber_writer-0.4.2.19/src/gerber_writer/writer_test.py
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2023-12-06 19:19:56.049621 gerber_writer-0.4.2.19/src/gerber_writer.egg-info/
--rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2745 2023-12-06 19:19:56.000000 gerber_writer-0.4.2.19/src/gerber_writer.egg-info/PKG-INFO
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      418 2023-12-06 19:19:56.000000 gerber_writer-0.4.2.19/src/gerber_writer.egg-info/SOURCES.txt
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)        1 2023-12-06 19:19:56.000000 gerber_writer-0.4.2.19/src/gerber_writer.egg-info/dependency_links.txt
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       14 2023-12-06 19:19:56.000000 gerber_writer-0.4.2.19/src/gerber_writer.egg-info/top_level.txt
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2023-12-06 19:19:56.049621 gerber_writer-0.4.2.19/tests/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2401 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.19/tests/test_arcs.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1264 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.19/tests/test_contours.py
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-08 09:42:33.925345 gerber_writer-0.4.2.20/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    11357 2023-12-04 16:10:40.000000 gerber_writer-0.4.2.20/LICENSE
+-rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2743 2024-04-08 09:42:33.925345 gerber_writer-0.4.2.20/PKG-INFO
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1981 2024-03-16 14:00:10.000000 gerber_writer-0.4.2.20/README.rst
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1068 2024-03-26 17:03:58.000000 gerber_writer-0.4.2.20/pyproject.toml
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       38 2024-04-08 09:42:33.925345 gerber_writer-0.4.2.20/setup.cfg
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-08 09:42:33.921345 gerber_writer-0.4.2.20/src/
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-08 09:42:33.921345 gerber_writer-0.4.2.20/src/gerber_writer/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       78 2024-03-26 16:34:58.000000 gerber_writer-0.4.2.20/src/gerber_writer/__init__.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      250 2024-03-24 15:01:36.000000 gerber_writer-0.4.2.20/src/gerber_writer/lutils.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2133 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.20/src/gerber_writer/macros.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    10754 2024-03-16 14:00:10.000000 gerber_writer-0.4.2.20/src/gerber_writer/padmasters.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    56441 2024-03-16 14:00:10.000000 gerber_writer-0.4.2.20/src/gerber_writer/writer.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    20619 2023-12-04 16:51:31.000000 gerber_writer-0.4.2.20/src/gerber_writer/writer_test.py
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-08 09:42:33.925345 gerber_writer-0.4.2.20/src/gerber_writer.egg-info/
+-rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2743 2024-04-08 09:42:33.000000 gerber_writer-0.4.2.20/src/gerber_writer.egg-info/PKG-INFO
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      418 2024-04-08 09:42:33.000000 gerber_writer-0.4.2.20/src/gerber_writer.egg-info/SOURCES.txt
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)        1 2024-04-08 09:42:33.000000 gerber_writer-0.4.2.20/src/gerber_writer.egg-info/dependency_links.txt
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       14 2024-04-08 09:42:33.000000 gerber_writer-0.4.2.20/src/gerber_writer.egg-info/top_level.txt
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-08 09:42:33.925345 gerber_writer-0.4.2.20/tests/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2401 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.20/tests/test_arcs.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1264 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.20/tests/test_contours.py
```

### Comparing `gerber_writer-0.4.2.19/LICENSE` & `gerber_writer-0.4.2.20/LICENSE`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.19/PKG-INFO` & `gerber_writer-0.4.2.20/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gerber_writer
-Version: 0.4.2.19
+Version: 0.4.2.20
 Summary: A library to write Gerber files
 Author-email: Karel Tavernier <karel_tavernier@hotmail.com>
 License: Apache 2.0 License
-Project-URL: Homepage, https://github.com/Karel-Tavernier/gerber_writer
+Project-URL: Homepage, https://github.com/alaindef/gerber_writer_project
 Project-URL: Documentation, https://alaindef.github.io/
 Keywords: Gerber,RS-274X,PCB,CAD,CAM,library
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Readme
 ======
 
 Purpose
@@ -61,15 +61,15 @@
 
 .. image:: https://github.com/Karel-Tavernier/gerber_writer/assets/56170852/7b351186-9cdc-4cc0-9f3b-04708ee50216
 	:width: 800
 
 Installation
 ------------
 
-This package requires Python 3.10 or later, you can find it `here <https://www.python.org/downloads/>`_.
+This package requires Python 3.9 or later, you can find it `here <https://www.python.org/downloads/>`_.
 
 +++++++
 Windows
 +++++++
 
 .. code-block:: batch
 
@@ -82,15 +82,15 @@
 .. code-block:: batch
 
 	$ python3 -m pip install gerber_writer
 
 Requirements
 ------------
 
-* Python 3.10 or higher
+* Python 3.9 or higher
 * Standard library only.
 * OS independent.
 
 License
 -------
 
 Apache 2.0 license
```

### Comparing `gerber_writer-0.4.2.19/README.rst` & `gerber_writer-0.4.2.20/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 .. image:: https://github.com/Karel-Tavernier/gerber_writer/assets/56170852/7b351186-9cdc-4cc0-9f3b-04708ee50216
 	:width: 800
 
 Installation
 ------------
 
-This package requires Python 3.10 or later, you can find it `here <https://www.python.org/downloads/>`_.
+This package requires Python 3.9 or later, you can find it `here <https://www.python.org/downloads/>`_.
 
 +++++++
 Windows
 +++++++
 
 .. code-block:: batch
 
@@ -62,15 +62,15 @@
 .. code-block:: batch
 
 	$ python3 -m pip install gerber_writer
 
 Requirements
 ------------
 
-* Python 3.10 or higher
+* Python 3.9 or higher
 * Standard library only.
 * OS independent.
 
 License
 -------
 
 Apache 2.0 license
```

### Comparing `gerber_writer-0.4.2.19/src/gerber_writer/macros.py` & `gerber_writer-0.4.2.20/src/gerber_writer/macros.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.19/src/gerber_writer/padmasters.py` & `gerber_writer-0.4.2.20/src/gerber_writer/padmasters.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 # Copyright: Karel Tavernier
 # License: Apache 2.0 license
 # 
 # Revision history
 
 from dataclasses import dataclass
 from math import sqrt
+from .lutils import isreal
+
 
 @dataclass(frozen = True)
 class Circle:
     """A pad master with circular shape.
     
     A pad master serves to add pads to the graphics objects list. It defines
     their geometric shape, function and polarity (positive or negative).
@@ -40,15 +42,15 @@
     :param bool negative: Polarity, negative if True, positive if False (default)
     """
     
     diameter: float
     function: str
     negative: bool = False
     def __post_init__(self):
-        if not isinstance(self.diameter, float|int):
+        if not isreal(self.diameter):
             raise TypeError('diameter must be int or float')
         if self.diameter <0 :
             raise ValueError('diameter must be >=0')
         if not isinstance(self.function, str):
             raise TypeError('function must be str')
         if not isinstance(self.negative, bool):
             raise TypeError('function must be bool')
@@ -64,19 +66,19 @@
     """
     
     x_size: float
     y_size: float
     function: str
     negative: bool = False
     def __post_init__(self):
-        if not isinstance(self.x_size, float|int):
+        if not isreal(self.x_size):
             raise TypeError('X size must be int or float')
         if self.x_size <= 0:
             raise ValueError('X size must be >=0')
-        if not isinstance(self.y_size, float|int):
+        if not isreal(self.y_size):
             raise TypeError('Y size must be int or float')
         if  self.y_size <= 0:
             raise ValueError('Y size must be >=0')
         if not isinstance(self.function, str):
             raise TypeError('Function must be str')
         if not isinstance(self.negative, bool):
             raise TypeError('Function must be bool')
@@ -94,23 +96,23 @@
     
     x_size: float
     y_size: float
     radius: float
     function: str
     negative: bool = False
     def __post_init__(self):
-        if not isinstance(self.x_size, float|int):
+        if not isreal(self.x_size):
             raise TypeError('x_size must be int or float')
         if self.x_size <= 0:
             raise ValueError('x_size must be >0')
-        if not isinstance(self.y_size, float|int):
+        if not isreal(self.y_size):
             raise TypeError('y_size must be int or float')
         if  self.y_size <= 0:
             raise ValueError('y_size must be >0')
-        if not isinstance(self.radius, float|int):
+        if not isreal(self.radius):
             raise TypeError('radius must be int or float')
         if not (0 <= self.radius <= 0.5*min(self.x_size, self.y_size)):
             raise ValueError('radius must be: 0 <= radius <= half the smallest side')            
         if not isinstance(self.function, str):
             raise TypeError('function must be str')
         if not isinstance(self.negative, bool):
             raise TypeError('Function must be bool')
@@ -128,23 +130,23 @@
     
     x_size: float
     y_size: float
     cutoff: float
     function: str
     negative: bool = False
     def __post_init__(self):
-        if not isinstance(self.x_size, float|int):
+        if not isreal(self.x_size):
             raise TypeError('X size must be int or float')
         if self.x_size <= 0:
             raise ValueError('X size must be >=0')
-        if not isinstance(self.y_size, float|int):
+        if not isreal(self.y_size):
             raise TypeError('Y size must be int or float')
         if  self.y_size <= 0:
             raise ValueError('Y size must be >=0')
-        if not isinstance(self.cutoff, float|int):
+        if not isreal(self.cutoff):
             raise TypeError('Cutoff must be int or float')
         if not (0 <= self.cutoff <= 0.5*min(self.x_size, self.y_size)):
             raise ValueError('Cutoff must be: 0 <= cutoff <= half the smallest side')            
         if not isinstance(self.function, str):
             raise TypeError('Function must be str')
 
 @dataclass(frozen=True)      
@@ -160,15 +162,15 @@
     
     outer_diameter: float
     inner_diameter: float
     gap: float
     function: str
     negative: bool = False
     def __post_init__(self):
-        if not (isinstance(self.outer_diameter, int|float) and isinstance(self.inner_diameter, int|float) and isinstance(self.gap, int|float)):
+        if not (isreal(self.outer_diameter) and isreal(self.inner_diameter) and isreal(self.gap)):
             raise TypeError('arguments must be int or float')
         if not (0 < self.inner_diameter < self.outer_diameter):
             raise ValueError('diameter values invalid')
         if not(0 < self.gap < self.outer_diameter/sqrt(2)):
             raise ValueError('gap only valid if 0 < gap <= outer_diameter/math.sqrt(2)')
             
 @dataclass(frozen=True)      
@@ -184,15 +186,15 @@
     
     outer_diameter: float
     inner_diameter: float
     gap: float
     function: str
     negative: bool = False
     def __post_init__(self):
-        if not (isinstance(self.outer_diameter, int|float) and isinstance(self.inner_diameter, int|float) and isinstance(self.gap, int|float)):
+        if not (isreal(self.outer_diameter) and isreal(self.inner_diameter) and isreal(self.gap)):
             raise TypeError('arguments must be int or float')
         if not (self.outer_diameter>0 and self.inner_diameter>0 and self.gap>0):
             raise ValueError('parameters must be strictly positive')
         if (self.gap + self.outer_diameter - self.inner_diameter)*2*sqrt(2) >= (self.outer_diameter + self.inner_diameter): # for simpler rounding
 #        if self.gap*sqrt(2) >= (self.inner_diameter - (1 + sqrt(2))*(self.outer_diameter - self.inner_diameter)):
             raise ValueError('gap too big in relation to diameters')
             
@@ -209,15 +211,15 @@
     """
     
     outer_diameter: float
     vertices: int
     function: str
     negative: bool = False
     def __post_init__(self):
-        if not isinstance(self.outer_diameter, float|int):
+        if not isreal(self.outer_diameter):
             raise TypeError('outer_diameter must be int or float')
         if self.outer_diameter <= 0:
             raise ValueError('outer_diameter must be >=0')
         if not isinstance(self.vertices, int):
             raise TypeError('vertices must be int or float')
         if self.vertices not in range(3,13) :
             raise ValueError('vertices must be from 3 up to 12')
```

### Comparing `gerber_writer-0.4.2.19/src/gerber_writer/writer.py` & `gerber_writer-0.4.2.20/src/gerber_writer/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-.. module:: gerber_wrier
+.. module:: gerber_writer
    :synopsis: A simple API for writing Gerber files
 .. moduleauthor:: Karel Tavernier <karel_tavernier@hotmail.com>
 
 Gerber format - a primer
 ========================
 
 A Gerber file represents the image of PCB layer. 
@@ -266,15 +266,15 @@
 from collections import deque
 from math import sqrt, sin, cos, acos, radians
 from typing import NamedTuple, Set, Dict, List, Tuple, Deque
 import types
 
 # adf  #todo check if import math is needed
 import math
-from .lutils import report_with_line
+from .lutils import report_with_line, isreal
 # import inspect    # for debug reporting
 
 from .__init__ import __version__
 from .padmasters import (
     Circle,
     Rectangle,
     RoundedRectangle,
@@ -644,15 +644,15 @@
         >>> top.add_pad(smd_pad, (5, -2.5), 45)        
         
         """
         if not isinstance(master.function, str):
             raise ValueError('function must be string')        
         if not isinstance(position, tuple):
             raise ValueError('position must be a tuple of two float coordinates')
-        if not isinstance(angle, float|int):
+        if not isreal(angle):
             raise TypeError('angle must be int or float')                        
         # to be expanded with real checks on function, probably using regex
         self.g_o_stream.append(DataLayer._Pad(master, position, angle))
 
 # adf
         report_with_line(f'line has position {position} and datalayer has max {self.pointMax}')
         self.pointMax = _pnt_max(position, self.pointMax)
@@ -677,15 +677,15 @@
             raise TypeError('start is not a tuple')
         if not isinstance(end, tuple):
             raise TypeError('end is not a tuple')      
         if not isinstance(function, str):
             raise TypeError('function is not a str')
         if not isinstance(negative, bool):
             raise TypeError('negative is not bool')     
-        if not isinstance(width, float|int): 
+        if not isreal(width):
             raise TypeError('Width is not int or float')
         if width<0:
             raise ValueError('width is not >= 0')
         
         line = Path()
         line.moveto(start)
         line.lineto(end)      
@@ -718,15 +718,15 @@
             raise TypeError('end is not a tuple')
         if not isinstance(center, tuple):
             raise TypeError('center is not a tuple')                 
         if not isinstance(function, str):
             raise TypeError('function is not str')
         if not isinstance(negative, bool):
             raise TypeError('negative is not bool')     
-        if not isinstance(width, float|int): 
+        if not isreal(width):
             raise TypeError('Width is not int or float')
         if width<0:
             raise ValueError('width is not >= 0')
         arc = Path()
         arc.moveto(start)
         arc.arcto(end, center, orientation)      
         self.g_o_stream.append(DataLayer._TracesPath(arc, width, function, negative))
@@ -754,15 +754,15 @@
         >>> copper_top.add_traces_path(connection, 0.1, 'Conductor')
         >>> len(copper_top)
         1
         
         """        
         if not isinstance(path, Path):
             raise TypeError('path is not a Path instance')
-        if not isinstance(width, float|int): 
+        if not isreal(width):
             raise TypeError('width is not int or float')
         if width<0:
             raise ValueError('width is not >= 0')
         if not isinstance(function, str): 
             raise TypeError('function is not str')        
         if not isinstance(negative, bool):
             raise TypeError('negative flag is not bool')        
@@ -918,41 +918,38 @@
             
             :param Path path: the path that contains the operators.
             :param bool always_do2: if True always generate the d02
                                     even when not needed by current state
                                     d02 is mandatory at the start of a contour
             """
             for operator in path.operators:
-                match operator:
-                
-                    case _MoveTo():
+                if isinstance(operator, _MoveTo):
                         if always_d02:
                             body_commands.append(
                                 f'X{_pnt_gerber(operator.to)[0]}'
                                 f'Y{_pnt_gerber(operator.to)[1]}'
                                 f'D02*'
                                 )                                   
                         else:
                             handle_d02(operator.to)
                         
-                    case _LineTo():            
+                elif isinstance(operator, _LineTo):            
                         handle_g0n('G01*')
                         body_commands.append(
                             f'X{_pnt_gerber(operator.to)[0]}'
                             f'Y{_pnt_gerber(operator.to)[1]}'
                             f'D01*'
                             )
                             
-                    case _ArcTo():
-                        match operator.orientation:
-                            case '+':
-                                handle_g0n('G03*')                                        
-                            case '-':
+                elif isinstance(operator, _ArcTo):
+                        if operator.orientation == '+':
+                                handle_g0n('G03*')
+                        elif operator.orientation == '-':
                                 handle_g0n('G02*')
-                            case _:
+                        else:
                                 assert False, 'Orientation must be "+" or "-" '
                         chord_short = _pnt_linf(graphics_state.point, operator.to) < TOLERANCE/2
                         arc_small = _pnt_orientation(operator.center, graphics_state.point, operator.to) == operator.orientation
                         radius_long = _pnt_linf(operator.center, operator.to) > TOLERANCE
                         if chord_short and arc_small and radius_long:
                             # Output as line instead of arc segment to avoid instability
                             body_commands.append(
@@ -966,44 +963,43 @@
                                 f'X{_pnt_gerber(operator.to)[0]}'
                                 f'Y{_pnt_gerber(operator.to)[1]}'
                                 f'I{_pnt_gerber(_pnt_offset(operator.center, graphics_state.point))[0]}'
                                 f'J{_pnt_gerber(_pnt_offset(operator.center, graphics_state.point))[1]}'                                                            
                                 f'D01*'
                                 )
                             
-                    case _:
+                else:
                         assert False, 'Unknown path construction operator'
 
                 graphics_state.point = operator.to
         
         # Process graphics objects:
         # compute macro and aperture dicts, AD and operation command list        
         for graphics_object in self.g_o_stream:        
-            match graphics_object:
-            
-                case DataLayer._TracesPath():
+            # match graphics_object:
+            if isinstance(graphics_object, DataLayer._TracesPath):
                     handle_trace_lp_ad_dnn()
                     handle_path_operators(graphics_object.path, always_d02=False)            
             
-                case DataLayer._Region():
+            elif isinstance(graphics_object, DataLayer._Region):
                     handle_lp(graphics_object.negative)
                     if graphics_object.function != '':                        
                         body_commands.append(f'G04 #@! TA.AperFunction,{graphics_object.function}*')                
                     body_commands.append('G36*')
                     handle_path_operators(graphics_object.path, always_d02=True)
                     body_commands.append('G37*')
                     if graphics_object.function != '':                            
                         body_commands.append('G04 #@! TD*')
             
-                case DataLayer._Pad() if isinstance(graphics_object.master, Circle):
+            elif isinstance(graphics_object, DataLayer._Pad) and isinstance(graphics_object.master, Circle):
                     shape = f'Circle,{graphics_object.master.diameter}'
                     ad_body = f'C,{graphics_object.master.diameter}'
                     handle_flash(shape, ad_body)
 
-                case DataLayer._Pad() if isinstance(graphics_object.master, Rectangle):
+            elif isinstance(graphics_object, DataLayer._Pad) and isinstance(graphics_object.master, Rectangle):
                     shape = (
                         f'Rectangle,'
                         f'{graphics_object.master.x_size},'
                         f'{graphics_object.master.y_size},'
                         f'{graphics_object.angle}'
                         )
                     if graphics_object.angle%180 == 0:
@@ -1018,15 +1014,15 @@
                             f'Rectangle,'
                             f'{graphics_object.master.x_size/2}X'
                             f'{graphics_object.master.y_size/2}X'
                             f'{graphics_object.angle}'          
                             )                                    
                     handle_flash(shape, ad_body)             
 
-                case DataLayer._Pad() if isinstance(graphics_object.master, RoundedRectangle):                        
+            elif isinstance(graphics_object, DataLayer._Pad) and isinstance(graphics_object.master, RoundedRectangle):
                     x_size = graphics_object.master.x_size
                     y_size = graphics_object.master.y_size                            
                     radius = graphics_object.master.radius
                     angle = graphics_object.angle
                     shape = f'RoundedRectangle,{x_size},{y_size},{radius},{angle}'
                     if ((min(x_size, y_size) - 2*radius) < TOLERANCE) and (angle%90==0):
                         # Becomes obround
@@ -1048,15 +1044,15 @@
                             f'{round(center_q1[0], DECIMALS)}X'
                             f'{round(center_q1[1], DECIMALS)}X'
                             f'{round(center_q2[0], DECIMALS)}X'
                             f'{round(center_q2[1], DECIMALS)}'
                             )
                     handle_flash(shape, ad_body)                  
 
-                case DataLayer._Pad() if isinstance(graphics_object.master, ChamferedRectangle):
+            elif isinstance(graphics_object, DataLayer._Pad) and isinstance(graphics_object.master, ChamferedRectangle):
                     shape = (
                         f'ChamferedRectangle,'
                         f'{graphics_object.master.x_size},'
                         f'{graphics_object.master.y_size},'
                         f'{graphics_object.master.cutoff},'
                         f'{graphics_object.angle}'
                         )
@@ -1067,15 +1063,15 @@
                         f'{graphics_object.master.y_size/2}X'
                         f'{graphics_object.master.x_size/2-graphics_object.master.cutoff}X'
                         f'{graphics_object.master.y_size/2-graphics_object.master.cutoff}X'
                         f'{graphics_object.angle}'
                         )
                     handle_flash(shape, ad_body)
                                                                      
-                case DataLayer._Pad() if isinstance(graphics_object.master, Thermal):            
+            elif isinstance(graphics_object, DataLayer._Pad) and isinstance(graphics_object.master, Thermal):
                     shape = (
                         f'Thermal,'
                         f'{graphics_object.master.outer_diameter},'
                         f'{graphics_object.master.inner_diameter},'
                         f'{graphics_object.master.gap},'
                         f'{graphics_object.angle}'
                         )
@@ -1085,15 +1081,15 @@
                         f'{graphics_object.master.outer_diameter}X'
                         f'{graphics_object.master.inner_diameter}X'
                         f'{graphics_object.master.gap}X'
                         f'{graphics_object.angle}'
                         )
                     handle_flash(shape, ad_body)
                         
-                case DataLayer._Pad() if isinstance(graphics_object.master, RoundedThermal):
+            elif isinstance(graphics_object, DataLayer._Pad) and isinstance(graphics_object.master, RoundedThermal):
                     shape = (
                         f'RoundedThermal,'
                         f'{graphics_object.master.outer_diameter},'
                         f'{graphics_object.master.inner_diameter},'
                         f'{graphics_object.master.gap},'
                         f'{graphics_object.angle}'
                         )
@@ -1147,30 +1143,30 @@
                         f'{round(center_h[0], DECIMALS)}X'
                         f'{round(center_h[1], DECIMALS)}X'           
                         f'{round(center_v[0], DECIMALS)}X'          
                         f'{round(center_v[1], DECIMALS)}'                                                   
                         )
                     handle_flash(shape, ad_body)
                     
-                case DataLayer._Pad() if isinstance(graphics_object.master, RegularPolygon):
+            elif isinstance(graphics_object, DataLayer._Pad) and isinstance(graphics_object.master, RegularPolygon):
                     shape = (
                         f'RegularPolygon,'
                     f'{graphics_object.master.outer_diameter},'
                         f'{graphics_object.master.vertices},'
                         f'{graphics_object.angle}'
                         )
                     ad_body = (
                         r'P,'
                         f'{graphics_object.master.outer_diameter}X'
                         f'{graphics_object.master.vertices}X'
                         f'{graphics_object.angle}'
                         )
                     handle_flash(shape, ad_body)                            
                     
-                case DataLayer._Pad() if isinstance(graphics_object.master, UserPolygon):
+            elif isinstance(graphics_object, DataLayer._Pad) and isinstance(graphics_object.master, UserPolygon):
                     macro_name = polygons.get(graphics_object.master.polygon)
                     if macro_name is None: # polygon does not yet exist
                         # add polygon to polygons dict         
                         macro_name = f'UserPolygon_{next(generate_polygon_number)}'                                 
                         polygons[graphics_object.master.polygon] = macro_name
                         # define macro and add it to macros set                                                                 
                         macro_definition = []
@@ -1180,16 +1176,16 @@
                         macro_definition.append('$1*')
                         macro_definition.append('%')
                         macros.add('\n'.join(macro_definition))                       
                     shape = f'UserPolygon,{graphics_object.angle}'
                     ad_body = f'{macro_name},{graphics_object.angle}'
                     handle_flash(shape, ad_body)
                         
-                case _:
-                    assert False, 'Unknown graphics object'
+            else:
+                assert False, 'Unknown graphics object'
 
         # Construct list of all commands
         # Header
         all_commands: List = list() # Stream of all commands that will be in the Gerber file
         all_commands.append(f'G04 Created with the python gerber_writer {__version__}*')
         all_commands.append(f'G04 #@! TF.CreationDate,{datetime.datetime.now().isoformat()}*')
         if self.function != '':
```

### Comparing `gerber_writer-0.4.2.19/src/gerber_writer/writer_test.py` & `gerber_writer-0.4.2.20/src/gerber_writer/writer_test.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.19/src/gerber_writer.egg-info/PKG-INFO` & `gerber_writer-0.4.2.20/src/gerber_writer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: gerber-writer
-Version: 0.4.2.19
+Name: gerber_writer
+Version: 0.4.2.20
 Summary: A library to write Gerber files
 Author-email: Karel Tavernier <karel_tavernier@hotmail.com>
 License: Apache 2.0 License
-Project-URL: Homepage, https://github.com/Karel-Tavernier/gerber_writer
+Project-URL: Homepage, https://github.com/alaindef/gerber_writer_project
 Project-URL: Documentation, https://alaindef.github.io/
 Keywords: Gerber,RS-274X,PCB,CAD,CAM,library
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Readme
 ======
 
 Purpose
@@ -61,15 +61,15 @@
 
 .. image:: https://github.com/Karel-Tavernier/gerber_writer/assets/56170852/7b351186-9cdc-4cc0-9f3b-04708ee50216
 	:width: 800
 
 Installation
 ------------
 
-This package requires Python 3.10 or later, you can find it `here <https://www.python.org/downloads/>`_.
+This package requires Python 3.9 or later, you can find it `here <https://www.python.org/downloads/>`_.
 
 +++++++
 Windows
 +++++++
 
 .. code-block:: batch
 
@@ -82,15 +82,15 @@
 .. code-block:: batch
 
 	$ python3 -m pip install gerber_writer
 
 Requirements
 ------------
 
-* Python 3.10 or higher
+* Python 3.9 or higher
 * Standard library only.
 * OS independent.
 
 License
 -------
 
 Apache 2.0 license
```

### Comparing `gerber_writer-0.4.2.19/tests/test_arcs.py` & `gerber_writer-0.4.2.20/tests/test_arcs.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.19/tests/test_contours.py` & `gerber_writer-0.4.2.20/tests/test_contours.py`

 * *Files identical despite different names*

