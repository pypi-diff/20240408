# Comparing `tmp/nophp-0.1.8rc1.tar.gz` & `tmp/nophp-0.1.8rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nophp-0.1.8rc1.tar", max compression
+gzip compressed data, was "nophp-0.1.8rc2.tar", max compression
```

## Comparing `nophp-0.1.8rc1.tar` & `nophp-0.1.8rc2.tar`

### file list

```diff
@@ -1,54 +1,56 @@
--rw-r--r--   0        0        0     1891 2024-01-20 18:08:38.831834 nophp-0.1.8rc1/LICENSE
--rw-r--r--   0        0        0       28 2023-12-24 21:56:57.728726 nophp-0.1.8rc1/README.md
--rw-r--r--   0        0        0       40 2024-01-10 17:35:06.369895 nophp-0.1.8rc1/nophp/__main__.py
--rw-r--r--   0        0        0      478 2024-02-08 17:04:41.521723 nophp-0.1.8rc1/nophp/conv.py
--rw-r--r--   0        0        0        0 2024-01-06 14:18:53.957172 nophp-0.1.8rc1/nophp/lang/__init__.py
--rw-r--r--   0        0        0      146 2024-01-06 14:20:41.374844 nophp-0.1.8rc1/nophp/lang/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2462 2023-12-01 10:28:43.697648 nophp-0.1.8rc1/nophp/lang/__pycache__/compiler.cpython-310.pyc
--rw-r--r--   0        0        0    12416 2024-02-08 17:01:49.730048 nophp-0.1.8rc1/nophp/lang/__pycache__/compiler.cpython-312.pyc
--rw-r--r--   0        0        0     5819 2023-12-01 10:28:43.697648 nophp-0.1.8rc1/nophp/lang/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0    12429 2024-02-08 17:01:49.732048 nophp-0.1.8rc1/nophp/lang/__pycache__/exceptions.cpython-312.pyc
--rw-r--r--   0        0        0     2211 2023-12-01 10:28:43.698648 nophp-0.1.8rc1/nophp/lang/__pycache__/lexer.cpython-310.pyc
--rw-r--r--   0        0        0     3662 2024-01-07 00:41:38.526642 nophp-0.1.8rc1/nophp/lang/__pycache__/lexer.cpython-312.pyc
--rw-r--r--   0        0        0     7648 2024-02-08 17:01:49.746048 nophp-0.1.8rc1/nophp/lang/__pycache__/module.cpython-312.pyc
--rw-r--r--   0        0        0     5671 2023-12-01 10:28:43.698648 nophp-0.1.8rc1/nophp/lang/__pycache__/modules.cpython-310.pyc
--rw-r--r--   0        0        0    68418 2024-02-08 17:01:49.743048 nophp-0.1.8rc1/nophp/lang/__pycache__/modules.cpython-312.pyc
--rw-r--r--   0        0        0    24663 2023-12-01 10:28:43.698648 nophp-0.1.8rc1/nophp/lang/__pycache__/pparser.cpython-310.pyc
--rw-r--r--   0        0        0    52469 2024-02-08 17:01:49.808048 nophp-0.1.8rc1/nophp/lang/__pycache__/pparser.cpython-312.pyc
--rw-r--r--   0        0        0     2681 2023-12-01 10:28:43.698648 nophp-0.1.8rc1/nophp/lang/__pycache__/types.cpython-310.pyc
--rw-r--r--   0        0        0    12218 2024-02-08 17:01:49.750048 nophp-0.1.8rc1/nophp/lang/__pycache__/types.cpython-312.pyc
--rw-r--r--   0        0        0    11095 2024-02-26 21:10:01.859913 nophp-0.1.8rc1/nophp/lang/compiler.py
--rw-r--r--   0        0        0     4466 2024-01-20 18:46:14.559597 nophp-0.1.8rc1/nophp/lang/exceptions.py
--rw-r--r--   0        0        0     3336 2024-01-07 00:33:14.504709 nophp-0.1.8rc1/nophp/lang/lexer.py
--rw-r--r--   0        0        0     5941 2024-01-21 18:49:16.880115 nophp-0.1.8rc1/nophp/lang/module.py
--rw-r--r--   0        0        0    58244 2024-01-21 18:38:12.162696 nophp-0.1.8rc1/nophp/lang/modules.py
--rw-r--r--   0        0        0    38456 2024-01-20 14:58:44.976419 nophp-0.1.8rc1/nophp/lang/pparser.py
--rw-r--r--   0        0        0     4539 2024-01-11 23:49:02.244973 nophp-0.1.8rc1/nophp/lang/std/__pycache__/bcrypt.cpython-312.pyc
--rw-r--r--   0        0        0    10796 2024-01-11 23:49:02.242973 nophp-0.1.8rc1/nophp/lang/std/__pycache__/db.cpython-312.pyc
--rw-r--r--   0        0        0     1610 2024-02-08 17:03:44.168002 nophp-0.1.8rc1/nophp/lang/std/__pycache__/echo.cpython-312.pyc
--rw-r--r--   0        0        0     2500 2024-02-08 17:01:51.709040 nophp-0.1.8rc1/nophp/lang/std/__pycache__/htmlspecialchars.cpython-312.pyc
--rw-r--r--   0        0        0     2571 2024-01-19 23:30:27.264397 nophp-0.1.8rc1/nophp/lang/std/__pycache__/internal.cpython-312.pyc
--rw-r--r--   0        0        0     3348 2024-01-12 13:13:45.606975 nophp-0.1.8rc1/nophp/lang/std/__pycache__/json.cpython-312.pyc
--rw-r--r--   0        0        0     4034 2024-01-11 23:49:02.240973 nophp-0.1.8rc1/nophp/lang/std/__pycache__/primitives.cpython-312.pyc
--rw-r--r--   0        0        0     2677 2024-01-06 14:27:48.837511 nophp-0.1.8rc1/nophp/lang/std/__pycache__/rand.cpython-312.pyc
--rw-r--r--   0        0        0     2490 2024-01-12 12:09:57.634466 nophp-0.1.8rc1/nophp/lang/std/__pycache__/redirect.cpython-312.pyc
--rw-r--r--   0        0        0     5415 2024-01-06 14:27:48.852177 nophp-0.1.8rc1/nophp/lang/std/__pycache__/session.cpython-312.pyc
--rw-r--r--   0        0        0     4444 2023-12-27 22:15:06.862482 nophp-0.1.8rc1/nophp/lang/std/__pycache__/str.cpython-312.pyc
--rw-r--r--   0        0        0     5459 2024-01-11 23:49:02.238973 nophp-0.1.8rc1/nophp/lang/std/__pycache__/string.cpython-312.pyc
--rw-r--r--   0        0        0     2802 2024-01-11 00:48:29.049313 nophp-0.1.8rc1/nophp/lang/std/bcrypt.py
--rw-r--r--   0        0        0     7713 2024-02-26 21:19:58.215714 nophp-0.1.8rc1/nophp/lang/std/db.py
--rw-r--r--   0        0        0      883 2024-01-20 13:45:03.471515 nophp-0.1.8rc1/nophp/lang/std/echo.py
--rw-r--r--   0        0        0     1572 2024-01-21 22:13:36.764069 nophp-0.1.8rc1/nophp/lang/std/htmlspecialchars.py
--rw-r--r--   0        0        0     1929 2024-03-02 17:43:14.270386 nophp-0.1.8rc1/nophp/lang/std/internal.py
--rw-r--r--   0        0        0     2552 2024-01-20 13:39:45.447928 nophp-0.1.8rc1/nophp/lang/std/json.py
--rw-r--r--   0        0        0     2790 2024-01-20 18:36:05.123255 nophp-0.1.8rc1/nophp/lang/std/primitives.py
--rw-r--r--   0        0        0     1805 2024-01-06 14:26:59.763266 nophp-0.1.8rc1/nophp/lang/std/rand.py
--rw-r--r--   0        0        0     1656 2024-01-12 00:10:46.691653 nophp-0.1.8rc1/nophp/lang/std/redirect.py
--rw-r--r--   0        0        0     4018 2024-01-06 14:27:07.735447 nophp-0.1.8rc1/nophp/lang/std/session.py
--rw-r--r--   0        0        0     3783 2024-01-10 17:52:32.696445 nophp-0.1.8rc1/nophp/lang/std/string.py
--rw-r--r--   0        0        0     6667 2024-02-26 21:19:47.786774 nophp-0.1.8rc1/nophp/lang/types.py
--rw-r--r--   0        0        0     9594 2024-02-27 11:07:26.512946 nophp-0.1.8rc1/nophp/spindle.py
--rw-r--r--   0        0        0      349 2023-12-20 13:20:18.231075 nophp-0.1.8rc1/nophp/splitter.py
--rw-r--r--   0        0        0     5918 2024-02-08 17:04:56.517620 nophp-0.1.8rc1/nophp/weaver.py
--rw-r--r--   0        0        0      487 2024-03-02 17:43:43.721092 nophp-0.1.8rc1/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 nophp-0.1.8rc1/PKG-INFO
+-rw-r--r--   0        0        0     1530 2024-03-24 19:42:33.635558 nophp-0.1.8rc2/LICENSE
+-rw-r--r--   0        0        0     3474 2024-03-23 09:01:53.656269 nophp-0.1.8rc2/README.md
+-rw-r--r--   0        0        0       40 2024-01-10 17:35:06.369895 nophp-0.1.8rc2/nophp/__main__.py
+-rw-r--r--   0        0        0      478 2024-02-08 17:04:41.521723 nophp-0.1.8rc2/nophp/conv.py
+-rw-r--r--   0        0        0        0 2024-01-06 14:18:53.957172 nophp-0.1.8rc2/nophp/lang/__init__.py
+-rw-r--r--   0        0        0      146 2024-01-06 14:20:41.374844 nophp-0.1.8rc2/nophp/lang/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     2462 2023-12-01 10:28:43.697648 nophp-0.1.8rc2/nophp/lang/__pycache__/compiler.cpython-310.pyc
+-rw-r--r--   0        0        0    12416 2024-02-08 17:01:49.730048 nophp-0.1.8rc2/nophp/lang/__pycache__/compiler.cpython-312.pyc
+-rw-r--r--   0        0        0     5819 2023-12-01 10:28:43.697648 nophp-0.1.8rc2/nophp/lang/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0    12429 2024-02-08 17:01:49.732048 nophp-0.1.8rc2/nophp/lang/__pycache__/exceptions.cpython-312.pyc
+-rw-r--r--   0        0        0     2211 2023-12-01 10:28:43.698648 nophp-0.1.8rc2/nophp/lang/__pycache__/lexer.cpython-310.pyc
+-rw-r--r--   0        0        0     3662 2024-01-07 00:41:38.526642 nophp-0.1.8rc2/nophp/lang/__pycache__/lexer.cpython-312.pyc
+-rw-r--r--   0        0        0     7648 2024-02-08 17:01:49.746048 nophp-0.1.8rc2/nophp/lang/__pycache__/module.cpython-312.pyc
+-rw-r--r--   0        0        0     5671 2023-12-01 10:28:43.698648 nophp-0.1.8rc2/nophp/lang/__pycache__/modules.cpython-310.pyc
+-rw-r--r--   0        0        0    68418 2024-02-08 17:01:49.743048 nophp-0.1.8rc2/nophp/lang/__pycache__/modules.cpython-312.pyc
+-rw-r--r--   0        0        0    24663 2023-12-01 10:28:43.698648 nophp-0.1.8rc2/nophp/lang/__pycache__/pparser.cpython-310.pyc
+-rw-r--r--   0        0        0    52469 2024-02-08 17:01:49.808048 nophp-0.1.8rc2/nophp/lang/__pycache__/pparser.cpython-312.pyc
+-rw-r--r--   0        0        0     2681 2023-12-01 10:28:43.698648 nophp-0.1.8rc2/nophp/lang/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0        0        0    12218 2024-02-08 17:01:49.750048 nophp-0.1.8rc2/nophp/lang/__pycache__/types.cpython-312.pyc
+-rw-r--r--   0        0        0    11191 2024-03-23 09:46:32.721583 nophp-0.1.8rc2/nophp/lang/compiler.py
+-rw-r--r--   0        0        0     4466 2024-01-20 18:46:14.559597 nophp-0.1.8rc2/nophp/lang/exceptions.py
+-rw-r--r--   0        0        0     3336 2024-01-07 00:33:14.504709 nophp-0.1.8rc2/nophp/lang/lexer.py
+-rw-r--r--   0        0        0     5524 2024-04-03 16:53:03.510447 nophp-0.1.8rc2/nophp/lang/module.py
+-rw-r--r--   0        0        0    63939 2024-04-05 20:41:14.789970 nophp-0.1.8rc2/nophp/lang/modules.py
+-rw-r--r--   0        0        0    39003 2024-03-31 20:12:18.047800 nophp-0.1.8rc2/nophp/lang/pparser.py
+-rw-r--r--   0        0        0     4539 2024-01-11 23:49:02.244973 nophp-0.1.8rc2/nophp/lang/std/__pycache__/bcrypt.cpython-312.pyc
+-rw-r--r--   0        0        0    10796 2024-01-11 23:49:02.242973 nophp-0.1.8rc2/nophp/lang/std/__pycache__/db.cpython-312.pyc
+-rw-r--r--   0        0        0     1610 2024-02-08 17:03:44.168002 nophp-0.1.8rc2/nophp/lang/std/__pycache__/echo.cpython-312.pyc
+-rw-r--r--   0        0        0     2500 2024-02-08 17:01:51.709040 nophp-0.1.8rc2/nophp/lang/std/__pycache__/htmlspecialchars.cpython-312.pyc
+-rw-r--r--   0        0        0     2571 2024-01-19 23:30:27.264397 nophp-0.1.8rc2/nophp/lang/std/__pycache__/internal.cpython-312.pyc
+-rw-r--r--   0        0        0     3348 2024-01-12 13:13:45.606975 nophp-0.1.8rc2/nophp/lang/std/__pycache__/json.cpython-312.pyc
+-rw-r--r--   0        0        0     4034 2024-01-11 23:49:02.240973 nophp-0.1.8rc2/nophp/lang/std/__pycache__/primitives.cpython-312.pyc
+-rw-r--r--   0        0        0     2677 2024-01-06 14:27:48.837511 nophp-0.1.8rc2/nophp/lang/std/__pycache__/rand.cpython-312.pyc
+-rw-r--r--   0        0        0     2490 2024-01-12 12:09:57.634466 nophp-0.1.8rc2/nophp/lang/std/__pycache__/redirect.cpython-312.pyc
+-rw-r--r--   0        0        0     5415 2024-01-06 14:27:48.852177 nophp-0.1.8rc2/nophp/lang/std/__pycache__/session.cpython-312.pyc
+-rw-r--r--   0        0        0     4444 2023-12-27 22:15:06.862482 nophp-0.1.8rc2/nophp/lang/std/__pycache__/str.cpython-312.pyc
+-rw-r--r--   0        0        0     5459 2024-01-11 23:49:02.238973 nophp-0.1.8rc2/nophp/lang/std/__pycache__/string.cpython-312.pyc
+-rw-r--r--   0        0        0     2802 2024-01-11 00:48:29.049313 nophp-0.1.8rc2/nophp/lang/std/bcrypt.py
+-rw-r--r--   0        0        0     7780 2024-03-28 15:04:36.548750 nophp-0.1.8rc2/nophp/lang/std/db.py
+-rw-r--r--   0        0        0      883 2024-03-25 10:27:13.934559 nophp-0.1.8rc2/nophp/lang/std/echo.py
+-rw-r--r--   0        0        0     3055 2024-03-20 11:38:41.520416 nophp-0.1.8rc2/nophp/lang/std/htmlspecialchars.py
+-rw-r--r--   0        0        0     2784 2024-04-05 19:32:28.917381 nophp-0.1.8rc2/nophp/lang/std/internal.py
+-rw-r--r--   0        0        0     2552 2024-01-20 13:39:45.447928 nophp-0.1.8rc2/nophp/lang/std/json.py
+-rw-r--r--   0        0        0     1638 2024-04-03 12:52:18.612664 nophp-0.1.8rc2/nophp/lang/std/memory.py
+-rw-r--r--   0        0        0     3824 2024-04-07 10:58:39.790142 nophp-0.1.8rc2/nophp/lang/std/primitives.py
+-rw-r--r--   0        0        0     1805 2024-01-06 14:26:59.763266 nophp-0.1.8rc2/nophp/lang/std/rand.py
+-rw-r--r--   0        0        0     1656 2024-01-12 00:10:46.691653 nophp-0.1.8rc2/nophp/lang/std/redirect.py
+-rw-r--r--   0        0        0     4102 2024-03-23 09:40:43.160037 nophp-0.1.8rc2/nophp/lang/std/session.py
+-rw-r--r--   0        0        0     4428 2024-03-28 12:49:47.742830 nophp-0.1.8rc2/nophp/lang/std/string.py
+-rw-r--r--   0        0        0     3586 2024-03-28 16:51:48.114101 nophp-0.1.8rc2/nophp/lang/std/stripe.py
+-rw-r--r--   0        0        0     6879 2024-03-31 20:20:55.247486 nophp-0.1.8rc2/nophp/lang/types.py
+-rw-r--r--   0        0        0     9889 2024-03-28 16:30:02.507510 nophp-0.1.8rc2/nophp/spindle.py
+-rw-r--r--   0        0        0      349 2023-12-20 13:20:18.231075 nophp-0.1.8rc2/nophp/splitter.py
+-rw-r--r--   0        0        0     5918 2024-02-08 17:04:56.517620 nophp-0.1.8rc2/nophp/weaver.py
+-rw-r--r--   0        0        0      505 2024-04-08 21:24:19.921665 nophp-0.1.8rc2/pyproject.toml
+-rw-r--r--   0        0        0     4123 1970-01-01 00:00:00.000000 nophp-0.1.8rc2/PKG-INFO
```

### Comparing `nophp-0.1.8rc1/LICENSE` & `nophp-0.1.8rc2/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-BSD 3-Clause License with Commercial Use Clause
+BSD 3-Clause License
 
 Copyright (c) 2023, ByteFor
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted for non-commercial purposes only, provided that
 the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions, and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice,
    this list of conditions, and the following disclaimer in the documentation
    and/or other materials provided with the distribution.
 
