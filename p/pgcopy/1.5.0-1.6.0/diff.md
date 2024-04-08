# Comparing `tmp/pgcopy-1.5.0.tar.gz` & `tmp/pgcopy-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pgcopy-1.5.0.tar", last modified: Tue Jan 12 13:28:03 2021, max compression
+gzip compressed data, was "pgcopy-1.6.0.tar", last modified: Mon Apr  8 16:26:37 2024, max compression
```

## Comparing `pgcopy-1.5.0.tar` & `pgcopy-1.6.0.tar`

### file list

```diff
@@ -1,25 +1,39 @@
-drwxr-x---   0 altaurog  (1000) altaurog  (1000)        0 2021-01-12 13:28:03.000000 pgcopy-1.5.0/
--rw-r-----   0 altaurog  (1000) altaurog  (1000)      441 2020-01-29 20:51:20.000000 pgcopy-1.5.0/AUTHORS.rst
--rw-r-----   0 altaurog  (1000) altaurog  (1000)     1921 2021-01-12 10:43:36.000000 pgcopy-1.5.0/CHANGELOG.rst
--rw-r-----   0 altaurog  (1000) altaurog  (1000)     1131 2021-01-12 10:44:33.000000 pgcopy-1.5.0/LICENSE.txt
--rw-r-----   0 altaurog  (1000) altaurog  (1000)       20 2015-08-11 13:55:20.000000 pgcopy-1.5.0/MANIFEST.in
--rw-r-----   0 altaurog  (1000) altaurog  (1000)     3999 2021-01-12 13:28:03.000000 pgcopy-1.5.0/PKG-INFO
--rw-r-----   0 altaurog  (1000) altaurog  (1000)     2443 2021-01-12 10:39:20.000000 pgcopy-1.5.0/README.rst
-drwxr-x---   0 altaurog  (1000) altaurog  (1000)        0 2021-01-12 13:28:03.000000 pgcopy-1.5.0/pgcopy/
--rw-r-----   0 altaurog  (1000) altaurog  (1000)       89 2019-12-14 20:07:18.000000 pgcopy-1.5.0/pgcopy/__init__.py
--rw-r-----   0 altaurog  (1000) altaurog  (1000)    10255 2021-01-12 10:28:03.000000 pgcopy-1.5.0/pgcopy/copy.py
-drwxr-x---   0 altaurog  (1000) altaurog  (1000)        0 2021-01-12 13:28:03.000000 pgcopy-1.5.0/pgcopy/errors/
--rw-r-----   0 altaurog  (1000) altaurog  (1000)      234 2020-10-16 11:14:25.000000 pgcopy-1.5.0/pgcopy/errors/__init__.py
--rw-r-----   0 altaurog  (1000) altaurog  (1000)      290 2020-10-16 11:14:25.000000 pgcopy-1.5.0/pgcopy/errors/py2.py
--rw-r-----   0 altaurog  (1000) altaurog  (1000)      143 2020-10-16 11:14:25.000000 pgcopy-1.5.0/pgcopy/errors/py3.py
--rw-r-----   0 altaurog  (1000) altaurog  (1000)     1160 2019-12-14 20:07:18.000000 pgcopy-1.5.0/pgcopy/inspect.py
--rw-r-----   0 altaurog  (1000) altaurog  (1000)    12278 2020-04-26 18:42:46.000000 pgcopy-1.5.0/pgcopy/util.py
--rw-r-----   0 altaurog  (1000) altaurog  (1000)       22 2021-01-12 10:45:56.000000 pgcopy-1.5.0/pgcopy/version.py
-drwxr-x---   0 altaurog  (1000) altaurog  (1000)        0 2021-01-12 13:28:03.000000 pgcopy-1.5.0/pgcopy.egg-info/
--rw-r-----   0 altaurog  (1000) altaurog  (1000)     3999 2021-01-12 13:28:03.000000 pgcopy-1.5.0/pgcopy.egg-info/PKG-INFO
--rw-r-----   0 altaurog  (1000) altaurog  (1000)      381 2021-01-12 13:28:03.000000 pgcopy-1.5.0/pgcopy.egg-info/SOURCES.txt
--rw-r-----   0 altaurog  (1000) altaurog  (1000)        1 2021-01-12 13:28:03.000000 pgcopy-1.5.0/pgcopy.egg-info/dependency_links.txt
--rw-r-----   0 altaurog  (1000) altaurog  (1000)       14 2021-01-12 13:28:03.000000 pgcopy-1.5.0/pgcopy.egg-info/requires.txt
--rw-r-----   0 altaurog  (1000) altaurog  (1000)        7 2021-01-12 13:28:03.000000 pgcopy-1.5.0/pgcopy.egg-info/top_level.txt
--rw-r-----   0 altaurog  (1000) altaurog  (1000)      177 2021-01-12 13:28:03.000000 pgcopy-1.5.0/setup.cfg
--rw-r-----   0 altaurog  (1000) altaurog  (1000)     1625 2021-01-12 13:09:14.000000 pgcopy-1.5.0/setup.py
+drwxr-x---   0 altaurog  (1000) altaurog  (1000)        0 2024-04-08 16:26:37.886091 pgcopy-1.6.0/
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)      505 2024-04-08 11:55:31.000000 pgcopy-1.6.0/AUTHORS.rst
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)     2282 2024-04-08 11:55:31.000000 pgcopy-1.6.0/CHANGELOG.rst
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)     1131 2024-04-08 11:55:31.000000 pgcopy-1.6.0/LICENSE.txt
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)       20 2015-08-11 13:55:20.000000 pgcopy-1.6.0/MANIFEST.in
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)     3320 2024-04-08 16:26:37.886091 pgcopy-1.6.0/PKG-INFO
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)     2580 2024-04-08 11:55:31.000000 pgcopy-1.6.0/README.rst
+drwxr-x---   0 altaurog  (1000) altaurog  (1000)        0 2024-04-08 16:26:37.882091 pgcopy-1.6.0/pgcopy/
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)       89 2023-02-27 14:52:59.000000 pgcopy-1.6.0/pgcopy/__init__.py
+drwxr-x---   0 altaurog  (1000) altaurog  (1000)        0 2024-04-08 16:26:37.882091 pgcopy-1.6.0/pgcopy/contrib/
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)        0 2024-04-08 11:55:31.000000 pgcopy-1.6.0/pgcopy/contrib/__init__.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)      580 2024-04-08 11:55:31.000000 pgcopy-1.6.0/pgcopy/contrib/vector.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)    10453 2024-04-08 11:55:31.000000 pgcopy-1.6.0/pgcopy/copy.py
+drwxr-x---   0 altaurog  (1000) altaurog  (1000)        0 2024-04-08 16:26:37.886091 pgcopy-1.6.0/pgcopy/errors/
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)      235 2023-03-01 16:57:33.000000 pgcopy-1.6.0/pgcopy/errors/__init__.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)      337 2023-03-01 16:57:33.000000 pgcopy-1.6.0/pgcopy/errors/py2.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)      143 2023-03-01 16:57:33.000000 pgcopy-1.6.0/pgcopy/errors/py3.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)     1160 2023-03-01 17:20:33.000000 pgcopy-1.6.0/pgcopy/inspect.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)      325 2024-04-08 11:55:31.000000 pgcopy-1.6.0/pgcopy/thread.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)    12501 2024-04-08 11:55:31.000000 pgcopy-1.6.0/pgcopy/util.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)       22 2024-04-08 11:55:31.000000 pgcopy-1.6.0/pgcopy/version.py
+drwxr-x---   0 altaurog  (1000) altaurog  (1000)        0 2024-04-08 16:26:37.882091 pgcopy-1.6.0/pgcopy.egg-info/
+-rw-r--r--   0 altaurog  (1000) altaurog  (1000)     3320 2024-04-08 16:26:37.000000 pgcopy-1.6.0/pgcopy.egg-info/PKG-INFO
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)      653 2024-04-08 16:26:37.000000 pgcopy-1.6.0/pgcopy.egg-info/SOURCES.txt
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)        1 2024-04-08 16:26:37.000000 pgcopy-1.6.0/pgcopy.egg-info/dependency_links.txt
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)       14 2024-04-08 16:26:37.000000 pgcopy-1.6.0/pgcopy.egg-info/requires.txt
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)        7 2024-04-08 16:26:37.000000 pgcopy-1.6.0/pgcopy.egg-info/top_level.txt
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)      177 2024-04-08 16:26:37.886091 pgcopy-1.6.0/setup.cfg
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)     1628 2024-04-08 11:55:31.000000 pgcopy-1.6.0/setup.py
+drwxr-x---   0 altaurog  (1000) altaurog  (1000)        0 2024-04-08 16:26:37.886091 pgcopy-1.6.0/tests/
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)      651 2023-03-01 16:57:33.000000 pgcopy-1.6.0/tests/test_array.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)      332 2024-04-08 11:55:31.000000 pgcopy-1.6.0/tests/test_contrib.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)     6851 2024-04-08 11:55:31.000000 pgcopy-1.6.0/tests/test_datatypes.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)     1507 2024-04-08 11:55:31.000000 pgcopy-1.6.0/tests/test_errors.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)     7205 2024-04-08 11:55:31.000000 pgcopy-1.6.0/tests/test_replace.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)     1380 2024-04-08 11:55:31.000000 pgcopy-1.6.0/tests/test_sanity.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)     1120 2024-04-08 11:55:31.000000 pgcopy-1.6.0/tests/test_schema.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)      540 2024-04-08 11:55:31.000000 pgcopy-1.6.0/tests/test_stringio.py
+-rw-r-----   0 altaurog  (1000) altaurog  (1000)     1385 2024-04-08 11:55:31.000000 pgcopy-1.6.0/tests/test_threading_copy.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pgcopy-1.5.0/LICENSE.txt` & `pgcopy-1.6.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 License
 --------
 
