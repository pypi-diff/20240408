# Comparing `tmp/chyk-0.1.8-py3-none-any.whl.zip` & `tmp/chyk-0.2.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2942 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     2392 b- defN 24-Apr-08 19:23 chyk/__init__.py
--rw-rw-rw-  2.0 fat     1066 b- defN 24-Apr-08 19:24 chyk-0.1.8.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      384 b- defN 24-Apr-08 19:24 chyk-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 19:24 chyk-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-08 19:24 chyk-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      446 b- defN 24-Apr-08 19:24 chyk-0.1.8.dist-info/RECORD
-6 files, 4385 bytes uncompressed, 2136 bytes compressed:  51.3%
+Zip file size: 3087 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     2664 b- defN 24-Apr-08 19:33 chyk/__init__.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 24-Apr-08 19:42 chyk-0.2.0.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      438 b- defN 24-Apr-08 19:42 chyk-0.2.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 19:42 chyk-0.2.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-08 19:42 chyk-0.2.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      456 b- defN 24-Apr-08 19:42 chyk-0.2.0.1.dist-info/RECORD
+6 files, 4721 bytes uncompressed, 2261 bytes compressed:  52.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: chyk/__init__.py
 Comment: 
 
-Filename: chyk-0.1.8.dist-info/LICENSE.txt
+Filename: chyk-0.2.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: chyk-0.1.8.dist-info/METADATA
+Filename: chyk-0.2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: chyk-0.1.8.dist-info/WHEEL
+Filename: chyk-0.2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: chyk-0.1.8.dist-info/top_level.txt
+Filename: chyk-0.2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: chyk-0.1.8.dist-info/RECORD
+Filename: chyk-0.2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chyk/__init__.py

```diff
@@ -32,16 +32,25 @@
 def ang(imag):
     return atan2(im(imag),re(imag))*180/pi
 
 # Custom notation to pretty-fy outputs for phasor notation
 deg = Symbol('^\circ')
 deg_C = Symbol('^\circ\,C')
 deg_K = Symbol('^\circ\,K')
-def cphas(mag_in, angle_in):
-    return f'{mag_in}' r'\,\, $\angle$' + f'\,{angle_in}' + r'$^\circ$'
+
+# Angle Notation
+def cphas(mag_in, angle_in, omega=None):
+    if omega is not None:
+        return f'{mag_in:.3f}\,\, cos({omega}t {angle_in:.3f}' + r'$^\circ$)'
+    else:
+        return f'{mag_in}' r'\,\, $\angle$' + f'\,{angle_in}' + r'$^\circ$'
+
+# Cosine Notation, including Frequency
+def cphas2(cnum,omega=None):
+    return cphas(abs(cnum), ang(cnum), omega)
 
 # Phasor to Rectangular
 def p2r(mag, phi):
     r_num = mag * (cos(phi) + sin(phi)*1j)
     if abs(r_num.real) < 1e-10: r_num = complex(0, r_num.imag)
     if abs(r_num.imag) < 1e-10: r_num = complex(r_num.real, 0)
     return r_num
```

## Comparing `chyk-0.1.8.dist-info/LICENSE.txt` & `chyk-0.2.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