-3. Commercial use of this software, including but not limited to the creation of
-   commercial products or services, is expressly ALLOWED without the prior
-   written permission of the copyright holder. Any commercial products or services
-   must explicitly mention this copyright and the copyright holder when used in some
-   form.
-
-4. Neither the name of the copyright holder nor the names of its contributors may
+3. Neither the name of the copyright holder nor the names of its contributors may
    be used to endorse or promote products derived from this software without
    specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
 ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
```

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/compiler.cpython-310.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/compiler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/compiler.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/compiler.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/exceptions.cpython-310.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/exceptions.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/exceptions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/lexer.cpython-310.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/lexer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/lexer.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/lexer.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/module.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/module.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/modules.cpython-310.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/modules.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/modules.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/modules.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/pparser.cpython-310.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/pparser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/pparser.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/pparser.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/types.cpython-310.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/__pycache__/types.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/__pycache__/types.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/compiler.py` & `nophp-0.1.8rc2/nophp/lang/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,18 @@
         self.stop = False
 
         # Keep track of current and previous module run
         self.curr = None
         self.prev = None
 
         self.persistent = False
+        self._console = Console()
+
+    def log(self, *args):
+        self._console.print(*args)
 
     def new_instance(
         self,
         tree = None,
         namespace = '_anon',
         namespaces = {},
         variables = {},
```