-Copyright (C) 2014 - 2021 Aryeh Leib Taurog <python@aryehleib.com>
+Copyright (C) 2014 - 2024 Aryeh Leib Taurog <python@aryehleib.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following conditions:
```

### Comparing `pgcopy-1.5.0/README.rst` & `pgcopy-1.6.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. home-start
 
 pgcopy
 =======
 
-.. image:: https://travis-ci.org/altaurog/pgcopy.svg?branch=master
-    :target: https://travis-ci.org/altaurog/pgcopy
+.. image:: https://github.com/altaurog/pgcopy/actions/workflows/test.yaml/badge.svg?branch=master
+    :target: https://github.com/altaurog/pgcopy/actions/workflows/test.yaml?query=branch%3Avector
 
 .. image:: https://coveralls.io/repos/github/altaurog/pgcopy/badge.svg?branch=master
     :target: https://coveralls.io/github/altaurog/pgcopy?branch=master
 
 .. image:: https://img.shields.io/pypi/l/pgcopy.svg
     :target: https://pypi.org/project/pgcopy/
 
@@ -25,14 +25,15 @@
 .. _pgcopy: https://pgcopy.readthedocs.io/en/latest/
 
 Features
 ---------
 * Support for many data types
 * Support for multi-dimensional array types
 * Support for schema and schema search path
