# Comparing `tmp/chyk-0.1.7-py3-none-any.whl.zip` & `tmp/chyk-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2813 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     2064 b- defN 24-Apr-08 17:36 chyk/__init__.py
--rw-rw-rw-  2.0 fat     1066 b- defN 24-Apr-08 17:36 chyk-0.1.7.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      384 b- defN 24-Apr-08 17:36 chyk-0.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 17:36 chyk-0.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-08 17:36 chyk-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      446 b- defN 24-Apr-08 17:36 chyk-0.1.7.dist-info/RECORD
-6 files, 4057 bytes uncompressed, 2007 bytes compressed:  50.5%
+Zip file size: 2942 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     2392 b- defN 24-Apr-08 19:23 chyk/__init__.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 24-Apr-08 19:24 chyk-0.1.8.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      384 b- defN 24-Apr-08 19:24 chyk-0.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 19:24 chyk-0.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-08 19:24 chyk-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      446 b- defN 24-Apr-08 19:24 chyk-0.1.8.dist-info/RECORD
+6 files, 4385 bytes uncompressed, 2136 bytes compressed:  51.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: chyk/__init__.py
 Comment: 
 
-Filename: chyk-0.1.7.dist-info/LICENSE.txt
+Filename: chyk-0.1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: chyk-0.1.7.dist-info/METADATA
+Filename: chyk-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: chyk-0.1.7.dist-info/WHEEL
+Filename: chyk-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: chyk-0.1.7.dist-info/top_level.txt
+Filename: chyk-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: chyk-0.1.7.dist-info/RECORD
+Filename: chyk-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chyk/__init__.py

```diff
@@ -22,29 +22,39 @@
 from sympy import re, im
 from tabulate import tabulate
 import pandas as pd
 from fgmkr import fgmk, fgmk2, fgmk_help
 
 # Separates imaginary and real components
 def ri(imag):
-    return [sp.re(imag), sp.im(imag)]
+    return [re(imag), im(imag)]
 
 # Finds angle in degrees of an imaginary number
 def ang(imag):
     return atan2(im(imag),re(imag))*180/pi
 
 # Custom notation to pretty-fy outputs for phasor notation
 deg = Symbol('^\circ')
 deg_C = Symbol('^\circ\,C')
 deg_K = Symbol('^\circ\,K')
-aag = Symbol('\, Magnitude\, \, @ \,')
 def cphas(mag_in, angle_in):
-    return mag_in*aag + angle_in*deg
+    return f'{mag_in}' r'\,\, $\angle$' + f'\,{angle_in}' + r'$^\circ$'
 
-# Zero Shift Timescale
+# Phasor to Rectangular
+def p2r(mag, phi):
+    r_num = mag * (cos(phi) + sin(phi)*1j)
+    if abs(r_num.real) < 1e-10: r_num = complex(0, r_num.imag)
+    if abs(r_num.imag) < 1e-10: r_num = complex(r_num.real, 0)
+    return r_num
+
+# Phasor to Rectangular, Degree Inputs
+def p2rd(mag, phi):
+    return p2r(mag, phi*pi/180)
+
+# Zero Shift Array Timescale
 def zeroshift(raw):
     return raw - min(raw) if raw.size else np.array([])
 
 # Embedded Separators
 Part_A = Symbol('Part\, A\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :')
 Part_B = Symbol('Part\, B\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :')
 Part_C = Symbol('Part\, C\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :\quad :')
```

## Comparing `chyk-0.1.7.dist-info/LICENSE.txt` & `chyk-0.1.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