### Comparing `nophp-0.1.8rc1/nophp/lang/exceptions.py` & `nophp-0.1.8rc2/nophp/lang/exceptions.py`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/lexer.py` & `nophp-0.1.8rc2/nophp/lang/lexer.py`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/module.py` & `nophp-0.1.8rc2/nophp/lang/module.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,68 +19,44 @@
     def __init__(
         self,
         #type: MODULE_TYPES
     ):
         self.type = "Unknown"
         self.built = ""
         self.template = ""
-        self.o1 = False
-        self.o2 = False
-        self.o3 = False
         self.no_construct = False        
 
     def __call__(
         self,
         tree,
         no_construct = False
     ):
 
         self.no_construct = no_construct
         _values = self.proc_tree(tree)
         self.override()
         return _values
     
-    # Future
-    #def optimise(self): pass
-    optimise = None
 
     def remove_quotes(_,s):
         if type(s) != str: return str(s)
         if len(s) >= 2 and s[0] == '"' and s[-1] == '"':
             return s.strip('"')
     
         return s
 
-    # Future: Return true for now
-    def verify(self): return True
-
     def override(self):
         """
         Warning: this should be used with caution since it bypasses the default build structure
         """
         pass
 
     # Implemented in module child
     def proc_tree(self, tree) -> dict: "Return a dict containing values processed from the tree"
 
-    # Format
-    # TODO: Remove this as it's not used
-    def _constructor(
-        self,
-        arguments: dict
-    ) -> BUILT_TYPE:
-        if arguments == None:
-            raise ModuleExceptions.InvalidModuleConstruction(self)
-        try:
-            return self.template.format(
-                    **arguments
-                )
-        except Exception:
-            raise Exception(f"In '{self.name}' - Failed to unpack elements. Perhaps you need to set `no_construct` to True to avoid this module's construction?")
-
     def base(self, tree, ref=False):
         values = []
 
         if 'FUNCTION_ARGUMENTS' not in tree:
             # Advanced handling
             for var in tree:
                 value = self.ref_resolve(var) if ref else self.safely_resolve(var)
@@ -114,14 +90,16 @@
             v = self.compiler_instance.get_variable(value)
             # print(v)
             value = self.safely_resolve(v['object'])
         elif type(resolved) == String:
             value = self.remove_quotes(resolved.value)
         elif type(resolved) == Int32:
             value = resolved.value
+        elif type(resolved) == Float:
+            value = resolved.value
         elif type(resolved) == Bool:
             value = resolved.value
         elif type(resolved) == sInnerMut:
             value = func_module.run_sInnerMut(resolved).value
         elif type(resolved) == type(self.compiler_instance):
             value = resolved
         elif type(resolved) == SqlConnector:
@@ -136,18 +114,23 @@
         elif type(resolved) == Map:
             _value = resolved.value
             value = {}
             for key in _value:
                 value[
                     self.safely_resolve(key)
                 ] = self.safely_resolve(_value[key])
+
+        elif type(resolved) == Session:
+            value = resolved.value
                 
         # Legacy
         # Markup safe breaks this a bit...
-        elif type(resolved) in [int, str, list, tuple, float, markupsafe.Markup]:
+        elif type(resolved) == markupsafe.Markup:
+            value = resolved.unescape()
+        elif type(resolved) in [int, str, list, tuple, dict, float, markupsafe.Markup]:
             value = resolved
         elif type(resolved) == Auto:
             value = resolved.value
         else:
             print(f"Couldnt resolve {resolved} of {type(resolved)} in Module, returning None")
 
         print(value)