+* Support for mixed-case table and column names
 * Transparent string encoding
 * Utility for replacing entire table
 
 Quickstart
 -----------
 
 .. quickstart-start
@@ -79,14 +80,15 @@
 * timestamp
 * timestamp with time zone
 * numeric
 * json
 * jsonb
 * uuid
 * arrays
+* vector
 
 Documentation
 --------------
 
 `Read the docs.`_
 
 .. _Read the docs.: pgcopy_
```

### Comparing `pgcopy-1.5.0/pgcopy/copy.py` & `pgcopy-1.6.0/pgcopy/copy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,81 @@
 import calendar
 import functools
 import os
 import struct
-import sys
 import tempfile
-import threading
-
 from datetime import date, datetime
 
 try:
     from itertools import izip as zip
 except ImportError:
     pass
 
 from psycopg2.extensions import encodings
+
 from . import errors, inspect, util
+from .thread import RaisingThread
 
-__all__ = ['CopyManager']
+__all__ = ["CopyManager"]
 
-BINCOPY_HEADER = struct.pack('>11sii', b'PGCOPY\n\377\r\n\0', 0, 0)
-BINCOPY_TRAILER = struct.pack('>h', -1)
+BINCOPY_HEADER = struct.pack(">11sii", b"PGCOPY\n\377\r\n\0", 0, 0)
+BINCOPY_TRAILER = struct.pack(">h", -1)
 
 MAX_INT64 = 0xFFFFFFFFFFFFFFFF
 
 
 def simple_formatter(fmt):
-    size = struct.calcsize('>' + fmt)
-    return lambda val: ('i' + fmt, (size, val))
+    size = struct.calcsize(">" + fmt)
+    return lambda val: ("i" + fmt, (size, val))
+
 
 def str_formatter(val):
     size = len(val)
-    return ('i%ss' % size, (size, val))
+    return ("i%ss" % size, (size, val))
+
 
 psql_epoch = 946684800
 psql_epoch_date = date(2000, 1, 1)
 
+
 def timestamp(dt):
-    'get microseconds since 2000-01-01 00:00'
+    "get microseconds since 2000-01-01 00:00"
     # see http://stackoverflow.com/questions/2956886/
     dt = util.to_utc(dt)
     unix_timestamp = calendar.timegm(dt.timetuple())
     # timetuple doesn't maintain microseconds
     # see http://stackoverflow.com/a/14369386/519015
     val = ((unix_timestamp - psql_epoch) * 1000000) + dt.microsecond
-    return ('iq', (8, val))
+    return ("iq", (8, val))
+
 
 def time_formatter(t):
-    'get microseconds since 2000-01-01 00:00'
+    "get microseconds since 2000-01-01 00:00"
     t = util.to_utc_time(t)
     dt = datetime.combine(psql_epoch_date, t)
     return timestamp(dt)
 
+
 def datestamp(d):
-    'days since 2000-01-01'
-    return ('ii', (4, (d - psql_epoch_date).days))
+    "days since 2000-01-01"
+    return ("ii", (4, (d - psql_epoch_date).days))
+
 
 def numeric(n):
     """
     NBASE = 1000
     ndigits = total number of base-NBASE digits
     weight = base-NBASE weight of first digit
     sign = 0x0000 if positive, 0x4000 if negative, 0xC000 if nan
     dscale = decimal digits after decimal place
     """
     try:
         nt = n.as_tuple()
     except AttributeError:
