# Comparing `tmp/iranholidays-0.2.2.tar.gz` & `tmp/iranholidays-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iranholidays-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "iranholidays-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `iranholidays-0.2.2.tar` & `iranholidays-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2024-03-28 17:45:22.277181 iranholidays-0.2.2/LICENSE
--rw-r--r--   0        0        0     2066 2024-02-10 05:01:51.433894 iranholidays-0.2.2/README.rst
--rw-r--r--   0        0        0     6129 2024-03-28 17:51:09.635739 iranholidays-0.2.2/iranholidays/__init__.py
--rw-r--r--   0        0        0      859 2024-03-28 17:50:25.441034 iranholidays-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3680 2024-02-06 04:06:22.635762 iranholidays-0.2.2/tests/test_init.py
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 iranholidays-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-28 17:45:22.277181 iranholidays-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2066 2024-02-10 05:01:51.433894 iranholidays-0.2.3/README.rst
+-rw-r--r--   0        0        0     5976 2024-04-08 15:31:05.836102 iranholidays-0.2.3/iranholidays/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-08 15:07:39.143385 iranholidays-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3680 2024-02-06 04:06:22.635762 iranholidays-0.2.3/tests/test_init.py
+-rw-r--r--   0        0        0     2426 1970-01-01 00:00:00.000000 iranholidays-0.2.3/PKG-INFO
```

### Comparing `iranholidays-0.2.2/LICENSE` & `iranholidays-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iranholidays-0.2.2/README.rst` & `iranholidays-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `iranholidays-0.2.2/iranholidays/__init__.py` & `iranholidays-0.2.3/iranholidays/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from collections.abc import Callable as _Callable, Container as _Container
 from datetime import date as _date, datetime as _datetime
 from typing import Literal as _Literal
 
+from gshconverter import (
+    gregorian_to_solar_hijri as _g_to_sh,
+    solar_hijri_to_gregorian as _sh_to_g,
+)
 from hijri_converter import Gregorian as _Gregorian, Hijri as _Hijri
 from jdatetime import date as _jdate, datetime as _jdatetime
-from jdatetime.jalali import (
-    GregorianToJalali as _GregorianToJalali,
-    JalaliToGregorian as _JalaliToGregorian,
-)
 
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 SOLAR_HOLIDAYS = [
     None,
     {  # Farvardīn
         1: 'Nowruz',
         2: 'Nowruz',
         3: 'Nowruz',
@@ -105,15 +105,15 @@
 ) -> OffOccasion:
     if date.weekday() in weekend:
         return 'Weekend'
     year, month, day = date.year, date.month, date.day
     _, hm, hd = _Gregorian(year, month, day).to_hijri().datetuple()
     if (occ := HIJRI_HOLIDAYS[hm].get(hd)) is not None:
         return occ
-    sy, sm, sd = _GregorianToJalali(year, month, day).getJalaliList()
+    sy, sm, sd = _sh_to_g(year, month, day)
     return SOLAR_HOLIDAYS[sm].get(sd)
 
 
 def off_occasion_solar(
     date: _jdate, /, weekend: Weekend = (4,)
 ) -> OffOccasion:
     if date.weekday() in weekend:
@@ -130,17 +130,15 @@
     date: _Hijri, /, weekend: Weekend = (4,)
 ) -> OffOccasion:
     if date.weekday() in weekend:
         return 'Weekend'
     month, day = date.month, date.day
     if (occ := HIJRI_HOLIDAYS[month].get(day)) is not None:
         return occ
-    sy, sm, sd = _GregorianToJalali(
-        *date.to_gregorian().datetuple()
-    ).getJalaliList()
+    sy, sm, sd = _g_to_sh(*date.to_gregorian().datetuple())
     return SOLAR_HOLIDAYS[sm].get(sd)
 
 
 Calendar = _Literal['S', 'L', 'G']
 
 
 def off_occasion_ymd(
@@ -150,15 +148,15 @@
     calendar: Calendar,
     /,
     weekend: Weekend = (4,),
 ) -> OffOccasion:
     if calendar == 'S':
         if (occ := SOLAR_HOLIDAYS[month].get(day)) is not None:
             return occ
-        gy, gm, gd = _JalaliToGregorian(year, month, day).getGregorianList()
+        gy, gm, gd = _sh_to_g(year, month, day)
         gdate = _Gregorian(gy, gm, gd)
         if _date(gy, gm, gd).weekday() in weekend:
             return 'Weekend'
         hdate = gdate.to_hijri()
         hy, hm, hd = hdate.datetuple()
         return HIJRI_HOLIDAYS[hm].get(hd)
 
@@ -168,17 +166,15 @@
 
     elif calendar == 'L':
         if (occ := HIJRI_HOLIDAYS[month].get(day)) is not None:
             return occ
         hdate = _Hijri(year, month, day)
         if hdate.weekday() in weekend:
             return 'Weekend'
-        sy, sm, sd = _GregorianToJalali(
-            *hdate.to_gregorian().datetuple()
-        ).getJalaliList()
+        sy, sm, sd = _g_to_sh(*hdate.to_gregorian().datetuple())
         return SOLAR_HOLIDAYS[sm].get(sd)
 
     else:
         raise ValueError(f'unknown {calendar=}')
 
 
 DateTuple = tuple[int, int, int, Calendar]
```

### Comparing `iranholidays-0.2.2/pyproject.toml` & `iranholidays-0.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 name = 'iranholidays'
 authors = [
     { name = '5j9', email = '5j9@users.noreply.github.com' },
 ]
 description = 'provides functions to tell if a date is a holiday in Iran or not'
 readme = 'README.rst'
 requires-python = '>=3.11'
-dependencies = ['jdatetime', 'hijri-converter']
+dependencies = ['gshconverter', 'hijri-converter']
 dynamic = ['version']
 license = {text = "GPL-3.0"}
 
 [project.urls]
 Homepage = "https://github.com/5j9/iranholidays"
 
 [tool.ruff]
```

### Comparing `iranholidays-0.2.2/tests/test_init.py` & `iranholidays-0.2.3/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iranholidays-0.2.2/PKG-INFO` & `iranholidays-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: iranholidays
-Version: 0.2.2
+Version: 0.2.3
 Summary: provides functions to tell if a date is a holiday in Iran or not
 Author-email: 5j9 <5j9@users.noreply.github.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
-Requires-Dist: jdatetime
+Requires-Dist: gshconverter
 Requires-Dist: hijri-converter
 Project-URL: Homepage, https://github.com/5j9/iranholidays
 
 ``iranholidays`` is a small python library that provides functions to check if a date is a holiday in Iran or not. 
 
 **Warning:** For Islamic holidays, like Eid al-Fitr, the calculation may be off by a day or two since those events depend on seeing the moon by naked eye and cannot be predicted by computers.
```