@@ -174,14 +157,16 @@
                 value = String("")
             else:
                 value = v['object']
         elif type(resolved) == String:
             value = resolved
         elif type(resolved) == Int32:
             value = resolved
+        elif type(resolved) == Float:
+            value = resolved
         elif type(resolved) == sInnerMut:
             value = func_module.run_sInnerMut(resolved)
         elif type(resolved) == SqlConnector:
             value = resolved
         elif type(resolved) == DynArray:
             value = resolved
         else:
```

### Comparing `nophp-0.1.8rc1/nophp/lang/modules.py` & `nophp-0.1.8rc2/nophp/lang/modules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from copy import deepcopy
 import inspect
 import pprint
 import re
 
+import markupsafe
+
 from .exceptions import ModuleExceptions, TranspilerExceptions, RuntimeExceptions, Warn
 from .module import Module
 from nophp.splitter import split_php
 
 from .lexer import PyettyLexer
 from .pparser import PyettyParser
 from .types import *
@@ -39,66 +41,73 @@
         first, second = tree['0'], tree['1']
 
         supported_types = {
             ID,
             String,
             Int32,
             Bool,
+            Float,
             Auto,
             Nil
         }
 
         print(self.compiler_instance.namespace)
 
         first_resolved = resolution_module(first)
         second_resolved = resolution_module(second)
 
 
         # Todo: Legacy, remove as it's not used and may cause issues
-        if type(first_resolved) == str: first_resolved = String(first_resolved)
-        if type(second_resolved) == str: second_resolved = String(second_resolved)
+        if type(first_resolved) in BASE_TYPES: first_resolved = Auto(first_resolved, "basic").value
+        if type(second_resolved) in BASE_TYPES: second_resolved = Auto(second_resolved, "basic").value
 
         if type(first_resolved) not in supported_types or\
               type(second_resolved) not in supported_types:
             # Invalid type
             raise TranspilerExceptions.Generic(f"Not Implemented: {first_resolved} {second_resolved} Only supports: {supported_types}")
         
         first_value = ""
         if type(first_resolved) == ID:
             first_var: BasicType  = self.compiler_instance.get_variable(first_resolved.value)
 
-            if first_var["type"] not in [String, Int32, Bool, Auto, Nil]:
+            if first_var["type"] not in supported_types:
                 # Invalid type
                 raise TranspilerExceptions.Generic(f"Expected an ID() of String() type, got {first_var['type'].__name__}()")
             
             first_value = first_var["object"].value
         elif type(first_resolved) == String:
             first_value = first_resolved.value
-        elif type(first_resolved) ==  Int32:
+        elif type(first_resolved) == Int32 or type(first_resolved) == Float:
             first_value = f"\"{first_resolved.value}\""
         elif type(first_resolved) == Auto:
             first_value = first_resolved.value
 
 
         second_value = ""
         if type(second_resolved) == ID:
             second_var: BasicType  = self.compiler_instance.get_variable(second_resolved.value)
 
-            if second_var["type"] not in [String, Int32, Bool, Auto, Nil]:
+            if second_var["type"] not in supported_types:
                 # Invalid type
                 raise TranspilerExceptions.Generic(f"Expected an ID() of String() type, got {second_var['type'].__name__}()")
         
             second_value = second_var["object"].value
         elif type(second_resolved) == String:
             second_value = second_resolved.value
-        elif type(second_resolved) ==  Int32:
+        elif type(second_resolved) == Int32 or type(second_resolved) == Float:
             second_value = f"\"{second_resolved.value}\""
         elif type(second_resolved) == Auto:
             second_value = second_resolved.value
 
+        # TODO: Patch with exhaustive matching later
+        if second_value in NOPHP_TYPES:
+            second_value = second_value.value
+        if first_value in NOPHP_TYPES:
+            first_value = first_value.value
+
         return String(self.remove_quotes(first_value) + self.remove_quotes(second_value))
 
 class PhpMod(Module):
     name="PHP"
     type = Module.MODULE_TYPES.NON_WRITEABLE
 
     def __init__(self, compiler_instance):
@@ -138,15 +147,15 @@
                     # print("     attr:", attr)
                     self.host.attrs[attr[0]] = attr[1]
         
 
         self.parser = MyHTMLParser(self)
 
     def proc_tree(self, tree):
-        # pprint("[HTML] triggered simplified HTML build.")
+        # pprint("[HTML] triggered simplified HTML build.") No longer simple heh
 
         self.tag = ""
         self.attrs = {}
 
         if len(tree['PROGRAM']) == 0:
             value = ""
         elif tree['PROGRAM'][0] == 'HTML':
@@ -180,24 +189,25 @@
         start = tree['LABEL']['START'] if tree['LABEL']['START'] is not None else ""
         end = tree['LABEL']['END'] if tree['LABEL']['END'] is not None else ""
 
         # Test parse of the start
         self.tag = ""
         self.attrs = {}
         self.parser.feed(start)
-        # print(self.tag)
-        # print(self.attrs)
+        print(self.tag)
+        print(self.attrs)
         
         if self.attrs != {}:
             final = []
             # parse content of the attribute
             for attr in self.attrs:
                 if self.attrs[attr] is None:
                     raise TranspilerExceptions.Generic(f"Invalid HTML at tag {self.tag}")
                 if self.attrs[attr].startswith('$'):