-        raise TypeError('numeric field requires Decimal value (got %r)' % n)
+        raise TypeError("numeric field requires Decimal value (got %r)" % n)
     digits = []
     if isinstance(nt.exponent, str):
         # NaN, Inf, -Inf
         ndigits = 0
         weight = 0
         sign = 0xC000
         dscale = 0
@@ -86,57 +91,58 @@
             digits.insert(0, ndig(decdigits[:4]))
             del decdigits[:4]
         ndigits = len(digits)
         weight += nt.exponent // 4 + ndigits - 1
         sign = nt.sign * 0x4000
         dscale = -min(0, nt.exponent)
     data = [ndigits, weight, sign, dscale] + digits
-    return ('ihhHH%dH' % ndigits, [2 * len(data)] + data)
+    return ("ihhHH%dH" % ndigits, [2 * len(data)] + data)
+
 
 def ndig(a):
     res = 0
     for i, d in enumerate(a):
-        res += d * 10 ** i
+        res += d * 10**i
     return res
 
 
 def jsonb_formatter(val):
     size = len(val)
     # first char must me binary format of jsonb in postgresql
-    return 'ib%is' % size, (size + 1, 1, val)
+    return "ib%is" % size, (size + 1, 1, val)
 
 
 def uuid_formatter(guid):
-    return 'i2Q', (16, (guid.int >> 64) & MAX_INT64, guid.int & MAX_INT64)
+    return "i2Q", (16, (guid.int >> 64) & MAX_INT64, guid.int & MAX_INT64)
 
 
 type_formatters = {
-    'bool': simple_formatter('?'),
-    'int2': simple_formatter('h'),
-    'int4': simple_formatter('i'),
-    'int8': simple_formatter('q'),
-    'float4' : simple_formatter('f'),
-    'float8': simple_formatter('d'),
-    'varchar': str_formatter,
-    'bpchar': str_formatter,
-    'bytea': str_formatter,
-    'text': str_formatter,
-    'json': str_formatter,
-    'jsonb': jsonb_formatter,
-    'date': datestamp,
-    'time': time_formatter,
-    'timestamp': timestamp,
-    'timestamptz': timestamp,
-    'numeric': numeric,
-    'uuid': uuid_formatter,
+    "bool": simple_formatter("?"),
+    "int2": simple_formatter("h"),
+    "int4": simple_formatter("i"),
+    "int8": simple_formatter("q"),
+    "float4": simple_formatter("f"),
+    "float8": simple_formatter("d"),
+    "varchar": str_formatter,
+    "bpchar": str_formatter,
+    "bytea": str_formatter,
+    "text": str_formatter,
+    "json": str_formatter,
+    "jsonb": jsonb_formatter,
+    "date": datestamp,
+    "time": time_formatter,
+    "timestamp": timestamp,
+    "timestamptz": timestamp,
+    "numeric": numeric,
+    "uuid": uuid_formatter,
 }
 
 
 def null_formatter(formatter):
-    return lambda v: ('i', (-1,)) if v is None else formatter(v)
+    return lambda v: ("i", (-1,)) if v is None else formatter(v)
 
 
 def array_formatter(typelem, formatter, val):
     """
     i   total size in bytes
     i   number of dimensions
     i   whether there are nulls or not
@@ -147,84 +153,84 @@
         i   lower bound (when unraveled, 1-based, seems to always be 1)
 
     each element, unnested
     """
     info = util.array_info(val)
     ndim, lengths = info[0], info[1:]
     if ndim == 0:
-        raise ValueError('{} is not an array type'.format(val))
+        raise ValueError("{} is not an array type".format(val))
     elems = list(util.array_iter(val))
-    fmt = ['>3i{}i'.format(2 * ndim)]
+    fmt = [">3i{}i".format(2 * ndim)]
     data = [ndim, None in elems, typelem] + [1] * ndim * 2
     data[3::2] = lengths
     for f, d in map(null_formatter(formatter), elems):
         fmt.append(f)
         data.extend(d)
-    return str_formatter(struct.pack(''.join(fmt), *data))
+    return str_formatter(struct.pack("".join(fmt), *data))
 
 
 def null(att, _, formatter):
     if not att.not_null:
         return null_formatter(formatter)
     message = 'null value in column "{}" not allowed'.format(att.attname)
+
     def nullcheck(v):
         if v is None:
             raise ValueError(message)
         return formatter(v)
+
     return nullcheck
 
 
 def array(att, _, formatter):
-    if att.type_category != 'A':
+    if att.type_category != "A":
         return formatter
     return lambda v: array_formatter(att.typelem, formatter, v)
 
 
 def maxsize(att, _, formatter):
