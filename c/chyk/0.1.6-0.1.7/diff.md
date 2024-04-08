# Comparing `tmp/chyk-0.1.6-py3-none-any.whl.zip` & `tmp/chyk-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2729 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     1862 b- defN 24-Mar-26 21:35 chyk/__init__.py
--rw-rw-rw-  2.0 fat     1066 b- defN 24-Mar-26 21:36 chyk-0.1.6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      384 b- defN 24-Mar-26 21:36 chyk-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-26 21:36 chyk-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-Mar-26 21:36 chyk-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      446 b- defN 24-Mar-26 21:36 chyk-0.1.6.dist-info/RECORD
-6 files, 3855 bytes uncompressed, 1923 bytes compressed:  50.1%
+Zip file size: 2813 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     2064 b- defN 24-Apr-08 17:36 chyk/__init__.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 24-Apr-08 17:36 chyk-0.1.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      384 b- defN 24-Apr-08 17:36 chyk-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 17:36 chyk-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-08 17:36 chyk-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      446 b- defN 24-Apr-08 17:36 chyk-0.1.7.dist-info/RECORD
+6 files, 4057 bytes uncompressed, 2007 bytes compressed:  50.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: chyk/__init__.py
 Comment: 
 
-Filename: chyk-0.1.6.dist-info/LICENSE.txt
+Filename: chyk-0.1.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: chyk-0.1.6.dist-info/METADATA
+Filename: chyk-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: chyk-0.1.6.dist-info/WHEEL
+Filename: chyk-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: chyk-0.1.6.dist-info/top_level.txt
+Filename: chyk-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: chyk-0.1.6.dist-info/RECORD
+Filename: chyk-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chyk/__init__.py

```diff
@@ -1,46 +1,53 @@
 import handcalcs.render
 import forallpeople as u
 u.environment('default')
 from IPython.display import Latex
-from math import sqrt, pi, cos, sin, tan, log10, log2, log, e, atan2, acos, asin
+from numpy import sqrt, pi, cos, sin, tan, log10, log2, log, e, arctan, arccos, arcsin
 import numpy as np
+from math import atan2,acos,asin
 sqrt = np.emath.sqrt
 from matplotlib import pyplot as plt
 from scipy.integrate import quad
 from scipy.optimize import fsolve
+from scipy.optimize import curve_fit
 from scipy.constants import c
 from latex2sympy2 import latex2sympy, latex2latex
 import sympy as sym
 from sympy import roots
 from sympy.abc import x, a, b
 from sympy import integrate
 from sympy import lambdify
 from sympy import Symbol
 from sympy.solvers import solve
+from sympy import re, im
 from tabulate import tabulate
 import pandas as pd
 from fgmkr import fgmk, fgmk2, fgmk_help
 
 # Separates imaginary and real components
 def ri(imag):
     return [sp.re(imag), sp.im(imag)]
 
 # Finds angle in degrees of an imaginary number
 def ang(imag):
-    return atan2(sp.im(imag),sp.re(imag))*180/pi
+    return atan2(im(imag),re(imag))*180/pi
 
 # Custom notation to pretty-fy outputs for phasor notation
 deg = Symbol('^\circ')
 deg_C = Symbol('^\circ\,C')
 deg_K = Symbol('^\circ\,K')
 aag = Symbol('\, Magnitude\, \, @ \,')
 def cphas(mag_in, angle_in):
     return mag_in*aag + angle_in*deg
 
+# Zero Shift Timescale
+def zeroshift(raw):
+    return raw - min(raw) if raw.size else np.array([])
+
 # Embedded Separators
 Part_A = Symbol('Part\, A\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :')
 Part_B = Symbol('Part\, B\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :')
 Part_C = Symbol('Part\, C\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :')
 Part_D = Symbol('Part\, D\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :')
 
 # Debugging Marker
```

## Comparing `chyk-0.1.6.dist-info/LICENSE.txt` & `chyk-0.1.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

