# Comparing `tmp/dovekie-0.4.0.tar.gz` & `tmp/dovekie-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dovekie-0.4.0.tar", last modified: Wed Apr  3 21:45:33 2024, max compression
+gzip compressed data, was "dovekie-0.5.0.tar", last modified: Mon Apr  8 18:29:55 2024, max compression
```

## Comparing `dovekie-0.4.0.tar` & `dovekie-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxr-x   0 cph       (1000) cph       (1000)        0 2024-04-03 21:45:33.339960 dovekie-0.4.0/
--rw-rw-r--   0 cph       (1000) cph       (1000)     1071 2024-04-02 14:50:52.000000 dovekie-0.4.0/LICENSE
--rw-r--r--   0 cph       (1000) cph       (1000)     2221 2024-04-03 21:45:33.339960 dovekie-0.4.0/PKG-INFO
--rw-rw-r--   0 cph       (1000) cph       (1000)     1932 2024-04-02 17:32:37.000000 dovekie-0.4.0/README.md
-drwxrwxr-x   0 cph       (1000) cph       (1000)        0 2024-04-03 21:45:33.339960 dovekie-0.4.0/dovekie/
--rw-rw-r--   0 cph       (1000) cph       (1000)       95 2024-04-03 21:43:11.000000 dovekie-0.4.0/dovekie/__init__.py
--rw-rw-r--   0 cph       (1000) cph       (1000)      237 2024-04-03 21:43:37.000000 dovekie-0.4.0/dovekie/core.py
-drwxrwxr-x   0 cph       (1000) cph       (1000)        0 2024-04-03 21:45:33.339960 dovekie-0.4.0/dovekie.egg-info/
--rw-r--r--   0 cph       (1000) cph       (1000)     2221 2024-04-03 21:45:33.000000 dovekie-0.4.0/dovekie.egg-info/PKG-INFO
--rw-rw-r--   0 cph       (1000) cph       (1000)      205 2024-04-03 21:45:33.000000 dovekie-0.4.0/dovekie.egg-info/SOURCES.txt
--rw-rw-r--   0 cph       (1000) cph       (1000)        1 2024-04-03 21:45:33.000000 dovekie-0.4.0/dovekie.egg-info/dependency_links.txt
--rw-rw-r--   0 cph       (1000) cph       (1000)        8 2024-04-03 21:45:33.000000 dovekie-0.4.0/dovekie.egg-info/top_level.txt
--rw-rw-r--   0 cph       (1000) cph       (1000)       38 2024-04-03 21:45:33.339960 dovekie-0.4.0/setup.cfg
--rw-rw-r--   0 cph       (1000) cph       (1000)      457 2024-04-03 21:43:30.000000 dovekie-0.4.0/setup.py
-drwxrwxr-x   0 cph       (1000) cph       (1000)        0 2024-04-03 21:45:33.339960 dovekie-0.4.0/tests/
--rw-rw-r--   0 cph       (1000) cph       (1000)      418 2024-04-03 21:27:22.000000 dovekie-0.4.0/tests/test_core.py
+drwxr-xr-x   0 cph       (1000) cph       (1000)        0 2024-04-08 18:29:55.490364 dovekie-0.5.0/
+-rw-r--r--   0 cph       (1000) cph       (1000)     1071 2024-04-07 17:09:48.000000 dovekie-0.5.0/LICENSE
+-rw-r--r--   0 cph       (1000) cph       (1000)     2248 2024-04-08 18:29:55.490364 dovekie-0.5.0/PKG-INFO
+-rw-r--r--   0 cph       (1000) cph       (1000)     1920 2024-04-08 18:20:58.000000 dovekie-0.5.0/README.md
+drwxr-xr-x   0 cph       (1000) cph       (1000)        0 2024-04-08 18:29:55.490364 dovekie-0.5.0/dovekie/
+-rw-r--r--   0 cph       (1000) cph       (1000)       48 2024-04-08 18:20:22.000000 dovekie-0.5.0/dovekie/__init__.py
+-rw-r--r--   0 cph       (1000) cph       (1000)      271 2024-04-08 18:22:30.000000 dovekie-0.5.0/dovekie/core.py
+drwxr-xr-x   0 cph       (1000) cph       (1000)        0 2024-04-08 18:29:55.490364 dovekie-0.5.0/dovekie.egg-info/
+-rw-r--r--   0 cph       (1000) cph       (1000)     2248 2024-04-08 18:29:55.000000 dovekie-0.5.0/dovekie.egg-info/PKG-INFO
+-rw-r--r--   0 cph       (1000) cph       (1000)      186 2024-04-08 18:29:55.000000 dovekie-0.5.0/dovekie.egg-info/SOURCES.txt
+-rw-r--r--   0 cph       (1000) cph       (1000)        1 2024-04-08 18:29:55.000000 dovekie-0.5.0/dovekie.egg-info/dependency_links.txt
+-rw-r--r--   0 cph       (1000) cph       (1000)        8 2024-04-08 18:29:55.000000 dovekie-0.5.0/dovekie.egg-info/top_level.txt
+-rw-r--r--   0 cph       (1000) cph       (1000)       38 2024-04-08 18:29:55.490364 dovekie-0.5.0/setup.cfg
+-rw-r--r--   0 cph       (1000) cph       (1000)      457 2024-04-08 18:28:28.000000 dovekie-0.5.0/setup.py
```

### Comparing `dovekie-0.4.0/LICENSE` & `dovekie-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dovekie-0.4.0/PKG-INFO` & `dovekie-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: dovekie
-Version: 0.4.0
+Version: 0.5.0
 Summary: A library that defines common SKI combinators from Combinatory Logic.