-    if att.type_name not in ('varchar', 'bpchar'):
+    if att.type_name not in ("varchar", "bpchar"):
         return formatter
+
     def _maxsize(v):
         # postgres reports size + 4
         size = min(len(v), att.type_mod - 4) if att.type_mod >= 0 else len(v)
         return formatter(v[:size])
+
     return _maxsize
 
 
 def encode(att, encoding, formatter):
-    is_text_type = att.type_name in ('varchar', 'text', 'json')
-    is_enum_type = att.type_category == 'E'
+    is_text_type = att.type_name in ("varchar", "text", "json")
+    is_enum_type = att.type_category == "E"
     if not (is_text_type or is_enum_type):
         return formatter
+
     def _encode(v):
         try:
             encf = v.encode
         except AttributeError:
             return formatter(v)
         else:
             return formatter(encf(encoding))
+
     return _encode
 
+
 def diagnostic(att, encoding, formatter):
-    template = 'error formatting value {} for column {}'
+    template = "error formatting value {} for column {}"
+
     def f(v):
         try:
             return formatter(v)
         except Exception as exc:
             message = template.format(v, att.attname)
             errors.raise_from(ValueError, message, exc)
-    return f
-
 
-def get_formatter(att):
-    if att.type_category == 'E':
-        return str_formatter
-    try:
-        return type_formatters[att.type_name]
-    except KeyError:
-        raise TypeError('type {} is not supported'.format(att.type_name))
+    return f
 
 
 class CopyManager(object):
     """
     Facility for bulk-loading data using binary copy.
 
     Inspects the database on instantiation for the column types.
@@ -236,18 +242,25 @@
     :type table: str
 
     :param cols: columns in the table into which to copy data
     :type cols: list of str
 
     :raises ValueError: if the table or columns do not exist.
     """
+
+    type_formatters = {}
+
     def __init__(self, conn, table, cols):
+        self._type_formatters = {
+            **type_formatters,
+            **self.type_formatters,
+        }
         self.conn = conn
-        if '.' in table:
-            self.schema, self.table = table.split('.', 1)
+        if "." in table:
+            self.schema, self.table = table.split(".", 1)
         else:
             self.schema, self.table = util.get_schema(conn, table), table
         self.cols = cols
         self.compile()
 
     def compile(self):
         self.formatters = []
@@ -256,17 +269,25 @@
         for column in self.cols:
             att = type_dict.get(column)
             if att is None:
                 message = '"%s" is not a column of table "%s"."%s"'
                 raise ValueError(message % (column, self.schema, self.table))
             funcs = [encode, maxsize, array, diagnostic, null]
             reducer = lambda f, mf: mf(att, encoding, f)
-            f = functools.reduce(reducer, funcs, get_formatter(att))
+            f = functools.reduce(reducer, funcs, self.get_formatter(att))
             self.formatters.append(f)
 
+    def get_formatter(self, att):
+        if att.type_category == "E":
+            return str_formatter
+        try:
+            return self._type_formatters[att.type_name]
+        except KeyError:
+            raise TypeError("type {} is not supported".format(att.type_name))
+
     def copy(self, data, fobject_factory=tempfile.TemporaryFile):
         """
         Copy data into the database using a temporary file.
 
         :param data: the data to be inserted
         :type data: iterable of iterables
 
@@ -300,33 +321,33 @@
         """
         Copy data, serializing directly to the database.
 
         :param data: the data to be inserted
         :type data: iterable of iterables
         """
         r_fd, w_fd = os.pipe()
-        rstream = os.fdopen(r_fd, 'rb')
-        wstream = os.fdopen(w_fd, 'wb')
-        copy_thread = threading.Thread(target=self.copystream, args=(rstream,))
+        rstream = os.fdopen(r_fd, "rb")
+        wstream = os.fdopen(w_fd, "wb")
+        copy_thread = RaisingThread(target=self.copystream, args=(rstream,))
         copy_thread.start()
         self.writestream(data, wstream)
         wstream.close()
         copy_thread.join()
 
     def writestream(self, data, datastream):
         datastream.write(BINCOPY_HEADER)
         count = len(self.cols)
         for record in data:
-            fmt = ['>h']
+            fmt = [">h"]
             rdat = [count]
             for formatter, val in zip(self.formatters, record):
                 f, d = formatter(val)
                 fmt.append(f)
                 rdat.extend(d)
-            datastream.write(struct.pack(''.join(fmt), *rdat))
+            datastream.write(struct.pack("".join(fmt), *rdat))
         datastream.write(BINCOPY_TRAILER)
 
     def copystream(self, datastream):
         columns = '", "'.join(self.cols)
         cmd = 'COPY "{0}"."{1}" ("{2}") FROM STDIN WITH BINARY'
         sql = cmd.format(self.schema, self.table, columns)
         cursor = self.conn.cursor()
```

### Comparing `pgcopy-1.5.0/pgcopy/inspect.py` & `pgcopy-1.6.0/pgcopy/inspect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from psycopg2.extras import NamedTupleCursor
 
+
 def get_types(conn, schema, table):
     # for arrays:
     # typname has '_' prefix
     # attndims > 0
     # typcategory is 'A'
     # typelem is typid of individual elem (otherwise zero)
     query = """