+                    self.compiler_instance.log(attr)
                     code = f"echo {self.attrs[attr]}"
                     lexer = PyettyLexer()
                     parser = PyettyParser()
                     ast = parser.parse(lexer.tokenize(code))
 
                     instance = self.compiler_instance.new_instance(
                         tree=ast,
@@ -206,15 +216,15 @@
                     instance.run()
                     out = ''.join(instance.finished)
                     final.append(f"{attr}=\"{out}\"")
                 else:
                     final.append(f"{attr}=\"{self.attrs[attr]}\"")
             start = f"<{self.tag} {' '.join(final)}>"
 
-        # Todo: Legacy
+        # TODO: Legacy
         if type(value) == String:
             value = self.remove_quotes(value.value)
 
         return String(start + str(value) + end)
     
 class NamespaceMod(Module):
     name="NAMESPACE"
@@ -453,84 +463,135 @@
 
         # pprint(tree)
         line = tree['LINE']
         name = resolution_module(tree['EXPRESSION'])
         index = resolution_module(tree['INDEX'])
 
         # print(index)
-        # print(name)
+        print(name, type(name))
 
         if type(index) == String:
             index_value = self.remove_quotes(index.value)
         else: index_value = index.value
 
         if type(name) == ID:
             var = self.compiler_instance.get_variable(name.value)
             # print(var)
             if var['type'] == DynArray:
                 if 0 <= index_value < var['object'].length:
-                    return var['object'].value[index_value]
+                    return Auto(var['object'].value[index_value], "basic").value
                 else:
                     print(var['object'])
+                    print(f"DynArray does not contain {index_value}, it only contains: {list(var['object'].value)}")
                     raise TranspilerExceptions.OutOfBounds(index_value, var['object'].length)
             # DONE: Session and Request types need to be compatible with printing out in echo
             elif var['type'] == Session:
-                if index_value in var['object'].value:
+                # Rebuild
+                value = {}
+                for key, v in var['object'].value.items():
+                    if type(key) not in BASE_TYPES:
+                        value[self.remove_quotes(key.value) if type(key.value) == str else key.value] = v
+                    else:
+                        value[self.remove_quotes(key)] = v
+                if index_value in value:
                     # print("Session contains:",var['object'].value[index_value], type(var['object'].value[index_value]), var['object'].value)
-                    return Auto(var['object'].value[index_value], "basic")
+                    return Auto(value[index_value], "basic")
                 else:
-                    # print(f"Session does not contain {index_value}, it only contains: {list(var['object'].value.keys())}")
+                    print(f"Session does not contain {index_value}, it only contains: {list(value.keys())}")
                     return Nil()
             elif var['type'] == Request:
                 if index_value.lower() in var['object'].value.__dir__():
                     # print("Request contains:", getattr(var['object'].value, index_value.lower()), index_value.lower(), list(var['object'].value.__dir__()))
                     return Auto(getattr(var['object'].value, index_value.lower()), type="basic")
                 else:
                     # print("Request contains:",list(var['object'].value.__dir__()))
                     return Nil()
             elif var['type'] == Map:
-                if index_value in var['object'].value:
+                value = {}
+                for key, v in var['object'].value.items():
+                    if type(key) not in BASE_TYPES:
+                        value[self.remove_quotes(key.value) if type(key.value) == str else key.value] = v
+                    else:
+                        value[self.remove_quotes(key)] = v
+                if index_value in value:
                     print("Found mapping")
-                    return Auto(var['object'].value[index_value], "basic")
+                    return Auto(value[index_value], "basic")
                 else:
+                    print(f"Map does not contain {index_value}, it only contains: {list(value.keys())}")
                     return Nil()
             else:
                 raise TranspilerExceptions.TypeMissmatch("Get ID Index Actor", var['type'], [ID, DynArray, Session, Request], line)
         elif type(name) == DynArray:
             if 0 <= index_value < name.length:
                 return Auto(name.value[index_value], "basic")
             else:
                 raise TranspilerExceptions.OutOfBounds(index_value, name.length)
             # raise TranspilerExceptions.Generic(f"{name.value}")
         elif type(name) == Auto:
             # This is dumb but assume we got passed some internal object right?
+            if type(name.value) == markupsafe.Markup:
+                if str(name.value) != "":
+                    def add_quotes_if_missing(match):
+                        content = match.group(1)  # The content within the parentheses
+                        # Check if the content is already wrapped in double quotes
+                        if not (content.startswith('"') and content.endswith('"')) and not (content.startswith("'") and content.endswith("'")):
+                            return f'String("{content}")'  # Add quotes if they're missing
+                        else:
+                            return f'String({content})'  # Keep as is if quotes are present
+                    v = str(name.value)
+                    v = re.sub(r'String\(([^)]+)\)', add_quotes_if_missing, v)
+                    print(v)
+                    try:
+                        name.value = eval(str(v)) # TODO: Oh god forgive me   
+                    except NameError as e:
+                        raise TranspilerExceptions.Generic(f"Failed to convert Markupsafe to a valid entity: {name.value}\nError: {e}")
+                else:
+                    return Nil()
             from werkzeug.datastructures import ImmutableMultiDict
             if type(name.value) == ImmutableMultiDict:
                 if index_value in name.value.to_dict():
                     return Auto(name.value.to_dict()[index_value], "basic")
                 else:
+                    print(f"ImmutableMultiDict does not contain {index_value}, it only contains: {list(name.value.to_dict())}")
+                    
                     # Not present
                     return Nil()
             elif type(name.value) == dict:
-                if index_value in name.value:
-                    return Auto(name.value[index_value], "basic")
+                # Rebuild
+                value = {}
+                for key, v in name.value.items():
+                    if type(key) not in BASE_TYPES:
+                        value[self.remove_quotes(key.value) if type(key.value) == str else key.value] = v
+                    else:
+                        value[self.remove_quotes(key)] = v
+                if index_value in value:
+                    return Auto(value[index_value], "basic")
                 else:
+                    print(f"dict does not contain {index_value}, it only contains: {list(value.keys())}")
                     return Nil()
             elif type(name.value) == Map:
-                if index_value in name.value.value:
-                    return Auto(name.value.value[index_value], "basic")
+                value = {}
+                for key, v in name.value.value.items():
+                    if type(key) not in BASE_TYPES:
+                        value[self.remove_quotes(key.value) if type(key.value) == str else key.value] = v
+                    else:
+                        value[self.remove_quotes(key)] = v
+                if index_value in value:
+                    return Auto(value[index_value], "basic")
                 else:
+                    print(f"Map does not contain {index_value}, it only contains: {list(value.keys())}")
                     return Nil()
             elif type(name.value) == DynArray:
                 if 0 <= index_value < name.value.length:
                     return Auto(name.value.value[index_value], "basic")
                 else:
                     raise TranspilerExceptions.OutOfBounds(index_value, name.value.length)
             # raise TranspilerExceptions.Generic(f"Can't get index on {name.value}")
-            return Nil()
+            else:
+                raise TranspilerExceptions.TypeMissmatch(f"Get Index Actor: {name.value}", type(name.value), [ID, DynArray, Map], line)
         elif type(name) == Nil:
             return Nil()
         else:
             raise TranspilerExceptions.TypeMissmatch(f"Get Index Actor: {name}", type(name), [ID, DynArray], line)
         return Nil()
 
 class SetIndexMod(Module):
@@ -545,46 +606,68 @@
         # Dependencies
         resolution_module: Module = self.compiler_instance.get_action('RESOLUT')
 
         # pprint(tree)
         # exit()
         line = tree['ID'][-1]
         name = resolution_module(tree['ID'][1]['EXPRESSION'])
-        index = resolution_module(tree['ID'][1]['INDEX'])
+        index_value = resolution_module(tree['ID'][1]['INDEX'])
         value = resolution_module(tree['EXPRESSION'])
 
-        if type(index) == String:
-            index_value = self.remove_quotes(index.value)
-        else: index_value = index.value
+        while type(index_value) not in BASE_TYPES:
+            index_value = index_value.value
+            if type(index_value) == str:
+                index_value = self.remove_quotes(index_value)
+
 
         if type(value) == String:
             value = self.remove_quotes(value.value)
+
+        if type(name.value) == markupsafe.Markup:
+            if str(name.value) != "":
+                def add_quotes_if_missing(match):
+                    content = match.group(1)  # The content within the parentheses
+                    # Check if the content is already wrapped in quotes
+                    if not (content.startswith('"') and content.endswith('"')) and not (content.startswith("'") and content.endswith("'")):
+                        return f'String("{content}")'  # Add quotes if they're missing
+                    else:
+                        return f'String({content})'  # Keep as is if quotes are present
+                v = str(name.value)
+                v = re.sub(r'String\(([^)]+)\)', add_quotes_if_missing, v)
+                print(v)
+                try:
+                    name.value = eval(str(v)) # TODO: Oh god forgive me   
+                except NameError as e:
+                    raise TranspilerExceptions.Generic(f"Failed to convert Markupsafe to a valid entity: {name.value}\nError: {e}")
+            else:
+                return Nil()
+    
         
 
         if type(name) == ID:
             var = self.compiler_instance.get_variable(name.value)
             if var['type'] == DynArray:
                 if 0 <= index_value < var['object'].length:
                     var['object'].value[index_value] = value
                 else:
                     raise TranspilerExceptions.OutOfBounds(index_value, var['object'].length)
             elif var['type'] == Session:
-                # print("Session contains:",var['object'].value[index_value], type(var['object'].value[index_value]))
-                var['object'].value[index_value] = value.value
+                print("Session contains:",var['object'].value.get(index_value), type(var['object'].value.get(index_value)))
+                var['object'].value[index_value] = value # Auto(value, "basic").value
             else:
                 raise TranspilerExceptions.TypeMissmatch("Get ID Index Actor", var['type'], [ID, DynArray], line)
         elif type(name) == DynArray:
             raise TranspilerExceptions.NotImplemented
         elif type(name) == Auto:
             if type(name.value) == dict:
                 name.value[index_value] = value
             elif type(name.value) == Map:
                 name.value.value[index_value] = value
             else:
-                raise TranspilerExceptions.Generic(f"{name.value} is not a map.")
+                raise TranspilerExceptions.Generic(f"{name.value} of type {type(name.value)} is not a map.")
         else:
             raise TranspilerExceptions.TypeMissmatch(f"Get Index Actor '{name}'", type(name), [ID, DynArray], line)
         
 class ResolutionMod(Module):
     name="RESOLUT"
     type = Module.MODULE_TYPES.ACTION
 
@@ -601,16 +684,19 @@
         if tree[0] == 'FORMATTED_STRING':
             pattern = re.compile(r":\$(\w+):")
             text = tree[1]['VALUE']
 
             def replace(match):
                 variable_name = match.group(1)
                 value = self.compiler_instance.get_variable(variable_name)['object']
+
+                if type(value) in NOPHP_TYPES:
+                    value = value.value
                 
-                return str(self.safely_resolve(value.value))
+                return str(self.safely_resolve(value))
 
             result = pattern.sub(replace, text)
             return String(result)
 
         elif tree[0] == 'INT':
             return Int32(tree[1]['VALUE'])
         
@@ -941,15 +1027,15 @@
     name="FUNCTION_CALL"
     type = Module.MODULE_TYPES.SPECIAL_ACTION
 
     def __init__(self, compiler_instance):
         super().__init__()
         self.compiler_instance = compiler_instance
 
-    def run_sInnerMut(self, funcobj, arguments):
+    def run_sInnerMut(self, funcobj, arguments={}):
         # Dependencies
         resolution_module: Module = self.compiler_instance.get_action('RESOLUT')
         if 'POSITIONAL_ARGS' in arguments:
             parsed_args = [
                 resolution_module(arg)
                 for arg in arguments['POSITIONAL_ARGS']
             ]
@@ -1032,14 +1118,15 @@
                     resolution_module(arg)
                     for arg in arguments['POSITIONAL_ARGS']
                 ]
             else: parsed_args = []
 
         console.log(f"[FunctionCallMod] {funcname}(...) from {cls}")
 