+Home-page: UNKNOWN
 Author: Conor Hoekstra
 Author-email: codereport@outlook.com
 License: MIT
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <p align="center">`dovekie`</p>
 
 <p align="center">
@@ -41,15 +43,17 @@
 ```
 
 And how to use:
 ```py
 import operator as op
 from itertools import accumulate
 
-from dovekie import _phi1_, _r_
+import dovekie as d
 
 
 def mco(xs: list[int]) -> int:
-    return max(accumulate(xs, _phi1_(op.add, op.mul, _r_)))
+    return max(accumulate(xs, d.phi1(op.add, op.mul, d.r)))
 
 print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3
 ```
+
+
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: dovekie Version: 0.4.0 Summary: A library that
-defines common SKI combinators from Combinatory Logic. Author: Conor Hoekstra
-Author-email: codereport@outlook.com License: MIT Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE #
+Metadata-Version: 2.1 Name: dovekie Version: 0.5.0 Summary: A library that
+defines common SKI combinators from Combinatory Logic. Home-page: UNKNOWN
+Author: Conor Hoekstra Author-email: codereport@outlook.com License: MIT
+Platform: UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE #
                                    `dovekie`
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_n_t_r_i_b_u_t_i_o_n_s_-_w_e_l_c_o_m_e_-_b_r_i_g_h_t_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
       _b_a_d_g_e_/_P_y_t_h_o_n_-_3_-_f_f_6_9_b_4_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_f_o_l_l_o_w_e_r_s_/
 _c_o_d_e_r_e_p_o_r_t_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_a_b_e_l_=_F_o_l_l_o_w_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/
 _c_o_d_e_r_e_p_o_r_t_/_d_o_v_e_k_i_e_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_a_b_e_l_=_S_t_a_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/
             _f_o_l_l_o_w_/_c_o_d_e___r_e_p_o_r_t_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_a_b_e_l_=_@_c_o_d_e___r_e_p_o_r_t_]
@@ -13,10 +14,10 @@
 combinators from [Combinatory Logic](https://combinatorylogic.com/) and common
 unary and binary functions that are often used with these combinators. It is
 the spritual equivalent of the: * C++ [`blackbird` library](https://github.com/
 codereport/blackbird) * Rust [`bluebird` library](https://github.com/
 codereport/bluebird)
                            [image-removebg-preview]
 How to install: ```bash pip3 install dovekie ``` And how to use: ```py import
-operator as op from itertools import accumulate from dovekie import _phi1_, _r_
-def mco(xs: list[int]) -> int: return max(accumulate(xs, _phi1_(op.add, op.mul,
-_r_))) print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3 ```
+operator as op from itertools import accumulate import dovekie as d def mco(xs:
+list[int]) -> int: return max(accumulate(xs, d.phi1(op.add, op.mul, d.r)))
+print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3 ```
```

### Comparing `dovekie-0.4.0/README.md` & `dovekie-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ```
 
 And how to use:
 ```py
 import operator as op
 from itertools import accumulate
 