@@ -20,9 +21,9 @@
                     JOIN pg_catalog.pg_type t ON a.atttypid = t.oid
                     LEFT JOIN pg_catalog.pg_type et ON t.typelem = et.oid
                     LEFT JOIN pg_catalog.pg_namespace n ON n.oid = c.relnamespace
             WHERE n.nspname = %s and relname = %s and attnum > 0
             ORDER BY c.relname, a.attnum;
             """
     cursor = conn.cursor(cursor_factory=NamedTupleCursor)
-    cursor.execute(query, (schema, table,))
+    cursor.execute(query, (schema, table))
     return {r.attname: r for r in cursor}
```

### Comparing `pgcopy-1.5.0/pgcopy/util.py` & `pgcopy-1.6.0/pgcopy/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,80 +1,93 @@
-import re
 import random
+import re
 import string
 from datetime import datetime, time
+
+from psycopg2 import sql
 from pytz import UTC
 
+
 def array_info(arr):
     """
     returns ndims, *lengths
     """
     if not isinstance(arr, (list, tuple, set)):
-        return 0,
+        return (0,)
     subs = set([array_info(elem) for elem in arr])
     if len(subs) > 1:
-        raise ValueError('subarray dimensions must match')
+        raise ValueError("subarray dimensions must match")
     if len(subs) == 0:
         return 1, 0
     s = subs.pop()
     dim, lengths = s[0], s[1:]
     return (dim + 1, len(arr)) + lengths
 
+
 def array_iter(arr):
     for i in arr:
         if isinstance(i, (list, tuple, set)):
             for x in array_iter(i):
                 yield x
         else:
             yield i
 
+
 def get_schema(conn, table):
     cur = conn.cursor()
+    quoted_table = sql.Identifier(table).as_string(cur)
     query = """
         SELECT n.nspname, c.relname
         FROM pg_catalog.pg_class c
         JOIN pg_catalog.pg_namespace n ON n.oid = c.relnamespace
         WHERE c.oid = %s::regclass
         """
-    cur.execute(query, (table,))
+    cur.execute(query, (quoted_table,))
     return cur.fetchone()[0]
 
+
 def to_utc(dt):
     if not isinstance(dt, datetime):
         dt = datetime(dt.year, dt.month, dt.day)
     if dt.tzinfo is None:
         return UTC.localize(dt)
     else:
         return dt.astimezone(UTC)
 
+
 def to_utc_time(t):
     if not isinstance(t, time):
         t = time(t.hour, t.minute, t.second, t.microsecond)
-    
+
     return UTC.localize(t)
 
+
 source = string.ascii_lowercase + string.digits
+
+
 def uid():
     vals = [random.choice(source) for i in range(5)]
-    return ''.join(vals)
+    return "".join(vals)
 
 
-idre = lambda name: re.compile(r'\b%s\b' % re.escape(name))
+idre = lambda name: re.compile(r"\b%s\b" % re.escape(name))
+
 
 class Replace(object):
     """
     Context manager for fast updates on table involving most rows in the table.
     Instead of `executemany("UPDATE ...")`, create and populate
     a new table (which can be done using COPY), then rename.
     This is possible only if no other tables in the db depend on the table.
 
     :param connection: database connection
     :type connection: psycopg2 connection
 
-    :param table: the table name.  Schema may be specified using dot notation: ``schema.table``.
+    :param table: the table name.  Schema may be specified using dot
+        notation: ``schema.table``.  Mixed-case names are not supported.
     :type table: str
 
     On entry, it creates a new table like the original, with a
     temporary name.  Default column values are included.
 
     On exit, it recreates the constraints, indices, triggers, and views on
     the new table, then replaces the old table with the new::
@@ -88,24 +101,25 @@
     Names of foreign key and check constraints will be mangled.
 
     .. note:: on PostgreSQL 9.1 and earlier, concurrent queries on the table
         `will fail`_ once the table is dropped.
 
     .. _will fail: https://gist.github.com/altaurog/ab0019837719d2a93e6b
     """
+
     def __init__(self, connection, table):
         self.cursor = connection.cursor()
         self.uid = uid()
-        if '.' in table:
-            self.schema, self.table = table.rsplit('.', 1)
+        if "." in table:
+            self.schema, self.table = table.rsplit(".", 1)
         else:
             self.schema, self.table = get_schema(connection, table), table
         self.name_re = idre(self.table)
         self.temp_name = self.newname()
-        self.rename = [('TABLE', self.nameformat(self.temp_name), self.table)]
+        self.rename = [("TABLE", self.nameformat(self.temp_name), self.table)]
         self.inspect()
 
     def __enter__(self):
         self.create_temp()
         self.create_defaults()
         return self.temp_name
 
@@ -144,15 +158,15 @@
             SELECT attname
             FROM pg_catalog.pg_attribute
             WHERE attrelid = %s::regclass
             AND attnum > 0 AND attnotnull
             """
         self.cursor.execute(attquery, (self.nameformat(self.table),))
         self.notnull = [an for (an,) in self.cursor]