+        # sInnerMut is cursed, find an alternative?
         if type(funcobj) == sInnerMut:
             return self.run_sInnerMut(funcobj, arguments)
         elif cls is not None:
             if cls == 'parent':
                 function_parent = self.compiler_instance.parent
                 class_parent    = function_parent.parent # grandad
                 if class_parent is None:
@@ -1168,15 +1255,15 @@
     def proc_tree(self, tree):
         # Dependencies
         resolution_module: Module = self.compiler_instance.get_action('RESOLUT')
 
         v = resolution_module(tree["EXPRESSION"])
 
         self.compiler_instance.returns = v
-        self.compiler_instance.stop = True
+        self.compiler_instance.stop = True # This hard kills the compiler instance
         
 
 
 class TarrowMod(Module):
     name="TARROW"
     type = Module.MODULE_TYPES.NON_WRITEABLE
 
@@ -1188,14 +1275,16 @@
         # TODO: Add sometihng idk
         # TODO: Add parent
         if tree["FROM"] == "this":
             # print(self.compiler_instance.get_variable(tree["TO"])['object'])
             return self.compiler_instance.get_variable(tree["TO"])['object']
         elif tree["FROM"] in self.compiler_instance.variables:
             o = self.compiler_instance.get_variable(tree["FROM"])['object']
+            if type(o) == Nil:
+                raise TranspilerExceptions.Generic(f"Unable to find callable unit on a value of Nil. '{tree['FROM']}' was Nil\n::Information::\n'{self.compiler_instance.get_variable(tree['FROM'])}'")
             # print(tree["TO"], o.get_variable(tree["TO"]), self.compiler_instance.namespace)
             return Auto(o.get_variable(tree["TO"])['object'], 'basic').value
         else:
             raise TranspilerExceptions.NotImplemented
         
 class ClassAttrMod(Module):
     name="CLASS_ATTR"
@@ -1346,20 +1435,25 @@
         # Process first and second value
         first = resolution_module(tree[1])
         second = resolution_module(tree[2])
         
         def atomize(val):
             if type(val) == ID:
                 val = self.compiler_instance.get_variable(val.value)['object']
+            
+            val = Auto(val, "basic").value
             return val
         
         first = atomize(first)
         second = atomize(second)
 
-        return Int32(op(first, second))
+        try:
+            return Auto(op(first, second), "basic").value # This should now handle floats
+        except TypeError as e:
+            raise TranspilerExceptions.Generic(f"Failed to perform a mathematical operation:\n{e}\nFirst:{first}\nSecond:{second}")
 
 class ConditionalMod(Module):
     name="CONDITIONAL"
     type = Module.MODULE_TYPES.SPECIAL_ACTION
 
     def __init__(self, compiler_instance):
         super().__init__()
@@ -1424,16 +1518,16 @@
             def atomize(val):
                 if type(val) == ID:
                     val = atomize(self.compiler_instance.get_variable(val.value)['object'])
                 elif type(val) in [Int32, String, Bool, Float] :
                     val = val.value
                 elif type(val) == Auto:
                     val = atomize(val.value)
-                else:
-                    print(type(val))
+                # else:
+                    # print(type(val))
                 return val
 
             first = atomize(first)
             second = atomize(second)
 
             # Evaluate condition and run it's code
             c = condition(first, second)
@@ -1460,15 +1554,15 @@
         self.compiler_instance = compiler_instance
     
     def proc_tree(self, tree):
         resolution_module: Module = self.compiler_instance.get_action('RESOLUT')
         conditional_module: Module = self.compiler_instance.get_action('CONDITIONAL')
         empty: Module = self.compiler_instance.get_action('empty') # Actually a function
 
-        pprint(tree)
+        # pprint(tree)
         op = tree[0]
         first = tree[1]
         second = tree[2]
 
         if op == 'AND':
             return empty((first,)).value and empty((second,)).value
         elif op == 'OR':
@@ -1550,19 +1644,23 @@
 
         finished = []
 
         program = tree['PROGRAM']
 
         if type(iterable) == ID:
             var = self.compiler_instance.get_variable(iterable.value)
+            if type(var['object']) == Auto:
+                var['object'] = var['object'].value
 
-            if var['type'] == DynArray:
+            if type(var['object']) == DynArray:
                 for value in var['object'].value:
                     # Inject value as the variable
                     
+                    # Automatically convert to a typed object
+                    value = Auto(value, "basic").value
 
                     instance = self.compiler_instance.new_instance(
                         tree=program,
                         sync="advanced"
                     )
 
                     instance.create_variable(
```

### Comparing `nophp-0.1.8rc1/nophp/lang/pparser.py` & `nophp-0.1.8rc2/nophp/lang/pparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 from sly import Parser
 from sly.yacc import YaccProduction, YaccSymbol
 import logging
 
 from .lexer import PyettyLexer
 
 class PyettyParser(Parser):
@@ -219,14 +220,30 @@
         ("left", "+", "-"),
         ("left", "*", "/", "%"),
         ("right", UMINUS, UPLUS),
         ("right", "!"),
         ("left", COLON_COLON),
     )
 
+    def error(self, p):
+        if p:
+            print("Syntax error at token", p.type)
+            print(f"Line: {p.lineno}")
+            if hasattr(p, 'index'):
+                print(f"Position: {p.index}")
+            # Attempt to give context by printing surrounding tokens
+            print("Context (tokens around error):")
+            context_range = 5  # Number of tokens to show before/after the error
+            token_list = list(itertools.islice(self.tokens, max(0, p.index - context_range), p.index + context_range))
+            for tok in token_list:
+                print(f"  {tok.type} at line {tok.lineno}, position {tok.index}")
+        else:
+            print("Syntax error at EOF")
+        exit(0)
+
     # Program START
     @_("program statement")
     def program(self, p):
         return p.program + (p.statement,)
 
     @_("statement")
     def program(self, p):
@@ -310,22 +327,14 @@
         return p.sandbox
     
     @_("expression")
     def statement(self, p):
         return p.expression
         
 
