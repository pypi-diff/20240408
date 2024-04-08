# Comparing `tmp/praklib-0.1.421.tar.gz` & `tmp/praklib-0.1.422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.1.421.tar", last modified: Mon Apr  8 18:54:39 2024, max compression
+gzip compressed data, was "praklib-0.1.422.tar", last modified: Mon Apr  8 20:51:40 2024, max compression
```

## Comparing `praklib-0.1.421.tar` & `praklib-0.1.422.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 18:54:38.996932 praklib-0.1.421/
--rw-rw-rw-   0        0        0      263 2024-04-08 18:54:38.995854 praklib-0.1.421/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-08 18:54:38.975005 praklib-0.1.421/praklib/
--rw-rw-rw-   0        0        0     6680 2024-04-08 18:54:18.000000 praklib-0.1.421/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.421/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:54:38.993851 praklib-0.1.421/praklib.egg-info/
--rw-rw-rw-   0        0        0      263 2024-04-08 18:54:38.000000 praklib-0.1.421/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-08 18:54:38.000000 praklib-0.1.421/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 18:54:38.000000 praklib-0.1.421/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 18:54:38.000000 praklib-0.1.421/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 18:54:38.997933 praklib-0.1.421/setup.cfg
--rw-rw-rw-   0        0        0      382 2024-04-08 18:54:37.000000 praklib-0.1.421/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:51:40.633944 praklib-0.1.422/
+-rw-rw-rw-   0        0        0      263 2024-04-08 20:51:40.631912 praklib-0.1.422/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-08 20:51:40.611247 praklib-0.1.422/praklib/
+-rw-rw-rw-   0        0        0     7177 2024-04-08 20:51:20.000000 praklib-0.1.422/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.422/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:51:40.628791 praklib-0.1.422/praklib.egg-info/
+-rw-rw-rw-   0        0        0      263 2024-04-08 20:51:40.000000 praklib-0.1.422/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-08 20:51:40.000000 praklib-0.1.422/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 20:51:40.000000 praklib-0.1.422/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 20:51:40.000000 praklib-0.1.422/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 20:51:40.633944 praklib-0.1.422/setup.cfg
+-rw-rw-rw-   0        0        0      382 2024-04-08 19:01:22.000000 praklib-0.1.422/setup.py
```

### Comparing `praklib-0.1.421/praklib/Praktika.py` & `praklib-0.1.422/praklib/Praktika.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from lmfit import Model
 import uncertainties.unumpy as unp
+import math
 
 
+def first_significant_digit_is_one(num):
+    # Convert number to string
+    num_str = str(num)
+
+    # Remove leading zeros and decimal point
+    num_str = num_str.lstrip('0').lstrip('.').lstrip('0')
+    print(num_str)
+
+    for char in num_str:
+        # If the character is not a decimal point
+        print(char)
+        if char != '.':
+            # Check if the first non-zero digit is '1'
+            return char == '1'
+
+        # If no non-zero digit is found, return False
+    return False
+
 def round_uncertainties(array):
     rounded_values = []
     rounded_errors = []
     for x in array:
         rounded_value, rounded_error = custom_round(x.nominal_value, x.std_dev)
         rounded_values.append(rounded_value)
         rounded_errors.append(rounded_error)
@@ -22,22 +41,23 @@
         return 0.0, 0.0
 
     # Calculate the magnitude of the error
     error_magnitude = int(np.floor(np.log10(error)))
 
     # Determine the rounding precision based on the first decimal digit of the error
     if error_magnitude < 0:
-        rounding_precision = -error_magnitude
-    elif error_magnitude == 0:
-        if int(error * 10) % 10 == 1:
-            rounding_precision = 2
+        if first_significant_digit_is_one(error):
+            rounding_precision = -error_magnitude+1
         else:
-            rounding_precision = 1
+            rounding_precision = -error_magnitude
     else:
-        rounding_precision = 0
+            if first_significant_digit_is_one(error):
+                rounding_precision = error_magnitude+1
+            else :
+                rounding_precision = error_magnitude
 
     # Round the value and the error
     rounded_value = round(value, rounding_precision)
     rounded_error = round(error, rounding_precision)
 
     return rounded_value, rounded_error
 
@@ -176,13 +196,7 @@
     uncertainties = unp.std_devs(unumpy_array)
 
     if imag_errs==False:
         return np.column_stack((values, uncertainties))
     if imag_errs==True:
         result = values + 1j * uncertainties
         return result
-
-unumpy_array = unp.uarray([1, 2, 3], [0.1, 0.2, 0.3])
-
-# Convert to two-dimensional column array
-result = unp_to_np(unumpy_array)
-print(result)
```