-        # primary key is recreated as a constraint, 
+        # primary key is recreated as a constraint,
         # but all other unique constraints are only
         # recreated as unique index
         conquery = """
             SELECT DISTINCT contype, conname, pg_catalog.pg_get_constraintdef(oid)
             FROM pg_catalog.pg_constraint
             WHERE conrelid = %s::regclass AND contype != 'u'
             """
@@ -183,112 +197,116 @@
             JOIN pg_catalog.pg_namespace n ON n.oid = c.relnamespace
             WHERE d.refobjid = %s::regclass;
             """
         self.cursor.execute(viewquery, (self.nameformat(self.table),))
         self.views = self.cursor.fetchall()
 
     def create_temp(self):
-        create = 'CREATE TABLE {} AS TABLE {} WITH NO DATA'
-        self.cursor.execute(create.format(
-            self.nameformat(self.temp_name),
-            self.nameformat(self.table)
-        ))
+        create = "CREATE TABLE {} AS TABLE {} WITH NO DATA"
+        self.cursor.execute(
+            create.format(
+                self.nameformat(self.temp_name),
+                self.nameformat(self.table),
+            )
+        )
 
     def create_defaults(self):
         defsql = 'ALTER TABLE {} ALTER COLUMN "{}" SET DEFAULT {}'
         for col, default in self.defaults:
-            self.cursor.execute(defsql.format(
-                self.nameformat(self.temp_name), col, default
-            ))
+            self.cursor.execute(
+                defsql.format(self.nameformat(self.temp_name), col, default)
+            )
 
     def create_notnull(self):
         nnsql = 'ALTER TABLE {} ALTER COLUMN "{}" SET NOT NULL'
         for col in self.notnull:
             self.cursor.execute(nnsql.format(self.nameformat(self.temp_name), col))
 
     def create_constraints(self):
         consql = 'ALTER TABLE {} ADD CONSTRAINT "{}" {}'
         for i, (contype, conname, condef) in enumerate(self.constraints):
-            newname = self.newname('con', i)
-            self.cursor.execute(consql.format(
-                self.nameformat(self.temp_name), newname, condef
-            ))
-            if 'p' == contype:
-                self.rename.append(('INDEX', self.nameformat(newname), conname))
+            newname = self.newname("con", i)
+            self.cursor.execute(
+                consql.format(self.nameformat(self.temp_name), newname, condef)
+            )
+            if "p" == contype:
+                self.rename.append(("INDEX", self.nameformat(newname), conname))
 
     def create_indices(self):
         for i, (oldidxname, indexsql) in enumerate(self.indices):
-            newidxname = self.newname('idx', i)
+            newidxname = self.newname("idx", i)
             newsql = self.sqlrename(indexsql, oldidxname, newidxname)
             self.cursor.execute(newsql)
-            self.rename.append(('INDEX', self.nameformat(newidxname), oldidxname))
+            self.rename.append(("INDEX", self.nameformat(newidxname), oldidxname))
 
     def create_triggers(self):
         for i, (oldtrigname, trigsql) in enumerate(self.triggers):
-            newtrigname = self.newname('tg', i)
+            newtrigname = self.newname("tg", i)
             newsql = self.sqlrename(trigsql, oldtrigname, newtrigname)
             self.cursor.execute(newsql)
-            self.rename.append((
-                'TRIGGER',
-                '%s ON %s' % (newtrigname, self.nameformat(self.table)),
-                oldtrigname,
-            ))
+            self.rename.append(
+                (
+                    "TRIGGER",
+                    "%s ON %s" % (newtrigname, self.nameformat(self.table)),
+                    oldtrigname,
+                )
+            )
 
     def swap(self):
         self.drop_views()
         self.drop_defaults()
         self.move_sequences()
         self.drop_original_table()
         self.rename_temp_table()
 
     def drop_views(self):
         for schema, viewname, viewdef in self.views:
-            sql = 'DROP VIEW {}'.format(self.nameformat(viewname, schema))
+            sql = "DROP VIEW {}".format(self.nameformat(viewname, schema))
             self.cursor.execute(sql)
 
     def drop_defaults(self):
         dropdefsql = 'ALTER TABLE {} ALTER COLUMN "{}" DROP DEFAULT'
         for col, default in self.defaults:
             self.cursor.execute(dropdefsql.format(self.nameformat(self.table), col))
 
     def move_sequences(self):
         seqownersql = 'ALTER SEQUENCE "{}" OWNED BY {}."{}"'
         for col, seq in self.sequences:
-            self.cursor.execute(seqownersql.format(
-                seq, self.nameformat(self.temp_name), col
-            ))
+            self.cursor.execute(
+                seqownersql.format(seq, self.nameformat(self.temp_name), col)
+            )
 
     def drop_original_table(self):
-        self.cursor.execute('DROP TABLE {}'.format(self.nameformat(self.table)))
+        self.cursor.execute("DROP TABLE {}".format(self.nameformat(self.table)))
 
     def rename_temp_table(self):
-        template = 'ALTER {} {} RENAME TO {}'
+        template = "ALTER {} {} RENAME TO {}"
         for obj_type, oldname, newname in self.rename:
             self.cursor.execute(template.format(obj_type, oldname, newname))
 
     def create_views(self):
-        viewsql = 'CREATE VIEW {} AS {}'
+        viewsql = "CREATE VIEW {} AS {}"
         for schema, viewname, viewdef in self.views:
             sql = viewsql.format(self.nameformat(viewname, schema), viewdef)
             self.cursor.execute(sql)
 
+    unsafe_re = re.compile(r"\W+")
 
-    unsafe_re = re.compile(r'\W+')
     def newname(self, pre=None, i=None):
-        parts = ['%s']
+        parts = ["%s"]
         vals = [self.table]
         if pre is not None:
-            parts.append('%s')
+            parts.append("%s")
             vals.append(pre)
         if i is not None:
-            parts.append('%02d')
+            parts.append("%02d")
             vals.append(i)
-        parts.append('%s')
+        parts.append("%s")
         vals.append(self.uid)
-        return self.unsafe_re.sub('', '_'.join(parts) % tuple(vals)).lower()
+        return self.unsafe_re.sub("", "_".join(parts) % tuple(vals)).lower()
 
     def sqlrename(self, sql, *args):
         newsql = self.name_re.sub(self.temp_name, sql)
         try:
             old, new = args
         except ValueError:
             return newsql
@@ -317,14 +335,15 @@
         from pgcopy import CopyManager
         from pgcopy.util import RenameReplace
         xform = lambda s: s + '_old'
         with RenameReplace(conn, 'mytable', xform) as temp_name:
             mgr = CopyManager(conn, temp_name, cols)
             mgr.copy(records)
     """