-from dovekie import _phi1_, _r_
+import dovekie as d
 
 
 def mco(xs: list[int]) -> int:
-    return max(accumulate(xs, _phi1_(op.add, op.mul, _r_)))
+    return max(accumulate(xs, d.phi1(op.add, op.mul, d.r)))
 
 print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3
 ```
```

#### html2text {}

```diff
@@ -10,10 +10,10 @@
 combinators from [Combinatory Logic](https://combinatorylogic.com/) and common
 unary and binary functions that are often used with these combinators. It is
 the spritual equivalent of the: * C++ [`blackbird` library](https://github.com/
 codereport/blackbird) * Rust [`bluebird` library](https://github.com/
 codereport/bluebird)
                            [image-removebg-preview]
 How to install: ```bash pip3 install dovekie ``` And how to use: ```py import
-operator as op from itertools import accumulate from dovekie import _phi1_, _r_
-def mco(xs: list[int]) -> int: return max(accumulate(xs, _phi1_(op.add, op.mul,
-_r_))) print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3 ```
+operator as op from itertools import accumulate import dovekie as d def mco(xs:
+list[int]) -> int: return max(accumulate(xs, d.phi1(op.add, op.mul, d.r)))
+print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3 ```
```

### Comparing `dovekie-0.4.0/dovekie.egg-info/PKG-INFO` & `dovekie-0.5.0/dovekie.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: dovekie
-Version: 0.4.0
+Version: 0.5.0
 Summary: A library that defines common SKI combinators from Combinatory Logic.
+Home-page: UNKNOWN
 Author: Conor Hoekstra
 Author-email: codereport@outlook.com
 License: MIT
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <p align="center">`dovekie`</p>
 
 <p align="center">
@@ -41,15 +43,17 @@
 ```
 
 And how to use:
 ```py
 import operator as op
 from itertools import accumulate
 
-from dovekie import _phi1_, _r_
+import dovekie as d
 
 
 def mco(xs: list[int]) -> int:
-    return max(accumulate(xs, _phi1_(op.add, op.mul, _r_)))
+    return max(accumulate(xs, d.phi1(op.add, op.mul, d.r)))
 
 print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3
 ```
+
+
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: dovekie Version: 0.4.0 Summary: A library that
-defines common SKI combinators from Combinatory Logic. Author: Conor Hoekstra
-Author-email: codereport@outlook.com License: MIT Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE #
+Metadata-Version: 2.1 Name: dovekie Version: 0.5.0 Summary: A library that
+defines common SKI combinators from Combinatory Logic. Home-page: UNKNOWN
+Author: Conor Hoekstra Author-email: codereport@outlook.com License: MIT
+Platform: UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE #
                                    `dovekie`
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_n_t_r_i_b_u_t_i_o_n_s_-_w_e_l_c_o_m_e_-_b_r_i_g_h_t_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
       _b_a_d_g_e_/_P_y_t_h_o_n_-_3_-_f_f_6_9_b_4_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_f_o_l_l_o_w_e_r_s_/
 _c_o_d_e_r_e_p_o_r_t_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_a_b_e_l_=_F_o_l_l_o_w_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/
 _c_o_d_e_r_e_p_o_r_t_/_d_o_v_e_k_i_e_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_a_b_e_l_=_S_t_a_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/
             _f_o_l_l_o_w_/_c_o_d_e___r_e_p_o_r_t_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_a_b_e_l_=_@_c_o_d_e___r_e_p_o_r_t_]
@@ -13,10 +14,10 @@
 combinators from [Combinatory Logic](https://combinatorylogic.com/) and common
 unary and binary functions that are often used with these combinators. It is
 the spritual equivalent of the: * C++ [`blackbird` library](https://github.com/
 codereport/blackbird) * Rust [`bluebird` library](https://github.com/
 codereport/bluebird)
                            [image-removebg-preview]
 How to install: ```bash pip3 install dovekie ``` And how to use: ```py import
-operator as op from itertools import accumulate from dovekie import _phi1_, _r_
-def mco(xs: list[int]) -> int: return max(accumulate(xs, _phi1_(op.add, op.mul,
-_r_))) print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3 ```
+operator as op from itertools import accumulate import dovekie as d def mco(xs:
+list[int]) -> int: return max(accumulate(xs, d.phi1(op.add, op.mul, d.r)))
+print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3 ```
```