-    def error(self, p):
-        print("Whoa. You are seriously hosed.")
-        if not p:
-            print("End of File!")
-        else:
-            print("Failed at ", p)
-        exit(1)
-
     # Statements END
     ###########################################################################
     # Statment syntax START
 
     @_("LIMPORT expression ';'")
     def sandbox(self, p):
         return ("LIMPORT", {"EXPRESSION": p.expression}, p.lineno)
```

### Comparing `nophp-0.1.8rc1/nophp/lang/std/__pycache__/bcrypt.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/std/__pycache__/bcrypt.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/__pycache__/db.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/std/__pycache__/db.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/__pycache__/echo.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/std/__pycache__/echo.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/__pycache__/htmlspecialchars.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/std/__pycache__/htmlspecialchars.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/__pycache__/internal.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/std/__pycache__/internal.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/__pycache__/json.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/std/__pycache__/json.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/__pycache__/primitives.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/std/__pycache__/primitives.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/__pycache__/rand.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/std/__pycache__/rand.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/__pycache__/redirect.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/std/__pycache__/redirect.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/__pycache__/session.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/std/__pycache__/session.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/__pycache__/str.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/std/__pycache__/str.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/__pycache__/string.cpython-312.pyc` & `nophp-0.1.8rc2/nophp/lang/std/__pycache__/string.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/bcrypt.py` & `nophp-0.1.8rc2/nophp/lang/std/bcrypt.py`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/db.py` & `nophp-0.1.8rc2/nophp/lang/std/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         elif type(value) == SqlConnector:
             value = value.value
         elif type(value) == DynArray:
             _value = value.value
             value = []
             for i in _value:
                 value.append(self.safely_resolve(i)) 
+        elif type(value) == Float:
+            value = value.value
         return value
     
 
 # sql_connect("db.sql")
 class DbConnect(DbCommonMod):
     name="DBCONN"
     type = Module.MODULE_TYPES.FUNCTION
```

### Comparing `nophp-0.1.8rc1/nophp/lang/std/echo.py` & `nophp-0.1.8rc2/nophp/lang/std/echo.py`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/htmlspecialchars.py` & `nophp-0.1.8rc2/nophp/lang/std/htmlspecialchars.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 def htmlspecialchars(text):
     return (
         text.replace("&", "&amp;").
         replace('"', "&quot;").
         replace("<", "&lt;").
         replace(">", "&gt;")
     )
+def invert_htmlspecialchars(text):
+    return (
+        text.replace( "&amp;", "&").
+        replace("&quot;", '"').
+        replace("&lt;", "<").
+        replace("&gt;", ">")
+    )
 
 
 class HTMLSpecialCharMod(Module):
     name="htmlspecialchars"
     type = Module.MODULE_TYPES.FUNCTION
 
     def __init__(self, compiler_instance):
@@ -42,12 +49,52 @@
                 value = self.remove_quotes(resolved.value)
 
             
 
             values.append(value) 
 
         if len(values) > 1:
-            raise TranspilerExceptions.TooManyValues(values, "echo($msg)")
+            raise TranspilerExceptions.TooManyValues(values, "htmlspecialchars($msg)")
         
 
 
         return String(htmlspecialchars(str(value)))
+
+class InvertHTMLSpecialCharMod(Module):
+    name="inverthtmlspecialchars"
+    type = Module.MODULE_TYPES.FUNCTION
+
+    def __init__(self, compiler_instance):
+        super().__init__()
+        self.compiler_instance = compiler_instance
+
+    def proc_tree(self, tree):
+        # Dependencies
+        resolution_module: Module = self.compiler_instance.get_action('RESOLUT')
+        values = []
+
+        for var in tree['FUNCTION_ARGUMENTS']['POSITIONAL_ARGS']:
+            resolved = resolution_module(var)
+            value: BasicType = None
+            
+            if type(resolved) == ID:
+                value = resolved.value
+                v = self.compiler_instance.get_variable(value)
+                if v["type"] == String:
+                    value = self.remove_quotes(v['object'].value)
+                elif v["type"] == type(None):
+                    value = ""
+                else:
+                    value = v['object'].value
+            elif type(resolved) == String:
+                value = self.remove_quotes(resolved.value)
+
+            
+
+            values.append(value) 
+
+        if len(values) > 1:
+            raise TranspilerExceptions.TooManyValues(values, "invert_htmlspecialchars($msg)")
+        
+
+
+        return String(invert_htmlspecialchars(str(value)))
```

### Comparing `nophp-0.1.8rc1/nophp/lang/std/internal.py` & `nophp-0.1.8rc2/nophp/lang/std/internal.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,18 +52,57 @@
     def __init__(self, compiler_instance):
         super().__init__(compiler_instance)
         self.compiler_instance = compiler_instance
 
     def proc_tree(self, tree):
         # Mirror functionality of INTERNAL_CALL(die)
         self.compiler_instance.stop = True
+
+
+# typeof($var)
+class NoPHPTypeOf(CommonInternalMod):
+    name="typeof"
+    type = Module.MODULE_TYPES.FUNCTION
+
+    def __init__(self, compiler_instance):
+        super().__init__(compiler_instance)
+        self.compiler_instance = compiler_instance
+
+    def proc_tree(self, tree):
+        values = self.base(tree)
+        value = values[0]
+
+        return String(
+            str(type(value))
+        )
     