+
     def __init__(self, connection, table, xform):
         """
         xform must be a function which translates old
         names to new ones, used on tables & pk constraints
         """
         super(RenameReplace, self).__init__(connection, table)
         self.xform = xform
```

### Comparing `pgcopy-1.5.0/setup.py` & `pgcopy-1.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,54 @@
-from os.path import join, dirname
+from os.path import dirname, join
+
 from setuptools import setup
 
 package_name = "pgcopy"
 base_dir = dirname(__file__)
 
+
 def read(filename):
     f = open(join(base_dir, filename))
     return f.read()
 
-def get_version(package_name, default='0.1'):
+
+def get_version(package_name, default="0.1"):
     try:
-        f = open(join(base_dir, package_name, 'version.py'))
+        f = open(join(base_dir, package_name, "version.py"))
     except IOError:
         try:
-            f = open(join(base_dir, package_name + '.py'))
+            f = open(join(base_dir, package_name + ".py"))
         except IOError:
             return default
     for line in f:
         parts = line.split()
-        if parts[:2] == ['__version__', '=']:
+        if parts[:2] == ["__version__", "="]:
             return parts[2].strip("'\"")
     return default
 
+
 setup(
-    name = package_name,
-    version = get_version(package_name),
-    description = "Fast db insert with postgresql binary copy",
-    long_description = read("README.rst"),
-    long_description_content_type = 'text/x-rst',
-    author = "Aryeh Leib Taurog",
-    author_email = "python@aryehleib.com",
-    license = 'MIT',
-    url = "https://pgcopy.readthedocs.io/en/latest/",
-    packages = ['pgcopy', 'pgcopy.errors'],
-    install_requires = ["psycopg2", "pytz"],
-    classifiers = [
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
+    name=package_name,
+    version=get_version(package_name),
+    description="Fast db insert with postgresql binary copy",
+    long_description=read("README.rst"),
+    long_description_content_type="text/x-rst",
+    author="Aryeh Leib Taurog",
+    author_email="python@aryehleib.com",
+    license="MIT",
+    url="https://pgcopy.readthedocs.io/en/latest/",
+    packages=["pgcopy", "pgcopy.errors", "pgcopy.contrib"],
+    install_requires=["psycopg2", "pytz"],
+    classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Topic :: Database",
     ],
 )
```