+
+# toInt($var)
+class NoPHPToInt(CommonInternalMod):
+    name="toInt"
+    type = Module.MODULE_TYPES.FUNCTION
+
+    def __init__(self, compiler_instance):
+        super().__init__(compiler_instance)
+        self.compiler_instance = compiler_instance
+
+    def proc_tree(self, tree):
+        values = self.base(tree)
+        value = values[0]
+
+        return Int32(
+            value
+        )
+    
+
 _MODS = {
     "nophp_version": VersionInfo,
-    "die": NoPHPDie
+    "die": NoPHPDie,
+    "typeof": NoPHPTypeOf,
+    "toInt": NoPHPToInt,
 }
 
 def build_funcs(c):
     functions = {}
     for f in _MODS:
         functions[f] = {
                 "run_func": _MODS[f](c)
```

### Comparing `nophp-0.1.8rc1/nophp/lang/std/json.py` & `nophp-0.1.8rc2/nophp/lang/std/json.py`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/primitives.py` & `nophp-0.1.8rc2/nophp/lang/std/primitives.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 from ..exceptions import TranspilerExceptions, Warn
 from ..module import Module
 from ..types import *
 
 
 class CommonMod(Module):
     name="COMMON"
@@ -83,23 +84,59 @@
 
     def __init__(self, compiler_instance):
         super().__init__(compiler_instance)
         self.compiler_instance = compiler_instance
 
     def proc_tree(self, tree):
         array, value = self.base(tree, ref=True)[:2]
+        line = tree['ID'][-1]
 
+        if type(array) == Auto  :
+            array = array.value
+
+        if type(array) != DynArray:
+            raise TranspilerExceptions.TypeMissmatch("args[0]", type(array), DynArray, line) 
+        
         array.value.append(value)
 
-        return Bool(True)
+        print("array1212:", hash(array))
+
+        return array;
+
+
+# array_push_deep($array, $value)
+class ArrayPushDeepMod(CommonMod):
+    name="array_push_deep"
+    type = Module.MODULE_TYPES.FUNCTION
+
+    def __init__(self, compiler_instance):
+        super().__init__(compiler_instance)
+        self.compiler_instance = compiler_instance
+
+    def proc_tree(self, tree):
+        array, value = self.base(tree, ref=True)[:2]
+        line = tree['ID'][-1]
+
+        if type(array) == Auto:
+            array = array.value
+
+        if type(array) != DynArray:
+            raise TranspilerExceptions.TypeMissmatch("args[0]", type(array), DynArray, line) 
+        
+        array.value.append(value)
+
+        print("array1212:", hash(array))
+
+        return array;
     
 _MODS = {
     "count": CountMod,
-    "ArrayMod": ArrayMod,
+    "array": ArrayMod,
     "array_push": ArrayPushMod,
+    "array_push_deep": ArrayPushDeepMod,
     "empty": EmptyMod
 }
 
 def build_funcs(c):
     functions = {}
     for f in _MODS:
         functions[f] = {
```

### Comparing `nophp-0.1.8rc1/nophp/lang/std/rand.py` & `nophp-0.1.8rc2/nophp/lang/std/rand.py`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/redirect.py` & `nophp-0.1.8rc2/nophp/lang/std/redirect.py`

 * *Files identical despite different names*

### Comparing `nophp-0.1.8rc1/nophp/lang/std/session.py` & `nophp-0.1.8rc2/nophp/lang/std/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,25 +70,25 @@
         if len(values) != 0:
             raise TranspilerExceptions.IncorrectNumberOfValues(values, "session_start()")
         
         # session['aa'] = "bb"
 
         # Session already exists
         if "_noid" in session:
-            print("Session exists")
+            self.compiler_instance.log("Session exists")
         else:
             global SESSION_TRACKER
             try:
                 session['_noid'] = generate_session()
             except RuntimeError as e:
-                print("No secret key was set. Unable to securely create a session. Please add a 'secret_key' entry to the wool.yaml config.")
+                self.compiler_instance.log("No secret key was set. Unable to securely create a session. Please add a 'secret_key' entry to the wool.yaml config.")
             SESSION_TRACKER[session['_noid']] = {
                 "_cin": self.compiler_instance.namespace # Created in
             }
-            print(f"Session created for {session['_noid']}")
+            self.compiler_instance.log(f"Session created for {session['_noid']}")
 
         # Add new variable 
         self.compiler_instance.create_variable(
             "_SESSION",
             Session,
             Session(), 
             force=True
@@ -111,13 +111,13 @@
         if len(values) != 0:
             raise TranspilerExceptions.IncorrectNumberOfValues(values, "session_destroy()")
         
         # session['aa'] = "bb"
 
         # Session already exists
         if "_noid" in session:
-            print("Session exists, destroying")
+            self.compiler_instance.log("Session exists, destroying")
             global SESSION_TRACKER
             if session['_noid'] in SESSION_TRACKER:
                 del SESSION_TRACKER[session['_noid']]
             session.clear()
         return Nil
```

### Comparing `nophp-0.1.8rc1/nophp/lang/std/string.py` & `nophp-0.1.8rc2/nophp/lang/std/string.py`

 * *Files 9% similar despite different names*

```diff
@@ -114,8 +114,31 @@
         # Check if all arguments are strings or integers
         if not isinstance(subject_str, str) or not isinstance(start, int) or (length is not None and not isinstance(length, int)):
             raise TranspilerExceptions.TypeMissmatch("substr()", "string, int[, int]", 0)
 
         # Perform the substring operation
         result_str = subject_str[start:start+length] if length is not None else subject_str[start:]
         # print("res:",result_str, subject_str, start, length)
-        return String(result_str)
+        return String(result_str)
+    
+
+
+class EscapeStrMod(StrMod):
+    name = "escape_str"
+    type = Module.MODULE_TYPES.FUNCTION
+
+    def __init__(self, compiler_instance):
+        super().__init__(compiler_instance)
+
+    def proc_tree(self, tree):
+        values = self.base(tree)
+
+        if len(values) != 1:
+            raise TranspilerExceptions.IncorrectNumberOfValues(values, "escape_str()")
+
+        # Extract the values from the list
+        subject_str = self.remove_quotes(values[0])
+
+        if not isinstance(subject_str, str):
+            raise TranspilerExceptions.TypeMissmatch("substr()", "string", 0)
+
+        return String(subject_str.replace('"', '\\"'))
```

### Comparing `nophp-0.1.8rc1/nophp/lang/types.py` & `nophp-0.1.8rc2/nophp/lang/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from markupsafe import Markup
 from werkzeug.datastructures import ImmutableMultiDict
 
 class BasicType:
     def __init__(self):
         self.value: object
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.value})"
@@ -16,18 +17,21 @@
         return str(self.value)
 
 class String(BasicType):
     '''
     Simple String type
     '''
     def __init__(self, value):
-        self.value = f'"{value}"'
+        self.value = f'{value}'
         self.length = len(value)
         super().__init__()
 
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}('{self.value}')"
+
 class ID(BasicType):
     '''
     Simple ID type
     '''
     def __init__(self, value):
         self.value = value
         self.length = len(value)
@@ -173,15 +177,16 @@
     This is used for wrapping Python objects.
 
     For example: 
 
         Basic matching.
 
         We expect that the object contains all or most
-        of the known types
+        of the known types. It will optimally match
+        a type.
         ```
         [Request]      -->      [Auto(Request)]
         |- str(method)            |- String(method)
         |- bytes(data)            |- DynArray(data, type=Char)
         |- ...                    |- ...
         ```
         
@@ -206,14 +211,15 @@
         if type(value) == Auto:
             value = value.value
         if _type == 'basic':
             _f = {
                 None: Nil,
                 str: String,
                 int: Int32,
+                float: Float,
                 dict: Map,
                 list: DynArray,
                 tuple: DynArray,
                 # bad bad bad
                 type(None): Nil,
                 ImmutableMultiDict: Map
             }
@@ -309,9 +315,11 @@
 )
 
 BASE_TYPES = (
     str,
     list,
     int,
     tuple,
-    float
+    float,
+    dict,
+    Markup
 )
```

### Comparing `nophp-0.1.8rc1/nophp/spindle.py` & `nophp-0.1.8rc2/nophp/spindle.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     session,
     redirect,
     primitives,
     db,
     bcrypt,
     json,
     internal,
+    stripe,
 )
 
 # Read wool config
 # from sys import argv
 import argparse
 
 import yaml
@@ -192,23 +193,29 @@
             },
             "rand": {
                 "run_func": rand.RandMod(_c)
             },
             "htmlspecialchars": {
                 "run_func": htmlspecialchars.HTMLSpecialCharMod(_c)
             },
+            "invert_htmlspecialchars": {
+                "run_func": htmlspecialchars.InvertHTMLSpecialCharMod(_c)
+            },
             "strlen": {
                 "run_func": string.StrLenMod(_c)
             },
             "str_replace": {
                 "run_func": string.StrReplaceMod(_c)
             },
             "substr": {
                 "run_func": string.SubstrMod(_c)
             },
+            "escape_str": {
+                "run_func": string.EscapeStrMod(_c)
+            },
             "nl2br": {
                 "run_func": string.Nl2BrMod(_c)
             },
             "session_start": {
                 "run_func": session.SessionStartMod(_c)
             },
             "session_destroy": {
@@ -219,14 +226,15 @@
             },
 
             **db.build_funcs(_c),
             **primitives.build_funcs(_c),
             **bcrypt.build_funcs(_c),
             **json.build_funcs(_c),
             **internal.build_funcs(_c),
+            **stripe.build_funcs(_c),
             
             "require_once": {
                 "run_func": RequireOnceMod(_c)
             },
             "include": {
                 "run_func": IncludeMod(_c)
             },
@@ -257,15 +265,15 @@
         
     
     def register(self, route, file):
         global BIGGEST_PAGES
         def _func(*args, **kwargs):
             _c = Compiler([])
             out = self.build_sp(file, _c)
-            return out
+            return "<!DOCTYPE html>" + out
         
         name = f"_func_" + str(random.randint(0,BIGGEST_PAGES))
         while name in self.functions:
             name = f"_func_" + str(random.randint(0,BIGGEST_PAGES))
 
 
         _func.__name__ = _func.__qualname__ = name
```

### Comparing `nophp-0.1.8rc1/nophp/weaver.py` & `nophp-0.1.8rc2/nophp/weaver.py`

 * *Files identical despite different names*

