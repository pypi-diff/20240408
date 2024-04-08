# Comparing `tmp/lpsd-1.0.3.tar.gz` & `tmp/lpsd-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpsd-1.0.3.tar", max compression
+gzip compressed data, was "lpsd-1.0.4.tar", max compression
```

## Comparing `lpsd-1.0.3.tar` & `lpsd-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35059 2023-01-09 06:38:34.325494 lpsd-1.0.3/LICENSE
--rw-r--r--   0        0        0     1594 2023-01-09 06:38:34.325494 lpsd-1.0.3/README.md
--rw-r--r--   0        0        0      362 2023-01-09 06:38:34.325494 lpsd-1.0.3/build.py
--rw-r--r--   0        0        0      455 2023-01-09 06:38:34.325494 lpsd-1.0.3/lpsd/__init__.py
--rw-r--r--   0        0        0    15439 2023-01-09 06:38:34.325494 lpsd-1.0.3/lpsd/_helpers.py
--rw-r--r--   0        0        0     8239 2023-01-09 06:38:34.325494 lpsd-1.0.3/lpsd/_lcsd.py
--rw-r--r--   0        0        0    13807 2023-01-09 06:38:34.333494 lpsd-1.0.3/lpsd/flattop.py
--rwxr-xr-x   0        0        0   107008 2023-01-09 06:38:34.333494 lpsd-1.0.3/lpsd/ltpda_dft.dll
--rwxr-xr-x   0        0        0    94440 2023-01-09 08:04:40.000000 lpsd-1.0.3/lpsd/ltpda_dft.so
--rw-r--r--   0        0        0     5097 2023-01-09 06:38:34.333494 lpsd-1.0.3/lpsd/wrapper.py
--rw-r--r--   0        0        0     1707 2023-01-09 07:09:22.936853 lpsd-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2579 1970-01-01 00:00:00.000000 lpsd-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35059 2024-04-08 13:51:39.319023 lpsd-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1594 2024-04-08 13:51:39.319023 lpsd-1.0.4/README.md
+-rw-r--r--   0        0        0      362 2024-04-08 13:51:39.319023 lpsd-1.0.4/build.py
+-rw-r--r--   0        0        0      455 2024-04-08 13:51:39.319023 lpsd-1.0.4/lpsd/__init__.py
+-rw-r--r--   0        0        0    15439 2024-04-08 13:51:39.319023 lpsd-1.0.4/lpsd/_helpers.py
+-rw-r--r--   0        0        0     8240 2024-04-08 14:40:51.339233 lpsd-1.0.4/lpsd/_lcsd.py
+-rw-r--r--   0        0        0    13808 2024-04-08 14:40:51.339233 lpsd-1.0.4/lpsd/flattop.py
+-rwxr-xr-x   0        0        0   107008 2024-04-08 13:51:39.323023 lpsd-1.0.4/lpsd/ltpda_dft.dll
+-rwxr-xr-x   0        0        0    93832 2024-04-08 14:52:41.000000 lpsd-1.0.4/lpsd/ltpda_dft.so
+-rw-r--r--   0        0        0     5098 2024-04-08 14:40:51.339233 lpsd-1.0.4/lpsd/wrapper.py
+-rw-r--r--   0        0        0     1705 2024-04-08 14:40:51.343233 lpsd-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2630 1970-01-01 00:00:00.000000 lpsd-1.0.4/PKG-INFO
```

### Comparing `lpsd-1.0.3/LICENSE` & `lpsd-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lpsd-1.0.3/README.md` & `lpsd-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lpsd-1.0.3/lpsd/_helpers.py` & `lpsd-1.0.4/lpsd/_helpers.py`

 * *Files identical despite different names*

### Comparing `lpsd-1.0.3/lpsd/_lcsd.py` & `lpsd-1.0.4/lpsd/_lcsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module contains LCSD class which holds all necessary parameters for logarithmic spectral density (LCSD/LPSD)
 calculation
 """
+
 from typing import Callable, Optional, Union
 from warnings import warn
 
 import numpy as np
 from pandas import DataFrame, Series
 from pandas.core.indexes.datetimes import DatetimeIndex
```

### Comparing `lpsd-1.0.3/lpsd/flattop.py` & `lpsd-1.0.4/lpsd/flattop.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 Spectrum and spectral density estimation by the Discrete Fourier transform (DFT), including a comprehensive list of window functions and some new flat-top windows
 G. Heinzel, A. Rudiger, and R. Schilling
 Maz-Planck-Institut fur Gravitationsphysik
 (Albert-Einstein-Institut)
 Teilinstitut Hannover
 February 15, 2002
 """
+
 import numpy as np
 
 
 def SFT3F(M):
     """Flat-top window function SFT3F.
 
     Differentiable, -31.7 dB, NBW 3.1681 bins, 0.0082 dB, first zero at +/- 3 bins.
```

### Comparing `lpsd-1.0.3/lpsd/ltpda_dft.dll` & `lpsd-1.0.4/lpsd/ltpda_dft.dll`

 * *Files identical despite different names*

### Comparing `lpsd-1.0.3/lpsd/ltpda_dft.so` & `lpsd-1.0.4/lpsd/ltpda_dft.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 4% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -4,17 +4,17 @@
   Data:                              2's complement, little endian
   Version:                           1 (current)
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
-  Entry point address:               0x1140
+  Entry point address:               0x0
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          92648 (bytes into file)
+  Start of section headers:          92040 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         9
   Size of section headers:           64 (bytes)
   Number of section headers:         28
   Section header string table index: 27
```

#### readelf --wide --program-header {}

```diff
@@ -1,23 +1,23 @@
 
 Elf file type is DYN (Shared object file)
-Entry point 0x1140
+Entry point 0x0
 There are 9 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
   LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x000860 0x000860 R   0x1000
-  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x00b29d 0x00b29d R E 0x1000
+  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x00b081 0x00b081 R E 0x1000
   LOAD           0x00d000 0x000000000000d000 0x000000000000d000 0x0088a4 0x0088a4 R   0x1000
-  LOAD           0x015e10 0x0000000000016e10 0x0000000000016e10 0x000290 0x000298 RW  0x1000
-  DYNAMIC        0x015e20 0x0000000000016e20 0x0000000000016e20 0x0001c0 0x0001c0 RW  0x8
+  LOAD           0x015df8 0x0000000000016df8 0x0000000000016df8 0x000290 0x000298 RW  0x1000
+  DYNAMIC        0x015e08 0x0000000000016e08 0x0000000000016e08 0x0001c0 0x0001c0 RW  0x8
   NOTE           0x000238 0x0000000000000238 0x0000000000000238 0x000024 0x000024 R   0x4
   GNU_EH_FRAME   0x015618 0x0000000000015618 0x0000000000015618 0x00008c 0x00008c R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
-  GNU_RELRO      0x015e10 0x0000000000016e10 0x0000000000016e10 0x0001f0 0x0001f0 R   0x1
+  GNU_RELRO      0x015df8 0x0000000000016df8 0x0000000000016df8 0x000208 0x000208 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     .note.gnu.build-id .gnu.hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt 
    01     .init .plt .plt.got .text .fini 
    02     .rodata .eh_frame_hdr .eh_frame 
    03     .init_array .fini_array .dynamic .got .got.plt .data .bss
```

#### readelf --wide --sections {}

```diff
@@ -1,8 +1,8 @@
-There are 28 section headers, starting at offset 0x169e8:
+There are 28 section headers, starting at offset 0x16788:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .note.gnu.build-id NOTE            0000000000000238 000238 000024 00   A  0   0  4
   [ 2] .gnu.hash         GNU_HASH        0000000000000260 000260 000064 00   A  3   0  8
   [ 3] .dynsym           DYNSYM          00000000000002c8 0002c8 000210 18   A  4   1  8
@@ -10,28 +10,28 @@
   [ 5] .gnu.version      VERSYM          00000000000005da 0005da 00002c 02   A  3   0  2
   [ 6] .gnu.version_r    VERNEED         0000000000000608 000608 000030 00   A  4   1  8
   [ 7] .rela.dyn         RELA            0000000000000638 000638 0000a8 18   A  3   0  8
   [ 8] .rela.plt         RELA            00000000000006e0 0006e0 000180 18  AI  3  21  8
   [ 9] .init             PROGBITS        0000000000001000 001000 000017 00  AX  0   0  4
   [10] .plt              PROGBITS        0000000000001020 001020 000110 10  AX  0   0 16
   [11] .plt.got          PROGBITS        0000000000001130 001130 000008 08  AX  0   0  8
-  [12] .text             PROGBITS        0000000000001140 001140 00b152 00  AX  0   0 16
-  [13] .fini             PROGBITS        000000000000c294 00c294 000009 00  AX  0   0  4
+  [12] .text             PROGBITS        0000000000001140 001140 00af36 00  AX  0   0 16
+  [13] .fini             PROGBITS        000000000000c078 00c078 000009 00  AX  0   0  4
   [14] .rodata           PROGBITS        000000000000d000 00d000 008618 00   A  0   0 16
   [15] .eh_frame_hdr     PROGBITS        0000000000015618 015618 00008c 00   A  0   0  4
   [16] .eh_frame         PROGBITS        00000000000156a8 0156a8 0001fc 00   A  0   0  8
-  [17] .init_array       INIT_ARRAY      0000000000016e10 015e10 000008 08  WA  0   0  8
-  [18] .fini_array       FINI_ARRAY      0000000000016e18 015e18 000008 08  WA  0   0  8
-  [19] .dynamic          DYNAMIC         0000000000016e20 015e20 0001c0 10  WA  4   0  8
-  [20] .got              PROGBITS        0000000000016fe0 015fe0 000020 08  WA  0   0  8
-  [21] .got.plt          PROGBITS        0000000000017000 016000 000098 08  WA  0   0  8
-  [22] .data             PROGBITS        0000000000017098 016098 000008 00  WA  0   0  8
-  [23] .bss              NOBITS          00000000000170a0 0160a0 000008 00  WA  0   0  1
-  [24] .comment          PROGBITS        0000000000000000 0160a0 000027 01  MS  0   0  1
-  [25] .symtab           SYMTAB          0000000000000000 0160c8 000618 18     26  44  8
-  [26] .strtab           STRTAB          0000000000000000 0166e0 000214 00      0   0  1
-  [27] .shstrtab         STRTAB          0000000000000000 0168f4 0000f1 00      0   0  1
+  [17] .init_array       INIT_ARRAY      0000000000016df8 015df8 000008 08  WA  0   0  8
+  [18] .fini_array       FINI_ARRAY      0000000000016e00 015e00 000008 08  WA  0   0  8
+  [19] .dynamic          DYNAMIC         0000000000016e08 015e08 0001c0 10  WA  4   0  8
+  [20] .got              PROGBITS        0000000000016fc8 015fc8 000020 08  WA  0   0  8
+  [21] .got.plt          PROGBITS        0000000000016fe8 015fe8 000098 08  WA  0   0  8
+  [22] .data             PROGBITS        0000000000017080 016080 000008 00  WA  0   0  8
+  [23] .bss              NOBITS          0000000000017088 016088 000008 00  WA  0   0  1
+  [24] .comment          PROGBITS        0000000000000000 016088 00001f 01  MS  0   0  1
+  [25] .symtab           SYMTAB          0000000000000000 0160a8 0003d8 18     26  20  8
+  [26] .strtab           STRTAB          0000000000000000 016480 000214 00      0   0  1
+  [27] .shstrtab         STRTAB          0000000000000000 016694 0000f1 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -5,89 +5,65 @@
      1: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5 (2)
      2: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
      3: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND calloc@GLIBC_2.2.5 (2)
      4: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
      5: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcpy@GLIBC_2.14 (3)
      6: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
      7: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (2)
-     8: 00000000000026d0  3469 FUNC    GLOBAL DEFAULT   12 polyreg6
-     9: 0000000000001200   104 FUNC    GLOBAL DEFAULT   12 polyreg0
-    10: 0000000000006470  9957 FUNC    GLOBAL DEFAULT   12 polyreg9
-    11: 000000000000ba50    94 FUNC    GLOBAL DEFAULT   12 myround
-    12: 0000000000001520   809 FUNC    GLOBAL DEFAULT   12 polyreg3
-    13: 0000000000001850  1409 FUNC    GLOBAL DEFAULT   12 polyreg4
-    14: 0000000000003460  4991 FUNC    GLOBAL DEFAULT   12 polyreg7
-    15: 0000000000001270   204 FUNC    GLOBAL DEFAULT   12 polyreg1
-    16: 000000000000bbb0  1762 FUNC    GLOBAL DEFAULT   12 dft
-    17: 00000000000047e0  7303 FUNC    GLOBAL DEFAULT   12 polyreg8
-    18: 0000000000001340   477 FUNC    GLOBAL DEFAULT   12 polyreg2
-    19: 0000000000008b60 12001 FUNC    GLOBAL DEFAULT   12 polyreg10
-    20: 000000000000bab0   244 FUNC    GLOBAL DEFAULT   12 detrend
-    21: 0000000000001de0  2283 FUNC    GLOBAL DEFAULT   12 polyreg5
+     8: 0000000000002640  3397 FUNC    GLOBAL DEFAULT   12 polyreg6
+     9: 0000000000001200    95 FUNC    GLOBAL DEFAULT   12 polyreg0
+    10: 0000000000006380  9951 FUNC    GLOBAL DEFAULT   12 polyreg9
+    11: 000000000000b920    94 FUNC    GLOBAL DEFAULT   12 myround
+    12: 00000000000014f0   787 FUNC    GLOBAL DEFAULT   12 polyreg3
+    13: 0000000000001810  1379 FUNC    GLOBAL DEFAULT   12 polyreg4
+    14: 0000000000003390  4943 FUNC    GLOBAL DEFAULT   12 polyreg7
+    15: 0000000000001260   194 FUNC    GLOBAL DEFAULT   12 polyreg1
+    16: 000000000000ba80  1526 FUNC    GLOBAL DEFAULT   12 dft
+    17: 00000000000046e0  7323 FUNC    GLOBAL DEFAULT   12 polyreg8
+    18: 0000000000001330   433 FUNC    GLOBAL DEFAULT   12 polyreg2
+    19: 0000000000008a60 11965 FUNC    GLOBAL DEFAULT   12 polyreg10
+    20: 000000000000b980   244 FUNC    GLOBAL DEFAULT   12 detrend
+    21: 0000000000001d80  2237 FUNC    GLOBAL DEFAULT   12 polyreg5
 
-Symbol table '.symtab' contains 65 entries:
+Symbol table '.symtab' contains 41 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000238     0 SECTION LOCAL  DEFAULT    1 .note.gnu.build-id
-     2: 0000000000000260     0 SECTION LOCAL  DEFAULT    2 .gnu.hash
-     3: 00000000000002c8     0 SECTION LOCAL  DEFAULT    3 .dynsym
-     4: 00000000000004d8     0 SECTION LOCAL  DEFAULT    4 .dynstr
-     5: 00000000000005da     0 SECTION LOCAL  DEFAULT    5 .gnu.version
-     6: 0000000000000608     0 SECTION LOCAL  DEFAULT    6 .gnu.version_r
-     7: 0000000000000638     0 SECTION LOCAL  DEFAULT    7 .rela.dyn
-     8: 00000000000006e0     0 SECTION LOCAL  DEFAULT    8 .rela.plt
-     9: 0000000000001000     0 SECTION LOCAL  DEFAULT    9 .init
-    10: 0000000000001020     0 SECTION LOCAL  DEFAULT   10 .plt
-    11: 0000000000001130     0 SECTION LOCAL  DEFAULT   11 .plt.got
-    12: 0000000000001140     0 SECTION LOCAL  DEFAULT   12 .text
-    13: 000000000000c294     0 SECTION LOCAL  DEFAULT   13 .fini
-    14: 000000000000d000     0 SECTION LOCAL  DEFAULT   14 .rodata
-    15: 0000000000015618     0 SECTION LOCAL  DEFAULT   15 .eh_frame_hdr
-    16: 00000000000156a8     0 SECTION LOCAL  DEFAULT   16 .eh_frame
-    17: 0000000000016e10     0 SECTION LOCAL  DEFAULT   17 .init_array
-    18: 0000000000016e18     0 SECTION LOCAL  DEFAULT   18 .fini_array
-    19: 0000000000016e20     0 SECTION LOCAL  DEFAULT   19 .dynamic
-    20: 0000000000016fe0     0 SECTION LOCAL  DEFAULT   20 .got
-    21: 0000000000017000     0 SECTION LOCAL  DEFAULT   21 .got.plt
-    22: 0000000000017098     0 SECTION LOCAL  DEFAULT   22 .data
-    23: 00000000000170a0     0 SECTION LOCAL  DEFAULT   23 .bss
-    24: 0000000000000000     0 SECTION LOCAL  DEFAULT   24 .comment
-    25: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    26: 0000000000001140     0 FUNC    LOCAL  DEFAULT   12 deregister_tm_clones
-    27: 0000000000001170     0 FUNC    LOCAL  DEFAULT   12 register_tm_clones
-    28: 00000000000011b0     0 FUNC    LOCAL  DEFAULT   12 __do_global_dtors_aux
-    29: 00000000000170a0     1 OBJECT  LOCAL  DEFAULT   23 completed.0
-    30: 0000000000016e18     0 OBJECT  LOCAL  DEFAULT   18 __do_global_dtors_aux_fini_array_entry
-    31: 00000000000011f0     0 FUNC    LOCAL  DEFAULT   12 frame_dummy
-    32: 0000000000016e10     0 OBJECT  LOCAL  DEFAULT   17 __frame_dummy_init_array_entry
-    33: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS ltpda_dft.c
-    34: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    35: 00000000000158a0     0 OBJECT  LOCAL  DEFAULT   16 __FRAME_END__
-    36: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
-    37: 000000000000c294     0 FUNC    LOCAL  DEFAULT   13 _fini
-    38: 0000000000017098     0 OBJECT  LOCAL  DEFAULT   22 __dso_handle
-    39: 0000000000016e20     0 OBJECT  LOCAL  DEFAULT   19 _DYNAMIC
-    40: 0000000000015618     0 NOTYPE  LOCAL  DEFAULT   15 __GNU_EH_FRAME_HDR
-    41: 00000000000170a0     0 OBJECT  LOCAL  DEFAULT   22 __TMC_END__
-    42: 0000000000017000     0 OBJECT  LOCAL  DEFAULT   21 _GLOBAL_OFFSET_TABLE_
-    43: 0000000000001000     0 FUNC    LOCAL  DEFAULT    9 _init
-    44: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5
-    45: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-    46: 000000000000bbb0  1762 FUNC    GLOBAL DEFAULT   12 dft
-    47: 00000000000026d0  3469 FUNC    GLOBAL DEFAULT   12 polyreg6
-    48: 00000000000047e0  7303 FUNC    GLOBAL DEFAULT   12 polyreg8
-    49: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND calloc@GLIBC_2.2.5
-    50: 0000000000001200   104 FUNC    GLOBAL DEFAULT   12 polyreg0
-    51: 0000000000001340   477 FUNC    GLOBAL DEFAULT   12 polyreg2
-    52: 0000000000001850  1409 FUNC    GLOBAL DEFAULT   12 polyreg4
-    53: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-    54: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcpy@GLIBC_2.14
-    55: 0000000000008b60 12001 FUNC    GLOBAL DEFAULT   12 polyreg10
-    56: 000000000000bab0   244 FUNC    GLOBAL DEFAULT   12 detrend
-    57: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-    58: 0000000000006470  9957 FUNC    GLOBAL DEFAULT   12 polyreg9
-    59: 0000000000001de0  2283 FUNC    GLOBAL DEFAULT   12 polyreg5
-    60: 0000000000003460  4991 FUNC    GLOBAL DEFAULT   12 polyreg7
-    61: 000000000000ba50    94 FUNC    GLOBAL DEFAULT   12 myround
-    62: 0000000000001270   204 FUNC    GLOBAL DEFAULT   12 polyreg1
-    63: 0000000000001520   809 FUNC    GLOBAL DEFAULT   12 polyreg3
-    64: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
+     2: 0000000000001140     0 FUNC    LOCAL  DEFAULT   12 deregister_tm_clones
+     3: 0000000000001170     0 FUNC    LOCAL  DEFAULT   12 register_tm_clones
+     4: 00000000000011b0     0 FUNC    LOCAL  DEFAULT   12 __do_global_dtors_aux
+     5: 0000000000017088     1 OBJECT  LOCAL  DEFAULT   23 completed.0
+     6: 0000000000016e00     0 OBJECT  LOCAL  DEFAULT   18 __do_global_dtors_aux_fini_array_entry
+     7: 00000000000011f0     0 FUNC    LOCAL  DEFAULT   12 frame_dummy
+     8: 0000000000016df8     0 OBJECT  LOCAL  DEFAULT   17 __frame_dummy_init_array_entry
+     9: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS ltpda_dft.c
+    10: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
+    11: 00000000000158a0     0 OBJECT  LOCAL  DEFAULT   16 __FRAME_END__
+    12: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
+    13: 000000000000c078     0 FUNC    LOCAL  DEFAULT   13 _fini
+    14: 0000000000017080     0 OBJECT  LOCAL  DEFAULT   22 __dso_handle
+    15: 0000000000016e08     0 OBJECT  LOCAL  DEFAULT   19 _DYNAMIC
+    16: 0000000000015618     0 NOTYPE  LOCAL  DEFAULT   15 __GNU_EH_FRAME_HDR
+    17: 0000000000017088     0 OBJECT  LOCAL  DEFAULT   22 __TMC_END__
+    18: 0000000000016fe8     0 OBJECT  LOCAL  DEFAULT   21 _GLOBAL_OFFSET_TABLE_
+    19: 0000000000001000     0 FUNC    LOCAL  DEFAULT    9 _init
+    20: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5
+    21: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
+    22: 000000000000ba80  1526 FUNC    GLOBAL DEFAULT   12 dft
+    23: 0000000000002640  3397 FUNC    GLOBAL DEFAULT   12 polyreg6
+    24: 00000000000046e0  7323 FUNC    GLOBAL DEFAULT   12 polyreg8
+    25: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND calloc@GLIBC_2.2.5
+    26: 0000000000001200    95 FUNC    GLOBAL DEFAULT   12 polyreg0
+    27: 0000000000001330   433 FUNC    GLOBAL DEFAULT   12 polyreg2
+    28: 0000000000001810  1379 FUNC    GLOBAL DEFAULT   12 polyreg4
+    29: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
+    30: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcpy@GLIBC_2.14
+    31: 0000000000008a60 11965 FUNC    GLOBAL DEFAULT   12 polyreg10
+    32: 000000000000b980   244 FUNC    GLOBAL DEFAULT   12 detrend
+    33: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+    34: 0000000000006380  9951 FUNC    GLOBAL DEFAULT   12 polyreg9
+    35: 0000000000001d80  2237 FUNC    GLOBAL DEFAULT   12 polyreg5
+    36: 0000000000003390  4943 FUNC    GLOBAL DEFAULT   12 polyreg7
+    37: 000000000000b920    94 FUNC    GLOBAL DEFAULT   12 myround
+    38: 0000000000001260   194 FUNC    GLOBAL DEFAULT   12 polyreg1
+    39: 00000000000014f0   787 FUNC    GLOBAL DEFAULT   12 polyreg3
+    40: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
```

#### readelf --wide --relocs {}

```diff
@@ -1,29 +1,29 @@
 
 Relocation section '.rela.dyn' at offset 0x638 contains 7 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000016e10  0000000000000008 R_X86_64_RELATIVE                         11f0
-0000000000016e18  0000000000000008 R_X86_64_RELATIVE                         11b0
-0000000000017098  0000000000000008 R_X86_64_RELATIVE                         17098
-0000000000016fe0  0000000200000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
-0000000000016fe8  0000000400000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
-0000000000016ff0  0000000600000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
-0000000000016ff8  0000000700000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
+0000000000016df8  0000000000000008 R_X86_64_RELATIVE                         11f0
+0000000000016e00  0000000000000008 R_X86_64_RELATIVE                         11b0
+0000000000017080  0000000000000008 R_X86_64_RELATIVE                         17080
+0000000000016fc8  0000000200000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
+0000000000016fd0  0000000400000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
+0000000000016fd8  0000000600000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
+0000000000016fe0  0000000700000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
 
 Relocation section '.rela.plt' at offset 0x6e0 contains 16 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000017018  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
-0000000000017020  0000000800000007 R_X86_64_JUMP_SLOT     00000000000026d0 polyreg6 + 0
-0000000000017028  0000001100000007 R_X86_64_JUMP_SLOT     00000000000047e0 polyreg8 + 0
-0000000000017030  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 calloc@GLIBC_2.2.5 + 0
-0000000000017038  0000000900000007 R_X86_64_JUMP_SLOT     0000000000001200 polyreg0 + 0
-0000000000017040  0000001200000007 R_X86_64_JUMP_SLOT     0000000000001340 polyreg2 + 0
-0000000000017048  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000001850 polyreg4 + 0
-0000000000017050  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 memcpy@GLIBC_2.14 + 0
-0000000000017058  0000001300000007 R_X86_64_JUMP_SLOT     0000000000008b60 polyreg10 + 0
-0000000000017060  0000001400000007 R_X86_64_JUMP_SLOT     000000000000bab0 detrend + 0
-0000000000017068  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000006470 polyreg9 + 0
-0000000000017070  0000001500000007 R_X86_64_JUMP_SLOT     0000000000001de0 polyreg5 + 0
-0000000000017078  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000003460 polyreg7 + 0
-0000000000017080  0000000b00000007 R_X86_64_JUMP_SLOT     000000000000ba50 myround + 0
-0000000000017088  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000001270 polyreg1 + 0
-0000000000017090  0000000c00000007 R_X86_64_JUMP_SLOT     0000000000001520 polyreg3 + 0
+0000000000017000  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
+0000000000017008  0000000800000007 R_X86_64_JUMP_SLOT     0000000000002640 polyreg6 + 0
+0000000000017010  0000001100000007 R_X86_64_JUMP_SLOT     00000000000046e0 polyreg8 + 0
+0000000000017018  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 calloc@GLIBC_2.2.5 + 0
+0000000000017020  0000000900000007 R_X86_64_JUMP_SLOT     0000000000001200 polyreg0 + 0
+0000000000017028  0000001200000007 R_X86_64_JUMP_SLOT     0000000000001330 polyreg2 + 0
+0000000000017030  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000001810 polyreg4 + 0
+0000000000017038  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 memcpy@GLIBC_2.14 + 0
+0000000000017040  0000001300000007 R_X86_64_JUMP_SLOT     0000000000008a60 polyreg10 + 0
+0000000000017048  0000001400000007 R_X86_64_JUMP_SLOT     000000000000b980 detrend + 0
+0000000000017050  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000006380 polyreg9 + 0
+0000000000017058  0000001500000007 R_X86_64_JUMP_SLOT     0000000000001d80 polyreg5 + 0
+0000000000017060  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000003390 polyreg7 + 0
+0000000000017068  0000000b00000007 R_X86_64_JUMP_SLOT     000000000000b920 myround + 0
+0000000000017070  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000001260 polyreg1 + 0
+0000000000017078  0000000c00000007 R_X86_64_JUMP_SLOT     00000000000014f0 polyreg3 + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -1,23 +1,23 @@
 
-Dynamic section at offset 0x15e20 contains 24 entries:
+Dynamic section at offset 0x15e08 contains 24 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x000000000000000c (INIT)               0x1000
- 0x000000000000000d (FINI)               0xc294
- 0x0000000000000019 (INIT_ARRAY)         0x16e10
+ 0x000000000000000d (FINI)               0xc078
+ 0x0000000000000019 (INIT_ARRAY)         0x16df8
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
- 0x000000000000001a (FINI_ARRAY)         0x16e18
+ 0x000000000000001a (FINI_ARRAY)         0x16e00
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x260
  0x0000000000000005 (STRTAB)             0x4d8
  0x0000000000000006 (SYMTAB)             0x2c8
  0x000000000000000a (STRSZ)              257 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
- 0x0000000000000003 (PLTGOT)             0x17000
+ 0x0000000000000003 (PLTGOT)             0x16fe8
  0x0000000000000002 (PLTRELSZ)           384 (bytes)
  0x0000000000000014 (PLTREL)             RELA
  0x0000000000000017 (JMPREL)             0x6e0
  0x0000000000000007 (RELA)               0x638
  0x0000000000000008 (RELASZ)             168 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
  0x000000006ffffffe (VERNEED)            0x608
```

#### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 40f7a5f19aeafc07aecae1455626a1f8cc693a6b
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 938aef8e7e7bc39f648f42586e844036b668828c
```

#### readelf --wide --version-info {}

```diff
@@ -1,12 +1,12 @@
 
 Version symbols section '.gnu.version' contains 22 entries:
  Addr: 0x00000000000005da  Offset: 0x000005da  Link: 3 (.dynsym)
-  000:   0 (*local*)       2 (GLIBC_2.2.5)   0 (*local*)       2 (GLIBC_2.2.5)
-  004:   0 (*local*)       3 (GLIBC_2.14)    0 (*local*)       2 (GLIBC_2.2.5)
+  000:   0 (*local*)       2 (GLIBC_2.2.5)   1 (*global*)      2 (GLIBC_2.2.5)
+  004:   1 (*global*)      3 (GLIBC_2.14)    1 (*global*)      2 (GLIBC_2.2.5)
   008:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   00c:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   010:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   014:   1 (*global*)      1 (*global*)   
 
 Version needs section '.gnu.version_r' contains 1 entry:
  Addr: 0x0000000000000608  Offset: 0x00000608  Link: 4 (.dynstr)
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -29,159 +29,159 @@
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000058 0000000000000010 0000005c FDE cie=00000000 pc=0000000000001200..0000000000001268
+00000058 0000000000000010 0000005c FDE cie=00000000 pc=0000000000001200..000000000000125f
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000006c 0000000000000010 00000070 FDE cie=00000000 pc=0000000000001270..000000000000133c
+0000006c 0000000000000010 00000070 FDE cie=00000000 pc=0000000000001260..0000000000001322
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000080 0000000000000010 00000084 FDE cie=00000000 pc=0000000000001340..000000000000151d
+00000080 0000000000000010 00000084 FDE cie=00000000 pc=0000000000001330..00000000000014e1
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000094 0000000000000010 00000098 FDE cie=00000000 pc=0000000000001520..0000000000001849
+00000094 0000000000000010 00000098 FDE cie=00000000 pc=00000000000014f0..0000000000001803
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000a8 0000000000000018 000000ac FDE cie=00000000 pc=0000000000001850..0000000000001dd1
-  DW_CFA_advance_loc: 4 to 0000000000001854
-  DW_CFA_def_cfa_offset: 72
-  DW_CFA_advance_loc2: 1347 to 0000000000001d97
+000000a8 0000000000000018 000000ac FDE cie=00000000 pc=0000000000001810..0000000000001d73
+  DW_CFA_advance_loc: 4 to 0000000000001814
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc2: 1339 to 0000000000001d4f
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 9 to 0000000000001da0
+  DW_CFA_advance_loc: 1 to 0000000000001d50
   DW_CFA_restore_state
 
-000000c4 0000000000000018 000000c8 FDE cie=00000000 pc=0000000000001de0..00000000000026cb
-  DW_CFA_advance_loc: 4 to 0000000000001de4
-  DW_CFA_def_cfa_offset: 104
-  DW_CFA_advance_loc2: 2219 to 000000000000268f
+000000c4 0000000000000018 000000c8 FDE cie=00000000 pc=0000000000001d80..000000000000263d
+  DW_CFA_advance_loc: 4 to 0000000000001d84
+  DW_CFA_def_cfa_offset: 88
+  DW_CFA_advance_loc2: 2184 to 000000000000260c
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000002690
+  DW_CFA_advance_loc: 4 to 0000000000002610
   DW_CFA_restore_state
 
-000000e0 000000000000001c 000000e4 FDE cie=00000000 pc=00000000000026d0..000000000000345d
-  DW_CFA_advance_loc: 7 to 00000000000026d7
+000000e0 000000000000001c 000000e4 FDE cie=00000000 pc=0000000000002640..0000000000003385
+  DW_CFA_advance_loc: 7 to 0000000000002647
   DW_CFA_def_cfa_offset: 168
-  DW_CFA_advance_loc2: 3391 to 0000000000003416
+  DW_CFA_advance_loc2: 3334 to 000000000000334d
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 10 to 0000000000003420
+  DW_CFA_advance_loc: 3 to 0000000000003350
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000100 000000000000001c 00000104 FDE cie=00000000 pc=0000000000003460..00000000000047df
-  DW_CFA_advance_loc: 7 to 0000000000003467
-  DW_CFA_def_cfa_offset: 264
-  DW_CFA_advance_loc2: 4906 to 0000000000004791
+00000100 000000000000001c 00000104 FDE cie=00000000 pc=0000000000003390..00000000000046df
+  DW_CFA_advance_loc: 7 to 0000000000003397
+  DW_CFA_def_cfa_offset: 232
+  DW_CFA_advance_loc2: 4877 to 00000000000046a4
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 0000000000004798
+  DW_CFA_advance_loc: 4 to 00000000000046a8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000120 000000000000001c 00000124 FDE cie=00000000 pc=00000000000047e0..0000000000006467
-  DW_CFA_advance_loc: 7 to 00000000000047e7
-  DW_CFA_def_cfa_offset: 328
-  DW_CFA_advance_loc2: 7211 to 0000000000006412
+00000120 000000000000001c 00000124 FDE cie=00000000 pc=00000000000046e0..000000000000637b
+  DW_CFA_advance_loc: 7 to 00000000000046e7
+  DW_CFA_def_cfa_offset: 312
+  DW_CFA_advance_loc2: 7235 to 000000000000632a
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 6 to 0000000000006418
+  DW_CFA_advance_loc: 6 to 0000000000006330
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000140 000000000000001c 00000144 FDE cie=00000000 pc=0000000000006470..0000000000008b55
-  DW_CFA_advance_loc: 7 to 0000000000006477
-  DW_CFA_def_cfa_offset: 376
-  DW_CFA_advance_loc2: 9852 to 0000000000008af3
+00000140 000000000000001c 00000144 FDE cie=00000000 pc=0000000000006380..0000000000008a5f
+  DW_CFA_advance_loc: 7 to 0000000000006387
+  DW_CFA_def_cfa_offset: 360
+  DW_CFA_advance_loc2: 9855 to 0000000000008a06
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 5 to 0000000000008af8
+  DW_CFA_advance_loc: 10 to 0000000000008a10
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000160 000000000000001c 00000164 FDE cie=00000000 pc=0000000000008b60..000000000000ba41
-  DW_CFA_advance_loc: 7 to 0000000000008b67
-  DW_CFA_def_cfa_offset: 488
-  DW_CFA_advance_loc2: 11876 to 000000000000b9cb
+00000160 000000000000001c 00000164 FDE cie=00000000 pc=0000000000008a60..000000000000b91d
+  DW_CFA_advance_loc: 7 to 0000000000008a67
+  DW_CFA_def_cfa_offset: 472
+  DW_CFA_advance_loc2: 11846 to 000000000000b8ad
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 5 to 000000000000b9d0
+  DW_CFA_advance_loc: 3 to 000000000000b8b0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000180 0000000000000010 00000184 FDE cie=00000000 pc=000000000000ba50..000000000000baae
+00000180 0000000000000010 00000184 FDE cie=00000000 pc=000000000000b920..000000000000b97e
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000194 0000000000000010 00000198 FDE cie=00000000 pc=000000000000bab0..000000000000bba4
+00000194 0000000000000010 00000198 FDE cie=00000000 pc=000000000000b980..000000000000ba74
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001a8 000000000000004c 000001ac FDE cie=00000000 pc=000000000000bbb0..000000000000c292
-  DW_CFA_advance_loc: 2 to 000000000000bbb2
+000001a8 000000000000004c 000001ac FDE cie=00000000 pc=000000000000ba80..000000000000c076
+  DW_CFA_advance_loc: 2 to 000000000000ba82
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 6 to 000000000000bbb8
+  DW_CFA_advance_loc: 6 to 000000000000ba88
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000bbba
+  DW_CFA_advance_loc: 2 to 000000000000ba8a
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000000bbbc
+  DW_CFA_advance_loc: 2 to 000000000000ba8c
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000bbbd
+  DW_CFA_advance_loc: 1 to 000000000000ba8d
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 000000000000bbbe
+  DW_CFA_advance_loc: 1 to 000000000000ba8e
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 000000000000bbc5
-  DW_CFA_def_cfa_offset: 240
-  DW_CFA_advance_loc2: 1262 to 000000000000c0b3
+  DW_CFA_advance_loc: 7 to 000000000000ba95
+  DW_CFA_def_cfa_offset: 224
+  DW_CFA_advance_loc2: 1164 to 000000000000bf21
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 000000000000c0b4
+  DW_CFA_advance_loc: 1 to 000000000000bf22
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000c0b5
+  DW_CFA_advance_loc: 1 to 000000000000bf23
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000c0b7
+  DW_CFA_advance_loc: 2 to 000000000000bf25
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000c0b9
+  DW_CFA_advance_loc: 2 to 000000000000bf27
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000c0bb
+  DW_CFA_advance_loc: 2 to 000000000000bf29
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000c0bd
+  DW_CFA_advance_loc: 2 to 000000000000bf2b
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 3 to 000000000000c0c0
+  DW_CFA_advance_loc: 5 to 000000000000bf30
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
 000001f8 ZERO terminator
```

#### strings --all --bytes=8 {}

```diff
@@ -13,17 +13,16 @@
 polyreg8
 polyreg9
 polyreg10
 libc.so.6
 GLIBC_2.14
 GLIBC_2.2.5
 AVAUATUSH
-D$`H9\$ 
 []A\A]A^A_
-GCC: (Debian 10.2.1-6) 10.2.1 20210110
+GCC: (Debian 12.2.0-14) 12.2.0
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.0
 __do_global_dtors_aux_fini_array_entry
 frame_dummy
 __frame_dummy_init_array_entry
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.init {}

```diff
@@ -2,13 +2,13 @@
 
 
 Disassembly of section .init:
 
 0000000000001000 <_init>:
 _init():
 	sub    $0x8,%rsp
-	mov    0x15fdd(%rip),%rax        
+	mov    0x15fc5(%rip),%rax        
 	test   %rax,%rax
 	je     1012 <_init+0x12>
 	call   *%rax
 	add    $0x8,%rsp
 	ret
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -1,89 +1,89 @@
 
 
 
 Disassembly of section .plt:
 
-0000000000001020 <.plt>:
-	push   0x15fe2(%rip)        
-	jmp    *0x15fe4(%rip)        
+0000000000001020 <free@plt-0x10>:
+	push   0x15fca(%rip)        
+	jmp    *0x15fcc(%rip)        
 	nopl   0x0(%rax)
 
 0000000000001030 <free@plt>:
-	jmp    *0x15fe2(%rip)        
+	jmp    *0x15fca(%rip)        
 	push   $0x0
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 0000000000001040 <polyreg6@plt>:
-	jmp    *0x15fda(%rip)        
+	jmp    *0x15fc2(%rip)        
 	push   $0x1
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 0000000000001050 <polyreg8@plt>:
-	jmp    *0x15fd2(%rip)        
+	jmp    *0x15fba(%rip)        
 	push   $0x2
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 0000000000001060 <calloc@plt>:
-	jmp    *0x15fca(%rip)        
+	jmp    *0x15fb2(%rip)        
 	push   $0x3
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 0000000000001070 <polyreg0@plt>:
-	jmp    *0x15fc2(%rip)        
+	jmp    *0x15faa(%rip)        
 	push   $0x4
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 0000000000001080 <polyreg2@plt>:
-	jmp    *0x15fba(%rip)        
+	jmp    *0x15fa2(%rip)        
 	push   $0x5
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 0000000000001090 <polyreg4@plt>:
-	jmp    *0x15fb2(%rip)        
+	jmp    *0x15f9a(%rip)        
 	push   $0x6
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 00000000000010a0 <memcpy@plt>:
-	jmp    *0x15faa(%rip)        
+	jmp    *0x15f92(%rip)        
 	push   $0x7
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 00000000000010b0 <polyreg10@plt>:
-	jmp    *0x15fa2(%rip)        
+	jmp    *0x15f8a(%rip)        
 	push   $0x8
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 00000000000010c0 <detrend@plt>:
-	jmp    *0x15f9a(%rip)        
+	jmp    *0x15f82(%rip)        
 	push   $0x9
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 00000000000010d0 <polyreg9@plt>:
-	jmp    *0x15f92(%rip)        
+	jmp    *0x15f7a(%rip)        
 	push   $0xa
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 00000000000010e0 <polyreg5@plt>:
-	jmp    *0x15f8a(%rip)        
+	jmp    *0x15f72(%rip)        
 	push   $0xb
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 00000000000010f0 <polyreg7@plt>:
-	jmp    *0x15f82(%rip)        
+	jmp    *0x15f6a(%rip)        
 	push   $0xc
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 0000000000001100 <myround@plt>:
-	jmp    *0x15f7a(%rip)        
+	jmp    *0x15f62(%rip)        
 	push   $0xd
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 0000000000001110 <polyreg1@plt>:
-	jmp    *0x15f72(%rip)        
+	jmp    *0x15f5a(%rip)        
 	push   $0xe
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
 
 0000000000001120 <polyreg3@plt>:
-	jmp    *0x15f6a(%rip)        
+	jmp    *0x15f52(%rip)        
 	push   $0xf
-	jmp    1020 <.plt>
+	jmp    1020 <_init+0x20>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.got {}

```diff
@@ -1,8 +1,8 @@
 
 
 
 Disassembly of section .plt.got:
 
 0000000000001130 <__cxa_finalize@plt>:
-	jmp    *0x15ec2(%rip)        
+	jmp    *0x15eaa(%rip)        
 	xchg   %ax,%ax
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1,1944 +1,1944 @@
 
 
 
 Disassembly of section .text:
 
 0000000000001140 <deregister_tm_clones>:
 deregister_tm_clones():
-	lea    0x15f59(%rip),%rdi        
-	lea    0x15f52(%rip),%rax        
+	lea    0x15f41(%rip),%rdi        
+	lea    0x15f3a(%rip),%rax        
 	cmp    %rdi,%rax
 	je     1168 <deregister_tm_clones+0x28>
-	mov    0x15e86(%rip),%rax        
+	mov    0x15e6e(%rip),%rax        
 	test   %rax,%rax
 	je     1168 <deregister_tm_clones+0x28>
 	jmp    *%rax
 	nopl   0x0(%rax)
 	ret
 	nopl   0x0(%rax)
 
 0000000000001170 <register_tm_clones>:
 register_tm_clones():
-	lea    0x15f29(%rip),%rdi        
-	lea    0x15f22(%rip),%rsi        
+	lea    0x15f11(%rip),%rdi        
+	lea    0x15f0a(%rip),%rsi        
 	sub    %rdi,%rsi
 	mov    %rsi,%rax
 	shr    $0x3f,%rsi
 	sar    $0x3,%rax
 	add    %rax,%rsi
 	sar    $1,%rsi
 	je     11a8 <register_tm_clones+0x38>
-	mov    0x15e55(%rip),%rax        
+	mov    0x15e3d(%rip),%rax        
 	test   %rax,%rax
 	je     11a8 <register_tm_clones+0x38>
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
 	ret
 	nopl   0x0(%rax)
 
 00000000000011b0 <__do_global_dtors_aux>:
 __do_global_dtors_aux():
-	cmpb   $0x0,0x15ee9(%rip)        
+	endbr64
+	cmpb   $0x0,0x15ecd(%rip)        
 	jne    11e8 <__do_global_dtors_aux+0x38>
 	push   %rbp
-	cmpq   $0x0,0x15e36(%rip)        
+	cmpq   $0x0,0x15e1a(%rip)        
 	mov    %rsp,%rbp
-	je     11d3 <__do_global_dtors_aux+0x23>
-	mov    0x15eca(%rip),%rdi        
+	je     11d7 <__do_global_dtors_aux+0x27>
+	mov    0x15eae(%rip),%rdi        
 	call   1130 <__cxa_finalize@plt>
 	call   1140 <deregister_tm_clones>
-	movb   $0x1,0x15ec1(%rip)        
+	movb   $0x1,0x15ea5(%rip)        
 	pop    %rbp
 	ret
-	nopl   0x0(%rax)
+	nopl   (%rax)
 	ret
 	nopl   0x0(%rax)
 
 00000000000011f0 <frame_dummy>:
 frame_dummy():
+	endbr64
 	jmp    1170 <register_tm_clones>
-	cs nopw 0x0(%rax,%rax,1)
-	nop
+	nopl   0x0(%rax)
 
 0000000000001200 <polyreg0>:
 polyreg0():
 	mov    %esi,-0xc(%rsp)
 	fildl  -0xc(%rsp)
-	mov    %rcx,%r8
 	fldz
 	fld    %st(0)
-	fld    %st(1)
-	faddp  %st,%st(3)
+	fxch   %st(2)
+	fadd   %st(1),%st
 	fld1
-	fdivp  %st,%st(3)
+	fdivp  %st,%st(1)
 	test   %esi,%esi
-	jle    1260 <polyreg0+0x60>
-	fstp   %st(0)
-	lea    -0x1(%rsi),%ecx
+	jle    1258 <polyreg0+0x58>
+	fstp   %st(2)
+	fxch   %st(1)
+	fxch   %st(1)
+	movslq %esi,%rsi
 	mov    %rdi,%rax
-	lea    0x8(%rdi,%rcx,8),%rcx
-	nopl   0x0(%rax,%rax,1)
+	shl    $0x3,%rsi
+	lea    (%rsi,%rdi,1),%r8
+	nopl   0x0(%rax)
 	faddl  (%rax)
 	add    $0x8,%rax
-	cmp    %rax,%rcx
+	cmp    %rax,%r8
 	jne    1230 <polyreg0+0x30>
 	fmulp  %st,%st(1)
-	mov    %esi,%esi
 	xor    %eax,%eax
-	nopl   0x0(%rax)
+	nop
 	fld    %st(0)
-	fsubrl (%rdi,%rax,8)
-	fstpl  (%rdx,%rax,8)
-	add    $0x1,%rax
+	fsubrl (%rdi,%rax,1)
+	fstpl  (%rdx,%rax,1)
+	add    $0x8,%rax
 	cmp    %rax,%rsi
-	jne    1248 <polyreg0+0x48>
-	fstpl  (%r8)
+	jne    1240 <polyreg0+0x40>
+	fstpl  (%rcx)
 	ret
-	nopl   (%rax)
+	nopl   0x0(%rax)
 	fstp   %st(1)
 	fmulp  %st,%st(1)
-	fstpl  (%r8)
+	fstpl  (%rcx)
 	ret
-	nopl   0x0(%rax,%rax,1)
+	nop
 
-0000000000001270 <polyreg1>:
+0000000000001260 <polyreg1>:
 polyreg1():
 	mov    %esi,-0x10(%rsp)
 	fildl  -0x10(%rsp)
 	fld1
 	fld    %st(1)
 	fsub   %st(1),%st
 	fld    %st(0)
-	fdivrs 0xbdaa(%rip)        
-	fldz
-	fld    %st(0)
-	fadd   %st(5),%st
-	fdivr  %st(4),%st
-	fldt   0xbdcc(%rip)        
-	fld    %st(6)
+	fdivrs 0xbdba(%rip)        
+	fldt   0xbdd4(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmulp  %st,%st(6)
+	fmul   %st(4),%st
 	fldz
-	faddp  %st,%st(6)
-	fxch   %st(3)
-	fdivp  %st,%st(5)
+	fld    %st(0)
+	fxch   %st(2)
+	fadd   %st(1),%st
+	fdivrp %st,%st(4)
+	fadd   %st,%st(5)
+	fxch   %st(5)
+	fdivr  %st(4),%st
 	test   %esi,%esi
-	jle    1330 <polyreg1+0xc0>
-	fstp   %st(0)
-	fldz
+	jle    1310 <polyreg1+0xb0>
 	movslq %esi,%rsi
 	xor    %eax,%eax
-	fldz
-	nopw   0x0(%rax,%rax,1)
+	nopl   (%rax)
 	fldl   (%rdi,%rax,8)
 	mov    %eax,-0x10(%rsp)
 	add    $0x1,%rax
-	fadd   %st,%st(1)
+	fadd   %st,%st(6)
 	fildl  -0x10(%rsp)
 	fmul   %st(4),%st
 	fsub   %st(6),%st
 	fmulp  %st,%st(1)
 	faddp  %st,%st(2)
-	cmp    %rax,%rsi
-	jne    12c0 <polyreg1+0x50>
+	cmp    %rsi,%rax
+	jne    12a0 <polyreg1+0x40>
 	fstp   %st(4)
 	fxch   %st(1)
 	fxch   %st(2)
 	fxch   %st(3)
-	fmulp  %st,%st(3)
+	fmulp  %st,%st(4)
 	xor    %eax,%eax
-	fmulp  %st,%st(3)
+	fmulp  %st,%st(2)
 	fld1
 	xchg   %ax,%ax
 	mov    %eax,-0x10(%rsp)
 	fildl  -0x10(%rsp)
 	fmul   %st(2),%st
 	fsub   %st(1),%st
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fmul   %st(3),%st
+	fadd   %st(4),%st
 	fsubrl (%rdi,%rax,8)
 	fstpl  (%rdx,%rax,8)
 	add    $0x1,%rax
-	cmp    %rsi,%rax
-	jne    12f0 <polyreg1+0x80>
+	cmp    %rax,%rsi
+	jne    12d0 <polyreg1+0x70>
 	fstp   %st(0)
 	fstp   %st(0)
+	fxch   %st(1)
 	fstpl  -0x10(%rsp)
 	movsd  -0x10(%rsp),%xmm0
 	fstpl  -0x10(%rsp)
 	movhpd -0x10(%rsp),%xmm0
 	movups %xmm0,(%rcx)
 	ret
-	nopl   0x0(%rax,%rax,1)
+	nopl   (%rax)
+	fstp   %st(5)
 	fstp   %st(3)
 	fstp   %st(0)
+	fxch   %st(2)
+	fmul   %st(1),%st
+	fxch   %st(2)
+	fmulp  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st,%st(1)
-	fmulp  %st,%st(2)
-	jmp    1313 <polyreg1+0xa3>
-	nopl   0x0(%rax)
+	jmp    12f5 <polyreg1+0x95>
+	data16 cs nopw 0x0(%rax,%rax,1)
+	nopl   (%rax)
 
-0000000000001340 <polyreg2>:
+0000000000001330 <polyreg2>:
 polyreg2():
-	mov    %esi,-0x48(%rsp)
-	fildl  -0x48(%rsp)
-	mov    %rcx,%r8
+	mov    %esi,-0x38(%rsp)
+	fildl  -0x38(%rsp)
 	fld1
 	fld    %st(1)
 	fsub   %st(1),%st
 	fld    %st(0)
 	fstpt  -0x18(%rsp)
-	fdivrs 0xbcd3(%rip)        
+	fdivrs 0xbce6(%rip)        
 	fld    %st(0)
-	fstpt  -0x28(%rsp)
+	fstpt  -0x38(%rsp)
 	test   %esi,%esi
-	jle    1500 <polyreg2+0x1c0>
-	pxor   %xmm1,%xmm1
-	movslq %esi,%rcx
+	jle    14d0 <polyreg2+0x1a0>
+	fldz
+	movslq %esi,%r8
 	xor    %eax,%eax
-	movss  %xmm1,-0x2c(%rsp)
-	flds   -0x2c(%rsp)
 	fld    %st(0)
 	fld    %st(1)
-	nopw   0x0(%rax,%rax,1)
-	mov    %eax,-0x48(%rsp)
-	fildl  -0x48(%rsp)
+	nopl   0x0(%rax,%rax,1)
+	mov    %eax,-0x38(%rsp)
+	fildl  -0x38(%rsp)
 	fmul   %st(4),%st
 	fsub   %st(5),%st
 	fldl   (%rdi,%rax,8)
 	add    $0x1,%rax
 	fadd   %st,%st(4)
 	fmul   %st(1),%st
 	fadd   %st,%st(2)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(2)
-	cmp    %rax,%rcx
-	jne    1388 <polyreg2+0x48>
+	cmp    %r8,%rax
+	jne    1368 <polyreg2+0x38>
 	fstp   %st(4)
 	fxch   %st(1)
 	fxch   %st(2)
-	fstpt  -0x28(%rsp)
+	fstpt  -0x38(%rsp)
 	fld    %st(3)
-	fmuls  0xbc78(%rip)        
+	fmuls  0xbc98(%rip)        
 	fld1
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fsubs  0xbc70(%rip)        
-	fldt   0xbca2(%rip)        
+	fsubs  0xbc90(%rip)        
+	fldt   0xbcb2(%rip)        
 	fmul   %st(5),%st
-	flds   -0x2c(%rsp)
+	fldz
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
-	fldt   0xbca0(%rip)        
+	fldt   0xbcb2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(6),%st
-	fld    %st(1)
+	fadd   %st(1),%st
+	fdivrp %st,%st(2)
 	fxch   %st(1)
-	fadd   %st(2),%st
-	fdivrp %st,%st(3)
-	fxch   %st(2)
-	fstpt  -0x48(%rsp)
-	fldt   0xbc98(%rip)        
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
+	fstpt  -0x28(%rsp)
+	fldt   0xbcae(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(1),%st
 	fmul   %st(5),%st
 	fld1
 	faddp  %st,%st(1)
-	fldt   0xbc98(%rip)        
+	fldt   0xbcae(%rip)        
 	fmul   %st(6),%st
-	fld    %st(2)
-	fxch   %st(1)
-	faddp  %st,%st(3)
-	fxch   %st(2)
+	fadd   %st(2),%st
 	fmul   %st(6),%st
-	fldt   0xbc96(%rip)        
+	fldt   0xbcb2(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(6),%st
 	fadd   %st(2),%st
 	fdivrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   -0x48(%rsp)
+	fldt   -0x28(%rsp)
 	fmul   %st(3),%st
 	faddp  %st,%st(1)
-	fldt   0xbc2e(%rip)        
+	fldt   0xbc4a(%rip)        
 	fmul   %st(6),%st
-	fldt   0xbc26(%rip)        
+	fldt   0xbc42(%rip)        
 	fadd   %st(1),%st
 	fmul   %st(7),%st
 	faddp  %st,%st(3)
 	fldt   -0x18(%rsp)
 	fdivp  %st,%st(3)
 	fxch   %st(5)
 	fmulp  %st,%st(2)
 	fld1
 	fsubr  %st,%st(5)
 	fxch   %st(5)
 	fmul   %st(6),%st
 	faddp  %st,%st(5)
 	fxch   %st(4)
 	fmul   %st(5),%st
-	fldt   0xbc02(%rip)        
+	fldt   0xbc1e(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xbc5a(%rip)        
-	fmul   %st(6),%st
-	fldt   0xbc52(%rip)        
+	fstpt  -0x18(%rsp)
+	fldt   0xbc72(%rip)        
+	fld    %st(5)
+	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xbc58(%rip)        
+	fmul   %st(5),%st
+	fldt   0xbc74(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmulp  %st,%st(6)
-	fxch   %st(5)
-	fadds  -0x2c(%rsp)
-	fdivrp %st,%st(5)
-	fxch   %st(1)
-	fmulp  %st,%st(4)
-	fldt   -0x48(%rsp)
+	fmulp  %st,%st(5)
+	fldz
+	faddp  %st,%st(5)
+	fldt   -0x18(%rsp)
+	fdivp  %st,%st(5)
+	fxch   %st(4)
+	fmulp  %st,%st(1)
+	fldt   -0x28(%rsp)
 	fmulp  %st,%st(2)
-	fxch   %st(1)
-	faddp  %st,%st(3)
+	faddp  %st,%st(1)
 	test   %esi,%esi
-	jle    14d8 <polyreg2+0x198>
-	fldt   -0x28(%rsp)
+	jle    14b0 <polyreg2+0x180>
+	fldt   -0x38(%rsp)
 	movslq %esi,%rsi
 	xor    %eax,%eax
-	nopl   (%rax)
-	mov    %eax,-0x48(%rsp)
-	fildl  -0x48(%rsp)
+	nopl   0x0(%rax)
+	mov    %eax,-0x38(%rsp)
+	fildl  -0x38(%rsp)
 	fmul   %st(1),%st
 	fld1
 	fsubrp %st,%st(1)
-	fld    %st(4)
+	fld    %st(2)
 	fmul   %st(1),%st
-	fadd   %st(3),%st
+	fadd   %st(5),%st
 	fmulp  %st,%st(1)
 	fadd   %st(3),%st
 	fsubrl (%rdi,%rax,8)
 	fstpl  (%rdx,%rax,8)
 	add    $0x1,%rax
-	cmp    %rsi,%rax
-	jne    14a8 <polyreg2+0x168>
+	cmp    %rax,%rsi
+	jne    1480 <polyreg2+0x150>
 	fstp   %st(0)
 	fxch   %st(1)
-	jmp    14da <polyreg2+0x19a>
+	jmp    14b2 <polyreg2+0x182>
 	nopl   (%rax)
 	fxch   %st(1)
-	fstpl  -0x48(%rsp)
-	movsd  -0x48(%rsp),%xmm0
-	fstpl  -0x48(%rsp)
-	movhpd -0x48(%rsp),%xmm0
-	fstpl  0x10(%r8)
-	movups %xmm0,(%r8)
+	fstpl  -0x38(%rsp)
+	fxch   %st(1)
+	movsd  -0x38(%rsp),%xmm0
+	fstpl  -0x38(%rsp)
+	movhpd -0x38(%rsp),%xmm0
+	fstpl  0x10(%rcx)
+	movups %xmm0,(%rcx)
 	ret
-	nopw   0x0(%rax,%rax,1)
+	nop
 	fstp   %st(0)
 	fstp   %st(0)
-	pxor   %xmm2,%xmm2
-	movss  %xmm2,-0x2c(%rsp)
-	flds   -0x2c(%rsp)
+	fldz
 	fld    %st(0)
 	fld    %st(1)
 	fxch   %st(1)
-	jmp    13b4 <polyreg2+0x74>
-	nopl   (%rax)
+	jmp    1394 <polyreg2+0x64>
+	data16 cs nopw 0x0(%rax,%rax,1)
+	nopl   0x0(%rax)
 
-0000000000001520 <polyreg3>:
+00000000000014f0 <polyreg3>:
 polyreg3():
-	mov    %esi,-0x68(%rsp)
-	fildl  -0x68(%rsp)
-	mov    %rcx,%r8
+	mov    %esi,-0x58(%rsp)
+	fildl  -0x58(%rsp)
 	fld1
 	fld    %st(1)
 	fsub   %st(1),%st
-	fdivrs 0xbaf9(%rip)        
+	fdivrs 0xbb2c(%rip)        
 	fld    %st(0)
 	fstpt  -0x18(%rsp)
 	test   %esi,%esi
-	jle    1828 <polyreg3+0x308>
-	pxor   %xmm1,%xmm1
-	movslq %esi,%rcx
+	jle    17e8 <polyreg3+0x2f8>
+	fldz
+	movslq %esi,%r8
 	xor    %eax,%eax
-	movss  %xmm1,-0x4c(%rsp)
-	flds   -0x4c(%rsp)
 	fld    %st(0)
 	fld    %st(1)
 	fld    %st(2)
 	fxch   %st(6)
 	fstpt  -0x48(%rsp)
-	nopl   0x0(%rax)
-	mov    %eax,-0x68(%rsp)
-	fildl  -0x68(%rsp)
+	nopl   (%rax)
+	mov    %eax,-0x58(%rsp)
+	fildl  -0x58(%rsp)
 	fmul   %st(4),%st
 	fsub   %st(5),%st
 	fldl   (%rdi,%rax,8)
 	add    $0x1,%rax
 	fadd   %st,%st(4)
 	fmul   %st(1),%st
 	fadd   %st,%st(7)
 	fmul   %st(1),%st
 	fadd   %st,%st(2)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(2)
-	cmp    %rax,%rcx
-	jne    1568 <polyreg3+0x48>
+	cmp    %rax,%r8
+	jne    1528 <polyreg3+0x38>
 	fstp   %st(4)
 	fstp   %st(2)
 	fxch   %st(2)
 	fldt   -0x48(%rsp)
-	fxch   %st(4)
-	fstpt  -0x38(%rsp)
-	fld    %st(3)
-	fmuls  0xba8e(%rip)        
+	fxch   %st(3)
+	fstpt  -0x58(%rsp)
+	fld    %st(2)
+	fmuls  0xbace(%rip)        
 	fld1
 	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xbc5e(%rip)        
+	fsubrp %st,%st(1)
+	fldt   0xbae6(%rip)        
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xbc2e(%rip)        
+	fldt   0xbae8(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xbab6(%rip)        
-	fmul   %st(5),%st
-	flds   -0x4c(%rsp)
+	fmul   %st(4),%st
+	fldz
 	fadd   %st,%st(1)
+	fxch   %st(2)
+	fdivp  %st,%st(1)
+	fldt   0xbae6(%rip)        
+	fmul   %st(5),%st
+	faddp  %st,%st(2)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fldt   0xbab4(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	fadd   %st(1),%st
-	fdivrp %st,%st(2)
-	fxch   %st(1)
-	fstpt  -0x68(%rsp)
-	fldt   0xbab0(%rip)        
+	fmul   %st(4),%st
+	fld1
+	faddp  %st,%st(1)
+	fldt   0xbae4(%rip)        
 	fmul   %st(5),%st
-	fadd   %st(1),%st
+	fldz
+	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fld1
+	fldt   0xbae6(%rip)        
 	faddp  %st,%st(1)
-	fldt   0xbab0(%rip)        
-	fmul   %st(6),%st
-	fadd   %st(2),%st
-	fmul   %st(6),%st
-	fldt   0xbab4(%rip)        
+	fmul   %st(5),%st
+	fldz
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(2)
-	fdivp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   -0x68(%rsp)
+	fdivrp %st,%st(1)
+	fldt   -0x58(%rsp)
+	fmulp  %st,%st(1)
+	fxch   %st(1)
+	fld    %st(0)
+	fstpt  -0x38(%rsp)
 	fmul   %st(2),%st
 	faddp  %st,%st(1)
-	fstpt  -0x28(%rsp)
-	fldt   0xbac8(%rip)        
-	fmul   %st(4),%st
-	fldt   0xbad0(%rip)        
+	fstpt  -0x48(%rsp)
+	fldt   0xbaf0(%rip)        
+	fmul   %st(3),%st
+	fldt   0xbaf8(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xbad6(%rip)        
+	fmul   %st(3),%st
+	fldt   0xbafe(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xbadc(%rip)        
+	fmul   %st(3),%st
+	fldt   0xbb04(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(3),%st
 	fld1
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xba1c(%rip)        
-	fsubr  %st,%st(1)
-	fldt   0xbad4(%rip)        
-	fld    %st(6)
+	fmul   %st(3),%st
+	fldt   0xba44(%rip)        
+	fsubrp %st,%st(1)
+	fldt   0xbafc(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xbad6(%rip)        
+	fmul   %st(4),%st
+	fldt   0xbafe(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xbad6(%rip)        
+	fmul   %st(4),%st
+	fldt   0xbafe(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fadds  -0x4c(%rsp)
-	fdivrp %st,%st(2)
-	fxch   %st(1)
-	fstpt  -0x48(%rsp)
-	fldt   0xbaca(%rip)        
-	fld    %st(5)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fldt   0xbaf8(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xbacc(%rip)        
+	fmul   %st(4),%st
+	fldt   0xbafa(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
 	fld1
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fldt   0xbac2(%rip)        
-	fld    %st(6)
+	fldt   0xbaf0(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xbac4(%rip)        
+	fmul   %st(5),%st
+	fldt   0xbaf2(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0xbac4(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xbaf2(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fadds  -0x4c(%rsp)
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   -0x38(%rsp)
-	fmulp  %st,%st(1)
-	fldt   -0x48(%rsp)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
+	fxch   %st(1)
+	fld    %st(0)
+	fstpt  -0x28(%rsp)
+	fmul   %st(3),%st
 	faddp  %st,%st(1)
-	fld    %st(5)
-	fmul   %st(2),%st
+	fldt   0xb99e(%rip)        
+	fmul   %st(4),%st
 	fld1
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(2)
-	fldt   0xb9be(%rip)        
-	fld    %st(6)
-	fmul   %st(1),%st
+	fmul   %st(4),%st
+	fldt   0xb98a(%rip)        
+	fsubrp %st,%st(1)
+	fldt   0xb9e2(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb9da(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xb9c0(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb9e0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fadds  -0x4c(%rsp)
-	fdivrp %st,%st(2)
-	fxch   %st(1)
-	fmulp  %st,%st(2)
-	fldt   -0x68(%rsp)
-	fmulp  %st,%st(4)
-	fxch   %st(3)
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldz
 	faddp  %st,%st(1)
-	fldt   0xba6c(%rip)        
+	fdivrp %st,%st(1)
+	fmulp  %st,%st(2)
+	fldt   -0x38(%rsp)
+	fldt   -0x58(%rsp)
+	fmulp  %st,%st(1)
+	faddp  %st,%st(2)
+	fldt   0xba8c(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
-	fldt   0xbaa2(%rip)        
+	fldt   0xbac2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
 	fld1
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xba8c(%rip)        
+	fldt   0xbaac(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fldt   0xba50(%rip)        
+	fldt   0xba70(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xba52(%rip)        
+	fldt   0xba72(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xba52(%rip)        
+	fldt   0xba72(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmulp  %st,%st(5)
-	fxch   %st(4)
-	fadds  -0x4c(%rsp)
-	fdivrp %st,%st(4)
+	fldz
+	faddp  %st,%st(5)
+	fdivp  %st,%st(4)
 	fxch   %st(3)
-	fmulp  %st,%st(1)
-	fldt   -0x48(%rsp)
-	fldt   -0x38(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
+	fmulp  %st,%st(2)
+	fldt   -0x28(%rsp)
+	fmulp  %st,%st(4)
+	fxch   %st(1)
+	faddp  %st,%st(3)
 	test   %esi,%esi
-	jle    17e7 <polyreg3+0x2c7>
+	jle    17af <polyreg3+0x2bf>
 	fldt   -0x18(%rsp)
 	movslq %esi,%rsi
 	xor    %eax,%eax
-	fldt   -0x28(%rsp)
-	nopl   0x0(%rax)
-	mov    %eax,-0x68(%rsp)
-	fildl  -0x68(%rsp)
+	fldt   -0x48(%rsp)
+	nopl   (%rax)
+	mov    %eax,-0x58(%rsp)
+	fildl  -0x58(%rsp)
 	fmul   %st(2),%st
 	fld1
 	fsubrp %st,%st(1)
-	fld    %st(3)
+	fld    %st(5)
 	fmul   %st(1),%st
-	fadd   %st(6),%st
+	fadd   %st(4),%st
 	fmul   %st(1),%st
 	fadd   %st(5),%st
 	fmulp  %st,%st(1)
 	fadd   %st(1),%st
 	fsubrl (%rdi,%rax,8)
 	fstpl  (%rdx,%rax,8)
 	add    $0x1,%rax
-	cmp    %rsi,%rax
-	jne    17b8 <polyreg3+0x298>
+	cmp    %rax,%rsi
+	jne    1780 <polyreg3+0x290>
 	fstp   %st(0)
 	fstp   %st(0)
-	fldt   -0x28(%rsp)
-	fstpl  -0x68(%rsp)
-	fxch   %st(1)
-	movsd  -0x68(%rsp),%xmm0
-	fstpl  -0x68(%rsp)
+	fldt   -0x48(%rsp)
+	fstpl  -0x58(%rsp)
 	fxch   %st(1)
-	movhpd -0x68(%rsp),%xmm0
-	fstpl  -0x68(%rsp)
-	movups %xmm0,(%r8)
-	movsd  -0x68(%rsp),%xmm0
-	fstpl  -0x68(%rsp)
-	movhpd -0x68(%rsp),%xmm0
-	movups %xmm0,0x10(%r8)
+	movsd  -0x58(%rsp),%xmm0
+	fstpl  -0x58(%rsp)
+	movhpd -0x58(%rsp),%xmm0
+	fstpl  -0x58(%rsp)
+	movups %xmm0,(%rcx)
+	movsd  -0x58(%rsp),%xmm0
+	fstpl  -0x58(%rsp)
+	movhpd -0x58(%rsp),%xmm0
+	movups %xmm0,0x10(%rcx)
 	ret
-	nopl   0x0(%rax)
+	nopl   (%rax)
 	fstp   %st(0)
 	fstp   %st(0)
-	pxor   %xmm2,%xmm2
-	movss  %xmm2,-0x4c(%rsp)
-	flds   -0x4c(%rsp)
+	fldz
 	fld    %st(0)
 	fld    %st(1)
 	fld    %st(2)
-	fstpt  -0x38(%rsp)
-	jmp    159e <polyreg3+0x7e>
-	nopl   0x0(%rax)
+	fstpt  -0x58(%rsp)
+	fxch   %st(2)
+	fxch   %st(3)
+	fxch   %st(2)
+	jmp    155e <polyreg3+0x6e>
+	data16 cs nopw 0x0(%rax,%rax,1)
+	xchg   %ax,%ax
 
-0000000000001850 <polyreg4>:
+0000000000001810 <polyreg4>:
 polyreg4():
-	sub    $0x40,%rsp
-	mov    %rcx,%r8
-	mov    %esi,-0x70(%rsp)
-	fildl  -0x70(%rsp)
+	sub    $0x20,%rsp
+	mov    %esi,-0x78(%rsp)
+	fildl  -0x78(%rsp)
 	fld1
 	fld    %st(1)
 	fsub   %st(1),%st
-	fdivrs 0xb7c5(%rip)        
-	fstpt  -0x58(%rsp)
+	fdivrs 0xb808(%rip)        
+	fstpt  -0x68(%rsp)
 	test   %esi,%esi
-	jle    1da0 <polyreg4+0x550>
-	pxor   %xmm1,%xmm1
-	movslq %esi,%rcx
+	jle    1d50 <polyreg4+0x540>
+	fldz
+	movslq %esi,%r8
 	xor    %eax,%eax
-	movss  %xmm1,-0x70(%rsp)
-	flds   -0x70(%rsp)
 	fld    %st(0)
 	fld    %st(1)
 	fld    %st(2)
 	fld    %st(3)
 	fxch   %st(6)
-	fstpt  -0x48(%rsp)
-	nopl   0x0(%rax,%rax,1)
-	mov    %eax,-0x68(%rsp)
-	fildl  -0x68(%rsp)
-	fldt   -0x58(%rsp)
+	fstpt  -0x58(%rsp)
+	nopl   0x0(%rax)
+	mov    %eax,-0x78(%rsp)
+	fildl  -0x78(%rsp)
+	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
 	fsub   %st(5),%st
 	fldl   (%rdi,%rax,8)
 	add    $0x1,%rax
 	fadd   %st,%st(5)
 	fmul   %st(1),%st
 	fadd   %st,%st(7)
 	fmul   %st(1),%st
 	fadd   %st,%st(2)
 	fmul   %st(1),%st
 	fadd   %st,%st(3)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(3)
-	cmp    %rax,%rcx
-	jne    18a0 <polyreg4+0x50>
+	cmp    %rax,%r8
+	jne    1850 <polyreg4+0x40>
 	fstp   %st(4)
 	fxch   %st(1)
 	fxch   %st(2)
 	fxch   %st(3)
-	fldt   -0x48(%rsp)
+	fldt   -0x58(%rsp)
 	fxch   %st(4)
-	fstpt  -0x48(%rsp)
-	fstpt  -0x38(%rsp)
-	fxch   %st(1)
-	fstpt  -0x28(%rsp)
-	fldt   0xb7f0(%rip)        
-	fmul   %st(2),%st
-	fldt   0xb8f8(%rip)        
-	fadd   %st(1),%st
+	fstpt  -0x78(%rsp)
+	fxch   %st(2)
+	fstpt  -0x58(%rsp)
+	fldt   0xb834(%rip)        
 	fmul   %st(3),%st
-	fldt   0xb80e(%rip)        
+	fldt   0xb93c(%rip)        
+	fadd   %st(1),%st
+	fmul   %st(4),%st
+	fldt   0xb852(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fsubs  0xb724(%rip)        
-	fmul   %st(3),%st
+	fmul   %st(4),%st
+	fsubs  0xb778(%rip)        
+	fmul   %st(4),%st
 	fld1
-	fadd   %st,%st(1)
-	fldt   0xb8e8(%rip)        
+	faddp  %st,%st(1)
+	fldt   0xb92c(%rip)        
 	fmul   %st(5),%st
-	fadds  -0x70(%rsp)
+	fldz
+	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb8ea(%rip)        
+	fldt   0xb92e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x70(%rsp)
+	fldz
+	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb8ea(%rip)        
+	fldt   0xb92e(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x70(%rsp)
-	fdivrp %st,%st(2)
-	fxch   %st(1)
-	fstpt  -0x18(%rsp)
-	fldt   0xb8e4(%rip)        
-	fmul   %st(4),%st
-	fldt   0xb8ec(%rip)        
-	fsubr  %st,%st(1)
-	fxch   %st(1)
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  -0x48(%rsp)
+	fldt   0xb92a(%rip)        
+	fld    %st(4)
+	fmul   %st(1),%st
+	fldt   0xb930(%rip)        
+	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(2),%st
+	fld1
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xb920(%rip)        
+	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xb8c8(%rip)        
 	faddp  %st,%st(1)
-	fldt   0xb8e0(%rip)        
+	fldt   0xb924(%rip)        
 	fmul   %st(5),%st
-	fadds  -0x70(%rsp)
+	fldz
+	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb8e2(%rip)        
+	fldt   0xb926(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x70(%rsp)
+	fldz
+	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb8e2(%rip)        
+	fldt   0xb926(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	flds   -0x70(%rsp)
+	fldz
 	fadd   %st,%st(1)
 	fxch   %st(2)
 	fdivp  %st,%st(1)
-	fstpt  -0x8(%rsp)
-	fldt   0xb8da(%rip)        
+	fstpt  -0x38(%rsp)
+	fldt   0xb920(%rip)        
 	fmul   %st(5),%st
 	fadd   %st(1),%st
 	fmul   %st(5),%st
-	fldt   0xb8de(%rip)        
+	fldt   0xb924(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(1),%st
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fld1
+	faddp  %st,%st(1)
+	fldt   0xb922(%rip)        
 	fmul   %st(5),%st
-	fadd   %st(2),%st
-	fldt   0xb8de(%rip)        
-	fmul   %st(6),%st
-	faddp  %st,%st(2)
-	fxch   %st(1)
+	fldz
+	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb8e0(%rip)        
+	fldt   0xb924(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x70(%rsp)
+	fldz
+	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb8e0(%rip)        
+	fldt   0xb924(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x70(%rsp)
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   -0x48(%rsp)
+	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
+	fldt   -0x48(%rsp)
+	fmul   %st(4),%st
+	faddp  %st,%st(1)
 	fldt   -0x38(%rsp)
-	fldt   -0x18(%rsp)
+	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   -0x28(%rsp)
-	fldt   -0x8(%rsp)
-	fmulp  %st,%st(1)
+	fstpt  -0x8(%rsp)
+	fldt   0xb726(%rip)        
 	faddp  %st,%st(1)
-	fstpt  -0x68(%rsp)
-	fldt   0xb6de(%rip)        
-	faddp  %st,%st(2)
-	fxch   %st(1)
 	fmul   %st(3),%st
-	fldt   0xb6e2(%rip)        
+	fldt   0xb72c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xb6e8(%rip)        
+	fldt   0xb732(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fadd   %st(1),%st
+	fld1
+	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xb62a(%rip)        
-	fsubr  %st,%st(1)
-	fldt   0xb6e2(%rip)        
-	fld    %st(5)
+	fldt   0xb672(%rip)        
+	fsubrp %st,%st(1)
+	fldt   0xb72a(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xb6e4(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb72c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb6e4(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb72c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x70(%rsp)
-	fdivrp %st,%st(2)
-	fxch   %st(1)
-	fstpt  0x8(%rsp)
-	fldt   0xb6d8(%rip)        
-	fld    %st(4)
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  -0x28(%rsp)
+	fldt   0xb722(%rip)        
+	fld    %st(3)
 	fmul   %st(1),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xb6da(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb724(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fld1
+	fadd   %st,%st(1)
+	fxch   %st(1)
 	fmul   %st(4),%st
-	fsub   %st(2),%st
-	fldt   0xb6d4(%rip)        
-	fld    %st(5)
+	fsubp  %st,%st(1)
+	fldt   0xb71a(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xb6d6(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb71c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb6d6(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb71c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fadds  -0x70(%rsp)
-	fdivrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8(%rsp)
-	fmul   %st(4),%st
 	faddp  %st,%st(1)
-	fstpt  0x28(%rsp)
-	fldt   0xb7f2(%rip)        
 	fmul   %st(4),%st
-	fldt   0xb7fa(%rip)        
+	fldz
 	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb800(%rip)        
+	fldt   -0x28(%rsp)
+	fmul   %st(2),%st
+	faddp  %st,%st(1)
+	fstpt  0x8(%rsp)
+	fldt   0xb838(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb840(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xb846(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xb806(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb84c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0xb808(%rip)        
+	fmul   %st(3),%st
+	fld1
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xb84c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xb80e(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb852(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xb814(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb858(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xb81c(%rip)        
-	fld    %st(5)
+	fldt   0xb860(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xb81e(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb862(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb81e(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb862(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb81e(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb862(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x70(%rsp)
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0x18(%rsp)
-	fldt   0xb814(%rip)        
-	fld    %st(4)
+	fstpt  -0x18(%rsp)
+	fldt   0xb858(%rip)        
+	fld    %st(3)
 	fmul   %st(1),%st
-	fldt   0xb81a(%rip)        
+	fldt   0xb85e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xb820(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fadd   %st(2),%st
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb81e(%rip)        
+	fldt   0xb864(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fldt   0xb51a(%rip)        
+	faddp  %st,%st(1)
 	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fldt   0xb81e(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb85c(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(3),%st
+	fld1
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xb4fc(%rip)        
+	fsubrp %st,%st(1)
+	fldt   0xb854(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb820(%rip)        
+	fldt   0xb856(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb820(%rip)        
+	fldt   0xb856(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb820(%rip)        
+	fldt   0xb856(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fadds  -0x70(%rsp)
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   -0x38(%rsp)
-	fmulp  %st,%st(1)
-	fldt   -0x18(%rsp)
+	fmul   %st(2),%st
 	fldt   -0x48(%rsp)
+	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   -0x28(%rsp)
-	fldt   0x18(%rsp)
+	fldt   -0x18(%rsp)
+	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0xb59c(%rip)        
-	fld    %st(4)
-	fmul   %st(1),%st
-	flds   0xb42a(%rip)        
+	fldt   0xb5d6(%rip)        
+	fmul   %st(4),%st
+	flds   0xb476(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
+	fmul   %st(5),%st
+	fld1
+	fadd   %st,%st(1)
+	fxch   %st(1)
 	fmul   %st(6),%st
-	fadd   %st(4),%st
-	fmul   %st(6),%st
-	fsub   %st(4),%st
-	fmul   %st(6),%st
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb5b2(%rip)        
+	fsubrp %st,%st(1)
+	fldt   0xb5ba(%rip)        
 	fmul   %st(5),%st
-	fsubp  %st,%st(1)
-	fldt   0xb588(%rip)        
-	fld    %st(5)
-	fmul   %st(1),%st
+	fldt   0xb5b2(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb58a(%rip)        
+	fldt   0xb5b8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb58a(%rip)        
+	fldt   0xb5b8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x70(%rsp)
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fmulp  %st,%st(3)
-	fldt   0x8(%rsp)
+	fmulp  %st,%st(2)
+	fldt   -0x28(%rsp)
 	fmulp  %st,%st(5)
-	fxch   %st(4)
-	faddp  %st,%st(2)
-	fldt   0xb798(%rip)        
+	fxch   %st(1)
+	faddp  %st,%st(4)
+	fldt   0xb7c6(%rip)        
 	fld    %st(3)
 	fmul   %st(1),%st
-	fldt   0xb79e(%rip)        
+	fldt   0xb7cc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
-	fldt   0xb7a2(%rip)        
-	fadd   %st,%st(1)
+	fldt   0xb7d0(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fld1
+	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
-	fsub   %st(4),%st
-	fmul   %st(6),%st
-	fadd   %st(4),%st
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xb7ba(%rip)        
+	fsubrp %st,%st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fldt   0xb794(%rip)        
+	fldt   0xb7ba(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb796(%rip)        
+	fldt   0xb7bc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb796(%rip)        
+	fldt   0xb7bc(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb796(%rip)        
+	fldt   0xb7bc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmulp  %st,%st(4)
-	fxch   %st(3)
-	fadds  -0x70(%rsp)
-	fdivrp %st,%st(3)
-	fldt   -0x28(%rsp)
+	fldz
+	faddp  %st,%st(4)
+	fdivp  %st,%st(3)
+	fldt   -0x58(%rsp)
 	fmulp  %st,%st(3)
-	fldt   -0x8(%rsp)
-	fldt   -0x48(%rsp)
-	fmulp  %st,%st(1)
 	fldt   -0x38(%rsp)
-	fldt   0x18(%rsp)
+	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
+	fldt   -0x18(%rsp)
+	fmulp  %st,%st(3)
+	faddp  %st,%st(2)
+	fxch   %st(2)
 	faddp  %st,%st(1)
-	faddp  %st,%st(3)
 	test   %esi,%esi
-	jle    1d50 <polyreg4+0x500>
-	fldt   -0x58(%rsp)
+	jle    1d0d <polyreg4+0x4fd>
+	fldt   -0x68(%rsp)
 	movslq %esi,%rsi
 	xor    %eax,%eax
-	fldt   0x28(%rsp)
-	nopl   0x0(%rax,%rax,1)
-	mov    %eax,-0x70(%rsp)
-	fildl  -0x70(%rsp)
-	fmul   %st(2),%st
-	fsub   %st(3),%st
-	fld    %st(5)
-	fmul   %st(1),%st
-	fadd   %st(5),%st
+	fldt   -0x8(%rsp)
+	fldt   0x8(%rsp)
+	nopl   (%rax)
+	mov    %eax,-0x78(%rsp)
+	fildl  -0x78(%rsp)
+	fmul   %st(3),%st
+	fld1
+	fsubrp %st,%st(1)
+	fld    %st(4)
 	fmul   %st(1),%st
 	fadd   %st(7),%st
 	fmul   %st(1),%st
+	fadd   %st(6),%st
+	fmul   %st(1),%st
 	fadd   %st(2),%st
 	fmulp  %st,%st(1)
-	fldt   -0x68(%rsp)
-	faddp  %st,%st(1)
+	fadd   %st(2),%st
 	fsubrl (%rdi,%rax,8)
 	fstpl  (%rdx,%rax,8)
 	add    $0x1,%rax
-	cmp    %rsi,%rax
-	jne    1d10 <polyreg4+0x4c0>
+	cmp    %rax,%rsi
+	jne    1cd8 <polyreg4+0x4c8>
 	fstp   %st(0)
 	fstp   %st(0)
 	fstp   %st(0)
-	jmp    1d52 <polyreg4+0x502>
-	nopl   0x0(%rax)
-	fstp   %st(0)
-	fldt   -0x68(%rsp)
-	fstpl  -0x70(%rsp)
-	fldt   0x28(%rsp)
-	movsd  -0x70(%rsp),%xmm0
-	fstpl  -0x70(%rsp)
-	fxch   %st(2)
-	movhpd -0x70(%rsp),%xmm0
-	fstpl  -0x70(%rsp)
+	fldt   -0x8(%rsp)
+	fstpl  -0x78(%rsp)
+	fldt   0x8(%rsp)
+	movsd  -0x78(%rsp),%xmm0
+	fstpl  -0x78(%rsp)
+	fxch   %st(1)
+	movhpd -0x78(%rsp),%xmm0
+	fstpl  -0x78(%rsp)
 	fxch   %st(1)
-	movups %xmm0,(%r8)
-	movsd  -0x70(%rsp),%xmm0
-	fstpl  -0x70(%rsp)
-	movhpd -0x70(%rsp),%xmm0
-	fstpl  0x20(%r8)
-	movups %xmm0,0x10(%r8)
-	add    $0x40,%rsp
+	movups %xmm0,(%rcx)
+	movsd  -0x78(%rsp),%xmm0
+	fstpl  -0x78(%rsp)
+	movhpd -0x78(%rsp),%xmm0
+	fstpl  0x20(%rcx)
+	movups %xmm0,0x10(%rcx)
+	add    $0x20,%rsp
 	ret
-	nopl   0x0(%rax,%rax,1)
 	fstp   %st(0)
-	pxor   %xmm2,%xmm2
-	movss  %xmm2,-0x70(%rsp)
-	flds   -0x70(%rsp)
-	fld    %st(0)
+	fldz
+	fstpt  -0x58(%rsp)
+	fldt   -0x58(%rsp)
 	fld    %st(0)
-	fstpt  -0x28(%rsp)
 	fld    %st(1)
-	fld    %st(0)
-	fstpt  -0x38(%rsp)
-	fxch   %st(2)
-	fstpt  -0x48(%rsp)
+	fld    %st(2)
+	fstpt  -0x78(%rsp)
 	fxch   %st(1)
 	fxch   %st(2)
-	fxch   %st(1)
-	jmp    18ea <polyreg4+0x9a>
+	fxch   %st(3)
+	fxch   %st(2)
+	jmp    1896 <polyreg4+0x86>
 	data16 cs nopw 0x0(%rax,%rax,1)
-	nopl   0x0(%rax)
+	xchg   %ax,%ax
 
-0000000000001de0 <polyreg5>:
+0000000000001d80 <polyreg5>:
 polyreg5():
-	sub    $0x60,%rsp
-	mov    %rcx,%r8
+	sub    $0x50,%rsp
 	mov    %esi,-0x78(%rsp)
 	fildl  -0x78(%rsp)
 	fld    %st(0)
 	fld1
 	fsubrp %st,%st(1)
-	fdivrs 0xb235(%rip)        
+	fdivrs 0xb298(%rip)        
 	fstpt  -0x48(%rsp)
 	test   %esi,%esi
-	jle    2690 <polyreg5+0x8b0>
-	pxor   %xmm1,%xmm1
-	movslq %esi,%rcx
+	jle    2610 <polyreg5+0x890>
+	fldz
+	movslq %esi,%r8
 	xor    %eax,%eax
-	movss  %xmm1,-0x38(%rsp)
-	flds   -0x38(%rsp)
 	fld    %st(0)
 	fld    %st(1)
 	fld    %st(2)
 	fld    %st(3)
-	fld    %st(0)
+	fld    %st(4)
 	fstpt  -0x78(%rsp)
 	fxch   %st(5)
 	fstpt  -0x58(%rsp)
-	xchg   %ax,%ax
+	nop
 	mov    %eax,-0x68(%rsp)
 	fildl  -0x68(%rsp)
 	fldt   -0x48(%rsp)
 	fmulp  %st,%st(1)
 	fld1
 	fsubrp %st,%st(1)
 	fldl   (%rdi,%rax,8)
-	add    $0x1,%rax
-	fadd   %st,%st(5)
-	fmul   %st(1),%st
 	fldt   -0x78(%rsp)
+	add    $0x1,%rax
 	fadd   %st(1),%st
 	fstpt  -0x78(%rsp)
 	fmul   %st(1),%st
+	fadd   %st,%st(5)
+	fmul   %st(1),%st
+	fadd   %st,%st(6)
+	fmul   %st(1),%st
 	fadd   %st,%st(2)
 	fmul   %st(1),%st
 	fadd   %st,%st(3)
-	fmul   %st(1),%st
-	fadd   %st,%st(6)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(3)
-	cmp    %rax,%rcx
-	jne    1e30 <polyreg5+0x50>
+	cmp    %rax,%r8
+	jne    1dc0 <polyreg5+0x40>
 	fldt   -0x58(%rsp)
 	fxch   %st(4)
+	fstpt  -0x38(%rsp)
+	fxch   %st(1)
 	fstpt  -0x28(%rsp)
 	fxch   %st(1)
-	fstpt  -0x58(%rsp)
-	fxch   %st(3)
 	fstpt  -0x18(%rsp)
-	fstpt  -0x8(%rsp)
-	fldt   0xb254(%rip)        
-	fmul   %st(1),%st
-	fldt   0xb35c(%rip)        
-	faddp  %st,%st(1)
-	fmul   %st(1),%st
-	fldt   0xb272(%rip)        
+	fldt   0xb2b8(%rip)        
+	fmul   %st(2),%st
+	fldt   0xb3c0(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(1),%st
-	fsubs  0xb188(%rip)        
-	fmul   %st(1),%st
-	fld1
+	fmul   %st(2),%st
+	fldt   0xb2d6(%rip)        
 	faddp  %st,%st(1)
-	fldt   0xb34c(%rip)        
 	fmul   %st(2),%st
-	flds   -0x38(%rsp)
+	flds   0xb1fc(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(2),%st
+	fld1
+	fadd   %st,%st(1)
+	fldt   0xb3ae(%rip)        
+	fmul   %st(4),%st
+	fldz
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(3),%st
-	fldt   0xb34a(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb3ae(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0xb34c(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb3b0(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fld    %st(1)
+	fmul   %st(5),%st
+	faddp  %st,%st(1)
+	fdivrp %st,%st(2)
+	fldt   0xb3b2(%rip)        
+	fld    %st(4)
+	fmul   %st(1),%st
+	fldt   0xb3b8(%rip)        
+	fsubr  %st,%st(1)
 	fxch   %st(1)
-	faddp  %st,%st(2)
+	fmul   %st(6),%st
+	faddp  %st,%st(3)
 	fxch   %st(2)
-	fdivp  %st,%st(1)
-	fldt   0xb348(%rip)        
-	fld    %st(3)
-	fmul   %st(1),%st
-	fldt   0xb34e(%rip)        
-	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fsubp  %st,%st(2)
+	fxch   %st(1)
 	fmul   %st(4),%st
-	fld1
 	faddp  %st,%st(1)
+	fldt   0xb3ae(%rip)        
 	fmul   %st(4),%st
-	fldt   0xb33e(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(4),%st
+	fldz
 	faddp  %st,%st(1)
-	fldt   0xb342(%rip)        
 	fmul   %st(4),%st
-	fld    %st(3)
-	fxch   %st(1)
-	faddp  %st,%st(4)
-	fxch   %st(3)
-	fmul   %st(4),%st
-	fldt   0xb340(%rip)        
+	fldt   0xb3b0(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0xb342(%rip)        
+	fldz
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fld    %st(3)
-	fxch   %st(1)
-	faddp  %st,%st(4)
-	fxch   %st(1)
-	fdivp  %st,%st(3)
-	fldt   0xb33e(%rip)        
-	fmul   %st(4),%st
-	fadd   %st(1),%st
+	fldt   0xb3b0(%rip)        
+	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb342(%rip)        
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(2)
+	fdivp  %st,%st(1)
+	fldt   0xb3ae(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xb3b2(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(1),%st
+	fmul   %st(5),%st
+	faddp  %st,%st(2)
+	fxch   %st(1)
 	fmul   %st(4),%st
 	fld1
 	faddp  %st,%st(1)
-	fldt   0xb340(%rip)        
+	fldt   0xb3ae(%rip)        
 	fmul   %st(5),%st
-	fld    %st(2)
-	fxch   %st(1)
-	faddp  %st,%st(3)
-	fxch   %st(2)
+	fldz
+	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb33e(%rip)        
+	fldt   0xb3b0(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(2),%st
+	fldz
+	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb340(%rip)        
+	fldt   0xb3b0(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(2),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   -0x28(%rsp)
+	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fxch   %st(2)
-	fld    %st(0)
-	fstpt  -0x38(%rsp)
-	fmul   %st(5),%st
-	faddp  %st,%st(2)
-	fxch   %st(2)
+	fld    %st(2)
+	fmul   %st(6),%st
+	faddp  %st,%st(1)
+	fxch   %st(1)
 	fld    %st(0)
-	fstpt  0x48(%rsp)
-	fldt   -0x18(%rsp)
+	fstpt  0x28(%rsp)
+	fldt   -0x28(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	fstpt  -0x68(%rsp)
-	fldt   0xb4bc(%rip)        
-	fmul   %st(2),%st
-	fldt   0xb4c4(%rip)        
+	fldt   0xb530(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb538(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xb4ca(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb53e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xb4d0(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb544(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xb4d6(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb54a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xb4dc(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb550(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xb4e2(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb556(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xb4e8(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb55c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
+	fmul   %st(3),%st
 	fld1
-	fadd   %st,%st(1)
-	fxch   %st(1)
+	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xb056(%rip)        
+	fldt   0xb0cc(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xb4de(%rip)        
+	fldt   0xb554(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb4e0(%rip)        
+	fldt   0xb556(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb4e0(%rip)        
+	fldt   0xb556(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb4e0(%rip)        
+	fldt   0xb556(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb4e0(%rip)        
+	fldt   0xb556(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0x8(%rsp)
-	fldt   0xb4d8(%rip)        
-	fmul   %st(3),%st
-	fldt   0xb4e0(%rip)        
+	fldt   0xb550(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb558(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb4e6(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb55e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb4ec(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb564(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb4f2(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb56a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb4f8(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb570(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
+	fmul   %st(4),%st
+	fld1
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xb4fa(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb570(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xb500(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb576(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xb506(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb57c(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xb50e(%rip)        
-	fld    %st(3)
+	fldt   0xb584(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb510(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb586(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb510(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb586(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb510(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb586(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb510(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb586(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldz
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(2),%st
 	fdivrp %st,%st(1)
-	fstpt  0x18(%rsp)
-	fldt   0xb508(%rip)        
-	fld    %st(2)
+	fstpt  -0x8(%rsp)
+	fldt   0xb57c(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	fsubp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xb50a(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb57e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xb50a(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb57e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xb50a(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb57e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
+	fmul   %st(4),%st
 	fld1
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fldt   0xb500(%rip)        
-	fld    %st(3)
+	fldt   0xb574(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb502(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb576(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb502(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb576(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb502(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb576(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb502(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb576(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldz
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(2),%st
 	fdivrp %st,%st(1)
-	fldt   -0x78(%rsp)
+	fldt   -0x38(%rsp)
 	fmulp  %st,%st(1)
-	fldt   -0x58(%rsp)
+	fxch   %st(1)
+	fld    %st(0)
+	fstpt  0x38(%rsp)
+	fmul   %st(3),%st
+	faddp  %st,%st(1)
+	fldt   -0x18(%rsp)
 	fld    %st(0)
-	fldt   0x8(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
 	fldt   -0x8(%rsp)
-	fldt   0x18(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(2)
 	fxch   %st(1)
 	fstpt  -0x58(%rsp)
-	fldt   0xb0f8(%rip)        
-	fmul   %st(3),%st
-	fldt   0xb100(%rip)        
+	fldt   0xb16a(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb172(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb106(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb178(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb10c(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb17e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
+	fmul   %st(4),%st
 	fld1
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb10c(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb17e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb112(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb184(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb118(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb18a(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xb120(%rip)        
-	fld    %st(4)
+	fldt   0xb192(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xb122(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb194(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xb122(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb194(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xb122(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb194(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fmul   %st(5),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0x28(%rsp)
-	fldt   0xb11a(%rip)        
-	fld    %st(3)
+	fstpt  0x8(%rsp)
+	fldt   0xb18a(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
-	fldt   0xb120(%rip)        
+	fldt   0xb190(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xb126(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb196(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaddc(%rip)        
-	fadd   %st,%st(1)
-	fxch   %st(1)
 	fmul   %st(5),%st
-	fsubp  %st,%st(2)
-	fxch   %st(1)
+	fldt   0xae4c(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb11a(%rip)        
+	fldt   0xb18e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
 	fld1
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fsubp  %st,%st(1)
-	fldt   0xb118(%rip)        
-	fld    %st(4)
+	fldt   0xae2e(%rip)        
+	fsubrp %st,%st(1)
+	fldt   0xb186(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xb11a(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb188(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xb11a(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb188(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xb11a(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb188(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fmul   %st(5),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   -0x38(%rsp)
+	fmul   %st(5),%st
+	fldt   -0x78(%rsp)
+	fmulp  %st,%st(3)
+	faddp  %st,%st(2)
+	fldt   0x8(%rsp)
 	fldt   -0x28(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x28(%rsp)
-	fldt   -0x18(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0xb3ac(%rip)        
+	faddp  %st,%st(2)
+	fldt   0xb41c(%rip)        
 	fmul   %st(4),%st
-	fldt   0xb3b4(%rip)        
+	fldt   0xb424(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
-	fldt   0xb3b8(%rip)        
+	fldt   0xb428(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb3b8(%rip)        
+	fldt   0xb428(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb3be(%rip)        
+	fldt   0xb42e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
 	fld1
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb3be(%rip)        
+	fldt   0xb42e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb3c4(%rip)        
+	fldt   0xb434(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fldt   0xb3c8(%rip)        
+	fldt   0xb438(%rip)        
 	fmul   %st(5),%st
-	fldt   0xb3c0(%rip)        
+	fldt   0xb430(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb3c6(%rip)        
+	fldt   0xb436(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb3c6(%rip)        
+	fldt   0xb436(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb3c6(%rip)        
+	fldt   0xb436(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb3c6(%rip)        
+	fldt   0xb436(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0x38(%rsp)
-	fldt   0xb3be(%rip)        
+	fstpt  0x18(%rsp)
+	fldt   0xb42c(%rip)        
 	fmul   %st(4),%st
-	fldt   0xb3c6(%rip)        
+	fldt   0xb434(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb3cc(%rip)        
+	fldt   0xb43a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb3d2(%rip)        
+	fldt   0xb440(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb3d8(%rip)        
+	fldt   0xb446(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb3de(%rip)        
+	fldt   0xb44c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
 	fld1
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb3de(%rip)        
+	fldt   0xb44c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb3e4(%rip)        
+	fldt   0xb452(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xb3ea(%rip)        
+	fldt   0xb458(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xb3f2(%rip)        
+	fldt   0xb460(%rip)        
 	fmul   %st(5),%st
-	fldt   0xb3ea(%rip)        
+	fldt   0xb458(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb3f0(%rip)        
+	fldt   0xb45e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb3f0(%rip)        
+	fldt   0xb45e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb3f0(%rip)        
+	fldt   0xb45e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb3f0(%rip)        
+	fldt   0xb45e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fxch   %st(4)
-	fsts   -0x38(%rsp)
-	faddp  %st,%st(4)
-	fdivp  %st,%st(3)
-	fld    %st(1)
-	fmulp  %st,%st(3)
-	fldt   0x8(%rsp)
-	fldt   -0x78(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(3)
-	fldt   -0x8(%rsp)
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fmul   %st(3),%st
 	fldt   0x38(%rsp)
+	fldt   -0x38(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(3)
-	fldt   0xaf7a(%rip)        
+	faddp  %st,%st(1)
+	fldt   0x18(%rsp)
+	fmulp  %st,%st(2)
+	faddp  %st,%st(1)
+	fldt   0xaff2(%rip)        
 	fmul   %st(4),%st
-	fldt   0xaf82(%rip)        
+	fldt   0xaffa(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xaf88(%rip)        
-	fadd   %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(5),%st
+	fldt   0xb000(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
 	fld1
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fsubp  %st,%st(1)
+	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xaf5c(%rip)        
+	fldt   0xafea(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xafd0(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xaf42(%rip)        
+	fldt   0xafb6(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xaf6a(%rip)        
+	fldt   0xafde(%rip)        
 	fmul   %st(5),%st
-	fldt   0xaf62(%rip)        
+	fldt   0xafd6(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xaf68(%rip)        
+	fldt   0xafdc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xaf68(%rip)        
+	fldt   0xafdc(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xaf68(%rip)        
+	fldt   0xafdc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x38(%rsp)
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   -0x18(%rsp)
-	fmulp  %st,%st(1)
-	fldt   0x48(%rsp)
 	fldt   -0x28(%rsp)
 	fmulp  %st,%st(1)
 	fldt   0x28(%rsp)
+	fldt   -0x78(%rsp)
+	fmulp  %st,%st(1)
+	fldt   0x8(%rsp)
 	fmulp  %st,%st(7)
 	faddp  %st,%st(6)
 	faddp  %st,%st(5)
-	fldt   0xb328(%rip)        
+	fldt   0xb39c(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
-	fldt   0xb32e(%rip)        
+	fldt   0xb3a2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xacb4(%rip)        
+	fldt   0xad28(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xacfa(%rip)        
+	fldt   0xad6e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
 	fld1
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xace4(%rip)        
+	fldt   0xad58(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xac8a(%rip)        
+	fldt   0xacfe(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb2f0(%rip)        
+	fldt   0xb364(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fldt   0xb2f4(%rip)        
-	fld    %st(5)
-	fmul   %st(1),%st
+	fldt   0xb368(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb360(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb2f6(%rip)        
+	fldt   0xb366(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb2f6(%rip)        
+	fldt   0xb366(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb2f6(%rip)        
+	fldt   0xb366(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xb2f6(%rip)        
+	fldt   0xb366(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmulp  %st,%st(5)
-	fxch   %st(4)
-	fadds  -0x38(%rsp)
-	fdivrp %st,%st(4)
-	fldt   -0x8(%rsp)
+	fldz
+	faddp  %st,%st(5)
+	fdivp  %st,%st(4)
+	fldt   -0x18(%rsp)
 	fmulp  %st,%st(4)
-	fldt   0x18(%rsp)
-	fldt   -0x78(%rsp)
+	fldt   -0x8(%rsp)
+	fldt   -0x38(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x38(%rsp)
-	fmulp  %st,%st(3)
-	faddp  %st,%st(2)
+	fldt   0x18(%rsp)
+	fmulp  %st,%st(4)
+	faddp  %st,%st(3)
 	fxch   %st(3)
-	faddp  %st,%st(1)
+	faddp  %st,%st(2)
 	test   %esi,%esi
-	jle    2635 <polyreg5+0x855>
+	jle    25b5 <polyreg5+0x835>
 	fldt   -0x48(%rsp)
 	movslq %esi,%rsi
 	xor    %eax,%eax
-	nopl   (%rax)
+	nopl   0x0(%rax,%rax,1)
 	mov    %eax,-0x78(%rsp)
 	fildl  -0x78(%rsp)
 	fmul   %st(1),%st
 	fld1
 	fsubrp %st,%st(1)
-	fld    %st(2)
+	fld    %st(3)
 	fmul   %st(1),%st
 	fadd   %st(6),%st
 	fmul   %st(1),%st
-	fadd   %st(4),%st
-	fmul   %st(1),%st
 	fadd   %st(5),%st
 	fmul   %st(1),%st
+	fadd   %st(3),%st
+	fmul   %st(1),%st
 	fldt   -0x58(%rsp)
 	faddp  %st,%st(1)
 	fmulp  %st,%st(1)
 	fldt   -0x68(%rsp)
 	faddp  %st,%st(1)
 	fsubrl (%rdi,%rax,8)
 	fstpl  (%rdx,%rax,8)
 	add    $0x1,%rax
-	cmp    %rsi,%rax
-	jne    25f8 <polyreg5+0x818>
+	cmp    %rax,%rsi
+	jne    2578 <polyreg5+0x7f8>
 	fstp   %st(0)
 	fldt   -0x68(%rsp)
 	fstpl  -0x78(%rsp)
 	fldt   -0x58(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	fxch   %st(2)
 	movhpd -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	movups %xmm0,(%r8)
+	fxch   %st(1)
+	movups %xmm0,(%rcx)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	fxch   %st(1)
 	movhpd -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	movups %xmm0,0x10(%r8)
+	movups %xmm0,0x10(%rcx)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	movups %xmm0,0x20(%r8)
-	add    $0x60,%rsp
+	movups %xmm0,0x20(%rcx)
+	add    $0x50,%rsp
 	ret
-	pxor   %xmm2,%xmm2
-	movss  %xmm2,-0x38(%rsp)
-	flds   -0x38(%rsp)
-	fld    %st(0)
-	fld    %st(0)
-	fstpt  -0x8(%rsp)
-	fxch   %st(1)
+	nopl   (%rax)
+	fldz
 	fstpt  -0x18(%rsp)
 	fldt   -0x18(%rsp)
-	fxch   %st(1)
+	fstpt  -0x28(%rsp)
+	fldt   -0x28(%rsp)
 	fld    %st(0)
-	fstpt  -0x58(%rsp)
 	fld    %st(1)
+	fstpt  -0x38(%rsp)
+	fldt   -0x38(%rsp)
 	fstpt  -0x78(%rsp)
 	fxch   %st(1)
-	fstpt  -0x28(%rsp)
+	fxch   %st(2)
 	fxch   %st(1)
-	jmp    1e86 <polyreg5+0xa6>
-	nopl   0x0(%rax,%rax,1)
+	jmp    1e12 <polyreg5+0x92>
+	nopl   (%rax)
 
-00000000000026d0 <polyreg6>:
+0000000000002640 <polyreg6>:
 polyreg6():
 	sub    $0xa0,%rsp
-	mov    %rcx,%r8
 	mov    %esi,-0x78(%rsp)
 	fildl  -0x78(%rsp)
 	fld    %st(0)
 	fld1
 	fsubrp %st,%st(1)
-	fdivrs 0xa942(%rip)        
-	fstpt  -0x28(%rsp)
+	fdivrs 0xa9d5(%rip)        
+	fstpt  -0x58(%rsp)
 	test   %esi,%esi
-	jle    3420 <polyreg6+0xd50>
-	pxor   %xmm1,%xmm1
-	movslq %esi,%rcx
+	jle    3350 <polyreg6+0xd10>
+	fldz
+	movslq %esi,%r8
 	xor    %eax,%eax
-	movss  %xmm1,-0x18(%rsp)
-	flds   -0x18(%rsp)
 	fld    %st(0)
 	fld    %st(1)
 	fld    %st(2)
 	fld    %st(3)
-	fld    %st(0)
+	fld    %st(4)
 	fstpt  -0x68(%rsp)
-	fld    %st(0)
+	fldt   -0x68(%rsp)
 	fstpt  -0x78(%rsp)
 	fxch   %st(5)
-	fstpt  -0x48(%rsp)
+	fstpt  -0x38(%rsp)
 	nopw   0x0(%rax,%rax,1)
-	mov    %eax,-0x58(%rsp)
-	fildl  -0x58(%rsp)
-	fldt   -0x28(%rsp)
+	mov    %eax,-0x48(%rsp)
+	fildl  -0x48(%rsp)
+	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
 	fld1
 	fsubrp %st,%st(1)
 	fldl   (%rdi,%rax,8)
 	fldt   -0x78(%rsp)
 	add    $0x1,%rax
 	fadd   %st(1),%st
@@ -1946,5159 +1946,5143 @@
 	fmul   %st(1),%st
 	fldt   -0x68(%rsp)
 	fadd   %st(1),%st
 	fstpt  -0x68(%rsp)
 	fmul   %st(1),%st
 	fadd   %st,%st(5)
 	fmul   %st(1),%st
-	fadd   %st,%st(2)
-	fmul   %st(1),%st
 	fadd   %st,%st(6)
 	fmul   %st(1),%st
+	fadd   %st,%st(2)
+	fmul   %st(1),%st
 	fadd   %st,%st(3)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(3)
-	cmp    %rax,%rcx
-	jne    2730 <polyreg6+0x60>
-	fldt   -0x48(%rsp)
+	cmp    %rax,%r8
+	jne    2690 <polyreg6+0x50>
+	fldt   -0x38(%rsp)
 	fxch   %st(4)
-	fstpt  -0x58(%rsp)
-	fstpt  0x18(%rsp)
-	fxch   %st(3)
-	fstpt  -0x8(%rsp)
+	fstpt  -0x18(%rsp)
+	fxch   %st(1)
 	fstpt  0x8(%rsp)
-	fldt   0xb12a(%rip)        
-	fmul   %st(1),%st
-	fldt   0xb132(%rip)        
+	fxch   %st(1)
+	fstpt  -0x8(%rsp)
+	fldt   0xb1bc(%rip)        
+	fmul   %st(2),%st
+	fldt   0xb1c4(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(1),%st
-	fldt   0xb138(%rip)        
+	fmul   %st(2),%st
+	fldt   0xb1ca(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(1),%st
-	fldt   0xb13e(%rip)        
+	fmul   %st(2),%st
+	fldt   0xb1d0(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(1),%st
-	fldt   0xb144(%rip)        
+	fmul   %st(2),%st
+	fldt   0xb1d6(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(1),%st
+	fmul   %st(2),%st
 	fld1
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(2),%st
-	fsubs  0xa86a(%rip)        
-	fldt   0xb13c(%rip)        
 	fmul   %st(3),%st
-	flds   -0x18(%rsp)
+	fsubs  0xa90c(%rip)        
+	fldt   0xb1ce(%rip)        
+	fmul   %st(4),%st
+	fldz
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
-	fldt   0xb13a(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb1ce(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fadd   %st(1),%st
-	fmul   %st(4),%st
-	fldt   0xb13c(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb1d0(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fadd   %st(1),%st
-	fmul   %st(4),%st
-	fldt   0xb13e(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb1d2(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fadd   %st(1),%st
 	fdivrp %st,%st(2)
 	fxch   %st(1)
-	fstpt  -0x38(%rsp)
-	fldt   0xb13a(%rip)        
-	fmul   %st(3),%st
-	fldt   0xb142(%rip)        
+	fstpt  -0x28(%rsp)
+	fldt   0xb1ce(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb1d6(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb148(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb1dc(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb14e(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb1e2(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xb154(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb1e8(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fsubs  0xa7f2(%rip)        
-	fldt   0xb150(%rip)        
 	fmul   %st(4),%st
 	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fldt   0xb154(%rip)        
+	fsubs  0xa896(%rip)        
+	fldt   0xb1e4(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xb1e8(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0xb156(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb1ea(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0xb158(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb1ec(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
 	fdivrp %st,%st(1)
-	fstpt  0x28(%rsp)
-	fldt   0xb156(%rip)        
-	fmul   %st(3),%st
-	fldt   0xb15e(%rip)        
+	fstpt  0x18(%rsp)
+	fldt   0xb1ea(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb1f2(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
-	flds   0xa7a2(%rip)        
+	fmul   %st(5),%st
+	flds   0xa846(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
+	fmul   %st(6),%st
+	fadd   %st(4),%st
+	fmul   %st(6),%st
+	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	faddp  %st,%st(4)
-	fxch   %st(3)
+	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fsubp  %st,%st(3)
-	fxch   %st(2)
-	fmul   %st(3),%st
-	faddp  %st,%st(2)
-	fxch   %st(1)
-	fmul   %st(2),%st
-	fldt   0xb144(%rip)        
+	fldt   0xb1de(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xb14c(%rip)        
-	fmul   %st(3),%st
+	fldt   0xb1e6(%rip)        
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fldt   0xb150(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb1ea(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fldt   0xb152(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb1ec(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fldt   0xb154(%rip)        
+	fmul   %st(5),%st
+	fldt   0xb1ee(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
 	fdivrp %st,%st(1)
-	fldt   0xb156(%rip)        
-	fmul   %st(3),%st
-	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fldt   0xb15a(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fldt   0xb152(%rip)        
-	fsubrp %st,%st(1)
-	fldt   0xb15a(%rip)        
+	fstpt  0x28(%rsp)
+	fldt   0xb1ec(%rip)        
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0xb15e(%rip)        
+	fldt   0xb1f0(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0xb160(%rip)        
-	faddp  %st,%st(1)
+	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0xb162(%rip)        
+	fldt   0xb1ea(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fdivrp %st,%st(1)
+	fldt   0xb1f2(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xb1f6(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xb1f8(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xb1fa(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	faddp  %st,%st(2)
+	fdivp  %st,%st(1)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   -0x58(%rsp)
-	fld    %st(0)
-	fldt   -0x38(%rsp)
+	fldt   -0x28(%rsp)
+	fldt   -0x18(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
-	fldt   0x28(%rsp)
+	faddp  %st,%st(1)
+	fldt   0x18(%rsp)
+	fmul   %st(3),%st
+	faddp  %st,%st(1)
 	fldt   -0x8(%rsp)
+	fldt   0x28(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
-	fldt   0x8(%rsp)
-	fxch   %st(3)
-	fld    %st(0)
-	fstpt  0x78(%rsp)
-	fmulp  %st,%st(3)
-	fxch   %st(1)
-	faddp  %st,%st(2)
-	fxch   %st(1)
-	fstpt  -0x58(%rsp)
-	fldt   0xaadc(%rip)        
+	faddp  %st,%st(1)
+	fstpt  -0x48(%rsp)
+	fldt   0xab82(%rip)        
 	fmul   %st(3),%st
-	fldt   0xaae4(%rip)        
+	fldt   0xab8a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xaaea(%rip)        
+	fldt   0xab90(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xaaf0(%rip)        
+	fldt   0xab96(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xaaf6(%rip)        
+	fldt   0xab9c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xaafc(%rip)        
+	fldt   0xaba2(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xab02(%rip)        
+	fldt   0xaba8(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xab08(%rip)        
+	fldt   0xabae(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fld1
-	faddp  %st,%st(1)
+	fadd   %st(1),%st
 	fmul   %st(3),%st
-	fldt   0xa678(%rip)        
+	fldt   0xa720(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xab00(%rip)        
+	fldt   0xaba8(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xab02(%rip)        
+	fldt   0xabaa(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xab02(%rip)        
+	fldt   0xabaa(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xab02(%rip)        
+	fldt   0xabaa(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xab02(%rip)        
+	fldt   0xabaa(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fld    %st(3)
-	fxch   %st(1)
-	faddp  %st,%st(4)
-	fxch   %st(1)
-	fdivp  %st,%st(3)
-	fxch   %st(2)
-	fstpt  -0x18(%rsp)
-	fldt   0xaaf2(%rip)        
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  0x38(%rsp)
+	fldt   0xaba0(%rip)        
 	fmul   %st(3),%st
-	fldt   0xaafa(%rip)        
+	fldt   0xaba8(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xab00(%rip)        
+	fldt   0xabae(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xab06(%rip)        
+	fldt   0xabb4(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xab0c(%rip)        
+	fldt   0xabba(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xab12(%rip)        
+	fldt   0xabc0(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fld1
-	faddp  %st,%st(1)
+	fadd   %st(1),%st
 	fmul   %st(3),%st
-	fldt   0xab12(%rip)        
+	fldt   0xabc2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xab18(%rip)        
+	fldt   0xabc8(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xab1e(%rip)        
+	fldt   0xabce(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xab26(%rip)        
+	fldt   0xabd6(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xab28(%rip)        
+	fldt   0xabd8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xab28(%rip)        
+	fldt   0xabd8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xab28(%rip)        
+	fldt   0xabd8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xab28(%rip)        
+	fldt   0xabd8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  0x48(%rsp)
+	fldt   0xabce(%rip)        
 	fld    %st(3)
-	fxch   %st(1)
-	faddp  %st,%st(4)
-	fxch   %st(1)
-	fdivp  %st,%st(3)
-	fldt   0xab1e(%rip)        
-	fld    %st(4)
 	fmul   %st(1),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xab20(%rip)        
+	fmul   %st(3),%st
+	fldt   0xabd0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xab20(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xabd0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xab20(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xabd0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fld1
-	fadd   %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
-	fldt   0xab16(%rip)        
-	fld    %st(5)
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fadd   %st(1),%st
+	fmul   %st(3),%st
+	fsub   %st(1),%st
+	fldt   0xabca(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xab18(%rip)        
+	fmul   %st(4),%st
+	fldt   0xabcc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xab18(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xabcc(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xab18(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xabcc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xab18(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xabcc(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(2),%st
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x18(%rsp)
-	fldt   -0x18(%rsp)
+	fldt   0x38(%rsp)
+	fmul   %st(5),%st
+	faddp  %st,%st(1)
+	fldt   0x8(%rsp)
+	fldt   0x48(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fxch   %st(3)
-	fld    %st(0)
-	fstpt  0x88(%rsp)
-	fmul   %st(5),%st
-	faddp  %st,%st(3)
-	fxch   %st(2)
-	fstpt  -0x48(%rsp)
-	fldt   0xaefd(%rip)        
+	fstpt  -0x38(%rsp)
+	fldt   0xafb8(%rip)        
 	fmul   %st(3),%st
-	fldt   0xaf05(%rip)        
+	fldt   0xafc0(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xaf0b(%rip)        
+	fldt   0xafc6(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xaf11(%rip)        
+	fldt   0xafcc(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xaf17(%rip)        
+	fldt   0xafd2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xaf1d(%rip)        
+	fldt   0xafd8(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xaf23(%rip)        
+	fldt   0xafde(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xaf29(%rip)        
+	fldt   0xafe4(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fld1
-	faddp  %st,%st(1)
+	fadd   %st(1),%st
 	fmul   %st(3),%st
-	fldt   0xaf29(%rip)        
+	fldt   0xafe6(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xaf2f(%rip)        
+	fldt   0xafec(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xaf35(%rip)        
+	fldt   0xaff2(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xaf3d(%rip)        
+	fldt   0xaffa(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xaf3f(%rip)        
+	fldt   0xaffc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xaf3f(%rip)        
+	fldt   0xaffc(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xaf3f(%rip)        
+	fldt   0xaffc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xaf3f(%rip)        
+	fldt   0xaffc(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xaf3f(%rip)        
+	fldt   0xaffc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  0x58(%rsp)
+	fldt   0xaff2(%rip)        
 	fld    %st(3)
-	fxch   %st(1)
-	faddp  %st,%st(4)
-	fxch   %st(1)
-	fdivp  %st,%st(3)
-	fldt   0xaf35(%rip)        
-	fld    %st(4)
 	fmul   %st(1),%st
-	fldt   0xaf3b(%rip)        
+	fldt   0xaff8(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xaf3d(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaffa(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf43(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb000(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf49(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb006(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf4f(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb00c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa435(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa4f2(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf45(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(1),%st
+	fmul   %st(3),%st
+	fldt   0xb004(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf4b(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb00a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf51(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb010(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xaf59(%rip)        
-	fld    %st(5)
+	fldt   0xb018(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xaf5b(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb01a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xaf5b(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb01a(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xaf5b(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb01a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xaf5b(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb01a(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xaf5b(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb01a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(2),%st
-	fdivrp %st,%st(1)
-	fstpt  0x38(%rsp)
-	fldt   0xaf53(%rip)        
+	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xaf5b(%rip)        
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  0x68(%rsp)
+	fldt   0xb010(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb018(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf61(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb01e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf67(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb024(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf6d(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb02a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf73(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb030(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf79(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb036(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf7f(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb03c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf85(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb042(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xaf8b(%rip)        
+	fmul   %st(3),%st
+	fldt   0xb048(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa28b(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(1),%st
+	fmul   %st(3),%st
+	fldt   0xa34a(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xaf83(%rip)        
-	fld    %st(5)
+	fldt   0xb042(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xaf85(%rip)        
+	fmul   %st(4),%st
+	fldt   0xb044(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xaf85(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb044(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xaf85(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb044(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xaf85(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb044(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xaf85(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xb044(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(2),%st
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fld    %st(2)
+	fldt   -0x18(%rsp)
 	fmulp  %st,%st(1)
-	fldt   -0x38(%rsp)
+	fldt   -0x28(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fld    %st(3)
-	fldt   -0x8(%rsp)
-	fmulp  %st,%st(1)
+	fldt   0x58(%rsp)
+	fmul   %st(3),%st
 	faddp  %st,%st(1)
-	fldt   0x8(%rsp)
-	fldt   0x38(%rsp)
+	fldt   -0x8(%rsp)
+	fldt   0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fstpt  -0x38(%rsp)
-	fldt   0xa847(%rip)        
-	fmul   %st(4),%st
-	fldt   0xa84f(%rip)        
+	fstpt  -0x28(%rsp)
+	fldt   0xa904(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa90c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	fldt   0xa853(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa910(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa853(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa910(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa859(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa916(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa859(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(2),%st
+	fmul   %st(4),%st
+	fldt   0xa918(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa85f(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa91e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
+	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fldt   0xa863(%rip)        
-	fld    %st(5)
+	fldt   0xa922(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa865(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa924(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa865(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa924(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa865(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa924(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa865(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa924(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(2),%st
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0x48(%rsp)
-	fldt   0xa85d(%rip)        
+	fldt   0xa91e(%rip)        
 	fmul   %st(4),%st
-	fldt   0xa865(%rip)        
+	fldt   0xa926(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa86b(%rip)        
+	fldt   0xa92c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa871(%rip)        
+	fldt   0xa932(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa877(%rip)        
+	fldt   0xa938(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa87d(%rip)        
+	fldt   0xa93e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fld1
-	faddp  %st,%st(1)
+	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fldt   0xa87d(%rip)        
+	fldt   0xa940(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa883(%rip)        
+	fldt   0xa946(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa889(%rip)        
+	fldt   0xa94c(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xa891(%rip)        
+	fldt   0xa954(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa893(%rip)        
+	fldt   0xa956(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa893(%rip)        
+	fldt   0xa956(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa893(%rip)        
+	fldt   0xa956(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa893(%rip)        
+	fldt   0xa956(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(2),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   0x18(%rsp)
-	fmulp  %st,%st(1)
-	fldt   -0x18(%rsp)
+	fmul   %st(5),%st
+	fldt   0x38(%rsp)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x48(%rsp)
-	fmul   %st(6),%st
+	fldt   0x8(%rsp)
+	fxch   %st(2)
+	fld    %st(0)
+	fstpt  0x88(%rsp)
+	fmulp  %st,%st(2)
 	faddp  %st,%st(1)
-	fstpt  0x68(%rsp)
-	fldt   0xade1(%rip)        
-	fmul   %st(4),%st
-	fldt   0xade9(%rip)        
+	fstpt  0x78(%rsp)
+	fldt   0xae9b(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaea3(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	fldt   0xaded(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xadef(%rip)        
-	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xadf5(%rip)        
+	fldt   0xaea7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fld1
+	fsubp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaea9(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xadf5(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaeaf(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xadfb(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(1),%st
+	fmul   %st(3),%st
+	fldt   0xaeb1(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaeb7(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xae01(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaebd(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xae07(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaec3(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xae0d(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaec9(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xae15(%rip)        
-	fld    %st(5)
+	fldt   0xaed1(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xae17(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaed3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xae17(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaed3(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xae17(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaed3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xae17(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaed3(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xae17(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaed3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(2),%st
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0x58(%rsp)
-	fldt   0xae0f(%rip)        
-	fld    %st(4)
+	fstpt  0x38(%rsp)
+	fldt   0xaec9(%rip)        
+	fld    %st(3)
 	fmul   %st(1),%st
-	fldt   0xae15(%rip)        
+	fldt   0xaecf(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xae17(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaed1(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xae1d(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaed7(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xae23(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaedd(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xae29(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaee3(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xae2f(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaee9(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xae2f(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(1),%st
+	fmul   %st(3),%st
+	fldt   0xaeeb(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xae35(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaef1(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xae3b(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaef7(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xae43(%rip)        
-	fld    %st(5)
+	fldt   0xaeff(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xae45(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaf01(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xae45(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaf01(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xae45(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaf01(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xae45(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaf01(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xae45(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaf01(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fxch   %st(2)
-	fsts   -0x18(%rsp)
-	faddp  %st,%st(2)
-	fdivp  %st,%st(1)
-	fldt   -0x8(%rsp)
-	fmulp  %st,%st(1)
-	fldt   0x28(%rsp)
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fmul   %st(2),%st
+	fldt   0x18(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fld    %st(2)
-	fmulp  %st,%st(4)
-	faddp  %st,%st(3)
-	faddp  %st,%st(2)
-	fldt   0x8(%rsp)
 	fldt   0x58(%rsp)
+	fldt   -0x18(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
-	fldt   0xa6a7(%rip)        
-	fld    %st(3)
+	faddp  %st,%st(1)
+	faddp  %st,%st(1)
+	fldt   -0x8(%rsp)
+	fldt   0x38(%rsp)
+	fmulp  %st,%st(1)
+	faddp  %st,%st(1)
+	fldt   0xa765(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
-	fldt   0xa6ad(%rip)        
+	fldt   0xa76b(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa033(%rip)        
-	fadd   %st,%st(1)
-	fxch   %st(1)
 	fmul   %st(5),%st
-	fldt   0xa077(%rip)        
-	fsubrp %st,%st(1)
+	fldt   0xa0f1(%rip)        
+	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fld1
-	fadd   %st,%st(1)
+	fldt   0xa137(%rip)        
+	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
-	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa061(%rip)        
+	fadd   %st(4),%st
+	fmul   %st(6),%st
+	fsub   %st(4),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa673(%rip)        
+	fldt   0xa0cf(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa735(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fldt   0xa677(%rip)        
-	fld    %st(4)
-	fmul   %st(1),%st
+	fldt   0xa739(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa731(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa679(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa737(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa679(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa737(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa679(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa737(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa679(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa737(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
+	fmul   %st(6),%st
+	faddp  %st,%st(1)
 	fmul   %st(5),%st
+	fldz
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fadds  -0x18(%rsp)
 	fdivrp %st,%st(1)
-	fmulp  %st,%st(4)
-	fldt   0x88(%rsp)
-	fldt   -0x68(%rsp)
+	fldt   0x8(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x18(%rsp)
 	fldt   0x48(%rsp)
+	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	faddp  %st,%st(4)
-	fldt   0xad56(%rip)        
-	fld    %st(3)
+	fldt   0x88(%rsp)
+	fmulp  %st,%st(7)
+	faddp  %st,%st(6)
+	faddp  %st,%st(5)
+	fldt   0xae14(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
-	fldt   0xad5c(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xad62(%rip)        
-	fadd   %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(5),%st
-	fldt   0xad66(%rip)        
+	fldt   0xae1a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xad6c(%rip)        
+	fldt   0xae20(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fld1
-	fsubr  %st,%st(1)
+	fldt   0xae26(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xae2c(%rip)        
+	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
+	fsub   %st(4),%st
+	fmul   %st(6),%st
+	fadd   %st(4),%st
+	fmul   %st(6),%st
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xae04(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xad56(%rip)        
+	fldt   0xadea(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xad3c(%rip)        
+	fldt   0xadd0(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xad0e(%rip)        
-	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fsubp  %st,%st(1)
-	fldt   0xad42(%rip)        
-	fld    %st(4)
-	fmul   %st(1),%st
+	fldt   0xae04(%rip)        
+	fmul   %st(5),%st
+	fldt   0xadfc(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xad44(%rip)        
+	fmul   %st(5),%st
+	fldt   0xae02(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xad44(%rip)        
+	fmul   %st(5),%st
+	fldt   0xae02(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xad44(%rip)        
+	fmul   %st(5),%st
+	fldt   0xae02(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xad44(%rip)        
+	fmul   %st(5),%st
+	fldt   0xae02(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xad44(%rip)        
+	fmul   %st(5),%st
+	fldt   0xae02(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
+	fmulp  %st,%st(5)
+	fldz
+	faddp  %st,%st(5)
+	fdivp  %st,%st(4)
+	fldt   -0x8(%rsp)
 	fmulp  %st,%st(4)
-	fxch   %st(3)
-	fadds  -0x18(%rsp)
-	fdivrp %st,%st(3)
-	fldt   0x8(%rsp)
-	fmulp  %st,%st(3)
-	fldt   0x78(%rsp)
+	fldt   0x28(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x38(%rsp)
-	fmulp  %st,%st(2)
-	faddp  %st,%st(1)
-	fldt   0x58(%rsp)
-	fldt   -0x8(%rsp)
+	fldt   0x68(%rsp)
+	fldt   -0x18(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	faddp  %st,%st(2)
+	fldt   0x38(%rsp)
+	fmulp  %st,%st(4)
+	faddp  %st,%st(3)
+	fxch   %st(2)
+	faddp  %st,%st(3)
 	test   %esi,%esi
-	jle    33af <polyreg6+0xcdf>
-	fldt   -0x28(%rsp)
+	jle    32e8 <polyreg6+0xca8>
+	fldt   0x78(%rsp)
 	movslq %esi,%rsi
 	xor    %eax,%eax
-	fldt   0x68(%rsp)
-	nopl   (%rax)
+	nopl   0x0(%rax,%rax,1)
 	mov    %eax,-0x78(%rsp)
 	fildl  -0x78(%rsp)
-	fmul   %st(2),%st
-	fld1
-	fsubrp %st,%st(1)
+	fldt   -0x58(%rsp)
+	fmulp  %st,%st(1)
+	fsub   %st(2),%st
 	fld    %st(4)
 	fmul   %st(1),%st
 	fadd   %st(6),%st
 	fmul   %st(1),%st
 	fadd   %st(4),%st
 	fmul   %st(1),%st
 	fadd   %st(2),%st
 	fmul   %st(1),%st
-	fldt   -0x38(%rsp)
+	fldt   -0x28(%rsp)
 	faddp  %st,%st(1)
 	fmul   %st(1),%st
-	fldt   -0x48(%rsp)
+	fldt   -0x38(%rsp)
 	faddp  %st,%st(1)
 	fmulp  %st,%st(1)
-	fldt   -0x58(%rsp)
+	fldt   -0x48(%rsp)
 	faddp  %st,%st(1)
 	fsubrl (%rdi,%rax,8)
 	fstpl  (%rdx,%rax,8)
 	add    $0x1,%rax
-	cmp    %rsi,%rax
-	jne    3368 <polyreg6+0xc98>
+	cmp    %rax,%rsi
+	jne    3298 <polyreg6+0xc58>
 	fstp   %st(0)
 	fstp   %st(0)
-	fldt   -0x58(%rsp)
-	fstpl  -0x78(%rsp)
+	jmp    32ea <polyreg6+0xcaa>
+	nopl   0x0(%rax,%rax,1)
+	fstp   %st(0)
 	fldt   -0x48(%rsp)
-	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	fldt   -0x38(%rsp)
+	movsd  -0x78(%rsp),%xmm0
+	fstpl  -0x78(%rsp)
+	fldt   -0x28(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	movups %xmm0,(%r8)
+	movups %xmm0,(%rcx)
 	fstpl  -0x78(%rsp)
-	fldt   0x68(%rsp)
+	fldt   0x78(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	movhpd -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	fxch   %st(1)
-	movups %xmm0,0x10(%r8)
+	movups %xmm0,0x10(%rcx)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	fstpl  0x30(%r8)
-	movups %xmm0,0x20(%r8)
+	fstpl  0x30(%rcx)
+	movups %xmm0,0x20(%rcx)
 	add    $0xa0,%rsp
 	ret
-	nopw   0x0(%rax,%rax,1)
-	pxor   %xmm2,%xmm2
-	movss  %xmm2,-0x18(%rsp)
-	flds   -0x18(%rsp)
-	fld    %st(0)
-	fld    %st(0)
-	fstpt  0x8(%rsp)
-	fxch   %st(1)
+	xchg   %ax,%ax
+	fldz
 	fstpt  -0x8(%rsp)
 	fldt   -0x8(%rsp)
+	fstpt  0x8(%rsp)
+	fldt   0x8(%rsp)
 	fld    %st(0)
-	fld    %st(0)
-	fstpt  0x18(%rsp)
-	fld    %st(0)
-	fstpt  -0x58(%rsp)
+	fld    %st(1)
+	fstpt  -0x18(%rsp)
+	fldt   -0x18(%rsp)
 	fstpt  -0x68(%rsp)
+	fldt   -0x68(%rsp)
 	fstpt  -0x78(%rsp)
 	fxch   %st(1)
-	jmp    2790 <polyreg6+0xc0>
-	nopl   (%rax)
+	fxch   %st(2)
+	fxch   %st(1)
+	jmp    26ee <polyreg6+0xae>
+	data16 cs nopw 0x0(%rax,%rax,1)
 
-0000000000003460 <polyreg7>:
+0000000000003390 <polyreg7>:
 polyreg7():
-	sub    $0x100,%rsp
-	mov    %rcx,%r8
+	sub    $0xe0,%rsp
 	mov    %esi,-0x78(%rsp)
 	fildl  -0x78(%rsp)
 	fld    %st(0)
 	fld1
 	fsubrp %st,%st(1)
-	fdivrs 0x9bb2(%rip)        
-	fstpt  0x8(%rsp)
+	fdivrs 0x9c85(%rip)        
+	fstpt  -0x8(%rsp)
 	test   %esi,%esi
-	jle    4798 <polyreg7+0x1338>
-	pxor   %xmm1,%xmm1
-	movslq %esi,%rcx
+	jle    46a8 <polyreg7+0x1318>
+	fldz
+	movslq %esi,%r8
 	xor    %eax,%eax
-	movss  %xmm1,-0x2c(%rsp)
-	flds   -0x2c(%rsp)
 	fld    %st(0)
 	fld    %st(1)
 	fld    %st(2)
-	fld    %st(3)
-	fld    %st(0)
 	fstpt  -0x58(%rsp)
+	fldt   -0x58(%rsp)
 	fld    %st(0)
 	fstpt  -0x68(%rsp)
-	fxch   %st(4)
-	fstpt  0x18(%rsp)
-	fxch   %st(3)
+	fldt   -0x68(%rsp)
 	fld    %st(0)
 	fstpt  -0x78(%rsp)
-	fxch   %st(4)
-	fstpt  -0x28(%rsp)
-	fld    %st(3)
+	fxch   %st(5)
+	fstpt  -0x38(%rsp)
 	nopw   0x0(%rax,%rax,1)
 	mov    %eax,-0x48(%rsp)
 	fildl  -0x48(%rsp)
-	fldt   0x8(%rsp)
+	fldt   -0x8(%rsp)
 	fmulp  %st,%st(1)
 	fld1
 	fsubrp %st,%st(1)
 	fldl   (%rdi,%rax,8)
 	fldt   -0x78(%rsp)
 	add    $0x1,%rax
 	fadd   %st(1),%st
 	fstpt  -0x78(%rsp)
 	fmul   %st(1),%st
-	fadd   %st,%st(2)
+	fadd   %st,%st(6)
 	fmul   %st(1),%st
 	fldt   -0x68(%rsp)
 	fadd   %st(1),%st
 	fstpt  -0x68(%rsp)
 	fmul   %st(1),%st
-	fadd   %st,%st(6)
+	fadd   %st,%st(2)
 	fmul   %st(1),%st
 	fldt   -0x58(%rsp)
 	fadd   %st(1),%st
 	fstpt  -0x58(%rsp)
 	fmul   %st(1),%st
 	fadd   %st,%st(5)
 	fmul   %st(1),%st
 	fadd   %st,%st(3)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(3)
-	cmp    %rax,%rcx
-	jne    34d0 <polyreg7+0x70>
-	fldt   -0x28(%rsp)
+	cmp    %rax,%r8
+	jne    33e8 <polyreg7+0x58>
+	fldt   -0x38(%rsp)
+	fxch   %st(4)
+	fstpt  0x8(%rsp)
 	fxch   %st(1)
 	fstpt  0x18(%rsp)
-	fxch   %st(4)
-	fstpt  0x28(%rsp)
-	fstpt  0x38(%rsp)
-	fstpt  0x48(%rsp)
-	fldt   0xa37e(%rip)        
-	fmul   %st(2),%st
-	fldt   0xa386(%rip)        
+	fldt   0xa45e(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa466(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xa38c(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa46c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xa392(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa472(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xa398(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa478(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
+	fmul   %st(3),%st
 	fld1
-	fadd   %st,%st(1)
-	fxch   %st(1)
+	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fsubs  0x9abe(%rip)        
-	fldt   0xa390(%rip)        
+	fsubs  0x9bb0(%rip)        
+	fldt   0xa472(%rip)        
 	fmul   %st(4),%st
-	flds   -0x2c(%rsp)
+	fldz
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
-	fldt   0xa38e(%rip)        
+	fldt   0xa472(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
 	fadd   %st(1),%st
 	fmul   %st(5),%st
-	fldt   0xa390(%rip)        
+	fldt   0xa474(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
 	fadd   %st(1),%st
 	fmul   %st(5),%st
-	fldt   0xa392(%rip)        
+	fldt   0xa476(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(1),%st
-	fdivrp %st,%st(2)
-	fxch   %st(1)
-	fstpt  -0x18(%rsp)
-	fldt   0xa38e(%rip)        
-	fmul   %st(4),%st
-	fldt   0xa396(%rip)        
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  -0x28(%rsp)
+	fldt   0xa474(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa47c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa39c(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa482(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa3a2(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa488(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa3a8(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa48e(%rip)        
 	fsubrp %st,%st(1)
+	fmul   %st(3),%st
+	fld1
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fsubs  0x9b3a(%rip)        
+	fldt   0xa488(%rip)        
 	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fsubs  0x9a46(%rip)        
-	fldt   0xa3a4(%rip)        
-	fmul   %st(5),%st
-	fadd   %st(2),%st
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(1)
 	fmul   %st(5),%st
-	fldt   0xa3a8(%rip)        
+	fldt   0xa488(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(2),%st
+	fadd   %st(1),%st
 	fmul   %st(5),%st
-	fldt   0xa3aa(%rip)        
+	fldt   0xa48a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fld    %st(2)
-	fxch   %st(1)
-	fadd   %st(3),%st
-	fmul   %st(6),%st
-	fldt   0xa3a8(%rip)        
+	fadd   %st(1),%st
+	fmul   %st(5),%st
+	fldt   0xa48c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(3)
-	fxch   %st(1)
-	fdivp  %st,%st(2)
-	fxch   %st(1)
-	fstpt  0x58(%rsp)
-	fldt   0xa3a2(%rip)        
-	fmul   %st(4),%st
-	fldt   0xa3aa(%rip)        
+	fmul   %st(5),%st
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  0x28(%rsp)
+	fldt   0xa48a(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa492(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	flds   0x99ee(%rip)        
+	fmul   %st(4),%st
+	flds   0x9ae6(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fadd   %st(4),%st
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
+	fld1
 	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa396(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xa47c(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xa39e(%rip)        
-	fmul   %st(5),%st
-	fadd   %st(2),%st
+	fldt   0xa484(%rip)        
+	fmul   %st(4),%st
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(1)
 	fmul   %st(5),%st
-	fldt   0xa3a2(%rip)        
+	fldt   0xa484(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fld    %st(2)
-	fxch   %st(1)
-	fadd   %st(3),%st
-	fmul   %st(6),%st
-	fldt   0xa3a0(%rip)        
+	fadd   %st(1),%st
+	fmul   %st(5),%st
+	fldt   0xa486(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fadd   %st(3),%st
-	fmul   %st(6),%st
-	fldt   0xa3a2(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(3)
-	fxch   %st(1)
-	fdivp  %st,%st(2)
-	fldt   0xa3a2(%rip)        
 	fmul   %st(5),%st
 	fadd   %st(1),%st
 	fmul   %st(5),%st
-	fldt   0xa3a6(%rip)        
+	fldt   0xa488(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
 	fadd   %st(1),%st
-	fmul   %st(5),%st
-	fadd   %st(3),%st
-	fmul   %st(5),%st
+	fdivrp %st,%st(2)
+	fxch   %st(1)
+	fstpt  0x38(%rsp)
+	fldt   0xa484(%rip)        
+	fmul   %st(4),%st
 	fadd   %st(1),%st
-	fmul   %st(5),%st
-	fldt   0xa3a0(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa488(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xa3a8(%rip)        
-	fmul   %st(6),%st
+	fmul   %st(4),%st
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fld1
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(1)
+	fmul   %st(4),%st
+	fldt   0xa47c(%rip)        
+	fsubrp %st,%st(1)
+	fldt   0xa484(%rip)        
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(6),%st
-	fldt   0xa3ac(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa488(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(6),%st
-	fldt   0xa3ae(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa48a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(6),%st
-	fldt   0xa3b0(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa48c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(2)
 	fdivp  %st,%st(1)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
 	fldt   -0x68(%rsp)
-	fldt   -0x18(%rsp)
+	fldt   -0x28(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	fldt   -0x58(%rsp)
-	fldt   0x58(%rsp)
+	fldt   0x28(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
+	fldt   0x18(%rsp)
 	fldt   0x38(%rsp)
-	fxch   %st(2)
-	fld    %st(0)
-	fstpt  0xc8(%rsp)
-	fmulp  %st,%st(2)
+	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	fstpt  -0x48(%rsp)
-	fldt   0xa92d(%rip)        
+	fldt   0xaa10(%rip)        
 	fmul   %st(3),%st
-	fldt   0xa935(%rip)        
+	fldt   0xaa18(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa93b(%rip)        
+	fldt   0xaa1e(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa941(%rip)        
+	fldt   0xaa24(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa947(%rip)        
+	fldt   0xaa2a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa94d(%rip)        
+	fldt   0xaa30(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa953(%rip)        
+	fldt   0xaa36(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa959(%rip)        
+	fldt   0xaa3c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa95f(%rip)        
+	fldt   0xaa42(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa965(%rip)        
+	fldt   0xaa48(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa96b(%rip)        
+	fldt   0xaa4e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa971(%rip)        
+	fldt   0xaa54(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fadd   %st(1),%st
+	fld1
+	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98a3(%rip)        
+	fldt   0x9984(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xa96b(%rip)        
+	fldt   0xaa4c(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa96d(%rip)        
+	fldt   0xaa4e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa96d(%rip)        
+	fldt   0xaa4e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa96d(%rip)        
+	fldt   0xaa4e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa96d(%rip)        
+	fldt   0xaa4e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa96d(%rip)        
+	fldt   0xaa4e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa96d(%rip)        
+	fldt   0xaa4e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadds  -0x2c(%rsp)
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   0xa967(%rip)        
-	fmul   %st(4),%st
-	fldt   0xa96f(%rip)        
+	fstpt  -0x18(%rsp)
+	fldt   0xaa44(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaa4c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa975(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaa52(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa97b(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaa58(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa981(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaa5e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa987(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaa64(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa98d(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaa6a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa993(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaa70(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa999(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaa76(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa99f(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaa7c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0xa9a1(%rip)        
+	fmul   %st(3),%st
+	fld1
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaa7c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa9a7(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaa82(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa9ad(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaa88(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xa9b5(%rip)        
-	fld    %st(5)
+	fldt   0xaa90(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9b7(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaa92(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa9b7(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaa92(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa9b7(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaa92(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa9b7(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaa92(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa9b7(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaa92(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa9b7(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaa92(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x2c(%rsp)
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0x68(%rsp)
-	fldt   0xa9ad(%rip)        
-	fld    %st(4)
+	fstpt  0x48(%rsp)
+	fldt   0xaa88(%rip)        
+	fld    %st(3)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa9af(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaa8a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa9af(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaa8a(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa9af(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaa8a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa9af(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaa8a(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa9af(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaa8a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fsubp  %st,%st(1)
+	fmul   %st(3),%st
+	fld1
+	fadd   %st,%st(1)
+	fxch   %st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldz
+	faddp  %st,%st(1)
+	fldt   0xaa7a(%rip)        
 	fmul   %st(4),%st
-	fadds  -0x2c(%rsp)
-	fldt   0xa9a3(%rip)        
-	fmul   %st(5),%st
-	fldt   0xa9ab(%rip)        
+	fldt   0xaa82(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9b1(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaa88(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9b7(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaa8e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9bd(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaa94(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9c3(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaa9a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9c9(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaaa0(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9cf(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaaa6(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9d5(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaaac(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9db(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaab2(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9e1(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaab8(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9e7(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaabe(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9ed(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaac4(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9f3(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaaca(%rip)        
 	fsubrp %st,%st(1)
 	fxch   %st(1)
 	fld    %st(0)
-	fstpt  0xb8(%rsp)
+	fstpt  0xc8(%rsp)
 	fdivrp %st,%st(1)
-	fstpt  0x78(%rsp)
-	fldt   0xa9ea(%rip)        
-	fld    %st(4)
+	fstpt  0x58(%rsp)
+	fldt   0xaac1(%rip)        
+	fld    %st(3)
 	fmul   %st(1),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa9ec(%rip)        
+	fmul   %st(3),%st
+	fldt   0xaac3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa9ec(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaac3(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa9ec(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaac3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa9ec(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaac3(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa9ec(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xaac3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fld1
+	fadd   %st,%st(1)
+	fxch   %st(1)
 	fmul   %st(4),%st
-	fsub   %st(2),%st
-	fldt   0xa9e6(%rip)        
-	fld    %st(5)
+	fsubp  %st,%st(1)
+	fldt   0xaab9(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa9e8(%rip)        
+	fmul   %st(4),%st
+	fldt   0xaabb(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa9e8(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaabb(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa9e8(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaabb(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa9e8(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaabb(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa9e8(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaabb(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa9e8(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xaabb(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x2c(%rsp)
-	fdivrp %st,%st(1)
-	fldt   0x18(%rsp)
-	fmulp  %st,%st(1)
-	fxch   %st(1)
-	fld    %st(0)
-	fstpt  -0x8(%rsp)
-	fldt   0x28(%rsp)
-	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x68(%rsp)
-	fmul   %st(3),%st
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fmul   %st(4),%st
+	fldt   -0x18(%rsp)
+	fmul   %st(2),%st
 	faddp  %st,%st(1)
 	fldt   0x48(%rsp)
-	fldt   0x78(%rsp)
+	fldt   0x8(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fstpt  -0x28(%rsp)
-	fldt   0x9f84(%rip)        
+	fldt   0x58(%rsp)
+	fmul   %st(3),%st
+	faddp  %st,%st(1)
+	fstpt  -0x38(%rsp)
+	fldt   0xa063(%rip)        
 	fmul   %st(3),%st
-	fldt   0x9f8c(%rip)        
+	fldt   0xa06b(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9f92(%rip)        
+	fldt   0xa071(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9f98(%rip)        
+	fldt   0xa077(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9f9e(%rip)        
+	fldt   0xa07d(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9fa4(%rip)        
+	fldt   0xa083(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9faa(%rip)        
+	fldt   0xa089(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9fb0(%rip)        
+	fldt   0xa08f(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fadd   %st(1),%st
+	fld1
+	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9fb2(%rip)        
+	fldt   0xa08f(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9fb8(%rip)        
+	fldt   0xa095(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9fbe(%rip)        
+	fldt   0xa09b(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9fc6(%rip)        
+	fldt   0xa0a3(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9fc8(%rip)        
+	fldt   0xa0a5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9fc8(%rip)        
+	fldt   0xa0a5(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9fc8(%rip)        
+	fldt   0xa0a5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9fc8(%rip)        
+	fldt   0xa0a5(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9fc8(%rip)        
+	fldt   0xa0a5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	flds   -0x2c(%rsp)
-	fadd   %st,%st(1)
-	fxch   %st(2)
-	fdivp  %st,%st(1)
-	fstpt  0x88(%rsp)
-	fldt   0x9fb7(%rip)        
-	fld    %st(4)
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  0x68(%rsp)
+	fldt   0xa09b(%rip)        
+	fld    %st(3)
 	fmul   %st(1),%st
-	fldt   0x9fbd(%rip)        
+	fldt   0xa0a1(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9fbf(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xa0a3(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9fc5(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0a9(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9fcb(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0af(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9fd1(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0b5(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x94b7(%rip)        
+	fmul   %st(3),%st
+	fldt   0x959b(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0x9fc9(%rip)        
+	fmul   %st(3),%st
+	fld1
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xa0ab(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9fcf(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0b1(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9fd5(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0b7(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9fdd(%rip)        
-	fld    %st(5)
+	fldt   0xa0bf(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fdf(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0c1(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9fdf(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa0c1(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9fdf(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa0c1(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9fdf(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa0c1(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9fdf(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa0c1(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	faddp  %st,%st(2)
-	fdivp  %st,%st(1)
-	fldt   0x9fdb(%rip)        
+	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9fe3(%rip)        
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  0x78(%rsp)
+	fldt   0xa0b7(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0bf(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9fe9(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0c5(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9fef(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0cb(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9ff5(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0d1(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9ffb(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0d7(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa001(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0dd(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa007(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0e3(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa00d(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0e9(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa013(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa0ef(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0x9315(%rip)        
+	fmul   %st(3),%st
+	fld1
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0x93ef(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xa00d(%rip)        
-	fld    %st(5)
+	fldt   0xa0e7(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa00f(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0e9(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa00f(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa0e9(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa00f(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa0e9(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa00f(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa0e9(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa00f(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa0e9(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x2c(%rsp)
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
-	fldt   -0x18(%rsp)
+	fldt   -0x28(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	fldt   -0x58(%rsp)
-	fldt   0x88(%rsp)
+	fldt   0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x38(%rsp)
-	fxch   %st(2)
-	fld    %st(0)
-	fstpt  0xd8(%rsp)
-	fmulp  %st,%st(2)
+	fldt   0x18(%rsp)
+	fldt   0x78(%rsp)
+	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fstpt  -0x18(%rsp)
-	fldt   0xa701(%rip)        
+	fstpt  -0x28(%rsp)
+	fldt   0xa7e5(%rip)        
 	fmul   %st(3),%st
-	fldt   0xa709(%rip)        
+	fldt   0xa7ed(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa70f(%rip)        
+	fldt   0xa7f3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa715(%rip)        
+	fldt   0xa7f9(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa71b(%rip)        
+	fldt   0xa7ff(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa721(%rip)        
+	fldt   0xa805(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa727(%rip)        
+	fldt   0xa80b(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa72d(%rip)        
+	fldt   0xa811(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa733(%rip)        
+	fldt   0xa817(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa739(%rip)        
+	fldt   0xa81d(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fadd   %st(1),%st
+	fld1
+	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa73b(%rip)        
+	fldt   0xa81d(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa741(%rip)        
+	fldt   0xa823(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0xa747(%rip)        
+	fldt   0xa829(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xa74f(%rip)        
+	fldt   0xa831(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa751(%rip)        
+	fldt   0xa833(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa751(%rip)        
+	fldt   0xa833(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa751(%rip)        
+	fldt   0xa833(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa751(%rip)        
+	fldt   0xa833(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa751(%rip)        
+	fldt   0xa833(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa751(%rip)        
+	fldt   0xa833(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	flds   -0x2c(%rsp)
+	fldz
 	fadd   %st,%st(1)
 	fxch   %st(2)
 	fdivp  %st,%st(1)
-	fstpt  0x98(%rsp)
-	fldt   0xa740(%rip)        
+	fstpt  0x88(%rsp)
+	fldt   0xa824(%rip)        
 	fmul   %st(4),%st
-	fldt   0xa748(%rip)        
+	fldt   0xa82c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa74e(%rip)        
+	fldt   0xa832(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa754(%rip)        
+	fldt   0xa838(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa75a(%rip)        
+	fldt   0xa83e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa760(%rip)        
+	fldt   0xa844(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa766(%rip)        
+	fldt   0xa84a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa76c(%rip)        
+	fldt   0xa850(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fld1
+	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa76e(%rip)        
+	fldt   0xa850(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa774(%rip)        
+	fldt   0xa856(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa77a(%rip)        
+	fldt   0xa85c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa780(%rip)        
+	fldt   0xa862(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa786(%rip)        
+	fldt   0xa868(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xa78e(%rip)        
+	fldt   0xa870(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa790(%rip)        
+	fldt   0xa872(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa790(%rip)        
+	fldt   0xa872(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa790(%rip)        
+	fldt   0xa872(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa790(%rip)        
+	fldt   0xa872(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa790(%rip)        
+	fldt   0xa872(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa790(%rip)        
+	fldt   0xa872(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(2),%st
-	fdivrp %st,%st(1)
-	fldt   0xa78c(%rip)        
-	fmul   %st(5),%st
-	fldt   0xa794(%rip)        
+	faddp  %st,%st(2)
+	fdivp  %st,%st(1)
+	fstpt  0x98(%rsp)
+	fldt   0xa867(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa86f(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa79a(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa875(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa7a0(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa87b(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa7a6(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa881(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa7ac(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa887(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa7b2(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa88d(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa7b8(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa893(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa7be(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa899(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa7c4(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa89f(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fadd   %st(3),%st
-	fmul   %st(5),%st
-	fldt   0xa7c6(%rip)        
+	fmul   %st(3),%st
+	fld1
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xa89f(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa7cc(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa8a5(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa7d2(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa8ab(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xa7da(%rip)        
-	fld    %st(6)
+	fldt   0xa8b3(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xa7dc(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa8b5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xa7dc(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa8b5(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xa7dc(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa8b5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xa7dc(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa8b5(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xa7dc(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa8b5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xa7dc(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa8b5(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(3)
-	fdivp  %st,%st(2)
-	fldt   0x28(%rsp)
-	fmulp  %st,%st(2)
-	fldt   -0x8(%rsp)
-	fldt   0x18(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
-	fldt   0x98(%rsp)
 	fmul   %st(4),%st
-	faddp  %st,%st(2)
-	fldt   0x48(%rsp)
-	fxch   %st(1)
-	fld    %st(0)
-	fstpt  0xe8(%rsp)
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fmul   %st(1),%st
+	fldt   -0x18(%rsp)
+	fmul   %st(5),%st
+	faddp  %st,%st(1)
+	fldt   0x88(%rsp)
+	fldt   0x8(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fstpt  -0x8(%rsp)
-	fldt   0x9cb4(%rip)        
+	fldt   0x98(%rsp)
+	fmul   %st(3),%st
+	faddp  %st,%st(1)
+	fstpt  -0x18(%rsp)
+	fldt   0x9d97(%rip)        
 	fmul   %st(3),%st
-	fldt   0x9cbc(%rip)        
+	fldt   0x9d9f(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(4),%st
-	fldt   0x9cc0(%rip)        
+	fldt   0x9da3(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
 	fsubp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9cc2(%rip)        
+	fldt   0x9da5(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9cc8(%rip)        
+	fldt   0x9dab(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fadd   %st(1),%st
+	fld1
+	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9cca(%rip)        
+	fldt   0x9dab(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9cd0(%rip)        
+	fldt   0x9db1(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9cd6(%rip)        
+	fldt   0x9db7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9cdc(%rip)        
+	fldt   0x9dbd(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9ce2(%rip)        
+	fldt   0x9dc3(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9cea(%rip)        
+	fldt   0x9dcb(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cec(%rip)        
+	fldt   0x9dcd(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cec(%rip)        
+	fldt   0x9dcd(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cec(%rip)        
+	fldt   0x9dcd(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cec(%rip)        
+	fldt   0x9dcd(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cec(%rip)        
+	fldt   0x9dcd(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	flds   -0x2c(%rsp)
+	fldz
 	fadd   %st,%st(1)
 	fxch   %st(2)
 	fdivp  %st,%st(1)
 	fstpt  0xa8(%rsp)
-	fldt   0x9cdb(%rip)        
+	fldt   0x9dbe(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
-	fldt   0x9ce1(%rip)        
+	fldt   0x9dc4(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ce3(%rip)        
+	fldt   0x9dc6(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ce9(%rip)        
+	fldt   0x9dcc(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cef(%rip)        
+	fldt   0x9dd2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cf5(%rip)        
+	fldt   0x9dd8(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cfb(%rip)        
+	fldt   0x9dde(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fld1
+	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cfd(%rip)        
+	fldt   0x9dde(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d03(%rip)        
+	fldt   0x9de4(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d09(%rip)        
+	fldt   0x9dea(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9d11(%rip)        
+	fldt   0x9df2(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d13(%rip)        
+	fldt   0x9df4(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d13(%rip)        
+	fldt   0x9df4(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d13(%rip)        
+	fldt   0x9df4(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d13(%rip)        
+	fldt   0x9df4(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d13(%rip)        
+	fldt   0x9df4(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(2),%st
-	fdivrp %st,%st(1)
+	faddp  %st,%st(2)
+	fdivp  %st,%st(1)
 	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x58(%rsp)
+	fldt   0x28(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x88(%rsp)
+	fldt   0x68(%rsp)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x38(%rsp)
+	fldt   0x18(%rsp)
 	fldt   0xa8(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fstpt  0x58(%rsp)
-	fldt   0xa5cb(%rip)        
-	fmul   %st(4),%st
-	fldt   0xa5d3(%rip)        
+	fstpt  0xb8(%rsp)
+	fldt   0xa6ac(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa6b4(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa5d9(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa6ba(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa5df(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa6c0(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa5e5(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa6c6(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa5eb(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa6cc(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa5f1(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa6d2(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa5f7(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa6d8(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0xa5f9(%rip)        
+	fmul   %st(3),%st
+	fld1
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0xa6d8(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa5ff(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa6de(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa605(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa6e4(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa60b(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa6ea(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0xa611(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa6f0(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xa619(%rip)        
-	fld    %st(5)
+	fldt   0xa6f8(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa61b(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa6fa(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa61b(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa6fa(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa61b(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa6fa(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa61b(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa6fa(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa61b(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa6fa(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa61b(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa6fa(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fadd   %st(2),%st
-	fdivrp %st,%st(1)
-	fldt   0xa617(%rip)        
 	fmul   %st(5),%st
-	fldt   0xa61f(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(2)
+	fdivp  %st,%st(1)
+	fstpt  0x68(%rsp)
+	fldt   0xa6ee(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa6f6(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa625(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa6fc(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa62b(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa702(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa631(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa708(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa637(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa70e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa63d(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa714(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa643(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa71a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fadd   %st(3),%st
-	fmul   %st(5),%st
-	fldt   0xa645(%rip)        
+	fmul   %st(4),%st
+	fld1
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa71a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa64b(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa720(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa651(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa726(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa657(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa72c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa65d(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa732(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0xa665(%rip)        
-	fld    %st(6)
+	fldt   0xa73a(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xa667(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa73c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0xa667(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa73c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0xa667(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa73c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0xa667(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa73c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0xa667(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa73c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0xa667(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa73c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	faddp  %st,%st(3)
-	fdivp  %st,%st(2)
-	fxch   %st(1)
-	fmul   %st(3),%st
-	fldt   0x68(%rsp)
-	fldt   0x18(%rsp)
-	fmulp  %st,%st(1)
-	fldt   0x98(%rsp)
-	fldt   0x28(%rsp)
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	faddp  %st,%st(2)
+	fdivp  %st,%st(1)
+	fldt   0x8(%rsp)
 	fmulp  %st,%st(1)
+	fldt   0x48(%rsp)
+	fmul   %st(5),%st
+	fldt   0x88(%rsp)
+	fmul   %st(3),%st
 	faddp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x48(%rsp)
-	fld    %st(0)
-	fxch   %st(3)
-	fld    %st(0)
-	fstpt  0x48(%rsp)
-	fmulp  %st,%st(3)
-	fxch   %st(1)
-	faddp  %st,%st(2)
-	fldt   0x9ac0(%rip)        
-	fld    %st(5)
+	fldt   0x68(%rsp)
+	fmul   %st(3),%st
+	faddp  %st,%st(1)
+	fstpt  0x28(%rsp)
+	fldt   0x9ba3(%rip)        
+	fld    %st(3)
 	fmul   %st(1),%st
-	fldt   0x9ac6(%rip)        
+	fldt   0x9ba9(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9acc(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9baf(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9ad2(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bb5(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9ad8(%rip)        
-	fadd   %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9bbb(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fld1
+	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsub   %st(5),%st
-	fmul   %st(7),%st
-	faddp  %st,%st(5)
-	fxch   %st(4)
-	fmul   %st(6),%st
-	fsubp  %st,%st(4)
-	fxch   %st(3)
 	fmul   %st(5),%st
-	fldt   0x9aac(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9a92(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ba5(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9a78(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9b8b(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(3)
-	fldt   0x9aac(%rip)        
-	fld    %st(5)
-	fmul   %st(1),%st
+	fmul   %st(4),%st
+	fldt   0x9b71(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b57(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9aae(%rip)        
+	fmul   %st(4),%st
+	fsubp  %st,%st(1)
+	fldt   0x9b8b(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9b83(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b89(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9aae(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b89(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9aae(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b89(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9aae(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b89(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9aae(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b89(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadds  -0x2c(%rsp)
-	fdivrp %st,%st(3)
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fldt   0x18(%rsp)
+	fmulp  %st,%st(1)
 	fldt   0x38(%rsp)
-	fmulp  %st,%st(3)
-	fldt   0xc8(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0xd8(%rsp)
+	fldt   0x78(%rsp)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	fldt   -0x58(%rsp)
 	fldt   0xa8(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	faddp  %st,%st(3)
-	fldt   0xa535(%rip)        
-	fmul   %st(5),%st
-	fldt   0xa53d(%rip)        
+	faddp  %st,%st(1)
+	fldt   0xa616(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa61e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa543(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa624(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa549(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa62a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa54f(%rip)        
-	fadd   %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(6),%st
-	fldt   0xa553(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa630(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa636(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xa559(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa63c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0xa539(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa61c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa50b(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa602(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa5e8(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa4f1(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa5ce(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa4d7(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa5b4(%rip)        
 	faddp  %st,%st(1)
-	fmulp  %st,%st(5)
-	fldt   0xa4bd(%rip)        
-	fsubrp %st,%st(5)
-	fldt   0xb8(%rsp)
-	fdivrp %st,%st(5)
 	fmulp  %st,%st(4)
-	fldt   0x78(%rsp)
-	fldt   0x18(%rsp)
+	fldt   0xa59a(%rip)        
+	fsubrp %st,%st(4)
+	fldt   0xc8(%rsp)
+	fdivrp %st,%st(4)
+	fxch   %st(3)
+	fmulp  %st,%st(2)
+	fldt   0x58(%rsp)
+	fmulp  %st,%st(4)
+	fldt   0x98(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0xe8(%rsp)
-	fldt   0x28(%rsp)
+	faddp  %st,%st(3)
+	fldt   0x68(%rsp)
+	fldt   0x8(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x48(%rsp)
-	fmulp  %st,%st(4)
 	faddp  %st,%st(3)
-	fxch   %st(3)
 	faddp  %st,%st(2)
 	test   %esi,%esi
-	jle    470f <polyreg7+0x12af>
-	fldt   0x8(%rsp)
+	jle    4623 <polyreg7+0x1293>
+	fldt   -0x8(%rsp)
 	movslq %esi,%rsi
 	xor    %eax,%eax
-	fldt   0x58(%rsp)
-	cs nopw 0x0(%rax,%rax,1)
+	fldt   0xb8(%rsp)
+	fldt   0x28(%rsp)
+	nopl   0x0(%rax)
 	mov    %eax,-0x78(%rsp)
 	fildl  -0x78(%rsp)
-	fmul   %st(2),%st
+	fmul   %st(3),%st
 	fld1
 	fsubrp %st,%st(1)
-	fld    %st(4)
-	fmul   %st(1),%st
-	fadd   %st(4),%st
+	fld    %st(5)
 	fmul   %st(1),%st
-	fadd   %st(6),%st
+	fadd   %st(5),%st
 	fmul   %st(1),%st
 	fadd   %st(2),%st
 	fmul   %st(1),%st
-	fldt   -0x8(%rsp)
-	faddp  %st,%st(1)
+	fadd   %st(3),%st
 	fmul   %st(1),%st
 	fldt   -0x18(%rsp)
 	faddp  %st,%st(1)
 	fmul   %st(1),%st
 	fldt   -0x28(%rsp)
 	faddp  %st,%st(1)
+	fmul   %st(1),%st
+	fldt   -0x38(%rsp)
+	faddp  %st,%st(1)
 	fmulp  %st,%st(1)
 	fldt   -0x48(%rsp)
 	faddp  %st,%st(1)
 	fsubrl (%rdi,%rax,8)
 	fstpl  (%rdx,%rax,8)
 	add    $0x1,%rax
 	cmp    %rax,%rsi
-	jne    46c0 <polyreg7+0x1260>
-	fstp   %st(0)
+	jne    45d0 <polyreg7+0x1240>
+	fstp   %st(2)
 	fstp   %st(0)
+	fstpt  0x28(%rsp)
 	fldt   -0x48(%rsp)
 	fstpl  -0x78(%rsp)
-	fldt   -0x28(%rsp)
+	fldt   -0x38(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	fldt   -0x18(%rsp)
+	fldt   -0x28(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	movups %xmm0,(%r8)
+	movups %xmm0,(%rcx)
 	fstpl  -0x78(%rsp)
-	fldt   -0x8(%rsp)
+	fldt   -0x18(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	fldt   0x58(%rsp)
+	fldt   0xb8(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	movups %xmm0,0x10(%r8)
+	movups %xmm0,0x10(%rcx)
 	fstpl  -0x78(%rsp)
-	fxch   %st(2)
+	fldt   0x28(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	fxch   %st(1)
 	movhpd -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	movups %xmm0,0x20(%r8)
+	movups %xmm0,0x20(%rcx)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	movups %xmm0,0x30(%r8)
-	add    $0x100,%rsp
+	movups %xmm0,0x30(%rcx)
+	add    $0xe0,%rsp
 	ret
-	nopw   0x0(%rax,%rax,1)
-	pxor   %xmm2,%xmm2
-	movss  %xmm2,-0x2c(%rsp)
-	flds   -0x2c(%rsp)
-	fld    %st(0)
+	nopl   (%rax)
+	fldz
 	fld    %st(0)
-	fstpt  0x48(%rsp)
+	fstpt  0x18(%rsp)
+	fldt   0x18(%rsp)
+	fstpt  0x8(%rsp)
+	fldt   0x8(%rsp)
+	fstpt  -0x58(%rsp)
+	fldt   -0x58(%rsp)
 	fld    %st(0)
-	fstpt  0x38(%rsp)
-	fld    %st(1)
+	fstpt  -0x68(%rsp)
+	fldt   -0x68(%rsp)
 	fld    %st(0)
-	fstpt  -0x58(%rsp)
-	fxch   %st(2)
-	fstpt  0x28(%rsp)
-	fldt   0x28(%rsp)
+	fstpt  -0x78(%rsp)
+	fxch   %st(3)
 	fxch   %st(2)
-	fstpt  -0x68(%rsp)
 	fxch   %st(1)
-	fstpt  0x18(%rsp)
-	fldt   0x18(%rsp)
-	fstpt  -0x78(%rsp)
-	jmp    353c <polyreg7+0xdc>
+	jmp    344c <polyreg7+0xbc>
 	nop
 
-00000000000047e0 <polyreg8>:
+00000000000046e0 <polyreg8>:
 polyreg8():
-	sub    $0x140,%rsp
-	mov    %rcx,%r8
+	sub    $0x130,%rsp
 	mov    %esi,-0x78(%rsp)
 	fildl  -0x78(%rsp)
 	fld    %st(0)
 	fld1
 	fsubrp %st,%st(1)
-	fdivrs 0x8832(%rip)        
+	fdivrs 0x8935(%rip)        
 	fstpt  0x18(%rsp)
 	test   %esi,%esi
-	jle    6418 <polyreg8+0x1c38>
+	jle    6330 <polyreg8+0x1c50>
 	fldz
-	movslq %esi,%rcx
+	movslq %esi,%r8
 	xor    %eax,%eax
 	fld    %st(0)
 	fld    %st(1)
-	fld    %st(2)
-	fld    %st(3)
-	fld    %st(4)
+	fstpt  0x28(%rsp)
+	fldt   0x28(%rsp)
 	fstpt  -0x48(%rsp)
 	fldt   -0x48(%rsp)
-	fstpt  -0x68(%rsp)
-	fldt   -0x68(%rsp)
+	fld    %st(0)
 	fstpt  -0x58(%rsp)
 	fldt   -0x58(%rsp)
+	fld    %st(0)
+	fstpt  -0x68(%rsp)
+	fldt   -0x68(%rsp)
 	fstpt  -0x78(%rsp)
-	fldt   -0x78(%rsp)
-	fxch   %st(6)
+	fxch   %st(4)
 	fstpt  -0x28(%rsp)
-	fxch   %st(5)
-	fstps  -0x18(%rsp)
+	fld    %st(3)
 	nopw   0x0(%rax,%rax,1)
 	mov    %eax,-0x38(%rsp)
 	fildl  -0x38(%rsp)
 	fldt   0x18(%rsp)
 	fmulp  %st,%st(1)
 	fld1
 	fsubrp %st,%st(1)
 	fldl   (%rdi,%rax,8)
 	fldt   -0x78(%rsp)
 	add    $0x1,%rax
 	fadd   %st(1),%st
 	fstpt  -0x78(%rsp)
 	fmul   %st(1),%st
+	fldt   -0x68(%rsp)
+	fadd   %st(1),%st
+	fstpt  -0x68(%rsp)
+	fmul   %st(1),%st
+	fadd   %st,%st(6)
+	fmul   %st(1),%st
 	fldt   -0x58(%rsp)
 	fadd   %st(1),%st
 	fstpt  -0x58(%rsp)
 	fmul   %st(1),%st
-	fldt   -0x68(%rsp)
-	fadd   %st(1),%st
-	fstpt  -0x68(%rsp)
+	fadd   %st,%st(3)
 	fmul   %st(1),%st
 	fldt   -0x48(%rsp)
 	fadd   %st(1),%st
 	fstpt  -0x48(%rsp)
 	fmul   %st(1),%st
-	fadd   %st,%st(5)
-	fmul   %st(1),%st
-	fadd   %st,%st(6)
-	fmul   %st(1),%st
 	fadd   %st,%st(2)
 	fmul   %st(1),%st
-	fadd   %st,%st(3)
+	fadd   %st,%st(5)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(3)
-	cmp    %rax,%rcx
-	jne    4850 <polyreg8+0x70>
+	cmp    %rax,%r8
+	jne    4748 <polyreg8+0x68>
 	fldt   -0x28(%rsp)
-	fxch   %st(4)
-	fstpt  0x28(%rsp)
-	fxch   %st(4)
-	fstpt  0x48(%rsp)
-	fxch   %st(3)
+	fxch   %st(5)
 	fstpt  0x38(%rsp)
-	fxch   %st(2)
-	fstpt  0x58(%rsp)
+	fxch   %st(1)
+	fstpt  0x48(%rsp)
+	fstpt  0x28(%rsp)
 	fxch   %st(1)
 	fstpt  0x68(%rsp)
-	flds   -0x18(%rsp)
-	fldt   0xa2c4(%rip)        
-	fmul   %st(2),%st
-	fldt   0xa2cc(%rip)        
+	fstpt  0x58(%rsp)
+	fldt   0xa3c4(%rip)        
+	fmul   %st(1),%st
+	fldt   0xa3cc(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xa2d2(%rip)        
+	fmul   %st(1),%st
+	fldt   0xa3d2(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xa2d8(%rip)        
+	fmul   %st(1),%st
+	fldt   0xa3d8(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xa2de(%rip)        
+	fmul   %st(1),%st
+	fldt   0xa3de(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xa2e4(%rip)        
+	fmul   %st(1),%st
+	fldt   0xa3e4(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xa2ea(%rip)        
+	fmul   %st(1),%st
+	fldt   0xa3ea(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fsubs  0x8710(%rip)        
-	fmul   %st(2),%st
+	fmul   %st(1),%st
+	flds   0x8820(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(1),%st
 	fld1
 	fadd   %st,%st(1)
-	fldt   0xa2e4(%rip)        
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fldt   0xa3e2(%rip)        
+	fmul   %st(3),%st
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(1)
 	fmul   %st(4),%st
-	fldt   0xa2e8(%rip)        
+	fldt   0xa3e2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0xa2ea(%rip)        
+	fldt   0xa3e4(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0xa2ec(%rip)        
+	fldt   0xa3e6(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0xa2ee(%rip)        
+	fldt   0xa3e8(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fdivrp %st,%st(2)
-	fxch   %st(1)
-	fstpt  -0x18(%rsp)
-	fldt   0xa2ea(%rip)        
-	fmul   %st(3),%st
-	fldt   0xa2f2(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xa2f8(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xa2fe(%rip)        
-	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xa304(%rip)        
-	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xa30a(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(3),%st
 	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0xa30c(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xa312(%rip)        
-	faddp  %st,%st(1)
-	fldt   0xa31a(%rip)        
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fdivrp %st,%st(3)
+	fldt   0xa3ea(%rip)        
 	fmul   %st(4),%st
-	fldt   0xa31e(%rip)        
+	fldt   0xa3f2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fldt   0xa3f8(%rip)        
+	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa320(%rip)        
+	fldt   0xa3fe(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fldt   0xa404(%rip)        
+	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0xa322(%rip)        
+	fldt   0xa40a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fldt   0xa324(%rip)        
-	faddp  %st,%st(1)
+	fldt   0xa40c(%rip)        
+	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fldt   0xa412(%rip)        
+	faddp  %st,%st(1)
+	fldt   0xa41a(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xa41e(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xa420(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xa422(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xa424(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(2),%st
 	fdivrp %st,%st(1)
 	fstpt  0x8(%rsp)
-	fldt   0xa322(%rip)        
-	fmul   %st(3),%st
-	fldt   0xa32a(%rip)        
+	fldt   0xa422(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa42a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xa330(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa430(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xa336(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa436(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xa33c(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa43c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0xa342(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa442(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xa344(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(2),%st
+	fmul   %st(4),%st
+	fldt   0xa444(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0xa34a(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa44a(%rip)        
 	faddp  %st,%st(1)
-	fldt   0xa352(%rip)        
-	fmul   %st(3),%st
+	fldt   0xa452(%rip)        
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fldt   0xa356(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa456(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fldt   0xa358(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa458(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fldt   0xa35a(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa45a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fldt   0xa35c(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa45c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(2),%st
-	fdivrp %st,%st(1)
-	flds   0x85a2(%rip)        
+	fmul   %st(5),%st
+	faddp  %st,%st(2)
+	fdivp  %st,%st(1)
+	fstpt  0x78(%rsp)
+	flds   0x86ae(%rip)        
 	fld    %st(3)
 	fmul   %st(1),%st
-	flds   0x859c(%rip)        
+	flds   0x86a8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
-	flds   0x8594(%rip)        
-	fadd   %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(6),%st
-	flds   0x858c(%rip)        
+	fldt   0xb464(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xb46a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fadds  0x8584(%rip)        
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
+	fadds  0x868a(%rip)        
+	fmul   %st(6),%st
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xb442(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
 	faddp  %st,%st(1)
-	fldt   0xa31a(%rip)        
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fldt   0xa412(%rip)        
 	fmul   %st(4),%st
-	fldt   0xa31e(%rip)        
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(1)
+	fmul   %st(5),%st
+	fldt   0xa412(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0xa320(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(1),%st
+	fmul   %st(5),%st
+	fldt   0xa414(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0xa322(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(1),%st
+	fmul   %st(5),%st
+	fldt   0xa416(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
+	fadd   %st(1),%st
+	fmul   %st(5),%st
 	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fld1
-	fadd   %st,%st(1)
-	fxch   %st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(1),%st
 	fdivrp %st,%st(2)
 	fxch   %st(1)
-	fstpt  0x78(%rsp)
-	fldt   0xa312(%rip)        
+	fstpt  0x88(%rsp)
+	fldt   0xa407(%rip)        
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0xa316(%rip)        
+	fldt   0xa40b(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0xa318(%rip)        
+	fldt   0xa40d(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0xa31a(%rip)        
+	fldt   0xa40f(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	faddp  %st,%st(1)
-	fldt   0xa31a(%rip)        
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0xa31e(%rip)        
+	fadd   %st(2),%st
+	fldt   0xa40f(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xa413(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0xa320(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xa415(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0xa322(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xa417(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0xa324(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0xa419(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fdivrp %st,%st(1)
+	fmul   %st(5),%st
+	faddp  %st,%st(2)
+	fdivp  %st,%st(1)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   -0x68(%rsp)
-	fldt   -0x18(%rsp)
+	fxch   %st(2)
+	fld    %st(0)
+	fstpt  -0x18(%rsp)
+	fldt   0x38(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x28(%rsp)
+	faddp  %st,%st(2)
 	fldt   0x8(%rsp)
+	fldt   0x48(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x38(%rsp)
-	fxch   %st(2)
-	fld    %st(0)
-	fstpt  0x128(%rsp)
-	fmulp  %st,%st(2)
-	faddp  %st,%st(1)
-	fldt   0x68(%rsp)
-	fld    %st(0)
+	faddp  %st,%st(2)
 	fldt   0x78(%rsp)
+	fldt   0x28(%rsp)
+	fmulp  %st,%st(1)
+	faddp  %st,%st(2)
+	fldt   0x58(%rsp)
+	fldt   0x88(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(2)
 	fxch   %st(1)
 	fstpt  -0x38(%rsp)
-	fldt   0x9481(%rip)        
-	fmul   %st(3),%st
-	fldt   0x9489(%rip)        
+	fldt   0x9578(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9580(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x948f(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9586(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9495(%rip)        
+	fmul   %st(2),%st
+	fldt   0x958c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x949b(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9592(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x94a1(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9598(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x94a7(%rip)        
+	fmul   %st(2),%st
+	fldt   0x959e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x94ad(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95a4(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x94b3(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95aa(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x94b9(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95b0(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x94bf(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95b6(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x94c5(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95bc(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fld1
-	fadd   %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(4),%st
-	fldt   0x83f3(%rip)        
-	fsubr  %st,%st(1)
-	fldt   0x94bb(%rip)        
-	fld    %st(6)
+	fmul   %st(2),%st
+	fadd   %st(1),%st
+	fmul   %st(2),%st
+	fldt   0x84ee(%rip)        
+	fsubrp %st,%st(1)
+	fldt   0x95b6(%rip)        
+	fld    %st(3)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x94bd(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95b8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x94bd(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95b8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x94bd(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95b8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x94bd(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95b8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x94bd(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95b8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x94bd(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95b8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fadd   %st(5),%st
-	fdivrp %st,%st(2)
-	fxch   %st(1)
+	fmul   %st(3),%st
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
 	fstpt  -0x8(%rsp)
-	fldt   0x94b3(%rip)        
-	fmul   %st(5),%st
-	fldt   0x94bb(%rip)        
+	fldt   0x95ae(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95b6(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94c1(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95bc(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94c7(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95c2(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94cd(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95c8(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94d3(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95ce(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94d9(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95d4(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94df(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95da(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94e5(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95e0(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94eb(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95e6(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fadd   %st(2),%st
-	fmul   %st(5),%st
-	fldt   0x94ed(%rip)        
+	fmul   %st(2),%st
+	fadd   %st(1),%st
+	fmul   %st(2),%st
+	fldt   0x95e8(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94f3(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95ee(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94f9(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95f4(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9501(%rip)        
-	fld    %st(6)
+	fldt   0x95fc(%rip)        
+	fld    %st(3)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9503(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95fe(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9503(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95fe(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9503(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95fe(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9503(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95fe(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9503(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95fe(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9503(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95fe(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldz
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fadd   %st(5),%st
 	fdivrp %st,%st(1)
-	fstpt  0x68(%rsp)
-	fldt   0x94fb(%rip)        
-	fld    %st(5)
+	fstpt  0x98(%rsp)
+	fldt   0x95f1(%rip)        
+	fld    %st(2)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94fd(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95f3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(3),%st
 	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94fd(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95f3(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(3),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94fd(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95f3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(3),%st
 	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94fd(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95f3(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(3),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94fd(%rip)        
+	fmul   %st(2),%st
+	fldt   0x95f3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(3),%st
 	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fadd   %st(2),%st
-	fmul   %st(5),%st
-	faddp  %st,%st(2)
-	fxch   %st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fldt   0x94f1(%rip)        
-	fmul   %st(5),%st
-	fldt   0x94f9(%rip)        
+	fmul   %st(2),%st
+	fadd   %st(1),%st
+	fmul   %st(2),%st
+	fadd   %st(1),%st
+	fmul   %st(2),%st
+	fldz
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x94ff(%rip)        
+	fldt   0x95e7(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95ef(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9505(%rip)        
+	fmul   %st(3),%st
+	fldt   0x95f5(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0x95fb(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x950b(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9601(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9511(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9607(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9517(%rip)        
+	fmul   %st(3),%st
+	fldt   0x960d(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x951d(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9613(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9523(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9619(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9529(%rip)        
+	fmul   %st(3),%st
+	fldt   0x961f(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x952f(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9625(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9535(%rip)        
+	fmul   %st(3),%st
+	fldt   0x962b(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x953b(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9631(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9541(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9637(%rip)        
 	fsubrp %st,%st(1)
 	fxch   %st(1)
 	fld    %st(0)
-	fstpt  0x118(%rsp)
+	fstpt  0xd8(%rsp)
 	fdivrp %st,%st(1)
-	fstpt  0x88(%rsp)
-	fldt   0x9535(%rip)        
-	fld    %st(4)
+	fldt   0x9632(%rip)        
+	fld    %st(3)
 	fmul   %st(1),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9537(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9634(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9537(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0x9634(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9537(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0x9634(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9537(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0x9634(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9537(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0x9634(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
-	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fld1
-	fadd   %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(1)
-	fldt   0x952d(%rip)        
-	fld    %st(5)
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fadd   %st(2),%st
+	fmul   %st(3),%st
+	fsub   %st(2),%st
+	fldt   0x962e(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x952f(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9630(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x952f(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9630(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x952f(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9630(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x952f(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9630(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x952f(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9630(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x952f(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9630(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   -0x58(%rsp)
+	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
-	fldt   -0x48(%rsp)
+	fldt   -0x58(%rsp)
 	fldt   -0x8(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x48(%rsp)
-	fldt   0x68(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x58(%rsp)
-	fldt   0x88(%rsp)
+	fldt   -0x48(%rsp)
+	fldt   0x98(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
+	fldt   0x68(%rsp)
+	fld    %st(0)
+	fxch   %st(3)
+	fld    %st(0)
+	fstpt  0xe8(%rsp)
+	fmulp  %st,%st(3)
+	fxch   %st(1)
+	faddp  %st,%st(2)
+	fxch   %st(1)
 	fstpt  -0x28(%rsp)
-	fldt   0x9eda(%rip)        
-	fmul   %st(4),%st
-	fldt   0x9ee2(%rip)        
+	fldt   0x9fcc(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9fd4(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9ee8(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9fda(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9eee(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9fe0(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9ef4(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9fe6(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9efa(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9fec(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9f00(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9ff2(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9f06(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9ff8(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9f0c(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9ffe(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9f12(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa004(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9f18(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa00a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9f1e(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa010(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9f24(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa016(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9f2a(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa01c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9f30(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa022(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9f30(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(2),%st
+	fmul   %st(3),%st
+	fldt   0xa024(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9f36(%rip)        
+	fmul   %st(3),%st
+	fldt   0xa02a(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9f3e(%rip)        
-	fld    %st(5)
+	fldt   0xa032(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f40(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa034(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9f40(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa034(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9f40(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa034(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9f40(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa034(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9f40(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa034(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9f40(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa034(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9f40(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa034(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9f40(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa034(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   0x9f3c(%rip)        
-	fmul   %st(5),%st
-	fldt   0x9f44(%rip)        
+	fldt   0xa02e(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa036(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f4a(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa03c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f50(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa042(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f56(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa048(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f5c(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa04e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f62(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa054(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f68(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa05a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f6e(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa060(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f74(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa066(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f7a(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa06c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f80(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa072(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f86(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa078(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f86(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(3),%st
+	fmul   %st(4),%st
+	fldt   0xa07a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f8c(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa080(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f92(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa086(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9f98(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa08c(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9fa0(%rip)        
-	fld    %st(6)
+	fldt   0xa094(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9fa2(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa096(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9fa2(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa096(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9fa2(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa096(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9fa2(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa096(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9fa2(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa096(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9fa2(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa096(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9fa2(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa096(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9fa2(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa096(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fadd   %st(5),%st
-	fdivrp %st,%st(1)
-	fstpt  0x98(%rsp)
-	fldt   0x9f97(%rip)        
-	fmul   %st(5),%st
-	fldt   0x9f9f(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9fa5(%rip)        
+	fldz
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fab(%rip)        
+	fdivrp %st,%st(1)
+	fstpt  0xa8(%rsp)
+	fldt   0xa089(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa091(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa097(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0xa09d(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fb1(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0a3(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fb7(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0a9(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fbd(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0af(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fc3(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0b5(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fc9(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0bb(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fcf(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0c1(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fd5(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0c7(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fdb(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0cd(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fe1(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0d3(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fe1(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(3),%st
+	fmul   %st(4),%st
+	fldt   0xa0d5(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fe7(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0db(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9fed(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0e1(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9ff3(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0e7(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9ffb(%rip)        
-	fld    %st(6)
+	fldt   0xa0ef(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9ffd(%rip)        
+	fmul   %st(5),%st
+	fldt   0xa0f1(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9ffd(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa0f1(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9ffd(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa0f1(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9ffd(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa0f1(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9ffd(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa0f1(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9ffd(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa0f1(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9ffd(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa0f1(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9ffd(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0xa0f1(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fadd   %st(5),%st
-	fdivrp %st,%st(1)
-	fstpt  0xa8(%rsp)
-	fldt   0x9ff2(%rip)        
+	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9ffa(%rip)        
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  0xb8(%rsp)
+	fldt   0xa0e4(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0ec(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa000(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0f2(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa006(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0f8(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa00c(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa0fe(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa012(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa104(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa018(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa10a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa01e(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa110(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa024(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa116(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa02a(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa11c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa030(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa122(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa036(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa128(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa03c(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa12e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0xa042(%rip)        
+	fmul   %st(4),%st
+	fldt   0xa134(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fsubp  %st,%st(2)
-	fldt   0xa040(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(3),%st
+	fmul   %st(4),%st
+	fldt   0x7d06(%rip)        
+	fsubrp %st,%st(1)
+	fldt   0xa12e(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa042(%rip)        
+	fldt   0xa130(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa042(%rip)        
+	fldt   0xa130(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa042(%rip)        
+	fldt   0xa130(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa042(%rip)        
+	fldt   0xa130(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa042(%rip)        
+	fldt   0xa130(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa042(%rip)        
+	fldt   0xa130(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0xa042(%rip)        
+	fldt   0xa130(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
-	fdivrp %st,%st(2)
-	fldt   -0x68(%rsp)
-	fmulp  %st,%st(2)
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fldt   0x38(%rsp)
+	fmulp  %st,%st(1)
 	fldt   -0x18(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
-	fldt   0x28(%rsp)
-	fmul   %st(1),%st
-	faddp  %st,%st(2)
-	fldt   0x38(%rsp)
-	fldt   0x98(%rsp)
+	faddp  %st,%st(1)
+	fxch   %st(1)
+	fld    %st(0)
+	fstpt  0xf8(%rsp)
+	fldt   0x48(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
-	fld    %st(2)
+	faddp  %st,%st(1)
 	fldt   0xa8(%rsp)
+	fldt   0x28(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
-	fxch   %st(1)
+	faddp  %st,%st(1)
+	fldt   0x58(%rsp)
+	fldt   0xb8(%rsp)
+	fmulp  %st,%st(1)
+	faddp  %st,%st(1)
 	fstpt  -0x18(%rsp)
-	fldt   0x8fe2(%rip)        
-	fmul   %st(4),%st
-	fldt   0x8fea(%rip)        
+	fldt   0x90c3(%rip)        
+	fmul   %st(3),%st
+	fldt   0x90cb(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8ff0(%rip)        
+	fmul   %st(3),%st
+	fldt   0x90d1(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8ff6(%rip)        
+	fmul   %st(3),%st
+	fldt   0x90d7(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8ffc(%rip)        
+	fmul   %st(3),%st
+	fldt   0x90dd(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9002(%rip)        
+	fmul   %st(3),%st
+	fldt   0x90e3(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9008(%rip)        
+	fmul   %st(3),%st
+	fldt   0x90e9(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x900e(%rip)        
+	fmul   %st(3),%st
+	fldt   0x90ef(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9014(%rip)        
+	fmul   %st(3),%st
+	fldt   0x90f5(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x901a(%rip)        
+	fmul   %st(3),%st
+	fldt   0x90fb(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x901a(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(2),%st
+	fmul   %st(3),%st
+	fldt   0x90fd(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9020(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9103(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9026(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9109(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x902e(%rip)        
-	fld    %st(5)
+	fldt   0x9111(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9030(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9113(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9030(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9113(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9030(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9113(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9030(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9113(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9030(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9113(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9030(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9113(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   0x902c(%rip)        
-	fmul   %st(5),%st
-	fldt   0x9034(%rip)        
+	fstpt  0xc8(%rsp)
+	fldt   0x9106(%rip)        
+	fmul   %st(3),%st
+	fldt   0x910e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x903a(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9114(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9040(%rip)        
+	fmul   %st(3),%st
+	fldt   0x911a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9046(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9120(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x904c(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9126(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9052(%rip)        
+	fmul   %st(3),%st
+	fldt   0x912c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9058(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9132(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9058(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(2),%st
+	fmul   %st(3),%st
+	fldt   0x9134(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x905e(%rip)        
+	fmul   %st(3),%st
+	fldt   0x913a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9064(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9140(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x906a(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9146(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9070(%rip)        
+	fmul   %st(3),%st
+	fldt   0x914c(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9078(%rip)        
-	fld    %st(6)
+	fldt   0x9154(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x907a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9156(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x907a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9156(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x907a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9156(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x907a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9156(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x907a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9156(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x907a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9156(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fadd   %st(5),%st
 	fdivrp %st,%st(1)
-	fstpt  0xb8(%rsp)
-	fldt   0x906f(%rip)        
-	fmul   %st(5),%st
-	fldt   0x9077(%rip)        
+	fldt   0x9150(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9158(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x907d(%rip)        
+	fmul   %st(4),%st
+	fldt   0x915e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9083(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9164(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9089(%rip)        
+	fmul   %st(4),%st
+	fldt   0x916a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x908f(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9170(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9095(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9176(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x909b(%rip)        
+	fmul   %st(4),%st
+	fldt   0x917c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x90a1(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9182(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x90a7(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9188(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x90a7(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(3),%st
+	fmul   %st(4),%st
+	fldt   0x918a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x90ad(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9190(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x90b3(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9196(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x90bb(%rip)        
-	fld    %st(6)
+	fldt   0x919e(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x90bd(%rip)        
+	fmul   %st(5),%st
+	fldt   0x91a0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x90bd(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x91a0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x90bd(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x91a0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x90bd(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x91a0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x90bd(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x91a0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x90bd(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x91a0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fadd   %st(5),%st
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   -0x48(%rsp)
+	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
 	fldt   -0x8(%rsp)
-	fldt   -0x58(%rsp)
+	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x48(%rsp)
-	fmul   %st(2),%st
-	faddp  %st,%st(1)
-	fldt   0x58(%rsp)
-	fldt   0xb8(%rsp)
+	fldt   -0x48(%rsp)
+	fldt   0xc8(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
+	fxch   %st(1)
+	fld    %st(0)
+	fstpt  0x108(%rsp)
+	fmulp  %st,%st(2)
+	faddp  %st,%st(1)
 	fstpt  -0x8(%rsp)
-	fldt   0x9cec(%rip)        
-	fmul   %st(5),%st
-	fldt   0x9cf4(%rip)        
+	fldt   0x9dc6(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9dce(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9cfa(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9dd4(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d00(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9dda(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d06(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9de0(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d0c(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9de6(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d12(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9dec(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d18(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9df2(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d1e(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9df8(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d24(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9dfe(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d2a(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9e04(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d30(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9e0a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d36(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9e10(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d36(%rip)        
+	fmul   %st(2),%st
+	fadd   %st(1),%st
+	fmul   %st(2),%st
+	fldt   0x9e12(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d3c(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9e18(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d42(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9e1e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d48(%rip)        
+	fmul   %st(2),%st
+	fldt   0x9e24(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9d50(%rip)        
-	fld    %st(6)
+	fldt   0x9e2c(%rip)        
+	fld    %st(3)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9d52(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e2e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9d52(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e2e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9d52(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e2e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9d52(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e2e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9d52(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e2e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9d52(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e2e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9d52(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e2e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9d52(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e2e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(4),%st
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldz
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fadd   %st(5),%st
 	fdivrp %st,%st(1)
-	fstpt  0xc8(%rsp)
-	fldt   0x9d47(%rip)        
-	fmul   %st(5),%st
-	fldt   0x9d4f(%rip)        
+	fldt   0x9e28(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e30(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d55(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e36(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d5b(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e3c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d61(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e42(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d67(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e48(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d6d(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e4e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d73(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e54(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d79(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e5a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d7f(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e60(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d85(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e66(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d85(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(2),%st
+	fmul   %st(3),%st
+	fldt   0x9e68(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d8b(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e6e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d91(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e74(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d97(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e7a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9d9d(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e80(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9da3(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9e86(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9dab(%rip)        
-	fld    %st(6)
+	fldt   0x9e8e(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9dad(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9e90(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9dad(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9e90(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9dad(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9e90(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9dad(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9e90(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9dad(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9e90(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9dad(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9e90(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9dad(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9e90(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9dad(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9e90(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
+	fmul   %st(5),%st
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fadd   %st(5),%st
 	fdivrp %st,%st(1)
-	fstpt  0xd8(%rsp)
-	fldt   0x9da2(%rip)        
-	fmul   %st(5),%st
-	fldt   0x9daa(%rip)        
+	fldt   0x9e8a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9e92(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9db0(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9e98(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9db6(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9e9e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9dbc(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ea4(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9dc2(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9eaa(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9dc8(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9eb0(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9dce(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9eb6(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9dd4(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ebc(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9dda(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ec2(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9de0(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ec8(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9de6(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ece(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9dec(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ed4(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9dec(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(3),%st
+	fmul   %st(4),%st
+	fldt   0x9ed6(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9df2(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9edc(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9df8(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ee2(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9dfe(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ee8(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9e06(%rip)        
-	fld    %st(6)
+	fldt   0x9ef0(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9e08(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9ef2(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9e08(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9ef2(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9e08(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9ef2(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9e08(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9ef2(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9e08(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9ef2(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9e08(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9ef2(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9e08(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9ef2(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9e08(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9ef2(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fadd   %st(5),%st
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   0x28(%rsp)
+	fldt   0x48(%rsp)
 	fmulp  %st,%st(1)
 	fldt   0x8(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   -0x68(%rsp)
-	fmulp  %st,%st(4)
-	faddp  %st,%st(3)
-	faddp  %st,%st(2)
+	fldt   0xf8(%rsp)
 	fldt   0x38(%rsp)
-	fldt   0xc8(%rsp)
-	fmulp  %st,%st(1)
+	fmul   %st,%st(1)
+	fxch   %st(2)
+	faddp  %st,%st(1)
 	faddp  %st,%st(2)
-	fld    %st(2)
-	fldt   0xd8(%rsp)
+	fxch   %st(3)
+	fld    %st(0)
+	fstpt  0xf8(%rsp)
+	fldt   0x28(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
-	fxch   %st(1)
+	faddp  %st,%st(1)
+	fldt   0x58(%rsp)
+	fxch   %st(2)
+	fld    %st(0)
+	fstpt  0x118(%rsp)
+	fmulp  %st,%st(2)
+	faddp  %st,%st(1)
 	fstpt  0x8(%rsp)
-	fldt   0x8c88(%rip)        
-	fmul   %st(4),%st
-	fldt   0x8c90(%rip)        
+	fldt   0x8d5f(%rip)        
+	fmul   %st(3),%st
+	fldt   0x8d67(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8c96(%rip)        
+	fmul   %st(3),%st
+	fldt   0x8d6d(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8c9c(%rip)        
+	fmul   %st(3),%st
+	fldt   0x8d73(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8ca2(%rip)        
+	fmul   %st(3),%st
+	fldt   0x8d79(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8ca8(%rip)        
+	fmul   %st(3),%st
+	fldt   0x8d7f(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8cae(%rip)        
+	fmul   %st(3),%st
+	fldt   0x8d85(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8cb4(%rip)        
+	fmul   %st(3),%st
+	fldt   0x8d8b(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fld1
-	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8cb4(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(2),%st
+	fmul   %st(3),%st
+	fldt   0x8d8d(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8cba(%rip)        
+	fmul   %st(3),%st
+	fldt   0x8d93(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8cc0(%rip)        
+	fmul   %st(3),%st
+	fldt   0x8d99(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8cc6(%rip)        
+	fmul   %st(3),%st
+	fldt   0x8d9f(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8ccc(%rip)        
+	fmul   %st(3),%st
+	fldt   0x8da5(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x8cd4(%rip)        
-	fld    %st(5)
+	fldt   0x8dad(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x8cd6(%rip)        
+	fmul   %st(4),%st
+	fldt   0x8daf(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8cd6(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x8daf(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8cd6(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x8daf(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8cd6(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x8daf(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8cd6(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x8daf(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8cd6(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x8daf(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0xe8(%rsp)
-	fldt   0x8ccb(%rip)        
+	fldt   0x8da9(%rip)        
 	fmul   %st(4),%st
-	fldt   0x8cd3(%rip)        
+	fldt   0x8db1(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8cd9(%rip)        
+	fldt   0x8db7(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8cdf(%rip)        
+	fldt   0x8dbd(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8ce5(%rip)        
+	fldt   0x8dc3(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8ceb(%rip)        
+	fldt   0x8dc9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8cf1(%rip)        
+	fldt   0x8dcf(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8cf7(%rip)        
+	fldt   0x8dd5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fld1
-	faddp  %st,%st(1)
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x8cf7(%rip)        
+	fldt   0x8dd7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8cfd(%rip)        
+	fldt   0x8ddd(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8d03(%rip)        
+	fldt   0x8de3(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8d09(%rip)        
+	fldt   0x8de9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8d0f(%rip)        
+	fldt   0x8def(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x8d17(%rip)        
+	fldt   0x8df7(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8d19(%rip)        
+	fldt   0x8df9(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8d19(%rip)        
+	fldt   0x8df9(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8d19(%rip)        
+	fldt   0x8df9(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8d19(%rip)        
+	fldt   0x8df9(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8d19(%rip)        
+	fldt   0x8df9(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8d19(%rip)        
+	fldt   0x8df9(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   0x48(%rsp)
+	fldt   -0x48(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x68(%rsp)
+	fldt   0x98(%rsp)
+	fldt   -0x68(%rsp)
+	fmulp  %st,%st(1)
+	fldt   0xc8(%rsp)
 	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
-	fldt   -0x48(%rsp)
-	fmulp  %st,%st(3)
-	faddp  %st,%st(2)
 	faddp  %st,%st(1)
-	fldt   0x58(%rsp)
-	fldt   0xe8(%rsp)
-	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fstpt  0x108(%rsp)
-	fldt   0x9ba5(%rip)        
-	fmul   %st(3),%st
-	fldt   0x9bad(%rip)        
+	fldt   0x68(%rsp)
+	fld    %st(0)
+	fxch   %st(3)
+	fld    %st(0)
+	fstpt  0x98(%rsp)
+	fmulp  %st,%st(3)
+	fxch   %st(1)
+	faddp  %st,%st(2)
+	fxch   %st(1)
+	fstpt  0x68(%rsp)
+	fldt   0x9c72(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9c7a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9bb3(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9c80(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9bb9(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9c86(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9bbf(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9c8c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9bc5(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9c92(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9bcb(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9c98(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9bd1(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9c9e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9bd7(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ca4(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9bdd(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9caa(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9be3(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9cb0(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fld1
-	fadd   %st,%st(1)
-	fxch   %st(1)
 	fmul   %st(4),%st
-	fldt   0x9be1(%rip)        
+	fadd   %st(3),%st
+	fmul   %st(4),%st
+	fldt   0x9cb2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9be7(%rip)        
+	fldt   0x9cb8(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bed(%rip)        
+	fldt   0x9cbe(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bf3(%rip)        
+	fldt   0x9cc4(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bf9(%rip)        
+	fldt   0x9cca(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bff(%rip)        
+	fldt   0x9cd0(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9c07(%rip)        
+	fldt   0x9cd8(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c09(%rip)        
+	fldt   0x9cda(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c09(%rip)        
+	fldt   0x9cda(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c09(%rip)        
+	fldt   0x9cda(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c09(%rip)        
+	fldt   0x9cda(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c09(%rip)        
+	fldt   0x9cda(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c09(%rip)        
+	fldt   0x9cda(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c09(%rip)        
+	fldt   0x9cda(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c09(%rip)        
+	fldt   0x9cda(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0xf8(%rsp)
-	fldt   0x9bfe(%rip)        
-	fmul   %st(4),%st
-	fldt   0x9c06(%rip)        
+	fldt   0x9cd4(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9cdc(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c0c(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9ce2(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c12(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9ce8(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c18(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9cee(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c1e(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9cf4(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c24(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9cfa(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c2a(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9d00(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c30(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9d06(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c36(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9d0c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c3c(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9d12(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9c3e(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(4),%st
+	fmul   %st(5),%st
+	fldt   0x9d14(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9c44(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9d1a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9c4a(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9d20(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9c50(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9d26(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9c56(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9d2c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9c5c(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9d32(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9c64(%rip)        
-	fld    %st(4)
+	fldt   0x9d3a(%rip)        
+	fld    %st(6)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c66(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9d3c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(7),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c66(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9d3c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(7),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c66(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9d3c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(7),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c66(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9d3c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(7),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c66(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9d3c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(7),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c66(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9d3c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(7),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c66(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9d3c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(7),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9c66(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9d3c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(7),%st
+	faddp  %st,%st(1)
+	fmul   %st(6),%st
+	fldz
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fldt   0x38(%rsp)
+	fldt   0x28(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x128(%rsp)
+	fldt   0x78(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x98(%rsp)
-	fldt   -0x68(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0xc8(%rsp)
-	fldt   0x28(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	faddp  %st,%st(1)
-	fxch   %st(1)
-	fld    %st(0)
-	fstpt  0x68(%rsp)
+	fldt   0xa8(%rsp)
+	fmulp  %st,%st(5)
+	faddp  %st,%st(4)
 	fldt   0xf8(%rsp)
+	fldt   0x48(%rsp)
 	fmulp  %st,%st(1)
+	faddp  %st,%st(4)
+	faddp  %st,%st(3)
+	fldt   0x58(%rsp)
+	fld    %st(0)
+	fxch   %st(2)
+	fld    %st(0)
+	fstpt  0x58(%rsp)
+	fmulp  %st,%st(2)
+	fxch   %st(3)
 	faddp  %st,%st(1)
-	fldt   0x8a1c(%rip)        
-	fld    %st(3)
+	fldt   0x8af6(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
-	fldt   0x8a22(%rip)        
+	fldt   0x8afc(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8a28(%rip)        
+	fmul   %st(6),%st
+	fldt   0x8b02(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(6),%st
+	fldt   0x8b08(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(6),%st
+	fldt   0x8b0e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x8a2e(%rip)        
-	fsubr  %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(5),%st
-	fldt   0x8a32(%rip)        
-	fadd   %st,%st(1)
-	fxch   %st(1)
 	fmul   %st(6),%st
-	fldt   0x8a36(%rip)        
+	fldt   0x8b14(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x8a3c(%rip)        
+	fldt   0x8b1a(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(7),%st
 	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x8a1c(%rip)        
+	fldt   0x8afa(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fsubp  %st,%st(1)
-	fmul   %st(5),%st
+	fldt   0x8ae0(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(6),%st
+	fldt   0x8ac6(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x89da(%rip)        
+	fmul   %st(6),%st
+	fldt   0x8aac(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x89c0(%rip)        
+	fmul   %st(6),%st
+	fldt   0x8a92(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fldt   0x118(%rsp)
+	fldt   0xd8(%rsp)
 	fdivrp %st,%st(1)
-	fldt   0x58(%rsp)
+	fmulp  %st,%st(2)
+	fldt   0xe8(%rsp)
+	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x88(%rsp)
+	fldt   0x108(%rsp)
 	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
-	fldt   -0x48(%rsp)
-	fldt   0xb8(%rsp)
-	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x48(%rsp)
-	fldt   0xe8(%rsp)
+	fldt   -0x48(%rsp)
+	fldt   0x98(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
+	faddp  %st,%st(2)
+	fldt   0x9c3e(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9c46(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9c4c(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9b68(%rip)        
-	fld    %st(4)
-	fmul   %st(1),%st
-	fldt   0x9b6e(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9c52(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b74(%rip)        
+	fldt   0x9c58(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b7a(%rip)        
+	fldt   0x9c5e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b80(%rip)        
+	fldt   0x9c64(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b86(%rip)        
+	fldt   0x9c6a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
-	fldt   0x9b8a(%rip)        
-	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9b90(%rip)        
-	fsubr  %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(7),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9b70(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9c4a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
+	fmul   %st(5),%st
+	fldt   0x9c30(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b42(%rip)        
+	fldt   0x9c16(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b28(%rip)        
+	fldt   0x9bfc(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b0e(%rip)        
+	fldt   0x9be2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9af4(%rip)        
+	fldt   0x9bc8(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fsubp  %st,%st(1)
-	fldt   0x9b58(%rip)        
-	fld    %st(5)
-	fmul   %st(1),%st
+	fldt   0x9bae(%rip)        
+	fsubrp %st,%st(1)
+	fldt   0x9c26(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9c1e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9b5a(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9c24(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9b5a(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9c24(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9b5a(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9c24(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9b5a(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9c24(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9b5a(%rip)        
+	fmul   %st(6),%st
+	fldt   0x9c24(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fld1
-	fadd   %st,%st(1)
-	fxch   %st(1)
 	fmul   %st(6),%st
-	faddp  %st,%st(1)
+	fadd   %st(5),%st
+	fmul   %st(6),%st
+	faddp  %st,%st(5)
+	fxch   %st(4)
 	fmul   %st(5),%st
-	fldt   0x9b4e(%rip)        
+	fldt   0x9c1a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmulp  %st,%st(5)
-	fxch   %st(4)
-	faddp  %st,%st(3)
+	fldz
+	faddp  %st,%st(5)
 	fxch   %st(3)
-	fdivp  %st,%st(2)
-	fldt   0x68(%rsp)
-	fmulp  %st,%st(2)
-	fldt   0x78(%rsp)
+	fdivp  %st,%st(4)
+	fxch   %st(1)
+	fmulp  %st,%st(3)
+	fldt   0x88(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0xa8(%rsp)
-	fldt   -0x68(%rsp)
+	fldt   0xb8(%rsp)
+	fldt   0x38(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0xd8(%rsp)
-	fldt   0x28(%rsp)
+	fldt   0x118(%rsp)
+	fldt   0x48(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x38(%rsp)
-	fldt   0xf8(%rsp)
+	fldt   0x58(%rsp)
+	fldt   0x28(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	faddp  %st,%st(2)
+	faddp  %st,%st(3)
 	test   %esi,%esi
-	jle    6387 <polyreg8+0x1ba7>
+	jle    62a7 <polyreg8+0x1bc7>
 	fldt   0x18(%rsp)
 	movslq %esi,%rsi
 	xor    %eax,%eax
-	fldt   0x108(%rsp)
-	nopw   0x0(%rax,%rax,1)
+	fldt   0x68(%rsp)
+	cs nopw 0x0(%rax,%rax,1)
 	mov    %eax,-0x78(%rsp)
 	fildl  -0x78(%rsp)
 	fmul   %st(2),%st
 	fld1
 	fsubrp %st,%st(1)
-	fld    %st(4)
-	fmul   %st(1),%st
-	fadd   %st(6),%st
+	fld    %st(5)
 	fmul   %st(1),%st
 	fadd   %st(4),%st
 	fmul   %st(1),%st
+	fadd   %st(5),%st
+	fmul   %st(1),%st
 	fadd   %st(2),%st
 	fmul   %st(1),%st
 	fldt   0x8(%rsp)
 	faddp  %st,%st(1)
 	fmul   %st(1),%st
 	fldt   -0x8(%rsp)
 	faddp  %st,%st(1)
@@ -7111,7126 +7095,7136 @@
 	fmulp  %st,%st(1)
 	fldt   -0x38(%rsp)
 	faddp  %st,%st(1)
 	fsubrl (%rdi,%rax,8)
 	fstpl  (%rdx,%rax,8)
 	add    $0x1,%rax
 	cmp    %rax,%rsi
-	jne    6330 <polyreg8+0x1b50>
+	jne    6250 <polyreg8+0x1b70>
 	fstp   %st(0)
 	fstp   %st(0)
 	fldt   -0x38(%rsp)
 	fstpl  -0x78(%rsp)
 	fldt   -0x28(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	fldt   -0x18(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	movups %xmm0,(%r8)
+	movups %xmm0,(%rcx)
 	fstpl  -0x78(%rsp)
 	fldt   -0x8(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	fldt   0x8(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	movups %xmm0,0x10(%r8)
+	movups %xmm0,0x10(%rcx)
 	fstpl  -0x78(%rsp)
-	fldt   0x108(%rsp)
+	fldt   0x68(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
+	fxch   %st(1)
 	movhpd -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	fxch   %st(1)
-	movups %xmm0,0x20(%r8)
+	movups %xmm0,0x20(%rcx)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	fstpl  0x40(%r8)
-	movups %xmm0,0x30(%r8)
-	add    $0x140,%rsp
+	fstpl  0x40(%rcx)
+	movups %xmm0,0x30(%rcx)
+	add    $0x130,%rsp
 	ret
 	nopl   0x0(%rax,%rax,1)
 	fldz
-	fstpt  0x68(%rsp)
-	fldt   0x68(%rsp)
 	fstpt  0x58(%rsp)
 	fldt   0x58(%rsp)
-	fstpt  0x38(%rsp)
-	fldt   0x38(%rsp)
-	fstpt  0x48(%rsp)
-	fldt   0x48(%rsp)
+	fstpt  0x68(%rsp)
+	fldt   0x68(%rsp)
 	fstpt  0x28(%rsp)
 	fldt   0x28(%rsp)
 	fstpt  -0x48(%rsp)
 	fldt   -0x48(%rsp)
-	fstpt  -0x68(%rsp)
-	fldt   -0x68(%rsp)
+	fstpt  0x48(%rsp)
+	fldt   0x48(%rsp)
 	fstpt  -0x58(%rsp)
 	fldt   -0x58(%rsp)
+	fstpt  0x38(%rsp)
+	fldt   0x38(%rsp)
+	fstpt  -0x68(%rsp)
+	fldt   -0x68(%rsp)
 	fstpt  -0x78(%rsp)
-	fldt   -0x78(%rsp)
-	jmp    48d6 <polyreg8+0xf6>
-	nopw   0x0(%rax,%rax,1)
+	jmp    47c6 <polyreg8+0xe6>
+	nopl   0x0(%rax,%rax,1)
 
-0000000000006470 <polyreg9>:
+0000000000006380 <polyreg9>:
 polyreg9():
-	sub    $0x170,%rsp
-	mov    %rcx,%r8
+	sub    $0x160,%rsp
 	mov    %esi,-0x78(%rsp)
 	fildl  -0x78(%rsp)
 	fld    %st(0)
 	fld1
 	fsubrp %st,%st(1)
-	fdivrs 0x6ba2(%rip)        
-	fstpt  0x38(%rsp)
+	fdivrs 0x6c95(%rip)        
+	fstpt  0x28(%rsp)
 	test   %esi,%esi
-	jle    8af8 <polyreg9+0x2688>
+	jle    8a10 <polyreg9+0x2690>
 	fldz
-	movslq %esi,%rcx
+	movslq %esi,%r8
 	xor    %eax,%eax
 	fld    %st(0)
 	fld    %st(1)
-	fld    %st(2)
-	fld    %st(3)
-	fld    %st(4)
-	fstpt  -0x38(%rsp)
-	fldt   -0x38(%rsp)
 	fstpt  -0x48(%rsp)
 	fldt   -0x48(%rsp)
+	fld    %st(0)
+	fld    %st(1)
 	fstpt  -0x58(%rsp)
 	fldt   -0x58(%rsp)
+	fld    %st(0)
+	fstpt  -0x38(%rsp)
+	fldt   -0x38(%rsp)
 	fstpt  -0x68(%rsp)
 	fldt   -0x68(%rsp)
 	fstpt  -0x78(%rsp)
-	fldt   -0x78(%rsp)
-	fxch   %st(6)
-	fstpt  -0x18(%rsp)
 	fxch   %st(5)
-	fstps  -0x8(%rsp)
-	nop
+	fstpt  -0x18(%rsp)
+	nopw   0x0(%rax,%rax,1)
 	mov    %eax,-0x28(%rsp)
 	fildl  -0x28(%rsp)
-	fldt   0x38(%rsp)
+	fldt   0x28(%rsp)
 	fmulp  %st,%st(1)
 	fld1
 	fsubrp %st,%st(1)
 	fldl   (%rdi,%rax,8)
 	fldt   -0x78(%rsp)
 	add    $0x1,%rax
 	fadd   %st(1),%st
 	fstpt  -0x78(%rsp)
 	fmul   %st(1),%st
 	fldt   -0x68(%rsp)
 	fadd   %st(1),%st
 	fstpt  -0x68(%rsp)
 	fmul   %st(1),%st
+	fldt   -0x38(%rsp)
+	fadd   %st(1),%st
+	fstpt  -0x38(%rsp)
+	fmul   %st(1),%st
+	fadd   %st,%st(6)
+	fmul   %st(1),%st
 	fldt   -0x58(%rsp)
 	fadd   %st(1),%st
 	fstpt  -0x58(%rsp)
 	fmul   %st(1),%st
+	fadd   %st,%st(3)
+	fmul   %st(1),%st
+	fadd   %st,%st(2)
+	fmul   %st(1),%st
 	fldt   -0x48(%rsp)
 	fadd   %st(1),%st
 	fstpt  -0x48(%rsp)
 	fmul   %st(1),%st
-	fldt   -0x38(%rsp)
-	fadd   %st(1),%st
-	fstpt  -0x38(%rsp)
-	fmul   %st(1),%st
 	fadd   %st,%st(5)
-	fmul   %st(1),%st
-	fadd   %st,%st(6)
-	fmul   %st(1),%st
-	fadd   %st,%st(2)
-	fmul   %st(1),%st
-	fadd   %st,%st(3)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(3)
-	cmp    %rcx,%rax
-	jne    64e0 <polyreg9+0x70>
+	cmp    %rax,%r8
+	jne    63e8 <polyreg9+0x68>
 	fldt   -0x18(%rsp)
-	fxch   %st(4)
+	fxch   %st(2)
+	fstpt  0x38(%rsp)
 	fstpt  0x48(%rsp)
-	fxch   %st(4)
+	fxch   %st(2)
 	fstpt  0x58(%rsp)
-	fxch   %st(3)
 	fstpt  0x68(%rsp)
-	fxch   %st(2)
-	fstpt  0x78(%rsp)
-	fxch   %st(1)
-	fstpt  0x88(%rsp)
-	flds   -0x8(%rsp)
-	fldt   0x8625(%rip)        
-	fmul   %st(2),%st
-	fldt   0x862d(%rip)        
+	fldt   0x871e(%rip)        
+	fmul   %st(1),%st
+	fldt   0x8726(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0x8633(%rip)        
+	fmul   %st(1),%st
+	fldt   0x872c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0x8639(%rip)        
+	fmul   %st(1),%st
+	fldt   0x8732(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0x863f(%rip)        
+	fmul   %st(1),%st
+	fldt   0x8738(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0x8645(%rip)        
+	fmul   %st(1),%st
+	fldt   0x873e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0x864b(%rip)        
+	fmul   %st(1),%st
+	fldt   0x8744(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fsubs  0x6a71(%rip)        
-	fmul   %st(2),%st
+	fmul   %st(1),%st
+	flds   0x6b7a(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(1),%st
 	fld1
 	fadd   %st,%st(1)
-	fldt   0x8645(%rip)        
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fldt   0x873c(%rip)        
+	fmul   %st(3),%st
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(1)
 	fmul   %st(4),%st
-	fldt   0x8649(%rip)        
+	fldt   0x873c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x864b(%rip)        
+	fldt   0x873e(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x864d(%rip)        
+	fldt   0x8740(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x864f(%rip)        
+	fldt   0x8742(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fdivrp %st,%st(2)
-	fxch   %st(1)
-	fstpt  -0x8(%rsp)
-	fldt   0x864b(%rip)        
-	fmul   %st(3),%st
-	fldt   0x8653(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x8659(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x865f(%rip)        
-	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x8665(%rip)        
-	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x866b(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(3),%st
 	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0x866d(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x8673(%rip)        
-	faddp  %st,%st(1)
-	fldt   0x867b(%rip)        
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fdivrp %st,%st(3)
+	fldt   0x8744(%rip)        
 	fmul   %st(4),%st
-	fldt   0x867f(%rip)        
+	fldt   0x874c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fldt   0x8752(%rip)        
+	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8681(%rip)        
+	fldt   0x8758(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fldt   0x875e(%rip)        
+	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8683(%rip)        
+	fldt   0x8764(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fldt   0x8685(%rip)        
-	faddp  %st,%st(1)
+	fldt   0x8766(%rip)        
+	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fdivrp %st,%st(1)
-	fstpt  0x18(%rsp)
-	fldt   0x8683(%rip)        
-	fmul   %st(3),%st
-	fldt   0x868b(%rip)        
-	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x8691(%rip)        
+	fldt   0x876c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x8697(%rip)        
+	fldt   0x8774(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0x8778(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x869d(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0x877a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x86a3(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0x86a5(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0x877c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x86ab(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0x877e(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x86b3(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fdivrp %st,%st(1)
+	fstpt  0x8(%rsp)
+	fldt   0x877c(%rip)        
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fldt   0x8784(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x878a(%rip)        
+	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x86b7(%rip)        
+	fldt   0x8790(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0x86b9(%rip)        
+	fldt   0x8796(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0x86bb(%rip)        
+	fldt   0x879c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fldt   0x86bd(%rip)        
-	faddp  %st,%st(1)
+	fldt   0x879e(%rip)        
+	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fdivrp %st,%st(1)
-	fstpt  0x98(%rsp)
-	flds   0x68fc(%rip)        
+	fldt   0x87a4(%rip)        
+	faddp  %st,%st(1)
+	fldt   0x87ac(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0x87b0(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0x87b2(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0x87b4(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(2),%st
+	fmul   %st(5),%st
+	fldt   0x87b6(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	faddp  %st,%st(2)
+	fdivp  %st,%st(1)
+	fstpt  0x78(%rsp)
+	flds   0x6a08(%rip)        
 	fld    %st(3)
 	fmul   %st(1),%st
-	flds   0x68f6(%rip)        
+	flds   0x6a02(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
-	flds   0x68ee(%rip)        
-	fadd   %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(6),%st
-	flds   0x68e6(%rip)        
+	fldt   0x97be(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x97c4(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fadds  0x68de(%rip)        
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
+	fadds  0x69e4(%rip)        
+	fmul   %st(6),%st
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x979c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
 	faddp  %st,%st(1)
-	fldt   0x8674(%rip)        
+	fldt   0x876c(%rip)        
 	fmul   %st(4),%st
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(1)
+	fmul   %st(5),%st
+	fldt   0x876c(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(1),%st
+	fmul   %st(5),%st
+	fldt   0x876e(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(1),%st
+	fmul   %st(5),%st
+	fldt   0x8770(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(1),%st
+	fmul   %st(5),%st
 	fadd   %st(3),%st
+	fmul   %st(5),%st
+	fadd   %st(1),%st
+	fdivrp %st,%st(2)
+	fxch   %st(1)
+	fstpt  0x88(%rsp)
+	fldt   0x8761(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x8678(%rip)        
+	fldt   0x8765(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x867a(%rip)        
+	fldt   0x8767(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x867c(%rip)        
+	fldt   0x8769(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
 	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fdivrp %st,%st(1)
-	fstpt  0xa8(%rsp)
-	fldt   0x866f(%rip)        
-	fmul   %st(3),%st
+	fldt   0x8769(%rip)        
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fldt   0x8673(%rip)        
+	fmul   %st(5),%st
+	fldt   0x876d(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fldt   0x8675(%rip)        
+	fmul   %st(5),%st
+	fldt   0x876f(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fldt   0x8677(%rip)        
+	fmul   %st(5),%st
+	fldt   0x8771(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
+	fmul   %st(5),%st
 	fadd   %st(2),%st
-	fmul   %st(3),%st
-	fadd   %st(1),%st
-	fldt   0x8677(%rip)        
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0x867b(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0x867d(%rip)        
-	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0x867f(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0x8681(%rip)        
+	fmul   %st(5),%st
+	fldt   0x8773(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fdivrp %st,%st(1)
+	fmul   %st(5),%st
+	faddp  %st,%st(2)
+	fdivp  %st,%st(1)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
+	fldt   -0x38(%rsp)
+	fld    %st(0)
+	fmul   %st(4),%st
+	faddp  %st,%st(2)
 	fldt   -0x58(%rsp)
-	fldt   -0x8(%rsp)
+	fldt   0x8(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   -0x38(%rsp)
-	fldt   0x18(%rsp)
+	faddp  %st,%st(2)
+	fldt   0x78(%rsp)
+	fldt   0x48(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
+	faddp  %st,%st(2)
 	fldt   0x58(%rsp)
-	fldt   0x98(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x78(%rsp)
-	fldt   0xa8(%rsp)
+	fldt   0x88(%rsp)
 	fmulp  %st,%st(1)
+	faddp  %st,%st(2)
+	fxch   %st(1)
+	fstpt  -0x38(%rsp)
+	fldt   0x96a8(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96b0(%rip)        
 	faddp  %st,%st(1)
-	fstpt  -0x28(%rsp)
-	fldt   0x9593(%rip)        
-	fmul   %st(3),%st
-	fldt   0x959b(%rip)        
-	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95a1(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96b6(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95a7(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96bc(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95ad(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96c2(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95b3(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96c8(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95b9(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96ce(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95bf(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96d4(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95c5(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96da(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95cb(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96e0(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95d1(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96e6(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95d7(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96ec(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95dd(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96f2(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95e3(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96f8(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95e9(%rip)        
+	fmul   %st(4),%st
+	fldt   0x96fe(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95ef(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9704(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95f5(%rip)        
+	fmul   %st(4),%st
+	fldt   0x970a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0x95f7(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(2),%st
+	fmul   %st(4),%st
+	fldt   0x970c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x95fd(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9712(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9605(%rip)        
-	fld    %st(4)
+	fldt   0x971a(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9607(%rip)        
+	fmul   %st(5),%st
+	fldt   0x971c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9607(%rip)        
+	fmul   %st(5),%st
+	fldt   0x971c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9607(%rip)        
+	fmul   %st(5),%st
+	fldt   0x971c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9607(%rip)        
+	fmul   %st(5),%st
+	fldt   0x971c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9607(%rip)        
+	fmul   %st(5),%st
+	fldt   0x971c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9607(%rip)        
+	fmul   %st(5),%st
+	fldt   0x971c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9607(%rip)        
+	fmul   %st(5),%st
+	fldt   0x971c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9607(%rip)        
+	fmul   %st(5),%st
+	fldt   0x971c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9607(%rip)        
+	fmul   %st(5),%st
+	fldt   0x971c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fmul   %st(5),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0x8(%rsp)
-	fldt   0x95ff(%rip)        
-	fmul   %st(3),%st
-	fldt   0x9607(%rip)        
+	fstpt  -0x8(%rsp)
+	fldt   0x9712(%rip)        
+	fmul   %st(4),%st
+	fldt   0x971a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x960d(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9720(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9613(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9726(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9619(%rip)        
+	fmul   %st(4),%st
+	fldt   0x972c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x961f(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9732(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9625(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9738(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x962b(%rip)        
+	fmul   %st(4),%st
+	fldt   0x973e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9631(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9744(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9637(%rip)        
+	fmul   %st(4),%st
+	fldt   0x974a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x963d(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9750(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9643(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9756(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9649(%rip)        
+	fmul   %st(4),%st
+	fldt   0x975c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x964f(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9762(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9655(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9768(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x965b(%rip)        
+	fmul   %st(4),%st
+	fldt   0x976e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9661(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9774(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0x9663(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(2),%st
+	fmul   %st(4),%st
+	fldt   0x9776(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9669(%rip)        
+	fmul   %st(4),%st
+	fldt   0x977c(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9671(%rip)        
-	fld    %st(4)
+	fldt   0x9784(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9673(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9786(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9673(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9786(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9673(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9786(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9673(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9786(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9673(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9786(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9673(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9786(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9673(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9786(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9673(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9786(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9673(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9786(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fmul   %st(5),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0x28(%rsp)
-	fldt   0x966b(%rip)        
-	fmul   %st(3),%st
-	fldt   0x9673(%rip)        
+	fstpt  0x18(%rsp)
+	fldt   0x977c(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9784(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9679(%rip)        
+	fmul   %st(4),%st
+	fldt   0x978a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x967f(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9790(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9685(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9796(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x968b(%rip)        
+	fmul   %st(4),%st
+	fldt   0x979c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9691(%rip)        
+	fmul   %st(4),%st
+	fldt   0x97a2(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9697(%rip)        
+	fmul   %st(4),%st
+	fldt   0x97a8(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x969d(%rip)        
+	fmul   %st(4),%st
+	fldt   0x97ae(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96a3(%rip)        
+	fmul   %st(4),%st
+	fldt   0x97b4(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96a9(%rip)        
+	fmul   %st(4),%st
+	fldt   0x97ba(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96af(%rip)        
+	fmul   %st(4),%st
+	fldt   0x97c0(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96b5(%rip)        
+	fmul   %st(4),%st
+	fldt   0x97c6(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96bb(%rip)        
+	fmul   %st(4),%st
+	fldt   0x97cc(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96c1(%rip)        
+	fmul   %st(4),%st
+	fldt   0x97d2(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96c7(%rip)        
+	fmul   %st(4),%st
+	fldt   0x97d8(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96cd(%rip)        
+	fmul   %st(4),%st
+	fldt   0x97de(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0x96cf(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(2),%st
+	fmul   %st(4),%st
+	fldt   0x97e0(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96d5(%rip)        
+	fmul   %st(4),%st
+	fldt   0x97e6(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x96dd(%rip)        
-	fld    %st(4)
+	fldt   0x97ee(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96df(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97f0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96df(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97f0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96df(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97f0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96df(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97f0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96df(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97f0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96df(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97f0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96df(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97f0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96df(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97f0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96df(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97f0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fdivrp %st,%st(1)
-	fstpt  0xb8(%rsp)
-	fldt   0x96d4(%rip)        
-	fld    %st(3)
+	fmul   %st(5),%st
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(2)
+	fdivp  %st,%st(1)
+	fstpt  0x98(%rsp)
+	fldt   0x97e1(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96d6(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97e3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96d6(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97e3(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96d6(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97e3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96d6(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97e3(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96d6(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97e3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96d6(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97e3(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96d6(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97e3(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0x96ce(%rip)        
+	fmul   %st(5),%st
+	fadd   %st(3),%st
+	fmul   %st(5),%st
+	fadd   %st(3),%st
+	fmul   %st(5),%st
+	fldt   0x97db(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(2),%st
-	fldt   0x96cc(%rip)        
-	fmul   %st(4),%st
-	fldt   0x96d4(%rip)        
+	fmul   %st(5),%st
+	faddp  %st,%st(1)
+	fldt   0x97d9(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97e1(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96da(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97e7(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96e0(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97ed(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96e6(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97f3(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96ec(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97f9(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96f2(%rip)        
+	fmul   %st(5),%st
+	fldt   0x97ff(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96f8(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9805(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x96fe(%rip)        
+	fmul   %st(5),%st
+	fldt   0x980b(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9704(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9811(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x970a(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9817(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9710(%rip)        
+	fmul   %st(5),%st
+	fldt   0x981d(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9716(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9823(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x971c(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9829(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9722(%rip)        
+	fmul   %st(5),%st
+	fldt   0x982f(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9728(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9835(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x972e(%rip)        
+	fmul   %st(5),%st
+	fldt   0x983b(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9734(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9841(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x973a(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9847(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9740(%rip)        
+	fmul   %st(5),%st
+	fldt   0x984d(%rip)        
 	faddp  %st,%st(1)
 	fxch   %st(1)
 	fld    %st(0)
-	fstpt  0x158(%rsp)
+	fstpt  0x128(%rsp)
 	fdivrp %st,%st(1)
-	fstpt  0xc8(%rsp)
-	fldt   0x9734(%rip)        
-	fld    %st(3)
+	fstpt  0xa8(%rsp)
+	fldt   0x9841(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9736(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9843(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9736(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9843(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9736(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9843(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9736(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9843(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9736(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9843(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9736(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9843(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9736(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9843(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fsub   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0x972e(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(2),%st
+	fmul   %st(4),%st
+	fsub   %st(2),%st
+	fmul   %st(4),%st
+	fldt   0x983b(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
-	fldt   0x9730(%rip)        
-	fld    %st(4)
+	fldt   0x983d(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9732(%rip)        
+	fmul   %st(5),%st
+	fldt   0x983f(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9732(%rip)        
+	fmul   %st(5),%st
+	fldt   0x983f(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9732(%rip)        
+	fmul   %st(5),%st
+	fldt   0x983f(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9732(%rip)        
+	fmul   %st(5),%st
+	fldt   0x983f(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9732(%rip)        
+	fmul   %st(5),%st
+	fldt   0x983f(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9732(%rip)        
+	fmul   %st(5),%st
+	fldt   0x983f(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9732(%rip)        
+	fmul   %st(5),%st
+	fldt   0x983f(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9732(%rip)        
+	fmul   %st(5),%st
+	fldt   0x983f(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9732(%rip)        
+	fmul   %st(5),%st
+	fldt   0x983f(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fmul   %st(5),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
-	fldt   -0x48(%rsp)
-	fldt   0x8(%rsp)
-	fmulp  %st,%st(1)
+	fldt   -0x8(%rsp)
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fldt   0x48(%rsp)
-	fldt   0x28(%rsp)
+	fldt   0x18(%rsp)
+	fldt   0x38(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x68(%rsp)
-	fldt   0xb8(%rsp)
+	fldt   -0x48(%rsp)
+	fldt   0x98(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x88(%rsp)
-	fldt   0xc8(%rsp)
+	fldt   0x68(%rsp)
+	fldt   0xa8(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fstpt  -0x18(%rsp)
-	fldt   0x96eb(%rip)        
-	fmul   %st(3),%st
-	fldt   0x96f3(%rip)        
+	fstpt  -0x28(%rsp)
+	fldt   0x97fd(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9805(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96f9(%rip)        
+	fmul   %st(4),%st
+	fldt   0x980b(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x96ff(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9811(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9705(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9817(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x970b(%rip)        
+	fmul   %st(4),%st
+	fldt   0x981d(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9711(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9823(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9717(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9829(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x971d(%rip)        
+	fmul   %st(4),%st
+	fldt   0x982f(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9723(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9835(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9729(%rip)        
+	fmul   %st(4),%st
+	fldt   0x983b(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x972f(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9841(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0x9731(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(2),%st
+	fmul   %st(4),%st
+	fldt   0x9843(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9737(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9849(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x973d(%rip)        
+	fmul   %st(4),%st
+	fldt   0x984f(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9745(%rip)        
-	fld    %st(4)
+	fldt   0x9857(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9747(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9859(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9747(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9859(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9747(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9859(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9747(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9859(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9747(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9859(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9747(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9859(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9747(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9859(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fmul   %st(5),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   0x9743(%rip)        
+	fstpt  0xb8(%rsp)
+	fldt   0x984c(%rip)        
 	fmul   %st(4),%st
-	fldt   0x974b(%rip)        
+	fldt   0x9854(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9751(%rip)        
+	fldt   0x985a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9757(%rip)        
+	fldt   0x9860(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x975d(%rip)        
+	fldt   0x9866(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9763(%rip)        
+	fldt   0x986c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9769(%rip)        
+	fldt   0x9872(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x976f(%rip)        
+	fldt   0x9878(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9775(%rip)        
+	fldt   0x987e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x977b(%rip)        
+	fldt   0x9884(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9781(%rip)        
+	fldt   0x988a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9787(%rip)        
+	fldt   0x9890(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
 	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fldt   0x9789(%rip)        
+	fldt   0x9892(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x978f(%rip)        
+	fldt   0x9898(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9795(%rip)        
+	fldt   0x989e(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x979d(%rip)        
+	fldt   0x98a6(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x979f(%rip)        
+	fldt   0x98a8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x979f(%rip)        
+	fldt   0x98a8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x979f(%rip)        
+	fldt   0x98a8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x979f(%rip)        
+	fldt   0x98a8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x979f(%rip)        
+	fldt   0x98a8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x979f(%rip)        
+	fldt   0x98a8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x979f(%rip)        
+	fldt   0x98a8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0xd8(%rsp)
-	fldt   0x9794(%rip)        
+	fstpt  0xc8(%rsp)
+	fldt   0x989b(%rip)        
 	fmul   %st(4),%st
-	fldt   0x979c(%rip)        
+	fldt   0x98a3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97a2(%rip)        
+	fldt   0x98a9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97a8(%rip)        
+	fldt   0x98af(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97ae(%rip)        
+	fldt   0x98b5(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97b4(%rip)        
+	fldt   0x98bb(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97ba(%rip)        
+	fldt   0x98c1(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97c0(%rip)        
+	fldt   0x98c7(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97c6(%rip)        
+	fldt   0x98cd(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97cc(%rip)        
+	fldt   0x98d3(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
 	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fldt   0x97ce(%rip)        
+	fldt   0x98d5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97d4(%rip)        
+	fldt   0x98db(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97da(%rip)        
+	fldt   0x98e1(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97e0(%rip)        
+	fldt   0x98e7(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97e6(%rip)        
+	fldt   0x98ed(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x97ee(%rip)        
+	fldt   0x98f5(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97f0(%rip)        
+	fldt   0x98f7(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97f0(%rip)        
+	fldt   0x98f7(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97f0(%rip)        
+	fldt   0x98f7(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97f0(%rip)        
+	fldt   0x98f7(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97f0(%rip)        
+	fldt   0x98f7(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97f0(%rip)        
+	fldt   0x98f7(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97f0(%rip)        
+	fldt   0x98f7(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0xe8(%rsp)
-	fldt   0x80b5(%rip)        
+	fstpt  0xd8(%rsp)
+	fldt   0x819a(%rip)        
 	fmul   %st(4),%st
-	fldt   0x80bd(%rip)        
+	fldt   0x81a2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x80c3(%rip)        
+	fldt   0x81a8(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x80c9(%rip)        
+	fldt   0x81ae(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x80cf(%rip)        
+	fldt   0x81b4(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x80d5(%rip)        
+	fldt   0x81ba(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x80db(%rip)        
+	fldt   0x81c0(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x80e1(%rip)        
+	fldt   0x81c6(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x80e7(%rip)        
+	fldt   0x81cc(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x80ed(%rip)        
+	fldt   0x81d2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x80f3(%rip)        
+	fldt   0x81d8(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x80f9(%rip)        
+	fldt   0x81de(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x80ff(%rip)        
+	fldt   0x81e4(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8105(%rip)        
+	fldt   0x81ea(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
 	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fldt   0x5cd7(%rip)        
+	fldt   0x5dbc(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x80ff(%rip)        
+	fldt   0x81e4(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8101(%rip)        
+	fldt   0x81e6(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8101(%rip)        
+	fldt   0x81e6(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8101(%rip)        
+	fldt   0x81e6(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8101(%rip)        
+	fldt   0x81e6(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8101(%rip)        
+	fldt   0x81e6(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8101(%rip)        
+	fldt   0x81e6(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x8101(%rip)        
+	fldt   0x81e6(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
+	fmul   %st(1),%st
+	fldt   -0x78(%rsp)
+	fmulp  %st,%st(4)
+	faddp  %st,%st(3)
 	fldt   -0x58(%rsp)
+	fldt   0xb8(%rsp)
 	fmulp  %st,%st(1)
-	fldt   -0x8(%rsp)
-	fldt   -0x78(%rsp)
+	faddp  %st,%st(3)
+	fldt   0xc8(%rsp)
+	fldt   0x48(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   -0x38(%rsp)
-	fxch   %st(2)
-	fld    %st(0)
-	fstpt  0x138(%rsp)
-	fmulp  %st,%st(2)
-	faddp  %st,%st(1)
+	faddp  %st,%st(3)
 	fldt   0x58(%rsp)
 	fldt   0xd8(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x78(%rsp)
-	fldt   0xe8(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fstpt  -0x8(%rsp)
-	fldt   0x9686(%rip)        
+	faddp  %st,%st(3)
+	fxch   %st(2)
+	fstpt  -0x18(%rsp)
+	fldt   0x9793(%rip)        
 	fmul   %st(3),%st
-	fldt   0x968e(%rip)        
+	fldt   0x979b(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9694(%rip)        
+	fldt   0x97a1(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x969a(%rip)        
+	fldt   0x97a7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96a0(%rip)        
+	fldt   0x97ad(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96a6(%rip)        
+	fldt   0x97b3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96ac(%rip)        
+	fldt   0x97b9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96b2(%rip)        
+	fldt   0x97bf(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96b8(%rip)        
+	fldt   0x97c5(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96be(%rip)        
+	fldt   0x97cb(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96c4(%rip)        
+	fldt   0x97d1(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96ca(%rip)        
+	fldt   0x97d7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96d0(%rip)        
+	fldt   0x97dd(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96d6(%rip)        
+	fldt   0x97e3(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96dc(%rip)        
+	fldt   0x97e9(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
 	fadd   %st(1),%st
 	fmul   %st(3),%st
-	fldt   0x96de(%rip)        
+	fldt   0x97eb(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96e4(%rip)        
+	fldt   0x97f1(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96ea(%rip)        
+	fldt   0x97f7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x96f0(%rip)        
+	fldt   0x97fd(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x96f8(%rip)        
+	fldt   0x9805(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96fa(%rip)        
+	fldt   0x9807(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96fa(%rip)        
+	fldt   0x9807(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96fa(%rip)        
+	fldt   0x9807(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96fa(%rip)        
+	fldt   0x9807(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96fa(%rip)        
+	fldt   0x9807(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96fa(%rip)        
+	fldt   0x9807(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96fa(%rip)        
+	fldt   0x9807(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96fa(%rip)        
+	fldt   0x9807(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96fa(%rip)        
+	fldt   0x9807(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fdivrp %st,%st(1)
-	fldt   0x96f6(%rip)        
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(2)
+	fdivp  %st,%st(1)
+	fstpt  0xe8(%rsp)
+	fldt   0x97f8(%rip)        
 	fmul   %st(4),%st
-	fldt   0x96fe(%rip)        
+	fldt   0x9800(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9704(%rip)        
+	fldt   0x9806(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x970a(%rip)        
+	fldt   0x980c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9710(%rip)        
+	fldt   0x9812(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9716(%rip)        
+	fldt   0x9818(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x971c(%rip)        
+	fldt   0x981e(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9722(%rip)        
+	fldt   0x9824(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9728(%rip)        
+	fldt   0x982a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x972e(%rip)        
+	fldt   0x9830(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9734(%rip)        
+	fldt   0x9836(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x973a(%rip)        
+	fldt   0x983c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9740(%rip)        
+	fldt   0x9842(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9746(%rip)        
+	fldt   0x9848(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x974c(%rip)        
+	fldt   0x984e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
 	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fldt   0x974e(%rip)        
+	fldt   0x9850(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9754(%rip)        
+	fldt   0x9856(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x975a(%rip)        
+	fldt   0x985c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9760(%rip)        
+	fldt   0x9862(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9768(%rip)        
+	fldt   0x986a(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x976a(%rip)        
+	fldt   0x986c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x976a(%rip)        
+	fldt   0x986c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x976a(%rip)        
+	fldt   0x986c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x976a(%rip)        
+	fldt   0x986c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x976a(%rip)        
+	fldt   0x986c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x976a(%rip)        
+	fldt   0x986c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x976a(%rip)        
+	fldt   0x986c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x976a(%rip)        
+	fldt   0x986c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x976a(%rip)        
+	fldt   0x986c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
-	fdivrp %st,%st(1)
-	fstpt  0xf8(%rsp)
-	fldt   0x975f(%rip)        
+	faddp  %st,%st(2)
+	fdivp  %st,%st(1)
+	fldt   0x9868(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9767(%rip)        
+	fldt   0x9870(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x976d(%rip)        
+	fldt   0x9876(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9773(%rip)        
+	fldt   0x987c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9779(%rip)        
+	fldt   0x9882(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x977f(%rip)        
+	fldt   0x9888(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9785(%rip)        
+	fldt   0x988e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x978b(%rip)        
+	fldt   0x9894(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9791(%rip)        
+	fldt   0x989a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9797(%rip)        
+	fldt   0x98a0(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x979d(%rip)        
+	fldt   0x98a6(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97a3(%rip)        
+	fldt   0x98ac(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97a9(%rip)        
+	fldt   0x98b2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
 	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fldt   0x97ab(%rip)        
+	fldt   0x98b4(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97b1(%rip)        
+	fldt   0x98ba(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97b7(%rip)        
+	fldt   0x98c0(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97bd(%rip)        
+	fldt   0x98c6(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97c3(%rip)        
+	fldt   0x98cc(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97c9(%rip)        
+	fldt   0x98d2(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x97d1(%rip)        
+	fldt   0x98da(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d3(%rip)        
+	fldt   0x98dc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d3(%rip)        
+	fldt   0x98dc(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d3(%rip)        
+	fldt   0x98dc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d3(%rip)        
+	fldt   0x98dc(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d3(%rip)        
+	fldt   0x98dc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d3(%rip)        
+	fldt   0x98dc(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d3(%rip)        
+	fldt   0x98dc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d3(%rip)        
+	fldt   0x98dc(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d3(%rip)        
+	fldt   0x98dc(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fstpt  0x108(%rsp)
-	fldt   0x97c8(%rip)        
+	fstpt  0xf8(%rsp)
+	fldt   0x98cf(%rip)        
 	fmul   %st(4),%st
-	fldt   0x97d0(%rip)        
+	fldt   0x98d7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97d6(%rip)        
+	fldt   0x98dd(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97dc(%rip)        
+	fldt   0x98e3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97e2(%rip)        
+	fldt   0x98e9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97e8(%rip)        
+	fldt   0x98ef(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97ee(%rip)        
+	fldt   0x98f5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97f4(%rip)        
+	fldt   0x98fb(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97fa(%rip)        
+	fldt   0x9901(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9800(%rip)        
+	fldt   0x9907(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9806(%rip)        
+	fldt   0x990d(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x980c(%rip)        
+	fldt   0x9913(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9812(%rip)        
+	fldt   0x9919(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9818(%rip)        
+	fldt   0x991f(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x981e(%rip)        
+	fldt   0x9925(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9824(%rip)        
+	fldt   0x992b(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x982a(%rip)        
+	fldt   0x9931(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
 	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fldt   0x982c(%rip)        
+	fldt   0x9933(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9832(%rip)        
+	fldt   0x9939(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x983a(%rip)        
+	fldt   0x9941(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x983c(%rip)        
+	fldt   0x9943(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x983c(%rip)        
+	fldt   0x9943(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x983c(%rip)        
+	fldt   0x9943(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x983c(%rip)        
+	fldt   0x9943(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x983c(%rip)        
+	fldt   0x9943(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x983c(%rip)        
+	fldt   0x9943(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x983c(%rip)        
+	fldt   0x9943(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x983c(%rip)        
+	fldt   0x9943(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x983c(%rip)        
+	fldt   0x9943(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   -0x48(%rsp)
-	fmulp  %st,%st(1)
-	fldt   0x8(%rsp)
+	fmul   %st(5),%st
+	fldt   -0x8(%rsp)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x48(%rsp)
-	fmul   %st(2),%st
+	fldt   0xe8(%rsp)
+	fldt   0x38(%rsp)
+	fmulp  %st,%st(1)
+	faddp  %st,%st(1)
+	fldt   -0x48(%rsp)
+	fxch   %st(2)
+	fld    %st(0)
+	fstpt  0x138(%rsp)
+	fmulp  %st,%st(2)
 	faddp  %st,%st(1)
 	fldt   0x68(%rsp)
 	fldt   0xf8(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x88(%rsp)
-	fldt   0x108(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fstpt  0x8(%rsp)
-	fldt   0x97f9(%rip)        
-	fmul   %st(4),%st
-	fldt   0x9801(%rip)        
+	fstpt  -0x8(%rsp)
+	fldt   0x98fa(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9902(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9807(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9908(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x980d(%rip)        
+	fmul   %st(3),%st
+	fldt   0x990e(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9813(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9914(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9819(%rip)        
+	fmul   %st(3),%st
+	fldt   0x991a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x981f(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9920(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9825(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9926(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x982b(%rip)        
+	fmul   %st(3),%st
+	fldt   0x992c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9831(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9932(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0x9833(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(1),%st
+	fmul   %st(3),%st
+	fldt   0x9934(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9839(%rip)        
+	fmul   %st(3),%st
+	fldt   0x993a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x983f(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9940(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9845(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9946(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x984b(%rip)        
+	fmul   %st(3),%st
+	fldt   0x994c(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9853(%rip)        
-	fld    %st(5)
+	fldt   0x9954(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9855(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9956(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9855(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9956(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9855(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9956(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9855(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9956(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9855(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9956(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9855(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9956(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9855(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9956(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
-	fdivrp %st,%st(1)
-	fstpt  0x118(%rsp)
-	fldt   0x984a(%rip)        
+	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9852(%rip)        
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  0x108(%rsp)
+	fldt   0x9949(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9951(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9858(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9957(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x985e(%rip)        
+	fmul   %st(3),%st
+	fldt   0x995d(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9864(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9963(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x986a(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9969(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9870(%rip)        
+	fmul   %st(3),%st
+	fldt   0x996f(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9876(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9975(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x987c(%rip)        
+	fmul   %st(3),%st
+	fldt   0x997b(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9882(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9981(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0x9884(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(1),%st
+	fmul   %st(3),%st
+	fldt   0x9983(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x988a(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9989(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9890(%rip)        
+	fmul   %st(3),%st
+	fldt   0x998f(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9896(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9995(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x989c(%rip)        
+	fmul   %st(3),%st
+	fldt   0x999b(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x98a4(%rip)        
-	fld    %st(5)
+	fldt   0x99a3(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x98a6(%rip)        
+	fmul   %st(4),%st
+	fldt   0x99a5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98a6(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x99a5(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98a6(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x99a5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98a6(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x99a5(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98a6(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x99a5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98a6(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x99a5(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98a6(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x99a5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
-	fdivrp %st,%st(1)
-	fstpt  0x128(%rsp)
-	fldt   0x989b(%rip)        
+	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98a3(%rip)        
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(2)
+	fdivp  %st,%st(1)
+	fstpt  0x118(%rsp)
+	fldt   0x9996(%rip)        
+	fmul   %st(4),%st
+	fldt   0x999e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98a9(%rip)        
+	fldt   0x99a4(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98af(%rip)        
+	fldt   0x99aa(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98b5(%rip)        
+	fldt   0x99b0(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98bb(%rip)        
+	fldt   0x99b6(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98c1(%rip)        
+	fldt   0x99bc(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98c7(%rip)        
+	fldt   0x99c2(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98cd(%rip)        
+	fldt   0x99c8(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98d3(%rip)        
+	fldt   0x99ce(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98d9(%rip)        
+	fldt   0x99d4(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98df(%rip)        
+	fldt   0x99da(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
 	fadd   %st(2),%st
 	fmul   %st(4),%st
-	fldt   0x98e1(%rip)        
+	fldt   0x99dc(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98e7(%rip)        
+	fldt   0x99e2(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98ed(%rip)        
+	fldt   0x99e8(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x98f5(%rip)        
+	fldt   0x99f0(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98f7(%rip)        
+	fldt   0x99f2(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98f7(%rip)        
+	fldt   0x99f2(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98f7(%rip)        
+	fldt   0x99f2(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98f7(%rip)        
+	fldt   0x99f2(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98f7(%rip)        
+	fldt   0x99f2(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98f7(%rip)        
+	fldt   0x99f2(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x98f7(%rip)        
+	fldt   0x99f2(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
-	fdivrp %st,%st(1)
-	fldt   -0x38(%rsp)
+	faddp  %st,%st(2)
+	fdivp  %st,%st(1)
+	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x18(%rsp)
+	fldt   0x8(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x138(%rsp)
-	fldt   -0x58(%rsp)
-	fmulp  %st,%st(1)
+	fldt   0xb8(%rsp)
+	fmul   %st(4),%st
 	faddp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x58(%rsp)
-	fldt   0x118(%rsp)
+	fldt   0x108(%rsp)
+	fldt   0x48(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x78(%rsp)
-	fldt   0x128(%rsp)
+	fldt   0x58(%rsp)
+	fldt   0x118(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fstpt  0x18(%rsp)
-	fldt   0x98b0(%rip)        
-	fmul   %st(4),%st
-	fldt   0x98b8(%rip)        
+	fstpt  0x8(%rsp)
+	fldt   0x99af(%rip)        
+	fmul   %st(3),%st
+	fldt   0x99b7(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x98be(%rip)        
+	fmul   %st(3),%st
+	fldt   0x99bd(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x98c4(%rip)        
+	fmul   %st(3),%st
+	fldt   0x99c3(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x98ca(%rip)        
+	fmul   %st(3),%st
+	fldt   0x99c9(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x98d0(%rip)        
+	fmul   %st(3),%st
+	fldt   0x99cf(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x98d6(%rip)        
+	fmul   %st(3),%st
+	fldt   0x99d5(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x98dc(%rip)        
+	fmul   %st(3),%st
+	fldt   0x99db(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x98e2(%rip)        
+	fmul   %st(3),%st
+	fldt   0x99e1(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x98e8(%rip)        
+	fmul   %st(3),%st
+	fldt   0x99e7(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x98ee(%rip)        
+	fmul   %st(3),%st
+	fldt   0x99ed(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x98f4(%rip)        
+	fmul   %st(3),%st
+	fldt   0x99f3(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x98fa(%rip)        
+	fmul   %st(3),%st
+	fldt   0x99f9(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0x98fc(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(1),%st
+	fmul   %st(3),%st
+	fldt   0x99fb(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9902(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9a01(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9908(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9a07(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x990e(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9a0d(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9914(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9a13(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x991a(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9a19(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9922(%rip)        
-	fld    %st(5)
+	fldt   0x9a21(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9924(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a23(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9924(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9a23(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9924(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9a23(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9924(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9a23(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9924(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9a23(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9924(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9a23(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9924(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9a23(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9924(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9a23(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9924(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9a23(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   0x9920(%rip)        
-	fmul   %st(5),%st
-	fldt   0x9928(%rip)        
+	fldt   0x9a1d(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a25(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x992e(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a2b(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9934(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a31(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x993a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a37(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9940(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a3d(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9946(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a43(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x994c(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a49(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9952(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a4f(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9958(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a55(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x995e(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a5b(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9964(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a61(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x996a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a67(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fadd   %st(3),%st
-	fmul   %st(5),%st
-	fldt   0x996c(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(2),%st
+	fmul   %st(4),%st
+	fldt   0x9a69(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9972(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a6f(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9978(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a75(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x997e(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a7b(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9984(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a81(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x998a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a87(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9992(%rip)        
-	fld    %st(6)
+	fldt   0x9a8f(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9994(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a91(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9994(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a91(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9994(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a91(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9994(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a91(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9994(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a91(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9994(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a91(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9994(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a91(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9994(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a91(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9994(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a91(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fadd   %st(5),%st
-	fdivrp %st,%st(1)
-	fstpt  0x138(%rsp)
-	fldt   0x9989(%rip)        
+	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9991(%rip)        
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  0xb8(%rsp)
+	fldt   0x9a84(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a8c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9997(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a92(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x999d(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a98(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99a3(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a9e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99a9(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9aa4(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99af(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9aaa(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99b5(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ab0(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99bb(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ab6(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99c1(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9abc(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99c7(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ac2(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99cd(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ac8(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99d3(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ace(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99d9(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ad4(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99df(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ada(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fadd   %st(3),%st
-	fmul   %st(5),%st
-	fldt   0x99e1(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(2),%st
+	fmul   %st(4),%st
+	fldt   0x9adc(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99e7(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ae2(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99ed(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ae8(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x99f3(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9aee(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x99fb(%rip)        
-	fld    %st(6)
+	fldt   0x9af6(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x99fd(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9af8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x99fd(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9af8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x99fd(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9af8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x99fd(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9af8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x99fd(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9af8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x99fd(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9af8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x99fd(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9af8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x99fd(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9af8(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x99fd(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9af8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fadd   %st(5),%st
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   0x48(%rsp)
+	fldt   0x38(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x28(%rsp)
+	fldt   0x18(%rsp)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
+	fldt   0xe8(%rsp)
+	fmul   %st(7),%st
+	faddp  %st,%st(1)
+	faddp  %st,%st(1)
 	fldt   -0x48(%rsp)
-	fmulp  %st,%st(4)
-	faddp  %st,%st(3)
-	faddp  %st,%st(2)
+	fxch   %st(2)
+	fld    %st(0)
+	fstpt  0x148(%rsp)
+	fmulp  %st,%st(2)
+	faddp  %st,%st(1)
 	fldt   0x68(%rsp)
-	fmul   %st(1),%st
-	faddp  %st,%st(2)
-	fldt   0x88(%rsp)
-	fldt   0x138(%rsp)
+	fldt   0xb8(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
-	fxch   %st(1)
-	fstpt  0x28(%rsp)
-	fldt   0x99bf(%rip)        
-	fmul   %st(4),%st
-	fldt   0x99c7(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99cd(%rip)        
+	fstpt  0x18(%rsp)
+	fldt   0x9aaf(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9ab7(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(3),%st
+	fldt   0x9abd(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99d3(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9ac3(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99d9(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9ac9(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99df(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9acf(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99e5(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9ad5(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99eb(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9adb(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0x99ed(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(1),%st
+	fmul   %st(3),%st
+	fldt   0x9add(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99f3(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9ae3(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99f9(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9ae9(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99ff(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9aef(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a05(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9af5(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a0b(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9afb(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a11(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b01(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9a19(%rip)        
-	fld    %st(5)
+	fldt   0x9b09(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9a1b(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9b0b(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a1b(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b0b(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a1b(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b0b(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a1b(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b0b(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a1b(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b0b(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a1b(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b0b(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a1b(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b0b(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
-	fdivrp %st,%st(1)
-	fstpt  0x148(%rsp)
-	fldt   0x9a10(%rip)        
+	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a18(%rip)        
+	fldz
+	faddp  %st,%st(1)
+	fdivrp %st,%st(1)
+	fstpt  0xe8(%rsp)
+	fldt   0x9afe(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b06(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a1e(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b0c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a24(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b12(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a2a(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b18(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a30(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b1e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a36(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b24(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a3c(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b2a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a42(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b30(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a48(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b36(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0x9a4a(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(1),%st
+	fmul   %st(3),%st
+	fldt   0x9b38(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a50(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b3e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a56(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b44(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a5c(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b4a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a62(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b50(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9a6a(%rip)        
-	fld    %st(5)
+	fldt   0x9b58(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9a6c(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9b5a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a6c(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b5a(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a6c(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b5a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a6c(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b5a(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a6c(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b5a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a6c(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b5a(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a6c(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9b5a(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   0x58(%rsp)
+	fldt   0x48(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x98(%rsp)
+	fldt   0x78(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0xd8(%rsp)
-	fldt   -0x58(%rsp)
-	fmulp  %st,%st(1)
+	fldt   0xc8(%rsp)
+	fmul   %st(4),%st
 	faddp  %st,%st(1)
-	fldt   0x118(%rsp)
-	fldt   -0x38(%rsp)
+	fldt   0x108(%rsp)
+	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x78(%rsp)
-	fldt   0x148(%rsp)
+	fldt   0x58(%rsp)
+	fldt   0xe8(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fstpt  0xd8(%rsp)
-	fldt   0x9a1f(%rip)        
-	fmul   %st(4),%st
-	fldt   0x9a27(%rip)        
+	fstpt  0xc8(%rsp)
+	fldt   0x9b12(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b1a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a2d(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b20(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a33(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b26(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a39(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b2c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a3f(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b32(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a45(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b38(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a4b(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b3e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a51(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b44(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a57(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b4a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a5d(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b50(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a63(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b56(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a69(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b5c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a6f(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b62(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a75(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b68(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a7b(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b6e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a81(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b74(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a87(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b7a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a8d(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b80(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a93(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b86(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x158(%rsp)
+	fldt   0x128(%rsp)
 	fdivrp %st,%st(1)
-	fstpt  0x98(%rsp)
-	fldt   0x9a8b(%rip)        
-	fmul   %st(4),%st
-	fldt   0x9a93(%rip)        
+	fstpt  0x78(%rsp)
+	fldt   0x9b81(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b89(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a99(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b8f(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9a9f(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b95(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9aa5(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9b9b(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9aab(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9ba1(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9ab1(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9ba7(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9ab7(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9bad(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9abd(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9bb3(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9ac3(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9bb9(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9ac9(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9bbf(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9acf(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9bc5(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9ad5(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9bcb(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0x9ad7(%rip)        
+	fmul   %st(3),%st
+	fadd   %st(1),%st
+	fmul   %st(3),%st
+	fldt   0x9bcd(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9add(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9bd3(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9ae3(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9bd9(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9ae9(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9bdf(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9aef(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9be5(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9af5(%rip)        
+	fmul   %st(3),%st
+	fldt   0x9beb(%rip)        
 	faddp  %st,%st(1)
-	fldt   0x9afd(%rip)        
-	fld    %st(5)
+	fldt   0x9bf3(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9aff(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bf5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9aff(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9bf5(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9aff(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9bf5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9aff(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9bf5(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9aff(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9bf5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9aff(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9bf5(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9aff(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9bf5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9aff(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9bf5(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9aff(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(4),%st
+	fldt   0x9bf5(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
-	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fsubp  %st,%st(1)
+	fmul   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   0x68(%rsp)
+	fldt   -0x48(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0xb8(%rsp)
+	fldt   0x98(%rsp)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0xf8(%rsp)
-	fldt   -0x48(%rsp)
+	fldt   0x138(%rsp)
+	fmul   %st(6),%st
+	faddp  %st,%st(1)
+	fldt   0x148(%rsp)
+	fldt   0x38(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x48(%rsp)
-	fmulp  %st,%st(3)
-	faddp  %st,%st(2)
 	faddp  %st,%st(1)
-	fldt   0x88(%rsp)
-	fldt   0x98(%rsp)
+	fldt   0x68(%rsp)
+	fldt   0x78(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fld    %st(3)
-	fldt   0x761b(%rip)        
-	fmulp  %st,%st(1)
-	fldt   0x7623(%rip)        
+	fldt   0x76f4(%rip)        
+	fld    %st(4)
+	fmul   %st(1),%st
+	fldt   0x76fa(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x7629(%rip)        
+	fmul   %st(5),%st
+	fldt   0x7700(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x762f(%rip)        
+	fmul   %st(5),%st
+	fldt   0x7706(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x7635(%rip)        
-	fadd   %st,%st(1)
-	fxch   %st(1)
 	fmul   %st(5),%st
-	fldt   0x7639(%rip)        
-	fsubr  %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(6),%st
-	fldt   0x763d(%rip)        
+	fldt   0x770c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x7643(%rip)        
+	fmul   %st(5),%st
+	fldt   0x7712(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x7718(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x771e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x7623(%rip)        
-	fsubrp %st,%st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x75e1(%rip)        
+	fldt   0x76fe(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x76e4(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x75c7(%rip)        
+	fmul   %st(5),%st
+	fldt   0x76ca(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x75ad(%rip)        
+	fmul   %st(5),%st
+	fldt   0x76b0(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x7593(%rip)        
+	fmul   %st(5),%st
+	fldt   0x7696(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x760b(%rip)        
-	fld    %st(5)
-	fmul   %st(1),%st
+	fmul   %st(5),%st
+	fldt   0x767c(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fsubp  %st,%st(1)
+	fldt   0x76e0(%rip)        
+	fmul   %st(5),%st
+	fldt   0x76d8(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x760d(%rip)        
+	fldt   0x76de(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x760d(%rip)        
+	fldt   0x76de(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x760d(%rip)        
+	fldt   0x76de(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x760d(%rip)        
+	fldt   0x76de(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x760d(%rip)        
+	fldt   0x76de(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
 	fadd   %st(3),%st
 	fmul   %st(5),%st
 	fadd   %st(3),%st
 	fmul   %st(5),%st
-	fldt   0x7605(%rip)        
+	fldt   0x76d6(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fldz
+	faddp  %st,%st(1)
 	fdivrp %st,%st(1)
-	fldt   0x78(%rsp)
+	fldt   0x58(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0xa8(%rsp)
+	fldt   0x88(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0xe8(%rsp)
+	fldt   0xd8(%rsp)
+	fmulp  %st,%st(5)
+	faddp  %st,%st(4)
+	fldt   0x118(%rsp)
 	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x128(%rsp)
-	fldt   -0x38(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x58(%rsp)
-	fldt   0x148(%rsp)
+	faddp  %st,%st(4)
+	fldt   0xe8(%rsp)
+	fldt   0x48(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x996f(%rip)        
-	fld    %st(5)
+	faddp  %st,%st(4)
+	faddp  %st,%st(3)
+	fldt   0x9a62(%rip)        
+	fld    %st(4)
 	fmul   %st(1),%st
-	fldt   0x9975(%rip)        
+	fldt   0x9a68(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x997b(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a6e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9981(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a74(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9987(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a7a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x998d(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a80(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9993(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a86(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9999(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a8c(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x999f(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a92(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x997f(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a72(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9965(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a58(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x994b(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a3e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9931(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a24(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9917(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a0a(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x98fd(%rip)        
+	fmul   %st(5),%st
+	fldt   0x99f0(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x98e3(%rip)        
+	fmul   %st(5),%st
+	fldt   0x99d6(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
+	fmul   %st(5),%st
 	fsubp  %st,%st(1)
-	fldt   0x9957(%rip)        
-	fld    %st(6)
-	fmul   %st(1),%st
+	fldt   0x9a4a(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a42(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x9959(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9a48(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9959(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a48(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9959(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a48(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9959(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a48(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9959(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a48(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9959(%rip)        
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a48(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9959(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9a48(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
 	fmul   %st(6),%st
-	fadd   %st(4),%st
-	fmul   %st(6),%st
-	faddp  %st,%st(4)
-	fxch   %st(3)
-	fmulp  %st,%st(5)
-	fxch   %st(4)
+	fsubp  %st,%st(1)
+	fmul   %st(5),%st
+	fadd   %st(3),%st
+	fmul   %st(5),%st
 	faddp  %st,%st(3)
+	fxch   %st(2)
+	fmulp  %st,%st(4)
+	fldz
+	faddp  %st,%st(4)
 	fxch   %st(1)
-	fdivp  %st,%st(2)
-	fldt   0x88(%rsp)
-	fmulp  %st,%st(2)
-	fldt   0xc8(%rsp)
+	fdivp  %st,%st(3)
+	fldt   0x68(%rsp)
+	fmulp  %st,%st(3)
+	fldt   0xa8(%rsp)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x108(%rsp)
-	fldt   -0x48(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x48(%rsp)
-	fldt   0x138(%rsp)
+	fldt   0xf8(%rsp)
+	fmulp  %st,%st(5)
+	faddp  %st,%st(4)
+	fldt   0xb8(%rsp)
+	fldt   0x38(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x68(%rsp)
-	fldt   0x98(%rsp)
+	faddp  %st,%st(4)
+	fldt   -0x48(%rsp)
+	fldt   0x78(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	faddp  %st,%st(2)
+	faddp  %st,%st(4)
+	fxch   %st(2)
+	faddp  %st,%st(3)
 	test   %esi,%esi
-	jle    8a4f <polyreg9+0x25df>
-	fldt   0x38(%rsp)
+	jle    8967 <polyreg9+0x25e7>
+	fldt   0x28(%rsp)
 	movslq %esi,%rsi
 	xor    %eax,%eax
-	fldt   0xd8(%rsp)
-	nopl   0x0(%rax)
+	fldt   0xc8(%rsp)
+	nopl   (%rax)
 	mov    %eax,-0x78(%rsp)
 	fildl  -0x78(%rsp)
 	fmul   %st(2),%st
 	fld1
 	fsubrp %st,%st(1)
-	fld    %st(4)
-	fmul   %st(1),%st
-	fadd   %st(6),%st
+	fld    %st(5)
 	fmul   %st(1),%st
 	fadd   %st(4),%st
 	fmul   %st(1),%st
-	fadd   %st(2),%st
+	fadd   %st(5),%st
 	fmul   %st(1),%st
-	fldt   0x28(%rsp)
-	faddp  %st,%st(1)
+	fadd   %st(2),%st
 	fmul   %st(1),%st
 	fldt   0x18(%rsp)
 	faddp  %st,%st(1)
 	fmul   %st(1),%st
 	fldt   0x8(%rsp)
 	faddp  %st,%st(1)
 	fmul   %st(1),%st
 	fldt   -0x8(%rsp)
 	faddp  %st,%st(1)
 	fmul   %st(1),%st
 	fldt   -0x18(%rsp)
 	faddp  %st,%st(1)
-	fmulp  %st,%st(1)
+	fmul   %st(1),%st
 	fldt   -0x28(%rsp)
 	faddp  %st,%st(1)
+	fmulp  %st,%st(1)
+	fldt   -0x38(%rsp)
+	faddp  %st,%st(1)
 	fsubrl (%rdi,%rax,8)
 	fstpl  (%rdx,%rax,8)
 	add    $0x1,%rax
 	cmp    %rax,%rsi
-	jne    89f0 <polyreg9+0x2580>
+	jne    8908 <polyreg9+0x2588>
 	fstp   %st(0)
 	fstp   %st(0)
-	fldt   -0x28(%rsp)
+	fldt   -0x38(%rsp)
 	fstpl  -0x78(%rsp)
-	fldt   -0x18(%rsp)
+	fldt   -0x28(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	fldt   -0x8(%rsp)
+	fldt   -0x18(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	movups %xmm0,(%r8)
+	movups %xmm0,(%rcx)
 	fstpl  -0x78(%rsp)
-	fldt   0x8(%rsp)
+	fldt   -0x8(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	fldt   0x18(%rsp)
+	fldt   0x8(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	movups %xmm0,0x10(%r8)
+	movups %xmm0,0x10(%rcx)
 	fstpl  -0x78(%rsp)
-	fldt   0x28(%rsp)
+	fldt   0x18(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	fldt   0xd8(%rsp)
+	fldt   0xc8(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	movups %xmm0,0x20(%r8)
+	movups %xmm0,0x20(%rcx)
 	fstpl  -0x78(%rsp)
+	fxch   %st(1)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	fxch   %st(1)
 	movhpd -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	movups %xmm0,0x30(%r8)
+	movups %xmm0,0x30(%rcx)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	movups %xmm0,0x40(%r8)
-	add    $0x170,%rsp
+	movups %xmm0,0x40(%rcx)
+	add    $0x160,%rsp
 	ret
-	nopl   0x0(%rax)
+	nopw   0x0(%rax,%rax,1)
 	fldz
-	fstpt  0x88(%rsp)
-	fldt   0x88(%rsp)
-	fstpt  0x78(%rsp)
-	fldt   0x78(%rsp)
 	fstpt  0x68(%rsp)
 	fldt   0x68(%rsp)
 	fstpt  0x58(%rsp)
 	fldt   0x58(%rsp)
-	fstpt  0x48(%rsp)
-	fldt   0x48(%rsp)
-	fstpt  -0x38(%rsp)
-	fldt   -0x38(%rsp)
 	fstpt  -0x48(%rsp)
 	fldt   -0x48(%rsp)
+	fstpt  0x48(%rsp)
+	fldt   0x48(%rsp)
+	fstpt  0x38(%rsp)
+	fldt   0x38(%rsp)
 	fstpt  -0x58(%rsp)
 	fldt   -0x58(%rsp)
+	fld    %st(0)
+	fstpt  -0x38(%rsp)
+	fldt   -0x38(%rsp)
 	fstpt  -0x68(%rsp)
 	fldt   -0x68(%rsp)
 	fstpt  -0x78(%rsp)
-	fldt   -0x78(%rsp)
-	jmp    6575 <polyreg9+0x105>
-	data16 cs nopw 0x0(%rax,%rax,1)
+	fxch   %st(1)
+	jmp    646c <polyreg9+0xec>
+	nop
 
-0000000000008b60 <polyreg10>:
+0000000000008a60 <polyreg10>:
 polyreg10():
-	sub    $0x1e0,%rsp
+	sub    $0x1d0,%rsp
 	mov    %esi,-0x78(%rsp)
 	fildl  -0x78(%rsp)
 	fld    %st(0)
 	fld1
 	fsubrp %st,%st(1)
-	fdivrs 0x44b5(%rip)        
+	fdivrs 0x45b5(%rip)        
 	fstpt  0x58(%rsp)
 	test   %esi,%esi
-	jle    b9d0 <polyreg10+0x2e70>
+	jle    b8b0 <polyreg10+0x2e50>
 	fldz
 	movslq %esi,%r8
 	xor    %eax,%eax
 	fld    %st(0)
 	fld    %st(1)
 	fld    %st(2)
-	fld    %st(3)
-	fld    %st(4)
 	fstpt  -0x28(%rsp)
 	fldt   -0x28(%rsp)
-	fstpt  -0x58(%rsp)
-	fldt   -0x58(%rsp)
+	fld    %st(0)
 	fstpt  -0x38(%rsp)
 	fldt   -0x38(%rsp)
-	fstpt  -0x68(%rsp)
-	fldt   -0x68(%rsp)
+	fld    %st(0)
 	fstpt  -0x48(%rsp)
 	fldt   -0x48(%rsp)
+	fstpt  -0x68(%rsp)
+	fldt   -0x68(%rsp)
+	fstpt  -0x58(%rsp)
+	fldt   -0x58(%rsp)
 	fstpt  -0x78(%rsp)
-	fldt   -0x78(%rsp)
-	fxch   %st(6)
-	fstpt  -0x8(%rsp)
 	fxch   %st(5)
-	fstps  0x8(%rsp)
-	nopl   0x0(%rax)
+	fstpt  -0x8(%rsp)
+	nopw   0x0(%rax,%rax,1)
 	mov    %eax,-0x18(%rsp)
 	fildl  -0x18(%rsp)
 	fldt   0x58(%rsp)
 	fmulp  %st,%st(1)
 	fld1
 	fsubrp %st,%st(1)
 	fldl   (%rdi,%rax,8)
 	fldt   -0x78(%rsp)
 	add    $0x1,%rax
 	fadd   %st(1),%st
 	fstpt  -0x78(%rsp)
 	fmul   %st(1),%st
-	fldt   -0x48(%rsp)
+	fldt   -0x58(%rsp)
 	fadd   %st(1),%st
-	fstpt  -0x48(%rsp)
+	fstpt  -0x58(%rsp)
 	fmul   %st(1),%st
 	fldt   -0x68(%rsp)
 	fadd   %st(1),%st
 	fstpt  -0x68(%rsp)
 	fmul   %st(1),%st
+	fldt   -0x48(%rsp)
+	fadd   %st(1),%st
+	fstpt  -0x48(%rsp)
+	fmul   %st(1),%st
+	fadd   %st,%st(6)
+	fmul   %st(1),%st
 	fldt   -0x38(%rsp)
 	fadd   %st(1),%st
 	fstpt  -0x38(%rsp)
 	fmul   %st(1),%st
-	fldt   -0x58(%rsp)
-	fadd   %st(1),%st
-	fstpt  -0x58(%rsp)
+	fadd   %st,%st(2)
 	fmul   %st(1),%st
 	fldt   -0x28(%rsp)
 	fadd   %st(1),%st
 	fstpt  -0x28(%rsp)
 	fmul   %st(1),%st
 	fadd   %st,%st(5)
 	fmul   %st(1),%st
-	fadd   %st,%st(6)
-	fmul   %st(1),%st
-	fadd   %st,%st(2)
-	fmul   %st(1),%st
 	fadd   %st,%st(3)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(3)
-	cmp    %r8,%rax
-	jne    8bd8 <polyreg10+0x78>
+	cmp    %rax,%r8
+	jne    8ad0 <polyreg10+0x70>
 	fldt   -0x8(%rsp)
-	fxch   %st(4)
+	fxch   %st(5)
 	fstpt  0x68(%rsp)
-	fxch   %st(4)
-	fstpt  0x98(%rsp)
-	fxch   %st(3)
 	fstpt  0x78(%rsp)
 	fxch   %st(2)
-	fstpt  0xa8(%rsp)
-	fxch   %st(1)
 	fstpt  0x88(%rsp)
-	flds   0x8(%rsp)
-	fldt   0x965b(%rip)        
-	fmul   %st(2),%st
-	fldt   0x9663(%rip)        
+	fxch   %st(1)
+	fstpt  0x98(%rsp)
+	fstpt  0xa8(%rsp)
+	fldt   0x977b(%rip)        
+	fmul   %st(1),%st
+	fldt   0x9783(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0x9669(%rip)        
+	fmul   %st(1),%st
+	fldt   0x9789(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0x966f(%rip)        
+	fmul   %st(1),%st
+	fldt   0x978f(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0x9675(%rip)        
+	fmul   %st(1),%st
+	fldt   0x9795(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0x967b(%rip)        
+	fmul   %st(1),%st
+	fldt   0x979b(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0x9681(%rip)        
+	fmul   %st(1),%st
+	fldt   0x97a1(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0x9687(%rip)        
+	fmul   %st(1),%st
+	fldt   0x97a7(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
-	fldt   0x968d(%rip)        
+	fmul   %st(1),%st
+	fldt   0x97ad(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(2),%st
+	fmul   %st(1),%st
 	fld1
 	fadd   %st,%st(1)
 	fxch   %st(1)
+	fmul   %st(2),%st
+	fsubs  0x4463(%rip)        
+	fldt   0x97a5(%rip)        
 	fmul   %st(3),%st
-	fsubs  0x4353(%rip)        
-	fldt   0x9685(%rip)        
-	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fldz
+	fadd   %st,%st(1)
+	fxch   %st(1)
 	fmul   %st(4),%st
-	fldt   0x9689(%rip)        
+	fldt   0x97a5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x968b(%rip)        
+	fldt   0x97a7(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x968d(%rip)        
+	fldt   0x97a9(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x968f(%rip)        
+	fldt   0x97ab(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x9691(%rip)        
+	fldt   0x97ad(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fdivrp %st,%st(1)
-	fldt   0x9693(%rip)        
+	fadd   %st(1),%st
+	fdivrp %st,%st(2)
+	fldt   0x97af(%rip)        
 	fmul   %st(4),%st
-	fldt   0x969b(%rip)        
+	fldt   0x97b7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96a1(%rip)        
+	fldt   0x97bd(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96a7(%rip)        
+	fldt   0x97c3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96ad(%rip)        
+	fldt   0x97c9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96b3(%rip)        
+	fldt   0x97cf(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96b9(%rip)        
+	fldt   0x97d5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96bf(%rip)        
+	fldt   0x97db(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96c5(%rip)        
+	fldt   0x97e1(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fsubs  0x42a3(%rip)        
-	fldt   0x96c1(%rip)        
+	fsubs  0x43af(%rip)        
+	fldt   0x97dd(%rip)        
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x96c5(%rip)        
+	fldt   0x97e1(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x96c7(%rip)        
+	fldt   0x97e3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x96c9(%rip)        
+	fldt   0x97e5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x96cb(%rip)        
+	fldt   0x97e7(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x96cd(%rip)        
+	fldt   0x97e9(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fdivrp %st,%st(1)
 	fstpt  0x28(%rsp)
-	fldt   0x96cb(%rip)        
+	fldt   0x97e7(%rip)        
 	fmul   %st(4),%st
-	fldt   0x96d3(%rip)        
+	fldt   0x97ef(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96d9(%rip)        
+	fldt   0x97f5(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96df(%rip)        
+	fldt   0x97fb(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96e5(%rip)        
+	fldt   0x9801(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96eb(%rip)        
+	fldt   0x9807(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96f1(%rip)        
+	fldt   0x980d(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x96f3(%rip)        
+	fldt   0x980f(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96f9(%rip)        
+	fldt   0x9815(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x96ff(%rip)        
+	fldt   0x981b(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9707(%rip)        
+	fldt   0x9823(%rip)        
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x970b(%rip)        
+	fldt   0x9827(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x970d(%rip)        
+	fldt   0x9829(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x970f(%rip)        
+	fldt   0x982b(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x9711(%rip)        
+	fldt   0x982d(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x9713(%rip)        
+	fldt   0x982f(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fdivrp %st,%st(1)
 	fstpt  0x48(%rsp)
-	fldt   0x9711(%rip)        
+	fldt   0x982d(%rip)        
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x9715(%rip)        
+	fldt   0x9831(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x9717(%rip)        
+	fldt   0x9833(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
-	fldt   0x9719(%rip)        
+	fldt   0x9835(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(1),%st
 	fmul   %st(4),%st
 	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x9713(%rip)        
+	fadd   %st(1),%st
+	fmul   %st(4),%st
+	fldt   0x982f(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fldt   0x9717(%rip)        
+	fadd   %st(1),%st
+	fldt   0x9833(%rip)        
 	fmul   %st(5),%st
-	fldt   0x971f(%rip)        
+	fldt   0x983b(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9725(%rip)        
+	fldt   0x9841(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x972b(%rip)        
+	fldt   0x9847(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9731(%rip)        
+	fldt   0x984d(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9737(%rip)        
+	fldt   0x9853(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x973d(%rip)        
+	fldt   0x9859(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9743(%rip)        
+	fldt   0x985f(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9749(%rip)        
+	fldt   0x9865(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x974f(%rip)        
+	fldt   0x986b(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9755(%rip)        
+	fldt   0x9871(%rip)        
 	fsubrp %st,%st(1)
 	fdiv   %st(1),%st
 	fstpt  0xd8(%rsp)
-	fldt   0x9754(%rip)        
-	fmul   %st(5),%st
-	fldt   0x975c(%rip)        
-	faddp  %st,%st(1)
+	fldt   0x9870(%rip)        
 	fmul   %st(5),%st
-	fldt   0x9762(%rip)        
-	fsubr  %st,%st(1)
+	fldt   0x9878(%rip)        
+	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
-	fldt   0x9766(%rip)        
+	fldt   0x987c(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(6),%st
+	fldt   0x9882(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x976c(%rip)        
+	fldt   0x9888(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9772(%rip)        
+	fldt   0x988e(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x9758(%rip)        
+	fldt   0x9874(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(6),%st
-	fldt   0x973e(%rip)        
+	fldt   0x985a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x9710(%rip)        
+	fldt   0x9840(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9756(%rip)        
+	fldt   0x9872(%rip)        
 	fsubrp %st,%st(1)
 	fdivp  %st,%st(1)
-	fstpt  0xe8(%rsp)
-	fldt   0x9755(%rip)        
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0x9759(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0x975b(%rip)        
-	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0x975d(%rip)        
-	fsubrp %st,%st(1)
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fadd   %st(3),%st
-	fmul   %st(4),%st
-	fldt   0x9757(%rip)        
-	fsubrp %st,%st(1)
-	fldt   0x975f(%rip)        
+	fldt   0x9878(%rip)        
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x9763(%rip)        
+	fldt   0x987c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x9765(%rip)        
+	fldt   0x987e(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fldt   0x9767(%rip)        
+	fldt   0x9880(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
-	fmul   %st(5),%st
-	fldt   0x9769(%rip)        
-	faddp  %st,%st(1)
+	fadd   %st(2),%st
 	fmul   %st(5),%st
 	fadd   %st(4),%st
 	fmul   %st(5),%st
-	fldt   0x976b(%rip)        
-	fsubrp %st,%st(1)
+	fadd   %st(2),%st
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fldt   0x987a(%rip)        
+	fsubrp %st,%st(1)
+	fldt   0x9882(%rip)        
+	fmul   %st(6),%st
+	fadd   %st(3),%st
+	fmul   %st(6),%st
+	fldt   0x9886(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(6),%st
+	fadd   %st(3),%st
+	fmul   %st(6),%st
+	fldt   0x9888(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(6),%st
+	fadd   %st(3),%st
+	fmul   %st(6),%st
+	fldt   0x988a(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(6),%st
+	fadd   %st(3),%st
+	fmul   %st(6),%st
+	fldt   0x988c(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(6),%st
+	fadd   %st(3),%st
+	fmul   %st(6),%st
+	fldt   0x988e(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(6),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
 	fldt   -0x68(%rsp)
-	fxch   %st(2)
+	fxch   %st(4)
 	fld    %st(0)
 	fstpt  0x8(%rsp)
-	fmulp  %st,%st(2)
-	faddp  %st,%st(1)
-	fldt   -0x58(%rsp)
+	fmulp  %st,%st(4)
+	faddp  %st,%st(3)
 	fldt   0x28(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x48(%rsp)
 	fldt   0x68(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
+	faddp  %st,%st(3)
+	fldt   0x48(%rsp)
 	fldt   0x78(%rsp)
-	fldt   0xd8(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
+	faddp  %st,%st(3)
 	fldt   0x88(%rsp)
-	fldt   0xe8(%rsp)
+	fldt   0xd8(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
+	faddp  %st,%st(3)
+	fldt   0xa8(%rsp)
+	fxch   %st(1)
+	fld    %st(0)
+	fstpt  0x1a8(%rsp)
+	fmulp  %st,%st(1)
+	faddp  %st,%st(2)
+	fxch   %st(1)
 	fstpt  -0x18(%rsp)
-	fldt   0x971a(%rip)        
+	fldt   0x9834(%rip)        
 	fmul   %st(3),%st
-	fldt   0x9722(%rip)        
+	fldt   0x983c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9728(%rip)        
+	fldt   0x9842(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x972e(%rip)        
+	fldt   0x9848(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9734(%rip)        
+	fldt   0x984e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x973a(%rip)        
+	fldt   0x9854(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9740(%rip)        
+	fldt   0x985a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9746(%rip)        
+	fldt   0x9860(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x974c(%rip)        
+	fldt   0x9866(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9752(%rip)        
+	fldt   0x986c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9758(%rip)        
+	fldt   0x9872(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x975e(%rip)        
+	fldt   0x9878(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9764(%rip)        
+	fldt   0x987e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x976a(%rip)        
+	fldt   0x9884(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9770(%rip)        
+	fldt   0x988a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9776(%rip)        
+	fldt   0x9890(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fadd   %st(1),%st
+	fadd   %st(2),%st
 	fmul   %st(3),%st
-	fldt   0x3ef8(%rip)        
+	fldt   0x3ff2(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9770(%rip)        
+	fldt   0x988a(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9772(%rip)        
+	fldt   0x988c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9772(%rip)        
+	fldt   0x988c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9772(%rip)        
+	fldt   0x988c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9772(%rip)        
+	fldt   0x988c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9772(%rip)        
+	fldt   0x988c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9772(%rip)        
+	fldt   0x988c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9772(%rip)        
+	fldt   0x988c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9772(%rip)        
+	fldt   0x988c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(2),%st
 	fdivrp %st,%st(1)
-	fldt   0x976e(%rip)        
+	fldt   0x9888(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9776(%rip)        
+	fldt   0x9890(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x977c(%rip)        
+	fldt   0x9896(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9782(%rip)        
+	fldt   0x989c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9788(%rip)        
+	fldt   0x98a2(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x978e(%rip)        
+	fldt   0x98a8(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9794(%rip)        
+	fldt   0x98ae(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x979a(%rip)        
+	fldt   0x98b4(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97a0(%rip)        
+	fldt   0x98ba(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97a6(%rip)        
+	fldt   0x98c0(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97ac(%rip)        
+	fldt   0x98c6(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97b2(%rip)        
+	fldt   0x98cc(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97b8(%rip)        
+	fldt   0x98d2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97be(%rip)        
+	fldt   0x98d8(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x97c0(%rip)        
+	fldt   0x98da(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97c6(%rip)        
+	fldt   0x98e0(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97cc(%rip)        
+	fldt   0x98e6(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x97d4(%rip)        
+	fldt   0x98ee(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d6(%rip)        
+	fldt   0x98f0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d6(%rip)        
+	fldt   0x98f0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d6(%rip)        
+	fldt   0x98f0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d6(%rip)        
+	fldt   0x98f0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d6(%rip)        
+	fldt   0x98f0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d6(%rip)        
+	fldt   0x98f0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d6(%rip)        
+	fldt   0x98f0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d6(%rip)        
+	fldt   0x98f0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
 	fstpt  0x38(%rsp)
-	fldt   0x97ce(%rip)        
+	fldt   0x98e8(%rip)        
 	fmul   %st(4),%st
-	fldt   0x97d6(%rip)        
+	fldt   0x98f0(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97dc(%rip)        
+	fldt   0x98f6(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97e2(%rip)        
+	fldt   0x98fc(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97e8(%rip)        
+	fldt   0x9902(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97ee(%rip)        
+	fldt   0x9908(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97f4(%rip)        
+	fldt   0x990e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x97fa(%rip)        
+	fldt   0x9914(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9800(%rip)        
+	fldt   0x991a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9806(%rip)        
+	fldt   0x9920(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x980c(%rip)        
+	fldt   0x9926(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9812(%rip)        
+	fldt   0x992c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9818(%rip)        
+	fldt   0x9932(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x981e(%rip)        
+	fldt   0x9938(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x9820(%rip)        
+	fldt   0x993a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9826(%rip)        
+	fldt   0x9940(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x982c(%rip)        
+	fldt   0x9946(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9834(%rip)        
+	fldt   0x994e(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9836(%rip)        
+	fldt   0x9950(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9836(%rip)        
+	fldt   0x9950(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9836(%rip)        
+	fldt   0x9950(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9836(%rip)        
+	fldt   0x9950(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9836(%rip)        
+	fldt   0x9950(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9836(%rip)        
+	fldt   0x9950(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9836(%rip)        
+	fldt   0x9950(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9836(%rip)        
+	fldt   0x9950(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fstpt  0xf8(%rsp)
-	fldt   0x8ddb(%rip)        
+	fstpt  0xe8(%rsp)
+	fldt   0x8ef5(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8ddd(%rip)        
+	fldt   0x8ef7(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8ddd(%rip)        
+	fldt   0x8ef7(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8ddd(%rip)        
+	fldt   0x8ef7(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8ddd(%rip)        
+	fldt   0x8ef7(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8ddd(%rip)        
+	fldt   0x8ef7(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8ddd(%rip)        
+	fldt   0x8ef7(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x8ddd(%rip)        
+	fldt   0x8ef7(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
 	fadd   %st(3),%st
-	fldt   0x97a3(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(2),%st
+	fldt   0x98bd(%rip)        
 	fmul   %st(5),%st
-	fldt   0x97ab(%rip)        
+	fldt   0x98c5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97b1(%rip)        
+	fldt   0x98cb(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97b7(%rip)        
+	fldt   0x98d1(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97bd(%rip)        
+	fldt   0x98d7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97c3(%rip)        
+	fldt   0x98dd(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97c9(%rip)        
+	fldt   0x98e3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97cf(%rip)        
+	fldt   0x98e9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97d5(%rip)        
+	fldt   0x98ef(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97db(%rip)        
+	fldt   0x98f5(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97e1(%rip)        
+	fldt   0x98fb(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97e7(%rip)        
+	fldt   0x9901(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97ed(%rip)        
+	fldt   0x9907(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97f3(%rip)        
+	fldt   0x990d(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97f9(%rip)        
+	fldt   0x9913(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x97ff(%rip)        
+	fldt   0x9919(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9805(%rip)        
+	fldt   0x991f(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x980b(%rip)        
+	fldt   0x9925(%rip)        
 	fsubrp %st,%st(1)
 	fxch   %st(1)
 	fld    %st(0)
 	fstpt  0xc8(%rsp)
 	fdivrp %st,%st(1)
-	fstpt  0x108(%rsp)
-	fldt   0x97ff(%rip)        
-	fld    %st(4)
+	fldt   0x9920(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9801(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9922(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9801(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9922(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9801(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9922(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9801(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9922(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9801(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9922(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9801(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9922(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fsub   %st(2),%st
-	fmul   %st(4),%st
-	fadd   %st(2),%st
-	fmul   %st(4),%st
-	fldt   0x97f9(%rip)        
+	fmul   %st(5),%st
+	fsub   %st(4),%st
+	fmul   %st(5),%st
+	fadd   %st(4),%st
+	fmul   %st(5),%st
+	fldt   0x991a(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fldt   0x97fb(%rip)        
-	fld    %st(5)
+	fldt   0x991c(%rip)        
+	fld    %st(6)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x97fd(%rip)        
+	fmul   %st(6),%st
+	fldt   0x991e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x97fd(%rip)        
+	fmul   %st(6),%st
+	fldt   0x991e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x97fd(%rip)        
+	fmul   %st(6),%st
+	fldt   0x991e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x97fd(%rip)        
+	fmul   %st(6),%st
+	fldt   0x991e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x97fd(%rip)        
+	fmul   %st(6),%st
+	fldt   0x991e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x97fd(%rip)        
+	fmul   %st(6),%st
+	fldt   0x991e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x97fd(%rip)        
+	fmul   %st(6),%st
+	fldt   0x991e(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	fsubp  %st,%st(1)
-	fmul   %st(5),%st
-	fldt   0x97fd(%rip)        
+	fmul   %st(6),%st
+	fldt   0x991e(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(6),%st
+	fmul   %st(7),%st
 	faddp  %st,%st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fadd   %st(4),%st
 	fdivrp %st,%st(1)
-	fldt   -0x48(%rsp)
+	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
-	fldt   -0x38(%rsp)
-	fxch   %st(2)
+	fldt   -0x48(%rsp)
+	fxch   %st(3)
 	fld    %st(0)
 	fstpt  0x18(%rsp)
-	fmulp  %st,%st(2)
-	faddp  %st,%st(1)
-	fldt   -0x28(%rsp)
+	fmulp  %st,%st(3)
+	faddp  %st,%st(2)
+	fldt   -0x38(%rsp)
 	fldt   0x38(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x98(%rsp)
-	fldt   0xf8(%rsp)
+	faddp  %st,%st(2)
+	fldt   -0x28(%rsp)
+	fldt   0xe8(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0xa8(%rsp)
-	fldt   0x108(%rsp)
+	faddp  %st,%st(2)
+	fldt   0x98(%rsp)
+	fxch   %st(1)
+	fld    %st(0)
+	fstpt  0x1b8(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	fstpt  -0x8(%rsp)
-	fldt   0x97af(%rip)        
+	fldt   0x98cf(%rip)        
 	fmul   %st(3),%st
-	fldt   0x97b7(%rip)        
+	fldt   0x98d7(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x97bd(%rip)        
+	fldt   0x98dd(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x97c3(%rip)        
+	fldt   0x98e3(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x97c9(%rip)        
+	fldt   0x98e9(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x97cf(%rip)        
+	fldt   0x98ef(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x97d5(%rip)        
+	fldt   0x98f5(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x97db(%rip)        
+	fldt   0x98fb(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x97e1(%rip)        
+	fldt   0x9901(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x97e7(%rip)        
+	fldt   0x9907(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x97ed(%rip)        
+	fldt   0x990d(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x97f3(%rip)        
+	fldt   0x9913(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x97f9(%rip)        
+	fldt   0x9919(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x97ff(%rip)        
+	fldt   0x991f(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9805(%rip)        
+	fldt   0x9925(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x980b(%rip)        
+	fldt   0x992b(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fadd   %st(1),%st
+	fadd   %st(2),%st
 	fmul   %st(3),%st
-	fldt   0x980d(%rip)        
+	fldt   0x992d(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9813(%rip)        
+	fldt   0x9933(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9819(%rip)        
+	fldt   0x9939(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9821(%rip)        
+	fldt   0x9941(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9823(%rip)        
+	fldt   0x9943(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9823(%rip)        
+	fldt   0x9943(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9823(%rip)        
+	fldt   0x9943(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9823(%rip)        
+	fldt   0x9943(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9823(%rip)        
+	fldt   0x9943(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9823(%rip)        
+	fldt   0x9943(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9823(%rip)        
+	fldt   0x9943(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9823(%rip)        
+	fldt   0x9943(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9823(%rip)        
+	fldt   0x9943(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(2),%st
 	fdivrp %st,%st(1)
-	fstpt  0x118(%rsp)
-	fldt   0x9818(%rip)        
+	fstpt  0xf8(%rsp)
+	fldt   0x9938(%rip)        
 	fmul   %st(3),%st
-	fldt   0x9820(%rip)        
+	fldt   0x9940(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9826(%rip)        
+	fldt   0x9946(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x982c(%rip)        
+	fldt   0x994c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9832(%rip)        
+	fldt   0x9952(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9838(%rip)        
+	fldt   0x9958(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x983e(%rip)        
+	fldt   0x995e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9844(%rip)        
+	fldt   0x9964(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x984a(%rip)        
+	fldt   0x996a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9850(%rip)        
+	fldt   0x9970(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9856(%rip)        
+	fldt   0x9976(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x985c(%rip)        
+	fldt   0x997c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9862(%rip)        
+	fldt   0x9982(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9868(%rip)        
+	fldt   0x9988(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x986e(%rip)        
+	fldt   0x998e(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9874(%rip)        
+	fldt   0x9994(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fadd   %st(1),%st
+	fadd   %st(2),%st
 	fmul   %st(3),%st
-	fldt   0x9876(%rip)        
+	fldt   0x9996(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x987c(%rip)        
+	fldt   0x999c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9882(%rip)        
+	fldt   0x99a2(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x988a(%rip)        
+	fldt   0x99aa(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x988c(%rip)        
+	fldt   0x99ac(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x988c(%rip)        
+	fldt   0x99ac(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x988c(%rip)        
+	fldt   0x99ac(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x988c(%rip)        
+	fldt   0x99ac(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x988c(%rip)        
+	fldt   0x99ac(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x988c(%rip)        
+	fldt   0x99ac(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x988c(%rip)        
+	fldt   0x99ac(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x988c(%rip)        
+	fldt   0x99ac(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x988c(%rip)        
+	fldt   0x99ac(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(2),%st
 	fdivrp %st,%st(1)
-	fstpt  0x128(%rsp)
-	fldt   0x9881(%rip)        
+	fstpt  0x108(%rsp)
+	fldt   0x99a1(%rip)        
 	fmul   %st(3),%st
-	fldt   0x9889(%rip)        
+	fldt   0x99a9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x988f(%rip)        
+	fldt   0x99af(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9895(%rip)        
+	fldt   0x99b5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x989b(%rip)        
+	fldt   0x99bb(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98a1(%rip)        
+	fldt   0x99c1(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98a7(%rip)        
+	fldt   0x99c7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98ad(%rip)        
+	fldt   0x99cd(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98b3(%rip)        
+	fldt   0x99d3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98b9(%rip)        
+	fldt   0x99d9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98bf(%rip)        
+	fldt   0x99df(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98c5(%rip)        
+	fldt   0x99e5(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98cb(%rip)        
+	fldt   0x99eb(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98d1(%rip)        
+	fldt   0x99f1(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fadd   %st(1),%st
+	fadd   %st(2),%st
 	fmul   %st(3),%st
-	fldt   0x98d3(%rip)        
+	fldt   0x99f3(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98d9(%rip)        
+	fldt   0x99f9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98df(%rip)        
+	fldt   0x99ff(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98e5(%rip)        
+	fldt   0x9a05(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98eb(%rip)        
+	fldt   0x9a0b(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x98f3(%rip)        
+	fldt   0x9a13(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98f5(%rip)        
+	fldt   0x9a15(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98f5(%rip)        
+	fldt   0x9a15(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98f5(%rip)        
+	fldt   0x9a15(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98f5(%rip)        
+	fldt   0x9a15(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98f5(%rip)        
+	fldt   0x9a15(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98f5(%rip)        
+	fldt   0x9a15(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98f5(%rip)        
+	fldt   0x9a15(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98f5(%rip)        
+	fldt   0x9a15(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98f5(%rip)        
+	fldt   0x9a15(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(2),%st
 	fdivrp %st,%st(1)
-	fstpt  0x138(%rsp)
-	fldt   0x98ea(%rip)        
+	fstpt  0x118(%rsp)
+	fldt   0x9a0a(%rip)        
 	fld    %st(3)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98ec(%rip)        
+	fldt   0x9a0c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(4),%st
 	fsubp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98ec(%rip)        
+	fldt   0x9a0c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(4),%st
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98ec(%rip)        
+	fldt   0x9a0c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(4),%st
 	fsubp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98ec(%rip)        
+	fldt   0x9a0c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(4),%st
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98ec(%rip)        
+	fldt   0x9a0c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(4),%st
 	fsubp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98ec(%rip)        
+	fldt   0x9a0c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(4),%st
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x98ec(%rip)        
+	fldt   0x9a0c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(4),%st
 	fsubp  %st,%st(1)
 	fmul   %st(3),%st
-	fadd   %st(1),%st
+	fadd   %st(2),%st
 	fmul   %st(3),%st
-	fadd   %st(1),%st
+	fadd   %st(2),%st
 	fmul   %st(3),%st
-	fldt   0x98e4(%rip)        
+	fldt   0x9a04(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(4),%st
 	fsubp  %st,%st(1)
 	fmul   %st(3),%st
-	fadd   %st(2),%st
-	fldt   0x98e2(%rip)        
+	fadd   %st(1),%st
+	fldt   0x9a02(%rip)        
 	fmul   %st(4),%st
-	fldt   0x98ea(%rip)        
+	fldt   0x9a0a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98f0(%rip)        
+	fldt   0x9a10(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98f6(%rip)        
+	fldt   0x9a16(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x98fc(%rip)        
+	fldt   0x9a1c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9902(%rip)        
+	fldt   0x9a22(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9908(%rip)        
+	fldt   0x9a28(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x990e(%rip)        
+	fldt   0x9a2e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9914(%rip)        
+	fldt   0x9a34(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x991a(%rip)        
+	fldt   0x9a3a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9920(%rip)        
+	fldt   0x9a40(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9926(%rip)        
+	fldt   0x9a46(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x992c(%rip)        
+	fldt   0x9a4c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9932(%rip)        
+	fldt   0x9a52(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9938(%rip)        
+	fldt   0x9a58(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x993e(%rip)        
+	fldt   0x9a5e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9944(%rip)        
+	fldt   0x9a64(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x994a(%rip)        
+	fldt   0x9a6a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9950(%rip)        
+	fldt   0x9a70(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9956(%rip)        
+	fldt   0x9a76(%rip)        
 	fsubrp %st,%st(1)
 	fxch   %st(1)
 	fld    %st(0)
 	fstpt  0xb8(%rsp)
 	fdivrp %st,%st(1)
-	fstpt  0x148(%rsp)
-	fldt   0x994a(%rip)        
+	fstpt  0x128(%rsp)
+	fldt   0x9a6a(%rip)        
 	fmul   %st(3),%st
-	fldt   0x9952(%rip)        
+	fldt   0x9a72(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9958(%rip)        
+	fldt   0x9a78(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x995e(%rip)        
+	fldt   0x9a7e(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9964(%rip)        
+	fldt   0x9a84(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x996a(%rip)        
+	fldt   0x9a8a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9970(%rip)        
+	fldt   0x9a90(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9976(%rip)        
+	fldt   0x9a96(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x997c(%rip)        
+	fldt   0x9a9c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9982(%rip)        
+	fldt   0x9aa2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9988(%rip)        
+	fldt   0x9aa8(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x998e(%rip)        
+	fldt   0x9aae(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9994(%rip)        
+	fldt   0x9ab4(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x999a(%rip)        
+	fldt   0x9aba(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x99a0(%rip)        
+	fldt   0x9ac0(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x99a6(%rip)        
+	fldt   0x9ac6(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x99ac(%rip)        
+	fldt   0x9acc(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x99b2(%rip)        
+	fldt   0x9ad2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fadd   %st(1),%st
+	fadd   %st(2),%st
 	fmul   %st(3),%st
-	fldt   0x32d4(%rip)        
+	fldt   0x33d4(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x99ac(%rip)        
+	fldt   0x9acc(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99ae(%rip)        
+	fldt   0x9ace(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99ae(%rip)        
+	fldt   0x9ace(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99ae(%rip)        
+	fldt   0x9ace(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99ae(%rip)        
+	fldt   0x9ace(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99ae(%rip)        
+	fldt   0x9ace(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99ae(%rip)        
+	fldt   0x9ace(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99ae(%rip)        
+	fldt   0x9ace(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99ae(%rip)        
+	fldt   0x9ace(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99ae(%rip)        
+	fldt   0x9ace(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(3),%st
+	fadd   %st(2),%st
 	fdivrp %st,%st(1)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
 	fldt   0x8(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   -0x58(%rsp)
-	fldt   0x118(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x128(%rsp)
+	fldt   0xf8(%rsp)
 	fldt   0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
+	fldt   0x108(%rsp)
 	fldt   0x78(%rsp)
-	fldt   0x138(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	fldt   0x88(%rsp)
-	fldt   0x148(%rsp)
+	fldt   0x118(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
+	fldt   0xa8(%rsp)
+	fld    %st(0)
+	fldt   0x128(%rsp)
+	fmulp  %st,%st(1)
+	faddp  %st,%st(2)
+	fxch   %st(1)
 	fstpt  0x8(%rsp)
-	fldt   0x9955(%rip)        
-	fmul   %st(3),%st
-	fldt   0x995d(%rip)        
+	fldt   0x9a6e(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a76(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9963(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a7c(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9969(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a82(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x996f(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a88(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9975(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a8e(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x997b(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a94(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9981(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9a9a(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9987(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9aa0(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x998d(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9aa6(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9993(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9aac(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9999(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ab2(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x999f(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ab8(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x99a5(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9abe(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0x99a7(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(3),%st
+	fmul   %st(4),%st
+	fldt   0x9ac0(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x99ad(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ac6(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x99b3(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9acc(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x99bb(%rip)        
-	fld    %st(4)
+	fldt   0x9ad4(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99bd(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9ad6(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99bd(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9ad6(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99bd(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9ad6(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99bd(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9ad6(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99bd(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9ad6(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99bd(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9ad6(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99bd(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9ad6(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x99bd(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9ad6(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fldt   0x99b9(%rip)        
+	fstpt  0xa8(%rsp)
+	fldt   0x9acb(%rip)        
 	fmul   %st(4),%st
-	fldt   0x99c1(%rip)        
+	fldt   0x9ad3(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99c7(%rip)        
+	fldt   0x9ad9(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99cd(%rip)        
+	fldt   0x9adf(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99d3(%rip)        
+	fldt   0x9ae5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99d9(%rip)        
+	fldt   0x9aeb(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99df(%rip)        
+	fldt   0x9af1(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99e5(%rip)        
+	fldt   0x9af7(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99eb(%rip)        
+	fldt   0x9afd(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99f1(%rip)        
+	fldt   0x9b03(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99f7(%rip)        
+	fldt   0x9b09(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x99fd(%rip)        
+	fldt   0x9b0f(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x99ff(%rip)        
+	fldt   0x9b11(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a05(%rip)        
+	fldt   0x9b17(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a0b(%rip)        
+	fldt   0x9b1d(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a11(%rip)        
+	fldt   0x9b23(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a17(%rip)        
+	fldt   0x9b29(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9a1f(%rip)        
+	fldt   0x9b31(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a21(%rip)        
+	fldt   0x9b33(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a21(%rip)        
+	fldt   0x9b33(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a21(%rip)        
+	fldt   0x9b33(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a21(%rip)        
+	fldt   0x9b33(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a21(%rip)        
+	fldt   0x9b33(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a21(%rip)        
+	fldt   0x9b33(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a21(%rip)        
+	fldt   0x9b33(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a21(%rip)        
+	fldt   0x9b33(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fstpt  0x158(%rsp)
-	fldt   0x9a16(%rip)        
+	fstpt  0x138(%rsp)
+	fldt   0x9b28(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9a1e(%rip)        
+	fldt   0x9b30(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a24(%rip)        
+	fldt   0x9b36(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a2a(%rip)        
+	fldt   0x9b3c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a30(%rip)        
+	fldt   0x9b42(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a36(%rip)        
+	fldt   0x9b48(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a3c(%rip)        
+	fldt   0x9b4e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a42(%rip)        
+	fldt   0x9b54(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a48(%rip)        
+	fldt   0x9b5a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a4e(%rip)        
+	fldt   0x9b60(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a54(%rip)        
+	fldt   0x9b66(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a5a(%rip)        
+	fldt   0x9b6c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x9a5c(%rip)        
+	fldt   0x9b6e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a62(%rip)        
+	fldt   0x9b74(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a68(%rip)        
+	fldt   0x9b7a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a6e(%rip)        
+	fldt   0x9b80(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a74(%rip)        
+	fldt   0x9b86(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9a7c(%rip)        
+	fldt   0x9b8e(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a7e(%rip)        
+	fldt   0x9b90(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a7e(%rip)        
+	fldt   0x9b90(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a7e(%rip)        
+	fldt   0x9b90(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a7e(%rip)        
+	fldt   0x9b90(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a7e(%rip)        
+	fldt   0x9b90(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a7e(%rip)        
+	fldt   0x9b90(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a7e(%rip)        
+	fldt   0x9b90(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9a7e(%rip)        
+	fldt   0x9b90(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fstpt  0x168(%rsp)
-	fldt   0x9a73(%rip)        
+	fstpt  0x148(%rsp)
+	fldt   0x9b85(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9a7b(%rip)        
+	fldt   0x9b8d(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a81(%rip)        
+	fldt   0x9b93(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a87(%rip)        
+	fldt   0x9b99(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a8d(%rip)        
+	fldt   0x9b9f(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a93(%rip)        
+	fldt   0x9ba5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a99(%rip)        
+	fldt   0x9bab(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9a9f(%rip)        
+	fldt   0x9bb1(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9aa5(%rip)        
+	fldt   0x9bb7(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9aab(%rip)        
+	fldt   0x9bbd(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ab1(%rip)        
+	fldt   0x9bc3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ab7(%rip)        
+	fldt   0x9bc9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9abd(%rip)        
+	fldt   0x9bcf(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ac3(%rip)        
+	fldt   0x9bd5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x9ac5(%rip)        
+	fldt   0x9bd7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9acb(%rip)        
+	fldt   0x9bdd(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ad1(%rip)        
+	fldt   0x9be3(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9ad9(%rip)        
+	fldt   0x9beb(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9adb(%rip)        
+	fldt   0x9bed(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9adb(%rip)        
+	fldt   0x9bed(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9adb(%rip)        
+	fldt   0x9bed(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9adb(%rip)        
+	fldt   0x9bed(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9adb(%rip)        
+	fldt   0x9bed(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9adb(%rip)        
+	fldt   0x9bed(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9adb(%rip)        
+	fldt   0x9bed(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9adb(%rip)        
+	fldt   0x9bed(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fldt   -0x38(%rsp)
+	fldt   -0x48(%rsp)
 	fmulp  %st,%st(1)
 	fldt   0x18(%rsp)
-	fldt   -0x48(%rsp)
+	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   -0x28(%rsp)
-	fxch   %st(2)
-	fld    %st(0)
-	fstpt  0x1a8(%rsp)
-	fmulp  %st,%st(2)
+	fldt   -0x38(%rsp)
+	fldt   0xa8(%rsp)
+	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x98(%rsp)
-	fldt   0x158(%rsp)
+	fldt   -0x28(%rsp)
+	fldt   0x138(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0xa8(%rsp)
-	fldt   0x168(%rsp)
+	fldt   0x98(%rsp)
+	fldt   0x148(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	fstpt  0x18(%rsp)
-	fldt   0x9a8a(%rip)        
-	fmul   %st(3),%st
-	fldt   0x9a92(%rip)        
+	fldt   0x9ba3(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bab(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9a98(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bb1(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9a9e(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bb7(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9aa4(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bbd(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9aaa(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bc3(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9ab0(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bc9(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9ab6(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bcf(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9abc(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bd5(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9ac2(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bdb(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9ac8(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9be1(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9ace(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9be7(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9ad4(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bed(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9ada(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bf3(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0x9adc(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(3),%st
+	fmul   %st(4),%st
+	fldt   0x9bf5(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9ae2(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9bfb(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9ae8(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9c01(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9aee(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9c07(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9af4(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9c0d(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9afc(%rip)        
-	fld    %st(4)
+	fldt   0x9c15(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9afe(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9c17(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9afe(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9c17(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9afe(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9c17(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9afe(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9c17(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9afe(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9c17(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9afe(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9c17(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9afe(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9c17(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9afe(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9c17(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9afe(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9c17(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fldt   0x9afa(%rip)        
+	fstpt  0x158(%rsp)
+	fldt   0x9c0c(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9b02(%rip)        
+	fldt   0x9c14(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b08(%rip)        
+	fldt   0x9c1a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b0e(%rip)        
+	fldt   0x9c20(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b14(%rip)        
+	fldt   0x9c26(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b1a(%rip)        
+	fldt   0x9c2c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b20(%rip)        
+	fldt   0x9c32(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b26(%rip)        
+	fldt   0x9c38(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b2c(%rip)        
+	fldt   0x9c3e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b32(%rip)        
+	fldt   0x9c44(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b38(%rip)        
+	fldt   0x9c4a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b3e(%rip)        
+	fldt   0x9c50(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b44(%rip)        
+	fldt   0x9c56(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b4a(%rip)        
+	fldt   0x9c5c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x9b4c(%rip)        
+	fldt   0x9c5e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b52(%rip)        
+	fldt   0x9c64(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b58(%rip)        
+	fldt   0x9c6a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b5e(%rip)        
+	fldt   0x9c70(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b64(%rip)        
+	fldt   0x9c76(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9b6c(%rip)        
+	fldt   0x9c7e(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b6e(%rip)        
+	fldt   0x9c80(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b6e(%rip)        
+	fldt   0x9c80(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b6e(%rip)        
+	fldt   0x9c80(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b6e(%rip)        
+	fldt   0x9c80(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b6e(%rip)        
+	fldt   0x9c80(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b6e(%rip)        
+	fldt   0x9c80(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b6e(%rip)        
+	fldt   0x9c80(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b6e(%rip)        
+	fldt   0x9c80(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9b6e(%rip)        
+	fldt   0x9c80(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fstpt  0x178(%rsp)
-	fldt   0x9b63(%rip)        
+	fstpt  0x168(%rsp)
+	fldt   0x9c75(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9b6b(%rip)        
+	fldt   0x9c7d(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b71(%rip)        
+	fldt   0x9c83(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b77(%rip)        
+	fldt   0x9c89(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b7d(%rip)        
+	fldt   0x9c8f(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b83(%rip)        
+	fldt   0x9c95(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b89(%rip)        
+	fldt   0x9c9b(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b8f(%rip)        
+	fldt   0x9ca1(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b95(%rip)        
+	fldt   0x9ca7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9b9b(%rip)        
+	fldt   0x9cad(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ba1(%rip)        
+	fldt   0x9cb3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ba7(%rip)        
+	fldt   0x9cb9(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x9ba9(%rip)        
+	fldt   0x9cbb(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9baf(%rip)        
+	fldt   0x9cc1(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bb5(%rip)        
+	fldt   0x9cc7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bbb(%rip)        
+	fldt   0x9ccd(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bc1(%rip)        
+	fldt   0x9cd3(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bc7(%rip)        
+	fldt   0x9cd9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bcd(%rip)        
+	fldt   0x9cdf(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9bd5(%rip)        
+	fldt   0x9ce7(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9bd7(%rip)        
+	fldt   0x9ce9(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9bd7(%rip)        
+	fldt   0x9ce9(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9bd7(%rip)        
+	fldt   0x9ce9(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9bd7(%rip)        
+	fldt   0x9ce9(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9bd7(%rip)        
+	fldt   0x9ce9(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9bd7(%rip)        
+	fldt   0x9ce9(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9bd7(%rip)        
+	fldt   0x9ce9(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9bd7(%rip)        
+	fldt   0x9ce9(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9bd7(%rip)        
+	fldt   0x9ce9(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fstpt  0x188(%rsp)
-	fldt   0x9bcc(%rip)        
+	fstpt  0x178(%rsp)
+	fldt   0x9cde(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9bd4(%rip)        
+	fldt   0x9ce6(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bda(%rip)        
+	fldt   0x9cec(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9be0(%rip)        
+	fldt   0x9cf2(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9be6(%rip)        
+	fldt   0x9cf8(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bec(%rip)        
+	fldt   0x9cfe(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bf2(%rip)        
+	fldt   0x9d04(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bf8(%rip)        
+	fldt   0x9d0a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bfe(%rip)        
+	fldt   0x9d10(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c04(%rip)        
+	fldt   0x9d16(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c0a(%rip)        
+	fldt   0x9d1c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c10(%rip)        
+	fldt   0x9d22(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c16(%rip)        
+	fldt   0x9d28(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c1c(%rip)        
+	fldt   0x9d2e(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c22(%rip)        
+	fldt   0x9d34(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c28(%rip)        
+	fldt   0x9d3a(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x9c2a(%rip)        
+	fldt   0x9d3c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c30(%rip)        
+	fldt   0x9d42(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c36(%rip)        
+	fldt   0x9d48(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9c3e(%rip)        
+	fldt   0x9d50(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c40(%rip)        
+	fldt   0x9d52(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c40(%rip)        
+	fldt   0x9d52(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c40(%rip)        
+	fldt   0x9d52(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c40(%rip)        
+	fldt   0x9d52(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c40(%rip)        
+	fldt   0x9d52(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c40(%rip)        
+	fldt   0x9d52(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c40(%rip)        
+	fldt   0x9d52(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c40(%rip)        
+	fldt   0x9d52(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c40(%rip)        
+	fldt   0x9d52(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fldt   -0x58(%rsp)
+	fldt   0x68(%rsp)
 	fmulp  %st,%st(1)
 	fldt   0x28(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x118(%rsp)
+	fldt   0xf8(%rsp)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	faddp  %st,%st(1)
-	fxch   %st(1)
-	fld    %st(0)
-	fstpt  0x1c8(%rsp)
-	fldt   0x68(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
+	fldt   0x158(%rsp)
 	fldt   0x78(%rsp)
-	fld    %st(0)
-	fldt   0x178(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
+	faddp  %st,%st(1)
 	fldt   0x88(%rsp)
-	fldt   0x188(%rsp)
+	fldt   0x168(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
-	fxch   %st(1)
+	faddp  %st,%st(1)
+	fld    %st(1)
+	fldt   0x178(%rsp)
+	fmulp  %st,%st(1)
+	faddp  %st,%st(1)
 	fstpt  0x28(%rsp)
-	fldt   0x9bdf(%rip)        
+	fldt   0x9cfb(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9be7(%rip)        
+	fldt   0x9d03(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bed(%rip)        
+	fldt   0x9d09(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bf3(%rip)        
+	fldt   0x9d0f(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bf9(%rip)        
+	fldt   0x9d15(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9bff(%rip)        
+	fldt   0x9d1b(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c05(%rip)        
+	fldt   0x9d21(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c0b(%rip)        
+	fldt   0x9d27(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c11(%rip)        
+	fldt   0x9d2d(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c17(%rip)        
+	fldt   0x9d33(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c1d(%rip)        
+	fldt   0x9d39(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c23(%rip)        
+	fldt   0x9d3f(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x9c25(%rip)        
+	fldt   0x9d41(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c2b(%rip)        
+	fldt   0x9d47(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c31(%rip)        
+	fldt   0x9d4d(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c37(%rip)        
+	fldt   0x9d53(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c3d(%rip)        
+	fldt   0x9d59(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9c45(%rip)        
+	fldt   0x9d61(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c47(%rip)        
+	fldt   0x9d63(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c47(%rip)        
+	fldt   0x9d63(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c47(%rip)        
+	fldt   0x9d63(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c47(%rip)        
+	fldt   0x9d63(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c47(%rip)        
+	fldt   0x9d63(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c47(%rip)        
+	fldt   0x9d63(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c47(%rip)        
+	fldt   0x9d63(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9c47(%rip)        
+	fldt   0x9d63(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fstpt  0x118(%rsp)
-	fldt   0x9c3c(%rip)        
+	fstpt  0xf8(%rsp)
+	fldt   0x9d58(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9c44(%rip)        
+	fldt   0x9d60(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c4a(%rip)        
+	fldt   0x9d66(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c50(%rip)        
+	fldt   0x9d6c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c56(%rip)        
+	fldt   0x9d72(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c5c(%rip)        
+	fldt   0x9d78(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c62(%rip)        
+	fldt   0x9d7e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c68(%rip)        
+	fldt   0x9d84(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c6e(%rip)        
+	fldt   0x9d8a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c74(%rip)        
+	fldt   0x9d90(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x9c76(%rip)        
+	fldt   0x9d92(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c7c(%rip)        
+	fldt   0x9d98(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c82(%rip)        
+	fldt   0x9d9e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c88(%rip)        
+	fldt   0x9da4(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c8e(%rip)        
+	fldt   0x9daa(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c94(%rip)        
+	fldt   0x9db0(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9c9a(%rip)        
+	fldt   0x9db6(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9ca2(%rip)        
+	fldt   0x9dbe(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9ca4(%rip)        
+	fldt   0x9dc0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9ca4(%rip)        
+	fldt   0x9dc0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9ca4(%rip)        
+	fldt   0x9dc0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9ca4(%rip)        
+	fldt   0x9dc0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9ca4(%rip)        
+	fldt   0x9dc0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9ca4(%rip)        
+	fldt   0x9dc0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9ca4(%rip)        
+	fldt   0x9dc0(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9ca4(%rip)        
+	fldt   0x9dc0(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fstpt  0x198(%rsp)
-	fldt   0x9c99(%rip)        
+	fstpt  0x188(%rsp)
+	fldt   0x9db5(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9ca1(%rip)        
+	fldt   0x9dbd(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ca7(%rip)        
+	fldt   0x9dc3(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cad(%rip)        
+	fldt   0x9dc9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cb3(%rip)        
+	fldt   0x9dcf(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cb9(%rip)        
+	fldt   0x9dd5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cbf(%rip)        
+	fldt   0x9ddb(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cc5(%rip)        
+	fldt   0x9de1(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ccb(%rip)        
+	fldt   0x9de7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cd1(%rip)        
+	fldt   0x9ded(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cd7(%rip)        
+	fldt   0x9df3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cdd(%rip)        
+	fldt   0x9df9(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x9cdf(%rip)        
+	fldt   0x9dfb(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ce5(%rip)        
+	fldt   0x9e01(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ceb(%rip)        
+	fldt   0x9e07(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cf1(%rip)        
+	fldt   0x9e0d(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cf7(%rip)        
+	fldt   0x9e13(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9cff(%rip)        
+	fldt   0x9e1b(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d01(%rip)        
+	fldt   0x9e1d(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d01(%rip)        
+	fldt   0x9e1d(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d01(%rip)        
+	fldt   0x9e1d(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d01(%rip)        
+	fldt   0x9e1d(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d01(%rip)        
+	fldt   0x9e1d(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d01(%rip)        
+	fldt   0x9e1d(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d01(%rip)        
+	fldt   0x9e1d(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d01(%rip)        
+	fldt   0x9e1d(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fldt   -0x28(%rsp)
+	fldt   -0x38(%rsp)
 	fmulp  %st,%st(1)
 	fldt   0x38(%rsp)
-	fldt   -0x48(%rsp)
+	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x1a8(%rsp)
-	fldt   -0x38(%rsp)
+	fldt   0xa8(%rsp)
+	fldt   -0x48(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x98(%rsp)
-	fldt   0x118(%rsp)
+	fldt   -0x28(%rsp)
+	fldt   0xf8(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0xa8(%rsp)
-	fldt   0x198(%rsp)
+	fldt   0x98(%rsp)
+	fldt   0x188(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	fstpt  0x38(%rsp)
-	fldt   0x9cb4(%rip)        
+	fldt   0x9dd3(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9cbc(%rip)        
+	fldt   0x9ddb(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cc2(%rip)        
+	fldt   0x9de1(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cc8(%rip)        
+	fldt   0x9de7(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cce(%rip)        
+	fldt   0x9ded(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cd4(%rip)        
+	fldt   0x9df3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cda(%rip)        
+	fldt   0x9df9(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ce0(%rip)        
+	fldt   0x9dff(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ce6(%rip)        
+	fldt   0x9e05(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cec(%rip)        
+	fldt   0x9e0b(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cf2(%rip)        
+	fldt   0x9e11(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9cf8(%rip)        
+	fldt   0x9e17(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x9cfa(%rip)        
+	fldt   0x9e19(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d00(%rip)        
+	fldt   0x9e1f(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d06(%rip)        
+	fldt   0x9e25(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d0c(%rip)        
+	fldt   0x9e2b(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d12(%rip)        
+	fldt   0x9e31(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d18(%rip)        
+	fldt   0x9e37(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d1e(%rip)        
+	fldt   0x9e3d(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9d26(%rip)        
+	fldt   0x9e45(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d28(%rip)        
+	fldt   0x9e47(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d28(%rip)        
+	fldt   0x9e47(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d28(%rip)        
+	fldt   0x9e47(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d28(%rip)        
+	fldt   0x9e47(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d28(%rip)        
+	fldt   0x9e47(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d28(%rip)        
+	fldt   0x9e47(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d28(%rip)        
+	fldt   0x9e47(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d28(%rip)        
+	fldt   0x9e47(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9d28(%rip)        
+	fldt   0x9e47(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fstpt  0x1a8(%rsp)
-	fldt   0x9d1d(%rip)        
+	fstpt  0xa8(%rsp)
+	fldt   0x9e3c(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9d25(%rip)        
+	fldt   0x9e44(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d2b(%rip)        
+	fldt   0x9e4a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d31(%rip)        
+	fldt   0x9e50(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d37(%rip)        
+	fldt   0x9e56(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d3d(%rip)        
+	fldt   0x9e5c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d43(%rip)        
+	fldt   0x9e62(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d49(%rip)        
+	fldt   0x9e68(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d4f(%rip)        
+	fldt   0x9e6e(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d55(%rip)        
+	fldt   0x9e74(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d5b(%rip)        
+	fldt   0x9e7a(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d61(%rip)        
+	fldt   0x9e80(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d67(%rip)        
+	fldt   0x9e86(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d6d(%rip)        
+	fldt   0x9e8c(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d73(%rip)        
+	fldt   0x9e92(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d79(%rip)        
+	fldt   0x9e98(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d7f(%rip)        
+	fldt   0x9e9e(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d85(%rip)        
+	fldt   0x9ea4(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d8b(%rip)        
+	fldt   0x9eaa(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d91(%rip)        
+	fldt   0x9eb0(%rip)        
 	fsubrp %st,%st(1)
 	fldt   0xb8(%rsp)
 	fdivrp %st,%st(1)
-	fstpt  0x1b8(%rsp)
-	fldt   0x9d89(%rip)        
+	fstpt  0x198(%rsp)
+	fldt   0x9ea8(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9d91(%rip)        
+	fldt   0x9eb0(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d97(%rip)        
+	fldt   0x9eb6(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9d9d(%rip)        
+	fldt   0x9ebc(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9da3(%rip)        
+	fldt   0x9ec2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9da9(%rip)        
+	fldt   0x9ec8(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9daf(%rip)        
+	fldt   0x9ece(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9db5(%rip)        
+	fldt   0x9ed4(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9dbb(%rip)        
+	fldt   0x9eda(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9dc1(%rip)        
+	fldt   0x9ee0(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9dc7(%rip)        
+	fldt   0x9ee6(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9dcd(%rip)        
+	fldt   0x9eec(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9dd3(%rip)        
+	fldt   0x9ef2(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9dd9(%rip)        
+	fldt   0x9ef8(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fadd   %st(2),%st
+	fadd   %st(3),%st
 	fmul   %st(4),%st
-	fldt   0x9ddb(%rip)        
+	fldt   0x9efa(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9de1(%rip)        
+	fldt   0x9f00(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9de7(%rip)        
+	fldt   0x9f06(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ded(%rip)        
+	fldt   0x9f0c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9df3(%rip)        
+	fldt   0x9f12(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9dfb(%rip)        
+	fldt   0x9f1a(%rip)        
 	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9dfd(%rip)        
+	fldt   0x9f1c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9dfd(%rip)        
+	fldt   0x9f1c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9dfd(%rip)        
+	fldt   0x9f1c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9dfd(%rip)        
+	fldt   0x9f1c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9dfd(%rip)        
+	fldt   0x9f1c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9dfd(%rip)        
+	fldt   0x9f1c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9dfd(%rip)        
+	fldt   0x9f1c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9dfd(%rip)        
+	fldt   0x9f1c(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	faddp  %st,%st(1)
 	fmul   %st(5),%st
-	fldt   0x9dfd(%rip)        
+	fldt   0x9f1c(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
-	fadd   %st(4),%st
+	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fldt   0x68(%rsp)
+	fldt   0x78(%rsp)
 	fmulp  %st,%st(1)
 	fldt   0x48(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x128(%rsp)
+	fldt   0x108(%rsp)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x1c8(%rsp)
-	fldt   -0x58(%rsp)
+	fldt   0x158(%rsp)
+	fldt   0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x1a8(%rsp)
-	fmulp  %st,%st(2)
-	faddp  %st,%st(1)
 	fldt   0x88(%rsp)
-	fldt   0x1b8(%rsp)
+	fldt   0xa8(%rsp)
+	fmulp  %st,%st(1)
+	faddp  %st,%st(1)
+	fld    %st(1)
+	fldt   0x198(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	fstpt  0x48(%rsp)
-	fldt   0x9da8(%rip)        
-	fmul   %st(3),%st
-	fldt   0x9db0(%rip)        
+	fldt   0x9ec5(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ecd(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9db6(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ed3(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9dbc(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ed9(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9dc2(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9edf(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9dc8(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ee5(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9dce(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9eeb(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9dd4(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ef1(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9dda(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9ef7(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9de0(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9efd(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9de6(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f03(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9dec(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f09(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9df2(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f0f(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9df8(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f15(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9dfe(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f1b(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e04(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f21(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e0a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f27(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e10(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f2d(%rip)        
 	fsubrp %st,%st(1)
 	fldt   0xc8(%rsp)
 	fdivrp %st,%st(1)
-	fstpt  0x128(%rsp)
-	fldt   0x9e08(%rip)        
-	fmul   %st(3),%st
-	fldt   0x9e10(%rip)        
+	fstpt  0x108(%rsp)
+	fldt   0x9f25(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f2d(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e16(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f33(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e1c(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f39(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e22(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f3f(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e28(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f45(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e2e(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f4b(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e34(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f51(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e3a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f57(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e40(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f5d(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fadd   %st(1),%st
-	fmul   %st(3),%st
-	fldt   0x9e42(%rip)        
+	fmul   %st(4),%st
+	fadd   %st(3),%st
+	fmul   %st(4),%st
+	fldt   0x9f5f(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e48(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f65(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e4e(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f6b(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e54(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f71(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e5a(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f77(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e60(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f7d(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e66(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f83(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9e6e(%rip)        
-	fld    %st(4)
+	fldt   0x9f8b(%rip)        
+	fld    %st(5)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9e70(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9f8d(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9e70(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9f8d(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9e70(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9f8d(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9e70(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9f8d(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9e70(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9f8d(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9e70(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9f8d(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9e70(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9f8d(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	fsubp  %st,%st(1)
-	fmul   %st(4),%st
-	fldt   0x9e70(%rip)        
+	fmul   %st(5),%st
+	fldt   0x9f8d(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(5),%st
+	fmul   %st(6),%st
 	faddp  %st,%st(1)
-	fmul   %st(4),%st
+	fmul   %st(5),%st
 	fadd   %st(3),%st
 	fdivrp %st,%st(1)
-	fldt   0x98(%rsp)
+	fldt   -0x28(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0xf8(%rsp)
-	fldt   -0x48(%rsp)
+	fldt   0xe8(%rsp)
+	fldt   -0x58(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x158(%rsp)
-	fldt   -0x38(%rsp)
+	fldt   0x138(%rsp)
+	fldt   -0x48(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x118(%rsp)
-	fldt   -0x28(%rsp)
+	fldt   0xf8(%rsp)
+	fldt   -0x38(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0xa8(%rsp)
-	fldt   0x128(%rsp)
+	fldt   0x98(%rsp)
+	fldt   0x108(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fstpt  0x118(%rsp)
-	fldt   0x9e1d(%rip)        
-	fmul   %st(3),%st
-	fldt   0x9e25(%rip)        
+	fstpt  0xf8(%rsp)
+	fldt   0x9f3d(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f45(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e2b(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f4b(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e31(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f51(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e37(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f57(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e3d(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f5d(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e43(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f63(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e49(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f69(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e4f(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f6f(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e55(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f75(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e5b(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f7b(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e61(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f81(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e67(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f87(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e6d(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f8d(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e73(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f93(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e79(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f99(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e7f(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9f9f(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e85(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9fa5(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e8b(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9fab(%rip)        
 	faddp  %st,%st(1)
-	fmul   %st(3),%st
-	fldt   0x9e91(%rip)        
+	fmul   %st(4),%st
+	fldt   0x9fb1(%rip)        
 	fsubrp %st,%st(1)
 	fldt   0xb8(%rsp)
-	fdivr  %st,%st(1)
-	fxch   %st(1)
-	fstpt  0xf8(%rsp)
-	fldt   0x9e87(%rip)        
+	fdivrp %st,%st(1)
+	fstpt  0xe8(%rsp)
+	fldt   0x9fa9(%rip)        
 	fmul   %st(4),%st
-	fldt   0x9e8f(%rip)        
+	fldt   0x9fb1(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9e95(%rip)        
+	fldt   0x9fb7(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9e9b(%rip)        
+	fldt   0x9fbd(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ea1(%rip)        
+	fldt   0x9fc3(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ea7(%rip)        
+	fldt   0x9fc9(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ead(%rip)        
+	fldt   0x9fcf(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9eb3(%rip)        
+	fldt   0x9fd5(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9eb9(%rip)        
+	fldt   0x9fdb(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ebf(%rip)        
+	fldt   0x9fe1(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ec5(%rip)        
+	fldt   0x9fe7(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ecb(%rip)        
+	fldt   0x9fed(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(4),%st
-	faddp  %st,%st(2)
-	fxch   %st(1)
+	faddp  %st,%st(3)
+	fxch   %st(2)
 	fmul   %st(3),%st
-	fldt   0x9ecb(%rip)        
+	fldt   0x9fed(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9ed1(%rip)        
+	fldt   0x9ff3(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9ed7(%rip)        
+	fldt   0x9ff9(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9edd(%rip)        
+	fldt   0x9fff(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9ee3(%rip)        
+	fldt   0xa005(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9ee9(%rip)        
+	fldt   0xa00b(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9eef(%rip)        
+	fldt   0xa011(%rip)        
 	fsubrp %st,%st(1)
-	fldt   0x9ef7(%rip)        
+	fldt   0xa019(%rip)        
 	fld    %st(4)
 	fmul   %st(1),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ef9(%rip)        
+	fldt   0xa01b(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ef9(%rip)        
+	fldt   0xa01b(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ef9(%rip)        
+	fldt   0xa01b(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ef9(%rip)        
+	fldt   0xa01b(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ef9(%rip)        
+	fldt   0xa01b(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ef9(%rip)        
+	fldt   0xa01b(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ef9(%rip)        
+	fldt   0xa01b(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ef9(%rip)        
+	fldt   0xa01b(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
-	fldt   0x9ef9(%rip)        
+	fldt   0xa01b(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
 	fsubp  %st,%st(1)
 	fmul   %st(4),%st
-	faddp  %st,%st(3)
-	fdivp  %st,%st(2)
-	fldt   0x78(%rsp)
-	fmulp  %st,%st(2)
+	faddp  %st,%st(2)
+	fdivp  %st,%st(1)
+	fldt   0x88(%rsp)
+	fmulp  %st,%st(1)
 	fldt   0xd8(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x138(%rsp)
+	fldt   0x118(%rsp)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x178(%rsp)
-	fldt   -0x58(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x1a8(%rsp)
+	fldt   0x168(%rsp)
 	fldt   0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	faddp  %st,%st(2)
-	fldt   0x88(%rsp)
-	fldt   0xf8(%rsp)
+	fldt   0xa8(%rsp)
+	fldt   0x78(%rsp)
 	fmulp  %st,%st(1)
-	faddp  %st,%st(2)
+	faddp  %st,%st(1)
+	faddp  %st,%st(1)
 	fxch   %st(1)
-	fstpt  0xb8(%rsp)
-	fldt   0x6b38(%rip)        
+	fld    %st(0)
+	fstpt  0xa8(%rsp)
+	fldt   0xe8(%rsp)
+	fmulp  %st,%st(1)
+	faddp  %st,%st(1)
+	fldt   0x6c5c(%rip)        
 	fld    %st(2)
 	fmul   %st(1),%st
-	fldt   0x6b3e(%rip)        
+	fldt   0x6c62(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x6b44(%rip)        
+	fldt   0x6c68(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x6b4a(%rip)        
+	fldt   0x6c6e(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x6b50(%rip)        
+	fldt   0x6c74(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(4),%st
-	fldt   0x6b54(%rip)        
+	fldt   0x6c78(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
-	fldt   0x6b58(%rip)        
-	fadd   %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(6),%st
-	fldt   0x6b5c(%rip)        
+	fldt   0x6c7c(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x6c82(%rip)        
 	fsubrp %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x6b62(%rip)        
+	fmul   %st(5),%st
+	fldt   0x6c88(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	fsubp  %st,%st(1)
-	fmul   %st(6),%st
-	fldt   0x6b42(%rip)        
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
 	fsubp  %st,%st(1)
 	fmul   %st(5),%st
+	fldt   0x6c68(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x6c4e(%rip)        
+	fsubrp %st,%st(1)
+	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
 	fsubp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x6aec(%rip)        
+	fldt   0x6c0c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x6ad2(%rip)        
+	fldt   0x6bf2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x6ab8(%rip)        
+	fldt   0x6bd8(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
 	fsubp  %st,%st(1)
 	fldt   0xc8(%rsp)
 	fdivrp %st,%st(1)
-	fldt   0xa8(%rsp)
+	fldt   0x98(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x108(%rsp)
+	fldt   0x1b8(%rsp)
+	fldt   -0x58(%rsp)
+	fmulp  %st,%st(1)
+	fldt   0x148(%rsp)
 	fldt   -0x48(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x168(%rsp)
+	faddp  %st,%st(1)
+	fldt   0x188(%rsp)
 	fldt   -0x38(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x198(%rsp)
 	fldt   -0x28(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x98(%rsp)
-	fldt   0x128(%rsp)
+	fldt   0x108(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x9dab(%rip)        
+	fldt   0x9ece(%rip)        
 	fmul   %st(3),%st
-	fldt   0x9db3(%rip)        
+	fldt   0x9ed6(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9db9(%rip)        
+	fldt   0x9edc(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9dbf(%rip)        
+	fldt   0x9ee2(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9dc5(%rip)        
+	fldt   0x9ee8(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9dcb(%rip)        
+	fldt   0x9eee(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9dd1(%rip)        
+	fldt   0x9ef4(%rip)        
 	fadd   %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(4),%st
-	fldt   0x9dd5(%rip)        
+	fldt   0x9ef8(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
 	fmul   %st(5),%st
-	fldt   0x9dd9(%rip)        
-	fadd   %st,%st(1)
-	fxch   %st(1)
-	fmul   %st(6),%st
-	fldt   0x9ddd(%rip)        
+	fldt   0x9efc(%rip)        
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9f02(%rip)        
 	fsubr  %st,%st(1)
 	fxch   %st(1)
-	fmul   %st(7),%st
-	faddp  %st,%st(1)
 	fmul   %st(6),%st
-	fsubp  %st,%st(1)
+	faddp  %st,%st(1)
+	fmul   %st(5),%st
+	fldt   0x9ee2(%rip)        
+	fsubrp %st,%st(1)
 	fmul   %st(5),%st
 	faddp  %st,%st(1)
 	fmul   %st(4),%st
 	fsubp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9d81(%rip)        
+	fldt   0x9ea0(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9d67(%rip)        
+	fldt   0x9e86(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9d4d(%rip)        
+	fldt   0x9e6c(%rip)        
 	faddp  %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9d33(%rip)        
+	fldt   0x9e52(%rip)        
 	fsubrp %st,%st(1)
 	fmul   %st(3),%st
-	fldt   0x9d19(%rip)        
+	fldt   0x9e38(%rip)        
 	faddp  %st,%st(1)
 	fmulp  %st,%st(3)
-	fldt   0x9cff(%rip)        
+	fldt   0x9e1e(%rip)        
 	fsubrp %st,%st(3)
-	fxch   %st(2)
-	fdivp  %st,%st(1)
-	fldt   0x88(%rsp)
-	fmulp  %st,%st(1)
-	fldt   0xe8(%rsp)
+	fldt   0xb8(%rsp)
+	fdivrp %st,%st(3)
+	fldt   0xa8(%rsp)
+	fmulp  %st,%st(3)
+	fldt   0x1a8(%rsp)
 	fldt   -0x78(%rsp)
 	fmulp  %st,%st(1)
-	fldt   0x148(%rsp)
+	fldt   0x128(%rsp)
 	fldt   -0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
-	fldt   0x188(%rsp)
-	fldt   -0x58(%rsp)
-	fmulp  %st,%st(1)
-	faddp  %st,%st(1)
-	fldt   0x1b8(%rsp)
+	fldt   0x178(%rsp)
 	fldt   0x68(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
+	fldt   0x198(%rsp)
 	fldt   0x78(%rsp)
-	fldt   0xf8(%rsp)
 	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
+	fldt   0x88(%rsp)
+	fldt   0xe8(%rsp)
+	fmulp  %st,%st(1)
 	faddp  %st,%st(1)
+	faddp  %st,%st(3)
 	test   %esi,%esi
-	jle    b91e <polyreg10+0x2dbe>
+	jle    b807 <polyreg10+0x2da7>
 	fldt   0x58(%rsp)
 	movslq %esi,%rsi
 	xor    %eax,%eax
-	fldt   0x118(%rsp)
-	fldt   0xb8(%rsp)
-	nopw   0x0(%rax,%rax,1)
+	fldt   0xf8(%rsp)
+	nopl   0x0(%rax,%rax,1)
 	mov    %eax,-0x78(%rsp)
 	fildl  -0x78(%rsp)
-	fmul   %st(3),%st
+	fmul   %st(2),%st
 	fld1
 	fsubrp %st,%st(1)
-	fld    %st(4)
+	fld    %st(5)
 	fmul   %st(1),%st
-	fadd   %st(6),%st
+	fadd   %st(4),%st
 	fmul   %st(1),%st
-	fadd   %st(2),%st
+	fadd   %st(5),%st
 	fmul   %st(1),%st
-	fadd   %st(3),%st
+	fadd   %st(2),%st
 	fmul   %st(1),%st
 	fldt   0x48(%rsp)
 	faddp  %st,%st(1)
 	fmul   %st(1),%st
 	fldt   0x38(%rsp)
 	faddp  %st,%st(1)
 	fmul   %st(1),%st
@@ -14248,18 +14242,17 @@
 	fmulp  %st,%st(1)
 	fldt   -0x18(%rsp)
 	faddp  %st,%st(1)
 	fsubrl (%rdi,%rax,8)
 	fstpl  (%rdx,%rax,8)
 	add    $0x1,%rax
 	cmp    %rax,%rsi
-	jne    b8b0 <polyreg10+0x2d50>
-	fstp   %st(2)
+	jne    b7a0 <polyreg10+0x2d40>
+	fstp   %st(0)
 	fstp   %st(0)
-	fstpt  0xb8(%rsp)
 	fldt   -0x18(%rsp)
 	fstpl  -0x78(%rsp)
 	fldt   -0x8(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	fldt   0x8(%rsp)
 	movhpd -0x78(%rsp),%xmm0
@@ -14275,91 +14268,88 @@
 	fldt   0x38(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	fldt   0x48(%rsp)
 	movhpd -0x78(%rsp),%xmm0
 	movups %xmm0,0x20(%rcx)
 	fstpl  -0x78(%rsp)
-	fldt   0x118(%rsp)
+	fldt   0xf8(%rsp)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
-	fldt   0xb8(%rsp)
+	fxch   %st(1)
 	movhpd -0x78(%rsp),%xmm0
-	movups %xmm0,0x30(%rcx)
 	fstpl  -0x78(%rsp)
-	fxch   %st(1)
+	movups %xmm0,0x30(%rcx)
 	movsd  -0x78(%rsp),%xmm0
 	fstpl  -0x78(%rsp)
 	movhpd -0x78(%rsp),%xmm0
-	fstpl  0x50(%rcx)
 	movups %xmm0,0x40(%rcx)
-	add    $0x1e0,%rsp
+	fstpl  0x50(%rcx)
+	add    $0x1d0,%rsp
 	ret
-	nopl   0x0(%rax)
+	xchg   %ax,%ax
 	fldz
-	fstpt  0x88(%rsp)
-	fldt   0x88(%rsp)
 	fstpt  0xa8(%rsp)
 	fldt   0xa8(%rsp)
-	fstpt  0x78(%rsp)
-	fldt   0x78(%rsp)
 	fstpt  0x98(%rsp)
 	fldt   0x98(%rsp)
-	fstpt  0x68(%rsp)
-	fldt   0x68(%rsp)
+	fstpt  0x88(%rsp)
+	fldt   0x88(%rsp)
 	fstpt  -0x28(%rsp)
 	fldt   -0x28(%rsp)
-	fstpt  -0x58(%rsp)
-	fldt   -0x58(%rsp)
+	fstpt  0x78(%rsp)
+	fldt   0x78(%rsp)
 	fstpt  -0x38(%rsp)
 	fldt   -0x38(%rsp)
-	fstpt  -0x68(%rsp)
-	fldt   -0x68(%rsp)
+	fstpt  0x68(%rsp)
+	fldt   0x68(%rsp)
 	fstpt  -0x48(%rsp)
 	fldt   -0x48(%rsp)
+	fstpt  -0x68(%rsp)
+	fldt   -0x68(%rsp)
+	fstpt  -0x58(%rsp)
+	fldt   -0x58(%rsp)
 	fstpt  -0x78(%rsp)
-	fldt   -0x78(%rsp)
-	jmp    8c7f <polyreg10+0x11f>
-	data16 cs nopw 0x0(%rax,%rax,1)
-	nopl   0x0(%rax)
+	jmp    8b6f <polyreg10+0x10f>
+	nopl   (%rax)
 
-000000000000ba50 <myround>:
+000000000000b920 <myround>:
 myround():
-	addsd  0x9b98(%rip),%xmm0        
-	movsd  0x9b70(%rip),%xmm2        
-	movsd  0x9b90(%rip),%xmm3        
+	addsd  0x9cc8(%rip),%xmm0        
+	movsd  0x9cd8(%rip),%xmm2        
+	movsd  0x9cc0(%rip),%xmm3        
 	movapd %xmm0,%xmm1
 	andpd  %xmm2,%xmm1
 	ucomisd %xmm1,%xmm3
-	jbe    baa9 <myround+0x59>
+	jbe    b979 <myround+0x59>
 	cvttsd2si %xmm0,%rax
 	pxor   %xmm1,%xmm1
-	movsd  0x9b79(%rip),%xmm4        
+	movsd  0x9ca9(%rip),%xmm4        
 	andnpd %xmm0,%xmm2
 	cvtsi2sd %rax,%xmm1
 	movapd %xmm1,%xmm3
 	cmpnlesd %xmm0,%xmm3
 	andpd  %xmm4,%xmm3
 	subsd  %xmm3,%xmm1
 	orpd   %xmm2,%xmm1
 	movapd %xmm1,%xmm0
 	cvttsd2si %xmm0,%eax
 	ret
 	xchg   %ax,%ax
 
-000000000000bab0 <detrend>:
+000000000000b980 <detrend>:
 detrend():
 	add    $0x1,%edi
 	mov    %rsi,%r9
 	mov    %rcx,%r10
 	mov    %edx,%esi
 	mov    %r8,%rcx
 	cmp    $0xb,%edi
-	ja     bba3 <detrend+0xf3>
-	lea    0x1532(%rip),%rdx        
+	ja     ba73 <detrend+0xf3>
+	lea    0x1662(%rip),%rdx        
 	movslq (%rdx,%rdi,4),%rax
 	add    %rdx,%rax
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
 	mov    %r10,%rdx
 	mov    %r9,%rdi
 	jmp    10d0 <polyreg9@plt>
@@ -14409,372 +14399,331 @@
 	mov    %r10,%rdx
 	mov    %r9,%rdi
 	jmp    1050 <polyreg8@plt>
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nop
 
-000000000000bbb0 <dft>:
+000000000000ba80 <dft>:
 dft():
 	push   %r15
 	pxor   %xmm2,%xmm2
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
-	sub    $0xb8,%rsp
-	movsd  0x9a33(%rip),%xmm1        
-	divsd  0x9a3b(%rip),%xmm0        
-	movzbl 0x120(%rsp),%eax
-	mov    %rdi,0x88(%rsp)
+	sub    $0xa8,%rsp
+	movsd  0x9b63(%rip),%xmm1        
+	divsd  0x9b6b(%rip),%xmm0        
+	movzbl 0x110(%rsp),%eax
+	mov    %rdi,0x78(%rsp)
 	movapd %xmm1,%xmm3
-	mov    %rsi,0x90(%rsp)
-	mov    0x108(%rsp),%r14
+	mov    %rsi,0x80(%rsp)
+	mov    0xf8(%rsp),%r13
 	subsd  %xmm0,%xmm3
 	movapd %xmm1,%xmm0
 	mov    %al,0x4f(%rsp)
-	mov    0xf8(%rsp),%rax
-	sub    0x100(%rsp),%rax
-	mov    %r8,0xa8(%rsp)
+	mov    0xe8(%rsp),%rax
+	sub    0xf0(%rsp),%rax
+	mov    %rdx,0x88(%rsp)
 	cvtsi2sd %rax,%xmm2
-	mov    %rdx,0x98(%rsp)
-	mov    0x110(%rsp),%r15
+	mov    %rcx,0x90(%rsp)
+	mov    0x100(%rsp),%r14
 	divsd  %xmm3,%xmm0
 	pxor   %xmm3,%xmm3
 	mov    %r9,0x40(%rsp)
-	cvtsi2sdq 0x100(%rsp),%xmm3
-	mov    %rcx,0xa0(%rsp)
-	movsd  %xmm2,0x8(%rsp)
+	cvtsi2sdq 0xf0(%rsp),%xmm3
+	mov    %r8,0x98(%rsp)
+	movsd  %xmm2,(%rsp)
 	mulsd  %xmm2,%xmm0
 	divsd  %xmm3,%xmm0
 	addsd  %xmm1,%xmm0
 	call   1100 <myround@plt>
-	mov    0x118(%rsp),%esi
+	mov    0x9ac5(%rip),%rsi        
 	movslq %eax,%rdi
+	mov    %rdi,0x28(%rsp)
+	mov    %rsi,0x38(%rsp)
 	cmp    $0x1,%eax
-	mov    0x9984(%rip),%rax        
-	lea    0x1(%rsi),%r8d
-	mov    %rdi,0x20(%rsp)
-	movslq %r8d,%r8
-	je     c182 <dft+0x5d2>
-	lea    -0x1(%rdi),%rbx
+	je     bb72 <dft+0xf2>
+	lea    -0x1(%rdi),%rax
 	pxor   %xmm0,%xmm0
-	movsd  0x8(%rsp),%xmm2
-	movq   %rax,%xmm1
-	cvtsi2sd %rbx,%xmm0
-	mov    $0x8,%esi
-	mov    %r8,0x18(%rsp)
-	mov    0x100(%rsp),%rdi
-	movapd %xmm2,%xmm5
-	divsd  %xmm0,%xmm5
-	maxsd  %xmm5,%xmm1
+	movsd  (%rsp),%xmm2
+	movq   %rsi,%xmm1
+	cvtsi2sd %rax,%xmm0
+	divsd  %xmm0,%xmm2
+	maxsd  %xmm2,%xmm1
 	movsd  %xmm1,0x38(%rsp)
+	mov    0xf0(%rsp),%rdi
+	mov    $0x8,%esi
 	call   1060 <calloc@plt>
-	mov    0x18(%rsp),%r8
 	mov    $0x8,%esi
-	mov    %rax,0x10(%rsp)
-	mov    %rax,%rbp
-	mov    %r8,%rdi
-	mov    %r8,0x8(%rsp)
+	mov    %rax,%rbx
+	mov    0x108(%rsp),%eax
+	lea    0x1(%rax),%r12d
+	movslq %r12d,%r12
+	mov    %r12,%rdi
 	call   1060 <calloc@plt>
-	mov    0x100(%rsp),%rdi
+	mov    0xf0(%rsp),%rdi
 	mov    $0x8,%esi
 	mov    %rax,0x30(%rsp)
-	mov    %rax,%r13
 	call   1060 <calloc@plt>
-	mov    0x8(%rsp),%r8
 	mov    $0x8,%esi
-	mov    %rax,0x18(%rsp)
-	mov    %rax,%r12
-	mov    %r8,%rdi
+	mov    %r12,%rdi
+	mov    %rax,%rbp
 	call   1060 <calloc@plt>
-	cmpq   $0x0,0x20(%rsp)
-	mov    0x10(%rsp),%r11
-	mov    %rax,0x68(%rsp)
-	jle    c233 <dft+0x683>
-	mov    0x100(%rsp),%rax
-	mov    0x100(%rsp),%r11
-	pxor   %xmm5,%xmm5
-	xor    %ebx,%ebx
-	movsd  %xmm5,0x60(%rsp)
+	cmpq   $0x0,0x28(%rsp)
+	mov    %rax,0x58(%rsp)
+	jle    c039 <dft+0x5b9>
+	mov    0xf0(%rsp),%rax
+	xor    %r12d,%r12d
+	mov    0xf0(%rsp),%r15
+	movq   $0x0,0x8(%rsp)
+	movq   $0x0,0x10(%rsp)
 	shl    $0x3,%rax
-	shr    $1,%r11
-	movsd  %xmm5,0x58(%rsp)
-	mov    %rax,0x80(%rsp)
-	mov    0x100(%rsp),%eax
-	shl    $0x4,%r11
-	mov    %r11,%r13
-	movsd  %xmm5,0x18(%rsp)
-	mov    %eax,0x48(%rsp)
-	mov    0x100(%rsp),%rax
-	movsd  %xmm5,0x10(%rsp)
+	movq   $0x0,(%rsp)
+	shr    $1,%r15
+	mov    %rax,0x70(%rsp)
+	mov    0xf0(%rsp),%eax
+	shl    $0x4,%r15
+	mov    %eax,0x18(%rsp)
+	mov    0xf0(%rsp),%rax
 	and    $0xfffffffffffffffe,%rax
-	movsd  %xmm5,0x8(%rsp)
 	mov    %rax,0x50(%rsp)
 	shl    $0x3,%rax
-	lea    (%r14,%rax,1),%rdi
-	add    %r15,%rax
-	mov    %rdi,0x78(%rsp)
-	mov    %rax,0x70(%rsp)
-	nopl   0x0(%rax,%rax,1)
-	movsd  0x8(%rsp),%xmm0
+	lea    0x0(%r13,%rax,1),%rdi
+	add    %r14,%rax
+	mov    %rdi,0x68(%rsp)
+	mov    %rax,0x60(%rsp)
+	nopl   0x0(%rax)
+	movsd  (%rsp),%xmm0
 	call   1100 <myround@plt>
 	mov    0x40(%rsp),%rdi
-	mov    0x48(%rsp),%edx
-	mov    %rbp,%rcx
+	mov    0x18(%rsp),%edx
+	mov    %rbx,%rcx
 	cltq
-	movsd  0x8(%rsp),%xmm5
+	movsd  (%rsp),%xmm5
 	addsd  0x38(%rsp),%xmm5
 	shl    $0x3,%rax
 	mov    0x30(%rsp),%r8
 	lea    (%rdi,%rax,1),%rsi
-	mov    0x118(%rsp),%edi
-	mov    %rax,0x28(%rsp)
-	movsd  %xmm5,0x8(%rsp)
+	mov    0x108(%rsp),%edi
+	mov    %rax,0x20(%rsp)
+	movsd  %xmm5,(%rsp)
 	call   10c0 <detrend@plt>
 	cmpb   $0x0,0x4f(%rsp)
-	je     c0c0 <dft+0x510>
-	mov    0x28(%rsp),%rax
-	mov    0x68(%rsp),%r8
-	mov    %r12,%rcx
-	add    0xf0(%rsp),%rax
-	mov    0x48(%rsp),%edx
-	mov    0x118(%rsp),%edi
+	je     bf30 <dft+0x4b0>
+	mov    0x20(%rsp),%rax
+	mov    0x58(%rsp),%r8
+	mov    %rbp,%rcx
+	add    0xe0(%rsp),%rax
+	mov    0x18(%rsp),%edx
+	mov    0x108(%rsp),%edi
 	mov    %rax,%rsi
 	call   10c0 <detrend@plt>
-	pxor   %xmm5,%xmm5
-	cmpq   $0x0,0x100(%rsp)
-	jle    c0e6 <dft+0x536>
-	cmpq   $0x1,0x100(%rsp)
-	je     c164 <dft+0x5b4>
-	movapd %xmm5,%xmm2
-	movapd %xmm5,%xmm8
-	movapd %xmm5,%xmm1
+	cmpq   $0x0,0xf0(%rsp)
+	jle    bf4f <dft+0x4cf>
+	cmpq   $0x1,0xf0(%rsp)
+	je     bfc7 <dft+0x547>
+	pxor   %xmm2,%xmm2
 	xor    %eax,%eax
-	movapd %xmm5,%xmm0
+	movapd %xmm2,%xmm5
+	movapd %xmm2,%xmm1
+	movapd %xmm2,%xmm0
 	nopl   0x0(%rax)
-	movupd 0x0(%rbp,%rax,1),%xmm7
-	movupd (%r14,%rax,1),%xmm3
-	movupd (%r15,%rax,1),%xmm4
-	movupd (%r15,%rax,1),%xmm6
+	movupd (%rbx,%rax,1),%xmm7
+	movupd 0x0(%r13,%rax,1),%xmm3
 	mulpd  %xmm7,%xmm3
-	mulpd  %xmm7,%xmm4
-	movupd (%r14,%rax,1),%xmm7
 	addsd  %xmm3,%xmm0
 	unpckhpd %xmm3,%xmm3
-	addsd  %xmm4,%xmm1
-	unpckhpd %xmm4,%xmm4
 	addsd  %xmm3,%xmm0
-	movupd (%r12,%rax,1),%xmm3
-	addsd  %xmm4,%xmm1
+	movupd (%r14,%rax,1),%xmm3
 	mulpd  %xmm7,%xmm3
-	addsd  %xmm3,%xmm8
+	movupd 0x0(%r13,%rax,1),%xmm7
+	addsd  %xmm3,%xmm1
 	unpckhpd %xmm3,%xmm3
-	addsd  %xmm3,%xmm8
-	movupd (%r12,%rax,1),%xmm3
+	addsd  %xmm3,%xmm1
+	movupd 0x0(%rbp,%rax,1),%xmm3
+	mulpd  %xmm7,%xmm3
+	movupd 0x0(%rbp,%rax,1),%xmm7
+	addsd  %xmm3,%xmm5
+	unpckhpd %xmm3,%xmm3
+	addsd  %xmm3,%xmm5
+	movupd (%r14,%rax,1),%xmm3
 	add    $0x10,%rax
-	mulpd  %xmm6,%xmm3
+	mulpd  %xmm7,%xmm3
 	addsd  %xmm3,%xmm2
 	unpckhpd %xmm3,%xmm3
 	addsd  %xmm3,%xmm2
-	cmp    %rax,%r13
-	jne    be70 <dft+0x2c0>
+	cmp    %rax,%r15
+	jne    bd00 <dft+0x280>
 	mov    0x50(%rsp),%rax
-	cmp    0x100(%rsp),%rax
-	je     bf37 <dft+0x387>
-	mov    0x70(%rsp),%rdx
-	mov    0x78(%rsp),%rcx
-	movsd  (%rcx),%xmm6
-	movsd  0x0(%rbp,%rax,8),%xmm7
-	movsd  (%r12,%rax,8),%xmm4
-	movapd %xmm6,%xmm3
-	mulsd  %xmm7,%xmm3
-	mulsd  %xmm4,%xmm6
-	addsd  %xmm3,%xmm0
-	movsd  (%rdx),%xmm3
-	addsd  %xmm6,%xmm8
-	mulsd  %xmm3,%xmm7
+	cmp    %rax,0xf0(%rsp)
+	je     bdc4 <dft+0x344>
+	mov    0x60(%rsp),%rdx
+	mov    0x68(%rsp),%rcx
+	movsd  (%rcx),%xmm4
+	movsd  (%rbx,%rax,8),%xmm3
+	movapd %xmm4,%xmm6
+	mulsd  %xmm3,%xmm6
+	addsd  %xmm6,%xmm0
+	movsd  (%rdx),%xmm6
+	mulsd  %xmm6,%xmm3
+	addsd  %xmm3,%xmm1
+	movsd  0x0(%rbp,%rax,8),%xmm3
 	mulsd  %xmm3,%xmm4
-	addsd  %xmm7,%xmm1
-	addsd  %xmm4,%xmm2
-	movapd %xmm8,%xmm3
-	movapd %xmm8,%xmm6
+	mulsd  %xmm6,%xmm3
+	addsd  %xmm4,%xmm5
+	addsd  %xmm3,%xmm2
+	movapd %xmm5,%xmm3
+	movapd %xmm5,%xmm6
 	movapd %xmm2,%xmm4
 	mulsd  %xmm0,%xmm3
-	xorpd  0x968f(%rip),%xmm4        
+	xorpd  0x9804(%rip),%xmm4        
 	mulsd  %xmm1,%xmm6
-	test   %rbx,%rbx
-	je     c118 <dft+0x568>
+	test   %r12,%r12
+	je     bf80 <dft+0x500>
 	mulsd  %xmm4,%xmm1
-	movapd %xmm3,%xmm2
-	movsd  0x10(%rsp),%xmm9
-	movsd  0x18(%rsp),%xmm10
+	movsd  0x10(%rsp),%xmm7
+	pxor   %xmm2,%xmm2
+	cvtsi2sd %r12,%xmm2
 	mulsd  %xmm4,%xmm0
-	subsd  %xmm1,%xmm2
-	pxor   %xmm1,%xmm1
-	cvtsi2sd %rbx,%xmm1
+	add    $0x1,%r12
+	subsd  %xmm1,%xmm3
 	addsd  %xmm6,%xmm0
-	add    $0x1,%rbx
-	movapd %xmm2,%xmm4
-	subsd  %xmm9,%xmm4
-	movapd %xmm0,%xmm3
-	subsd  %xmm10,%xmm3
-	movapd %xmm4,%xmm6
-	divsd  %xmm1,%xmm6
-	movapd %xmm6,%xmm7
-	movapd %xmm3,%xmm6
-	divsd  %xmm1,%xmm6
-	addsd  %xmm9,%xmm7
-	movapd %xmm2,%xmm1
-	movapd %xmm3,%xmm2
+	movsd  0x8(%rsp),%xmm6
+	movapd %xmm3,%xmm1
 	subsd  %xmm7,%xmm1
-	movsd  %xmm7,0x10(%rsp)
-	addsd  %xmm10,%xmm6
-	subsd  %xmm6,%xmm0
-	movsd  %xmm6,0x18(%rsp)
-	movapd %xmm4,%xmm6
-	mulsd  %xmm1,%xmm6
-	mulsd  %xmm3,%xmm1
-	mulsd  %xmm0,%xmm2
-	mulsd  %xmm4,%xmm0
-	subsd  %xmm2,%xmm6
-	addsd  %xmm1,%xmm0
-	movsd  %xmm6,0x58(%rsp)
-	movsd  %xmm0,0x60(%rsp)
-	cmp    %rbx,0x20(%rsp)
-	jg     bdb8 <dft+0x208>
-	mov    %rbp,%rdi
+	movapd %xmm0,%xmm4
+	subsd  %xmm6,%xmm4
+	movapd %xmm1,%xmm5
+	divsd  %xmm2,%xmm5
+	addsd  %xmm7,%xmm5
+	movsd  %xmm5,0x10(%rsp)
+	movapd %xmm4,%xmm5
+	divsd  %xmm2,%xmm5
+	addsd  %xmm6,%xmm5
+	movsd  %xmm5,0x8(%rsp)
+	cmp    %r12,0x28(%rsp)
+	jne    bc50 <dft+0x1d0>
+	subsd  0x10(%rsp),%xmm3
+	movapd %xmm1,%xmm2
+	movapd %xmm4,%xmm5
+	mov    %rbx,%rdi
+	subsd  0x8(%rsp),%xmm0
+	mulsd  %xmm3,%xmm2
+	mulsd  %xmm0,%xmm5
+	mulsd  %xmm0,%xmm1
+	mulsd  %xmm3,%xmm4
+	subsd  %xmm5,%xmm2
+	addsd  %xmm4,%xmm1
+	movsd  %xmm2,0x18(%rsp)
+	movsd  %xmm1,(%rsp)
 	call   1030 <free@plt>
-	mov    %r12,%rdi
+	mov    %rbp,%rdi
 	call   1030 <free@plt>
 	mov    0x30(%rsp),%rdi
 	call   1030 <free@plt>
-	mov    0x68(%rsp),%rdi
+	mov    0x58(%rsp),%rdi
 	call   1030 <free@plt>
+	movsd  (%rsp),%xmm1
+	movsd  0x18(%rsp),%xmm2
+	mov    0x28(%rsp),%rax
+	pxor   %xmm3,%xmm3
+	sub    $0x1,%rax
+	cvtsi2sd %rax,%xmm3
+	divsd  %xmm3,%xmm2
+	divsd  %xmm3,%xmm1
+	mov    0x78(%rsp),%rax
+	movsd  0x10(%rsp),%xmm0
+	mov    0x28(%rsp),%rsi
+	movsd  %xmm0,(%rax)
+	mov    0x80(%rsp),%rax
+	movsd  0x8(%rsp),%xmm0
+	movsd  %xmm0,(%rax)
 	mov    0x88(%rsp),%rax
-	movsd  0x10(%rsp),%xmm5
-	movsd  %xmm5,(%rax)
+	movsd  %xmm2,(%rax)
 	mov    0x90(%rsp),%rax
-	movsd  0x18(%rsp),%xmm5
-	movsd  %xmm5,(%rax)
-	mov    0x20(%rsp),%rax
-	lea    -0x1(%rax),%rbx
-	cmp    $0x1,%rax
-	je     c1f0 <dft+0x640>
-	pxor   %xmm0,%xmm0
-	movsd  0x58(%rsp),%xmm1
-	mov    0x98(%rsp),%rax
-	cvtsi2sd %rbx,%xmm0
-	divsd  %xmm0,%xmm1
-	movsd  %xmm1,(%rax)
-	movsd  0x60(%rsp),%xmm1
-	mov    0xa0(%rsp),%rax
-	divsd  %xmm0,%xmm1
 	movsd  %xmm1,(%rax)
-	mov    0xa8(%rsp),%rax
-	mov    0x20(%rsp),%rsi
+	mov    0x98(%rsp),%rax
 	mov    %rsi,(%rax)
-	add    $0xb8,%rsp
+	add    $0xa8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
-	xchg   %ax,%ax
-	mov    0x80(%rsp),%rdx
-	mov    %rbp,%rsi
-	mov    %r12,%rdi
+	nopl   0x0(%rax)
+	mov    0x70(%rsp),%rdx
+	mov    %rbx,%rsi
+	mov    %rbp,%rdi
 	call   10a0 <memcpy@plt>
-	pxor   %xmm5,%xmm5
-	cmpq   $0x0,0x100(%rsp)
-	jg     be47 <dft+0x297>
-	mov    0x951b(%rip),%rax        
-	movapd %xmm5,%xmm6
-	movapd %xmm5,%xmm3
-	movapd %xmm5,%xmm2
-	movapd %xmm5,%xmm8
-	movapd %xmm5,%xmm1
-	movapd %xmm5,%xmm0
+	cmpq   $0x0,0xf0(%rsp)
+	jg     bcd8 <dft+0x258>
+	mov    0x127a(%rip),%rax        
+	pxor   %xmm6,%xmm6
+	movapd %xmm6,%xmm3
+	movapd %xmm6,%xmm2
+	movapd %xmm6,%xmm5
 	movq   %rax,%xmm4
-	test   %rbx,%rbx
-	jne    bf5e <dft+0x3ae>
+	movapd %xmm6,%xmm1
+	movapd %xmm6,%xmm0
+	test   %r12,%r12
+	jne    bde9 <dft+0x369>
 	nopl   0x0(%rax)
-	xorpd  0x94c0(%rip),%xmm2        
-	movapd %xmm8,%xmm4
-	cmpq   $0x1,0x20(%rsp)
-	mulsd  %xmm0,%xmm4
+	xorpd  0x9658(%rip),%xmm2        
+	movapd %xmm0,%xmm4
+	cmpq   $0x1,0x28(%rsp)
+	mulsd  %xmm5,%xmm4
+	mulsd  %xmm1,%xmm5
 	movapd %xmm2,%xmm3
 	mulsd  %xmm1,%xmm3
 	mulsd  %xmm0,%xmm2
-	mulsd  %xmm8,%xmm1
 	subsd  %xmm3,%xmm4
-	addsd  %xmm1,%xmm2
+	addsd  %xmm5,%xmm2
 	movsd  %xmm4,0x10(%rsp)
-	movsd  %xmm2,0x18(%rsp)
-	jle    c00c <dft+0x45c>
-	mov    $0x1,%ebx
-	jmp    bdb8 <dft+0x208>
-	mov    %r15,%rdx
-	mov    %r14,%rcx
-	movapd %xmm5,%xmm2
+	movsd  %xmm2,0x8(%rsp)
+	je     bfe4 <dft+0x564>
+	mov    $0x1,%r12d
+	jmp    bc50 <dft+0x1d0>
+	pxor   %xmm2,%xmm2
+	mov    %r14,%rdx
+	mov    %r13,%rcx
 	xor    %eax,%eax
-	movapd %xmm5,%xmm8
-	movapd %xmm5,%xmm1
-	movapd %xmm5,%xmm0
-	jmp    befe <dft+0x34e>
-	mov    0x100(%rsp),%rdi
-	mov    $0x8,%esi
-	mov    %r8,0x8(%rsp)
-	call   1060 <calloc@plt>
-	mov    0x8(%rsp),%r8
-	mov    $0x8,%esi
-	mov    %rax,%rbp
-	mov    %r8,%rdi
-	call   1060 <calloc@plt>
-	mov    0x100(%rsp),%rdi
-	mov    $0x8,%esi
-	mov    %rax,0x30(%rsp)
-	call   1060 <calloc@plt>
-	mov    0x8(%rsp),%r8
-	mov    $0x8,%esi
-	mov    %rax,%r12
-	mov    %r8,%rdi
-	call   1060 <calloc@plt>
-	mov    %rax,0x68(%rsp)
-	mov    0x941a(%rip),%rax        
-	mov    %rax,0x38(%rsp)
-	jmp    bd38 <dft+0x188>
-	movsd  0x10(%rsp),%xmm2
-	movapd %xmm5,%xmm1
-	mov    0x98(%rsp),%rax
-	mulsd  %xmm5,%xmm1
+	movapd %xmm2,%xmm5
+	movapd %xmm2,%xmm1
 	movapd %xmm2,%xmm0
-	mulsd  %xmm2,%xmm0
-	subsd  %xmm1,%xmm0
-	movsd  %xmm0,(%rax)
-	movapd %xmm5,%xmm0
-	mov    0xa0(%rsp),%rax
-	addsd  %xmm5,%xmm0
-	mulsd  %xmm2,%xmm0
-	movsd  %xmm0,(%rax)
-	jmp    c09c <dft+0x4ec>
-	mov    %r11,%rdi
-	mov    %rax,0x8(%rsp)
+	jmp    bd8d <dft+0x30d>
+	mov    %rbx,%rdi
+	call   1030 <free@plt>
+	mov    %rbp,%rdi
 	call   1030 <free@plt>
-	mov    0x18(%rsp),%rdi
+	mov    0x30(%rsp),%rdi
+	call   1030 <free@plt>
+	mov    0x58(%rsp),%rdi
+	call   1030 <free@plt>
+	movsd  0x8(%rsp),%xmm0
+	movsd  0x10(%rsp),%xmm5
+	movapd %xmm0,%xmm1
+	movapd %xmm5,%xmm2
+	mulsd  %xmm0,%xmm1
+	mulsd  %xmm5,%xmm2
+	subsd  %xmm1,%xmm2
+	movapd %xmm0,%xmm1
+	addsd  %xmm0,%xmm1
+	mulsd  %xmm5,%xmm1
+	jmp    bed1 <dft+0x451>
+	mov    %rbx,%rdi
+	call   1030 <free@plt>
+	mov    %rbp,%rdi
 	call   1030 <free@plt>
-	mov    %r13,%rdi
+	mov    0x30(%rsp),%rdi
 	call   1030 <free@plt>
-	mov    0x8(%rsp),%rax
-	mov    %rax,%rdi
+	mov    0x58(%rsp),%rdi
 	call   1030 <free@plt>
-	mov    0x88(%rsp),%rax
-	pxor   %xmm5,%xmm5
-	movsd  %xmm5,0x60(%rsp)
-	movq   $0x0,(%rax)
-	mov    0x90(%rsp),%rax
-	movsd  %xmm5,0x58(%rsp)
-	movq   $0x0,(%rax)
-	jmp    c067 <dft+0x4b7>
+	pxor   %xmm1,%xmm1
+	movapd %xmm1,%xmm2
+	movsd  %xmm1,0x8(%rsp)
+	movsd  %xmm1,0x10(%rsp)
+	jmp    beb7 <dft+0x437>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,10 +1,10 @@
 
 
 
 Disassembly of section .fini:
 
-000000000000c294 <_fini>:
+000000000000c078 <_fini>:
 _fini():
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,2149 +1,2149 @@
 
 Hex dump of section '.rodata':
-  0x0000d000 00ebffff 18ebffff 28ebffff 38ebffff ........(...8...
-  0x0000d010 48ebffff 58ebffff 68ebffff 78ebffff H...X...h...x...
-  0x0000d020 88ebffff 98ebffff e0eaffff f0eaffff ................
+  0x0000d000 d0e9ffff e8e9ffff f8e9ffff 08eaffff ................
+  0x0000d010 18eaffff 28eaffff 38eaffff 48eaffff ....(...8...H...
+  0x0000d020 58eaffff 68eaffff b0e9ffff c0e9ffff X...h...........
   0x0000d030 00000040 000000bf 0000003f 0000803e ...@.......?...>
-  0x0000d040 0000403f 20bacf3a 20ba4f3c dcc2353d ..@? ..: .O<..5=
-  0x0000d050 dcc2b53d 9333e33d 00000000 00000000 ...=.3.=........
-  0x0000d060 abaaaaaa aaaaaaaa fd3f0000 00000000 .........?......
-  0x0000d070 89888888 88888888 fc3f0000 00000000 .........?......
-  0x0000d080 89888888 88888888 fe3f0000 00000000 .........?......
-  0x0000d090 6edbb66d dbb66ddb fdbf0000 00000000 n..m..m.........
-  0x0000d0a0 0cc3300c c3300cc3 fcbf0000 00000000 ..0..0..........
-  0x0000d0b0 0cc3300c c3300cc3 fe3f0000 00000000 ..0..0...?......
-  0x0000d0c0 659d2b0f 48d6b9f2 f93f0000 00000000 e.+.H....?......
-  0x0000d0d0 659d2b0f 48d6b9f2 fb3f0000 00000000 e.+.H....?......
-  0x0000d0e0 49922449 92244992 fcbf0000 00000000 I.$I.$I.........
-  0x0000d0f0 6edbb66d dbb66ddb fd3f0000 00000000 n..m..m..?......
-  0x0000d100 0cc3300c c3300cc3 fb3f0000 00000000 ..0..0...?......
-  0x0000d110 6edbb66d dbb66ddb fe3f0000 00000000 n..m..m..?......
-  0x0000d120 79fb92e6 d64954b2 f73f0000 00000000 y....IT..?......
-  0x0000d130 526c579b fe7be490 fb3f0000 00000000 RlW..{...?......
-  0x0000d140 e85a65c3 11d39ec8 fc3f0000 00000000 .Ze......?......
-  0x0000d150 8c31c618 638c31c6 fb3f0000 00000000 .1..c.1..?......
-  0x0000d160 29a59452 4a29a594 fe3f0000 00000000 )..RJ)...?......
-  0x0000d170 0b20a900 920a20a9 f73f0000 00000000 . .... ..?......
-  0x0000d180 096a89a0 96086a89 fb3f0000 00000000 .j....j..?......
-  0x0000d190 0c44be40 e40b44be fc3f0000 00000000 .D.@..D..?......
-  0x0000d1a0 cdcccccc cccccccc fb3f0000 00000000 .........?......
-  0x0000d1b0 d66ca4ea 1aeccb95 f63f0000 00000000 .l.......?......
-  0x0000d1c0 dc304bbd ab5f6bf3 f93f0000 00000000 .0K.._k..?......
-  0x0000d1d0 71faf847 9e6985a8 fb3f0000 00000000 q..G.i...?......
-  0x0000d1e0 00000000 00000080 fe3f0000 00000000 .........?......
-  0x0000d1f0 49922449 92244992 fd3f0000 00000000 I.$I.$I..?......
-  0x0000d200 2dc9a8eb abd4a98e f83f0000 00000000 -........?......
-  0x0000d210 79fb92e6 d64954b2 fc3f0000 00000000 y....IT..?......
-  0x0000d220 2dc9a8eb abd4a98e fe3f0000 00000000 -........?......
-  0x0000d230 abaaaaaa aaaaaaaa fc3f0000 00000000 .........?......
-  0x0000d240 abaaaaaa aaaaaaaa fe3f0000 00000000 .........?......
-  0x0000d250 7d9c39b6 2a1defb8 f83f0000 00000000 }.9.*....?......
-  0x0000d260 9d03c863 75e42ae7 fc3f0000 00000000 ...cu.*..?......
-  0x0000d270 7d9c39b6 2a1defb8 fe3f0000 00000000 }.9.*....?......
-  0x0000d280 8de09dc3 9f4ef596 fa3f0000 00000000 .....N...?......
-  0x0000d290 32f721c6 0316ab90 fe3f0000 00000000 2.!......?......
-  0x0000d2a0 87d6a4ad 8bc5c1ab f83f0000 00000000 .........?......
-  0x0000d2b0 290c0e99 ee36b2d6 fc3f0000 00000000 )....6...?......
-  0x0000d2c0 87d6a4ad 8bc5c1ab fe3f0000 00000000 .........?......
-  0x0000d2d0 455b0d9e 2350b4d5 f9bf0000 00000000 E[..#P..........
-  0x0000d2e0 0b59c842 16b29085 fc3f0000 00000000 .Y.B.....?......
-  0x0000d2f0 fc7549e5 c3b85f97 fc3f0000 00000000 .uI..._..?......
-  0x0000d300 38bde94d 6f7ad39b fd3f0000 00000000 8..Moz...?......
-  0x0000d310 b4d5e039 02455b8d ff3f0000 00000000 ...9.E[..?......
-  0x0000d320 210b59c8 4216b290 fe3f0000 00000000 !.Y.B....?......
-  0x0000d330 35788e40 d15683e7 fb3f0000 00000000 5x.@.V...?......
-  0x0000d340 7dbf8eff 247341b9 f23f0000 00000000 }...$sA..?......
-  0x0000d350 895d9987 5950e3a7 f73f0000 00000000 .]..YP...?......
-  0x0000d360 830e9443 bf6192b0 fa3f0000 00000000 ...C.a...?......
-  0x0000d370 6d97809f 89a169d0 fb3f0000 00000000 m.....i..?......
-  0x0000d380 bc4026c5 0b6452bc f83f0000 00000000 .@&..dR..?......
-  0x0000d390 8db0dcd3 08cb3d8d fa3f0000 00000000 ......=..?......
-  0x0000d3a0 a578814c 8a17c8a4 fb3f0000 00000000 .x.L.....?......
-  0x0000d3b0 e3053229 5e2093e2 fe3f0000 00000000 ..2)^ ...?......
-  0x0000d3c0 fbe59dca 38b9e9ae f13f0000 00000000 ....8....?......
-  0x0000d3d0 6b189f77 dbcf839e f63f0000 00000000 k..w.....?......
-  0x0000d3e0 337f1e21 8ac4b6a6 f93f0000 00000000 3..!.....?......
-  0x0000d3f0 baa2f1e3 5ff0c6c4 fa3f0000 00000000 ...._....?......
-  0x0000d400 0feaa00e eaa00eea f93f0000 00000000 .........?......
-  0x0000d410 cdcccccc cccccccc fc3f0000 00000000 .........?......
-  0x0000d420 9a999999 99999999 fe3f0000 00000000 .........?......
-  0x0000d430 aff72724 cfd9e9ad f23f0000 00000000 ..'$.....?......
-  0x0000d440 7738c4b8 63ed9b9d f73f0000 00000000 w8..c....?......
-  0x0000d450 1318766e 99e3c2a5 fa3f0000 00000000 ..vn.....?......
-  0x0000d460 a5f6ac08 0915a7c3 fb3f0000 00000000 .........?......
-  0x0000d470 0533feed 4bf7a899 f5bf0000 00000000 .3..K...........
-  0x0000d480 884cfde4 f1727de6 f63f0000 00000000 .L...r}..?......
-  0x0000d490 27863d67 085448d3 f93f0000 00000000 '.=g.TH..?......
-  0x0000d4a0 feea2dcb ef5dabb1 fb3f0000 00000000 ..-..]...?......
-  0x0000d4b0 f8b3074d 0217e6fc fb3f0000 00000000 ...M.....?......
-  0x0000d4c0 6b2fda85 3a49dc9a fe3f0000 00000000 k/..:I...?......
-  0x0000d4d0 278747cb f0670f9a fd3f0000 00000000 '.G..g...?......
-  0x0000d4e0 084d0217 e6fce0c9 fe3f0000 00000000 .M.......?......
-  0x0000d4f0 09531988 b5cd4abe ed3f0000 00000000 .S....J..?......
-  0x0000d500 105ed52a 911d8fa0 f33f0000 00000000 .^.*.....?......
-  0x0000d510 d3f60908 294912b4 f73f0000 00000000 ....)I...?......
-  0x0000d520 4ba30910 e4b5139b fa3f0000 00000000 K........?......
-  0x0000d530 fb419e8c ccbe3fa7 fb3f0000 00000000 .A....?..?......
-  0x0000d540 a142850a 152a54a8 f73f0000 00000000 .B...*T..?......
-  0x0000d550 4a93264d 9a3469d2 f93f0000 00000000 J.&M.4i..?......
-  0x0000d560 8203070e 1c3870e0 f93f0000 00000000 .....8p..?......
-  0x0000d570 bd7af5ea d5ab57af fd3f0000 00000000 .z....W..?......
-  0x0000d580 4a2ef685 a5e4629f fe3f0000 00000000 J.....b..?......
-  0x0000d590 bd7af5ea d5ab57af fb3f0000 00000000 .z....W..?......
-  0x0000d5a0 a142850a 152a54a8 ff3f0000 00000000 .B...*T..?......
-  0x0000d5b0 4a93264d 9a3469b2 fe3f0000 00000000 J.&M.4i..?......
-  0x0000d5c0 08a9eb70 7b90ba8e fc3f0000 00000000 ...p{....?......
-  0x0000d5d0 e9c06165 74b1a784 f03f0000 00000000 ..aet....?......
-  0x0000d5e0 89f5146b 74fbdadf f53f0000 00000000 ...kt....?......
-  0x0000d5f0 9881dfc9 585f0ffb f93f0000 00000000 ....X_...?......
-  0x0000d600 ab933df6 fa5136d8 fc3f0000 00000000 ..=..Q6..?......
-  0x0000d610 19d5359a eec52ee9 fd3f0000 00000000 ..5......?......
-  0x0000d620 b69e6d74 51e80b8e f43f0000 00000000 ..mtQ....?......
-  0x0000d630 8c52fba2 5b65cd9f f93f0000 00000000 .R..[e...?......
-  0x0000d640 e39e4d33 f26e0de3 fc3f0000 00000000 ..M3.n...?......
-  0x0000d650 5be425eb 1d70a2cd fe3f0000 00000000 [.%..p...?......
-  0x0000d660 dcc5e99a 75ad519e ee3f0000 00000000 ....u.Q..?......
-  0x0000d670 f13eb53a 5bea9485 f43f0000 00000000 .>.:[....?......
-  0x0000d680 7bb7d789 64cad095 f83f0000 00000000 {...d....?......
-  0x0000d690 dec25ef7 fb4f0581 fb3f0000 00000000 ..^..O...?......
-  0x0000d6a0 e676275d 74c9258b fc3f0000 00000000 .v']t.%..?......
-  0x0000d6b0 ae8940ae 8940ae89 f7bf0000 00000000 ..@..@..........
-  0x0000d6c0 f1f0f0f0 f0f0f0f0 f93f0000 00000000 .........?......
-  0x0000d6d0 f1f0f0f0 f0f0f0f0 fa3f0000 00000000 .........?......
-  0x0000d6e0 f1f0f0f0 f0f0f0f0 fd3f0000 00000000 .........?......
-  0x0000d6f0 f1f0f0f0 f0f0f0f0 fe3f0000 00000000 .........?......
-  0x0000d700 0b9dc10a 9dc10a9d fe3f0000 00000000 .........?......
-  0x0000d710 d3d2d2d2 d2d2d2d2 fc3f0000 00000000 .........?......
-  0x0000d720 8b21d31f e7f300ba ed3f0000 00000000 .!.......?......
-  0x0000d730 4d24da02 cbcdf09c f33f0000 00000000 M$.......?......
-  0x0000d740 7e8add75 cd6603b0 f73f0000 00000000 ~..u.f...?......
-  0x0000d750 366f4f3a c4069597 fa3f0000 00000000 6oO:.....?......
-  0x0000d760 7b90f822 5ed67aa3 fb3f0000 00000000 {.."^.z..?......
-  0x0000d770 0e6bdfb0 f60d6bdf f53f0000 00000000 .k....k..?......
-  0x0000d780 e9a28b2e bae8a28b f83f0000 00000000 .........?......
-  0x0000d790 09f29420 4f09f294 f83f0000 00000000 ... O....?......
-  0x0000d7a0 2fbae8a2 8b2ebae8 fb3f0000 00000000 /........?......
-  0x0000d7b0 95204f09 f294208f fc3f0000 00000000 . O... ..?......
-  0x0000d7c0 54823c25 c853829c fd3f0000 00000000 T.<%.S...?......
-  0x0000d7d0 bf61ed1b d6be618d ff3f0000 00000000 .a....a..?......
-  0x0000d7e0 2fbae8a2 8b2eba90 fe3f0000 00000000 /........?......
-  0x0000d7f0 4a90a704 794a90e7 fb3f0000 00000000 J...yJ...?......
-  0x0000d800 1911b1ff f2191e81 ec3f0000 00000000 .........?......
-  0x0000d810 dacc7a0f cacbe2d9 f13f0000 00000000 ..z......?......
-  0x0000d820 dc9cea64 1c785df4 f53f0000 00000000 ...d.x]..?......
-  0x0000d830 1e593f4f cb4f72d2 f83f0000 00000000 .Y?O.Or..?......
-  0x0000d840 0e407525 9de9f6e2 f93f0000 00000000 .@u%.....?......
-  0x0000d850 08822008 82200882 f83f0000 00000000 .. .. ...?......
-  0x0000d860 49922449 92244992 fb3f0000 00000000 I.$I.$I..?......
-  0x0000d870 f745c463 3e6830c3 ee3f0000 00000000 .E.c>h0..?......
-  0x0000d880 099b2da4 f4d7b0a4 f43f0000 00000000 ..-......?......
-  0x0000d890 357be809 a58eb4b8 f83f0000 00000000 5{.......?......
-  0x0000d8a0 85d30dd8 f352119f fb3f0000 00000000 .....R...?......
-  0x0000d8b0 7e81afd5 9e8b8dab fc3f0000 00000000 ~........?......
-  0x0000d8c0 0b39bd5c b321a6ef f6bf0000 00000000 .9.\.!..........
-  0x0000d8d0 0b39bd5c b321a6ef f73f0000 00000000 .9.\.!...?......
-  0x0000d8e0 b27b0b8c 8a8e2ed9 fb3f0000 00000000 .{.......?......
-  0x0000d8f0 7a65f126 98bfabe0 fc3f0000 00000000 ze.&.....?......
-  0x0000d900 a2a643f6 1910d5c7 fd3f0000 00000000 ..C......?......
-  0x0000d910 9b5072ac 458311b2 f13f0000 00000000 .Pr.E....?......
-  0x0000d920 8706e4f6 dc52cf9b f73f0000 00000000 .....R...?......
-  0x0000d930 b6850758 81685588 fb3f0000 00000000 ...X.hU..?......
-  0x0000d940 ae9a0062 aeb353c8 fc3f0000 00000000 ...b..S..?......
-  0x0000d950 8fb823ee 883be28e f93f0000 00000000 ..#..;...?......
-  0x0000d960 8fb823ee 883be28e fb3f0000 00000000 ..#..;...?......
-  0x0000d970 9535654d 5953d694 fc3f0000 00000000 .5eMYS...?......
-  0x0000d980 ee883be2 8eb823ee fe3f0000 00000000 ..;...#..?......
-  0x0000d990 1e7147dc 1177c4bd ff3f0000 00000000 .qG..w...?......
-  0x0000d9a0 410a8482 3c6e08c1 f23f0000 00000000 A...<n...?......
-  0x0000d9b0 f98833f2 7460e7a8 f83f0000 00000000 ..3.t`...?......
-  0x0000d9c0 da17ed53 6674ca93 fc3f0000 00000000 ...Sft...?......
-  0x0000d9d0 898bd412 047c29d9 fd3f0000 00000000 .....|)..?......
-  0x0000d9e0 cdcccccc cccccccc fabf0000 00000000 ................
-  0x0000d9f0 9a999999 99999999 fd3f0000 00000000 .........?......
-  0x0000da00 cdcccccc cccccccc fa3f0000 00000000 .........?......
-  0x0000da10 0e005009 870579df f43f0000 00000000 ..P...y..?......
-  0x0000da20 0c002628 d6e489c3 fa3f0000 00000000 ..&(.....?......
-  0x0000da30 0b402163 3ba818ab fe3f0000 00000000 .@!c;....?......
-  0x0000da40 10007aea 372668fb ff3f0000 00000000 ..z.7&h..?......
-  0x0000da50 aa91ae9d 423b9c84 f63f0000 00000000 ....B;...?......
-  0x0000da60 f26598d7 0977c5c2 fb3f0000 00000000 .e...w...?......
-  0x0000da70 69657cfb a0d355c9 ff3f0000 00000000 ie|...U..?......
-  0x0000da80 c592d785 85e6b3dd f33f0000 00000000 .........?......
-  0x0000da90 6ca01cd5 b469fdc1 f93f0000 00000000 l....i...?......
-  0x0000daa0 5f0c793a 7ebcbda9 fd3f0000 00000000 _.y:~....?......
-  0x0000dab0 1d859236 56636af9 fe3f0000 00000000 ...6Vcj..?......
-  0x0000dac0 45b6242c 342e448a f2bf0000 00000000 E.$,4.D.........
-  0x0000dad0 d6e32d37 c139d5ac f43f0000 00000000 ..-7.9...?......
-  0x0000dae0 cc5cf984 31880ad8 f63f0000 00000000 .\..1....?......
-  0x0000daf0 f552e740 8fe33bb2 f93f0000 00000000 .R.@..;..?......
-  0x0000db00 ee1f44d5 629328a0 f63f0000 00000000 ..D.b.(..?......
-  0x0000db10 6ba7fad3 99c94ec6 fc3f0000 00000000 k.....N..?......
-  0x0000db20 8a38c08b fb3825aa fd3f0000 00000000 .8...8%..?......
-  0x0000db30 6b01799e 0e0b9494 fc3f0000 00000000 k.y......?......
-  0x0000db40 74379a4f 6f0d8b98 ff3f0000 00000000 t7.Oo....?......
-  0x0000db50 51c58023 cbd0ad9e fe3f0000 00000000 Q..#.....?......
-  0x0000db60 b53b016c abe7e2fd fb3f0000 00000000 .;.l.....?......
-  0x0000db70 9ea69ae7 f879f89a e73f0000 00000000 .....y...?......
-  0x0000db80 4e7ab105 866bedd9 ed3f0000 00000000 Nz...k...?......
-  0x0000db90 3dd86c28 7dac6cdc f23f0000 00000000 =.l(}.l..?......
-  0x0000dba0 32f53ee0 32058dc4 f63f0000 00000000 2.>.2....?......
-  0x0000dbb0 d123ef82 665c9796 f93f0000 00000000 .#..f\...?......
-  0x0000dbc0 ffc9003c 9aef3a99 fa3f0000 00000000 ...<..:..?......
-  0x0000dbd0 efbcb6da 44e6f7f3 f33f0000 00000000 ....D....?......
-  0x0000dbe0 51e55f3f 7ce978d5 f63f0000 00000000 Q._?|.x..?......
-  0x0000dbf0 a6e35503 1478d0e2 fa3f0000 00000000 ..U..x...?......
-  0x0000dc00 16841893 72af1cac fc3f0000 00000000 ....r....?......
-  0x0000dc10 0622ccc8 b43c6c89 fc3f0000 00000000 ."...<l..?......
-  0x0000dc20 c5a0c49b a6e76d93 fd3f0000 00000000 ......m..?......
-  0x0000dc30 7fae84f7 8385fca1 fe3f0000 00000000 .........?......
-  0x0000dc40 5e3128f1 a6e979db fc3f0000 00000000 ^1(...y..?......
-  0x0000dc50 d91377ca be78d4fa f93f0000 00000000 ..w..x...?......
-  0x0000dc60 f39b7d79 e112d4ca e93f0000 00000000 ..}y.....?......
-  0x0000dc70 a7516c89 461d9d8e f03f0000 00000000 .Ql.F....?......
-  0x0000dc80 b9e4767a ad723f90 f53f0000 00000000 ..vz.r?..?......
-  0x0000dc90 de3f632c d9ec9f80 f93f0000 00000000 .?c,.....?......
-  0x0000dca0 3fb352e2 a8bc18c5 fb3f0000 00000000 ?.R......?......
-  0x0000dcb0 d3524031 2bf18cc8 fc3f0000 00000000 .R@1+....?......
-  0x0000dcc0 167dea6b 866d01a2 f03f0000 00000000 .}.k.m...?......
-  0x0000dcd0 a1bbdfa1 492402f3 f13f0000 00000000 ....I$...?......
-  0x0000dce0 1d85ebf6 3f1192ea f53f0000 00000000 ....?....?......
-  0x0000dcf0 a74bef5f c8a30dba f73f0000 00000000 .K._.....?......
-  0x0000dd00 cdb000a7 0bd0abcd f93f0000 00000000 .........?......
-  0x0000dd10 b4b4614f 792279b9 fb3f0000 00000000 ..aOy"y..?......
-  0x0000dd20 8da858a3 0befada2 fb3f0000 00000000 ..X......?......
-  0x0000dd30 e4ba9bfb 229042f8 fd3f0000 00000000 ....".B..?......
-  0x0000dd40 926f2832 27d2bfba fc3f0000 00000000 .o(2'....?......
-  0x0000dd50 972f609f b53cfed3 fe3f0000 00000000 ./`..<...?......
-  0x0000dd60 a8c1f53a 47d0c7ed e63f0000 00000000 ...:G....?......
-  0x0000dd70 2acc7415 727e30a7 ed3f0000 00000000 *.t.r~0..?......
-  0x0000dd80 0a675ea8 8fea1aa9 f23f0000 00000000 .g^......?......
-  0x0000dd90 07c9cbab 7c2eca96 f63f0000 00000000 ....|....?......
-  0x0000dda0 c337a777 c09e0fe7 f83f0000 00000000 .7.w.....?......
-  0x0000ddb0 1c3f2c6e d0311ceb f93f0000 00000000 .?,n.1...?......
-  0x0000ddc0 fc4950e1 e89639d7 f4bf0000 00000000 .IP...9.........
-  0x0000ddd0 3b537afd c5c920f2 f73f0000 00000000 ;Sz... ..?......
-  0x0000dde0 0266b874 b5dba0ac f93f0000 00000000 .f.t.....?......
-  0x0000ddf0 182783c8 0357d1ce fc3f0000 00000000 .'...W...?......
-  0x0000de00 9cad43bf d93af49b fe3f0000 00000000 ..C..:...?......
-  0x0000de10 bce14775 89590b85 ff3f0000 00000000 ..Gu.Y...?......
-  0x0000de20 101a02db 578f8bb4 fe3f0000 00000000 ....W....?......
-  0x0000de30 9cad43bf d93af49b fd3f0000 00000000 ..C..:...?......
-  0x0000de40 c155b433 a5d75f9c fb3f0000 00000000 .U.3.._..?......
-  0x0000de50 73da8311 21dcff8a f83f0000 00000000 s...!....?......
-  0x0000de60 c8a56542 6d7193ee e83f0000 00000000 ..eBmq...?......
-  0x0000de70 9178afd2 c0abbfa7 ef3f0000 00000000 .x.......?......
-  0x0000de80 366a08c4 dabbaba9 f43f0000 00000000 6j.......?......
-  0x0000de90 d9259321 76504b97 f83f0000 00000000 .%.!vPK..?......
-  0x0000dea0 6d4ef9af c47ed5e7 fa3f0000 00000000 mN...~...?......
-  0x0000deb0 8bc14628 8789e5eb fb3f0000 00000000 ..F(.....?......
-  0x0000dec0 0037159f 0712f7e8 f23f0000 00000000 .7.......?......
-  0x0000ded0 209032ab c62fd8cb f53f0000 00000000  .2../...?......
-  0x0000dee0 22b9e515 c3b295d8 f93f0000 00000000 "........?......
-  0x0000def0 952e5960 5adfc585 fb3f0000 00000000 ..Y`Z....?......
-  0x0000df00 1a15196b d1a69fa5 fa3f0000 00000000 ...k.....?......
-  0x0000df10 4447ef0d 1fe6eae6 fd3f0000 00000000 DG.......?......
-  0x0000df20 f198c30d 56fb89ee fe3f0000 00000000 ....V....?......
-  0x0000df30 252aef87 82a59a9d fe3f0000 00000000 %*.......?......
-  0x0000df40 c189e26d a4a1ced3 fc3f0000 00000000 ...m.....?......
-  0x0000df50 260b4ceb bbb810f2 f93f0000 00000000 &.L......?......
-  0x0000df60 c5a30afc 6ec11db7 e63f0000 00000000 ....n....?......
-  0x0000df70 277b3709 02ecc080 ed3f0000 00000000 '{7......?......
-  0x0000df80 18511ffe 60993a82 f23f0000 00000000 .Q..`.:..?......
-  0x0000df90 96be4a73 458d3fe8 f53f0000 00000000 ..JsE.?..?......
-  0x0000dfa0 cc46239d 2b06f1b1 f83f0000 00000000 .F#.+....?......
-  0x0000dfb0 2e05f6dc e24b0fb5 f93f0000 00000000 .....K...?......
-  0x0000dfc0 09486937 0252da8d f63f0000 00000000 .Hi7.R...?......
-  0x0000dfd0 0cc3300c c3300cc3 f93f0000 00000000 ..0..0...?......
-  0x0000dfe0 cff33ccf f33ccff3 fb3f0000 00000000 ..<..<...?......
-  0x0000dff0 dbb66ddb b66ddbb6 fd3f0000 00000000 ..m..m...?......
-  0x0000e000 dbb66ddb b66ddbb6 fe3f0000 00000000 ..m..m...?......
-  0x0000e010 d5087ad3 762f6cd6 ea3f0000 00000000 ..z.v/l..?......
-  0x0000e020 36ceb18c 5f11c496 f13f0000 00000000 6..._....?......
-  0x0000e030 e8f9c571 81507e98 f63f0000 00000000 ...q.P~..?......
-  0x0000e040 8aebab82 392bfa87 fa3f0000 00000000 ....9+...?......
-  0x0000e050 fd21d873 cff85cd0 fc3f0000 00000000 .!.s..\..?......
-  0x0000e060 fc09da5d 6eb803d4 fd3f0000 00000000 ...]n....?......
-  0x0000e070 5446c630 bf895bdd ebbf0000 00000000 TF.0..[.........
-  0x0000e080 bfb49464 4fa704a6 ed3f0000 00000000 ...dO....?......
-  0x0000e090 0e053f7b 3ea4ce8d f23f0000 00000000 ..?{>....?......
-  0x0000e0a0 c7b964b2 abd2a0db f33f0000 00000000 ..d......?......
-  0x0000e0b0 ccd733ac 51582ef6 f63f0000 00000000 ..3.QX...?......
-  0x0000e0c0 3057f35f 6c9b02cb f83f0000 00000000 0W._l....?......
-  0x0000e0d0 cf560278 d0d0339f fa3f0000 00000000 .V.x..3..?......
-  0x0000e0e0 15924e65 5fa09e99 fc3f0000 00000000 ..Ne_....?......
-  0x0000e0f0 703241c2 20460dc5 fb3f0000 00000000 p2A. F...?......
-  0x0000e100 0d3b53cd 86b528b3 fe3f0000 00000000 .;S...(..?......
-  0x0000e110 787d1a91 31aff7d5 fd3f0000 00000000 x}..1....?......
-  0x0000e120 a5ce09f6 05f1e4bf fe3f0000 00000000 .........?......
-  0x0000e130 5a30365b 1d2fe984 e23f0000 00000000 Z06[./...?......
-  0x0000e140 82d80ce1 29395590 e93f0000 00000000 ....)9U..?......
-  0x0000e150 927102cc 6ba59fed ee3f0000 00000000 .q..k....?......
-  0x0000e160 0f9b72aa c7f1e1ba f33f0000 00000000 ..r......?......
-  0x0000e170 8bbf407f fa1e3591 f73f0000 00000000 ..@...5..?......
-  0x0000e180 6a30c586 8f6afbcd f93f0000 00000000 j0...j...?......
-  0x0000e190 7b6e6e89 96f13bc9 fa3f0000 00000000 {nn...;..?......
-  0x0000e1a0 d34faac2 a6fde2a9 ee3f0000 00000000 .O.......?......
-  0x0000e1b0 c8e35473 10bd5bd4 f03f0000 00000000 ..Ts..[..?......
-  0x0000e1c0 ae3fa32d f895e192 f43f0000 00000000 .?.-.....?......
-  0x0000e1d0 13ac7647 187325d2 f63f0000 00000000 ..vG.s%..?......
-  0x0000e1e0 57bfec45 9cb3f3ed f73f0000 00000000 W..E.....?......
-  0x0000e1f0 dc508ccb 22d20e80 fb3f0000 00000000 .P.."....?......
-  0x0000e200 6b293a15 e1b95287 fa3f0000 00000000 k):...R..?......
-  0x0000e210 44a1f9ed 653f77be fd3f0000 00000000 D...e?w..?......
-  0x0000e220 e02e13cb 436b93cc fe3f0000 00000000 ....Ck...?......
-  0x0000e230 6b86ce55 2e064d80 fd3f0000 00000000 k..U..M..?......
-  0x0000e240 8a404651 2f1c2fb4 ff3f0000 00000000 .@FQ/./..?......
-  0x0000e250 add09725 3be33ac1 fe3f0000 00000000 ...%;.:..?......
-  0x0000e260 f1a6acb7 9582959a fc3f0000 00000000 .........?......
-  0x0000e270 a60b732f f181b4db e33f0000 00000000 ..s/.....?......
-  0x0000e280 a7ee86e9 1b0596ee ea3f0000 00000000 .........?......
-  0x0000e290 727fc271 082466c4 f03f0000 00000000 r..q.$f..?......
-  0x0000e2a0 5c1332aa 0ffc759a f53f0000 00000000 \.2...u..?......
-  0x0000e2b0 341d12cf ef2008f0 f83f0000 00000000 4.... ...?......
-  0x0000e2c0 aba9520b 38323faa fb3f0000 00000000 ..R.82?..?......
-  0x0000e2d0 2f23f0a1 a89752a6 fc3f0000 00000000 /#....R..?......
-  0x0000e2e0 3f4d432a fb2115a9 e63f0000 00000000 ?MC*.!...?......
-  0x0000e2f0 e315e5bf e6f29cb7 ed3f0000 00000000 .........?......
-  0x0000e300 96998f5d 187c2597 f33f0000 00000000 ...].|%..?......
-  0x0000e310 9b3ea62c 561fbeed f73f0000 00000000 .>.,V....?......
-  0x0000e320 c307403e c0c7b9b8 fb3f0000 00000000 ..@>.....?......
-  0x0000e330 5d6f0431 b1210583 fe3f0000 00000000 ]o.1.!...?......
-  0x0000e340 45511445 51144591 f0bf0000 00000000 EQ.EQ.E.........
-  0x0000e350 398ee338 8ee338fe f23f0000 00000000 9..8..8..?......
-  0x0000e360 10044110 044110ec f43f0000 00000000 ..A..A...?......
-  0x0000e370 55555555 5555d5a6 f83f0000 00000000 UUUUUU...?......
-  0x0000e380 44444444 4444e481 f93f0000 00000000 DDDDDD...?......
-  0x0000e390 89888888 88883082 fb3f0000 00000000 ......0..?......
-  0x0000e3a0 363b6a11 f2d7348d fd3f0000 00000000 6;j...4..?......
-  0x0000e3b0 89888888 8888c0c0 fd3f0000 00000000 .........?......
-  0x0000e3c0 caa55cca a55caab6 f93f0000 00000000 ..\..\...?......
-  0x0000e3d0 32266332 2663a195 fe3f0000 00000000 2&c2&c...?......
-  0x0000e3e0 85544885 54488fd2 fe3f0000 00000000 .TH.TH...?......
-  0x0000e3f0 66599665 59965b8c fe3f0000 00000000 fY.eY.[..?......
-  0x0000e400 50077550 0775fcc0 fc3f0000 00000000 P.uP.u...?......
-  0x0000e410 5c0818a5 9a3c8edc f93f0000 00000000 \....<...?......
-  0x0000e420 a33773f4 5c0f9796 ea3f0000 00000000 .7s.\....?......
-  0x0000e430 26d4def4 71316af9 f03f0000 00000000 &...q1j..?......
-  0x0000e440 af8aab1b e669d196 f63f0000 00000000 .....i...?......
-  0x0000e450 fe2a80d4 a0202da3 fa3f0000 00000000 .*... -..?......
-  0x0000e460 5832835c 9685199f fd3f0000 00000000 X2.\.....?......
-  0x0000e470 ae0de157 e6d638ee fe3f0000 00000000 ...W..8..?......
-  0x0000e480 7d4cedc3 483b3195 e33f0000 00000000 }L..H;1..?......
-  0x0000e490 10b1c304 617603a2 ea3f0000 00000000 ....av...?......
-  0x0000e4a0 58a8e4d3 56ba5d85 f03f0000 00000000 X...V.]..?......
-  0x0000e4b0 67e6c029 a887c6d1 f43f0000 00000000 g..).....?......
-  0x0000e4c0 8fbe1723 90c9fea2 f83f0000 00000000 ...#.....?......
-  0x0000e4d0 ee947db6 e4f436e7 fa3f0000 00000000 ..}...6..?......
-  0x0000e4e0 74d3ac6e 0b97e2e1 fb3f0000 00000000 t..n.....?......
-  0x0000e4f0 b745f6fc 232919c7 eebf0000 00000000 .E..#)..........
-  0x0000e500 007d577d ff0336ae f13f0000 00000000 .}W}..6..?......
-  0x0000e510 a518883d 6d71c4a1 f33f0000 00000000 ...=mq...?......
-  0x0000e520 11d48254 3fe5a6e4 f63f0000 00000000 ...T?....?......
-  0x0000e530 9d2b9e10 cd02a7dd f63f0000 00000000 .+.......?......
-  0x0000e540 b4d4fd90 65e40294 fa3f0000 00000000 ....e....?......
-  0x0000e550 64f4da4c 7b0fdcee fb3f0000 00000000 d..L{....?......
-  0x0000e560 51e49beb ab553cde fa3f0000 00000000 Q....U<..?......
-  0x0000e570 dcc7b735 db4a60b8 fd3f0000 00000000 ...5.J`..?......
-  0x0000e580 0c42e2e2 d721c6e3 fe3f0000 00000000 .B...!...?......
-  0x0000e590 b2aba635 fa9415a0 fe3f0000 00000000 ...5.....?......
-  0x0000e5a0 78ace3dd b5c425d8 fc3f0000 00000000 x.....%..?......
-  0x0000e5b0 400ebb46 ab9706f7 f93f0000 00000000 @..F.....?......
-  0x0000e5c0 93e4795d 0261c3f0 e03f0000 00000000 ..y].a...?......
-  0x0000e5d0 1c2fc148 ac15ba82 e83f0000 00000000 ./.H.....?......
-  0x0000e5e0 6c6e3ff5 3f2739d7 ed3f0000 00000000 ln?.?'9..?......
-  0x0000e5f0 3a1bec3b d2f743a9 f23f0000 00000000 :..;..C..?......
-  0x0000e600 e72a5fde 3ce08483 f63f0000 00000000 .*_.<....?......
-  0x0000e610 dd1c3d0a 958490ba f83f0000 00000000 ..=......?......
-  0x0000e620 3291dcc6 35a043b6 f93f0000 00000000 2...5.C..?......
-  0x0000e630 ccbfcc43 e5a67e8e f13f0000 00000000 ...C..~..?......
-  0x0000e640 c65746ec c17b4ea0 f43f0000 00000000 .WF..{N..?......
-  0x0000e650 b21fb3e5 57fabdd5 f33f0000 00000000 ....W....?......
-  0x0000e660 b5868526 850a10cf f83f0000 00000000 ...&.....?......
-  0x0000e670 afa81fd3 221974e3 fa3f0000 00000000 ....".t..?......
-  0x0000e680 4f5f1460 ea97e4a1 fb3f0000 00000000 O_.`.....?......
-  0x0000e690 1b3800fb aee2a8aa fb3f0000 00000000 .8.......?......
-  0x0000e6a0 f4dd189c de09a986 fe3f0000 00000000 .........?......
-  0x0000e6b0 4305cd49 d651748c ff3f0000 00000000 C..I.Qt..?......
-  0x0000e6c0 0a62a935 859f16c3 fe3f0000 00000000 .b.5.....?......
-  0x0000e6d0 30af0eb1 cb5333aa fd3f0000 00000000 0....S3..?......
-  0x0000e6e0 18cfed9e 44813eab fb3f0000 00000000 ....D.>..?......
-  0x0000e6f0 c062d370 598f3798 f83f0000 00000000 .b.pY.7..?......
-  0x0000e700 fdf5c620 0cab6c93 e43f0000 00000000 ... ..l..?......
-  0x0000e710 200f982b bf0118a0 eb3f0000 00000000  ..+.....?......
-  0x0000e720 f5da6c1f 072cc983 f13f0000 00000000 ..l..,...?......
-  0x0000e730 fb500c5f 27314acf f53f0000 00000000 .P._'1J..?......
-  0x0000e740 4a46c64f 8e5a10a1 f93f0000 00000000 JF.O.Z...?......
-  0x0000e750 469c154b ab9579e4 fb3f0000 00000000 F..K..y..?......
-  0x0000e760 c65ccc8f 856235df fc3f0000 00000000 .\...b5..?......
-  0x0000e770 ed22df46 54fd2c81 ed3f0000 00000000 .".FT.,..?......
-  0x0000e780 a8eb9658 a93c78a1 ef3f0000 00000000 ...X.<x..?......
-  0x0000e790 ba818cba 61cb5ddf f23f0000 00000000 ....a.]..?......
-  0x0000e7a0 89aeaa3f b2a6c99f f53f0000 00000000 ...?.....?......
-  0x0000e7b0 567d919a 686be2c5 f63f0000 00000000 V}..hk...?......
-  0x0000e7c0 94526827 f17356cd f93f0000 00000000 .Rh'.sV..?......
-  0x0000e7d0 cd1b8bca 29b562a1 f83f0000 00000000 ....).b..?......
-  0x0000e7e0 432bc2eb 77ce4ba9 fc3f0000 00000000 C+..w.K..?......
-  0x0000e7f0 cf69e890 9dc3eb94 fd3f0000 00000000 .i.......?......
-  0x0000e800 4492e194 f89e5fb3 fc3f0000 00000000 D....._..?......
-  0x0000e810 e8718fa2 b4368d96 ff3f0000 00000000 .q...6...?......
-  0x0000e820 614e33cb 6184309c fe3f0000 00000000 aN3.a.0..?......
-  0x0000e830 9cb0eb11 363ae7f9 fb3f0000 00000000 ....6:...?......
-  0x0000e840 ef8220d2 4299f19d e03f0000 00000000 .. .B....?......
-  0x0000e850 304e2f90 6e5c84ab e73f0000 00000000 0N/.n\...?......
-  0x0000e860 0b4086d3 5870308d ed3f0000 00000000 .@..Xp0..?......
-  0x0000e870 aa47fd94 2ba714de f13f0000 00000000 .G..+....?......
-  0x0000e880 74c7fffd ab6d8eac f53f0000 00000000 t....m...?......
-  0x0000e890 ef98ca4f 2106c7f4 f73f0000 00000000 ...O!....?......
-  0x0000e8a0 5ebb969c 14a022ef f83f0000 00000000 ^....."..?......
-  0x0000e8b0 637f0bce 4bc864a2 f2bf0000 00000000 c...K.d.........
-  0x0000e8c0 28cf4f3b 68934adf f53f0000 00000000 (.O;h.J..?......
-  0x0000e8d0 3847d955 e01360ce f73f0000 00000000 8G.U..`..?......
-  0x0000e8e0 70dfdf7c 4562dc94 f53f0000 00000000 p..|Eb...?......
-  0x0000e8f0 33a0f2db f7375f91 fb3f0000 00000000 3....7_..?......
-  0x0000e900 feee1470 9d65e596 fd3f0000 00000000 ...p.e...?......
-  0x0000e910 fc7af2fc b48336a9 fe3f0000 00000000 .z....6..?......
-  0x0000e920 6e294372 ae5075f9 fe3f0000 00000000 n)Cr.Pu..?......
-  0x0000e930 74bf3b05 5c6759b9 fe3f0000 00000000 t.;.\gY..?......
-  0x0000e940 2bb79421 3957a8ba fd3f0000 00000000 +..!9W...?......
-  0x0000e950 8e03d991 acfab8f9 fb3f0000 00000000 .........?......
-  0x0000e960 3ed4cc5f 0d2408c8 f93f0000 00000000 >.._.$...?......
-  0x0000e970 73f794e8 c3487a91 f63f0000 00000000 s....Hz..?......
-  0x0000e980 5118048d eff0bc98 e43f0000 00000000 Q........?......
-  0x0000e990 68722223 a42ddda5 eb3f0000 00000000 hr"#.-...?......
-  0x0000e9a0 1da1b6a3 00268988 f13f0000 00000000 .....&...?......
-  0x0000e9b0 83ec8a0b 54d6c2d6 f53f0000 00000000 ....T....?......
-  0x0000e9c0 8ebfac02 ed79dea6 f93f0000 00000000 .....y...?......
-  0x0000e9d0 48f00afe 04b4b5ec fb3f0000 00000000 H........?......
-  0x0000e9e0 35785821 26e940e7 fc3f0000 00000000 5xX!&.@..?......
-  0x0000e9f0 43642718 b472ac95 f03f0000 00000000 Cd'..r...?......
-  0x0000ea00 cb502c9b 0a0162a8 f33f0000 00000000 .P,...b..?......
-  0x0000ea10 64163b24 0eac82e0 f23f0000 00000000 d.;$.....?......
-  0x0000ea20 b13d19b3 ad967ed9 f73f0000 00000000 .=....~..?......
-  0x0000ea30 dcc09253 6fdd0ad0 f93f0000 00000000 ...So....?......
-  0x0000ea40 d78c31b0 dff610f9 f73f0000 00000000 ..1......?......
-  0x0000ea50 d35aa692 cdefbab7 fc3f0000 00000000 .Z.......?......
-  0x0000ea60 9870bdb9 0ca9c197 fe3f0000 00000000 .p.......?......
-  0x0000ea70 b238ce3e 43798a86 ff3f0000 00000000 .8.>Cy...?......
-  0x0000ea80 d28a7cf9 be217eb7 fe3f0000 00000000 ..|..!~..?......
-  0x0000ea90 384e6281 fb73d89e fd3f0000 00000000 8Nb..s...?......
-  0x0000eaa0 26f3380a a7c5649f fb3f0000 00000000 &.8...d..?......
-  0x0000eab0 e849dd7a 94e8ae8d f83f0000 00000000 .I.z.....?......
-  0x0000eac0 bdd0a245 beaf2aaa e13f0000 00000000 ...E..*..?......
-  0x0000ead0 aece9e9f d85acab8 e83f0000 00000000 .....Z...?......
-  0x0000eae0 49c38fbe 89981d98 ee3f0000 00000000 I........?......
-  0x0000eaf0 bad4e0ac 386244ef f23f0000 00000000 ....8bD..?......
-  0x0000eb00 349de52c 4103e9b9 f63f0000 00000000 4..,A....?......
-  0x0000eb10 38a9730c 6734dc83 f93f0000 00000000 8.s.g4...?......
-  0x0000eb20 ee5ffed5 971dd280 fa3f0000 00000000 ._.......?......
-  0x0000eb30 250b20dc 78fb92de f33f0000 00000000 %. .x....?......
-  0x0000eb40 0e09da32 526cd7b4 f73f0000 00000000 ...2Rl...?......
-  0x0000eb50 cb8623a6 3d91a187 fa3f0000 00000000 ..#.=....?......
-  0x0000eb60 74cceb05 f134a8f8 fb3f0000 00000000 t....4...?......
-  0x0000eb70 c85fb3a3 1621699b fd3f0000 00000000 ._...!i..?......
-  0x0000eb80 01a35493 c79dde8b fe3f0000 00000000 ..T......?......
-  0x0000eb90 57d970c4 b4277eba fe3f0000 00000000 W.p..'~..?......
-  0x0000eba0 66028b6d 6ce0f3c2 f2bf0000 00000000 f..ml...........
-  0x0000ebb0 66028b6d 6ce0f3c2 f33f0000 00000000 f..ml....?......
-  0x0000ebc0 da1215c2 809a81e7 f83f0000 00000000 .........?......
-  0x0000ebd0 e33ecb73 026a8dea f93f0000 00000000 .>.s.j...?......
-  0x0000ebe0 5b3d4788 e0a36982 fd3f0000 00000000 [=G...i..?......
-  0x0000ebf0 5297e59b 300fbe89 fe3f0000 00000000 R...0....?......
-  0x0000ec00 57340db2 67f820bb fe3f0000 00000000 W4..g. ..?......
-  0x0000ec10 f9201d94 0abc778c ec3f0000 00000000 . ....w..?......
-  0x0000ec20 e94edbea 4940b083 f33f0000 00000000 .N..I@...?......
-  0x0000ec30 2a10f347 87afcb95 f83f0000 00000000 *..G.....?......
-  0x0000ec40 cfa636f1 28c3f7e0 fb3f0000 00000000 ..6.(....?......
-  0x0000ec50 18c5a0e6 8bb3069e fd3f0000 00000000 .........?......
-  0x0000ec60 01fe8433 ff017bcc f33f0000 00000000 ...3..{..?......
-  0x0000ec70 01fe8433 ff017bcc f53f0000 00000000 ...3..{..?......
-  0x0000ec80 a16e6b73 5f91948c f93f0000 00000000 .nks_....?......
-  0x0000ec90 79d27163 872d8e9c fb3f0000 00000000 y.qc.-...?......
-  0x0000eca0 895457d0 215653da fa3f0000 00000000 .TW.!VS..?......
-  0x0000ecb0 aa02a410 01a8069a fe3f0000 00000000 .........?......
-  0x0000ecc0 78ffabfc 32abfead fe3f0000 00000000 x...2....?......
-  0x0000ecd0 78ffabfc 32abfead fc3f0000 00000000 x...2....?......
-  0x0000ece0 2cfd3b37 3d4a1c97 eb3f0000 00000000 ,.;7=J...?......
-  0x0000ecf0 593dc863 9985aa8d f23f0000 00000000 Y=.c.....?......
-  0x0000ed00 fcf8e647 2b2b25a1 f73f0000 00000000 ...G++%..?......
-  0x0000ed10 7813760a e64e03f2 fa3f0000 00000000 x.v..N...?......
-  0x0000ed20 d17c23de 84d3ffa9 fc3f0000 00000000 .|#......?......
-  0x0000ed30 0bb4400b b4400bb4 f6bf0000 00000000 ..@..@..........
-  0x0000ed40 08877008 87700887 f93f0000 00000000 ..p..p...?......
-  0x0000ed50 0dd2200d d2200dd2 f93f0000 00000000 .. .. ...?......
-  0x0000ed60 3bb1133b b1133bb1 fd3f0000 00000000 ;..;..;..?......
-  0x0000ed70 27766227 766227f6 fe3f0000 00000000 'vb'vb'..?......
-  0x0000ed80 07699006 699006a9 ff3f0000 00000000 .i..i....?......
-  0x0000ed90 5dcdd55c cdd55ccd fd3f0000 00000000 ]..\..\..?......
-  0x0000eda0 e9888ee8 888ee888 fb3f0000 00000000 .........?......
-  0x0000edb0 a3744917 a3d345ba ed3f0000 00000000 .tI...E..?......
-  0x0000edc0 59ddd4e5 6876a1ae f43f0000 00000000 Y...hv...?......
-  0x0000edd0 6255d5eb b076a4c6 f93f0000 00000000 bU...v...?......
-  0x0000ede0 66d2a599 79ea2995 fd3f0000 00000000 f...y.)..?......
-  0x0000edf0 37a3327a 178e8ed1 fe3f0000 00000000 7.2z.....?......
-  0x0000ee00 8ee3388e e3388ee3 ed3f0000 00000000 ..8..8...?......
-  0x0000ee10 55555555 555555d5 f43f0000 00000000 UUUUUUU..?......
-  0x0000ee20 abaaaaaa aaaaaaf2 f93f0000 00000000 .........?......
-  0x0000ee30 398ee338 8ee338b6 fd3f0000 00000000 9..8..8..?......
-  0x0000ee40 2fc057f8 b1508ac9 ef3f0000 00000000 /.W..P...?......
-  0x0000ee50 d2e0b2c9 67d2d9a5 f63f0000 00000000 ....g....?......
-  0x0000ee60 5e0667c4 a09b8a9c fb3f0000 00000000 ^.g......?......
-  0x0000ee70 833efb55 5de427ae fe3f0000 00000000 .>.U].'..?......
-  0x0000ee80 d509d5ab 5ef21c85 ed3f0000 00000000 ....^....?......
-  0x0000ee90 6f722f82 714696f9 f33f0000 00000000 or/.qF...?......
-  0x0000eea0 7c2f3ef5 76def38d f93f0000 00000000 |/>.v....?......
-  0x0000eeb0 bf31339f 2b5c30d5 fc3f0000 00000000 .13.+\0..?......
-  0x0000eec0 0fab4f81 aa90c095 fe3f0000 00000000 ..O......?......
-  0x0000eed0 8f56ad95 a6b9a199 e2bf0000 00000000 .V..............
-  0x0000eee0 33ac183b 10280ac0 e43f0000 00000000 3..;.(...?......
-  0x0000eef0 a22f9e69 0627d6b0 e93f0000 00000000 ./.i.'...?......
-  0x0000ef00 4d46b707 49530ce9 eb3f0000 00000000 MF..IS...?......
-  0x0000ef10 af25f15c 4fa9a494 ef3f0000 00000000 .%.\O....?......
-  0x0000ef20 bbd3058e cd9432d7 f13f0000 00000000 ......2..?......
-  0x0000ef30 04aafc72 3bbeb1d2 f33f0000 00000000 ...r;....?......
-  0x0000ef40 e15f8b5b 28e7c5ba f63f0000 00000000 ._.[(....?......
-  0x0000ef50 ed0d1b8b cb18d8a7 f63f0000 00000000 .........?......
-  0x0000ef60 9262bc57 7debb196 fa3f0000 00000000 .b.W}....?......
-  0x0000ef70 52af4538 4018c5f1 f93f0000 00000000 R.E8@....?......
-  0x0000ef80 83c90161 81bc39b9 fc3f0000 00000000 ...a..9..?......
-  0x0000ef90 45336587 3fda8ec4 fd3f0000 00000000 E3e.?....?......
-  0x0000efa0 6ea57abd 51ba0bc9 f63f0000 00000000 n.z.Q....?......
-  0x0000efb0 b046df6b d3e082c9 fe3f0000 00000000 .F.k.....?......
-  0x0000efc0 2a178492 e5a3cf86 fe3f0000 00000000 *........?......
-  0x0000efd0 aabe39b7 d59fb2d7 fb3f0000 00000000 ..9......?......
-  0x0000efe0 35e8396a d20032e7 d43f0000 00000000 5.9j..2..?......
-  0x0000eff0 95009120 cf3895e3 dc3f0000 00000000 ... .8...?......
-  0x0000f000 78f56a05 c0619db8 e33f0000 00000000 x.j..a...?......
-  0x0000f010 a8abc780 001d999f e93f0000 00000000 .........?......
-  0x0000f020 33b4d688 8b45c19e ee3f0000 00000000 3....E...?......
-  0x0000f030 b1a278ba 1949fdb6 f23f0000 00000000 ..x..I...?......
-  0x0000f040 bb4df416 11b09be9 f53f0000 00000000 .M.......?......
-  0x0000f050 d95801d8 1eabd192 f83f0000 00000000 .X.......?......
-  0x0000f060 8b50c978 141f0086 f93f0000 00000000 .P.x.....?......
-  0x0000f070 3dbecb71 717abffd e43f0000 00000000 =..qqz...?......
-  0x0000f080 75469243 238b07de e73f0000 00000000 uF.C#....?......
-  0x0000f090 75469243 238b07de eb3f0000 00000000 uF.C#....?......
-  0x0000f0a0 75469243 238b07de ee3f0000 00000000 uF.C#....?......
-  0x0000f0b0 4d5b1242 ca687de2 f03f0000 00000000 M[.B.h}..?......
-  0x0000f0c0 f9f4b102 f2cbe59b f43f0000 00000000 .........?......
-  0x0000f0d0 16dd71d0 a6b5a7ab f13f0000 00000000 ..q......?......
-  0x0000f0e0 9bb6d065 798e07b0 f83f0000 00000000 ...ey....?......
-  0x0000f0f0 d8c4c0f8 03aeacae f93f0000 00000000 .........?......
-  0x0000f100 5edc2d1e 2022d2dc fa3f0000 00000000 ^.-. "...?......
-  0x0000f110 58a1de75 1149ea83 fd3f0000 00000000 X..u.I...?......
-  0x0000f120 5aac6b0d 95103397 fd3f0000 00000000 Z.k...3..?......
-  0x0000f130 4c661fff 0a98b3e3 fc3f0000 00000000 Lf.......?......
-  0x0000f140 60aab2f5 39d6fa9e ff3f0000 00000000 `...9....?......
-  0x0000f150 f2d04cea e2200ecd fe3f0000 00000000 ..L.. ...?......
-  0x0000f160 3c8c960f 38a7ad8b fd3f0000 00000000 <...8....?......
-  0x0000f170 fb0dacc8 ade3a19f fa3f0000 00000000 .........?......
-  0x0000f180 1c6fd004 1cbd7af5 d63f0000 00000000 .o....z..?......
-  0x0000f190 5f2dbd94 27d2a4f1 de3f0000 00000000 _-..'....?......
-  0x0000f1a0 7920a81b 7a5e05c4 e53f0000 00000000 y ..z^...?......
-  0x0000f1b0 3545a4e5 a76b75a9 eb3f0000 00000000 5E...ku..?......
-  0x0000f1c0 9f0d2bb7 4e3e90a8 f03f0000 00000000 ..+.N>...?......
-  0x0000f1d0 e3265a00 94904bc2 f43f0000 00000000 .&Z...K..?......
-  0x0000f1e0 ad7204f4 0d960af8 f73f0000 00000000 .r.......?......
-  0x0000f1f0 da8c350c 7adae39b fa3f0000 00000000 ..5.z....?......
-  0x0000f200 2549241d 5b8f478e fb3f0000 00000000 %I$.[.G..?......
-  0x0000f210 05a56942 616c04b3 e7bf0000 00000000 ..iBal..........
-  0x0000f220 a5d9b66a edf964c9 ea3f0000 00000000 ...j..d..?......
-  0x0000f230 cd26ca74 501dfdce ed3f0000 00000000 .&.tP....?......
-  0x0000f240 8178420d e469639e f13f0000 00000000 .xB..ic..?......
-  0x0000f250 582541e8 7bd2629d ec3f0000 00000000 X%A.{.b..?......
-  0x0000f260 d32fa174 d5ab1a8c f63f0000 00000000 ./.t.....?......
-  0x0000f270 cbecac78 b48445db f73f0000 00000000 ...x..E..?......
-  0x0000f280 b194048f 0de3ca80 f83f0000 00000000 .........?......
-  0x0000f290 8f2d1057 5ede8db0 fb3f0000 00000000 .-.W^....?......
-  0x0000f2a0 eb5be260 fc5b63c6 fc3f0000 00000000 .[.`.[c..?......
-  0x0000f2b0 a54b7356 a1a394f8 fb3f0000 00000000 .KsV.....?......
-  0x0000f2c0 0a59ed84 3c5e4c97 fd3f0000 00000000 .Y..<^L..?......
-  0x0000f2d0 c7271282 b86e93d2 fe3f0000 00000000 .'...n...?......
-  0x0000f2e0 adb1128a c44603b9 fe3f0000 00000000 .....F...?......
-  0x0000f2f0 1c6fe6f8 c88a11a4 fd3f0000 00000000 .o.......?......
-  0x0000f300 e613cb59 5419fda5 fb3f0000 00000000 ...YT....?......
-  0x0000f310 b01198c1 bca48b93 f83f0000 00000000 .........?......
-  0x0000f320 0cb86b70 ecd950ae da3f0000 00000000 ..kp..P..?......
-  0x0000f330 2c09aabe 849697ab e23f0000 00000000 ,........?......
-  0x0000f340 1c445559 c4f7318b e93f0000 00000000 .DUY..1..?......
-  0x0000f350 7044dd6e c399aaf0 ee3f0000 00000000 pD.n.....?......
-  0x0000f360 8751d0af 231f65ef f33f0000 00000000 .Q..#.e..?......
-  0x0000f370 ff757c49 b53df889 f83f0000 00000000 .u|I.=...?......
-  0x0000f380 33c8e484 239222b0 fb3f0000 00000000 3...#."..?......
-  0x0000f390 2d5a1365 816a65dd fd3f0000 00000000 -Z.e.je..?......
-  0x0000f3a0 d38de20b 71ff10ca fe3f0000 00000000 ....q....?......
-  0x0000f3b0 eb910fd8 8264b6f9 e53f0000 00000000 .....d...?......
-  0x0000f3c0 70ad0b22 62cb48bb e73f0000 00000000 p.."b.H..?......
-  0x0000f3d0 56ef1fe9 ddaa90ff ec3f0000 00000000 V........?......
-  0x0000f3e0 c831387a b85993c3 ee3f0000 00000000 .18z.Y...?......
-  0x0000f3f0 f1feb33b 41d40dbf f23f0000 00000000 ...;A....?......
-  0x0000f400 9b8198b4 bab67597 f43f0000 00000000 ......u..?......
-  0x0000f410 2f9585d2 8ed6abfb f63f0000 00000000 /........?......
-  0x0000f420 34f8d11a ddbb2ad6 f83f0000 00000000 4.....*..?......
-  0x0000f430 51dc3678 c352b58a fa3f0000 00000000 Q.6x.R...?......
-  0x0000f440 726de6d3 f151418c fc3f0000 00000000 rm...QA..?......
-  0x0000f450 506d6d75 c699f187 fb3f0000 00000000 Pmmu.....?......
-  0x0000f460 4e6d7293 f3418093 fe3f0000 00000000 Nmr..A...?......
-  0x0000f470 068914c6 4e437794 fd3f0000 00000000 ....NCw..?......
-  0x0000f480 b8cc8ac2 abadcfca fe3f0000 00000000 .........?......
-  0x0000f490 10ac758d a2c516da da3f0000 00000000 ..u......?......
-  0x0000f4a0 704f2ce6 b70ef0ac e23f0000 00000000 pO,......?......
-  0x0000f4b0 b0f86006 ed82e4d7 e83f0000 00000000 ..`......?......
-  0x0000f4c0 2918569a daecce87 ee3f0000 00000000 ).V......?......
-  0x0000f4d0 416286b9 a2a01bb7 f23f0000 00000000 Ab.......?......
-  0x0000f4e0 53a5aa81 4cf8b181 f63f0000 00000000 S...L....?......
-  0x0000f4f0 50a87d00 026427ae f83f0000 00000000 P.}..d'..?......
-  0x0000f500 38b7ff6c 306219a5 f93f0000 00000000 8..l0b...?......
-  0x0000f510 e6e06478 d3313ff8 e5bf0000 00000000 ..dx.1?.........
-  0x0000f520 81beb8f3 068ca38b e93f0000 00000000 .........?......
-  0x0000f530 05529a41 ce88848f ec3f0000 00000000 .R.A.....?......
-  0x0000f540 fc40059a 95e9a3db ef3f0000 00000000 .@.......?......
-  0x0000f550 0ea0c2a8 2997a48d ee3f0000 00000000 ....)....?......
-  0x0000f560 488a261a 7e1d49d4 f43f0000 00000000 H.&.~.I..?......
-  0x0000f570 0aa5cb97 31336a8a f63f0000 00000000 ....13j..?......
-  0x0000f580 d468548c 6d6496d2 f73f0000 00000000 .hT.md...?......
-  0x0000f590 dede2023 64d7d1a7 fa3f0000 00000000 .. #d....?......
-  0x0000f5a0 d11bee10 d4b1f3f0 fa3f0000 00000000 .........?......
-  0x0000f5b0 79bffd42 c2ad13b7 fb3f0000 00000000 y..B.....?......
-  0x0000f5c0 b698d3d7 6ea464fa fd3f0000 00000000 ....n.d..?......
-  0x0000f5d0 98eb198b e0dd56ea fe3f0000 00000000 ......V..?......
-  0x0000f5e0 709d88d0 11d97db1 fe3f0000 00000000 p.....}..?......
-  0x0000f5f0 3d424dd5 ea4dbe9a fd3f0000 00000000 =BM..M...?......
-  0x0000f600 30ea9814 def4a79b fb3f0000 00000000 0........?......
-  0x0000f610 d67a6bd9 e1675c8a f83f0000 00000000 .zk..g\..?......
-  0x0000f620 13ad5b50 76a0a1b4 d53f0000 00000000 ..[Pv....?......
-  0x0000f630 5e3e1a77 f419cfb1 dd3f0000 00000000 ^>.w.....?......
-  0x0000f640 98f4f2f9 0d003d90 e43f0000 00000000 ......=..?......
-  0x0000f650 35762561 c3c662f9 e93f0000 00000000 5v%a..b..?......
-  0x0000f660 30a60b15 548111f8 ee3f0000 00000000 0...T....?......
-  0x0000f670 bf27afbd 2fe8f78e f33f0000 00000000 .'../....?......
-  0x0000f680 1b15d26e 373884b6 f63f0000 00000000 ...n78...?......
-  0x0000f690 02ce78e7 52dc6ae5 f83f0000 00000000 ..x.R.j..?......
-  0x0000f6a0 8838ad80 c92863d1 f93f0000 00000000 .8...(c..?......
-  0x0000f6b0 ff4bbaf5 772bf0d4 e83f0000 00000000 .K..w+...?......
-  0x0000f6c0 3f14f078 e21d6592 ec3f0000 00000000 ?..x..e..?......
-  0x0000f6d0 d4b94cf5 9c82cfdd ed3f0000 00000000 ..L......?......
-  0x0000f6e0 896ce87f 9387bea7 f23f0000 00000000 .l.......?......
-  0x0000f6f0 6acc3a74 79dcfdf3 f33f0000 00000000 j.:ty....?......
-  0x0000f700 705ccdc0 e4127a80 f63f0000 00000000 p\....z..?......
-  0x0000f710 f53342ee 5ab41580 f93f0000 00000000 .3B.Z....?......
-  0x0000f720 2928f2e7 198d2b94 fa3f0000 00000000 )(....+..?......
-  0x0000f730 595bd23a d39a2a9f f53f0000 00000000 Y[.:..*..?......
-  0x0000f740 63e23c62 003dcdda fc3f0000 00000000 c.<b.=...?......
-  0x0000f750 37da4799 0a675b9e fe3f0000 00000000 7.G..g[..?......
-  0x0000f760 0f1fb234 e1fe0989 ff3f0000 00000000 ...4.....?......
-  0x0000f770 aab7a253 0a8cb3ca fe3f0000 00000000 ...S.....?......
-  0x0000f780 55a2be6f f0185ace fd3f0000 00000000 U..o..Z..?......
-  0x0000f790 c67f0c41 a4d8bf8a fc3f0000 00000000 ...A.....?......
-  0x0000f7a0 f8a4352f 0939b5de f93f0000 00000000 ..5/.9...?......
-  0x0000f7b0 ccbd0f0b 7b29f8a1 f63f0000 00000000 ....{)...?......
-  0x0000f7c0 9cf50b07 7d07cc96 d93f0000 00000000 ....}....?......
-  0x0000f7d0 c5c5ef12 5fd77094 e13f0000 00000000 ...._.p..?......
-  0x0000f7e0 8801b994 1568d4f0 e73f0000 00000000 .....h...?......
-  0x0000f7f0 b6dbc6b6 150c32d0 ed3f0000 00000000 ......2..?......
-  0x0000f800 e5715721 6b7b18cf f23f0000 00000000 .qW!k{...?......
-  0x0000f810 e33257b5 0b9cb5ee f63f0000 00000000 .2W......?......
-  0x0000f820 a7e72495 dfe95e98 fa3f0000 00000000 ..$...^..?......
-  0x0000f830 4d3ae255 b47386bf fc3f0000 00000000 M:.U.s...?......
-  0x0000f840 feb875e6 aeadcdae fd3f0000 00000000 ..u......?......
-  0x0000f850 df0bbf0a 32e074f6 e33f0000 00000000 ....2.t..?......
-  0x0000f860 632a67c9 2b44a6d7 e63f0000 00000000 c*g.+D...?......
-  0x0000f870 632a67c9 2b44a6d7 ea3f0000 00000000 c*g.+D...?......
-  0x0000f880 632a67c9 2b44a6d7 ed3f0000 00000000 c*g.+D...?......
-  0x0000f890 a90f60fc 05e77ae2 ef3f0000 00000000 ..`...z..?......
-  0x0000f8a0 32ec71d2 83cf429a f33f0000 00000000 2.q...B..?......
-  0x0000f8b0 71d2a393 631737af f13f0000 00000000 q...c.7..?......
-  0x0000f8c0 20540af5 fc62dcb7 f73f0000 00000000  T...b...?......
-  0x0000f8d0 d0833673 7a3defa6 f83f0000 00000000 ..6sz=...?......
-  0x0000f8e0 039e9774 c126d88a fa3f0000 00000000 ...t.&...?......
-  0x0000f8f0 da57af0d 23e52e8c fc3f0000 00000000 .W..#....?......
-  0x0000f900 a3762e22 54cfcca8 fb3f0000 00000000 .v."T....?......
-  0x0000f910 88c4fc50 b38e70c5 fd3f0000 00000000 ...P..p..?......
-  0x0000f920 24fa38b8 4eec8b91 ff3f0000 00000000 $.8.N....?......
-  0x0000f930 4406e7b6 92d3bcb6 fe3f0000 00000000 D........?......
-  0x0000f940 e5cdf763 197c04f7 fc3f0000 00000000 ...c.|...?......
-  0x0000f950 ccbed6a6 5722278d fa3f0000 00000000 ....W"'..?......
-  0x0000f960 207ad7bd d734b992 d43f0000 00000000  z...4...?......
-  0x0000f970 381ce05e 04506e90 dc3f0000 00000000 8..^.Pn..?......
-  0x0000f980 7298976c 7cf852ea e23f0000 00000000 r..l|.R..?......
-  0x0000f990 f9da361d 4c4a92ca e83f0000 00000000 ..6.LJ...?......
-  0x0000f9a0 82cefcce c45480c9 ed3f0000 00000000 .....T...?......
-  0x0000f9b0 d495f15e 1cd642e8 f13f0000 00000000 ...^..B..?......
-  0x0000f9c0 91ab3032 1e354194 f53f0000 00000000 ..02.5A..?......
-  0x0000f9d0 1d062033 15fa59ba f73f0000 00000000 .. 3..Y..?......
-  0x0000f9e0 5a9b9555 5cd714aa f83f0000 00000000 Z..U\....?......
-  0x0000f9f0 6883fc4a b7384aad eabf0000 00000000 h..J.8J.........
-  0x0000fa00 c42aedec 144ecc8c ee3f0000 00000000 .*...N...?......
-  0x0000fa10 41a4bb1d e5c69cd8 ed3f0000 00000000 A........?......
-  0x0000fa20 7aed9414 3eb065ca f33f0000 00000000 z...>.e..?......
-  0x0000fa30 dac257b1 e668c29a f63f0000 00000000 ..W..h...?......
-  0x0000fa40 eddba30b 11f32580 f73f0000 00000000 ......%..?......
-  0x0000fa50 8e0fd4b5 6952fc87 f93f0000 00000000 ....iR...?......
-  0x0000fa60 09a6bdd5 10f697ee fb3f0000 00000000 .........?......
-  0x0000fa70 2e9ccca7 1c29e0b5 fd3f0000 00000000 .....)...?......
-  0x0000fa80 c383b534 6fc5d9b2 fe3f0000 00000000 ...4o....?......
-  0x0000fa90 efbabd4c f4389bf9 fe3f0000 00000000 ...L.8...?......
-  0x0000faa0 763bb62f e003cec2 fe3f0000 00000000 v;./.....?......
-  0x0000fab0 7d896723 6c0444da fd3f0000 00000000 }.g#l.D..?......
-  0x0000fac0 e12094a2 e92e6eaf fc3f0000 00000000 . ....n..?......
-  0x0000fad0 e005ed38 4518d6bf fa3f0000 00000000 ...8E....?......
-  0x0000fae0 a2a06886 fdbf0280 f83f0000 00000000 ..h......?......
-  0x0000faf0 78146da5 103b8d9d f43f0000 00000000 x.m..;...?......
-  0x0000fb00 f422ae2e 855c998d da3f0000 00000000 ."...\...?......
-  0x0000fb10 686af319 13f7628b e23f0000 00000000 hj....b..?......
-  0x0000fb20 a2eac452 dae423e2 e83f0000 00000000 ...R..#..?......
-  0x0000fb30 bb0449d3 ab1c7fc3 ee3f0000 00000000 ..I......?......
-  0x0000fb40 2d1e4adf 97b876c2 f33f0000 00000000 -.J...v..?......
-  0x0000fb50 9c6031fb 7d3426e0 f73f0000 00000000 .`1.}4&..?......
-  0x0000fb60 cac4a96b f0ab138f fb3f0000 00000000 ...k.....?......
-  0x0000fb70 caece5b2 05d2d7b3 fd3f0000 00000000 .........?......
-  0x0000fb80 4344644f 822724a4 fe3f0000 00000000 CDdO.'$..?......
-  0x0000fb90 abfe5717 a8fff9fb e73f0000 00000000 ..W......?......
-  0x0000fba0 167f0c90 c3df3bad eb3f0000 00000000 ......;..?......
-  0x0000fbb0 f929d336 d2df3c83 ed3f0000 00000000 .).6..<..?......
-  0x0000fbc0 49fcb8bf ba457fc6 f13f0000 00000000 I....E...?......
-  0x0000fbd0 9f7ad1fb 50cac386 f33f0000 00000000 .z..P....?......
-  0x0000fbe0 3934b2c0 21006cb2 f53f0000 00000000 94..!.l..?......
-  0x0000fbf0 96a37a7e e6c05d99 f83f0000 00000000 ..z~..]..?......
-  0x0000fc00 23df5dca c8b981ee f83f0000 00000000 #.]......?......
-  0x0000fc10 786bb29c ef1342b4 fa3f0000 00000000 xk....B..?......
-  0x0000fc20 a33a4a2e df982b88 fd3f0000 00000000 .:J...+..?......
-  0x0000fc30 8609f031 50084da7 fe3f0000 00000000 ...1P.M..?......
-  0x0000fc40 532cd2df 4814bc85 ff3f0000 00000000 S,..H....?......
-  0x0000fc50 512f4fa0 36f271c3 fe3f0000 00000000 Q/O.6.q..?......
-  0x0000fc60 aafe96e1 7979c2c5 fd3f0000 00000000 ....yy...?......
-  0x0000fc70 60342a7e 15ba9684 fc3f0000 00000000 `4*~.....?......
-  0x0000fc80 9040ed54 cb6897d4 f93f0000 00000000 .@.T.h...?......
-  0x0000fc90 f42e380f 4ea99c9a f63f0000 00000000 ..8.N....?......
-  0x0000fca0 8c015fe9 1141aed8 d63f0000 00000000 .._..A...?......
-  0x0000fcb0 8685b9a1 0d884bd5 de3f0000 00000000 ......K..?......
-  0x0000fcc0 502986b9 5d4506ad e53f0000 00000000 P)..]E...?......
-  0x0000fcd0 353ffcfd 67119495 eb3f0000 00000000 5?..g....?......
-  0x0000fce0 fda3d369 efc6c994 f03f0000 00000000 ...i.....?......
-  0x0000fcf0 11778411 2d4c80ab f43f0000 00000000 .w..-L...?......
-  0x0000fd00 f845c0b6 f228f1da f73f0000 00000000 .E...(...?......
-  0x0000fd10 7971ad2b df019a89 fa3f0000 00000000 yq.+.....?......
-  0x0000fd20 3c4f7d45 14f52cfb fa3f0000 00000000 <O}E..,..?......
-  0x0000fd30 08398824 797e2dd2 f03f0000 00000000 .9.$y~-..?......
-  0x0000fd40 77b53f92 91a60ac5 f43f0000 00000000 w.?......?......
-  0x0000fd50 c8bef75f bf5169ac f73f0000 00000000 ..._.Qi..?......
-  0x0000fd60 ae0ef7a7 e46dc7ba f93f0000 00000000 .....m...?......
-  0x0000fd70 034bf97d 6b92158c fb3f0000 00000000 .K.}k....?......
-  0x0000fd80 509ff870 a9ba179a fc3f0000 00000000 P..p.....?......
-  0x0000fd90 18da7933 8d1b6980 fd3f0000 00000000 ..y3..i..?......
-  0x0000fda0 8c610af9 906c19a5 fd3f0000 00000000 .a...l...?......
-  0x0000fdb0 0a0f6721 1ea04aa0 e13f0000 00000000 ..g!..J..?......
-  0x0000fdc0 da71f9c8 ef5936fe e83f0000 00000000 .q...Y6..?......
-  0x0000fdd0 57f1b853 b95fad9e ef3f0000 00000000 W..S._...?......
-  0x0000fde0 9b9393fa 0525a2c7 f43f0000 00000000 .....%...?......
-  0x0000fdf0 682c30f5 dac09486 f93f0000 00000000 h,0......?......
-  0x0000fe00 d06e689f 48b7a5be fc3f0000 00000000 .nh.H....?......
-  0x0000fe10 54c2803e a79cb0f2 ff3f0000 00000000 T..>.....?......
-  0x0000fe20 62847e2d b495f0fe dabf0000 00000000 b.~-............
-  0x0000fe30 4ae31e22 477034bf dc3f0000 00000000 J.."Gp4..?......
-  0x0000fe40 b8bfb5ed 28312181 e33f0000 00000000 ....(1!..?......
-  0x0000fe50 9d9cebcc e8aaafc3 e43f0000 00000000 .........?......
-  0x0000fe60 1620a4df b5e4d0d2 e93f0000 00000000 . .......?......
-  0x0000fe70 fce79ab3 58a831a2 eb3f0000 00000000 ....X.1..?......
-  0x0000fe80 299a2c67 1aba10b1 ef3f0000 00000000 ).,g.....?......
-  0x0000fe90 5e12ed3f 930e948b f13f0000 00000000 ^..?.....?......
-  0x0000fea0 2cad404c 8e2ee7a1 f43f0000 00000000 ,.@L.....?......
-  0x0000feb0 66626052 d4222185 f63f0000 00000000 fb`R."!..?......
-  0x0000fec0 60620e76 5a86149c f83f0000 00000000 `b.vZ....?......
-  0x0000fed0 86d9cb6e 91fe7d8b fa3f0000 00000000 ...n..}..?......
-  0x0000fee0 9cc5573a b90ab087 fb3f0000 00000000 ..W:.....?......
-  0x0000fef0 b4d29da1 4ea33295 fd3f0000 00000000 ....N.2..?......
-  0x0000ff00 a2de476e 12870eb7 fb3f0000 00000000 ..Gn.....?......
-  0x0000ff10 6c5b3eda 22b3bd89 ff3f0000 00000000 l[>."....?......
-  0x0000ff20 3bb83945 fa7585b6 fe3f0000 00000000 ;.9E.u...?......
-  0x0000ff30 8bd2faec 1e0639b2 ff3f0000 00000000 ......9..?......
-  0x0000ff40 0f6e4e91 7e5da1ed fd3f0000 00000000 .nN.~]...?......
-  0x0000ff50 9e3d8ff7 55eb86cd cf3f0000 00000000 .=..U....?......
-  0x0000ff60 e25b436e f4b3b18b d83f0000 00000000 .[Cn.....?......
-  0x0000ff70 97d7d761 12c76e9f df3f0000 00000000 ...a..n..?......
-  0x0000ff80 8fcf75bb d97acdc6 e53f0000 00000000 ..u..z...?......
-  0x0000ff90 3ec38038 def0a693 eb3f0000 00000000 >..8.....?......
-  0x0000ffa0 38d2671b 5f27ae85 f03f0000 00000000 8.g._'...?......
-  0x0000ffb0 056649b6 ea671891 f43f0000 00000000 .fI..g...?......
-  0x0000ffc0 454308e1 fd0e3cb2 f73f0000 00000000 EC....<..?......
-  0x0000ffd0 f7bb9485 72c8bbda f93f0000 00000000 ....r....?......
-  0x0000ffe0 374c7a4c b6faeac4 fa3f0000 00000000 7LzL.....?......
-  0x0000fff0 f415700c 052153fb dc3f0000 00000000 ..p..!S..?......
-  0x00010000 b90dc627 a3f4139d df3f0000 00000000 ...'.....?......
-  0x00010010 de52b056 6070fbd7 e43f0000 00000000 .R.V`p...?......
-  0x00010020 38646c4f e1c5e58b e73f0000 00000000 8dlO.....?......
-  0x00010030 201d2f28 4863a38e eb3f0000 00000000  ./(Hc...?......
-  0x00010040 32cdb5f8 ed71e4c3 ed3f0000 00000000 2....q...?......
-  0x00010050 3bcf3321 856d32b2 f03f0000 00000000 ;.3!.m2..?......
-  0x00010060 f3cd629c 88cc3e88 f33f0000 00000000 ..b...>..?......
-  0x00010070 f1253c69 fa812fc8 f43f0000 00000000 .%<i../..?......
-  0x00010080 efebf647 2b0d6dc3 f73f0000 00000000 ...G+.m..?......
-  0x00010090 cde51817 4b5feec2 f63f0000 00000000 ....K_...?......
-  0x000100a0 dbbcf33d 46bd6286 fb3f0000 00000000 ...=F.b..?......
-  0x000100b0 54281c76 6155148b fb3f0000 00000000 T(.vaU...?......
-  0x000100c0 6a870585 bd610284 fd3f0000 00000000 j....a...?......
-  0x000100d0 c9ca55b3 efbaf8a3 fe3f0000 00000000 ..U......?......
-  0x000100e0 2ab71e5f 5b36628a fd3f0000 00000000 *.._[6b..?......
-  0x000100f0 1800e36e 1c2647ab fe3f0000 00000000 ...n.&G..?......
-  0x00010100 fd9f2372 3c1b978a fe3f0000 00000000 ..#r<....?......
-  0x00010110 fbff3850 fa91bedd fb3f0000 00000000 ..8P.....?......
-  0x00010120 43b9500b ace223fc cf3f0000 00000000 C.P...#..?......
-  0x00010130 ecddb0ef 106460ab d83f0000 00000000 .....d`..?......
-  0x00010140 96108fe1 577e97c3 df3f0000 00000000 ....W~...?......
-  0x00010150 14b3f1ef da06e4f3 e53f0000 00000000 .........?......
-  0x00010160 c2e91b65 adab23b5 eb3f0000 00000000 ...e..#..?......
-  0x00010170 a264420b c2acffa3 f03f0000 00000000 .dB......?......
-  0x00010180 9f096387 36b000b2 f43f0000 00000000 ..c.6....?......
-  0x00010190 7e890bbb eb6aa8da f73f0000 00000000 ~....j...?......
-  0x000101a0 0a047e66 eac22b86 fa3f0000 00000000 ..~f..+..?......
-  0x000101b0 a87ad011 941894f1 fa3f0000 00000000 .z.......?......
-  0x000101c0 c06cdcb9 a946a5a6 e0bf0000 00000000 .l...F..........
-  0x000101d0 28dfa082 d49dd091 e33f0000 00000000 (........?......
-  0x000101e0 3b877606 44d6bde7 e73f0000 00000000 ;.v.D....?......
-  0x000101f0 39d2fb15 362f00dd ea3f0000 00000000 9...6/...?......
-  0x00010200 5da50082 a0a110dc ed3f0000 00000000 ]........?......
-  0x00010210 8e7603b6 2652a9f8 f03f0000 00000000 .v..&R...?......
-  0x00010220 550b1807 4ab68c8c f23f0000 00000000 U...J....?......
-  0x00010230 14c191e7 c41a9afc f53f0000 00000000 .........?......
-  0x00010240 21755a36 d8efa08b f53f0000 00000000 !uZ6.....?......
-  0x00010250 78bdd436 257f32d8 f93f0000 00000000 x..6%.2..?......
-  0x00010260 34c39aa4 9a7f2c86 fb3f0000 00000000 4.....,..?......
-  0x00010270 40065fd3 2e44a38c fb3f0000 00000000 @._..D...?......
-  0x00010280 8fbe7a30 04c84d83 fe3f0000 00000000 ..z0..M..?......
-  0x00010290 e407069e 3239b7c9 fe3f0000 00000000 ....29...?......
-  0x000102a0 3f8b05be f1e033b0 fc3f0000 00000000 ?.....3..?......
-  0x000102b0 9729e905 e8cbf8fb fe3f0000 00000000 .).......?......
-  0x000102c0 1b5b2eb3 ef7c0cbd ff3f0000 00000000 .[...|...?......
-  0x000102d0 39693413 c4e0bcb0 fd3f0000 00000000 9i4......?......
-  0x000102e0 427860f1 966efcc9 fa3f0000 00000000 Bx`..n...?......
-  0x000102f0 8e89c909 6cfec384 d33f0000 00000000 ....l....?......
-  0x00010300 fdf64ddd da6d7ab4 db3f0000 00000000 ..M..mz..?......
-  0x00010310 f538bf45 3dc3facd e23f0000 00000000 .8.E=....?......
-  0x00010320 d84f4381 14fc6b80 e93f0000 00000000 .OC...k..?......
-  0x00010330 943b747d b771c2be ee3f0000 00000000 .;t}.q...?......
-  0x00010340 f78a1fd3 8767b5ac f33f0000 00000000 .....g...?......
-  0x00010350 a7b6ef30 e4d074bb f73f0000 00000000 ...0..t..?......
-  0x00010360 b897d899 444b45e6 fa3f0000 00000000 ....DKE..?......
-  0x00010370 77dd3922 adf34b8d fd3f0000 00000000 w.9"..K..?......
-  0x00010380 905b3a7b fb9968fe fd3f0000 00000000 .[:{..h..?......
-  0x00010390 350abd48 22208bf0 d43f0000 00000000 5..H" ...?......
-  0x000103a0 f07c704d d78f7ea3 dd3f0000 00000000 .|pM..~..?......
-  0x000103b0 a9d45858 5f8c98ba e43f0000 00000000 ..XX_....?......
-  0x000103c0 5c6d9513 db65ace8 ea3f0000 00000000 \m...e...?......
-  0x000103d0 b5d337c9 52e4ceac f03f0000 00000000 ..7.R....?......
-  0x000103e0 13bd536b bcb6749c f53f0000 00000000 ..Sk..t..?......
-  0x000103f0 6a686d42 5ed7d0a9 f93f0000 00000000 jhmB^....?......
-  0x00010400 bd3fca0d efe299d0 fc3f0000 00000000 .?.......?......
-  0x00010410 21ee58b9 1db177e6 ff3f0000 00000000 !.X...w..?......
-  0x00010420 76e8a504 8da66082 e13f0000 00000000 v.....`..?......
-  0x00010430 85a53aa5 5ebbac92 e43f0000 00000000 ..:.^....?......
-  0x00010440 26d22c3a 2858cf87 e83f0000 00000000 &.,:(X...?......
-  0x00010450 e64e894e 36ea57b7 eb3f0000 00000000 .N.N6.W..?......
-  0x00010460 5e6a4560 0e8ba3fb ec3f0000 00000000 ^jE`.....?......
-  0x00010470 8e1a7332 d4119e95 f13f0000 00000000 ..s2.....?......
-  0x00010480 afcb0d76 00e6f9ce f13f0000 00000000 ...v.....?......
-  0x00010490 2bd2d489 039c8c9e f53f0000 00000000 +........?......
-  0x000104a0 4803c184 ccb77da3 f73f0000 00000000 H.....}..?......
-  0x000104b0 f91c995a df9c28c1 f53f0000 00000000 ...Z..(..?......
-  0x000104c0 75021c7c 4f93a58a fa3f0000 00000000 u..|O....?......
-  0x000104d0 5be82ba3 cbacdfc7 fb3f0000 00000000 [.+......?......
-  0x000104e0 1bfcecf4 0aefcfe5 fb3f0000 00000000 .........?......
-  0x000104f0 3009c759 332cf7b7 f53f0000 00000000 0..Y3,...?......
-  0x00010500 38e15bd3 256ccdb0 fc3f0000 00000000 8.[.%l...?......
-  0x00010510 2a2d8d4a b502b882 fd3f0000 00000000 *-.J.....?......
-  0x00010520 e1bf29fc 0c3b27c9 fc3f0000 00000000 ..)..;'..?......
-  0x00010530 d141ec3b 0b0eb5b6 fb3f0000 00000000 .A.;.....?......
-  0x00010540 e4383f45 0b0e4fba f93f0000 00000000 .8?E..O..?......
-  0x00010550 59a454af b49a9ba5 f63f0000 00000000 Y.T......?......
-  0x00010560 d6bbaaaa ed7ad9ba d83f0000 00000000 .....z...?......
-  0x00010570 306955cd 22760bd8 e03f0000 00000000 0iU."v...?......
-  0x00010580 5e2f2f1e dddeeccd e73f0000 00000000 ^//......?......
-  0x00010590 c877f750 822b0ad1 ed3f0000 00000000 .w.P.+...?......
-  0x000105a0 cd7a3169 d74311f4 f23f0000 00000000 .z1i.C...?......
-  0x000105b0 3d5f40b1 c49278a5 f73f0000 00000000 =_@...x..?......
-  0x000105c0 fedd8aad 2cf90bfb fa3f0000 00000000 ....,....?......
-  0x000105d0 f6554592 94a6e5c2 fd3f0000 00000000 .UE......?......
-  0x000105e0 473b548d 28a823f8 fe3f0000 00000000 G;T.(.#..?......
-  0x000105f0 20599851 aa08d3c3 d03f0000 00000000  Y.Q.....?......
-  0x00010600 948c75c3 e36f1985 d93f0000 00000000 ..u..o...?......
-  0x00010610 33a4e7ce 5af6e797 e03f0000 00000000 3...Z....?......
-  0x00010620 e90d8d2d 8adc6abd e63f0000 00000000 ...-..j..?......
-  0x00010630 008634a3 e07fae8c ec3f0000 00000000 ..4......?......
-  0x00010640 8d95a230 e222bdfe f03f0000 00000000 ...0."...?......
-  0x00010650 1b442ba7 45dd3e8a f53f0000 00000000 .D+.E.>..?......
-  0x00010660 e12551f1 a203d2a9 f83f0000 00000000 .%Q......?......
-  0x00010670 85ba757e 894a68d0 fa3f0000 00000000 ..u~.Jh..?......
-  0x00010680 e3d3c47b a2239fbb fb3f0000 00000000 ...{.#...?......
-  0x00010690 cfa8b41e ecd26a93 e8bf0000 00000000 ......j.........
-  0x000106a0 02d36126 a78745b8 ea3f0000 00000000 ..a&..E..?......
-  0x000106b0 5d932d1f 682180e2 ee3f0000 00000000 ].-.h!...?......
-  0x000106c0 4a99e285 5b6d1499 f13f0000 00000000 J...[m...?......
-  0x000106d0 a6e217e0 a378b1df f33f0000 00000000 .....x...?......
-  0x000106e0 0e7222dc 350495b2 f63f0000 00000000 .r".5....?......
-  0x000106f0 b1197059 f68640f7 f63f0000 00000000 ..pY..@..?......
-  0x00010700 f5edb989 52e4f6a9 fa3f0000 00000000 ....R....?......
-  0x00010710 e17439ea 450dfbe1 f93f0000 00000000 .t9.E....?......
-  0x00010720 ddc0b044 d47186e7 fc3f0000 00000000 ...D.q...?......
-  0x00010730 094b029f 7524e5eb fd3f0000 00000000 .K..u$...?......
-  0x00010740 911aae56 f4d779f1 f93f0000 00000000 ...V..y..?......
-  0x00010750 a06e8687 750ec4a0 ff3f0000 00000000 .n..u....?......
-  0x00010760 480a68e9 1212f5a8 fe3f0000 00000000 H.h......?......
-  0x00010770 06d5eced db742a87 fc3f0000 00000000 .....t*..?......
-  0x00010780 2df76a31 91e8d7dd da3f0000 00000000 -.j1.....?......
-  0x00010790 01d22f22 6b35eaaf e23f0000 00000000 ../"k5...?......
-  0x000107a0 688f179b edf79bdb e83f0000 00000000 h........?......
-  0x000107b0 9c91a1ec a171258a ee3f0000 00000000 .....q%..?......
-  0x000107c0 a06ec423 7d9942ba f23f0000 00000000 .n.#}.B..?......
-  0x000107d0 3d86aaea 2f8ced83 f63f0000 00000000 =.../....?......
-  0x000107e0 e811958e c7e626b1 f83f0000 00000000 ......&..?......
-  0x000107f0 4b9e3dbe 4efdf0a7 f93f0000 00000000 K.=.N....?......
-  0x00010800 61935f59 f84cb89b ea3f0000 00000000 a._Y.L...?......
-  0x00010810 f5a0334e 59434188 ed3f0000 00000000 ..3NYCA..?......
-  0x00010820 1415fa77 c46b4999 f03f0000 00000000 ...w.kI..?......
-  0x00010830 aeba873c 228f30a8 f33f0000 00000000 ...<".0..?......
-  0x00010840 49b752ff 89510ead f33f0000 00000000 I.R..Q...?......
-  0x00010850 6a56e6cb f6e149fa f73f0000 00000000 jV....I..?......
-  0x00010860 d374e060 893f52d4 f83f0000 00000000 .t.`.?R..?......
-  0x00010870 15be5c8b 8cc464c3 fa3f0000 00000000 ..\...d..?......
-  0x00010880 2d6a2ec1 88cb51cf fc3f0000 00000000 -j....Q..?......
-  0x00010890 55b03173 4e415ce1 fc3f0000 00000000 U.1sNA\..?......
-  0x000108a0 659148e9 a4f468cb fc3f0000 00000000 e.H...h..?......
-  0x000108b0 e5926b11 4b508dd0 fe3f0000 00000000 ..k.KP...?......
-  0x000108c0 e919a3a7 56f485a4 fe3f0000 00000000 ....V....?......
-  0x000108d0 576d5da5 976beadf fc3f0000 00000000 Wm]..k...?......
-  0x000108e0 adeab32a 6456e7ff f93f0000 00000000 ...*dV...?......
-  0x000108f0 94cc4496 0b4da596 dc3f0000 00000000 ..D..M...?......
-  0x00010900 731c5160 3028eaee e33f0000 00000000 s.Q`0(...?......
-  0x00010910 346365f4 e0ea2095 ea3f0000 00000000 4ce... ..?......
-  0x00010920 27f0ee28 12c09ebb ef3f0000 00000000 '..(.....?......
-  0x00010930 fc65087d d301f7fc f33f0000 00000000 .e.}.....?......
-  0x00010940 f36f3ebb ebc02cb3 f73f0000 00000000 .o>...,..?......
-  0x00010950 d01c2ee1 134498f0 f93f0000 00000000 .....D...?......
-  0x00010960 62d01690 43ec15e4 fa3f0000 00000000 b...C....?......
-  0x00010970 36ef4061 5924afa3 edbf0000 00000000 6.@aY$..........
-  0x00010980 1d0d698d e40825b8 f03f0000 00000000 ..i...%..?......
-  0x00010990 c575f5a7 cba8c1ff f13f0000 00000000 .u.......?......
-  0x000109a0 4179d32c 8390a894 f63f0000 00000000 Ay.,.....?......
-  0x000109b0 cbfa7c00 780651bf f73f0000 00000000 ..|.x.Q..?......
-  0x000109c0 aecf25ed d62c99e4 f83f0000 00000000 ..%..,...?......
-  0x000109d0 a36246a2 a2360ed8 fb3f0000 00000000 .bF..6...?......
-  0x000109e0 b5854785 309909e5 fc3f0000 00000000 ..G.0....?......
-  0x000109f0 a737fa5a 475b12ff fb3f0000 00000000 .7.ZG[...?......
-  0x00010a00 abc6061a 9d9d3fc1 fd3f0000 00000000 ......?..?......
-  0x00010a10 b3dcf42d 9147dd99 ff3f0000 00000000 ...-.G...?......
-  0x00010a20 f85885aa 7d1775dd fe3f0000 00000000 .X..}.u..?......
-  0x00010a30 cb897b1e 86250dc4 fd3f0000 00000000 ..{..%...?......
-  0x00010a40 eef83129 9c6b3bc6 fb3f0000 00000000 ..1).k;..?......
-  0x00010a50 d4c0815d 6ed134b0 f83f0000 00000000 ...]n.4..?......
-  0x00010a60 9fe749bf 69a8629f e03f0000 00000000 ..I.i.b..?......
-  0x00010a70 57355fb5 1777c6fc e73f0000 00000000 W5_..w...?......
-  0x00010a80 16bda88e 0fbec79d ee3f0000 00000000 .........?......
-  0x00010a90 1f2ea7d0 353e81c6 f33f0000 00000000 ....5>...?......
-  0x00010aa0 cca25bb3 2dfed185 f83f0000 00000000 ..[.-....?......
-  0x00010ab0 f7b65498 8fd191bd fb3f0000 00000000 ..T......?......
-  0x00010ac0 70838a5b dd868dfe fd3f0000 00000000 p..[.....?......
-  0x00010ad0 510c6083 8e6651f1 fe3f0000 00000000 Q.`..fQ..?......
-  0x00010ae0 ff15ab2d be5fd1a9 debf0000 00000000 ...-._..........
-  0x00010af0 3fb3f567 c6339794 e13f0000 00000000 ?..g.3...?......
-  0x00010b00 97ea8177 242927ec e53f0000 00000000 ...w$)'..?......
-  0x00010b10 ac6390b5 782a35e1 e83f0000 00000000 .c..x*5..?......
-  0x00010b20 318127f5 d40cbae5 eb3f0000 00000000 1.'......?......
-  0x00010b30 424dc116 537c1781 ef3f0000 00000000 BM..S|...?......
-  0x00010b40 e91f9ac1 9b8afaa0 f03f0000 00000000 .........?......
-  0x00010b50 0b279dfc d667ab89 f43f0000 00000000 .'...g...?......
-  0x00010b60 e03b2836 bb2f05aa f23f0000 00000000 .;(6./...?......
-  0x00010b70 7cdd0468 26d8df83 f83f0000 00000000 |..h&....?......
-  0x00010b80 5332aa29 eec3cc8b f93f0000 00000000 S2.).....?......
-  0x00010b90 7cd14977 35c6bb9a fa3f0000 00000000 |.Iw5....?......
-  0x00010ba0 b5ac2521 71d1dcba fc3f0000 00000000 ..%!q....?......
-  0x00010bb0 4856b6a2 2db44cac fc3f0000 00000000 HV..-.L..?......
-  0x00010bc0 312e2bec fed60fa3 fd3f0000 00000000 1.+......?......
-  0x00010bd0 15e4e622 1a7a2097 ff3f0000 00000000 ...".z ..?......
-  0x00010be0 f666c744 af4904c0 fe3f0000 00000000 .f.D.I...?......
-  0x00010bf0 12c174d3 f2a13b82 fd3f0000 00000000 ..t...;..?......
-  0x00010c00 3901aaf1 f06fd694 fa3f0000 00000000 9....o...?......
-  0x00010c10 a4ae0064 e72d32ca cd3f0000 00000000 ...d.-2..?......
-  0x00010c20 b376f845 331b6e89 d63f0000 00000000 .v.E3.n..?......
-  0x00010c30 791feddc e748d99c dd3f0000 00000000 y....H...?......
-  0x00010c40 2dc67f89 bda394c3 e33f0000 00000000 -........?......
-  0x00010c50 d51bf8df 87534291 e93f0000 00000000 .....SB..?......
-  0x00010c60 166099d0 44828383 ee3f0000 00000000 .`..D....?......
-  0x00010c70 30a6bf8a 4566be8e f23f0000 00000000 0...Ef...?......
-  0x00010c80 3a754cf7 538e58af f53f0000 00000000 :uL.S.X..?......
-  0x00010c90 86b0eec3 ac3f30d7 f73f0000 00000000 .....?0..?......
-  0x00010ca0 5bcfa129 84f5b9c1 f83f0000 00000000 [..).....?......
-  0x00010cb0 11f0523e 20617fe6 e03f0000 00000000 ..R> a...?......
-  0x00010cc0 0aa70e23 a2a6a781 e43f0000 00000000 ...#.....?......
-  0x00010cd0 12baeb40 2c051af0 e73f0000 00000000 ...@,....?......
-  0x00010ce0 cc50d2ab 4a9011a2 eb3f0000 00000000 .P..J....?......
-  0x00010cf0 0b3d4fa0 4efaacf9 ec3f0000 00000000 .=O.N....?......
-  0x00010d00 128dee44 5c9aea8b f13f0000 00000000 ...D\....?......
-  0x00010d10 b2382a9f 4f2d5af9 f03f0000 00000000 .8*.O-Z..?......
-  0x00010d20 e2c65858 abe9b3b9 f53f0000 00000000 ..XX.....?......
-  0x00010d30 a8020a5c 4c21199b f73f0000 00000000 ...\L!...?......
-  0x00010d40 8c9df8fe 10462bb6 f73f0000 00000000 .....F+..?......
-  0x00010d50 ea9f25f7 0bea3df4 fa3f0000 00000000 ..%...=..?......
-  0x00010d60 c4ca01fa aa6eb4f4 fb3f0000 00000000 .....n...?......
-  0x00010d70 f6b1458e 1646cffe f73f0000 00000000 ..E..F...?......
-  0x00010d80 71b55fea 2af93dcc fd3f0000 00000000 q._.*.=..?......
-  0x00010d90 64d9fb77 a49938df fe3f0000 00000000 d..w..8..?......
-  0x00010da0 eceefe3b d67005b5 fe3f0000 00000000 ...;.p...?......
-  0x00010db0 f0624671 13ff1e9f fd3f0000 00000000 .bFq.....?......
-  0x00010dc0 7d571ffa 19d081a0 fb3f0000 00000000 }W.......?......
-  0x00010dd0 376aff88 3347ac8e f83f0000 00000000 7j..3G...?......
-  0x00010de0 46214c5d 17df2dcf cf3f0000 00000000 F!L]..-..?......
-  0x00010df0 9dbe69e1 a12dd18c d83f0000 00000000 ..i..-...?......
-  0x00010e00 578cd9c9 6cdfb6a0 df3f0000 00000000 W...l....?......
-  0x00010e10 3162ca5f 129866c8 e53f0000 00000000 1b._..f..?......
-  0x00010e20 d4df156d f5cad694 eb3f0000 00000000 ...m.....?......
-  0x00010e30 7eed6e39 d340c186 f03f0000 00000000 ~.n9.@...?......
-  0x00010e40 eda763c9 0bff4292 f43f0000 00000000 ..c...B..?......
-  0x00010e50 fc3fd518 8dd8aab3 f73f0000 00000000 .?.......?......
-  0x00010e60 577895a5 a6e97ddc f93f0000 00000000 Wx....}..?......
-  0x00010e70 3189aefd ff3680c6 fa3f0000 00000000 1....6...?......
-  0x00010e80 0f65cf71 1caf3887 e4bf0000 00000000 .e.q..8.........
-  0x00010e90 f52a7d1c c7f0edb9 e73f0000 00000000 .*}......?......
-  0x00010ea0 cdafee38 4e2bb4b5 ea3f0000 00000000 ...8N+...?......
-  0x00010eb0 49360b00 043906b7 ee3f0000 00000000 I6...9...?......
-  0x00010ec0 2029b3aa 8e9fa78a ee3f0000 00000000  ).......?......
-  0x00010ed0 7ef60b20 43c847c3 f33f0000 00000000 ~.. C.G..?......
-  0x00010ee0 bfa19c76 53221cd5 f53f0000 00000000 ...vS"...?......
-  0x00010ef0 5c745f3a 25f753bb f43f0000 00000000 \t_:%.S..?......
-  0x00010f00 2a312043 96e2d6c1 f93f0000 00000000 *1 C.....?......
-  0x00010f10 70c53856 36a5da98 fb3f0000 00000000 p.8V6....?......
-  0x00010f20 9587e023 1397f2a8 fb3f0000 00000000 ...#.....?......
-  0x00010f30 3df6cdc3 89d79edb fb3f0000 00000000 =........?......
-  0x00010f40 59942d93 819fca8b fe3f0000 00000000 Y.-......?......
-  0x00010f50 7b58d8a7 02990190 ff3f0000 00000000 {X.......?......
-  0x00010f60 b63d3f3e 76a90bda fe3f0000 00000000 .=?>v....?......
-  0x00010f70 560de24b 09568ce0 fd3f0000 00000000 V..K.V...?......
-  0x00010f80 9f485019 b607ce97 fc3f0000 00000000 .HP......?......
-  0x00010f90 a2cdefb2 59bb26f4 f93f0000 00000000 ....Y.&..?......
-  0x00010fa0 bb4f513c 418890b1 f63f0000 00000000 .OQ<A....?......
-  0x00010fb0 0355e75f ba851488 d43f0000 00000000 .U._.....?......
-  0x00010fc0 91775e5a c9e5fbb8 dc3f0000 00000000 .w^Z.....?......
-  0x00010fd0 993ac202 e9361fd3 e33f0000 00000000 .:...6...?......
-  0x00010fe0 a031f18d 56c0a083 ea3f0000 00000000 .1..V....?......
-  0x00010ff0 55f51c05 539f85c3 ef3f0000 00000000 U...S....?......
-  0x00011000 8d8e4580 403705b1 f43f0000 00000000 ..E.@7...?......
-  0x00011010 d8b2d54f f0e122c0 f83f0000 00000000 ...O.."..?......
-  0x00011020 7af68768 adfe04ec fb3f0000 00000000 z..h.....?......
-  0x00011030 800b8ec5 0b01d390 fe3f0000 00000000 .........?......
-  0x00011040 498071c4 38496182 ff3f0000 00000000 I.q.8Ia..?......
-  0x00011050 61d76a87 4a6078f9 db3f0000 00000000 a.j.J`x..?......
-  0x00011060 9dc6a294 2e3ceb9b de3f0000 00000000 .....<...?......
-  0x00011070 18d15f0c c07263d6 e33f0000 00000000 .._..rc..?......
-  0x00011080 e4f8607c 9981dd8a e63f0000 00000000 ..`|.....?......
-  0x00011090 daa03788 330a5e8e ea3f0000 00000000 ..7.3.^..?......
-  0x000110a0 dc77f821 1e866cc3 ec3f0000 00000000 .w.!..l..?......
-  0x000110b0 f03c3771 90233fb4 ef3f0000 00000000 .<7q.#?..?......
-  0x000110c0 fa66485e 57067789 f23f0000 00000000 .fH^W.w..?......
-  0x000110d0 aa545627 67b5f8d0 f33f0000 00000000 .TV'g....?......
-  0x000110e0 68f138c8 c88485c9 f63f0000 00000000 h.8......?......
-  0x000110f0 a6b00023 b83286f5 f53f0000 00000000 ...#.2...?......
-  0x00011100 c2b0bff0 82316491 fa3f0000 00000000 .....1d..?......
-  0x00011110 0e6e33fa 0230b484 fa3f0000 00000000 .n3..0...?......
-  0x00011120 d61a5242 c8d114a3 fc3f0000 00000000 ..RB.....?......
-  0x00011130 d64b3646 716679ad fd3f0000 00000000 .K6Fqfy..?......
-  0x00011140 4b36b437 bcdf09c0 fa3f0000 00000000 K6.7.....?......
-  0x00011150 237444e6 29fa3fce fe3f0000 00000000 #tD.).?..?......
-  0x00011160 7c7137c3 ba003886 fe3f0000 00000000 |q7...8..?......
-  0x00011170 2c4ff2d1 2a01c0d6 fb3f0000 00000000 ,O..*....?......
-  0x00011180 3b07c493 2df1f381 cd3f0000 00000000 ;...-....?......
-  0x00011190 d579def4 d99ba7b0 d53f0000 00000000 .y.......?......
-  0x000111a0 e864fc21 f1a29dc9 dc3f0000 00000000 .d.!.....?......
-  0x000111b0 94e3abf1 97fb66fb e23f0000 00000000 ......f..?......
-  0x000111c0 2e86bc6c 07ddb7ba e83f0000 00000000 ...l.....?......
-  0x000111d0 b7964c0b f7b80ca9 ed3f0000 00000000 ..L......?......
-  0x000111e0 c30661cd 73267cb7 f13f0000 00000000 ..a.s&|..?......
-  0x000111f0 d1e59c06 e26c64e1 f43f0000 00000000 .....ld..?......
-  0x00011200 e2f90af2 c6a14d8a f73f0000 00000000 ......M..?......
-  0x00011210 79cb7059 3dd204f9 f73f0000 00000000 y.pY=....?......
-  0x00011220 77d7faa8 daf076cc ebbf0000 00000000 w.....v.........
-  0x00011230 66321afe f5ce05e6 ee3f0000 00000000 f2.......?......
-  0x00011240 55f803d4 2aecbc9f f03f0000 00000000 U...*....?......
-  0x00011250 b0d07796 be05b2b9 f43f0000 00000000 ..w......?......
-  0x00011260 dbea7077 2f8e44ba f53f0000 00000000 ..pw/.D..?......
-  0x00011270 5662d276 d6ccb082 f83f0000 00000000 Vb.v.....?......
-  0x00011280 16519281 df4ecaaa fa3f0000 00000000 .Q...N...?......
-  0x00011290 10df65ec 493c62d5 fa3f0000 00000000 ..e.I<b..?......
-  0x000112a0 ac6091ce 5677beee fb3f0000 00000000 .`..Vw...?......
-  0x000112b0 429ca51a 885e568c fe3f0000 00000000 B....^V..?......
-  0x000112c0 faa790ac 684a8c8a ff3f0000 00000000 ....hJ...?......
-  0x000112d0 7cf88b03 a1e65dbf fe3f0000 00000000 |.....]..?......
-  0x000112e0 9266544a ea1190a6 fd3f0000 00000000 .fTJ.....?......
-  0x000112f0 ba8ce1fc cb1f73a7 fb3f0000 00000000 ......s..?......
-  0x00011300 c227738b 431cd894 f83f0000 00000000 .'s.C....?......
-  0x00011310 5fbb8e14 1630c694 db3f0000 00000000 _....0...?......
-  0x00011320 295d9a04 4350f2eb e23f0000 00000000 )]..CP...?......
-  0x00011330 64bba11b 22a14693 e93f0000 00000000 d...".F..?......
-  0x00011340 142aeb35 3a0b4ab9 ee3f0000 00000000 .*.5:.J..?......
-  0x00011350 5013cc02 7d7ad2f9 f23f0000 00000000 P...}z...?......
-  0x00011360 d04d68a5 15e8f2b0 f63f0000 00000000 .Mh......?......
-  0x00011370 cdfe24bf 3b149bed f83f0000 00000000 ..$.;....?......
-  0x00011380 8f0e461e 248540e1 f93f0000 00000000 ..F.$.@..?......
-  0x00011390 758ec59d 17621d97 ee3f0000 00000000 u....b...?......
-  0x000113a0 e1a3ef78 e066c8cf f13f0000 00000000 ...x.f...?......
-  0x000113b0 28c62675 0c70f793 f23f0000 00000000 (.&u.p...?......
-  0x000113c0 9de4a006 9063009e f63f0000 00000000 .....c...?......
-  0x000113d0 6b6188ea 018f04e9 f83f0000 00000000 ka.......?......
-  0x000113e0 fd9065d5 58e35aee f93f0000 00000000 ..e.X.Z..?......
-  0x000113f0 22959f13 1946fbd8 f83f0000 00000000 "....F...?......
-  0x00011400 5b9b7f1d 29777ede fc3f0000 00000000 [...)w~..?......
-  0x00011410 1b1079e7 82d30198 fe3f0000 00000000 ..y......?......
-  0x00011420 975b5911 24fa22f1 fe3f0000 00000000 .[Y.$."..?......
-  0x00011430 d9ba7e26 ccce8abc fe3f0000 00000000 ..~&.....?......
-  0x00011440 c0102520 aa6a88bf fd3f0000 00000000 ..% .j...?......
-  0x00011450 0dd63e83 27f0a780 fc3f0000 00000000 ..>.'....?......
-  0x00011460 d0697bad df186ece f93f0000 00000000 .i{...n..?......
-  0x00011470 ddef1321 74862196 f63f0000 00000000 ...!t.!..?......
-  0x00011480 f99ee6d7 dedc07d6 de3f0000 00000000 .........?......
-  0x00011490 0fe033b5 243cb8a9 e63f0000 00000000 ..3.$<...?......
-  0x000114a0 67006269 9910e0d3 ec3f0000 00000000 g.bi.....?......
-  0x000114b0 acfb9a48 d4f94785 f23f0000 00000000 ...H..G..?......
-  0x000114c0 d502e893 725bb3b3 f63f0000 00000000 ....r[...?......
-  0x000114d0 4331c9ca 7c4890fe f93f0000 00000000 C1..|H...?......
-  0x000114e0 b5ad022f 56c6e9aa fc3f0000 00000000 .../V....?......
-  0x000114f0 9455c8f0 cbe606a2 fd3f0000 00000000 .U.......?......
-  0x00011500 ec822f3f 2dd03aa5 e93f0000 00000000 ../?-.:..?......
-  0x00011510 8e924997 27769390 ec3f0000 00000000 ..I.'v...?......
-  0x00011520 e0c4328a ece4a5a2 ef3f0000 00000000 ..2......?......
-  0x00011530 e8d0bede d80576b2 f23f0000 00000000 ......v..?......
-  0x00011540 9d520cd4 43447ada f23f0000 00000000 .R..CDz..?......
-  0x00011550 f6d34d33 a036698c f73f0000 00000000 ..M3.6i..?......
-  0x00011560 6d17c7b1 876813d9 f73f0000 00000000 m....h...?......
-  0x00011570 8707aa9f 909531fc f93f0000 00000000 ......1..?......
-  0x00011580 182b7705 6a8389e6 fb3f0000 00000000 .+w.j....?......
-  0x00011590 f790cd15 03065bdd fa3f0000 00000000 ......[..?......
-  0x000115a0 b0a59a9b 246756b7 fd3f0000 00000000 ....$gV..?......
-  0x000115b0 e4568d48 58936fe3 fe3f0000 00000000 .V.HX.o..?......
-  0x000115c0 9ace23d3 7b1a2ca0 fe3f0000 00000000 ..#.{.,..?......
-  0x000115d0 8da97eb1 582e4dd8 fc3f0000 00000000 ..~.X.M..?......
-  0x000115e0 0f54b581 aea233f7 f93f0000 00000000 .T....3..?......
-  0x000115f0 d8c7e7d1 0eacbbc4 d93f0000 00000000 .........?......
-  0x00011600 78cb72c0 6fd1009c e13f0000 00000000 x.r.o....?......
-  0x00011610 499eb23b 3778c0c2 e73f0000 00000000 I..;7x...?......
-  0x00011620 556a9406 78e804f5 ec3f0000 00000000 Uj..x....?......
-  0x00011630 26db3e04 83702da5 f13f0000 00000000 &.>..p-..?......
-  0x00011640 8f0f3c31 9e7cfde9 f43f0000 00000000 ..<1.|...?......
-  0x00011650 0dca8a1b 29aa199d f73f0000 00000000 ....)....?......
-  0x00011660 516b161e a2a4ee94 f83f0000 00000000 Qk.......?......
-  0x00011670 3336992d 4cb625d0 e2bf0000 00000000 36.-L.%.........
-  0x00011680 4355595f 54ed198f e63f0000 00000000 CUY_T....?......
-  0x00011690 6af0a22e 7b56d98b e93f0000 00000000 j...{V...?......
-  0x000116a0 eeefdb0d 9f85dd8c ed3f0000 00000000 .........?......
-  0x000116b0 39e11b69 df4aeb87 ec3f0000 00000000 9..i.J...?......
-  0x000116c0 326f8558 bcef9ea3 f23f0000 00000000 2o.X.....?......
-  0x000116d0 a7c76712 c4e08f9b f43f0000 00000000 ..g......?......
-  0x000116e0 8df98094 7c3c2e95 f53f0000 00000000 ....|<...?......
-  0x000116f0 33bcad3c c3f854ce f83f0000 00000000 3..<..T..?......
-  0x00011700 54fbbfd2 2a9842ea f93f0000 00000000 T...*.B..?......
-  0x00011710 26acd24d 5a5419e8 f83f0000 00000000 &..MZT...?......
-  0x00011720 113debc7 9527d8e9 fc3f0000 00000000 .=...'...?......
-  0x00011730 753ff640 94aec5a0 fe3f0000 00000000 u?.@.....?......
-  0x00011740 5e91d1ff 9e222d88 ff3f0000 00000000 ^...."-..?......
-  0x00011750 20d9aa6a 2baad1c8 fe3f0000 00000000  ..j+....?......
-  0x00011760 d529f15c d25f21cc fd3f0000 00000000 .).\._!..?......
-  0x00011770 b2759fa1 afb02889 fc3f0000 00000000 .u....(..?......
-  0x00011780 cb8b310b fbf718dc f93f0000 00000000 ..1......?......
-  0x00011790 4ef1c693 b62812a0 f63f0000 00000000 N....(...?......
-  0x000117a0 0439eada 05fb89c4 cf3f0000 00000000 .9.......?......
-  0x000117b0 c032cbfa 9dc89585 d83f0000 00000000 .2.......?......
-  0x000117c0 566dbf9c ffe07598 df3f0000 00000000 Vm....u..?......
-  0x000117d0 5ab6cfaa 95d21bbe e53f0000 00000000 Z........?......
-  0x000117e0 4f86c251 05ee318d eb3f0000 00000000 O..Q..1..?......
-  0x000117f0 1e98d8cd 861fabff ef3f0000 00000000 .........?......
-  0x00011800 a560f18a ca04c08a f43f0000 00000000 .`.......?......
-  0x00011810 35a03178 bfaa70aa f73f0000 00000000 5.1x..p..?......
-  0x00011820 36175479 51fe2ad1 f93f0000 00000000 6.TyQ.*..?......
-  0x00011830 30d2066e 306c4ebc fa3f0000 00000000 0..n0lN..?......
-  0x00011840 5083d440 16b5cebd e53f0000 00000000 P..@.....?......
-  0x00011850 b1aaac14 22f3379a e93f0000 00000000 ....".7..?......
-  0x00011860 ba13ef08 b98b88d5 ea3f0000 00000000 .........?......
-  0x00011870 5f35b8fd 806db0dd ef3f0000 00000000 _5...m...?......
-  0x00011880 ec48362c 71ae71d2 f13f0000 00000000 .H6,q.q..?......
-  0x00011890 7a2cc428 96b0bdb8 f33f0000 00000000 z,.(.....?......
-  0x000118a0 5d09707b 7037bbfe f63f0000 00000000 ].p{p7...?......
-  0x000118b0 2de5a5ce ab7ab7c0 f83f0000 00000000 -....z...?......
-  0x000118c0 732bab27 d63ac3a6 f73f0000 00000000 s+.'.:...?......
-  0x000118d0 839a6775 0647f29d fb3f0000 00000000 ..gu.G...?......
-  0x000118e0 47931acb 50aa9e9c fd3f0000 00000000 G...P....?......
-  0x000118f0 3b63484d 3b0a29a8 fe3f0000 00000000 ;cHM;.)..?......
-  0x00011900 579c5f8c 08d15ef4 fe3f0000 00000000 W._...^..?......
-  0x00011910 51ab0fd1 ca051ec5 fe3f0000 00000000 Q........?......
-  0x00011920 c0993734 1c9956de fd3f0000 00000000 ..74..V..?......
-  0x00011930 457c05f2 89e55db3 fc3f0000 00000000 E|....]..?......
-  0x00011940 e2171bc7 aeac82c4 fa3f0000 00000000 .........?......
-  0x00011950 3e97972a 0df13983 f83f0000 00000000 >..*..9..?......
-  0x00011960 127f7f6f c16382a1 f43f0000 00000000 ...o.c...?......
-  0x00011970 14937222 251ee9c3 d33f0000 00000000 ..r"%....?......
-  0x00011980 f7df693d 7d722885 dc3f0000 00000000 ..i=}r(..?......
-  0x00011990 e3cc6662 e817f997 e33f0000 00000000 ..fb.....?......
-  0x000119a0 0e1dcbf5 0c3980bd e93f0000 00000000 .....9...?......
-  0x000119b0 4f283ee4 605dbe8c ef3f0000 00000000 O(>.`]...?......
-  0x000119c0 83317aab 3bddd9fe f33f0000 00000000 .1z.;....?......
-  0x000119d0 c26a2b76 71744e8a f83f0000 00000000 .j+vqtN..?......
-  0x000119e0 488c748e 602ae5a9 fb3f0000 00000000 H.t.`*...?......
-  0x000119f0 1b4d9683 4acb7fd0 fd3f0000 00000000 .M..J....?......
-  0x00011a00 5888d902 4d4cb4bb fe3f0000 00000000 X...ML...?......
-  0x00011a10 7388fed2 7a4cdd88 e03f0000 00000000 s...zL...?......
-  0x00011a20 81595e2d 0af6f899 e33f0000 00000000 .Y^-.....?......
-  0x00011a30 7723c99b aa2f918e e73f0000 00000000 w#.../...?......
-  0x00011a40 e1efb5b8 8c3377c0 ea3f0000 00000000 .....3w..?......
-  0x00011a50 8b3c5c9d b48fa499 ec3f0000 00000000 .<\......?......
-  0x00011a60 f26e3c9f a5e430a9 f03f0000 00000000 .n<...0..?......
-  0x00011a70 a6da906e e03bb0fb ef3f0000 00000000 ...n.;...?......
-  0x00011a80 f9132f94 303215ee f43f0000 00000000 ../.02...?......
-  0x00011a90 588a3f2b 333bb0ba f63f0000 00000000 X.?+3;...?......
-  0x00011aa0 0894069e d0c0a89e f73f0000 00000000 .........?......
-  0x00011ab0 bc2ce368 a3c3aea3 fa3f0000 00000000 .,.h.....?......
-  0x00011ac0 ad34e1e1 f334c2f9 fa3f0000 00000000 .4...4...?......
-  0x00011ad0 f42dcba8 4cb839ab fb3f0000 00000000 .-..L.9..?......
-  0x00011ae0 e04dc99c 33b834f7 fd3f0000 00000000 .M..3.4..?......
-  0x00011af0 222e5da1 423686e9 fe3f0000 00000000 ".].B6...?......
-  0x00011b00 badf379a f39bc2b1 fe3f0000 00000000 ..7......?......
-  0x00011b10 60a04d7f 17ee139b fd3f0000 00000000 `.M......?......
-  0x00011b20 63d5640a 3dec069c fb3f0000 00000000 c.d.=....?......
-  0x00011b30 ca84925e fdd1b08a f83f0000 00000000 ...^.....?......
-  0x00011b40 38e98658 a4e00ab1 cd3f0000 00000000 8..X.....?......
-  0x00011b50 08655768 5fc9aaf0 d53f0000 00000000 .eWh_....?......
-  0x00011b60 6e37c4bc 1e265689 dd3f0000 00000000 n7...&V..?......
-  0x00011b70 bdae02ee 580440ab e33f0000 00000000 ....X.@..?......
-  0x00011b80 ff4a47bd ed9160fe e83f0000 00000000 .JG...`..?......
-  0x00011b90 0bd41bd4 c16d4ee6 ed3f0000 00000000 .....mN..?......
-  0x00011ba0 c743ee8e 76edf8f9 f13f0000 00000000 .C..v....?......
-  0x00011bb0 537f4afc 2b588899 f53f0000 00000000 S.J.+X...?......
-  0x00011bc0 7189ec52 a62d6bbc f73f0000 00000000 q..R.-k..?......
-  0x00011bd0 b522f0a1 3163a0a9 f83f0000 00000000 ."..1c...?......
-  0x00011be0 d79d47ab 8b3aee85 f0bf0000 00000000 ..G..:..........
-  0x00011bf0 7e6054f6 221fa3d9 f33f0000 00000000 ~`T."....?......
-  0x00011c00 050bcc83 f13beff6 f53f0000 00000000 .....;...?......
-  0x00011c10 5e48bf38 5a573aa3 f53f0000 00000000 ^H.8ZW:..?......
-  0x00011c20 f4c8153b b460a2c8 f93f0000 00000000 ...;.`...?......
-  0x00011c30 1e927948 e6219987 fc3f0000 00000000 ..yH.!...?......
-  0x00011c40 08bb20ec 82b00bc2 fd3f0000 00000000 .. ......?......
-  0x00011c50 e7ce9d3b 77eedcb9 fe3f0000 00000000 ...;w....?......
-  0x00011c60 096825a0 95805682 ff3f0000 00000000 .h%...V..?......
-  0x00011c70 16d7585c 63718dc5 fe3f0000 00000000 ..X\cq...?......
-  0x00011c80 e81c70b9 d742d3dc fd3f0000 00000000 ..p..B...?......
-  0x00011c90 96b89ff9 db5a41b1 fc3f0000 00000000 .....ZA..?......
-  0x00011ca0 09547880 2cccb3c1 fa3f0000 00000000 .Tx.,....?......
-  0x00011cb0 4b1942c2 7cda3881 f83f0000 00000000 K.B.|.8..?......
-  0x00011cc0 700b65db 85e50a9f f43f0000 00000000 p.e......?......
-  0x00011cd0 6598d4ee e215e0da df3f0000 00000000 e........?......
-  0x00011ce0 d89462f3 5ab18fad e73f0000 00000000 ..b.Z....?......
-  0x00011cf0 4cdcc481 2accabd8 ed3f0000 00000000 L...*....?......
-  0x00011d00 05959c0e 7f494c88 f33f0000 00000000 .....IL..?......
-  0x00011d10 0414d13b 93a6c4b7 f73f0000 00000000 ...;.....?......
-  0x00011d20 6aac46e1 5cb02982 fb3f0000 00000000 j.F.\.)..?......
-  0x00011d30 2deedbb1 0726c8ae fd3f0000 00000000 -....&...?......
-  0x00011d40 b80fd691 81c8b1a5 fe3f0000 00000000 .........?......
-  0x00011d50 9ca6aaa4 ac2d43b7 ed3f0000 00000000 .....-C..?......
-  0x00011d60 17a56a62 cd5efcfb f03f0000 00000000 ..jb.^...?......
-  0x00011d70 24c391b6 63c771b3 f13f0000 00000000 $...c.q..?......
-  0x00011d80 3418812d 6c3d9dbf f53f0000 00000000 4..-l=...?......
-  0x00011d90 0825d4a9 b89aabfe f73f0000 00000000 .%.......?......
-  0x00011da0 72599772 500c8287 f83f0000 00000000 rY.rP....?......
-  0x00011db0 78a73ac1 ebc2d5e0 fa3f0000 00000000 x.:......?......
-  0x00011dc0 ea52fd55 d55d6f8b fd3f0000 00000000 .R.U.]o..?......
-  0x00011dd0 b38010c3 b19226a4 fe3f0000 00000000 ......&..?......
-  0x00011de0 88df72f7 3bc1fcf6 fe3f0000 00000000 ..r.;....?......
-  0x00011df0 190b1f90 a3ec4dba fe3f0000 00000000 ......M..?......
-  0x00011e00 642df6c3 502a1ebc fd3f0000 00000000 d-..P*...?......
-  0x00011e10 c1371d19 da3bfffb fb3f0000 00000000 .7...;...?......
-  0x00011e20 f9770a9a 4f17f3c9 f93f0000 00000000 .w..O....?......
-  0x00011e30 876e4d87 c556df92 f63f0000 00000000 .nM..V...?......
-  0x00011e40 2b9e4f92 7c7c979d dc3f0000 00000000 +.O.||...?......
-  0x00011e50 d9440a90 6d3feef9 e33f0000 00000000 .D..m?...?......
-  0x00011e60 e86826a1 ef31019c ea3f0000 00000000 .h&..1...?......
-  0x00011e70 0235f440 605f45c4 ef3f0000 00000000 .5.@`_E..?......
-  0x00011e80 b92f8b82 b4785084 f43f0000 00000000 ./...xP..?......
-  0x00011e90 836321dc 8ab06fbb f73f0000 00000000 .c!...o..?......
-  0x00011ea0 7a6014d4 3730b0fb f93f0000 00000000 z`..70...?......
-  0x00011eb0 b1cda1b7 b9309aee fa3f0000 00000000 .....0...?......
-  0x00011ec0 f241ef55 a6d476a6 e7bf0000 00000000 .A.U..v.........
-  0x00011ed0 d34d90f0 5b670f9c eb3f0000 00000000 .M..[g...?......
-  0x00011ee0 073ad9ee d77266ad eb3f0000 00000000 .:...rf..?......
-  0x00011ef0 87c60252 abf56d8d f13f0000 00000000 ...R..m..?......
-  0x00011f00 9e796e12 b29b1681 f43f0000 00000000 .yn......?......
-  0x00011f10 16794d2f c166808c f53f0000 00000000 .yM/.f...?......
-  0x00011f20 24e8e796 140b97f3 f63f0000 00000000 $........?......
-  0x00011f30 1312f0b2 f7d2cc8e fa3f0000 00000000 .........?......
-  0x00011f40 7808738f 77202786 fc3f0000 00000000 x.s.w '..?......
-  0x00011f50 258351ba 2a543fa3 fd3f0000 00000000 %.Q.*T?..?......
-  0x00011f60 2ded3620 8b15748f fe3f0000 00000000 -.6 ..t..?......
-  0x00011f70 1adab088 a8bd1ebe fe3f0000 00000000 .........?......
-  0x00011f80 c172ac78 357f9cc1 fe3f0000 00000000 .r.x5....?......
-  0x00011f90 f6f19cca 407a4898 fe3f0000 00000000 ....@zH..?......
-  0x00011fa0 5aaba930 919103b8 fd3f0000 00000000 Z..0.....?......
-  0x00011fb0 8f324156 3ab4ffa7 fc3f0000 00000000 .2AV:....?......
-  0x00011fc0 b8cba1ef df2c8fe0 fa3f0000 00000000 .....,...?......
-  0x00011fd0 1e3418fe 5fc78fcf f83f0000 00000000 .4.._....?......
-  0x00011fe0 06218628 316d57ed f53f0000 00000000 .!.(1mW..?......
-  0x00011ff0 f6de5b4d 120e2afd f13f0000 00000000 ..[M..*..?......
-  0x00012000 4ee0d7c6 01810cf8 e43f0000 00000000 N........?......
-  0x00012010 3f668f71 d1288ac9 e83f0000 00000000 ?f.q.(...?......
-  0x00012020 2c6ed9ff 9008878b ea3f0000 00000000 ,n.......?......
-  0x00012030 7d119f89 564ddb90 ef3f0000 00000000 }...VM...?......
-  0x00012040 482044a5 e2edd882 f13f0000 00000000 H D......?......
-  0x00012050 0f76b747 d5175d8e f33f0000 00000000 .v.G..]..?......
-  0x00012060 14e338d6 3b8c5ca9 f63f0000 00000000 ..8.;.\..?......
-  0x00012070 b8fa1a6b af2805c3 f73f0000 00000000 ...k.(...?......
-  0x00012080 8c588ad7 ff7e1aa8 f83f0000 00000000 .X...~...?......
-  0x00012090 de991b2b 7535e8d5 fb3f0000 00000000 ...+u5...?......
-  0x000120a0 58d209b7 c11af8ad fd3f0000 00000000 X........?......
-  0x000120b0 0588b30e a79976af fe3f0000 00000000 ......v..?......
-  0x000120c0 31d1455e 7491eff7 fe3f0000 00000000 1.E^t....?......
-  0x000120d0 75122a5f bf178cc3 fe3f0000 00000000 u.*_.....?......
-  0x000120e0 374502e8 893493db fd3f0000 00000000 7E...4...?......
-  0x000120f0 d697e043 4264b2b0 fc3f0000 00000000 ...CBd...?......
-  0x00012100 0e3b9d87 4d3257c1 fa3f0000 00000000 .;..M2W..?......
-  0x00012110 e266f6c5 a2b60b81 f83f0000 00000000 .f.......?......
-  0x00012120 b4b991b8 ef56d39e f43f0000 00000000 .....V...?......
-  0x00012130 67d49312 a507eba6 d13f0000 00000000 g........?......
-  0x00012140 bcf44065 647ee7e2 d93f0000 00000000 ..@ed~...?......
-  0x00012150 e6381727 a0957b81 e13f0000 00000000 .8.'..{..?......
-  0x00012160 d84aa9fa f8f774a1 e73f0000 00000000 .J....t..?......
-  0x00012170 6e17aa2c cc90d4ef ec3f0000 00000000 n..,.....?......
-  0x00012180 3bdc1210 7bd022d9 f13f0000 00000000 ;...{."..?......
-  0x00012190 cd4226ba ab68adeb f53f0000 00000000 .B&..h...?......
-  0x000121a0 83dfea38 a6acc090 f93f0000 00000000 ...8.....?......
-  0x000121b0 628f03b7 76c9a4b1 fb3f0000 00000000 b...v....?......
-  0x000121c0 f0f72fde 811bed9f fc3f0000 00000000 ../......?......
-  0x000121d0 73c3e904 0629a2ae eb3f0000 00000000 s....)...?......
-  0x000121e0 aa5f3865 964b8cb9 ef3f0000 00000000 ._8e.K...?......
-  0x000121f0 aa5f3865 964b8cb9 f23f0000 00000000 ._8e.K...?......
-  0x00012200 947786fe 7b5eefe7 f43f0000 00000000 .w..{^...?......
-  0x00012210 a2a8b57e ac72f1ca f63f0000 00000000 ...~.r...?......
-  0x00012220 0314f6eb bcbde983 f83f0000 00000000 .........?......
-  0x00012230 0314f6eb bcbde983 f93f0000 00000000 .........?......
-  0x00012240 e0fa1405 72bc4acf f93f0000 00000000 ....r.J..?......
-  0x00012250 cc1c2d43 c7b58e81 fa3f0000 00000000 ..-C.....?......
-  0x00012260 f0c405df 44999885 da3f0000 00000000 ....D....?......
-  0x00012270 7a666a67 084a3594 e23f0000 00000000 zfjg.J5..?......
-  0x00012280 2914fdf1 e5f62985 e93f0000 00000000 ).....)..?......
-  0x00012290 e402faa1 069b92fa ee3f0000 00000000 .........?......
-  0x000122a0 573f19bb fa3a5585 f43f0000 00000000 W?...:U..?......
-  0x000122b0 2e454454 a5f7d2a1 f83f0000 00000000 .EDT.....?......
-  0x000122c0 1d6e900d 0b4370d6 fb3f0000 00000000 .n...Cp..?......
-  0x000122d0 6aabe1cb d0372e8a fe3f0000 00000000 j....7...?......
-  0x000122e0 29c04c36 fb7812bb ebbf0000 00000000 ).L6.x..........
-  0x000122f0 29c04c36 fb7812bb ec3f0000 00000000 ).L6.x...?......
-  0x00012300 b2f0c033 805e88e2 f23f0000 00000000 ...3.^...?......
-  0x00012310 328a2d2a 7283fee3 f33f0000 00000000 2.-*r....?......
-  0x00012320 d01965e6 4d3fa3a2 f83f0000 00000000 ..e.M?...?......
-  0x00012330 f9cf0daf 5b3933a6 f93f0000 00000000 ....[93..?......
-  0x00012340 431e4bf2 3e2e9c91 fc3f0000 00000000 C.K.>....?......
-  0x00012350 43fb3bad d461ff9b fd3f0000 00000000 C.;..a...?......
-  0x00012360 5f0262a9 154f00b2 fd3f0000 00000000 _.b..O...?......
-  0x00012370 8caa2200 a047d096 e43f0000 00000000 .."..G...?......
-  0x00012380 90ca1d80 8dfd9a81 ec3f0000 00000000 .........?......
-  0x00012390 e1a12218 8e93aa96 f23f0000 00000000 .."......?......
-  0x000123a0 f85920a9 574fbe8c f73f0000 00000000 .Y .WO...?......
-  0x000123b0 03982c02 23cd00c2 fa3f0000 00000000 ..,.#....?......
-  0x000123c0 e5771ea0 f30e8d84 fc3f0000 00000000 .w.......?......
-  0x000123d0 78827bfc 3f1b19b4 ee3f0000 00000000 x.{.?....?......
-  0x000123e0 78827bfc 3f1b19b4 f03f0000 00000000 x.{.?....?......
-  0x000123f0 1a2d017d 34615d99 f53f0000 00000000 .-.}4a]..?......
-  0x00012400 3300defc 445c66a0 f73f0000 00000000 3...D\f..?......
-  0x00012410 aca0a2e0 4f888af0 f93f0000 00000000 ....O....?......
-  0x00012420 3e1fd387 d9488291 fc3f0000 00000000 >....H...?......
-  0x00012430 d25b170b 470954fb f93f0000 00000000 .[..G.T..?......
-  0x00012440 428a11a7 acd05bda fe3f0000 00000000 B.....[..?......
-  0x00012450 4831e294 157a4bbb ff3f0000 00000000 H1...zK..?......
-  0x00012460 641ba706 839b96c1 e43f0000 00000000 d........?......
-  0x00012470 8a9bb799 a46d5da6 ec3f0000 00000000 .....m]..?......
-  0x00012480 9d71e525 dc3566c1 f23f0000 00000000 .q.%.5f..?......
-  0x00012490 e862edbe 1075a9b4 f73f0000 00000000 .b...u...?......
-  0x000124a0 6cd67efc eb0c07f9 fa3f0000 00000000 l.~......?......
-  0x000124b0 13dfd828 ae5e25aa fc3f0000 00000000 ...(.^%..?......
-  0x000124c0 a3099de3 5a1502c8 f0bf0000 00000000 ....Z...........
-  0x000124d0 3ac7b52a 04900196 f33f0000 00000000 :..*.....?......
-  0x000124e0 6b0ae803 77a18cbc f63f0000 00000000 k...w....?......
-  0x000124f0 21800cb0 04c2c1a8 f93f0000 00000000 !........?......
-  0x00012500 dfa2135d e7c21689 f63f0000 00000000 ...].....?......
-  0x00012510 461dfaca 1d2c8bf0 fc3f0000 00000000 F....,...?......
-  0x00012520 91651666 48265bb6 fe3f0000 00000000 .e.fH&[..?......
-  0x00012530 f6621ca5 eafd37c3 fe3f0000 00000000 .b....7..?......
-  0x00012540 0c8324b1 6d22e99c fd3f0000 00000000 ..$.m"...?......
-  0x00012550 10048641 92d836d1 fa3f0000 00000000 ...A..6..?......
-  0x00012560 080e78f8 48e50cb1 e53f0000 00000000 ..x.H....?......
-  0x00012570 0f2c87b5 0a152798 ed3f0000 00000000 .,....'..?......
-  0x00012580 05f039a6 0fa2e0b0 f33f0000 00000000 ..9......?......
-  0x00012590 d9c920a1 d9703aa5 f83f0000 00000000 .. ..p:..?......
-  0x000125a0 8def1f6e b2e6c0e3 fb3f0000 00000000 ...n.....?......
-  0x000125b0 55846122 85559c9b fd3f0000 00000000 U.a".U...?......
-  0x000125c0 684b3026 b62f02c7 e83f0000 00000000 hK0&./...?......
-  0x000125d0 cd80d188 00e105ab f03f0000 00000000 .........?......
-  0x000125e0 55bfa638 2a6fd0c6 f63f0000 00000000 U..8*o...?......
-  0x000125f0 df819394 5662b8b9 fb3f0000 00000000 ....Vb...?......
-  0x00012600 46729017 efebe8ae 00400000 00000000 Fr.......@......
-  0x00012610 0ab36fb1 cc9f4ded f33f0000 00000000 ..o...M..?......
-  0x00012620 0ab36fb1 cc9f4ded f63f0000 00000000 ..o...M..?......
-  0x00012630 b6d4ce23 e3a97b85 f73f0000 00000000 ...#..{..?......
-  0x00012640 dab758e6 cfc578de fb3f0000 00000000 ..X...x..?......
-  0x00012650 66df6299 3fbadcdf fd3f0000 00000000 f.b.?....?......
-  0x00012660 3ef4a97e 4d6998e9 fe3f0000 00000000 >..~Mi...?......
-  0x00012670 ddfd7be8 932d6e94 ff3f0000 00000000 ..{..-n..?......
-  0x00012680 7092d24a 0c3b28ef fe3f0000 00000000 p..J.;(..?......
-  0x00012690 37a65724 4435daef fd3f0000 00000000 7.W$D5...?......
-  0x000126a0 82939456 62e03089 fc3f0000 00000000 ...Vb.0..?......
-  0x000126b0 82939456 62e03089 f93f0000 00000000 ...Vb.0..?......
-  0x000126c0 d0e5eedf 439f36b5 f2bf0000 00000000 ....C.6.........
-  0x000126d0 449fead7 144784e2 f53f0000 00000000 D....G...?......
-  0x000126e0 2cf3e772 f7cfd4fe f73f0000 00000000 ,..r.....?......
-  0x000126f0 73f7efa1 4f35e3a9 f93f0000 00000000 s...O5...?......
-  0x00012700 85f8b1ad a5cea694 fa3f0000 00000000 .........?......
-  0x00012710 392a6fd0 c6c461b2 fa3f0000 00000000 9*o...a..?......
-  0x00012720 d0e5eedf 439f36b5 f23f0000 00000000 ....C.6..?......
-  0x00012730 079379e7 b9b4e0d1 e93f0000 00000000 ..y......?......
-  0x00012740 3e30555c 59c199a2 f13f0000 00000000 >0U\Y....?......
-  0x00012750 0ac15005 d5c0b5a4 f73f0000 00000000 ..P......?......
-  0x00012760 5d1576eb f16d41fd fb3f0000 00000000 ].v..mA..?......
-  0x00012770 6c2959b5 cae8e1b3 ff3f0000 00000000 l)Y......?......
-  0x00012780 1c2ef465 9ea51fe5 e63f0000 00000000 ...e.....?......
-  0x00012790 a0d79d1f 5432e7c4 ee3f0000 00000000 ....T2...?......
-  0x000127a0 10b15afe b45de6e4 f43f0000 00000000 ..Z..]...?......
-  0x000127b0 2868555a a710d3d5 f93f0000 00000000 (hUZ.....?......
-  0x000127c0 c8554329 dea25e93 fd3f0000 00000000 .UC)..^..?......
-  0x000127d0 869c9b37 90d060c9 fe3f0000 00000000 ...7..`..?......
-  0x000127e0 7fd4011b d52d19b7 e0bf0000 00000000 .....-..........
-  0x000127f0 5f5f41d4 5fe25289 e23f0000 00000000 __A._.R..?......
-  0x00012800 cebaf0ef 4d36b58b e83f0000 00000000 ....M6...?......
-  0x00012810 871f553c 2c366cd4 e93f0000 00000000 ..U<,6l..?......
-  0x00012820 af5e7c84 21f61ba3 ee3f0000 00000000 .^|.!....?......
-  0x00012830 0baaaebd 4f9987fd ef3f0000 00000000 ....O....?......
-  0x00012840 33953040 58df74b6 f33f0000 00000000 3.0@X.t..?......
-  0x00012850 21a7ffa9 c5ca7393 f53f0000 00000000 !.....s..?......
-  0x00012860 ba94d48d d23868c8 f73f0000 00000000 .....8h..?......
-  0x00012870 8d9c3e99 250d1aaf f93f0000 00000000 ..>.%....?......
-  0x00012880 6e47336e 37274cbe fa3f0000 00000000 nG3n7'L..?......
-  0x00012890 a14baf17 91a01fca fc3f0000 00000000 .K.......?......
-  0x000128a0 725fd8ff f4915b93 fb3f0000 00000000 r_....[..?......
-  0x000128b0 0d68d13a b54cf5c2 fe3f0000 00000000 .h.:.L...?......
-  0x000128c0 7f36b021 3eac2cfe fd3f0000 00000000 .6.!>.,..?......
-  0x000128d0 79daf0dd 837131b9 fe3f0000 00000000 y....q1..?......
-  0x000128e0 455d80cf cc289c93 d53f0000 00000000 E]...(...?......
-  0x000128f0 79673236 433dc1a3 dd3f0000 00000000 yg26C=...?......
-  0x00012900 f886e405 7beb2193 e43f0000 00000000 ....{.!..?......
-  0x00012910 a8bf3ba3 18b76d8a ea3f0000 00000000 ..;...m..?......
-  0x00012920 56cd8283 6ab95193 ef3f0000 00000000 V...j.Q..?......
-  0x00012930 6596044c 878eccb2 f33f0000 00000000 e..L.....?......
-  0x00012940 d285e4b2 77bfeeec f63f0000 00000000 ....w....?......
-  0x00012950 8cd82ac2 77e3ac98 f93f0000 00000000 ..*.w....?......
-  0x00012960 94980e44 d5486d8d fa3f0000 00000000 ...D.Hm..?......
-  0x00012970 e99e0ba1 5dd279b9 e33f0000 00000000 ....].y..?......
-  0x00012980 a4864e09 f546d8e7 e53f0000 00000000 ..N..F...?......
-  0x00012990 ac29461c 62780ce2 ea3f0000 00000000 .)F.bx...?......
-  0x000129a0 414ef6f9 748d8694 ed3f0000 00000000 AN..t....?......
-  0x000129b0 400dd471 afeb03c3 f03f0000 00000000 @..q.....?......
-  0x000129c0 9b8cde4a a2d79b8c f33f0000 00000000 ...J.....?......
-  0x000129d0 6bbd836d 45770088 f53f0000 00000000 k..mEw...?......
-  0x000129e0 eda1a373 a515f3f1 f73f0000 00000000 ...s.....?......
-  0x000129f0 fefe9f6b f94fbdbb f73f0000 00000000 ...k.O...?......
-  0x00012a00 0d9143cb 2959fcb9 fb3f0000 00000000 ..C.)Y...?......
-  0x00012a10 06bc6b10 19dc86af fb3f0000 00000000 ..k......?......
-  0x00012a20 d8fa3587 10bad9c5 fd3f0000 00000000 ..5......?......
-  0x00012a30 b99e1efa 3b0f05ee fe3f0000 00000000 ....;....?......
-  0x00012a40 07066f2c a8a76cc0 fd3f0000 00000000 ..o,..l..?......
-  0x00012a50 c4aa86c6 4eed3ebd ff3f0000 00000000 ....N.>..?......
-  0x00012a60 76552878 a2a88ecc fe3f0000 00000000 vU(x.....?......
-  0x00012a70 2b11ed2c b553a5a3 fc3f0000 00000000 +..,.S...?......
-  0x00012a80 51f7f945 ede113ba d63f0000 00000000 Q..E.....?......
-  0x00012a90 5e4ea139 a30e6ece de3f0000 00000000 ^N.9..n..?......
-  0x00012aa0 50047c2d 76c979b9 e53f0000 00000000 P.|-v.y..?......
-  0x00012ab0 25d56aa3 94e780ae eb3f0000 00000000 %.j......?......
-  0x00012ac0 1df13315 a50cb6b9 f03f0000 00000000 ..3......?......
-  0x00012ad0 1060591e 840a65e1 f43f0000 00000000 .`Y...e..?......
-  0x00012ae0 01a9fbe8 7eca5695 f83f0000 00000000 ....~.V..?......
-  0x00012af0 14e5328e 328b76c0 fa3f0000 00000000 ..2.2.v..?......
-  0x00012b00 71ff2d2a 4c8148b2 fb3f0000 00000000 q.-*L.H..?......
-  0x00012b10 77be96b1 a379d7e0 e5bf0000 00000000 w....y..........
-  0x00012b20 a8e6633b 6f8abcc4 e83f0000 00000000 ..c;o....?......
-  0x00012b30 a2412aca 55e83fc8 ec3f0000 00000000 .A*.U.?..?......
-  0x00012b40 437651f8 987ccfc7 ef3f0000 00000000 CvQ..|...?......
-  0x00012b50 86be13e1 774755c1 f13f0000 00000000 ....wGU..?......
-  0x00012b60 c5166657 3a49b087 f53f0000 00000000 ..fW:I...?......
-  0x00012b70 7397e716 2ff9d6ec f13f0000 00000000 s.../....?......
-  0x00012b80 67ed0a90 7b8be08a f93f0000 00000000 g...{....?......
-  0x00012b90 779d0fed 90efc89e fa3f0000 00000000 w........?......
-  0x00012ba0 5708bca4 87c118df fa3f0000 00000000 W........?......
-  0x00012bb0 a57c5ede 0325f6b1 fd3f0000 00000000 .|^..%...?......
-  0x00012bc0 cedf8117 cb9e6185 fe3f0000 00000000 ......a..?......
-  0x00012bd0 0a4d38b2 657bbccd fb3f0000 00000000 .M8.e{...?......
-  0x00012be0 ed48c55c 78efaeac fe3f0000 00000000 .H.\x....?......
-  0x00012bf0 546ddf76 0354d5ac fe3f0000 00000000 Tm.v.T...?......
-  0x00012c00 53ff0610 065375ee fc3f0000 00000000 S....Su..?......
-  0x00012c10 c24896e4 de0a4388 fa3f0000 00000000 .H....C..?......
-  0x00012c20 146eacb7 b84d21b3 d83f0000 00000000 .n...M!..?......
-  0x00012c30 1e4ac3eb 38f2b8c6 e03f0000 00000000 .J..8....?......
-  0x00012c40 4953b45a 24f68cb2 e73f0000 00000000 IS.Z$....?......
-  0x00012c50 cbbb7ac1 4af4fca7 ed3f0000 00000000 ..z.J....?......
-  0x00012c60 26fda136 52f9c6b2 f23f0000 00000000 &..6R....?......
-  0x00012c70 1f5d4397 e5a8fad8 f63f0000 00000000 .]C......?......
-  0x00012c80 e5ca2d85 9c5ec38f fa3f0000 00000000 ..-..^...?......
-  0x00012c90 344ed331 79ee46b9 fc3f0000 00000000 4N.1y.F..?......
-  0x00012ca0 2bc50b5a 6e6da0ab fd3f0000 00000000 +..Znm...?......
-  0x00012cb0 4a1b2080 5a4cd290 e63f0000 00000000 J. .ZL...?......
-  0x00012cc0 b41e24d0 e595eca2 e93f0000 00000000 ..$......?......
-  0x00012cd0 3bc82260 b7d2e39c ec3f0000 00000000 ;."`.....?......
-  0x00012ce0 0e2e36b8 d8e062f4 ef3f0000 00000000 ..6...b..?......
-  0x00012cf0 292feb4f a86a0d89 ef3f0000 00000000 )/.O.j...?......
-  0x00012d00 2a6bd5bb 9dc5ffaf f43f0000 00000000 *k.......?......
-  0x00012d10 0852c303 e44161a1 f63f0000 00000000 .R...Aa..?......
-  0x00012d20 47e3424e 730ab9eb ef3f0000 00000000 G.BNs....?......
-  0x00012d30 457e8515 ddf3c9a1 f93f0000 00000000 E~.......?......
-  0x00012d40 ff5a4a4c 2e95ecdd fa3f0000 00000000 .ZJL.....?......
-  0x00012d50 72146802 558f06f9 fa3f0000 00000000 r.h.U....?......
-  0x00012d60 70ae43f3 df6ed0bd f53f0000 00000000 p.C..n...?......
-  0x00012d70 1ffaddbc 6819e3c7 fb3f0000 00000000 ....h....?......
-  0x00012d80 632a1043 f55ffe91 fc3f0000 00000000 c*.C._...?......
-  0x00012d90 9365a639 cfa0d7df fb3f0000 00000000 .e.9.....?......
-  0x00012da0 f81c2ad0 ded209cb fa3f0000 00000000 ..*......?......
-  0x00012db0 a388206e 3bf9f2ce f83f0000 00000000 .. n;....?......
-  0x00012dc0 58b28e0c c36bf4b7 f53f0000 00000000 X....k...?......
-  0x00012dd0 bf079b3e c611b9bd de3f0000 00000000 ...>.....?......
-  0x00012de0 057fbca8 1bb8efab e63f0000 00000000 .........?......
-  0x00012df0 09583794 2c653ff6 ec3f0000 00000000 .X7.,e?..?......
-  0x00012e00 36e051e5 03d742b2 f23f0000 00000000 6.Q...B..?......
-  0x00012e10 006661cc 248a1e8b f73f0000 00000000 .fa.$....?......
-  0x00012e20 29ff6c69 d8ad2be7 fa3f0000 00000000 ).li..+..?......
-  0x00012e30 3f260cdc e7ebe4bd fd3f0000 00000000 ?&.......?......
-  0x00012e40 48aceaa4 1788f4fb fe3f0000 00000000 H........?......
-  0x00012e50 8e8d6447 85f4d5c6 d63f0000 00000000 ..dG.....?......
-  0x00012e60 098d33db 435b95dc de3f0000 00000000 ..3.C[...?......
-  0x00012e70 496e05c9 564b31c6 e53f0000 00000000 In..VK1..?......
-  0x00012e80 cadda5d1 63d377ba eb3f0000 00000000 ....c.w..?......
-  0x00012e90 8336ccb6 42b071c6 f03f0000 00000000 .6..B.q..?......
-  0x00012ea0 0de8c737 cc36d9f0 f43f0000 00000000 ...7.6...?......
-  0x00012eb0 1015ace5 0705949f f83f0000 00000000 .........?......
-  0x00012ec0 15f81799 b1b1a8cd fa3f0000 00000000 .........?......
-  0x00012ed0 88155aec 9fc481be fb3f0000 00000000 ..Z......?......
-  0x00012ee0 5ce9579e 2c5ae2c5 dcbf0000 00000000 \.W.,Z..........
-  0x00012ef0 b3e3edc5 b7f05af7 de3f0000 00000000 ......Z..?......
-  0x00012f00 4c6e2225 22530bb2 e43f0000 00000000 Ln"%"S...?......
-  0x00012f10 fd789a6c 70ff48e6 e63f0000 00000000 .x.lp.H..?......
-  0x00012f20 179f5e16 8d1a18f3 ea3f0000 00000000 ..^......?......
-  0x00012f30 9b1ca611 514569a6 ed3f0000 00000000 ....QEi..?......
-  0x00012f40 4a93ac9e ab70dd9a f03f0000 00000000 J....p...?......
-  0x00012f50 1a9362d2 d392d1eb f23f0000 00000000 ..b......?......
-  0x00012f60 07c3ddaf 3bed7ab0 f43f0000 00000000 ....;.z..?......
-  0x00012f70 ac8f5646 849a1cab f73f0000 00000000 ..VF.....?......
-  0x00012f80 5de7c9e4 d5d50eb6 f63f0000 00000000 ]........?......
-  0x00012f90 b063bce3 64cec0ee fa3f0000 00000000 .c..d....?......
-  0x00012fa0 04a9a215 9b00e2e8 fa3f0000 00000000 .........?......
-  0x00012fb0 1c713e83 993449fb fc3f0000 00000000 .q>..4I..?......
-  0x00012fc0 58d46bdb 99251d8f fe3f0000 00000000 X.k..%...?......
-  0x00012fd0 0069f74b a49c3afb fa3f0000 00000000 .i.K..:..?......
-  0x00012fe0 104756d9 d66545a7 ff3f0000 00000000 .GV..eE..?......
-  0x00012ff0 d4d8ab8f 4cbf16b1 fe3f0000 00000000 ....L....?......
-  0x00013000 76adbc3f 3dccab8d fc3f0000 00000000 v..?=....?......
-  0x00013010 7b1c4632 af9f9a92 cd3f0000 00000000 {.F2.....?......
-  0x00013020 b82a69cb 86efe7db d53f0000 00000000 .*i......?......
-  0x00013030 2d7f7176 647d9888 dd3f0000 00000000 -.qvd}...?......
-  0x00013040 4dda05ae de0ce8b6 e33f0000 00000000 M........?......
-  0x00013050 38c9463c 3c34fd8f e93f0000 00000000 8.F<<4...?......
-  0x00013060 be3e29d8 919e8188 ee3f0000 00000000 .>)......?......
-  0x00013070 8cf57042 092f7199 f23f0000 00000000 ..pB./q..?......
-  0x00013080 ca82344a 6cba51c1 f53f0000 00000000 ..4Jl.Q..?......
-  0x00013090 8f3ddcd7 74a251f1 f73f0000 00000000 .=..t.Q..?......
-  0x000130a0 7b00c494 a13679db f83f0000 00000000 {....6y..?......
-  0x000130b0 397d1d4d ac82bef5 de3f0000 00000000 9}.M.....?......
-  0x000130c0 92cd79c3 56b206d7 e13f0000 00000000 ..y.V....?......
-  0x000130d0 8ad985d2 63b2bfad e63f0000 00000000 ....c....?......
-  0x000130e0 31bb6cc4 3c2778a5 e93f0000 00000000 1.l.<'x..?......
-  0x000130f0 51f55525 10da41a7 ec3f0000 00000000 Q.U%..A..?......
-  0x00013100 cd00d912 a3ed58bc ef3f0000 00000000 ......X..?......
-  0x00013110 609483bf 6572bdda f03f0000 00000000 `...er...?......
-  0x00013120 f52af413 b90ad5c1 f43f0000 00000000 .*.......?......
-  0x00013130 861beed6 983683b9 f33f0000 00000000 .....6...?......
-  0x00013140 a8591e5a cf56efab f83f0000 00000000 .Y.Z.V...?......
-  0x00013150 38653c37 c3b9e4c6 f93f0000 00000000 8e<7.....?......
-  0x00013160 cae34408 07f05f9c fa3f0000 00000000 ..D..._..?......
-  0x00013170 3a908f2c fb187de4 fc3f0000 00000000 :..,..}..?......
-  0x00013180 123fcf15 19cf618f fd3f0000 00000000 .?....a..?......
-  0x00013190 52b95d0e 9d988b89 fc3f0000 00000000 R.]......?......
-  0x000131a0 be119c75 1648a3c8 fe3f0000 00000000 ...u.H...?......
-  0x000131b0 63c2f718 689160a6 fe3f0000 00000000 c...h.`..?......
-  0x000131c0 2e94b12b 76fe28e3 fc3f0000 00000000 ...+v.(..?......
-  0x000131d0 d19dae86 4348ce81 fa3f0000 00000000 ....CH...?......
-  0x000131e0 c2a9a4cd c88ab189 ce3f0000 00000000 .........?......
-  0x000131f0 a3fe7634 2d508ace d63f0000 00000000 ..v4-P...?......
-  0x00013200 03ba4a54 f5214b80 de3f0000 00000000 ..JT.!K..?......
-  0x00013210 6a2ab6b8 1b1fcaab e43f0000 00000000 j*.......?......
-  0x00013220 700dec10 28cf3c87 ea3f0000 00000000 p...(.<..?......
-  0x00013230 526eafb1 fca63580 ef3f0000 00000000 Rn....5..?......
-  0x00013240 4268a76b 56b41d90 f33f0000 00000000 Bh.kV....?......
-  0x00013250 22e833ef 1ac891b5 f63f0000 00000000 ".3......?......
-  0x00013260 fd92d307 bcd6a6e2 f83f0000 00000000 .........?......
-  0x00013270 e84790c1 0f5222ce f93f0000 00000000 .G...R"..?......
-  0x00013280 57c8a836 37bb2aa0 e2bf0000 00000000 W..67.*.........
-  0x00013290 62e17d1d 9e1230b4 e53f0000 00000000 b.}...0..?......
-  0x000132a0 e81916a5 ad106ba1 e93f0000 00000000 ......k..?......
-  0x000132b0 1a6c884a a47622db ec3f0000 00000000 .l.J.v"..?......
-  0x000132c0 40bf3cbe 2b002f92 ee3f0000 00000000 @.<.+./..?......
-  0x000132d0 8e0f725e d7998bb0 f23f0000 00000000 ..r^.....?......
-  0x000132e0 6065c138 8a13bdd6 f23f0000 00000000 `e.8.....?......
-  0x000132f0 9bc46ad7 935219cc f63f0000 00000000 ..j..R...?......
-  0x00013300 e419887f ec4b95c0 f83f0000 00000000 .....K...?......
-  0x00013310 6f686694 2677daf0 f63f0000 00000000 ohf.&w...?......
-  0x00013320 f06b54f0 ab5da5df fb3f0000 00000000 .kT..]...?......
-  0x00013330 94290d99 9dfcfc88 fd3f0000 00000000 .).......?......
-  0x00013340 b8c48e3a c2e6d1ce fc3f0000 00000000 ...:.....?......
-  0x00013350 318a3c16 88b8c3a2 fd3f0000 00000000 1.<......?......
-  0x00013360 64cc25c4 040d7e9f ff3f0000 00000000 d.%...~..?......
-  0x00013370 22cc354b 12bf98e8 fe3f0000 00000000 ".5K.....?......
-  0x00013380 56425c79 3e1f00cf fd3f0000 00000000 VB\y>....?......
-  0x00013390 519cdfa6 dbf0abd1 fb3f0000 00000000 Q........?......
-  0x000133a0 816e715b 8af25fba f83f0000 00000000 .nq[.._..?......
-  0x000133b0 3f743c8c 17afa4a1 d13f0000 00000000 ?t<......?......
-  0x000133c0 5eae5a52 a30677f2 d93f0000 00000000 ^.ZR..w..?......
-  0x000133d0 b79bb38a fbb69b96 e13f0000 00000000 .........?......
-  0x000133e0 c386c69d d178abc9 e73f0000 00000000 .....x...?......
-  0x000133f0 e06642c2 9697c29e ed3f0000 00000000 .fB......?......
-  0x00013400 358424ba 8b7f8296 f23f0000 00000000 5.$......?......
-  0x00013410 a7fb8921 01d32ea9 f63f0000 00000000 ...!.....?......
-  0x00013420 df80366c 6c9b26d5 f93f0000 00000000 ..6ll.&..?......
-  0x00013430 e84f3266 f6870985 fc3f0000 00000000 .O2f.....?......
-  0x00013440 87bfffe9 fef1fcf1 fc3f0000 00000000 .........?......
-  0x00013450 ae9133d3 bddf859b d43f0000 00000000 ..3......?......
-  0x00013460 855acdbc 9ccf48e9 dc3f0000 00000000 .Z....H..?......
-  0x00013470 6e7eb697 15dee790 e43f0000 00000000 n~.......?......
-  0x00013480 465a470a 42af08c2 ea3f0000 00000000 FZG.B....?......
-  0x00013490 6f3edcb1 91babf98 f03f0000 00000000 o>.......?......
-  0x000134a0 6987d362 129bcf90 f53f0000 00000000 i..b.....?......
-  0x000134b0 d7fd0b52 c9eec6a2 f93f0000 00000000 ...R.....?......
-  0x000134c0 c1038362 cc8814cd fc3f0000 00000000 ...b.....?......
-  0x000134d0 c5d7837a 4c5ad3e8 ff3f0000 00000000 ...zLZ...?......
-  0x000134e0 c950ccea af2267f3 e33f0000 00000000 .P..."g..?......
-  0x000134f0 8a776cf1 d8e756a7 e73f0000 00000000 .wl...V..?......
-  0x00013500 eaa65a7e cfe4598d ea3f0000 00000000 ..Z~..Y..?......
-  0x00013510 1c385072 c2f57895 ee3f0000 00000000 .8Pr..x..?......
-  0x00013520 1b6ce209 a71b47df ee3f0000 00000000 .l....G..?......
-  0x00013530 2a68c453 b5c0abf5 f23f0000 00000000 *h.S.....?......
-  0x00013540 a9bf9242 06e3dd9d f53f0000 00000000 ...B.....?......
-  0x00013550 4fa484e2 be2493d9 f43f0000 00000000 O....$...?......
-  0x00013560 14c18951 4c2dfcaa f83f0000 00000000 ...QL-...?......
-  0x00013570 22ad9f9a 28a5f5a8 fa3f0000 00000000 "...(....?......
-  0x00013580 0fc3d033 b8a20f8a fb3f0000 00000000 ...3.....?......
-  0x00013590 c36b4188 e2cfa3bf f93f0000 00000000 .kA......?......
-  0x000135a0 09656323 9bb9a8fe fb3f0000 00000000 .ec#.....?......
-  0x000135b0 06083645 e74f1898 fd3f0000 00000000 ..6E.O...?......
-  0x000135c0 097331f0 6cd8bbb9 fd3f0000 00000000 .s1.l....?......
-  0x000135d0 12cb323d 4064a891 fd3f0000 00000000 ..2=@d...?......
-  0x000135e0 3e860ec9 14328698 fc3f0000 00000000 >....2...?......
-  0x000135f0 b2c274e3 76e5d0cf fa3f0000 00000000 ..t.v....?......
-  0x00013600 113a9476 fa8196a7 f83f0000 00000000 .:.v.....?......
-  0x00013610 a40ea966 c9a5c3f3 f43f0000 00000000 ...f.....?......
-  0x00013620 5b947a77 3496a2ff d93f0000 00000000 [.zw4....?......
-  0x00013630 44ef9b59 a7f0b9bf db3f0000 00000000 D..Y.....?......
-  0x00013640 43d1a362 43764d8a e23f0000 00000000 C..bCvM..?......
-  0x00013650 0dafe47c 917673d1 e33f0000 00000000 ...|.vs..?......
-  0x00013660 e5883a67 87ee5bed e83f0000 00000000 ..:g..[..?......
-  0x00013670 f59ef6b2 365a63b6 ea3f0000 00000000 ....6Zc..?......
-  0x00013680 653a4481 36b936ce ee3f0000 00000000 e:D.6.6..?......
-  0x00013690 b780efe9 345748a2 f03f0000 00000000 ....4WH..?......
-  0x000136a0 e35f24ab 335059c0 f33f0000 00000000 ._$.3PY..?......
-  0x000136b0 87334749 e156dd9d f53f0000 00000000 .3GI.V...?......
-  0x000136c0 46774eda 7bebc5ba f73f0000 00000000 FwN.{....?......
-  0x000136d0 9ea1cb52 a68baca6 f93f0000 00000000 ...R.....?......
-  0x000136e0 fb0b7cda 79d7aea2 fa3f0000 00000000 ..|.y....?......
-  0x000136f0 ddf116e4 9da6adb2 fc3f0000 00000000 .........?......
-  0x00013700 f64370a4 036afad3 fa3f0000 00000000 .Cp..j...?......
-  0x00013710 64813e7c 5f4396a3 fe3f0000 00000000 d.>|_C...?......
-  0x00013720 48b52c01 f4af77bb fd3f0000 00000000 H.,...w..?......
-  0x00013730 0270b138 909b4fc4 fe3f0000 00000000 .p.8..O..?......
-  0x00013740 7dbb1d9c e6f518a9 cd3f0000 00000000 }........?......
-  0x00013750 3c992cea d970a5fd d53f0000 00000000 <.,..p...?......
-  0x00013760 df5bd91b adb78d9d dd3f0000 00000000 .[.......?......
-  0x00013770 8445b918 df47f8d2 e33f0000 00000000 .E...G...?......
-  0x00013780 48b906c2 ded414a6 e93f0000 00000000 H........?......
-  0x00013790 3f4dcac4 8b56739d ee3f0000 00000000 ?M...Vs..?......
-  0x000137a0 33a79161 0b1cfcb0 f23f0000 00000000 3..a.....?......
-  0x000137b0 da29262f 60f4fade f53f0000 00000000 .)&/`....?......
-  0x000137c0 f44b6218 71192c8b f83f0000 00000000 .Kb.q.,..?......
-  0x000137d0 fb5de815 fdba25fd f83f0000 00000000 .]....%..?......
-  0x000137e0 69bdcca5 1823598f e4bf0000 00000000 i....#Y.........
-  0x000137f0 784b2622 6bfddbfa e63f0000 00000000 xK&"k....?......
-  0x00013800 64b154e7 83c656ff ea3f0000 00000000 d.T...V..?......
-  0x00013810 a6e4aece 606dc7fe ed3f0000 00000000 ....`m...?......
-  0x00013820 945e40a8 10c47f84 f03f0000 00000000 .^@......?......
-  0x00013830 5c4597e7 e2f019b5 f33f0000 00000000 \E.......?......
-  0x00013840 fca5e902 6ce8cfd8 f03f0000 00000000 ....l....?......
-  0x00013850 50f03034 4f1748cd f73f0000 00000000 P.04O.H..?......
-  0x00013860 e973152e b8d9b8c5 f83f0000 00000000 .s.......?......
-  0x00013870 75b30a5a 2ce8d98a fa3f0000 00000000 u..Z,....?......
-  0x00013880 3df0ed62 ed482f99 fc3f0000 00000000 =..b.H/..?......
-  0x00013890 b61c2cb1 2055c783 fc3f0000 00000000 ..,. U...?......
-  0x000138a0 4f1c1044 e52fa591 fd3f0000 00000000 O..D./...?......
-  0x000138b0 d8d4a9af bbada1da fe3f0000 00000000 .........?......
-  0x000138c0 034c29cd c0a835a2 fe3f0000 00000000 .L)...5..?......
-  0x000138d0 05450867 51e7dddb fc3f0000 00000000 .E.gQ....?......
-  0x000138e0 e24ec075 38bf46fb f93f0000 00000000 .N.u8.F..?......
-  0x000138f0 83db892b 53f5adaa d33f0000 00000000 ...+S....?......
-  0x00013900 85ef4c44 28fc58bd db3f0000 00000000 ..LD(.X..?......
-  0x00013910 59cda902 449d20aa e23f0000 00000000 Y...D. ..?......
-  0x00013920 3c7451e7 932b10a0 e83f0000 00000000 <tQ..+...?......
-  0x00013930 c1731ee9 d4e357aa ed3f0000 00000000 .s....W..?......
-  0x00013940 9972d289 9f36bece f13f0000 00000000 .r...6...?......
-  0x00013950 ebf9a544 2126fb88 f53f0000 00000000 ...D!&...?......
-  0x00013960 7287751d 735989b0 f73f0000 00000000 r.u.sY...?......
-  0x00013970 7d10a760 5cb387a3 f83f0000 00000000 }..`\....?......
-  0x00013980 90efbe34 0c0f8482 e73f0000 00000000 ...4.....?......
-  0x00013990 82cd56bb ed90d492 ea3f0000 00000000 ..V......?......
-  0x000139a0 8783798e a265648d ed3f0000 00000000 ..y..ed..?......
-  0x000139b0 44340299 64d93edc f03f0000 00000000 D4..d.>..?......
-  0x000139c0 ef65877c 8487378b e63f0000 00000000 .e.|..7..?......
-  0x000139d0 e21ad34d 635950c1 f53f0000 00000000 ...McYP..?......
-  0x000139e0 c64283d0 78c21f8d f73f0000 00000000 .B..x....?......
-  0x000139f0 3794e4b7 a39ae987 f83f0000 00000000 7........?......
-  0x00013a00 c0e90686 b484148a fb3f0000 00000000 .........?......
-  0x00013a10 362da058 63450c83 fc3f0000 00000000 6-.XcE...?......
-  0x00013a20 858e53fb 6a816fdf f73f0000 00000000 ..S.j.o..?......
-  0x00013a30 7426a251 efe366f0 fd3f0000 00000000 t&.Q..f..?......
-  0x00013a40 6b01f602 a212a991 ff3f0000 00000000 k........?......
-  0x00013a50 1fe472d3 42335bcd fe3f0000 00000000 ..r.B3[..?......
-  0x00013a60 4a5bb467 0d6147b4 fd3f0000 00000000 J[.g.aG..?......
-  0x00013a70 cd36c43f 7100c5b5 fb3f0000 00000000 .6.?q....?......
-  0x00013a80 b6302055 0fab92a1 f83f0000 00000000 .0 U.....?......
-  0x00013a90 d538b271 67d39fea d53f0000 00000000 .8.qg....?......
-  0x00013aa0 86db1061 43a72482 de3f0000 00000000 ...aC.$..?......
-  0x00013ab0 3e110860 0c87dde9 e43f0000 00000000 >..`.....?......
-  0x00013ac0 912c658f b1d207dc ea3f0000 00000000 .,e......?......
-  0x00013ad0 3a15b596 198329ea ef3f0000 00000000 :.....)..?......
-  0x00013ae0 45616b1f fd76198e f43f0000 00000000 Eak..v...?......
-  0x00013af0 a07b7d61 36ff4cbc f73f0000 00000000 .{}a6.L..?......
-  0x00013b00 d1ef288f 14f6acf2 f93f0000 00000000 ..(......?......
-  0x00013b10 638283e9 7cddcbe0 fa3f0000 00000000 c...|....?......
-  0x00013b20 3e83356f fb26edee e9bf0000 00000000 >.5o.&..........
-  0x00013b30 3bca74dc cc0a43a4 ed3f0000 00000000 ;.t...C..?......
-  0x00013b40 3bca74dc cc0a43a4 ee3f0000 00000000 ;.t...C..?......
-  0x00013b50 e9239175 76f2209f f33f0000 00000000 .#.uv. ..?......
-  0x00013b60 e27c9ca2 8410618f f53f0000 00000000 .|....a..?......
-  0x00013b70 d95fa047 17784fd6 f53f0000 00000000 ._.G.xO..?......
-  0x00013b80 011c2dba 732695b3 f93f0000 00000000 ..-.s&...?......
-  0x00013b90 7af6402a 0ccc8f83 fb3f0000 00000000 z.@*.....?......
-  0x00013ba0 8b877aa4 884b5285 fb3f0000 00000000 ..z..KR..?......
-  0x00013bb0 6e9bb55a 76bdacde fb3f0000 00000000 n..Zv....?......
-  0x00013bc0 ce9a7255 5f5900ff fd3f0000 00000000 ..rU_Y...?......
-  0x00013bd0 c10d6dbc c54c2fe5 fe3f0000 00000000 ..m..L/..?......
-  0x00013be0 4d2cc8d5 fcc828c1 fe3f0000 00000000 M,....(..?......
-  0x00013bf0 e94ce641 7d3c97c6 fd3f0000 00000000 .L.A}<...?......
-  0x00013c00 6e10aaf3 25fd2686 fc3f0000 00000000 n...%.&..?......
-  0x00013c10 c86b80ca 87e1b2d7 f93f0000 00000000 .k.......?......
-  0x00013c20 d71f4693 a82fdf9c f63f0000 00000000 ..F../...?......
-  0x00013c30 71baa30a 309771f0 d93f0000 00000000 q...0.q..?......
-  0x00013c40 6bd1e6a5 dc015f85 e23f0000 00000000 k....._..?......
-  0x00013c50 dbeadad6 1e79aaef e83f0000 00000000 .....y...?......
-  0x00013c60 974f0841 72ec7ce1 ee3f0000 00000000 .O.Ar.|..?......
-  0x00013c70 f4a8a751 a457f8ef f33f0000 00000000 ...Q.W...?......
-  0x00013c80 0cd330a7 70bc9f91 f83f0000 00000000 ..0.p....?......
-  0x00013c90 5517d425 78a0f8c0 fb3f0000 00000000 U..%x....?......
-  0x00013ca0 f1e8fdd8 32d9b1f8 fd3f0000 00000000 ....2....?......
-  0x00013cb0 ee02577f fd395fe6 fe3f0000 00000000 ..W..9_..?......
-  0x00013cc0 454d1fe7 16af4399 e23f0000 00000000 EM....C..?......
-  0x00013cd0 9620e7a0 dc9a94bf e43f0000 00000000 . .......?......
-  0x00013ce0 2c26aee9 637dcaba e93f0000 00000000 ,&..c}...?......
-  0x00013cf0 c02128ae 6a6676f5 eb3f0000 00000000 .!(.jfv..?......
-  0x00013d00 d6ed27fe 696311a3 ef3f0000 00000000 ..'.ic...?......
-  0x00013d10 350b7c6d ae96c7ea f13f0000 00000000 5.|m.....?......
-  0x00013d20 7ba4b711 5e3d9ee9 f33f0000 00000000 {...^=...?......
-  0x00013d30 15e0e0ed 005610ce f63f0000 00000000 .....V...?......
-  0x00013d40 5af002e5 376e31b9 f63f0000 00000000 Z...7n1..?......
-  0x00013d50 312d096c 9aba32a6 fa3f0000 00000000 1-.l..2..?......
-  0x00013d60 b3e17d6a a36f6989 fa3f0000 00000000 ..}j.oi..?......
-  0x00013d70 9d6ba4a9 23d626c7 fc3f0000 00000000 .k..#.&..?......
-  0x00013d80 7f689ec8 aeab26cd fd3f0000 00000000 .h....&..?......
-  0x00013d90 66cdfe59 42385d9d fb3f0000 00000000 f..YB8]..?......
-  0x00013da0 b36c8ff7 f4a0889d ff3f0000 00000000 .l.......?......
-  0x00013db0 e0477335 32c9eaa4 fe3f0000 00000000 .Gs52....?......
-  0x00013dc0 19d3f55d 5b07ef83 fc3f0000 00000000 ...][....?......
-  0x00013dd0 6055f5e4 40f3ac9f d33f0000 00000000 `U..@....?......
-  0x00013de0 b62a00fe dbdd23b1 db3f0000 00000000 .*....#..?......
-  0x00013df0 35ba3773 07b8289f e23f0000 00000000 5.7s..(..?......
-  0x00013e00 588d7ffc ae61be95 e83f0000 00000000 X....a...?......
-  0x00013e10 82b0b005 4a6e5c9f ed3f0000 00000000 ....Jn\..?......
-  0x00013e20 1f4d2241 4afd69c1 f13f0000 00000000 .M"AJ.i..?......
-  0x00013e30 ba9f8181 a4522680 f53f0000 00000000 .....R&..?......
-  0x00013e40 b8d5aec9 6eac27a5 f73f0000 00000000 ....n.'..?......
-  0x00013e50 9ba1687e 13b1fc98 f83f0000 00000000 ..h~.....?......
-  0x00013e60 a4a3561c 240a61db e0bf0000 00000000 ..V.$.a.........
-  0x00013e70 1978e19f 682bcdf6 e33f0000 00000000 .x..h+...?......
-  0x00013e80 ec508f64 38cc17dd e73f0000 00000000 .P.d8....?......
-  0x00013e90 b2c4e2f3 0fc21296 eb3f0000 00000000 .........?......
-  0x00013ea0 ed43be78 10e4f6dc ec3f0000 00000000 .C.x.....?......
-  0x00013eb0 120b9b07 02457afd f03f0000 00000000 .....Ez..?......
-  0x00013ec0 6608332c 00711bf1 f03f0000 00000000 f.3,.q...?......
-  0x00013ed0 84eb0005 709468a4 f53f0000 00000000 ....p.h..?......
-  0x00013ee0 9dc22ff7 7c45eb88 f73f0000 00000000 ../.|E...?......
-  0x00013ef0 14b4c812 53dfa9ac f73f0000 00000000 ....S....?......
-  0x00013f00 bf9f4730 2f349bd7 fa3f0000 00000000 ..G0/4...?......
-  0x00013f10 a715f48e 6c364abf fb3f0000 00000000 ....l6J..?......
-  0x00013f20 a873fcd2 1c7c23d9 fa3f0000 00000000 .s...|#..?......
-  0x00013f30 ece0aad0 278f6480 fe3f0000 00000000 ....'.d..?......
-  0x00013f40 81fc5b0c a469d58e ff3f0000 00000000 ..[..i...?......
-  0x00013f50 b1315262 b7afd0c7 fe3f0000 00000000 .1Rb.....?......
-  0x00013f60 5b9b208c c382daae fd3f0000 00000000 [. ......?......
-  0x00013f70 3929e092 6a951bb0 fb3f0000 00000000 9)..j....?......
-  0x00013f80 f97955f4 ec4b8a9c f83f0000 00000000 .yU..K...?......
-  0x00013f90 d5226dca b8e460f0 cc3f0000 00000000 ."m...`..?......
-  0x00013fa0 20dad197 8aab48b4 d53f0000 00000000  .....H..?......
-  0x00013fb0 836beb84 5be7f7df dc3f0000 00000000 .k..[....?......
-  0x00013fc0 7fdba7e3 f667f395 e33f0000 00000000 .....g...?......
-  0x00013fd0 e2e50d0e 694817ec e83f0000 00000000 ....iH...?......
-  0x00013fe0 6a07dd13 8767d2df ed3f0000 00000000 j....g...?......
-  0x00013ff0 5737c882 a73097fb f13f0000 00000000 W7...0...?......
-  0x00014000 9841b4c1 e4c97c9e f53f0000 00000000 .A....|..?......
-  0x00014010 50e5358d 94b0d6c5 f73f0000 00000000 P.5......?......
-  0x00014020 be14e8be c2e5edb3 f83f0000 00000000 .........?......
-  0x00014030 39655154 82cedcbc e33f0000 00000000 9eQT.....?......
-  0x00014040 97f5f799 f9cdd781 e73f0000 00000000 .........?......
-  0x00014050 9089ee09 da1f5bdb e93f0000 00000000 ......[..?......
-  0x00014060 11f80ee7 a186f5e7 ed3f0000 00000000 .........?......
-  0x00014070 74f8c5ad a49fe5db ed3f0000 00000000 t........?......
-  0x00014080 186f8bcb cad923ea f23f0000 00000000 .o....#..?......
-  0x00014090 1008e762 9fdebcf8 f43f0000 00000000 ...b.....?......
-  0x000140a0 8e9c7a28 481215e1 f43f0000 00000000 ..z(H....?......
-  0x000140b0 7403f03a 29a2e081 f93f0000 00000000 t..:)....?......
-  0x000140c0 1331e2f7 f9095ab5 fa3f0000 00000000 .1....Z..?......
-  0x000140d0 bc40994a a7f8b7cc f93f0000 00000000 .@.J.....?......
-  0x000140e0 21ffd410 70dfb4a5 fc3f0000 00000000 !...p....?......
-  0x000140f0 cc730db2 7cce378b fe3f0000 00000000 .s..|.7..?......
-  0x00014100 cfc5c751 11d1d4ea fe3f0000 00000000 ...Q.....?......
-  0x00014110 54ddc6c9 70cfffbe fe3f0000 00000000 T...p....?......
-  0x00014120 a31ac244 e6584bc3 fd3f0000 00000000 ...D.XK..?......
-  0x00014130 546c5a74 d4499683 fc3f0000 00000000 TlZt.I...?......
-  0x00014140 104a79e4 10b25fd3 f93f0000 00000000 .Jy..._..?......
-  0x00014150 af7b6fbd ddf5b999 f63f0000 00000000 .{o......?......
-  0x00014160 584c99c1 f1f434b4 cf3f0000 00000000 XL....4..?......
-  0x00014170 42f93251 b5b72787 d83f0000 00000000 B.2Q..'..?......
-  0x00014180 38db87f8 708fe7a7 df3f0000 00000000 8...p....?......
-  0x00014190 51fa9adc b283d4e0 e53f0000 00000000 Q........?......
-  0x000141a0 c7b84d9b b919feb0 eb3f0000 00000000 ..M......?......
-  0x000141b0 075933ea a472cba7 f03f0000 00000000 .Y3..r...?......
-  0x000141c0 14b1e3b3 80c29cbc f43f0000 00000000 .........?......
-  0x000141d0 104f902a 2630a1ed f73f0000 00000000 .O.*&0...?......
-  0x000141e0 f4ceb5a2 efca5094 fa3f0000 00000000 ......P..?......
-  0x000141f0 cf404725 d1aae386 fb3f0000 00000000 .@G%.....?......
-  0x00014200 a66719f1 988a01fa e6bf0000 00000000 .g..............
-  0x00014210 36a4e443 9c4021cb ea3f0000 00000000 6..C.@!..?......
-  0x00014220 107f1540 a1d1d084 eb3f0000 00000000 ...@.....?......
-  0x00014230 4ecb703d b2edb1e7 f03f0000 00000000 N.p=.....?......
-  0x00014240 0cd515c5 e714e486 f33f0000 00000000 .........?......
-  0x00014250 2ca6515b ade358e1 f23f0000 00000000 ,.Q[..X..?......
-  0x00014260 1f33e7bf 6d50dcbd f73f0000 00000000 .3..mP...?......
-  0x00014270 063bb0a7 f4033db4 f93f0000 00000000 .;....=..?......
-  0x00014280 77213fc6 f6a6a583 fa3f0000 00000000 w!?......?......
-  0x00014290 504e9d14 af668b8a fa3f0000 00000000 PN...f...?......
-  0x000142a0 6ed0f54d e062a488 fd3f0000 00000000 n..M.b...?......
-  0x000142b0 e5140d23 60a141a7 fe3f0000 00000000 ...#`.A..?......
-  0x000142c0 ed16b229 e26c8c89 ff3f0000 00000000 ...).l...?......
-  0x000142d0 1ea9c622 7ffbbdd6 fe3f0000 00000000 ...".....?......
-  0x000142e0 f47cad0e 67b411f4 fd3f0000 00000000 .|..g....?......
-  0x000142f0 848db08a db96b8c5 fc3f0000 00000000 .........?......
-  0x00014300 c61a7bbe 118e13d9 fa3f0000 00000000 ..{......?......
-  0x00014310 b702899b 88461491 f83f0000 00000000 .....F...?......
-  0x00014320 44c81ed3 bb1b8fb2 f43f0000 00000000 D........?......
-  0x00014330 671b2170 28467493 d43f0000 00000000 g.!p(Ft..?......
-  0x00014340 1aa931a8 3c692edd dc3f0000 00000000 ..1.<i...?......
-  0x00014350 ce786951 16486389 e43f0000 00000000 .xiQ.Hc..?......
-  0x00014360 1aa3ac98 7d98f7b7 ea3f0000 00000000 ....}....?......
-  0x00014370 52d5d918 e1f8d290 f03f0000 00000000 R........?......
-  0x00014380 f6dae78c 4f474c89 f53f0000 00000000 ....OGL..?......
-  0x00014390 3e59aa34 6afc549a f93f0000 00000000 >Y.4j.T..?......
-  0x000143a0 079bf6a1 8bbb70c2 fc3f0000 00000000 ......p..?......
-  0x000143b0 af277a1a 5fe6b7f2 fe3f0000 00000000 .'z._....?......
-  0x000143c0 a7fe1f3a f60bbfdc ff3f0000 00000000 ...:.....?......
-  0x000143d0 0da28a08 76671c8b de3f0000 00000000 ....vg...?......
-  0x000143e0 969bf28e 0eb571f3 e03f0000 00000000 ......q..?......
-  0x000143f0 260914e8 4c2ab6c4 e53f0000 00000000 &...L*...?......
-  0x00014400 bab10034 548056bb e83f0000 00000000 ...4T.V..?......
-  0x00014410 2b31f153 ef490dc0 eb3f0000 00000000 +1.S.I...?......
-  0x00014420 696d5e41 0ed697d7 ee3f0000 00000000 im^A.....?......
-  0x00014430 ef9b9734 6711e782 f03f0000 00000000 ...4g....?......
-  0x00014440 de567afc 96c4d1e2 f33f0000 00000000 .Vz......?......
-  0x00014450 954abd8a deb80fa3 f23f0000 00000000 .J.......?......
-  0x00014460 2b8b53cf aff085d4 f73f0000 00000000 +.S......?......
-  0x00014470 f304bbde f69b68e6 f83f0000 00000000 ......h..?......
-  0x00014480 effe281d a2c1f4eb f93f0000 00000000 ..(......?......
-  0x00014490 eda145ce cb8da790 fc3f0000 00000000 ..E......?......
-  0x000144a0 7c297ce2 51e2ccf3 fb3f0000 00000000 |)|.Q....?......
-  0x000144b0 462c7259 c9687a95 fd3f0000 00000000 F,rY.hz..?......
-  0x000144c0 03366f84 f1aa70db fe3f0000 00000000 .6o...p..?......
-  0x000144d0 d01ffc55 770608a2 fe3f0000 00000000 ...Uw....?......
-  0x000144e0 ac3779d6 500b8edb fc3f0000 00000000 .7y.P....?......
-  0x000144f0 7bf66587 a57aebfa f93f0000 00000000 {.e..z...?......
-  0x00014500 3835dbb8 5b1403d4 cb3f0000 00000000 85..[....?......
-  0x00014510 ea67a4ca 444f029f d43f0000 00000000 .g..DO...?......
-  0x00014520 388edeed 89d689c5 db3f0000 00000000 8........?......
-  0x00014530 cd477f69 a9674184 e23f0000 00000000 .G.i.gA..?......
-  0x00014540 cab96630 c5fe3ad0 e73f0000 00000000 ..f0..:..?......
-  0x00014550 779bbf89 8fc368c5 ec3f0000 00000000 w.....h..?......
-  0x00014560 fbcc5043 dfa8e6dd f03f0000 00000000 ..PC.....?......
-  0x00014570 f8857666 5ee5c88b f43f0000 00000000 ..vf^....?......
-  0x00014580 e4211711 5a007eae f63f0000 00000000 .!..Z.~..?......
-  0x00014590 3ebbc256 b83fb29e f73f0000 00000000 >..V.?...?......
-  0x000145a0 29c3a66a 717282c2 e8bf0000 00000000 )..jqr..........
-  0x000145b0 2ca652f9 adaeb985 ec3f0000 00000000 ,.R......?......
-  0x000145c0 2ca652f9 adaeb985 ed3f0000 00000000 ,.R......?......
-  0x000145d0 fb108889 38e18b81 f23f0000 00000000 ....8....?......
-  0x000145e0 ba980f81 8b703bc5 f33f0000 00000000 .....p;..?......
-  0x000145f0 2aceab10 0d17d5ba f53f0000 00000000 *........?......
-  0x00014600 d9bb9601 90a203bb f83f0000 00000000 .........?......
-  0x00014610 3ffc1f2d 0f45b4bd f93f0000 00000000 ?..-.E...?......
-  0x00014620 258f9f6a acae90b9 f93f0000 00000000 %..j.....?......
-  0x00014630 40951a6c 2a8ba8e9 fc3f0000 00000000 @..l*....?......
-  0x00014640 0f1b3c6e c40a3d9a fe3f0000 00000000 ..<n..=..?......
-  0x00014650 6a8ca1f1 92bf2af2 fe3f0000 00000000 j.....*..?......
-  0x00014660 2f799298 d08629bc fe3f0000 00000000 /y....)..?......
-  0x00014670 d3c04390 a4e7f4be fd3f0000 00000000 ..C......?......
-  0x00014680 0d108399 25773580 fc3f0000 00000000 ....%w5..?......
-  0x00014690 6209d2e4 1043adcd f93f0000 00000000 b....C...?......
-  0x000146a0 8def5249 0c489595 f63f0000 00000000 ..RI.H...?......
-  0x000146b0 056ae6b2 2a6ca9b7 d53f0000 00000000 .j..*l...?......
-  0x000146c0 9d9d775e fff3bfcb dd3f0000 00000000 ..w^.....?......
-  0x000146d0 35438a1f dd5311b7 e43f0000 00000000 5C...S...?......
-  0x000146e0 4efa7df2 c4e93cac ea3f0000 00000000 N.}...<..?......
-  0x000146f0 d14d9939 c1ce4cb7 ef3f0000 00000000 .M.9..L..?......
-  0x00014700 8b140e0b 88e777de f33f0000 00000000 ......w..?......
-  0x00014710 92bf4a36 1e706693 f73f0000 00000000 ..J6.pf..?......
-  0x00014720 904b60a0 5edcf6bd f93f0000 00000000 .K`.^....?......
-  0x00014730 39759e6b 81f3f7af fa3f0000 00000000 9u.k.....?......
-  0x00014740 84703972 55575bc4 eb3f0000 00000000 .p9rUW[..?......
-  0x00014750 6babce6c f5368a9f ef3f0000 00000000 k..l.6...?......
-  0x00014760 7442f2c3 6aeccfab f03f0000 00000000 tB..j....?......
-  0x00014770 fed534bf 16f0988b f43f0000 00000000 ..4......?......
-  0x00014780 068e2b85 c9a4cc83 f73f0000 00000000 ..+......?......
-  0x00014790 f18779fd ae9c28b0 f83f0000 00000000 ..y...(..?......
-  0x000147a0 6babce6c f5368a9f f13f0000 00000000 k..l.6...?......
-  0x000147b0 a7d7341c 7598a9b9 fb3f0000 00000000 ..4.u....?......
-  0x000147c0 8a7592fd 212406aa fd3f0000 00000000 .u..!$...?......
-  0x000147d0 fd2f60bd a4fd20b2 fe3f0000 00000000 ./`... ..?......
-  0x000147e0 2643c8dd 24135185 ff3f0000 00000000 &C..$.Q..?......
-  0x000147f0 2299710f 3feaa4cc fe3f0000 00000000 ".q.?....?......
-  0x00014800 713acace ed4068e6 fd3f0000 00000000 q:...@h..?......
-  0x00014810 99b56e66 373eb0b9 fc3f0000 00000000 ..nf7>...?......
-  0x00014820 db2a40a3 f7f554cb fa3f0000 00000000 .*@...T..?......
-  0x00014830 3286c0d5 c31bc187 f83f0000 00000000 2........?......
-  0x00014840 3ee0b1df 7a0e15a7 f43f0000 00000000 >...z....?......
-  0x00014850 039106bd b1a9abca d93f0000 00000000 .........?......
-  0x00014860 df48b32d 4170d6e0 e13f0000 00000000 .H.-Ap...?......
-  0x00014870 9307d635 89d303ca e83f0000 00000000 ...5.....?......
-  0x00014880 94457683 7f7810be ee3f0000 00000000 .Ev..x...?......
-  0x00014890 6a1378cd 637645ca f33f0000 00000000 j.x.cvE..?......
-  0x000148a0 3620147b b0597ef5 f73f0000 00000000 6 .{.Y~..?......
-  0x000148b0 6d86ee7a dde6a7a2 fb3f0000 00000000 m..z.....?......
-  0x000148c0 dec96072 0117a0d1 fd3f0000 00000000 ..`r.....?......
-  0x000148d0 a3c5b451 985a2ec2 fe3f0000 00000000 ...Q.Z...?......
-  0x000148e0 577fff9f a5424594 e63f0000 00000000 W....BE..?......
-  0x000148f0 416fff53 faeacda6 e93f0000 00000000 Ao.S.....?......
-  0x00014900 481faac2 885da0a0 ec3f0000 00000000 H....]...?......
-  0x00014910 e226ff7d 77e034fa ef3f0000 00000000 .&.}w.4..?......
-  0x00014920 2b2bccdd ecce43ba ed3f0000 00000000 ++....C..?......
-  0x00014930 6e9cdf84 885fc0e8 f43f0000 00000000 n...._...?......
-  0x00014940 147dfb3b e9709d9f f63f0000 00000000 .}.;.p...?......
-  0x00014950 1e2fb06c 7ffa61c9 f73f0000 00000000 ./.l..a..?......
-  0x00014960 460cc672 53ec86aa fa3f0000 00000000 F..rS....?......
-  0x00014970 67da6229 593c02ec fa3f0000 00000000 g.b)Y<...?......
-  0x00014980 173b1b60 73c37ed9 fb3f0000 00000000 .;.`s.~..?......
-  0x00014990 326ff693 9afb418a fe3f0000 00000000 2o....A..?......
-  0x000149a0 76ca4b80 9dea528b ff3f0000 00000000 v.K...R..?......
-  0x000149b0 6185569e 8b95e7c0 fe3f0000 00000000 a.V......?......
-  0x000149c0 80490b10 0e4013a8 fd3f0000 00000000 .I...@...?......
-  0x000149d0 6aae5b19 69b607a9 fb3f0000 00000000 j.[.i....?......
-  0x000149e0 5ef06d4f 96be3f96 f83f0000 00000000 ^.mO..?..?......
-  0x000149f0 3b9ef20e 8506ccbf d33f0000 00000000 ;........?......
-  0x00014a00 8a27959c 3b57c6d4 db3f0000 00000000 .'..;W...?......
-  0x00014a10 503dc2a8 8f312dbf e23f0000 00000000 P=...1-..?......
-  0x00014a20 b1b9f6bd 20faddb3 e83f0000 00000000 .... ....?......
-  0x00014a30 d63d4b98 ea4e6bbf ed3f0000 00000000 .=K..Nk..?......
-  0x00014a40 da8ac412 508c52e8 f13f0000 00000000 ....P.R..?......
-  0x00014a50 d8e168f6 96dbed99 f53f0000 00000000 ..h......?......
-  0x00014a60 7fcc18a3 0aee60c6 f73f0000 00000000 ......`..?......
-  0x00014a70 096e097d 5c51c3b7 f83f0000 00000000 .n.}\Q...?......
-  0x00014a80 79b31a8d ac5002df e5bf0000 00000000 y....P..........
-  0x00014a90 d2b1a532 8ce131b5 e93f0000 00000000 ...2..1..?......
-  0x00014aa0 b05eec55 b775f2ec e93f0000 00000000 .^.U.u...?......
-  0x00014ab0 d3fec4e9 43e5acce ef3f0000 00000000 ....C....?......
-  0x00014ac0 089f13f5 27f3e6d3 f13f0000 00000000 ....'....?......
-  0x00014ad0 0164292c da8dae8f f33f0000 00000000 .d),.....?......
-  0x00014ae0 a24f667d 4b3899d9 f63f0000 00000000 .Of}K8...?......
-  0x00014af0 78b0efda eb300e9a f83f0000 00000000 x....0...?......
-  0x00014b00 45b02f7d 8d4927f2 f53f0000 00000000 E./}.I'..?......
-  0x00014b10 c9682162 5b1ee2bd fb3f0000 00000000 .h!b[....?......
-  0x00014b20 80d92717 c73bd9aa fd3f0000 00000000 ..'..;...?......
-  0x00014b30 73ebccd8 0f6354b2 fe3f0000 00000000 s....cT..?......
-  0x00014b40 30539a3e 08294385 ff3f0000 00000000 0S.>.)C..?......
-  0x00014b50 96bf0d1b 38da86cc fe3f0000 00000000 ....8....?......
-  0x00014b60 b42cb153 340642e6 fd3f0000 00000000 .,.S4.B..?......
-  0x00014b70 d0a8f612 29c08fb9 fc3f0000 00000000 ....)....?......
-  0x00014b80 b37aca46 688130cb fa3f0000 00000000 .z.Fh.0..?......
-  0x00014b90 b441e360 678aa887 f83f0000 00000000 .A.`g....?......
-  0x00014ba0 a29fdc4f bad1f6a6 f43f0000 00000000 ...O.....?......
-  0x00014bb0 0c91391f 64316d90 d03f0000 00000000 ..9.d1m..?......
-  0x00014bc0 9259d62e 16caa3d8 d83f0000 00000000 .Y.......?......
-  0x00014bd0 fbdc6fef 121d9186 e03f0000 00000000 ..o......?......
-  0x00014be0 16b44787 479630b4 e63f0000 00000000 ..G.G.0..?......
-  0x00014bf0 43efbe01 45b7d98d ec3f0000 00000000 C...E....?......
-  0x00014c00 724a260c 36957a86 f13f0000 00000000 rJ&.6.z..?......
-  0x00014c10 506f0177 9bc02997 f53f0000 00000000 Po.w..)..?......
-  0x00014c20 d56c1550 27ac72be f83f0000 00000000 .l.P'.r..?......
-  0x00014c30 4be980bc 0212bced fa3f0000 00000000 K........?......
-  0x00014c40 f4900677 30b636d8 fb3f0000 00000000 ...w0.6..?......
-  0x00014c50 a301c6ee 2eccc3c5 e83f0000 00000000 .........?......
-  0x00014c60 89a1d9ff 6b8f67b9 ec3f0000 00000000 ....k.g..?......
-  0x00014c70 1a096d88 2f8ddf84 ee3f0000 00000000 ..m./....?......
-  0x00014c80 85b2848a ed2579b7 f13f0000 00000000 .....%y..?......
-  0x00014c90 36b0fdca 5fc697d6 f43f0000 00000000 6..._....?......
-  0x00014ca0 9847db5b 421c70b1 f63f0000 00000000 .G.[B.p..?......
-  0x00014cb0 771c594f 1199ae92 f53f0000 00000000 w.YO.....?......
-  0x00014cc0 5b3b497f 8820abd1 f93f0000 00000000 [;I.. ...?......
-  0x00014cd0 06d1780c cc9609f6 fb3f0000 00000000 ..x......?......
-  0x00014ce0 12e4098f 374936a1 fd3f0000 00000000 ....7I6..?......
-  0x00014cf0 f65711bc 1601a292 fe3f0000 00000000 .W.......?......
-  0x00014d00 9d90955a 5d25f7c5 fe3f0000 00000000 ...Z]%...?......
-  0x00014d10 c24b298c ee69c6cb fe3f0000 00000000 .K)..i...?......
-  0x00014d20 c91a95e1 644c51a1 fe3f0000 00000000 ....dLQ..?......
-  0x00014d30 5d6b5136 136bb4c3 fd3f0000 00000000 ]kQ6.k...?......
-  0x00014d40 da6602ae 01591ab3 fc3f0000 00000000 .f...Y...?......
-  0x00014d50 03197f82 a036bdef fa3f0000 00000000 .....6...?......
-  0x00014d60 70f96f94 6118c2dd f83f0000 00000000 p.o.a....?......
-  0x00014d70 2ac60f52 ead8a6fd f53f0000 00000000 *..R.....?......
-  0x00014d80 e39c3ba3 27eb4787 f23f0000 00000000 ..;.'.G..?......
-  0x00014d90 2efd6b6f a0729df3 e23f0000 00000000 ..ko.r...?......
-  0x00014da0 0f3e9a4c ce3e7ca7 e63f0000 00000000 .>.L.>|..?......
-  0x00014db0 b20b0ad6 3b6f798d e93f0000 00000000 ....;oy..?......
-  0x00014dc0 6f1b179b 19509a95 ed3f0000 00000000 o....P...?......
-  0x00014dd0 47f0f76a 84bd36e5 ec3f0000 00000000 G..j..6..?......
-  0x00014de0 b90450f6 55725da0 f23f0000 00000000 ..P.Ur]..?......
-  0x00014df0 426d214e 8a59c5a1 f43f0000 00000000 Bm!N.Y...?......
-  0x00014e00 7e9f84a4 5028e9df f43f0000 00000000 ~...P(...?......
-  0x00014e10 eb1a3e7e 5bbbe4b9 f83f0000 00000000 ..>~[....?......
-  0x00014e20 1d9865a7 0691b1d5 f93f0000 00000000 ..e......?......
-  0x00014e30 c649e4b8 e5d0d7e9 f83f0000 00000000 .I.......?......
-  0x00014e40 2dfdae90 315cb2dc fc3f0000 00000000 -...1\...?......
-  0x00014e50 520187c4 a6514497 fe3f0000 00000000 R....QD..?......
-  0x00014e60 e79b2cf1 3d5eb0f0 fe3f0000 00000000 ..,.=^...?......
-  0x00014e70 827a4e38 b100bebc fe3f0000 00000000 .zN8.....?......
-  0x00014e80 64eed518 3b78d8bf fd3f0000 00000000 d...;x...?......
-  0x00014e90 be1d1085 81e1e680 fc3f0000 00000000 .........?......
-  0x00014ea0 13e2cd1a d28cd8ce f93f0000 00000000 .........?......
-  0x00014eb0 5447c42a 0df26e96 f63f0000 00000000 TG.*..n..?......
-  0x00014ec0 7aa38db4 26c191b9 cd3f0000 00000000 z...&....?......
-  0x00014ed0 9b3a6a07 dd502d8b d63f0000 00000000 .:j..P-..?......
-  0x00014ee0 1f301e16 dda3e6ac dd3f0000 00000000 .0.......?......
-  0x00014ef0 e3475202 6a3f85e7 e33f0000 00000000 .GR.j?...?......
-  0x00014f00 b27f3cd6 7e6942b6 e93f0000 00000000 ..<.~iB..?......
-  0x00014f10 113f8d8e e8b0c9ac ee3f0000 00000000 .?.......?......
-  0x00014f20 b36ba661 ed9639c2 f23f0000 00000000 .k.a..9..?......
-  0x00014f30 f7a9f9bf 3b6db3f4 f53f0000 00000000 ....;m...?......
-  0x00014f40 faa9497d 5da5ba98 f83f0000 00000000 ..I}]....?......
-  0x00014f50 9a963c44 923de78a f93f0000 00000000 ..<D.=...?......
-  0x00014f60 6a47bb8c 33efe7b8 ecbf0000 00000000 jG..3...........
-  0x00014f70 f492ef53 407059ad f03f0000 00000000 ...S@pY..?......
-  0x00014f80 036261f9 28000fe9 f23f0000 00000000 .ba.(....?......
-  0x00014f90 37aef33e 30140382 f33f0000 00000000 7..>0....?......
-  0x00014fa0 7ea30b68 7a88e1d6 f63f0000 00000000 ~..hz....?......
-  0x00014fb0 47e00cf6 9e461fb6 f93f0000 00000000 G....F...?......
-  0x00014fc0 87ea13bd 298c2f9f fb3f0000 00000000 ....)./..?......
-  0x00014fd0 9815a33c 9be503bc fc3f0000 00000000 ...<.....?......
-  0x00014fe0 30bf209c 5c39bba2 fd3f0000 00000000 0. .\9...?......
-  0x00014ff0 d13c8aaf 4249d6d5 fd3f0000 00000000 .<..BI...?......
-  0x00015000 1b851b00 294ca9d8 fd3f0000 00000000 ....)L...?......
-  0x00015010 b0519743 0e3ae2a9 fd3f0000 00000000 .Q.C.:...?......
-  0x00015020 507cced4 722fe3cc fc3f0000 00000000 P|..r/...?......
-  0x00015030 cd4b77aa e6fad5ba fb3f0000 00000000 .Kw......?......
-  0x00015040 74af8163 7edf90f9 f93f0000 00000000 t..c~....?......
-  0x00015050 cf8c4009 0d3d97e6 f73f0000 00000000 ..@..=...?......
-  0x00015060 6982d33f 0658d183 f53f0000 00000000 i..?.X...?......
-  0x00015070 4ebe0333 8f089b8c f13f0000 00000000 N..3.....?......
-  0x00015080 70bc5549 1beefcfc ea3f0000 00000000 p.UI.....?......
-  0x00015090 1ba9952b 76818dcd ee3f0000 00000000 ...+v....?......
-  0x000150a0 e2042be0 57505ddd ef3f0000 00000000 ..+.WP]..?......
-  0x000150b0 f8f32266 47d1dbb3 f33f0000 00000000 .."fG....?......
-  0x000150c0 1d5cdeae 0830399c f63f0000 00000000 .\...09..?......
-  0x000150d0 64f1ba5e fc1ba48a f73f0000 00000000 d..^.....?......
-  0x000150e0 2aab016f b06d1584 f93f0000 00000000 *..o.m...?......
-  0x000150f0 5a2107c9 86a60cf1 fb3f0000 00000000 Z!.......?......
-  0x00015100 0537e48b 0be96eb9 fd3f0000 00000000 .7....n..?......
-  0x00015110 71f3e43b 326c10b7 fe3f0000 00000000 q..;2l...?......
-  0x00015120 65ea113c 9ccf6c83 ff3f0000 00000000 e..<..l..?......
-  0x00015130 3d25c853 823c25c8 fe3f0000 00000000 =%.S.<%..?......
-  0x00015140 8a1873f8 f41955e0 fd3f0000 00000000 ..s...U..?......
-  0x00015150 639e3248 700158b4 fc3f0000 00000000 c.2Hp.X..?......
-  0x00015160 0c0bc8dd 50df3ac5 fa3f0000 00000000 ....P.:..?......
-  0x00015170 dd93bd94 cf859d83 f83f0000 00000000 .........?......
-  0x00015180 e87a5fa3 75f3fca1 f43f0000 00000000 .z_.u....?......
-  0x00015190 7c221fea 95e43daa d73f0000 00000000 |"....=..?......
-  0x000151a0 428aba4f 96a9dcbc df3f0000 00000000 B..O.....?......
-  0x000151b0 b440f99d 54e9b0a9 e63f0000 00000000 .@..T....?......
-  0x000151c0 f8427b31 4b13a79f ec3f0000 00000000 .B{1K....?......
-  0x000151d0 54409f7c 9a0be8a9 f13f0000 00000000 T@.|.....?......
-  0x000151e0 621cecd3 227836ce f53f0000 00000000 b..."x6..?......
-  0x000151f0 eca205df 9c35a188 f93f0000 00000000 .....5...?......
-  0x00015200 b2c5c913 3c7015b0 fb3f0000 00000000 ....<p...?......
-  0x00015210 92ca90bf 56541ca3 fc3f0000 00000000 ....VT...?......
-  0x00015220 b46ff021 829c24f0 e8bf0000 00000000 .o.!..$.........
-  0x00015230 af760f44 4ae626ff ec3f0000 00000000 .v.DJ.&..?......
-  0x00015240 8cd1596d 33393ec6 ef3f0000 00000000 ..Ym39>..?......
-  0x00015250 0aad1e89 7780279a f03f0000 00000000 ....w.'..?......
-  0x00015260 dd1197e6 6033a7cc f33f0000 00000000 ....`3...?......
-  0x00015270 1b7e73ee ac43a1d3 f63f0000 00000000 .~s..C...?......
-  0x00015280 0a9ef7f6 a92a30db f83f0000 00000000 .....*0..?......
-  0x00015290 0d423d12 a82f229a fa3f0000 00000000 .B=../"..?......
-  0x000152a0 b4790dbc 6780d0a0 fb3f0000 00000000 .y..g....?......
-  0x000152b0 6a8c6195 a01d8981 fc3f0000 00000000 j.a......?......
-  0x000152c0 6304689a 50c36ca4 fc3f0000 00000000 c.h.P.l..?......
-  0x000152d0 849d16d3 86620ba6 fc3f0000 00000000 .....b...?......
-  0x000152e0 cef4a086 9b95af85 fc3f0000 00000000 .........?......
-  0x000152f0 8c6583a0 70f4dbaa fb3f0000 00000000 .e..p....?......
-  0x00015300 cc4c5393 ac8e53ab fa3f0000 00000000 .LS...S..?......
-  0x00015310 f32a7782 92000584 f93f0000 00000000 .*w......?......
-  0x00015320 b7fc09e1 e7260a97 f73f0000 00000000 .....&...?......
-  0x00015330 cfde6148 57ddcdf1 f43f0000 00000000 ..aHW....?......
-  0x00015340 d6fd8310 a1dfdcf1 f13f0000 00000000 .........?......
-  0x00015350 8d94d65a 5bb4a2e3 ed3f0000 00000000 ...Z[....?......
-  0x00015360 a30e4e04 65b6e0ab e83f0000 00000000 ..N.e....?......
-  0x00015370 b92d09b4 feaa22a1 ec3f0000 00000000 .-...."..?......
-  0x00015380 ace3c8bd 17f5f5e6 ed3f0000 00000000 .........?......
-  0x00015390 956a7eb7 36f9749f f13f0000 00000000 .j~.6.t..?......
-  0x000153a0 a6541b11 42abf2ad f43f0000 00000000 .T..B....?......
-  0x000153b0 00cefdac 5e7f42d6 f53f0000 00000000 ....^.B..?......
-  0x000153c0 e23c2c6e 0c6eea84 f73f0000 00000000 .<,n.n...?......
-  0x000153d0 608379ed f2eb5eb4 fa3f0000 00000000 `.y...^..?......
-  0x000153e0 9d24d28f 8334dcad fc3f0000 00000000 .$...4...?......
-  0x000153f0 cfd671c9 f19dbfd5 fd3f0000 00000000 ..q......?......
-  0x00015400 d99eaabd 23f6cdbc fe3f0000 00000000 ....#....?......
-  0x00015410 1b888052 ab69f3fa fe3f0000 00000000 ...R.i...?......
-  0x00015420 c1db12dd c52b91c9 fe3f0000 00000000 .....+...?......
-  0x00015430 499dafa4 b7e6b9f3 fd3f0000 00000000 I........?......
-  0x00015440 ff8ccd3f 91619ade fc3f0000 00000000 ...?.a...?......
-  0x00015450 bfc3c33c 9bf5ce94 fb3f0000 00000000 ...<.....?......
-  0x00015460 08873396 8acf8f89 f93f0000 00000000 ..3......?......
-  0x00015470 8ea0ec7b 6e6d4e9d f63f0000 00000000 ...{nmN..?......
-  0x00015480 75de73c8 641fcba7 f23f0000 00000000 u.s.d....?......
-  0x00015490 d5ef5ba4 d05ae9b9 d23f0000 00000000 ..[..Z...?......
-  0x000154a0 e0f3447b 1c046f8b db3f0000 00000000 ..D{..o..?......
-  0x000154b0 17810382 934238ad e23f0000 00000000 .....B8..?......
-  0x000154c0 95e25537 2d8af2e7 e83f0000 00000000 ..U7-....?......
-  0x000154d0 ae4e853c 297398b6 ee3f0000 00000000 .N.<)s...?......
-  0x000154e0 9288308c f4411bad f33f0000 00000000 ..0..A...?......
-  0x000154f0 abf1514c 9a4695c2 f73f0000 00000000 ..QL.F...?......
-  0x00015500 c1926159 d1f026f5 fa3f0000 00000000 ..aY..&..?......
-  0x00015510 3707c924 5abe0299 fd3f0000 00000000 7..$Z....?......
-  0x00015520 02d09842 bdcf288b fe3f0000 00000000 ...B..(..?......
-  0x00015530 702592b0 3a95c9ca e73f0000 00000000 p%..:....?......
-  0x00015540 758cadb1 3561cff0 eb3f0000 00000000 u...5a...?......
-  0x00015550 029ff133 aea67487 ef3f0000 00000000 ...3..t..?......
-  0x00015560 ed4b96c9 7641e5bf f13f0000 00000000 .K..vA...?......
-  0x00015570 ed4b96c9 7641e5bf f33f0000 00000000 .K..vA...?......
-  0x00015580 f2b83017 19f1eb8f f53f0000 00000000 ..0......?......
-  0x00015590 708263f0 4799e8a7 f63f0000 00000000 p.c.G....?......
-  0x000155a0 b11dca83 3045ea9b f73f0000 00000000 ....0E...?......
-  0x000155b0 892cafc5 c867dfe9 f73f0000 00000000 .,...g...?......
-  0x000155c0 8df023ce c114ec8e f83f0000 00000000 ..#......?......
-  0x000155d0 ffffffff ffffff7f 00000000 00000000 ................
+  0x0000d040 0000403f 20bacf3a 20ba4f3c 9333e33d ..@? ..: .O<.3.=
+  0x0000d050 abaaaaaa aaaaaaaa fd3f0000 00000000 .........?......
+  0x0000d060 89888888 88888888 fc3f0000 00000000 .........?......
+  0x0000d070 89888888 88888888 fe3f0000 00000000 .........?......
+  0x0000d080 6edbb66d dbb66ddb fdbf0000 00000000 n..m..m.........
+  0x0000d090 0cc3300c c3300cc3 fcbf0000 00000000 ..0..0..........
+  0x0000d0a0 0cc3300c c3300cc3 fe3f0000 00000000 ..0..0...?......
+  0x0000d0b0 659d2b0f 48d6b9f2 f93f0000 00000000 e.+.H....?......
+  0x0000d0c0 659d2b0f 48d6b9f2 fb3f0000 00000000 e.+.H....?......
+  0x0000d0d0 49922449 92244992 fcbf0000 00000000 I.$I.$I.........
+  0x0000d0e0 6edbb66d dbb66ddb fd3f0000 00000000 n..m..m..?......
+  0x0000d0f0 0cc3300c c3300cc3 fb3f0000 00000000 ..0..0...?......
+  0x0000d100 6edbb66d dbb66ddb fe3f0000 00000000 n..m..m..?......
+  0x0000d110 79fb92e6 d64954b2 f73f0000 00000000 y....IT..?......
+  0x0000d120 526c579b fe7be490 fb3f0000 00000000 RlW..{...?......
+  0x0000d130 e85a65c3 11d39ec8 fc3f0000 00000000 .Ze......?......
+  0x0000d140 8c31c618 638c31c6 fb3f0000 00000000 .1..c.1..?......
+  0x0000d150 29a59452 4a29a594 fe3f0000 00000000 )..RJ)...?......
+  0x0000d160 0b20a900 920a20a9 f73f0000 00000000 . .... ..?......
+  0x0000d170 096a89a0 96086a89 fb3f0000 00000000 .j....j..?......
+  0x0000d180 0c44be40 e40b44be fc3f0000 00000000 .D.@..D..?......
+  0x0000d190 cdcccccc cccccccc fb3f0000 00000000 .........?......
+  0x0000d1a0 d66ca4ea 1aeccb95 f63f0000 00000000 .l.......?......
+  0x0000d1b0 dc304bbd ab5f6bf3 f93f0000 00000000 .0K.._k..?......
+  0x0000d1c0 71faf847 9e6985a8 fb3f0000 00000000 q..G.i...?......
+  0x0000d1d0 00000000 00000080 fe3f0000 00000000 .........?......
+  0x0000d1e0 49922449 92244992 fd3f0000 00000000 I.$I.$I..?......
+  0x0000d1f0 2dc9a8eb abd4a98e f83f0000 00000000 -........?......
+  0x0000d200 79fb92e6 d64954b2 fc3f0000 00000000 y....IT..?......
+  0x0000d210 2dc9a8eb abd4a98e fe3f0000 00000000 -........?......
+  0x0000d220 abaaaaaa aaaaaaaa fc3f0000 00000000 .........?......
+  0x0000d230 abaaaaaa aaaaaaaa fe3f0000 00000000 .........?......
+  0x0000d240 7d9c39b6 2a1defb8 f83f0000 00000000 }.9.*....?......
+  0x0000d250 9d03c863 75e42ae7 fc3f0000 00000000 ...cu.*..?......
+  0x0000d260 7d9c39b6 2a1defb8 fe3f0000 00000000 }.9.*....?......
+  0x0000d270 8de09dc3 9f4ef596 fa3f0000 00000000 .....N...?......
+  0x0000d280 32f721c6 0316ab90 fe3f0000 00000000 2.!......?......
+  0x0000d290 87d6a4ad 8bc5c1ab f83f0000 00000000 .........?......
+  0x0000d2a0 290c0e99 ee36b2d6 fc3f0000 00000000 )....6...?......
+  0x0000d2b0 87d6a4ad 8bc5c1ab fe3f0000 00000000 .........?......
+  0x0000d2c0 455b0d9e 2350b4d5 f9bf0000 00000000 E[..#P..........
+  0x0000d2d0 0b59c842 16b29085 fc3f0000 00000000 .Y.B.....?......
+  0x0000d2e0 fc7549e5 c3b85f97 fc3f0000 00000000 .uI..._..?......
+  0x0000d2f0 38bde94d 6f7ad39b fd3f0000 00000000 8..Moz...?......
+  0x0000d300 b4d5e039 02455b8d ff3f0000 00000000 ...9.E[..?......
+  0x0000d310 210b59c8 4216b290 fe3f0000 00000000 !.Y.B....?......
+  0x0000d320 35788e40 d15683e7 fb3f0000 00000000 5x.@.V...?......
+  0x0000d330 7dbf8eff 247341b9 f23f0000 00000000 }...$sA..?......
+  0x0000d340 895d9987 5950e3a7 f73f0000 00000000 .]..YP...?......
+  0x0000d350 830e9443 bf6192b0 fa3f0000 00000000 ...C.a...?......
+  0x0000d360 6d97809f 89a169d0 fb3f0000 00000000 m.....i..?......
+  0x0000d370 bc4026c5 0b6452bc f83f0000 00000000 .@&..dR..?......
+  0x0000d380 8db0dcd3 08cb3d8d fa3f0000 00000000 ......=..?......
+  0x0000d390 a578814c 8a17c8a4 fb3f0000 00000000 .x.L.....?......
+  0x0000d3a0 e3053229 5e2093e2 fe3f0000 00000000 ..2)^ ...?......
+  0x0000d3b0 fbe59dca 38b9e9ae f13f0000 00000000 ....8....?......
+  0x0000d3c0 6b189f77 dbcf839e f63f0000 00000000 k..w.....?......
+  0x0000d3d0 337f1e21 8ac4b6a6 f93f0000 00000000 3..!.....?......
+  0x0000d3e0 baa2f1e3 5ff0c6c4 fa3f0000 00000000 ...._....?......
+  0x0000d3f0 0feaa00e eaa00eea f93f0000 00000000 .........?......
+  0x0000d400 cdcccccc cccccccc fc3f0000 00000000 .........?......
+  0x0000d410 9a999999 99999999 fe3f0000 00000000 .........?......
+  0x0000d420 aff72724 cfd9e9ad f23f0000 00000000 ..'$.....?......
+  0x0000d430 7738c4b8 63ed9b9d f73f0000 00000000 w8..c....?......
+  0x0000d440 1318766e 99e3c2a5 fa3f0000 00000000 ..vn.....?......
+  0x0000d450 a5f6ac08 0915a7c3 fb3f0000 00000000 .........?......
+  0x0000d460 0533feed 4bf7a899 f5bf0000 00000000 .3..K...........
+  0x0000d470 884cfde4 f1727de6 f63f0000 00000000 .L...r}..?......
+  0x0000d480 27863d67 085448d3 f93f0000 00000000 '.=g.TH..?......
+  0x0000d490 feea2dcb ef5dabb1 fb3f0000 00000000 ..-..]...?......
+  0x0000d4a0 f8b3074d 0217e6fc fb3f0000 00000000 ...M.....?......
+  0x0000d4b0 6b2fda85 3a49dc9a fe3f0000 00000000 k/..:I...?......
+  0x0000d4c0 278747cb f0670f9a fd3f0000 00000000 '.G..g...?......
+  0x0000d4d0 084d0217 e6fce0c9 fe3f0000 00000000 .M.......?......
+  0x0000d4e0 09531988 b5cd4abe ed3f0000 00000000 .S....J..?......
+  0x0000d4f0 105ed52a 911d8fa0 f33f0000 00000000 .^.*.....?......
+  0x0000d500 d3f60908 294912b4 f73f0000 00000000 ....)I...?......
+  0x0000d510 4ba30910 e4b5139b fa3f0000 00000000 K........?......
+  0x0000d520 fb419e8c ccbe3fa7 fb3f0000 00000000 .A....?..?......
+  0x0000d530 a142850a 152a54a8 f73f0000 00000000 .B...*T..?......
+  0x0000d540 4a93264d 9a3469d2 f93f0000 00000000 J.&M.4i..?......
+  0x0000d550 8203070e 1c3870e0 f93f0000 00000000 .....8p..?......
+  0x0000d560 bd7af5ea d5ab57af fd3f0000 00000000 .z....W..?......
+  0x0000d570 4a2ef685 a5e4629f fe3f0000 00000000 J.....b..?......
+  0x0000d580 bd7af5ea d5ab57af fb3f0000 00000000 .z....W..?......
+  0x0000d590 a142850a 152a54a8 ff3f0000 00000000 .B...*T..?......
+  0x0000d5a0 4a93264d 9a3469b2 fe3f0000 00000000 J.&M.4i..?......
+  0x0000d5b0 08a9eb70 7b90ba8e fc3f0000 00000000 ...p{....?......
+  0x0000d5c0 e9c06165 74b1a784 f03f0000 00000000 ..aet....?......
+  0x0000d5d0 89f5146b 74fbdadf f53f0000 00000000 ...kt....?......
+  0x0000d5e0 9881dfc9 585f0ffb f93f0000 00000000 ....X_...?......
+  0x0000d5f0 ab933df6 fa5136d8 fc3f0000 00000000 ..=..Q6..?......
+  0x0000d600 19d5359a eec52ee9 fd3f0000 00000000 ..5......?......
+  0x0000d610 b69e6d74 51e80b8e f43f0000 00000000 ..mtQ....?......
+  0x0000d620 8c52fba2 5b65cd9f f93f0000 00000000 .R..[e...?......
+  0x0000d630 e39e4d33 f26e0de3 fc3f0000 00000000 ..M3.n...?......
+  0x0000d640 5be425eb 1d70a2cd fe3f0000 00000000 [.%..p...?......
+  0x0000d650 dcc5e99a 75ad519e ee3f0000 00000000 ....u.Q..?......
+  0x0000d660 f13eb53a 5bea9485 f43f0000 00000000 .>.:[....?......
+  0x0000d670 7bb7d789 64cad095 f83f0000 00000000 {...d....?......
+  0x0000d680 dec25ef7 fb4f0581 fb3f0000 00000000 ..^..O...?......
+  0x0000d690 e676275d 74c9258b fc3f0000 00000000 .v']t.%..?......
+  0x0000d6a0 ae8940ae 8940ae89 f7bf0000 00000000 ..@..@..........
+  0x0000d6b0 f1f0f0f0 f0f0f0f0 f93f0000 00000000 .........?......
+  0x0000d6c0 f1f0f0f0 f0f0f0f0 fa3f0000 00000000 .........?......
+  0x0000d6d0 f1f0f0f0 f0f0f0f0 fd3f0000 00000000 .........?......
+  0x0000d6e0 f1f0f0f0 f0f0f0f0 fe3f0000 00000000 .........?......
+  0x0000d6f0 0b9dc10a 9dc10a9d fe3f0000 00000000 .........?......
+  0x0000d700 d3d2d2d2 d2d2d2d2 fc3f0000 00000000 .........?......
+  0x0000d710 8b21d31f e7f300ba ed3f0000 00000000 .!.......?......
+  0x0000d720 4d24da02 cbcdf09c f33f0000 00000000 M$.......?......
+  0x0000d730 7e8add75 cd6603b0 f73f0000 00000000 ~..u.f...?......
+  0x0000d740 366f4f3a c4069597 fa3f0000 00000000 6oO:.....?......
+  0x0000d750 7b90f822 5ed67aa3 fb3f0000 00000000 {.."^.z..?......
+  0x0000d760 0e6bdfb0 f60d6bdf f53f0000 00000000 .k....k..?......
+  0x0000d770 e9a28b2e bae8a28b f83f0000 00000000 .........?......
+  0x0000d780 09f29420 4f09f294 f83f0000 00000000 ... O....?......
+  0x0000d790 2fbae8a2 8b2ebae8 fb3f0000 00000000 /........?......
+  0x0000d7a0 95204f09 f294208f fc3f0000 00000000 . O... ..?......
+  0x0000d7b0 54823c25 c853829c fd3f0000 00000000 T.<%.S...?......
+  0x0000d7c0 bf61ed1b d6be618d ff3f0000 00000000 .a....a..?......
+  0x0000d7d0 2fbae8a2 8b2eba90 fe3f0000 00000000 /........?......
+  0x0000d7e0 4a90a704 794a90e7 fb3f0000 00000000 J...yJ...?......
+  0x0000d7f0 1911b1ff f2191e81 ec3f0000 00000000 .........?......
+  0x0000d800 dacc7a0f cacbe2d9 f13f0000 00000000 ..z......?......
+  0x0000d810 dc9cea64 1c785df4 f53f0000 00000000 ...d.x]..?......
+  0x0000d820 1e593f4f cb4f72d2 f83f0000 00000000 .Y?O.Or..?......
+  0x0000d830 0e407525 9de9f6e2 f93f0000 00000000 .@u%.....?......
+  0x0000d840 08822008 82200882 f83f0000 00000000 .. .. ...?......
+  0x0000d850 49922449 92244992 fb3f0000 00000000 I.$I.$I..?......
+  0x0000d860 f745c463 3e6830c3 ee3f0000 00000000 .E.c>h0..?......
+  0x0000d870 099b2da4 f4d7b0a4 f43f0000 00000000 ..-......?......
+  0x0000d880 357be809 a58eb4b8 f83f0000 00000000 5{.......?......
+  0x0000d890 85d30dd8 f352119f fb3f0000 00000000 .....R...?......
+  0x0000d8a0 7e81afd5 9e8b8dab fc3f0000 00000000 ~........?......
+  0x0000d8b0 0b39bd5c b321a6ef f6bf0000 00000000 .9.\.!..........
+  0x0000d8c0 0b39bd5c b321a6ef f73f0000 00000000 .9.\.!...?......
+  0x0000d8d0 b27b0b8c 8a8e2ed9 fb3f0000 00000000 .{.......?......
+  0x0000d8e0 7a65f126 98bfabe0 fc3f0000 00000000 ze.&.....?......
+  0x0000d8f0 a2a643f6 1910d5c7 fd3f0000 00000000 ..C......?......
+  0x0000d900 9b5072ac 458311b2 f13f0000 00000000 .Pr.E....?......
+  0x0000d910 8706e4f6 dc52cf9b f73f0000 00000000 .....R...?......
+  0x0000d920 b6850758 81685588 fb3f0000 00000000 ...X.hU..?......
+  0x0000d930 ae9a0062 aeb353c8 fc3f0000 00000000 ...b..S..?......
+  0x0000d940 8fb823ee 883be28e f93f0000 00000000 ..#..;...?......
+  0x0000d950 8fb823ee 883be28e fb3f0000 00000000 ..#..;...?......
+  0x0000d960 9535654d 5953d694 fc3f0000 00000000 .5eMYS...?......
+  0x0000d970 ee883be2 8eb823ee fe3f0000 00000000 ..;...#..?......
+  0x0000d980 1e7147dc 1177c4bd ff3f0000 00000000 .qG..w...?......
+  0x0000d990 410a8482 3c6e08c1 f23f0000 00000000 A...<n...?......
+  0x0000d9a0 f98833f2 7460e7a8 f83f0000 00000000 ..3.t`...?......
+  0x0000d9b0 da17ed53 6674ca93 fc3f0000 00000000 ...Sft...?......
+  0x0000d9c0 898bd412 047c29d9 fd3f0000 00000000 .....|)..?......
+  0x0000d9d0 cdcccccc cccccccc fabf0000 00000000 ................
+  0x0000d9e0 9a999999 99999999 fd3f0000 00000000 .........?......
+  0x0000d9f0 cdcccccc cccccccc fa3f0000 00000000 .........?......
+  0x0000da00 0e005009 870579df f43f0000 00000000 ..P...y..?......
+  0x0000da10 0c002628 d6e489c3 fa3f0000 00000000 ..&(.....?......
+  0x0000da20 0b402163 3ba818ab fe3f0000 00000000 .@!c;....?......
+  0x0000da30 10007aea 372668fb ff3f0000 00000000 ..z.7&h..?......
+  0x0000da40 aa91ae9d 423b9c84 f63f0000 00000000 ....B;...?......
+  0x0000da50 f26598d7 0977c5c2 fb3f0000 00000000 .e...w...?......
+  0x0000da60 69657cfb a0d355c9 ff3f0000 00000000 ie|...U..?......
+  0x0000da70 c592d785 85e6b3dd f33f0000 00000000 .........?......
+  0x0000da80 6ca01cd5 b469fdc1 f93f0000 00000000 l....i...?......
+  0x0000da90 5f0c793a 7ebcbda9 fd3f0000 00000000 _.y:~....?......
+  0x0000daa0 1d859236 56636af9 fe3f0000 00000000 ...6Vcj..?......
+  0x0000dab0 45b6242c 342e448a f2bf0000 00000000 E.$,4.D.........
+  0x0000dac0 d6e32d37 c139d5ac f43f0000 00000000 ..-7.9...?......
+  0x0000dad0 cc5cf984 31880ad8 f63f0000 00000000 .\..1....?......
+  0x0000dae0 f552e740 8fe33bb2 f93f0000 00000000 .R.@..;..?......
+  0x0000daf0 ee1f44d5 629328a0 f63f0000 00000000 ..D.b.(..?......
+  0x0000db00 6ba7fad3 99c94ec6 fc3f0000 00000000 k.....N..?......
+  0x0000db10 8a38c08b fb3825aa fd3f0000 00000000 .8...8%..?......
+  0x0000db20 6b01799e 0e0b9494 fc3f0000 00000000 k.y......?......
+  0x0000db30 74379a4f 6f0d8b98 ff3f0000 00000000 t7.Oo....?......
+  0x0000db40 51c58023 cbd0ad9e fe3f0000 00000000 Q..#.....?......
+  0x0000db50 b53b016c abe7e2fd fb3f0000 00000000 .;.l.....?......
+  0x0000db60 9ea69ae7 f879f89a e73f0000 00000000 .....y...?......
+  0x0000db70 4e7ab105 866bedd9 ed3f0000 00000000 Nz...k...?......
+  0x0000db80 3dd86c28 7dac6cdc f23f0000 00000000 =.l(}.l..?......
+  0x0000db90 32f53ee0 32058dc4 f63f0000 00000000 2.>.2....?......
+  0x0000dba0 d123ef82 665c9796 f93f0000 00000000 .#..f\...?......
+  0x0000dbb0 ffc9003c 9aef3a99 fa3f0000 00000000 ...<..:..?......
+  0x0000dbc0 efbcb6da 44e6f7f3 f33f0000 00000000 ....D....?......
+  0x0000dbd0 51e55f3f 7ce978d5 f63f0000 00000000 Q._?|.x..?......
+  0x0000dbe0 a6e35503 1478d0e2 fa3f0000 00000000 ..U..x...?......
+  0x0000dbf0 16841893 72af1cac fc3f0000 00000000 ....r....?......
+  0x0000dc00 0622ccc8 b43c6c89 fc3f0000 00000000 ."...<l..?......
+  0x0000dc10 c5a0c49b a6e76d93 fd3f0000 00000000 ......m..?......
+  0x0000dc20 7fae84f7 8385fca1 fe3f0000 00000000 .........?......
+  0x0000dc30 5e3128f1 a6e979db fc3f0000 00000000 ^1(...y..?......
+  0x0000dc40 d91377ca be78d4fa f93f0000 00000000 ..w..x...?......
+  0x0000dc50 f39b7d79 e112d4ca e93f0000 00000000 ..}y.....?......
+  0x0000dc60 a7516c89 461d9d8e f03f0000 00000000 .Ql.F....?......
+  0x0000dc70 b9e4767a ad723f90 f53f0000 00000000 ..vz.r?..?......
+  0x0000dc80 de3f632c d9ec9f80 f93f0000 00000000 .?c,.....?......
+  0x0000dc90 3fb352e2 a8bc18c5 fb3f0000 00000000 ?.R......?......
+  0x0000dca0 d3524031 2bf18cc8 fc3f0000 00000000 .R@1+....?......
+  0x0000dcb0 167dea6b 866d01a2 f03f0000 00000000 .}.k.m...?......
+  0x0000dcc0 a1bbdfa1 492402f3 f13f0000 00000000 ....I$...?......
+  0x0000dcd0 1d85ebf6 3f1192ea f53f0000 00000000 ....?....?......
+  0x0000dce0 a74bef5f c8a30dba f73f0000 00000000 .K._.....?......
+  0x0000dcf0 cdb000a7 0bd0abcd f93f0000 00000000 .........?......
+  0x0000dd00 b4b4614f 792279b9 fb3f0000 00000000 ..aOy"y..?......
+  0x0000dd10 8da858a3 0befada2 fb3f0000 00000000 ..X......?......
+  0x0000dd20 e4ba9bfb 229042f8 fd3f0000 00000000 ....".B..?......
+  0x0000dd30 926f2832 27d2bfba fc3f0000 00000000 .o(2'....?......
+  0x0000dd40 972f609f b53cfed3 fe3f0000 00000000 ./`..<...?......
+  0x0000dd50 a8c1f53a 47d0c7ed e63f0000 00000000 ...:G....?......
+  0x0000dd60 2acc7415 727e30a7 ed3f0000 00000000 *.t.r~0..?......
+  0x0000dd70 0a675ea8 8fea1aa9 f23f0000 00000000 .g^......?......
+  0x0000dd80 07c9cbab 7c2eca96 f63f0000 00000000 ....|....?......
+  0x0000dd90 c337a777 c09e0fe7 f83f0000 00000000 .7.w.....?......
+  0x0000dda0 1c3f2c6e d0311ceb f93f0000 00000000 .?,n.1...?......
+  0x0000ddb0 fc4950e1 e89639d7 f4bf0000 00000000 .IP...9.........
+  0x0000ddc0 3b537afd c5c920f2 f73f0000 00000000 ;Sz... ..?......
+  0x0000ddd0 0266b874 b5dba0ac f93f0000 00000000 .f.t.....?......
+  0x0000dde0 182783c8 0357d1ce fc3f0000 00000000 .'...W...?......
+  0x0000ddf0 9cad43bf d93af49b fe3f0000 00000000 ..C..:...?......
+  0x0000de00 bce14775 89590b85 ff3f0000 00000000 ..Gu.Y...?......
+  0x0000de10 101a02db 578f8bb4 fe3f0000 00000000 ....W....?......
+  0x0000de20 9cad43bf d93af49b fd3f0000 00000000 ..C..:...?......
+  0x0000de30 c155b433 a5d75f9c fb3f0000 00000000 .U.3.._..?......
+  0x0000de40 73da8311 21dcff8a f83f0000 00000000 s...!....?......
+  0x0000de50 c8a56542 6d7193ee e83f0000 00000000 ..eBmq...?......
+  0x0000de60 9178afd2 c0abbfa7 ef3f0000 00000000 .x.......?......
+  0x0000de70 366a08c4 dabbaba9 f43f0000 00000000 6j.......?......
+  0x0000de80 d9259321 76504b97 f83f0000 00000000 .%.!vPK..?......
+  0x0000de90 6d4ef9af c47ed5e7 fa3f0000 00000000 mN...~...?......
+  0x0000dea0 8bc14628 8789e5eb fb3f0000 00000000 ..F(.....?......
+  0x0000deb0 0037159f 0712f7e8 f23f0000 00000000 .7.......?......
+  0x0000dec0 209032ab c62fd8cb f53f0000 00000000  .2../...?......
+  0x0000ded0 22b9e515 c3b295d8 f93f0000 00000000 "........?......
+  0x0000dee0 952e5960 5adfc585 fb3f0000 00000000 ..Y`Z....?......
+  0x0000def0 1a15196b d1a69fa5 fa3f0000 00000000 ...k.....?......
+  0x0000df00 4447ef0d 1fe6eae6 fd3f0000 00000000 DG.......?......
+  0x0000df10 f198c30d 56fb89ee fe3f0000 00000000 ....V....?......
+  0x0000df20 252aef87 82a59a9d fe3f0000 00000000 %*.......?......
+  0x0000df30 c189e26d a4a1ced3 fc3f0000 00000000 ...m.....?......
+  0x0000df40 260b4ceb bbb810f2 f93f0000 00000000 &.L......?......
+  0x0000df50 c5a30afc 6ec11db7 e63f0000 00000000 ....n....?......
+  0x0000df60 277b3709 02ecc080 ed3f0000 00000000 '{7......?......
+  0x0000df70 18511ffe 60993a82 f23f0000 00000000 .Q..`.:..?......
+  0x0000df80 96be4a73 458d3fe8 f53f0000 00000000 ..JsE.?..?......
+  0x0000df90 cc46239d 2b06f1b1 f83f0000 00000000 .F#.+....?......
+  0x0000dfa0 2e05f6dc e24b0fb5 f93f0000 00000000 .....K...?......
+  0x0000dfb0 09486937 0252da8d f63f0000 00000000 .Hi7.R...?......
+  0x0000dfc0 0cc3300c c3300cc3 f93f0000 00000000 ..0..0...?......
+  0x0000dfd0 cff33ccf f33ccff3 fb3f0000 00000000 ..<..<...?......
+  0x0000dfe0 dbb66ddb b66ddbb6 fd3f0000 00000000 ..m..m...?......
+  0x0000dff0 dbb66ddb b66ddbb6 fe3f0000 00000000 ..m..m...?......
+  0x0000e000 d5087ad3 762f6cd6 ea3f0000 00000000 ..z.v/l..?......
+  0x0000e010 36ceb18c 5f11c496 f13f0000 00000000 6..._....?......
+  0x0000e020 e8f9c571 81507e98 f63f0000 00000000 ...q.P~..?......
+  0x0000e030 8aebab82 392bfa87 fa3f0000 00000000 ....9+...?......
+  0x0000e040 fd21d873 cff85cd0 fc3f0000 00000000 .!.s..\..?......
+  0x0000e050 fc09da5d 6eb803d4 fd3f0000 00000000 ...]n....?......
+  0x0000e060 5446c630 bf895bdd ebbf0000 00000000 TF.0..[.........
+  0x0000e070 bfb49464 4fa704a6 ed3f0000 00000000 ...dO....?......
+  0x0000e080 0e053f7b 3ea4ce8d f23f0000 00000000 ..?{>....?......
+  0x0000e090 c7b964b2 abd2a0db f33f0000 00000000 ..d......?......
+  0x0000e0a0 ccd733ac 51582ef6 f63f0000 00000000 ..3.QX...?......
+  0x0000e0b0 3057f35f 6c9b02cb f83f0000 00000000 0W._l....?......
+  0x0000e0c0 cf560278 d0d0339f fa3f0000 00000000 .V.x..3..?......
+  0x0000e0d0 15924e65 5fa09e99 fc3f0000 00000000 ..Ne_....?......
+  0x0000e0e0 703241c2 20460dc5 fb3f0000 00000000 p2A. F...?......
+  0x0000e0f0 0d3b53cd 86b528b3 fe3f0000 00000000 .;S...(..?......
+  0x0000e100 787d1a91 31aff7d5 fd3f0000 00000000 x}..1....?......
+  0x0000e110 a5ce09f6 05f1e4bf fe3f0000 00000000 .........?......
+  0x0000e120 5a30365b 1d2fe984 e23f0000 00000000 Z06[./...?......
+  0x0000e130 82d80ce1 29395590 e93f0000 00000000 ....)9U..?......
+  0x0000e140 927102cc 6ba59fed ee3f0000 00000000 .q..k....?......
+  0x0000e150 0f9b72aa c7f1e1ba f33f0000 00000000 ..r......?......
+  0x0000e160 8bbf407f fa1e3591 f73f0000 00000000 ..@...5..?......
+  0x0000e170 6a30c586 8f6afbcd f93f0000 00000000 j0...j...?......
+  0x0000e180 7b6e6e89 96f13bc9 fa3f0000 00000000 {nn...;..?......
+  0x0000e190 d34faac2 a6fde2a9 ee3f0000 00000000 .O.......?......
+  0x0000e1a0 c8e35473 10bd5bd4 f03f0000 00000000 ..Ts..[..?......
+  0x0000e1b0 ae3fa32d f895e192 f43f0000 00000000 .?.-.....?......
+  0x0000e1c0 13ac7647 187325d2 f63f0000 00000000 ..vG.s%..?......
+  0x0000e1d0 57bfec45 9cb3f3ed f73f0000 00000000 W..E.....?......
+  0x0000e1e0 dc508ccb 22d20e80 fb3f0000 00000000 .P.."....?......
+  0x0000e1f0 6b293a15 e1b95287 fa3f0000 00000000 k):...R..?......
+  0x0000e200 44a1f9ed 653f77be fd3f0000 00000000 D...e?w..?......
+  0x0000e210 e02e13cb 436b93cc fe3f0000 00000000 ....Ck...?......
+  0x0000e220 6b86ce55 2e064d80 fd3f0000 00000000 k..U..M..?......
+  0x0000e230 8a404651 2f1c2fb4 ff3f0000 00000000 .@FQ/./..?......
+  0x0000e240 add09725 3be33ac1 fe3f0000 00000000 ...%;.:..?......
+  0x0000e250 f1a6acb7 9582959a fc3f0000 00000000 .........?......
+  0x0000e260 a60b732f f181b4db e33f0000 00000000 ..s/.....?......
+  0x0000e270 a7ee86e9 1b0596ee ea3f0000 00000000 .........?......
+  0x0000e280 727fc271 082466c4 f03f0000 00000000 r..q.$f..?......
+  0x0000e290 5c1332aa 0ffc759a f53f0000 00000000 \.2...u..?......
+  0x0000e2a0 341d12cf ef2008f0 f83f0000 00000000 4.... ...?......
+  0x0000e2b0 aba9520b 38323faa fb3f0000 00000000 ..R.82?..?......
+  0x0000e2c0 2f23f0a1 a89752a6 fc3f0000 00000000 /#....R..?......
+  0x0000e2d0 3f4d432a fb2115a9 e63f0000 00000000 ?MC*.!...?......
+  0x0000e2e0 e315e5bf e6f29cb7 ed3f0000 00000000 .........?......
+  0x0000e2f0 96998f5d 187c2597 f33f0000 00000000 ...].|%..?......
+  0x0000e300 9b3ea62c 561fbeed f73f0000 00000000 .>.,V....?......
+  0x0000e310 c307403e c0c7b9b8 fb3f0000 00000000 ..@>.....?......
+  0x0000e320 5d6f0431 b1210583 fe3f0000 00000000 ]o.1.!...?......
+  0x0000e330 45511445 51144591 f0bf0000 00000000 EQ.EQ.E.........
+  0x0000e340 398ee338 8ee338fe f23f0000 00000000 9..8..8..?......
+  0x0000e350 10044110 044110ec f43f0000 00000000 ..A..A...?......
+  0x0000e360 55555555 5555d5a6 f83f0000 00000000 UUUUUU...?......
+  0x0000e370 44444444 4444e481 f93f0000 00000000 DDDDDD...?......
+  0x0000e380 89888888 88883082 fb3f0000 00000000 ......0..?......
+  0x0000e390 363b6a11 f2d7348d fd3f0000 00000000 6;j...4..?......
+  0x0000e3a0 89888888 8888c0c0 fd3f0000 00000000 .........?......
+  0x0000e3b0 caa55cca a55caab6 f93f0000 00000000 ..\..\...?......
+  0x0000e3c0 32266332 2663a195 fe3f0000 00000000 2&c2&c...?......
+  0x0000e3d0 85544885 54488fd2 fe3f0000 00000000 .TH.TH...?......
+  0x0000e3e0 66599665 59965b8c fe3f0000 00000000 fY.eY.[..?......
+  0x0000e3f0 50077550 0775fcc0 fc3f0000 00000000 P.uP.u...?......
+  0x0000e400 5c0818a5 9a3c8edc f93f0000 00000000 \....<...?......
+  0x0000e410 a33773f4 5c0f9796 ea3f0000 00000000 .7s.\....?......
+  0x0000e420 26d4def4 71316af9 f03f0000 00000000 &...q1j..?......
+  0x0000e430 af8aab1b e669d196 f63f0000 00000000 .....i...?......
+  0x0000e440 fe2a80d4 a0202da3 fa3f0000 00000000 .*... -..?......
+  0x0000e450 5832835c 9685199f fd3f0000 00000000 X2.\.....?......
+  0x0000e460 ae0de157 e6d638ee fe3f0000 00000000 ...W..8..?......
+  0x0000e470 7d4cedc3 483b3195 e33f0000 00000000 }L..H;1..?......
+  0x0000e480 10b1c304 617603a2 ea3f0000 00000000 ....av...?......
+  0x0000e490 58a8e4d3 56ba5d85 f03f0000 00000000 X...V.]..?......
+  0x0000e4a0 67e6c029 a887c6d1 f43f0000 00000000 g..).....?......
+  0x0000e4b0 8fbe1723 90c9fea2 f83f0000 00000000 ...#.....?......
+  0x0000e4c0 ee947db6 e4f436e7 fa3f0000 00000000 ..}...6..?......
+  0x0000e4d0 74d3ac6e 0b97e2e1 fb3f0000 00000000 t..n.....?......
+  0x0000e4e0 b745f6fc 232919c7 eebf0000 00000000 .E..#)..........
+  0x0000e4f0 007d577d ff0336ae f13f0000 00000000 .}W}..6..?......
+  0x0000e500 a518883d 6d71c4a1 f33f0000 00000000 ...=mq...?......
+  0x0000e510 11d48254 3fe5a6e4 f63f0000 00000000 ...T?....?......
+  0x0000e520 9d2b9e10 cd02a7dd f63f0000 00000000 .+.......?......
+  0x0000e530 b4d4fd90 65e40294 fa3f0000 00000000 ....e....?......
+  0x0000e540 64f4da4c 7b0fdcee fb3f0000 00000000 d..L{....?......
+  0x0000e550 51e49beb ab553cde fa3f0000 00000000 Q....U<..?......
+  0x0000e560 dcc7b735 db4a60b8 fd3f0000 00000000 ...5.J`..?......
+  0x0000e570 0c42e2e2 d721c6e3 fe3f0000 00000000 .B...!...?......
+  0x0000e580 b2aba635 fa9415a0 fe3f0000 00000000 ...5.....?......
+  0x0000e590 78ace3dd b5c425d8 fc3f0000 00000000 x.....%..?......
+  0x0000e5a0 400ebb46 ab9706f7 f93f0000 00000000 @..F.....?......
+  0x0000e5b0 93e4795d 0261c3f0 e03f0000 00000000 ..y].a...?......
+  0x0000e5c0 1c2fc148 ac15ba82 e83f0000 00000000 ./.H.....?......
+  0x0000e5d0 6c6e3ff5 3f2739d7 ed3f0000 00000000 ln?.?'9..?......
+  0x0000e5e0 3a1bec3b d2f743a9 f23f0000 00000000 :..;..C..?......
+  0x0000e5f0 e72a5fde 3ce08483 f63f0000 00000000 .*_.<....?......
+  0x0000e600 dd1c3d0a 958490ba f83f0000 00000000 ..=......?......
+  0x0000e610 3291dcc6 35a043b6 f93f0000 00000000 2...5.C..?......
+  0x0000e620 ccbfcc43 e5a67e8e f13f0000 00000000 ...C..~..?......
+  0x0000e630 c65746ec c17b4ea0 f43f0000 00000000 .WF..{N..?......
+  0x0000e640 b21fb3e5 57fabdd5 f33f0000 00000000 ....W....?......
+  0x0000e650 b5868526 850a10cf f83f0000 00000000 ...&.....?......
+  0x0000e660 afa81fd3 221974e3 fa3f0000 00000000 ....".t..?......
+  0x0000e670 4f5f1460 ea97e4a1 fb3f0000 00000000 O_.`.....?......
+  0x0000e680 1b3800fb aee2a8aa fb3f0000 00000000 .8.......?......
+  0x0000e690 f4dd189c de09a986 fe3f0000 00000000 .........?......
+  0x0000e6a0 4305cd49 d651748c ff3f0000 00000000 C..I.Qt..?......
+  0x0000e6b0 0a62a935 859f16c3 fe3f0000 00000000 .b.5.....?......
+  0x0000e6c0 30af0eb1 cb5333aa fd3f0000 00000000 0....S3..?......
+  0x0000e6d0 18cfed9e 44813eab fb3f0000 00000000 ....D.>..?......
+  0x0000e6e0 c062d370 598f3798 f83f0000 00000000 .b.pY.7..?......
+  0x0000e6f0 fdf5c620 0cab6c93 e43f0000 00000000 ... ..l..?......
+  0x0000e700 200f982b bf0118a0 eb3f0000 00000000  ..+.....?......
+  0x0000e710 f5da6c1f 072cc983 f13f0000 00000000 ..l..,...?......
+  0x0000e720 fb500c5f 27314acf f53f0000 00000000 .P._'1J..?......
+  0x0000e730 4a46c64f 8e5a10a1 f93f0000 00000000 JF.O.Z...?......
+  0x0000e740 469c154b ab9579e4 fb3f0000 00000000 F..K..y..?......
+  0x0000e750 c65ccc8f 856235df fc3f0000 00000000 .\...b5..?......
+  0x0000e760 ed22df46 54fd2c81 ed3f0000 00000000 .".FT.,..?......
+  0x0000e770 a8eb9658 a93c78a1 ef3f0000 00000000 ...X.<x..?......
+  0x0000e780 ba818cba 61cb5ddf f23f0000 00000000 ....a.]..?......
+  0x0000e790 89aeaa3f b2a6c99f f53f0000 00000000 ...?.....?......
+  0x0000e7a0 567d919a 686be2c5 f63f0000 00000000 V}..hk...?......
+  0x0000e7b0 94526827 f17356cd f93f0000 00000000 .Rh'.sV..?......
+  0x0000e7c0 cd1b8bca 29b562a1 f83f0000 00000000 ....).b..?......
+  0x0000e7d0 432bc2eb 77ce4ba9 fc3f0000 00000000 C+..w.K..?......
+  0x0000e7e0 cf69e890 9dc3eb94 fd3f0000 00000000 .i.......?......
+  0x0000e7f0 4492e194 f89e5fb3 fc3f0000 00000000 D....._..?......
+  0x0000e800 e8718fa2 b4368d96 ff3f0000 00000000 .q...6...?......
+  0x0000e810 614e33cb 6184309c fe3f0000 00000000 aN3.a.0..?......
+  0x0000e820 9cb0eb11 363ae7f9 fb3f0000 00000000 ....6:...?......
+  0x0000e830 ef8220d2 4299f19d e03f0000 00000000 .. .B....?......
+  0x0000e840 304e2f90 6e5c84ab e73f0000 00000000 0N/.n\...?......
+  0x0000e850 0b4086d3 5870308d ed3f0000 00000000 .@..Xp0..?......
+  0x0000e860 aa47fd94 2ba714de f13f0000 00000000 .G..+....?......
+  0x0000e870 74c7fffd ab6d8eac f53f0000 00000000 t....m...?......
+  0x0000e880 ef98ca4f 2106c7f4 f73f0000 00000000 ...O!....?......
+  0x0000e890 5ebb969c 14a022ef f83f0000 00000000 ^....."..?......
+  0x0000e8a0 637f0bce 4bc864a2 f2bf0000 00000000 c...K.d.........
+  0x0000e8b0 28cf4f3b 68934adf f53f0000 00000000 (.O;h.J..?......
+  0x0000e8c0 3847d955 e01360ce f73f0000 00000000 8G.U..`..?......
+  0x0000e8d0 70dfdf7c 4562dc94 f53f0000 00000000 p..|Eb...?......
+  0x0000e8e0 33a0f2db f7375f91 fb3f0000 00000000 3....7_..?......
+  0x0000e8f0 feee1470 9d65e596 fd3f0000 00000000 ...p.e...?......
+  0x0000e900 fc7af2fc b48336a9 fe3f0000 00000000 .z....6..?......
+  0x0000e910 6e294372 ae5075f9 fe3f0000 00000000 n)Cr.Pu..?......
+  0x0000e920 74bf3b05 5c6759b9 fe3f0000 00000000 t.;.\gY..?......
+  0x0000e930 2bb79421 3957a8ba fd3f0000 00000000 +..!9W...?......
+  0x0000e940 8e03d991 acfab8f9 fb3f0000 00000000 .........?......
+  0x0000e950 3ed4cc5f 0d2408c8 f93f0000 00000000 >.._.$...?......
+  0x0000e960 73f794e8 c3487a91 f63f0000 00000000 s....Hz..?......
+  0x0000e970 5118048d eff0bc98 e43f0000 00000000 Q........?......
+  0x0000e980 68722223 a42ddda5 eb3f0000 00000000 hr"#.-...?......
+  0x0000e990 1da1b6a3 00268988 f13f0000 00000000 .....&...?......
+  0x0000e9a0 83ec8a0b 54d6c2d6 f53f0000 00000000 ....T....?......
+  0x0000e9b0 8ebfac02 ed79dea6 f93f0000 00000000 .....y...?......
+  0x0000e9c0 48f00afe 04b4b5ec fb3f0000 00000000 H........?......
+  0x0000e9d0 35785821 26e940e7 fc3f0000 00000000 5xX!&.@..?......
+  0x0000e9e0 43642718 b472ac95 f03f0000 00000000 Cd'..r...?......
+  0x0000e9f0 cb502c9b 0a0162a8 f33f0000 00000000 .P,...b..?......
+  0x0000ea00 64163b24 0eac82e0 f23f0000 00000000 d.;$.....?......
+  0x0000ea10 b13d19b3 ad967ed9 f73f0000 00000000 .=....~..?......
+  0x0000ea20 dcc09253 6fdd0ad0 f93f0000 00000000 ...So....?......
+  0x0000ea30 d78c31b0 dff610f9 f73f0000 00000000 ..1......?......
+  0x0000ea40 d35aa692 cdefbab7 fc3f0000 00000000 .Z.......?......
+  0x0000ea50 9870bdb9 0ca9c197 fe3f0000 00000000 .p.......?......
+  0x0000ea60 b238ce3e 43798a86 ff3f0000 00000000 .8.>Cy...?......
+  0x0000ea70 d28a7cf9 be217eb7 fe3f0000 00000000 ..|..!~..?......
+  0x0000ea80 384e6281 fb73d89e fd3f0000 00000000 8Nb..s...?......
+  0x0000ea90 26f3380a a7c5649f fb3f0000 00000000 &.8...d..?......
+  0x0000eaa0 e849dd7a 94e8ae8d f83f0000 00000000 .I.z.....?......
+  0x0000eab0 bdd0a245 beaf2aaa e13f0000 00000000 ...E..*..?......
+  0x0000eac0 aece9e9f d85acab8 e83f0000 00000000 .....Z...?......
+  0x0000ead0 49c38fbe 89981d98 ee3f0000 00000000 I........?......
+  0x0000eae0 bad4e0ac 386244ef f23f0000 00000000 ....8bD..?......
+  0x0000eaf0 349de52c 4103e9b9 f63f0000 00000000 4..,A....?......
+  0x0000eb00 38a9730c 6734dc83 f93f0000 00000000 8.s.g4...?......
+  0x0000eb10 ee5ffed5 971dd280 fa3f0000 00000000 ._.......?......
+  0x0000eb20 250b20dc 78fb92de f33f0000 00000000 %. .x....?......
+  0x0000eb30 0e09da32 526cd7b4 f73f0000 00000000 ...2Rl...?......
+  0x0000eb40 cb8623a6 3d91a187 fa3f0000 00000000 ..#.=....?......
+  0x0000eb50 74cceb05 f134a8f8 fb3f0000 00000000 t....4...?......
+  0x0000eb60 c85fb3a3 1621699b fd3f0000 00000000 ._...!i..?......
+  0x0000eb70 01a35493 c79dde8b fe3f0000 00000000 ..T......?......
+  0x0000eb80 57d970c4 b4277eba fe3f0000 00000000 W.p..'~..?......
+  0x0000eb90 66028b6d 6ce0f3c2 f2bf0000 00000000 f..ml...........
+  0x0000eba0 66028b6d 6ce0f3c2 f33f0000 00000000 f..ml....?......
+  0x0000ebb0 da1215c2 809a81e7 f83f0000 00000000 .........?......
+  0x0000ebc0 e33ecb73 026a8dea f93f0000 00000000 .>.s.j...?......
+  0x0000ebd0 5b3d4788 e0a36982 fd3f0000 00000000 [=G...i..?......
+  0x0000ebe0 5297e59b 300fbe89 fe3f0000 00000000 R...0....?......
+  0x0000ebf0 57340db2 67f820bb fe3f0000 00000000 W4..g. ..?......
+  0x0000ec00 f9201d94 0abc778c ec3f0000 00000000 . ....w..?......
+  0x0000ec10 e94edbea 4940b083 f33f0000 00000000 .N..I@...?......
+  0x0000ec20 2a10f347 87afcb95 f83f0000 00000000 *..G.....?......
+  0x0000ec30 cfa636f1 28c3f7e0 fb3f0000 00000000 ..6.(....?......
+  0x0000ec40 18c5a0e6 8bb3069e fd3f0000 00000000 .........?......
+  0x0000ec50 01fe8433 ff017bcc f33f0000 00000000 ...3..{..?......
+  0x0000ec60 01fe8433 ff017bcc f53f0000 00000000 ...3..{..?......
+  0x0000ec70 a16e6b73 5f91948c f93f0000 00000000 .nks_....?......
+  0x0000ec80 79d27163 872d8e9c fb3f0000 00000000 y.qc.-...?......
+  0x0000ec90 895457d0 215653da fa3f0000 00000000 .TW.!VS..?......
+  0x0000eca0 aa02a410 01a8069a fe3f0000 00000000 .........?......
+  0x0000ecb0 78ffabfc 32abfead fe3f0000 00000000 x...2....?......
+  0x0000ecc0 78ffabfc 32abfead fc3f0000 00000000 x...2....?......
+  0x0000ecd0 2cfd3b37 3d4a1c97 eb3f0000 00000000 ,.;7=J...?......
+  0x0000ece0 593dc863 9985aa8d f23f0000 00000000 Y=.c.....?......
+  0x0000ecf0 fcf8e647 2b2b25a1 f73f0000 00000000 ...G++%..?......
+  0x0000ed00 7813760a e64e03f2 fa3f0000 00000000 x.v..N...?......
+  0x0000ed10 d17c23de 84d3ffa9 fc3f0000 00000000 .|#......?......
+  0x0000ed20 0bb4400b b4400bb4 f6bf0000 00000000 ..@..@..........
+  0x0000ed30 08877008 87700887 f93f0000 00000000 ..p..p...?......
+  0x0000ed40 0dd2200d d2200dd2 f93f0000 00000000 .. .. ...?......
+  0x0000ed50 3bb1133b b1133bb1 fd3f0000 00000000 ;..;..;..?......
+  0x0000ed60 27766227 766227f6 fe3f0000 00000000 'vb'vb'..?......
+  0x0000ed70 07699006 699006a9 ff3f0000 00000000 .i..i....?......
+  0x0000ed80 5dcdd55c cdd55ccd fd3f0000 00000000 ]..\..\..?......
+  0x0000ed90 e9888ee8 888ee888 fb3f0000 00000000 .........?......
+  0x0000eda0 a3744917 a3d345ba ed3f0000 00000000 .tI...E..?......
+  0x0000edb0 59ddd4e5 6876a1ae f43f0000 00000000 Y...hv...?......
+  0x0000edc0 6255d5eb b076a4c6 f93f0000 00000000 bU...v...?......
+  0x0000edd0 66d2a599 79ea2995 fd3f0000 00000000 f...y.)..?......
+  0x0000ede0 37a3327a 178e8ed1 fe3f0000 00000000 7.2z.....?......
+  0x0000edf0 8ee3388e e3388ee3 ed3f0000 00000000 ..8..8...?......
+  0x0000ee00 55555555 555555d5 f43f0000 00000000 UUUUUUU..?......
+  0x0000ee10 abaaaaaa aaaaaaf2 f93f0000 00000000 .........?......
+  0x0000ee20 398ee338 8ee338b6 fd3f0000 00000000 9..8..8..?......
+  0x0000ee30 2fc057f8 b1508ac9 ef3f0000 00000000 /.W..P...?......
+  0x0000ee40 d2e0b2c9 67d2d9a5 f63f0000 00000000 ....g....?......
+  0x0000ee50 5e0667c4 a09b8a9c fb3f0000 00000000 ^.g......?......
+  0x0000ee60 833efb55 5de427ae fe3f0000 00000000 .>.U].'..?......
+  0x0000ee70 d509d5ab 5ef21c85 ed3f0000 00000000 ....^....?......
+  0x0000ee80 6f722f82 714696f9 f33f0000 00000000 or/.qF...?......
+  0x0000ee90 7c2f3ef5 76def38d f93f0000 00000000 |/>.v....?......
+  0x0000eea0 bf31339f 2b5c30d5 fc3f0000 00000000 .13.+\0..?......
+  0x0000eeb0 0fab4f81 aa90c095 fe3f0000 00000000 ..O......?......
+  0x0000eec0 8f56ad95 a6b9a199 e2bf0000 00000000 .V..............
+  0x0000eed0 33ac183b 10280ac0 e43f0000 00000000 3..;.(...?......
+  0x0000eee0 a22f9e69 0627d6b0 e93f0000 00000000 ./.i.'...?......
+  0x0000eef0 4d46b707 49530ce9 eb3f0000 00000000 MF..IS...?......
+  0x0000ef00 af25f15c 4fa9a494 ef3f0000 00000000 .%.\O....?......
+  0x0000ef10 bbd3058e cd9432d7 f13f0000 00000000 ......2..?......
+  0x0000ef20 04aafc72 3bbeb1d2 f33f0000 00000000 ...r;....?......
+  0x0000ef30 e15f8b5b 28e7c5ba f63f0000 00000000 ._.[(....?......
+  0x0000ef40 ed0d1b8b cb18d8a7 f63f0000 00000000 .........?......
+  0x0000ef50 9262bc57 7debb196 fa3f0000 00000000 .b.W}....?......
+  0x0000ef60 52af4538 4018c5f1 f93f0000 00000000 R.E8@....?......
+  0x0000ef70 83c90161 81bc39b9 fc3f0000 00000000 ...a..9..?......
+  0x0000ef80 45336587 3fda8ec4 fd3f0000 00000000 E3e.?....?......
+  0x0000ef90 6ea57abd 51ba0bc9 f63f0000 00000000 n.z.Q....?......
+  0x0000efa0 b046df6b d3e082c9 fe3f0000 00000000 .F.k.....?......
+  0x0000efb0 2a178492 e5a3cf86 fe3f0000 00000000 *........?......
+  0x0000efc0 aabe39b7 d59fb2d7 fb3f0000 00000000 ..9......?......
+  0x0000efd0 35e8396a d20032e7 d43f0000 00000000 5.9j..2..?......
+  0x0000efe0 95009120 cf3895e3 dc3f0000 00000000 ... .8...?......
+  0x0000eff0 78f56a05 c0619db8 e33f0000 00000000 x.j..a...?......
+  0x0000f000 a8abc780 001d999f e93f0000 00000000 .........?......
+  0x0000f010 33b4d688 8b45c19e ee3f0000 00000000 3....E...?......
+  0x0000f020 b1a278ba 1949fdb6 f23f0000 00000000 ..x..I...?......
+  0x0000f030 bb4df416 11b09be9 f53f0000 00000000 .M.......?......
+  0x0000f040 d95801d8 1eabd192 f83f0000 00000000 .X.......?......
+  0x0000f050 8b50c978 141f0086 f93f0000 00000000 .P.x.....?......
+  0x0000f060 3dbecb71 717abffd e43f0000 00000000 =..qqz...?......
+  0x0000f070 75469243 238b07de e73f0000 00000000 uF.C#....?......
+  0x0000f080 75469243 238b07de eb3f0000 00000000 uF.C#....?......
+  0x0000f090 75469243 238b07de ee3f0000 00000000 uF.C#....?......
+  0x0000f0a0 4d5b1242 ca687de2 f03f0000 00000000 M[.B.h}..?......
+  0x0000f0b0 f9f4b102 f2cbe59b f43f0000 00000000 .........?......
+  0x0000f0c0 16dd71d0 a6b5a7ab f13f0000 00000000 ..q......?......
+  0x0000f0d0 9bb6d065 798e07b0 f83f0000 00000000 ...ey....?......
+  0x0000f0e0 d8c4c0f8 03aeacae f93f0000 00000000 .........?......
+  0x0000f0f0 5edc2d1e 2022d2dc fa3f0000 00000000 ^.-. "...?......
+  0x0000f100 58a1de75 1149ea83 fd3f0000 00000000 X..u.I...?......
+  0x0000f110 5aac6b0d 95103397 fd3f0000 00000000 Z.k...3..?......
+  0x0000f120 4c661fff 0a98b3e3 fc3f0000 00000000 Lf.......?......
+  0x0000f130 60aab2f5 39d6fa9e ff3f0000 00000000 `...9....?......
+  0x0000f140 f2d04cea e2200ecd fe3f0000 00000000 ..L.. ...?......
+  0x0000f150 3c8c960f 38a7ad8b fd3f0000 00000000 <...8....?......
+  0x0000f160 fb0dacc8 ade3a19f fa3f0000 00000000 .........?......
+  0x0000f170 1c6fd004 1cbd7af5 d63f0000 00000000 .o....z..?......
+  0x0000f180 5f2dbd94 27d2a4f1 de3f0000 00000000 _-..'....?......
+  0x0000f190 7920a81b 7a5e05c4 e53f0000 00000000 y ..z^...?......
+  0x0000f1a0 3545a4e5 a76b75a9 eb3f0000 00000000 5E...ku..?......
+  0x0000f1b0 9f0d2bb7 4e3e90a8 f03f0000 00000000 ..+.N>...?......
+  0x0000f1c0 e3265a00 94904bc2 f43f0000 00000000 .&Z...K..?......
+  0x0000f1d0 ad7204f4 0d960af8 f73f0000 00000000 .r.......?......
+  0x0000f1e0 da8c350c 7adae39b fa3f0000 00000000 ..5.z....?......
+  0x0000f1f0 2549241d 5b8f478e fb3f0000 00000000 %I$.[.G..?......
+  0x0000f200 05a56942 616c04b3 e7bf0000 00000000 ..iBal..........
+  0x0000f210 a5d9b66a edf964c9 ea3f0000 00000000 ...j..d..?......
+  0x0000f220 cd26ca74 501dfdce ed3f0000 00000000 .&.tP....?......
+  0x0000f230 8178420d e469639e f13f0000 00000000 .xB..ic..?......
+  0x0000f240 582541e8 7bd2629d ec3f0000 00000000 X%A.{.b..?......
+  0x0000f250 d32fa174 d5ab1a8c f63f0000 00000000 ./.t.....?......
+  0x0000f260 cbecac78 b48445db f73f0000 00000000 ...x..E..?......
+  0x0000f270 b194048f 0de3ca80 f83f0000 00000000 .........?......
+  0x0000f280 8f2d1057 5ede8db0 fb3f0000 00000000 .-.W^....?......
+  0x0000f290 eb5be260 fc5b63c6 fc3f0000 00000000 .[.`.[c..?......
+  0x0000f2a0 a54b7356 a1a394f8 fb3f0000 00000000 .KsV.....?......
+  0x0000f2b0 0a59ed84 3c5e4c97 fd3f0000 00000000 .Y..<^L..?......
+  0x0000f2c0 c7271282 b86e93d2 fe3f0000 00000000 .'...n...?......
+  0x0000f2d0 adb1128a c44603b9 fe3f0000 00000000 .....F...?......
+  0x0000f2e0 1c6fe6f8 c88a11a4 fd3f0000 00000000 .o.......?......
+  0x0000f2f0 e613cb59 5419fda5 fb3f0000 00000000 ...YT....?......
+  0x0000f300 b01198c1 bca48b93 f83f0000 00000000 .........?......
+  0x0000f310 0cb86b70 ecd950ae da3f0000 00000000 ..kp..P..?......
+  0x0000f320 2c09aabe 849697ab e23f0000 00000000 ,........?......
+  0x0000f330 1c445559 c4f7318b e93f0000 00000000 .DUY..1..?......
+  0x0000f340 7044dd6e c399aaf0 ee3f0000 00000000 pD.n.....?......
+  0x0000f350 8751d0af 231f65ef f33f0000 00000000 .Q..#.e..?......
+  0x0000f360 ff757c49 b53df889 f83f0000 00000000 .u|I.=...?......
+  0x0000f370 33c8e484 239222b0 fb3f0000 00000000 3...#."..?......
+  0x0000f380 2d5a1365 816a65dd fd3f0000 00000000 -Z.e.je..?......
+  0x0000f390 d38de20b 71ff10ca fe3f0000 00000000 ....q....?......
+  0x0000f3a0 eb910fd8 8264b6f9 e53f0000 00000000 .....d...?......
+  0x0000f3b0 70ad0b22 62cb48bb e73f0000 00000000 p.."b.H..?......
+  0x0000f3c0 56ef1fe9 ddaa90ff ec3f0000 00000000 V........?......
+  0x0000f3d0 c831387a b85993c3 ee3f0000 00000000 .18z.Y...?......
+  0x0000f3e0 f1feb33b 41d40dbf f23f0000 00000000 ...;A....?......
+  0x0000f3f0 9b8198b4 bab67597 f43f0000 00000000 ......u..?......
+  0x0000f400 2f9585d2 8ed6abfb f63f0000 00000000 /........?......
+  0x0000f410 34f8d11a ddbb2ad6 f83f0000 00000000 4.....*..?......
+  0x0000f420 51dc3678 c352b58a fa3f0000 00000000 Q.6x.R...?......
+  0x0000f430 726de6d3 f151418c fc3f0000 00000000 rm...QA..?......
+  0x0000f440 506d6d75 c699f187 fb3f0000 00000000 Pmmu.....?......
+  0x0000f450 4e6d7293 f3418093 fe3f0000 00000000 Nmr..A...?......
+  0x0000f460 068914c6 4e437794 fd3f0000 00000000 ....NCw..?......
+  0x0000f470 b8cc8ac2 abadcfca fe3f0000 00000000 .........?......
+  0x0000f480 10ac758d a2c516da da3f0000 00000000 ..u......?......
+  0x0000f490 704f2ce6 b70ef0ac e23f0000 00000000 pO,......?......
+  0x0000f4a0 b0f86006 ed82e4d7 e83f0000 00000000 ..`......?......
+  0x0000f4b0 2918569a daecce87 ee3f0000 00000000 ).V......?......
+  0x0000f4c0 416286b9 a2a01bb7 f23f0000 00000000 Ab.......?......
+  0x0000f4d0 53a5aa81 4cf8b181 f63f0000 00000000 S...L....?......
+  0x0000f4e0 50a87d00 026427ae f83f0000 00000000 P.}..d'..?......
+  0x0000f4f0 38b7ff6c 306219a5 f93f0000 00000000 8..l0b...?......
+  0x0000f500 e6e06478 d3313ff8 e5bf0000 00000000 ..dx.1?.........
+  0x0000f510 81beb8f3 068ca38b e93f0000 00000000 .........?......
+  0x0000f520 05529a41 ce88848f ec3f0000 00000000 .R.A.....?......
+  0x0000f530 fc40059a 95e9a3db ef3f0000 00000000 .@.......?......
+  0x0000f540 0ea0c2a8 2997a48d ee3f0000 00000000 ....)....?......
+  0x0000f550 488a261a 7e1d49d4 f43f0000 00000000 H.&.~.I..?......
+  0x0000f560 0aa5cb97 31336a8a f63f0000 00000000 ....13j..?......
+  0x0000f570 d468548c 6d6496d2 f73f0000 00000000 .hT.md...?......
+  0x0000f580 dede2023 64d7d1a7 fa3f0000 00000000 .. #d....?......
+  0x0000f590 d11bee10 d4b1f3f0 fa3f0000 00000000 .........?......
+  0x0000f5a0 79bffd42 c2ad13b7 fb3f0000 00000000 y..B.....?......
+  0x0000f5b0 b698d3d7 6ea464fa fd3f0000 00000000 ....n.d..?......
+  0x0000f5c0 98eb198b e0dd56ea fe3f0000 00000000 ......V..?......
+  0x0000f5d0 709d88d0 11d97db1 fe3f0000 00000000 p.....}..?......
+  0x0000f5e0 3d424dd5 ea4dbe9a fd3f0000 00000000 =BM..M...?......
+  0x0000f5f0 30ea9814 def4a79b fb3f0000 00000000 0........?......
+  0x0000f600 d67a6bd9 e1675c8a f83f0000 00000000 .zk..g\..?......
+  0x0000f610 13ad5b50 76a0a1b4 d53f0000 00000000 ..[Pv....?......
+  0x0000f620 5e3e1a77 f419cfb1 dd3f0000 00000000 ^>.w.....?......
+  0x0000f630 98f4f2f9 0d003d90 e43f0000 00000000 ......=..?......
+  0x0000f640 35762561 c3c662f9 e93f0000 00000000 5v%a..b..?......
+  0x0000f650 30a60b15 548111f8 ee3f0000 00000000 0...T....?......
+  0x0000f660 bf27afbd 2fe8f78e f33f0000 00000000 .'../....?......
+  0x0000f670 1b15d26e 373884b6 f63f0000 00000000 ...n78...?......
+  0x0000f680 02ce78e7 52dc6ae5 f83f0000 00000000 ..x.R.j..?......
+  0x0000f690 8838ad80 c92863d1 f93f0000 00000000 .8...(c..?......
+  0x0000f6a0 ff4bbaf5 772bf0d4 e83f0000 00000000 .K..w+...?......
+  0x0000f6b0 3f14f078 e21d6592 ec3f0000 00000000 ?..x..e..?......
+  0x0000f6c0 d4b94cf5 9c82cfdd ed3f0000 00000000 ..L......?......
+  0x0000f6d0 896ce87f 9387bea7 f23f0000 00000000 .l.......?......
+  0x0000f6e0 6acc3a74 79dcfdf3 f33f0000 00000000 j.:ty....?......
+  0x0000f6f0 705ccdc0 e4127a80 f63f0000 00000000 p\....z..?......
+  0x0000f700 f53342ee 5ab41580 f93f0000 00000000 .3B.Z....?......
+  0x0000f710 2928f2e7 198d2b94 fa3f0000 00000000 )(....+..?......
+  0x0000f720 595bd23a d39a2a9f f53f0000 00000000 Y[.:..*..?......
+  0x0000f730 63e23c62 003dcdda fc3f0000 00000000 c.<b.=...?......
+  0x0000f740 37da4799 0a675b9e fe3f0000 00000000 7.G..g[..?......
+  0x0000f750 0f1fb234 e1fe0989 ff3f0000 00000000 ...4.....?......
+  0x0000f760 aab7a253 0a8cb3ca fe3f0000 00000000 ...S.....?......
+  0x0000f770 55a2be6f f0185ace fd3f0000 00000000 U..o..Z..?......
+  0x0000f780 c67f0c41 a4d8bf8a fc3f0000 00000000 ...A.....?......
+  0x0000f790 f8a4352f 0939b5de f93f0000 00000000 ..5/.9...?......
+  0x0000f7a0 ccbd0f0b 7b29f8a1 f63f0000 00000000 ....{)...?......
+  0x0000f7b0 9cf50b07 7d07cc96 d93f0000 00000000 ....}....?......
+  0x0000f7c0 c5c5ef12 5fd77094 e13f0000 00000000 ...._.p..?......
+  0x0000f7d0 8801b994 1568d4f0 e73f0000 00000000 .....h...?......
+  0x0000f7e0 b6dbc6b6 150c32d0 ed3f0000 00000000 ......2..?......
+  0x0000f7f0 e5715721 6b7b18cf f23f0000 00000000 .qW!k{...?......
+  0x0000f800 e33257b5 0b9cb5ee f63f0000 00000000 .2W......?......
+  0x0000f810 a7e72495 dfe95e98 fa3f0000 00000000 ..$...^..?......
+  0x0000f820 4d3ae255 b47386bf fc3f0000 00000000 M:.U.s...?......
+  0x0000f830 feb875e6 aeadcdae fd3f0000 00000000 ..u......?......
+  0x0000f840 df0bbf0a 32e074f6 e33f0000 00000000 ....2.t..?......
+  0x0000f850 632a67c9 2b44a6d7 e63f0000 00000000 c*g.+D...?......
+  0x0000f860 632a67c9 2b44a6d7 ea3f0000 00000000 c*g.+D...?......
+  0x0000f870 632a67c9 2b44a6d7 ed3f0000 00000000 c*g.+D...?......
+  0x0000f880 a90f60fc 05e77ae2 ef3f0000 00000000 ..`...z..?......
+  0x0000f890 32ec71d2 83cf429a f33f0000 00000000 2.q...B..?......
+  0x0000f8a0 71d2a393 631737af f13f0000 00000000 q...c.7..?......
+  0x0000f8b0 20540af5 fc62dcb7 f73f0000 00000000  T...b...?......
+  0x0000f8c0 d0833673 7a3defa6 f83f0000 00000000 ..6sz=...?......
+  0x0000f8d0 039e9774 c126d88a fa3f0000 00000000 ...t.&...?......
+  0x0000f8e0 da57af0d 23e52e8c fc3f0000 00000000 .W..#....?......
+  0x0000f8f0 a3762e22 54cfcca8 fb3f0000 00000000 .v."T....?......
+  0x0000f900 88c4fc50 b38e70c5 fd3f0000 00000000 ...P..p..?......
+  0x0000f910 24fa38b8 4eec8b91 ff3f0000 00000000 $.8.N....?......
+  0x0000f920 4406e7b6 92d3bcb6 fe3f0000 00000000 D........?......
+  0x0000f930 e5cdf763 197c04f7 fc3f0000 00000000 ...c.|...?......
+  0x0000f940 ccbed6a6 5722278d fa3f0000 00000000 ....W"'..?......
+  0x0000f950 207ad7bd d734b992 d43f0000 00000000  z...4...?......
+  0x0000f960 381ce05e 04506e90 dc3f0000 00000000 8..^.Pn..?......
+  0x0000f970 7298976c 7cf852ea e23f0000 00000000 r..l|.R..?......
+  0x0000f980 f9da361d 4c4a92ca e83f0000 00000000 ..6.LJ...?......
+  0x0000f990 82cefcce c45480c9 ed3f0000 00000000 .....T...?......
+  0x0000f9a0 d495f15e 1cd642e8 f13f0000 00000000 ...^..B..?......
+  0x0000f9b0 91ab3032 1e354194 f53f0000 00000000 ..02.5A..?......
+  0x0000f9c0 1d062033 15fa59ba f73f0000 00000000 .. 3..Y..?......
+  0x0000f9d0 5a9b9555 5cd714aa f83f0000 00000000 Z..U\....?......
+  0x0000f9e0 6883fc4a b7384aad eabf0000 00000000 h..J.8J.........
+  0x0000f9f0 c42aedec 144ecc8c ee3f0000 00000000 .*...N...?......
+  0x0000fa00 41a4bb1d e5c69cd8 ed3f0000 00000000 A........?......
+  0x0000fa10 7aed9414 3eb065ca f33f0000 00000000 z...>.e..?......
+  0x0000fa20 dac257b1 e668c29a f63f0000 00000000 ..W..h...?......
+  0x0000fa30 eddba30b 11f32580 f73f0000 00000000 ......%..?......
+  0x0000fa40 8e0fd4b5 6952fc87 f93f0000 00000000 ....iR...?......
+  0x0000fa50 09a6bdd5 10f697ee fb3f0000 00000000 .........?......
+  0x0000fa60 2e9ccca7 1c29e0b5 fd3f0000 00000000 .....)...?......
+  0x0000fa70 c383b534 6fc5d9b2 fe3f0000 00000000 ...4o....?......
+  0x0000fa80 efbabd4c f4389bf9 fe3f0000 00000000 ...L.8...?......
+  0x0000fa90 763bb62f e003cec2 fe3f0000 00000000 v;./.....?......
+  0x0000faa0 7d896723 6c0444da fd3f0000 00000000 }.g#l.D..?......
+  0x0000fab0 e12094a2 e92e6eaf fc3f0000 00000000 . ....n..?......
+  0x0000fac0 e005ed38 4518d6bf fa3f0000 00000000 ...8E....?......
+  0x0000fad0 a2a06886 fdbf0280 f83f0000 00000000 ..h......?......
+  0x0000fae0 78146da5 103b8d9d f43f0000 00000000 x.m..;...?......
+  0x0000faf0 f422ae2e 855c998d da3f0000 00000000 ."...\...?......
+  0x0000fb00 686af319 13f7628b e23f0000 00000000 hj....b..?......
+  0x0000fb10 a2eac452 dae423e2 e83f0000 00000000 ...R..#..?......
+  0x0000fb20 bb0449d3 ab1c7fc3 ee3f0000 00000000 ..I......?......
+  0x0000fb30 2d1e4adf 97b876c2 f33f0000 00000000 -.J...v..?......
+  0x0000fb40 9c6031fb 7d3426e0 f73f0000 00000000 .`1.}4&..?......
+  0x0000fb50 cac4a96b f0ab138f fb3f0000 00000000 ...k.....?......
+  0x0000fb60 caece5b2 05d2d7b3 fd3f0000 00000000 .........?......
+  0x0000fb70 4344644f 822724a4 fe3f0000 00000000 CDdO.'$..?......
+  0x0000fb80 abfe5717 a8fff9fb e73f0000 00000000 ..W......?......
+  0x0000fb90 167f0c90 c3df3bad eb3f0000 00000000 ......;..?......
+  0x0000fba0 f929d336 d2df3c83 ed3f0000 00000000 .).6..<..?......
+  0x0000fbb0 49fcb8bf ba457fc6 f13f0000 00000000 I....E...?......
+  0x0000fbc0 9f7ad1fb 50cac386 f33f0000 00000000 .z..P....?......
+  0x0000fbd0 3934b2c0 21006cb2 f53f0000 00000000 94..!.l..?......
+  0x0000fbe0 96a37a7e e6c05d99 f83f0000 00000000 ..z~..]..?......
+  0x0000fbf0 23df5dca c8b981ee f83f0000 00000000 #.]......?......
+  0x0000fc00 786bb29c ef1342b4 fa3f0000 00000000 xk....B..?......
+  0x0000fc10 a33a4a2e df982b88 fd3f0000 00000000 .:J...+..?......
+  0x0000fc20 8609f031 50084da7 fe3f0000 00000000 ...1P.M..?......
+  0x0000fc30 532cd2df 4814bc85 ff3f0000 00000000 S,..H....?......
+  0x0000fc40 512f4fa0 36f271c3 fe3f0000 00000000 Q/O.6.q..?......
+  0x0000fc50 aafe96e1 7979c2c5 fd3f0000 00000000 ....yy...?......
+  0x0000fc60 60342a7e 15ba9684 fc3f0000 00000000 `4*~.....?......
+  0x0000fc70 9040ed54 cb6897d4 f93f0000 00000000 .@.T.h...?......
+  0x0000fc80 f42e380f 4ea99c9a f63f0000 00000000 ..8.N....?......
+  0x0000fc90 8c015fe9 1141aed8 d63f0000 00000000 .._..A...?......
+  0x0000fca0 8685b9a1 0d884bd5 de3f0000 00000000 ......K..?......
+  0x0000fcb0 502986b9 5d4506ad e53f0000 00000000 P)..]E...?......
+  0x0000fcc0 353ffcfd 67119495 eb3f0000 00000000 5?..g....?......
+  0x0000fcd0 fda3d369 efc6c994 f03f0000 00000000 ...i.....?......
+  0x0000fce0 11778411 2d4c80ab f43f0000 00000000 .w..-L...?......
+  0x0000fcf0 f845c0b6 f228f1da f73f0000 00000000 .E...(...?......
+  0x0000fd00 7971ad2b df019a89 fa3f0000 00000000 yq.+.....?......
+  0x0000fd10 3c4f7d45 14f52cfb fa3f0000 00000000 <O}E..,..?......
+  0x0000fd20 08398824 797e2dd2 f03f0000 00000000 .9.$y~-..?......
+  0x0000fd30 77b53f92 91a60ac5 f43f0000 00000000 w.?......?......
+  0x0000fd40 c8bef75f bf5169ac f73f0000 00000000 ..._.Qi..?......
+  0x0000fd50 ae0ef7a7 e46dc7ba f93f0000 00000000 .....m...?......
+  0x0000fd60 034bf97d 6b92158c fb3f0000 00000000 .K.}k....?......
+  0x0000fd70 509ff870 a9ba179a fc3f0000 00000000 P..p.....?......
+  0x0000fd80 18da7933 8d1b6980 fd3f0000 00000000 ..y3..i..?......
+  0x0000fd90 8c610af9 906c19a5 fd3f0000 00000000 .a...l...?......
+  0x0000fda0 0a0f6721 1ea04aa0 e13f0000 00000000 ..g!..J..?......
+  0x0000fdb0 da71f9c8 ef5936fe e83f0000 00000000 .q...Y6..?......
+  0x0000fdc0 57f1b853 b95fad9e ef3f0000 00000000 W..S._...?......
+  0x0000fdd0 9b9393fa 0525a2c7 f43f0000 00000000 .....%...?......
+  0x0000fde0 682c30f5 dac09486 f93f0000 00000000 h,0......?......
+  0x0000fdf0 d06e689f 48b7a5be fc3f0000 00000000 .nh.H....?......
+  0x0000fe00 54c2803e a79cb0f2 ff3f0000 00000000 T..>.....?......
+  0x0000fe10 00000000 00dcc2b5 fa3f0000 00000000 .........?......
+  0x0000fe20 00000000 00dcc2b5 fb3f0000 00000000 .........?......
+  0x0000fe30 62847e2d b495f0fe dabf0000 00000000 b.~-............
+  0x0000fe40 4ae31e22 477034bf dc3f0000 00000000 J.."Gp4..?......
+  0x0000fe50 b8bfb5ed 28312181 e33f0000 00000000 ....(1!..?......
+  0x0000fe60 9d9cebcc e8aaafc3 e43f0000 00000000 .........?......
+  0x0000fe70 1620a4df b5e4d0d2 e93f0000 00000000 . .......?......
+  0x0000fe80 fce79ab3 58a831a2 eb3f0000 00000000 ....X.1..?......
+  0x0000fe90 299a2c67 1aba10b1 ef3f0000 00000000 ).,g.....?......
+  0x0000fea0 5e12ed3f 930e948b f13f0000 00000000 ^..?.....?......
+  0x0000feb0 2cad404c 8e2ee7a1 f43f0000 00000000 ,.@L.....?......
+  0x0000fec0 66626052 d4222185 f63f0000 00000000 fb`R."!..?......
+  0x0000fed0 60620e76 5a86149c f83f0000 00000000 `b.vZ....?......
+  0x0000fee0 86d9cb6e 91fe7d8b fa3f0000 00000000 ...n..}..?......
+  0x0000fef0 9cc5573a b90ab087 fb3f0000 00000000 ..W:.....?......
+  0x0000ff00 b4d29da1 4ea33295 fd3f0000 00000000 ....N.2..?......
+  0x0000ff10 a2de476e 12870eb7 fb3f0000 00000000 ..Gn.....?......
+  0x0000ff20 6c5b3eda 22b3bd89 ff3f0000 00000000 l[>."....?......
+  0x0000ff30 3bb83945 fa7585b6 fe3f0000 00000000 ;.9E.u...?......
+  0x0000ff40 8bd2faec 1e0639b2 ff3f0000 00000000 ......9..?......
+  0x0000ff50 0f6e4e91 7e5da1ed fd3f0000 00000000 .nN.~]...?......
+  0x0000ff60 9e3d8ff7 55eb86cd cf3f0000 00000000 .=..U....?......
+  0x0000ff70 e25b436e f4b3b18b d83f0000 00000000 .[Cn.....?......
+  0x0000ff80 97d7d761 12c76e9f df3f0000 00000000 ...a..n..?......
+  0x0000ff90 8fcf75bb d97acdc6 e53f0000 00000000 ..u..z...?......
+  0x0000ffa0 3ec38038 def0a693 eb3f0000 00000000 >..8.....?......
+  0x0000ffb0 38d2671b 5f27ae85 f03f0000 00000000 8.g._'...?......
+  0x0000ffc0 056649b6 ea671891 f43f0000 00000000 .fI..g...?......
+  0x0000ffd0 454308e1 fd0e3cb2 f73f0000 00000000 EC....<..?......
+  0x0000ffe0 f7bb9485 72c8bbda f93f0000 00000000 ....r....?......
+  0x0000fff0 374c7a4c b6faeac4 fa3f0000 00000000 7LzL.....?......
+  0x00010000 f415700c 052153fb dc3f0000 00000000 ..p..!S..?......
+  0x00010010 b90dc627 a3f4139d df3f0000 00000000 ...'.....?......
+  0x00010020 de52b056 6070fbd7 e43f0000 00000000 .R.V`p...?......
+  0x00010030 38646c4f e1c5e58b e73f0000 00000000 8dlO.....?......
+  0x00010040 201d2f28 4863a38e eb3f0000 00000000  ./(Hc...?......
+  0x00010050 32cdb5f8 ed71e4c3 ed3f0000 00000000 2....q...?......
+  0x00010060 3bcf3321 856d32b2 f03f0000 00000000 ;.3!.m2..?......
+  0x00010070 f3cd629c 88cc3e88 f33f0000 00000000 ..b...>..?......
+  0x00010080 f1253c69 fa812fc8 f43f0000 00000000 .%<i../..?......
+  0x00010090 efebf647 2b0d6dc3 f73f0000 00000000 ...G+.m..?......
+  0x000100a0 cde51817 4b5feec2 f63f0000 00000000 ....K_...?......
+  0x000100b0 dbbcf33d 46bd6286 fb3f0000 00000000 ...=F.b..?......
+  0x000100c0 54281c76 6155148b fb3f0000 00000000 T(.vaU...?......
+  0x000100d0 6a870585 bd610284 fd3f0000 00000000 j....a...?......
+  0x000100e0 c9ca55b3 efbaf8a3 fe3f0000 00000000 ..U......?......
+  0x000100f0 2ab71e5f 5b36628a fd3f0000 00000000 *.._[6b..?......
+  0x00010100 1800e36e 1c2647ab fe3f0000 00000000 ...n.&G..?......
+  0x00010110 fd9f2372 3c1b978a fe3f0000 00000000 ..#r<....?......
+  0x00010120 fbff3850 fa91bedd fb3f0000 00000000 ..8P.....?......
+  0x00010130 43b9500b ace223fc cf3f0000 00000000 C.P...#..?......
+  0x00010140 ecddb0ef 106460ab d83f0000 00000000 .....d`..?......
+  0x00010150 96108fe1 577e97c3 df3f0000 00000000 ....W~...?......
+  0x00010160 14b3f1ef da06e4f3 e53f0000 00000000 .........?......
+  0x00010170 c2e91b65 adab23b5 eb3f0000 00000000 ...e..#..?......
+  0x00010180 a264420b c2acffa3 f03f0000 00000000 .dB......?......
+  0x00010190 9f096387 36b000b2 f43f0000 00000000 ..c.6....?......
+  0x000101a0 7e890bbb eb6aa8da f73f0000 00000000 ~....j...?......
+  0x000101b0 0a047e66 eac22b86 fa3f0000 00000000 ..~f..+..?......
+  0x000101c0 a87ad011 941894f1 fa3f0000 00000000 .z.......?......
+  0x000101d0 c06cdcb9 a946a5a6 e0bf0000 00000000 .l...F..........
+  0x000101e0 28dfa082 d49dd091 e33f0000 00000000 (........?......
+  0x000101f0 3b877606 44d6bde7 e73f0000 00000000 ;.v.D....?......
+  0x00010200 39d2fb15 362f00dd ea3f0000 00000000 9...6/...?......
+  0x00010210 5da50082 a0a110dc ed3f0000 00000000 ]........?......
+  0x00010220 8e7603b6 2652a9f8 f03f0000 00000000 .v..&R...?......
+  0x00010230 550b1807 4ab68c8c f23f0000 00000000 U...J....?......
+  0x00010240 14c191e7 c41a9afc f53f0000 00000000 .........?......
+  0x00010250 21755a36 d8efa08b f53f0000 00000000 !uZ6.....?......
+  0x00010260 78bdd436 257f32d8 f93f0000 00000000 x..6%.2..?......
+  0x00010270 34c39aa4 9a7f2c86 fb3f0000 00000000 4.....,..?......
+  0x00010280 40065fd3 2e44a38c fb3f0000 00000000 @._..D...?......
+  0x00010290 8fbe7a30 04c84d83 fe3f0000 00000000 ..z0..M..?......
+  0x000102a0 e407069e 3239b7c9 fe3f0000 00000000 ....29...?......
+  0x000102b0 3f8b05be f1e033b0 fc3f0000 00000000 ?.....3..?......
+  0x000102c0 9729e905 e8cbf8fb fe3f0000 00000000 .).......?......
+  0x000102d0 1b5b2eb3 ef7c0cbd ff3f0000 00000000 .[...|...?......
+  0x000102e0 39693413 c4e0bcb0 fd3f0000 00000000 9i4......?......
+  0x000102f0 427860f1 966efcc9 fa3f0000 00000000 Bx`..n...?......
+  0x00010300 8e89c909 6cfec384 d33f0000 00000000 ....l....?......
+  0x00010310 fdf64ddd da6d7ab4 db3f0000 00000000 ..M..mz..?......
+  0x00010320 f538bf45 3dc3facd e23f0000 00000000 .8.E=....?......
+  0x00010330 d84f4381 14fc6b80 e93f0000 00000000 .OC...k..?......
+  0x00010340 943b747d b771c2be ee3f0000 00000000 .;t}.q...?......
+  0x00010350 f78a1fd3 8767b5ac f33f0000 00000000 .....g...?......
+  0x00010360 a7b6ef30 e4d074bb f73f0000 00000000 ...0..t..?......
+  0x00010370 b897d899 444b45e6 fa3f0000 00000000 ....DKE..?......
+  0x00010380 77dd3922 adf34b8d fd3f0000 00000000 w.9"..K..?......
+  0x00010390 905b3a7b fb9968fe fd3f0000 00000000 .[:{..h..?......
+  0x000103a0 350abd48 22208bf0 d43f0000 00000000 5..H" ...?......
+  0x000103b0 f07c704d d78f7ea3 dd3f0000 00000000 .|pM..~..?......
+  0x000103c0 a9d45858 5f8c98ba e43f0000 00000000 ..XX_....?......
+  0x000103d0 5c6d9513 db65ace8 ea3f0000 00000000 \m...e...?......
+  0x000103e0 b5d337c9 52e4ceac f03f0000 00000000 ..7.R....?......
+  0x000103f0 13bd536b bcb6749c f53f0000 00000000 ..Sk..t..?......
+  0x00010400 6a686d42 5ed7d0a9 f93f0000 00000000 jhmB^....?......
+  0x00010410 bd3fca0d efe299d0 fc3f0000 00000000 .?.......?......
+  0x00010420 21ee58b9 1db177e6 ff3f0000 00000000 !.X...w..?......
+  0x00010430 76e8a504 8da66082 e13f0000 00000000 v.....`..?......
+  0x00010440 85a53aa5 5ebbac92 e43f0000 00000000 ..:.^....?......
+  0x00010450 26d22c3a 2858cf87 e83f0000 00000000 &.,:(X...?......
+  0x00010460 e64e894e 36ea57b7 eb3f0000 00000000 .N.N6.W..?......
+  0x00010470 5e6a4560 0e8ba3fb ec3f0000 00000000 ^jE`.....?......
+  0x00010480 8e1a7332 d4119e95 f13f0000 00000000 ..s2.....?......
+  0x00010490 afcb0d76 00e6f9ce f13f0000 00000000 ...v.....?......
+  0x000104a0 2bd2d489 039c8c9e f53f0000 00000000 +........?......
+  0x000104b0 4803c184 ccb77da3 f73f0000 00000000 H.....}..?......
+  0x000104c0 f91c995a df9c28c1 f53f0000 00000000 ...Z..(..?......
+  0x000104d0 75021c7c 4f93a58a fa3f0000 00000000 u..|O....?......
+  0x000104e0 5be82ba3 cbacdfc7 fb3f0000 00000000 [.+......?......
+  0x000104f0 1bfcecf4 0aefcfe5 fb3f0000 00000000 .........?......
+  0x00010500 3009c759 332cf7b7 f53f0000 00000000 0..Y3,...?......
+  0x00010510 38e15bd3 256ccdb0 fc3f0000 00000000 8.[.%l...?......
+  0x00010520 2a2d8d4a b502b882 fd3f0000 00000000 *-.J.....?......
+  0x00010530 e1bf29fc 0c3b27c9 fc3f0000 00000000 ..)..;'..?......
+  0x00010540 d141ec3b 0b0eb5b6 fb3f0000 00000000 .A.;.....?......
+  0x00010550 e4383f45 0b0e4fba f93f0000 00000000 .8?E..O..?......
+  0x00010560 59a454af b49a9ba5 f63f0000 00000000 Y.T......?......
+  0x00010570 d6bbaaaa ed7ad9ba d83f0000 00000000 .....z...?......
+  0x00010580 306955cd 22760bd8 e03f0000 00000000 0iU."v...?......
+  0x00010590 5e2f2f1e dddeeccd e73f0000 00000000 ^//......?......
+  0x000105a0 c877f750 822b0ad1 ed3f0000 00000000 .w.P.+...?......
+  0x000105b0 cd7a3169 d74311f4 f23f0000 00000000 .z1i.C...?......
+  0x000105c0 3d5f40b1 c49278a5 f73f0000 00000000 =_@...x..?......
+  0x000105d0 fedd8aad 2cf90bfb fa3f0000 00000000 ....,....?......
+  0x000105e0 f6554592 94a6e5c2 fd3f0000 00000000 .UE......?......
+  0x000105f0 473b548d 28a823f8 fe3f0000 00000000 G;T.(.#..?......
+  0x00010600 20599851 aa08d3c3 d03f0000 00000000  Y.Q.....?......
+  0x00010610 948c75c3 e36f1985 d93f0000 00000000 ..u..o...?......
+  0x00010620 33a4e7ce 5af6e797 e03f0000 00000000 3...Z....?......
+  0x00010630 e90d8d2d 8adc6abd e63f0000 00000000 ...-..j..?......
+  0x00010640 008634a3 e07fae8c ec3f0000 00000000 ..4......?......
+  0x00010650 8d95a230 e222bdfe f03f0000 00000000 ...0."...?......
+  0x00010660 1b442ba7 45dd3e8a f53f0000 00000000 .D+.E.>..?......
+  0x00010670 e12551f1 a203d2a9 f83f0000 00000000 .%Q......?......
+  0x00010680 85ba757e 894a68d0 fa3f0000 00000000 ..u~.Jh..?......
+  0x00010690 e3d3c47b a2239fbb fb3f0000 00000000 ...{.#...?......
+  0x000106a0 cfa8b41e ecd26a93 e8bf0000 00000000 ......j.........
+  0x000106b0 02d36126 a78745b8 ea3f0000 00000000 ..a&..E..?......
+  0x000106c0 5d932d1f 682180e2 ee3f0000 00000000 ].-.h!...?......
+  0x000106d0 4a99e285 5b6d1499 f13f0000 00000000 J...[m...?......
+  0x000106e0 a6e217e0 a378b1df f33f0000 00000000 .....x...?......
+  0x000106f0 0e7222dc 350495b2 f63f0000 00000000 .r".5....?......
+  0x00010700 b1197059 f68640f7 f63f0000 00000000 ..pY..@..?......
+  0x00010710 f5edb989 52e4f6a9 fa3f0000 00000000 ....R....?......
+  0x00010720 e17439ea 450dfbe1 f93f0000 00000000 .t9.E....?......
+  0x00010730 ddc0b044 d47186e7 fc3f0000 00000000 ...D.q...?......
+  0x00010740 094b029f 7524e5eb fd3f0000 00000000 .K..u$...?......
+  0x00010750 911aae56 f4d779f1 f93f0000 00000000 ...V..y..?......
+  0x00010760 a06e8687 750ec4a0 ff3f0000 00000000 .n..u....?......
+  0x00010770 480a68e9 1212f5a8 fe3f0000 00000000 H.h......?......
+  0x00010780 06d5eced db742a87 fc3f0000 00000000 .....t*..?......
+  0x00010790 2df76a31 91e8d7dd da3f0000 00000000 -.j1.....?......
+  0x000107a0 01d22f22 6b35eaaf e23f0000 00000000 ../"k5...?......
+  0x000107b0 688f179b edf79bdb e83f0000 00000000 h........?......
+  0x000107c0 9c91a1ec a171258a ee3f0000 00000000 .....q%..?......
+  0x000107d0 a06ec423 7d9942ba f23f0000 00000000 .n.#}.B..?......
+  0x000107e0 3d86aaea 2f8ced83 f63f0000 00000000 =.../....?......
+  0x000107f0 e811958e c7e626b1 f83f0000 00000000 ......&..?......
+  0x00010800 4b9e3dbe 4efdf0a7 f93f0000 00000000 K.=.N....?......
+  0x00010810 61935f59 f84cb89b ea3f0000 00000000 a._Y.L...?......
+  0x00010820 f5a0334e 59434188 ed3f0000 00000000 ..3NYCA..?......
+  0x00010830 1415fa77 c46b4999 f03f0000 00000000 ...w.kI..?......
+  0x00010840 aeba873c 228f30a8 f33f0000 00000000 ...<".0..?......
+  0x00010850 49b752ff 89510ead f33f0000 00000000 I.R..Q...?......
+  0x00010860 6a56e6cb f6e149fa f73f0000 00000000 jV....I..?......
+  0x00010870 d374e060 893f52d4 f83f0000 00000000 .t.`.?R..?......
+  0x00010880 15be5c8b 8cc464c3 fa3f0000 00000000 ..\...d..?......
+  0x00010890 2d6a2ec1 88cb51cf fc3f0000 00000000 -j....Q..?......
+  0x000108a0 55b03173 4e415ce1 fc3f0000 00000000 U.1sNA\..?......
+  0x000108b0 659148e9 a4f468cb fc3f0000 00000000 e.H...h..?......
+  0x000108c0 e5926b11 4b508dd0 fe3f0000 00000000 ..k.KP...?......
+  0x000108d0 e919a3a7 56f485a4 fe3f0000 00000000 ....V....?......
+  0x000108e0 576d5da5 976beadf fc3f0000 00000000 Wm]..k...?......
+  0x000108f0 adeab32a 6456e7ff f93f0000 00000000 ...*dV...?......
+  0x00010900 94cc4496 0b4da596 dc3f0000 00000000 ..D..M...?......
+  0x00010910 731c5160 3028eaee e33f0000 00000000 s.Q`0(...?......
+  0x00010920 346365f4 e0ea2095 ea3f0000 00000000 4ce... ..?......
+  0x00010930 27f0ee28 12c09ebb ef3f0000 00000000 '..(.....?......
+  0x00010940 fc65087d d301f7fc f33f0000 00000000 .e.}.....?......
+  0x00010950 f36f3ebb ebc02cb3 f73f0000 00000000 .o>...,..?......
+  0x00010960 d01c2ee1 134498f0 f93f0000 00000000 .....D...?......
+  0x00010970 62d01690 43ec15e4 fa3f0000 00000000 b...C....?......
+  0x00010980 36ef4061 5924afa3 edbf0000 00000000 6.@aY$..........
+  0x00010990 1d0d698d e40825b8 f03f0000 00000000 ..i...%..?......
+  0x000109a0 c575f5a7 cba8c1ff f13f0000 00000000 .u.......?......
+  0x000109b0 4179d32c 8390a894 f63f0000 00000000 Ay.,.....?......
+  0x000109c0 cbfa7c00 780651bf f73f0000 00000000 ..|.x.Q..?......
+  0x000109d0 aecf25ed d62c99e4 f83f0000 00000000 ..%..,...?......
+  0x000109e0 a36246a2 a2360ed8 fb3f0000 00000000 .bF..6...?......
+  0x000109f0 b5854785 309909e5 fc3f0000 00000000 ..G.0....?......
+  0x00010a00 a737fa5a 475b12ff fb3f0000 00000000 .7.ZG[...?......
+  0x00010a10 abc6061a 9d9d3fc1 fd3f0000 00000000 ......?..?......
+  0x00010a20 b3dcf42d 9147dd99 ff3f0000 00000000 ...-.G...?......
+  0x00010a30 f85885aa 7d1775dd fe3f0000 00000000 .X..}.u..?......
+  0x00010a40 cb897b1e 86250dc4 fd3f0000 00000000 ..{..%...?......
+  0x00010a50 eef83129 9c6b3bc6 fb3f0000 00000000 ..1).k;..?......
+  0x00010a60 d4c0815d 6ed134b0 f83f0000 00000000 ...]n.4..?......
+  0x00010a70 9fe749bf 69a8629f e03f0000 00000000 ..I.i.b..?......
+  0x00010a80 57355fb5 1777c6fc e73f0000 00000000 W5_..w...?......
+  0x00010a90 16bda88e 0fbec79d ee3f0000 00000000 .........?......
+  0x00010aa0 1f2ea7d0 353e81c6 f33f0000 00000000 ....5>...?......
+  0x00010ab0 cca25bb3 2dfed185 f83f0000 00000000 ..[.-....?......
+  0x00010ac0 f7b65498 8fd191bd fb3f0000 00000000 ..T......?......
+  0x00010ad0 70838a5b dd868dfe fd3f0000 00000000 p..[.....?......
+  0x00010ae0 510c6083 8e6651f1 fe3f0000 00000000 Q.`..fQ..?......
+  0x00010af0 ff15ab2d be5fd1a9 debf0000 00000000 ...-._..........
+  0x00010b00 3fb3f567 c6339794 e13f0000 00000000 ?..g.3...?......
+  0x00010b10 97ea8177 242927ec e53f0000 00000000 ...w$)'..?......
+  0x00010b20 ac6390b5 782a35e1 e83f0000 00000000 .c..x*5..?......
+  0x00010b30 318127f5 d40cbae5 eb3f0000 00000000 1.'......?......
+  0x00010b40 424dc116 537c1781 ef3f0000 00000000 BM..S|...?......
+  0x00010b50 e91f9ac1 9b8afaa0 f03f0000 00000000 .........?......
+  0x00010b60 0b279dfc d667ab89 f43f0000 00000000 .'...g...?......
+  0x00010b70 e03b2836 bb2f05aa f23f0000 00000000 .;(6./...?......
+  0x00010b80 7cdd0468 26d8df83 f83f0000 00000000 |..h&....?......
+  0x00010b90 5332aa29 eec3cc8b f93f0000 00000000 S2.).....?......
+  0x00010ba0 7cd14977 35c6bb9a fa3f0000 00000000 |.Iw5....?......
+  0x00010bb0 b5ac2521 71d1dcba fc3f0000 00000000 ..%!q....?......
+  0x00010bc0 4856b6a2 2db44cac fc3f0000 00000000 HV..-.L..?......
+  0x00010bd0 312e2bec fed60fa3 fd3f0000 00000000 1.+......?......
+  0x00010be0 15e4e622 1a7a2097 ff3f0000 00000000 ...".z ..?......
+  0x00010bf0 f666c744 af4904c0 fe3f0000 00000000 .f.D.I...?......
+  0x00010c00 12c174d3 f2a13b82 fd3f0000 00000000 ..t...;..?......
+  0x00010c10 3901aaf1 f06fd694 fa3f0000 00000000 9....o...?......
+  0x00010c20 a4ae0064 e72d32ca cd3f0000 00000000 ...d.-2..?......
+  0x00010c30 b376f845 331b6e89 d63f0000 00000000 .v.E3.n..?......
+  0x00010c40 791feddc e748d99c dd3f0000 00000000 y....H...?......
+  0x00010c50 2dc67f89 bda394c3 e33f0000 00000000 -........?......
+  0x00010c60 d51bf8df 87534291 e93f0000 00000000 .....SB..?......
+  0x00010c70 166099d0 44828383 ee3f0000 00000000 .`..D....?......
+  0x00010c80 30a6bf8a 4566be8e f23f0000 00000000 0...Ef...?......
+  0x00010c90 3a754cf7 538e58af f53f0000 00000000 :uL.S.X..?......
+  0x00010ca0 86b0eec3 ac3f30d7 f73f0000 00000000 .....?0..?......
+  0x00010cb0 5bcfa129 84f5b9c1 f83f0000 00000000 [..).....?......
+  0x00010cc0 11f0523e 20617fe6 e03f0000 00000000 ..R> a...?......
+  0x00010cd0 0aa70e23 a2a6a781 e43f0000 00000000 ...#.....?......
+  0x00010ce0 12baeb40 2c051af0 e73f0000 00000000 ...@,....?......
+  0x00010cf0 cc50d2ab 4a9011a2 eb3f0000 00000000 .P..J....?......
+  0x00010d00 0b3d4fa0 4efaacf9 ec3f0000 00000000 .=O.N....?......
+  0x00010d10 128dee44 5c9aea8b f13f0000 00000000 ...D\....?......
+  0x00010d20 b2382a9f 4f2d5af9 f03f0000 00000000 .8*.O-Z..?......
+  0x00010d30 e2c65858 abe9b3b9 f53f0000 00000000 ..XX.....?......
+  0x00010d40 a8020a5c 4c21199b f73f0000 00000000 ...\L!...?......
+  0x00010d50 8c9df8fe 10462bb6 f73f0000 00000000 .....F+..?......
+  0x00010d60 ea9f25f7 0bea3df4 fa3f0000 00000000 ..%...=..?......
+  0x00010d70 c4ca01fa aa6eb4f4 fb3f0000 00000000 .....n...?......
+  0x00010d80 f6b1458e 1646cffe f73f0000 00000000 ..E..F...?......
+  0x00010d90 71b55fea 2af93dcc fd3f0000 00000000 q._.*.=..?......
+  0x00010da0 64d9fb77 a49938df fe3f0000 00000000 d..w..8..?......
+  0x00010db0 eceefe3b d67005b5 fe3f0000 00000000 ...;.p...?......
+  0x00010dc0 f0624671 13ff1e9f fd3f0000 00000000 .bFq.....?......
+  0x00010dd0 7d571ffa 19d081a0 fb3f0000 00000000 }W.......?......
+  0x00010de0 376aff88 3347ac8e f83f0000 00000000 7j..3G...?......
+  0x00010df0 46214c5d 17df2dcf cf3f0000 00000000 F!L]..-..?......
+  0x00010e00 9dbe69e1 a12dd18c d83f0000 00000000 ..i..-...?......
+  0x00010e10 578cd9c9 6cdfb6a0 df3f0000 00000000 W...l....?......
+  0x00010e20 3162ca5f 129866c8 e53f0000 00000000 1b._..f..?......
+  0x00010e30 d4df156d f5cad694 eb3f0000 00000000 ...m.....?......
+  0x00010e40 7eed6e39 d340c186 f03f0000 00000000 ~.n9.@...?......
+  0x00010e50 eda763c9 0bff4292 f43f0000 00000000 ..c...B..?......
+  0x00010e60 fc3fd518 8dd8aab3 f73f0000 00000000 .?.......?......
+  0x00010e70 577895a5 a6e97ddc f93f0000 00000000 Wx....}..?......
+  0x00010e80 3189aefd ff3680c6 fa3f0000 00000000 1....6...?......
+  0x00010e90 0f65cf71 1caf3887 e4bf0000 00000000 .e.q..8.........
+  0x00010ea0 f52a7d1c c7f0edb9 e73f0000 00000000 .*}......?......
+  0x00010eb0 cdafee38 4e2bb4b5 ea3f0000 00000000 ...8N+...?......
+  0x00010ec0 49360b00 043906b7 ee3f0000 00000000 I6...9...?......
+  0x00010ed0 2029b3aa 8e9fa78a ee3f0000 00000000  ).......?......
+  0x00010ee0 7ef60b20 43c847c3 f33f0000 00000000 ~.. C.G..?......
+  0x00010ef0 bfa19c76 53221cd5 f53f0000 00000000 ...vS"...?......
+  0x00010f00 5c745f3a 25f753bb f43f0000 00000000 \t_:%.S..?......
+  0x00010f10 2a312043 96e2d6c1 f93f0000 00000000 *1 C.....?......
+  0x00010f20 70c53856 36a5da98 fb3f0000 00000000 p.8V6....?......
+  0x00010f30 9587e023 1397f2a8 fb3f0000 00000000 ...#.....?......
+  0x00010f40 3df6cdc3 89d79edb fb3f0000 00000000 =........?......
+  0x00010f50 59942d93 819fca8b fe3f0000 00000000 Y.-......?......
+  0x00010f60 7b58d8a7 02990190 ff3f0000 00000000 {X.......?......
+  0x00010f70 b63d3f3e 76a90bda fe3f0000 00000000 .=?>v....?......
+  0x00010f80 560de24b 09568ce0 fd3f0000 00000000 V..K.V...?......
+  0x00010f90 9f485019 b607ce97 fc3f0000 00000000 .HP......?......
+  0x00010fa0 a2cdefb2 59bb26f4 f93f0000 00000000 ....Y.&..?......
+  0x00010fb0 bb4f513c 418890b1 f63f0000 00000000 .OQ<A....?......
+  0x00010fc0 0355e75f ba851488 d43f0000 00000000 .U._.....?......
+  0x00010fd0 91775e5a c9e5fbb8 dc3f0000 00000000 .w^Z.....?......
+  0x00010fe0 993ac202 e9361fd3 e33f0000 00000000 .:...6...?......
+  0x00010ff0 a031f18d 56c0a083 ea3f0000 00000000 .1..V....?......
+  0x00011000 55f51c05 539f85c3 ef3f0000 00000000 U...S....?......
+  0x00011010 8d8e4580 403705b1 f43f0000 00000000 ..E.@7...?......
+  0x00011020 d8b2d54f f0e122c0 f83f0000 00000000 ...O.."..?......
+  0x00011030 7af68768 adfe04ec fb3f0000 00000000 z..h.....?......
+  0x00011040 800b8ec5 0b01d390 fe3f0000 00000000 .........?......
+  0x00011050 498071c4 38496182 ff3f0000 00000000 I.q.8Ia..?......
+  0x00011060 61d76a87 4a6078f9 db3f0000 00000000 a.j.J`x..?......
+  0x00011070 9dc6a294 2e3ceb9b de3f0000 00000000 .....<...?......
+  0x00011080 18d15f0c c07263d6 e33f0000 00000000 .._..rc..?......
+  0x00011090 e4f8607c 9981dd8a e63f0000 00000000 ..`|.....?......
+  0x000110a0 daa03788 330a5e8e ea3f0000 00000000 ..7.3.^..?......
+  0x000110b0 dc77f821 1e866cc3 ec3f0000 00000000 .w.!..l..?......
+  0x000110c0 f03c3771 90233fb4 ef3f0000 00000000 .<7q.#?..?......
+  0x000110d0 fa66485e 57067789 f23f0000 00000000 .fH^W.w..?......
+  0x000110e0 aa545627 67b5f8d0 f33f0000 00000000 .TV'g....?......
+  0x000110f0 68f138c8 c88485c9 f63f0000 00000000 h.8......?......
+  0x00011100 a6b00023 b83286f5 f53f0000 00000000 ...#.2...?......
+  0x00011110 c2b0bff0 82316491 fa3f0000 00000000 .....1d..?......
+  0x00011120 0e6e33fa 0230b484 fa3f0000 00000000 .n3..0...?......
+  0x00011130 d61a5242 c8d114a3 fc3f0000 00000000 ..RB.....?......
+  0x00011140 d64b3646 716679ad fd3f0000 00000000 .K6Fqfy..?......
+  0x00011150 4b36b437 bcdf09c0 fa3f0000 00000000 K6.7.....?......
+  0x00011160 237444e6 29fa3fce fe3f0000 00000000 #tD.).?..?......
+  0x00011170 7c7137c3 ba003886 fe3f0000 00000000 |q7...8..?......
+  0x00011180 2c4ff2d1 2a01c0d6 fb3f0000 00000000 ,O..*....?......
+  0x00011190 3b07c493 2df1f381 cd3f0000 00000000 ;...-....?......
+  0x000111a0 d579def4 d99ba7b0 d53f0000 00000000 .y.......?......
+  0x000111b0 e864fc21 f1a29dc9 dc3f0000 00000000 .d.!.....?......
+  0x000111c0 94e3abf1 97fb66fb e23f0000 00000000 ......f..?......
+  0x000111d0 2e86bc6c 07ddb7ba e83f0000 00000000 ...l.....?......
+  0x000111e0 b7964c0b f7b80ca9 ed3f0000 00000000 ..L......?......
+  0x000111f0 c30661cd 73267cb7 f13f0000 00000000 ..a.s&|..?......
+  0x00011200 d1e59c06 e26c64e1 f43f0000 00000000 .....ld..?......
+  0x00011210 e2f90af2 c6a14d8a f73f0000 00000000 ......M..?......
+  0x00011220 79cb7059 3dd204f9 f73f0000 00000000 y.pY=....?......
+  0x00011230 77d7faa8 daf076cc ebbf0000 00000000 w.....v.........
+  0x00011240 66321afe f5ce05e6 ee3f0000 00000000 f2.......?......
+  0x00011250 55f803d4 2aecbc9f f03f0000 00000000 U...*....?......
+  0x00011260 b0d07796 be05b2b9 f43f0000 00000000 ..w......?......
+  0x00011270 dbea7077 2f8e44ba f53f0000 00000000 ..pw/.D..?......
+  0x00011280 5662d276 d6ccb082 f83f0000 00000000 Vb.v.....?......
+  0x00011290 16519281 df4ecaaa fa3f0000 00000000 .Q...N...?......
+  0x000112a0 10df65ec 493c62d5 fa3f0000 00000000 ..e.I<b..?......
+  0x000112b0 ac6091ce 5677beee fb3f0000 00000000 .`..Vw...?......
+  0x000112c0 429ca51a 885e568c fe3f0000 00000000 B....^V..?......
+  0x000112d0 faa790ac 684a8c8a ff3f0000 00000000 ....hJ...?......
+  0x000112e0 7cf88b03 a1e65dbf fe3f0000 00000000 |.....]..?......
+  0x000112f0 9266544a ea1190a6 fd3f0000 00000000 .fTJ.....?......
+  0x00011300 ba8ce1fc cb1f73a7 fb3f0000 00000000 ......s..?......
+  0x00011310 c227738b 431cd894 f83f0000 00000000 .'s.C....?......
+  0x00011320 5fbb8e14 1630c694 db3f0000 00000000 _....0...?......
+  0x00011330 295d9a04 4350f2eb e23f0000 00000000 )]..CP...?......
+  0x00011340 64bba11b 22a14693 e93f0000 00000000 d...".F..?......
+  0x00011350 142aeb35 3a0b4ab9 ee3f0000 00000000 .*.5:.J..?......
+  0x00011360 5013cc02 7d7ad2f9 f23f0000 00000000 P...}z...?......
+  0x00011370 d04d68a5 15e8f2b0 f63f0000 00000000 .Mh......?......
+  0x00011380 cdfe24bf 3b149bed f83f0000 00000000 ..$.;....?......
+  0x00011390 8f0e461e 248540e1 f93f0000 00000000 ..F.$.@..?......
+  0x000113a0 758ec59d 17621d97 ee3f0000 00000000 u....b...?......
+  0x000113b0 e1a3ef78 e066c8cf f13f0000 00000000 ...x.f...?......
+  0x000113c0 28c62675 0c70f793 f23f0000 00000000 (.&u.p...?......
+  0x000113d0 9de4a006 9063009e f63f0000 00000000 .....c...?......
+  0x000113e0 6b6188ea 018f04e9 f83f0000 00000000 ka.......?......
+  0x000113f0 fd9065d5 58e35aee f93f0000 00000000 ..e.X.Z..?......
+  0x00011400 22959f13 1946fbd8 f83f0000 00000000 "....F...?......
+  0x00011410 5b9b7f1d 29777ede fc3f0000 00000000 [...)w~..?......
+  0x00011420 1b1079e7 82d30198 fe3f0000 00000000 ..y......?......
+  0x00011430 975b5911 24fa22f1 fe3f0000 00000000 .[Y.$."..?......
+  0x00011440 d9ba7e26 ccce8abc fe3f0000 00000000 ..~&.....?......
+  0x00011450 c0102520 aa6a88bf fd3f0000 00000000 ..% .j...?......
+  0x00011460 0dd63e83 27f0a780 fc3f0000 00000000 ..>.'....?......
+  0x00011470 d0697bad df186ece f93f0000 00000000 .i{...n..?......
+  0x00011480 ddef1321 74862196 f63f0000 00000000 ...!t.!..?......
+  0x00011490 f99ee6d7 dedc07d6 de3f0000 00000000 .........?......
+  0x000114a0 0fe033b5 243cb8a9 e63f0000 00000000 ..3.$<...?......
+  0x000114b0 67006269 9910e0d3 ec3f0000 00000000 g.bi.....?......
+  0x000114c0 acfb9a48 d4f94785 f23f0000 00000000 ...H..G..?......
+  0x000114d0 d502e893 725bb3b3 f63f0000 00000000 ....r[...?......
+  0x000114e0 4331c9ca 7c4890fe f93f0000 00000000 C1..|H...?......
+  0x000114f0 b5ad022f 56c6e9aa fc3f0000 00000000 .../V....?......
+  0x00011500 9455c8f0 cbe606a2 fd3f0000 00000000 .U.......?......
+  0x00011510 ec822f3f 2dd03aa5 e93f0000 00000000 ../?-.:..?......
+  0x00011520 8e924997 27769390 ec3f0000 00000000 ..I.'v...?......
+  0x00011530 e0c4328a ece4a5a2 ef3f0000 00000000 ..2......?......
+  0x00011540 e8d0bede d80576b2 f23f0000 00000000 ......v..?......
+  0x00011550 9d520cd4 43447ada f23f0000 00000000 .R..CDz..?......
+  0x00011560 f6d34d33 a036698c f73f0000 00000000 ..M3.6i..?......
+  0x00011570 6d17c7b1 876813d9 f73f0000 00000000 m....h...?......
+  0x00011580 8707aa9f 909531fc f93f0000 00000000 ......1..?......
+  0x00011590 182b7705 6a8389e6 fb3f0000 00000000 .+w.j....?......
+  0x000115a0 f790cd15 03065bdd fa3f0000 00000000 ......[..?......
+  0x000115b0 b0a59a9b 246756b7 fd3f0000 00000000 ....$gV..?......
+  0x000115c0 e4568d48 58936fe3 fe3f0000 00000000 .V.HX.o..?......
+  0x000115d0 9ace23d3 7b1a2ca0 fe3f0000 00000000 ..#.{.,..?......
+  0x000115e0 8da97eb1 582e4dd8 fc3f0000 00000000 ..~.X.M..?......
+  0x000115f0 0f54b581 aea233f7 f93f0000 00000000 .T....3..?......
+  0x00011600 d8c7e7d1 0eacbbc4 d93f0000 00000000 .........?......
+  0x00011610 78cb72c0 6fd1009c e13f0000 00000000 x.r.o....?......
+  0x00011620 499eb23b 3778c0c2 e73f0000 00000000 I..;7x...?......
+  0x00011630 556a9406 78e804f5 ec3f0000 00000000 Uj..x....?......
+  0x00011640 26db3e04 83702da5 f13f0000 00000000 &.>..p-..?......
+  0x00011650 8f0f3c31 9e7cfde9 f43f0000 00000000 ..<1.|...?......
+  0x00011660 0dca8a1b 29aa199d f73f0000 00000000 ....)....?......
+  0x00011670 516b161e a2a4ee94 f83f0000 00000000 Qk.......?......
+  0x00011680 3336992d 4cb625d0 e2bf0000 00000000 36.-L.%.........
+  0x00011690 4355595f 54ed198f e63f0000 00000000 CUY_T....?......
+  0x000116a0 6af0a22e 7b56d98b e93f0000 00000000 j...{V...?......
+  0x000116b0 eeefdb0d 9f85dd8c ed3f0000 00000000 .........?......
+  0x000116c0 39e11b69 df4aeb87 ec3f0000 00000000 9..i.J...?......
+  0x000116d0 326f8558 bcef9ea3 f23f0000 00000000 2o.X.....?......
+  0x000116e0 a7c76712 c4e08f9b f43f0000 00000000 ..g......?......
+  0x000116f0 8df98094 7c3c2e95 f53f0000 00000000 ....|<...?......
+  0x00011700 33bcad3c c3f854ce f83f0000 00000000 3..<..T..?......
+  0x00011710 54fbbfd2 2a9842ea f93f0000 00000000 T...*.B..?......
+  0x00011720 26acd24d 5a5419e8 f83f0000 00000000 &..MZT...?......
+  0x00011730 113debc7 9527d8e9 fc3f0000 00000000 .=...'...?......
+  0x00011740 753ff640 94aec5a0 fe3f0000 00000000 u?.@.....?......
+  0x00011750 5e91d1ff 9e222d88 ff3f0000 00000000 ^...."-..?......
+  0x00011760 20d9aa6a 2baad1c8 fe3f0000 00000000  ..j+....?......
+  0x00011770 d529f15c d25f21cc fd3f0000 00000000 .).\._!..?......
+  0x00011780 b2759fa1 afb02889 fc3f0000 00000000 .u....(..?......
+  0x00011790 cb8b310b fbf718dc f93f0000 00000000 ..1......?......
+  0x000117a0 4ef1c693 b62812a0 f63f0000 00000000 N....(...?......
+  0x000117b0 0439eada 05fb89c4 cf3f0000 00000000 .9.......?......
+  0x000117c0 c032cbfa 9dc89585 d83f0000 00000000 .2.......?......
+  0x000117d0 566dbf9c ffe07598 df3f0000 00000000 Vm....u..?......
+  0x000117e0 5ab6cfaa 95d21bbe e53f0000 00000000 Z........?......
+  0x000117f0 4f86c251 05ee318d eb3f0000 00000000 O..Q..1..?......
+  0x00011800 1e98d8cd 861fabff ef3f0000 00000000 .........?......
+  0x00011810 a560f18a ca04c08a f43f0000 00000000 .`.......?......
+  0x00011820 35a03178 bfaa70aa f73f0000 00000000 5.1x..p..?......
+  0x00011830 36175479 51fe2ad1 f93f0000 00000000 6.TyQ.*..?......
+  0x00011840 30d2066e 306c4ebc fa3f0000 00000000 0..n0lN..?......
+  0x00011850 5083d440 16b5cebd e53f0000 00000000 P..@.....?......
+  0x00011860 b1aaac14 22f3379a e93f0000 00000000 ....".7..?......
+  0x00011870 ba13ef08 b98b88d5 ea3f0000 00000000 .........?......
+  0x00011880 5f35b8fd 806db0dd ef3f0000 00000000 _5...m...?......
+  0x00011890 ec48362c 71ae71d2 f13f0000 00000000 .H6,q.q..?......
+  0x000118a0 7a2cc428 96b0bdb8 f33f0000 00000000 z,.(.....?......
+  0x000118b0 5d09707b 7037bbfe f63f0000 00000000 ].p{p7...?......
+  0x000118c0 2de5a5ce ab7ab7c0 f83f0000 00000000 -....z...?......
+  0x000118d0 732bab27 d63ac3a6 f73f0000 00000000 s+.'.:...?......
+  0x000118e0 839a6775 0647f29d fb3f0000 00000000 ..gu.G...?......
+  0x000118f0 47931acb 50aa9e9c fd3f0000 00000000 G...P....?......
+  0x00011900 3b63484d 3b0a29a8 fe3f0000 00000000 ;cHM;.)..?......
+  0x00011910 579c5f8c 08d15ef4 fe3f0000 00000000 W._...^..?......
+  0x00011920 51ab0fd1 ca051ec5 fe3f0000 00000000 Q........?......
+  0x00011930 c0993734 1c9956de fd3f0000 00000000 ..74..V..?......
+  0x00011940 457c05f2 89e55db3 fc3f0000 00000000 E|....]..?......
+  0x00011950 e2171bc7 aeac82c4 fa3f0000 00000000 .........?......
+  0x00011960 3e97972a 0df13983 f83f0000 00000000 >..*..9..?......
+  0x00011970 127f7f6f c16382a1 f43f0000 00000000 ...o.c...?......
+  0x00011980 14937222 251ee9c3 d33f0000 00000000 ..r"%....?......
+  0x00011990 f7df693d 7d722885 dc3f0000 00000000 ..i=}r(..?......
+  0x000119a0 e3cc6662 e817f997 e33f0000 00000000 ..fb.....?......
+  0x000119b0 0e1dcbf5 0c3980bd e93f0000 00000000 .....9...?......
+  0x000119c0 4f283ee4 605dbe8c ef3f0000 00000000 O(>.`]...?......
+  0x000119d0 83317aab 3bddd9fe f33f0000 00000000 .1z.;....?......
+  0x000119e0 c26a2b76 71744e8a f83f0000 00000000 .j+vqtN..?......
+  0x000119f0 488c748e 602ae5a9 fb3f0000 00000000 H.t.`*...?......
+  0x00011a00 1b4d9683 4acb7fd0 fd3f0000 00000000 .M..J....?......
+  0x00011a10 5888d902 4d4cb4bb fe3f0000 00000000 X...ML...?......
+  0x00011a20 7388fed2 7a4cdd88 e03f0000 00000000 s...zL...?......
+  0x00011a30 81595e2d 0af6f899 e33f0000 00000000 .Y^-.....?......
+  0x00011a40 7723c99b aa2f918e e73f0000 00000000 w#.../...?......
+  0x00011a50 e1efb5b8 8c3377c0 ea3f0000 00000000 .....3w..?......
+  0x00011a60 8b3c5c9d b48fa499 ec3f0000 00000000 .<\......?......
+  0x00011a70 f26e3c9f a5e430a9 f03f0000 00000000 .n<...0..?......
+  0x00011a80 a6da906e e03bb0fb ef3f0000 00000000 ...n.;...?......
+  0x00011a90 f9132f94 303215ee f43f0000 00000000 ../.02...?......
+  0x00011aa0 588a3f2b 333bb0ba f63f0000 00000000 X.?+3;...?......
+  0x00011ab0 0894069e d0c0a89e f73f0000 00000000 .........?......
+  0x00011ac0 bc2ce368 a3c3aea3 fa3f0000 00000000 .,.h.....?......
+  0x00011ad0 ad34e1e1 f334c2f9 fa3f0000 00000000 .4...4...?......
+  0x00011ae0 f42dcba8 4cb839ab fb3f0000 00000000 .-..L.9..?......
+  0x00011af0 e04dc99c 33b834f7 fd3f0000 00000000 .M..3.4..?......
+  0x00011b00 222e5da1 423686e9 fe3f0000 00000000 ".].B6...?......
+  0x00011b10 badf379a f39bc2b1 fe3f0000 00000000 ..7......?......
+  0x00011b20 60a04d7f 17ee139b fd3f0000 00000000 `.M......?......
+  0x00011b30 63d5640a 3dec069c fb3f0000 00000000 c.d.=....?......
+  0x00011b40 ca84925e fdd1b08a f83f0000 00000000 ...^.....?......
+  0x00011b50 38e98658 a4e00ab1 cd3f0000 00000000 8..X.....?......
+  0x00011b60 08655768 5fc9aaf0 d53f0000 00000000 .eWh_....?......
+  0x00011b70 6e37c4bc 1e265689 dd3f0000 00000000 n7...&V..?......
+  0x00011b80 bdae02ee 580440ab e33f0000 00000000 ....X.@..?......
+  0x00011b90 ff4a47bd ed9160fe e83f0000 00000000 .JG...`..?......
+  0x00011ba0 0bd41bd4 c16d4ee6 ed3f0000 00000000 .....mN..?......
+  0x00011bb0 c743ee8e 76edf8f9 f13f0000 00000000 .C..v....?......
+  0x00011bc0 537f4afc 2b588899 f53f0000 00000000 S.J.+X...?......
+  0x00011bd0 7189ec52 a62d6bbc f73f0000 00000000 q..R.-k..?......
+  0x00011be0 b522f0a1 3163a0a9 f83f0000 00000000 ."..1c...?......
+  0x00011bf0 d79d47ab 8b3aee85 f0bf0000 00000000 ..G..:..........
+  0x00011c00 7e6054f6 221fa3d9 f33f0000 00000000 ~`T."....?......
+  0x00011c10 050bcc83 f13beff6 f53f0000 00000000 .....;...?......
+  0x00011c20 5e48bf38 5a573aa3 f53f0000 00000000 ^H.8ZW:..?......
+  0x00011c30 f4c8153b b460a2c8 f93f0000 00000000 ...;.`...?......
+  0x00011c40 1e927948 e6219987 fc3f0000 00000000 ..yH.!...?......
+  0x00011c50 08bb20ec 82b00bc2 fd3f0000 00000000 .. ......?......
+  0x00011c60 e7ce9d3b 77eedcb9 fe3f0000 00000000 ...;w....?......
+  0x00011c70 096825a0 95805682 ff3f0000 00000000 .h%...V..?......
+  0x00011c80 16d7585c 63718dc5 fe3f0000 00000000 ..X\cq...?......
+  0x00011c90 e81c70b9 d742d3dc fd3f0000 00000000 ..p..B...?......
+  0x00011ca0 96b89ff9 db5a41b1 fc3f0000 00000000 .....ZA..?......
+  0x00011cb0 09547880 2cccb3c1 fa3f0000 00000000 .Tx.,....?......
+  0x00011cc0 4b1942c2 7cda3881 f83f0000 00000000 K.B.|.8..?......
+  0x00011cd0 700b65db 85e50a9f f43f0000 00000000 p.e......?......
+  0x00011ce0 6598d4ee e215e0da df3f0000 00000000 e........?......
+  0x00011cf0 d89462f3 5ab18fad e73f0000 00000000 ..b.Z....?......
+  0x00011d00 4cdcc481 2accabd8 ed3f0000 00000000 L...*....?......
+  0x00011d10 05959c0e 7f494c88 f33f0000 00000000 .....IL..?......
+  0x00011d20 0414d13b 93a6c4b7 f73f0000 00000000 ...;.....?......
+  0x00011d30 6aac46e1 5cb02982 fb3f0000 00000000 j.F.\.)..?......
+  0x00011d40 2deedbb1 0726c8ae fd3f0000 00000000 -....&...?......
+  0x00011d50 b80fd691 81c8b1a5 fe3f0000 00000000 .........?......
+  0x00011d60 9ca6aaa4 ac2d43b7 ed3f0000 00000000 .....-C..?......
+  0x00011d70 17a56a62 cd5efcfb f03f0000 00000000 ..jb.^...?......
+  0x00011d80 24c391b6 63c771b3 f13f0000 00000000 $...c.q..?......
+  0x00011d90 3418812d 6c3d9dbf f53f0000 00000000 4..-l=...?......
+  0x00011da0 0825d4a9 b89aabfe f73f0000 00000000 .%.......?......
+  0x00011db0 72599772 500c8287 f83f0000 00000000 rY.rP....?......
+  0x00011dc0 78a73ac1 ebc2d5e0 fa3f0000 00000000 x.:......?......
+  0x00011dd0 ea52fd55 d55d6f8b fd3f0000 00000000 .R.U.]o..?......
+  0x00011de0 b38010c3 b19226a4 fe3f0000 00000000 ......&..?......
+  0x00011df0 88df72f7 3bc1fcf6 fe3f0000 00000000 ..r.;....?......
+  0x00011e00 190b1f90 a3ec4dba fe3f0000 00000000 ......M..?......
+  0x00011e10 642df6c3 502a1ebc fd3f0000 00000000 d-..P*...?......
+  0x00011e20 c1371d19 da3bfffb fb3f0000 00000000 .7...;...?......
+  0x00011e30 f9770a9a 4f17f3c9 f93f0000 00000000 .w..O....?......
+  0x00011e40 876e4d87 c556df92 f63f0000 00000000 .nM..V...?......
+  0x00011e50 2b9e4f92 7c7c979d dc3f0000 00000000 +.O.||...?......
+  0x00011e60 d9440a90 6d3feef9 e33f0000 00000000 .D..m?...?......
+  0x00011e70 e86826a1 ef31019c ea3f0000 00000000 .h&..1...?......
+  0x00011e80 0235f440 605f45c4 ef3f0000 00000000 .5.@`_E..?......
+  0x00011e90 b92f8b82 b4785084 f43f0000 00000000 ./...xP..?......
+  0x00011ea0 836321dc 8ab06fbb f73f0000 00000000 .c!...o..?......
+  0x00011eb0 7a6014d4 3730b0fb f93f0000 00000000 z`..70...?......
+  0x00011ec0 b1cda1b7 b9309aee fa3f0000 00000000 .....0...?......
+  0x00011ed0 f241ef55 a6d476a6 e7bf0000 00000000 .A.U..v.........
+  0x00011ee0 d34d90f0 5b670f9c eb3f0000 00000000 .M..[g...?......
+  0x00011ef0 073ad9ee d77266ad eb3f0000 00000000 .:...rf..?......
+  0x00011f00 87c60252 abf56d8d f13f0000 00000000 ...R..m..?......
+  0x00011f10 9e796e12 b29b1681 f43f0000 00000000 .yn......?......
+  0x00011f20 16794d2f c166808c f53f0000 00000000 .yM/.f...?......
+  0x00011f30 24e8e796 140b97f3 f63f0000 00000000 $........?......
+  0x00011f40 1312f0b2 f7d2cc8e fa3f0000 00000000 .........?......
+  0x00011f50 7808738f 77202786 fc3f0000 00000000 x.s.w '..?......
+  0x00011f60 258351ba 2a543fa3 fd3f0000 00000000 %.Q.*T?..?......
+  0x00011f70 2ded3620 8b15748f fe3f0000 00000000 -.6 ..t..?......
+  0x00011f80 1adab088 a8bd1ebe fe3f0000 00000000 .........?......
+  0x00011f90 c172ac78 357f9cc1 fe3f0000 00000000 .r.x5....?......
+  0x00011fa0 f6f19cca 407a4898 fe3f0000 00000000 ....@zH..?......
+  0x00011fb0 5aaba930 919103b8 fd3f0000 00000000 Z..0.....?......
+  0x00011fc0 8f324156 3ab4ffa7 fc3f0000 00000000 .2AV:....?......
+  0x00011fd0 b8cba1ef df2c8fe0 fa3f0000 00000000 .....,...?......
+  0x00011fe0 1e3418fe 5fc78fcf f83f0000 00000000 .4.._....?......
+  0x00011ff0 06218628 316d57ed f53f0000 00000000 .!.(1mW..?......
+  0x00012000 f6de5b4d 120e2afd f13f0000 00000000 ..[M..*..?......
+  0x00012010 4ee0d7c6 01810cf8 e43f0000 00000000 N........?......
+  0x00012020 3f668f71 d1288ac9 e83f0000 00000000 ?f.q.(...?......
+  0x00012030 2c6ed9ff 9008878b ea3f0000 00000000 ,n.......?......
+  0x00012040 7d119f89 564ddb90 ef3f0000 00000000 }...VM...?......
+  0x00012050 482044a5 e2edd882 f13f0000 00000000 H D......?......
+  0x00012060 0f76b747 d5175d8e f33f0000 00000000 .v.G..]..?......
+  0x00012070 14e338d6 3b8c5ca9 f63f0000 00000000 ..8.;.\..?......
+  0x00012080 b8fa1a6b af2805c3 f73f0000 00000000 ...k.(...?......
+  0x00012090 8c588ad7 ff7e1aa8 f83f0000 00000000 .X...~...?......
+  0x000120a0 de991b2b 7535e8d5 fb3f0000 00000000 ...+u5...?......
+  0x000120b0 58d209b7 c11af8ad fd3f0000 00000000 X........?......
+  0x000120c0 0588b30e a79976af fe3f0000 00000000 ......v..?......
+  0x000120d0 31d1455e 7491eff7 fe3f0000 00000000 1.E^t....?......
+  0x000120e0 75122a5f bf178cc3 fe3f0000 00000000 u.*_.....?......
+  0x000120f0 374502e8 893493db fd3f0000 00000000 7E...4...?......
+  0x00012100 d697e043 4264b2b0 fc3f0000 00000000 ...CBd...?......
+  0x00012110 0e3b9d87 4d3257c1 fa3f0000 00000000 .;..M2W..?......
+  0x00012120 e266f6c5 a2b60b81 f83f0000 00000000 .f.......?......
+  0x00012130 b4b991b8 ef56d39e f43f0000 00000000 .....V...?......
+  0x00012140 67d49312 a507eba6 d13f0000 00000000 g........?......
+  0x00012150 bcf44065 647ee7e2 d93f0000 00000000 ..@ed~...?......
+  0x00012160 e6381727 a0957b81 e13f0000 00000000 .8.'..{..?......
+  0x00012170 d84aa9fa f8f774a1 e73f0000 00000000 .J....t..?......
+  0x00012180 6e17aa2c cc90d4ef ec3f0000 00000000 n..,.....?......
+  0x00012190 3bdc1210 7bd022d9 f13f0000 00000000 ;...{."..?......
+  0x000121a0 cd4226ba ab68adeb f53f0000 00000000 .B&..h...?......
+  0x000121b0 83dfea38 a6acc090 f93f0000 00000000 ...8.....?......
+  0x000121c0 628f03b7 76c9a4b1 fb3f0000 00000000 b...v....?......
+  0x000121d0 f0f72fde 811bed9f fc3f0000 00000000 ../......?......
+  0x000121e0 73c3e904 0629a2ae eb3f0000 00000000 s....)...?......
+  0x000121f0 aa5f3865 964b8cb9 ef3f0000 00000000 ._8e.K...?......
+  0x00012200 aa5f3865 964b8cb9 f23f0000 00000000 ._8e.K...?......
+  0x00012210 947786fe 7b5eefe7 f43f0000 00000000 .w..{^...?......
+  0x00012220 a2a8b57e ac72f1ca f63f0000 00000000 ...~.r...?......
+  0x00012230 0314f6eb bcbde983 f83f0000 00000000 .........?......
+  0x00012240 0314f6eb bcbde983 f93f0000 00000000 .........?......
+  0x00012250 e0fa1405 72bc4acf f93f0000 00000000 ....r.J..?......
+  0x00012260 cc1c2d43 c7b58e81 fa3f0000 00000000 ..-C.....?......
+  0x00012270 f0c405df 44999885 da3f0000 00000000 ....D....?......
+  0x00012280 7a666a67 084a3594 e23f0000 00000000 zfjg.J5..?......
+  0x00012290 2914fdf1 e5f62985 e93f0000 00000000 ).....)..?......
+  0x000122a0 e402faa1 069b92fa ee3f0000 00000000 .........?......
+  0x000122b0 573f19bb fa3a5585 f43f0000 00000000 W?...:U..?......
+  0x000122c0 2e454454 a5f7d2a1 f83f0000 00000000 .EDT.....?......
+  0x000122d0 1d6e900d 0b4370d6 fb3f0000 00000000 .n...Cp..?......
+  0x000122e0 6aabe1cb d0372e8a fe3f0000 00000000 j....7...?......
+  0x000122f0 29c04c36 fb7812bb ebbf0000 00000000 ).L6.x..........
+  0x00012300 29c04c36 fb7812bb ec3f0000 00000000 ).L6.x...?......
+  0x00012310 b2f0c033 805e88e2 f23f0000 00000000 ...3.^...?......
+  0x00012320 328a2d2a 7283fee3 f33f0000 00000000 2.-*r....?......
+  0x00012330 d01965e6 4d3fa3a2 f83f0000 00000000 ..e.M?...?......
+  0x00012340 f9cf0daf 5b3933a6 f93f0000 00000000 ....[93..?......
+  0x00012350 431e4bf2 3e2e9c91 fc3f0000 00000000 C.K.>....?......
+  0x00012360 43fb3bad d461ff9b fd3f0000 00000000 C.;..a...?......
+  0x00012370 5f0262a9 154f00b2 fd3f0000 00000000 _.b..O...?......
+  0x00012380 8caa2200 a047d096 e43f0000 00000000 .."..G...?......
+  0x00012390 90ca1d80 8dfd9a81 ec3f0000 00000000 .........?......
+  0x000123a0 e1a12218 8e93aa96 f23f0000 00000000 .."......?......
+  0x000123b0 f85920a9 574fbe8c f73f0000 00000000 .Y .WO...?......
+  0x000123c0 03982c02 23cd00c2 fa3f0000 00000000 ..,.#....?......
+  0x000123d0 e5771ea0 f30e8d84 fc3f0000 00000000 .w.......?......
+  0x000123e0 78827bfc 3f1b19b4 ee3f0000 00000000 x.{.?....?......
+  0x000123f0 78827bfc 3f1b19b4 f03f0000 00000000 x.{.?....?......
+  0x00012400 1a2d017d 34615d99 f53f0000 00000000 .-.}4a]..?......
+  0x00012410 3300defc 445c66a0 f73f0000 00000000 3...D\f..?......
+  0x00012420 aca0a2e0 4f888af0 f93f0000 00000000 ....O....?......
+  0x00012430 3e1fd387 d9488291 fc3f0000 00000000 >....H...?......
+  0x00012440 d25b170b 470954fb f93f0000 00000000 .[..G.T..?......
+  0x00012450 428a11a7 acd05bda fe3f0000 00000000 B.....[..?......
+  0x00012460 4831e294 157a4bbb ff3f0000 00000000 H1...zK..?......
+  0x00012470 641ba706 839b96c1 e43f0000 00000000 d........?......
+  0x00012480 8a9bb799 a46d5da6 ec3f0000 00000000 .....m]..?......
+  0x00012490 9d71e525 dc3566c1 f23f0000 00000000 .q.%.5f..?......
+  0x000124a0 e862edbe 1075a9b4 f73f0000 00000000 .b...u...?......
+  0x000124b0 6cd67efc eb0c07f9 fa3f0000 00000000 l.~......?......
+  0x000124c0 13dfd828 ae5e25aa fc3f0000 00000000 ...(.^%..?......
+  0x000124d0 a3099de3 5a1502c8 f0bf0000 00000000 ....Z...........
+  0x000124e0 3ac7b52a 04900196 f33f0000 00000000 :..*.....?......
+  0x000124f0 6b0ae803 77a18cbc f63f0000 00000000 k...w....?......
+  0x00012500 21800cb0 04c2c1a8 f93f0000 00000000 !........?......
+  0x00012510 dfa2135d e7c21689 f63f0000 00000000 ...].....?......
+  0x00012520 461dfaca 1d2c8bf0 fc3f0000 00000000 F....,...?......
+  0x00012530 91651666 48265bb6 fe3f0000 00000000 .e.fH&[..?......
+  0x00012540 f6621ca5 eafd37c3 fe3f0000 00000000 .b....7..?......
+  0x00012550 0c8324b1 6d22e99c fd3f0000 00000000 ..$.m"...?......
+  0x00012560 10048641 92d836d1 fa3f0000 00000000 ...A..6..?......
+  0x00012570 080e78f8 48e50cb1 e53f0000 00000000 ..x.H....?......
+  0x00012580 0f2c87b5 0a152798 ed3f0000 00000000 .,....'..?......
+  0x00012590 05f039a6 0fa2e0b0 f33f0000 00000000 ..9......?......
+  0x000125a0 d9c920a1 d9703aa5 f83f0000 00000000 .. ..p:..?......
+  0x000125b0 8def1f6e b2e6c0e3 fb3f0000 00000000 ...n.....?......
+  0x000125c0 55846122 85559c9b fd3f0000 00000000 U.a".U...?......
+  0x000125d0 684b3026 b62f02c7 e83f0000 00000000 hK0&./...?......
+  0x000125e0 cd80d188 00e105ab f03f0000 00000000 .........?......
+  0x000125f0 55bfa638 2a6fd0c6 f63f0000 00000000 U..8*o...?......
+  0x00012600 df819394 5662b8b9 fb3f0000 00000000 ....Vb...?......
+  0x00012610 46729017 efebe8ae 00400000 00000000 Fr.......@......
+  0x00012620 0ab36fb1 cc9f4ded f33f0000 00000000 ..o...M..?......
+  0x00012630 0ab36fb1 cc9f4ded f63f0000 00000000 ..o...M..?......
+  0x00012640 b6d4ce23 e3a97b85 f73f0000 00000000 ...#..{..?......
+  0x00012650 dab758e6 cfc578de fb3f0000 00000000 ..X...x..?......
+  0x00012660 66df6299 3fbadcdf fd3f0000 00000000 f.b.?....?......
+  0x00012670 3ef4a97e 4d6998e9 fe3f0000 00000000 >..~Mi...?......
+  0x00012680 ddfd7be8 932d6e94 ff3f0000 00000000 ..{..-n..?......
+  0x00012690 7092d24a 0c3b28ef fe3f0000 00000000 p..J.;(..?......
+  0x000126a0 37a65724 4435daef fd3f0000 00000000 7.W$D5...?......
+  0x000126b0 82939456 62e03089 fc3f0000 00000000 ...Vb.0..?......
+  0x000126c0 82939456 62e03089 f93f0000 00000000 ...Vb.0..?......
+  0x000126d0 d0e5eedf 439f36b5 f2bf0000 00000000 ....C.6.........
+  0x000126e0 449fead7 144784e2 f53f0000 00000000 D....G...?......
+  0x000126f0 2cf3e772 f7cfd4fe f73f0000 00000000 ,..r.....?......
+  0x00012700 73f7efa1 4f35e3a9 f93f0000 00000000 s...O5...?......
+  0x00012710 85f8b1ad a5cea694 fa3f0000 00000000 .........?......
+  0x00012720 392a6fd0 c6c461b2 fa3f0000 00000000 9*o...a..?......
+  0x00012730 d0e5eedf 439f36b5 f23f0000 00000000 ....C.6..?......
+  0x00012740 079379e7 b9b4e0d1 e93f0000 00000000 ..y......?......
+  0x00012750 3e30555c 59c199a2 f13f0000 00000000 >0U\Y....?......
+  0x00012760 0ac15005 d5c0b5a4 f73f0000 00000000 ..P......?......
+  0x00012770 5d1576eb f16d41fd fb3f0000 00000000 ].v..mA..?......
+  0x00012780 6c2959b5 cae8e1b3 ff3f0000 00000000 l)Y......?......
+  0x00012790 1c2ef465 9ea51fe5 e63f0000 00000000 ...e.....?......
+  0x000127a0 a0d79d1f 5432e7c4 ee3f0000 00000000 ....T2...?......
+  0x000127b0 10b15afe b45de6e4 f43f0000 00000000 ..Z..]...?......
+  0x000127c0 2868555a a710d3d5 f93f0000 00000000 (hUZ.....?......
+  0x000127d0 c8554329 dea25e93 fd3f0000 00000000 .UC)..^..?......
+  0x000127e0 869c9b37 90d060c9 fe3f0000 00000000 ...7..`..?......
+  0x000127f0 7fd4011b d52d19b7 e0bf0000 00000000 .....-..........
+  0x00012800 5f5f41d4 5fe25289 e23f0000 00000000 __A._.R..?......
+  0x00012810 cebaf0ef 4d36b58b e83f0000 00000000 ....M6...?......
+  0x00012820 871f553c 2c366cd4 e93f0000 00000000 ..U<,6l..?......
+  0x00012830 af5e7c84 21f61ba3 ee3f0000 00000000 .^|.!....?......
+  0x00012840 0baaaebd 4f9987fd ef3f0000 00000000 ....O....?......
+  0x00012850 33953040 58df74b6 f33f0000 00000000 3.0@X.t..?......
+  0x00012860 21a7ffa9 c5ca7393 f53f0000 00000000 !.....s..?......
+  0x00012870 ba94d48d d23868c8 f73f0000 00000000 .....8h..?......
+  0x00012880 8d9c3e99 250d1aaf f93f0000 00000000 ..>.%....?......
+  0x00012890 6e47336e 37274cbe fa3f0000 00000000 nG3n7'L..?......
+  0x000128a0 a14baf17 91a01fca fc3f0000 00000000 .K.......?......
+  0x000128b0 725fd8ff f4915b93 fb3f0000 00000000 r_....[..?......
+  0x000128c0 0d68d13a b54cf5c2 fe3f0000 00000000 .h.:.L...?......
+  0x000128d0 7f36b021 3eac2cfe fd3f0000 00000000 .6.!>.,..?......
+  0x000128e0 79daf0dd 837131b9 fe3f0000 00000000 y....q1..?......
+  0x000128f0 455d80cf cc289c93 d53f0000 00000000 E]...(...?......
+  0x00012900 79673236 433dc1a3 dd3f0000 00000000 yg26C=...?......
+  0x00012910 f886e405 7beb2193 e43f0000 00000000 ....{.!..?......
+  0x00012920 a8bf3ba3 18b76d8a ea3f0000 00000000 ..;...m..?......
+  0x00012930 56cd8283 6ab95193 ef3f0000 00000000 V...j.Q..?......
+  0x00012940 6596044c 878eccb2 f33f0000 00000000 e..L.....?......
+  0x00012950 d285e4b2 77bfeeec f63f0000 00000000 ....w....?......
+  0x00012960 8cd82ac2 77e3ac98 f93f0000 00000000 ..*.w....?......
+  0x00012970 94980e44 d5486d8d fa3f0000 00000000 ...D.Hm..?......
+  0x00012980 e99e0ba1 5dd279b9 e33f0000 00000000 ....].y..?......
+  0x00012990 a4864e09 f546d8e7 e53f0000 00000000 ..N..F...?......
+  0x000129a0 ac29461c 62780ce2 ea3f0000 00000000 .)F.bx...?......
+  0x000129b0 414ef6f9 748d8694 ed3f0000 00000000 AN..t....?......
+  0x000129c0 400dd471 afeb03c3 f03f0000 00000000 @..q.....?......
+  0x000129d0 9b8cde4a a2d79b8c f33f0000 00000000 ...J.....?......
+  0x000129e0 6bbd836d 45770088 f53f0000 00000000 k..mEw...?......
+  0x000129f0 eda1a373 a515f3f1 f73f0000 00000000 ...s.....?......
+  0x00012a00 fefe9f6b f94fbdbb f73f0000 00000000 ...k.O...?......
+  0x00012a10 0d9143cb 2959fcb9 fb3f0000 00000000 ..C.)Y...?......
+  0x00012a20 06bc6b10 19dc86af fb3f0000 00000000 ..k......?......
+  0x00012a30 d8fa3587 10bad9c5 fd3f0000 00000000 ..5......?......
+  0x00012a40 b99e1efa 3b0f05ee fe3f0000 00000000 ....;....?......
+  0x00012a50 07066f2c a8a76cc0 fd3f0000 00000000 ..o,..l..?......
+  0x00012a60 c4aa86c6 4eed3ebd ff3f0000 00000000 ....N.>..?......
+  0x00012a70 76552878 a2a88ecc fe3f0000 00000000 vU(x.....?......
+  0x00012a80 2b11ed2c b553a5a3 fc3f0000 00000000 +..,.S...?......
+  0x00012a90 51f7f945 ede113ba d63f0000 00000000 Q..E.....?......
+  0x00012aa0 5e4ea139 a30e6ece de3f0000 00000000 ^N.9..n..?......
+  0x00012ab0 50047c2d 76c979b9 e53f0000 00000000 P.|-v.y..?......
+  0x00012ac0 25d56aa3 94e780ae eb3f0000 00000000 %.j......?......
+  0x00012ad0 1df13315 a50cb6b9 f03f0000 00000000 ..3......?......
+  0x00012ae0 1060591e 840a65e1 f43f0000 00000000 .`Y...e..?......
+  0x00012af0 01a9fbe8 7eca5695 f83f0000 00000000 ....~.V..?......
+  0x00012b00 14e5328e 328b76c0 fa3f0000 00000000 ..2.2.v..?......
+  0x00012b10 71ff2d2a 4c8148b2 fb3f0000 00000000 q.-*L.H..?......
+  0x00012b20 77be96b1 a379d7e0 e5bf0000 00000000 w....y..........
+  0x00012b30 a8e6633b 6f8abcc4 e83f0000 00000000 ..c;o....?......
+  0x00012b40 a2412aca 55e83fc8 ec3f0000 00000000 .A*.U.?..?......
+  0x00012b50 437651f8 987ccfc7 ef3f0000 00000000 CvQ..|...?......
+  0x00012b60 86be13e1 774755c1 f13f0000 00000000 ....wGU..?......
+  0x00012b70 c5166657 3a49b087 f53f0000 00000000 ..fW:I...?......
+  0x00012b80 7397e716 2ff9d6ec f13f0000 00000000 s.../....?......
+  0x00012b90 67ed0a90 7b8be08a f93f0000 00000000 g...{....?......
+  0x00012ba0 779d0fed 90efc89e fa3f0000 00000000 w........?......
+  0x00012bb0 5708bca4 87c118df fa3f0000 00000000 W........?......
+  0x00012bc0 a57c5ede 0325f6b1 fd3f0000 00000000 .|^..%...?......
+  0x00012bd0 cedf8117 cb9e6185 fe3f0000 00000000 ......a..?......
+  0x00012be0 0a4d38b2 657bbccd fb3f0000 00000000 .M8.e{...?......
+  0x00012bf0 ed48c55c 78efaeac fe3f0000 00000000 .H.\x....?......
+  0x00012c00 546ddf76 0354d5ac fe3f0000 00000000 Tm.v.T...?......
+  0x00012c10 53ff0610 065375ee fc3f0000 00000000 S....Su..?......
+  0x00012c20 c24896e4 de0a4388 fa3f0000 00000000 .H....C..?......
+  0x00012c30 146eacb7 b84d21b3 d83f0000 00000000 .n...M!..?......
+  0x00012c40 1e4ac3eb 38f2b8c6 e03f0000 00000000 .J..8....?......
+  0x00012c50 4953b45a 24f68cb2 e73f0000 00000000 IS.Z$....?......
+  0x00012c60 cbbb7ac1 4af4fca7 ed3f0000 00000000 ..z.J....?......
+  0x00012c70 26fda136 52f9c6b2 f23f0000 00000000 &..6R....?......
+  0x00012c80 1f5d4397 e5a8fad8 f63f0000 00000000 .]C......?......
+  0x00012c90 e5ca2d85 9c5ec38f fa3f0000 00000000 ..-..^...?......
+  0x00012ca0 344ed331 79ee46b9 fc3f0000 00000000 4N.1y.F..?......
+  0x00012cb0 2bc50b5a 6e6da0ab fd3f0000 00000000 +..Znm...?......
+  0x00012cc0 4a1b2080 5a4cd290 e63f0000 00000000 J. .ZL...?......
+  0x00012cd0 b41e24d0 e595eca2 e93f0000 00000000 ..$......?......
+  0x00012ce0 3bc82260 b7d2e39c ec3f0000 00000000 ;."`.....?......
+  0x00012cf0 0e2e36b8 d8e062f4 ef3f0000 00000000 ..6...b..?......
+  0x00012d00 292feb4f a86a0d89 ef3f0000 00000000 )/.O.j...?......
+  0x00012d10 2a6bd5bb 9dc5ffaf f43f0000 00000000 *k.......?......
+  0x00012d20 0852c303 e44161a1 f63f0000 00000000 .R...Aa..?......
+  0x00012d30 47e3424e 730ab9eb ef3f0000 00000000 G.BNs....?......
+  0x00012d40 457e8515 ddf3c9a1 f93f0000 00000000 E~.......?......
+  0x00012d50 ff5a4a4c 2e95ecdd fa3f0000 00000000 .ZJL.....?......
+  0x00012d60 72146802 558f06f9 fa3f0000 00000000 r.h.U....?......
+  0x00012d70 70ae43f3 df6ed0bd f53f0000 00000000 p.C..n...?......
+  0x00012d80 1ffaddbc 6819e3c7 fb3f0000 00000000 ....h....?......
+  0x00012d90 632a1043 f55ffe91 fc3f0000 00000000 c*.C._...?......
+  0x00012da0 9365a639 cfa0d7df fb3f0000 00000000 .e.9.....?......
+  0x00012db0 f81c2ad0 ded209cb fa3f0000 00000000 ..*......?......
+  0x00012dc0 a388206e 3bf9f2ce f83f0000 00000000 .. n;....?......
+  0x00012dd0 58b28e0c c36bf4b7 f53f0000 00000000 X....k...?......
+  0x00012de0 bf079b3e c611b9bd de3f0000 00000000 ...>.....?......
+  0x00012df0 057fbca8 1bb8efab e63f0000 00000000 .........?......
+  0x00012e00 09583794 2c653ff6 ec3f0000 00000000 .X7.,e?..?......
+  0x00012e10 36e051e5 03d742b2 f23f0000 00000000 6.Q...B..?......
+  0x00012e20 006661cc 248a1e8b f73f0000 00000000 .fa.$....?......
+  0x00012e30 29ff6c69 d8ad2be7 fa3f0000 00000000 ).li..+..?......
+  0x00012e40 3f260cdc e7ebe4bd fd3f0000 00000000 ?&.......?......
+  0x00012e50 48aceaa4 1788f4fb fe3f0000 00000000 H........?......
+  0x00012e60 8e8d6447 85f4d5c6 d63f0000 00000000 ..dG.....?......
+  0x00012e70 098d33db 435b95dc de3f0000 00000000 ..3.C[...?......
+  0x00012e80 496e05c9 564b31c6 e53f0000 00000000 In..VK1..?......
+  0x00012e90 cadda5d1 63d377ba eb3f0000 00000000 ....c.w..?......
+  0x00012ea0 8336ccb6 42b071c6 f03f0000 00000000 .6..B.q..?......
+  0x00012eb0 0de8c737 cc36d9f0 f43f0000 00000000 ...7.6...?......
+  0x00012ec0 1015ace5 0705949f f83f0000 00000000 .........?......
+  0x00012ed0 15f81799 b1b1a8cd fa3f0000 00000000 .........?......
+  0x00012ee0 88155aec 9fc481be fb3f0000 00000000 ..Z......?......
+  0x00012ef0 5ce9579e 2c5ae2c5 dcbf0000 00000000 \.W.,Z..........
+  0x00012f00 b3e3edc5 b7f05af7 de3f0000 00000000 ......Z..?......
+  0x00012f10 4c6e2225 22530bb2 e43f0000 00000000 Ln"%"S...?......
+  0x00012f20 fd789a6c 70ff48e6 e63f0000 00000000 .x.lp.H..?......
+  0x00012f30 179f5e16 8d1a18f3 ea3f0000 00000000 ..^......?......
+  0x00012f40 9b1ca611 514569a6 ed3f0000 00000000 ....QEi..?......
+  0x00012f50 4a93ac9e ab70dd9a f03f0000 00000000 J....p...?......
+  0x00012f60 1a9362d2 d392d1eb f23f0000 00000000 ..b......?......
+  0x00012f70 07c3ddaf 3bed7ab0 f43f0000 00000000 ....;.z..?......
+  0x00012f80 ac8f5646 849a1cab f73f0000 00000000 ..VF.....?......
+  0x00012f90 5de7c9e4 d5d50eb6 f63f0000 00000000 ]........?......
+  0x00012fa0 b063bce3 64cec0ee fa3f0000 00000000 .c..d....?......
+  0x00012fb0 04a9a215 9b00e2e8 fa3f0000 00000000 .........?......
+  0x00012fc0 1c713e83 993449fb fc3f0000 00000000 .q>..4I..?......
+  0x00012fd0 58d46bdb 99251d8f fe3f0000 00000000 X.k..%...?......
+  0x00012fe0 0069f74b a49c3afb fa3f0000 00000000 .i.K..:..?......
+  0x00012ff0 104756d9 d66545a7 ff3f0000 00000000 .GV..eE..?......
+  0x00013000 d4d8ab8f 4cbf16b1 fe3f0000 00000000 ....L....?......
+  0x00013010 76adbc3f 3dccab8d fc3f0000 00000000 v..?=....?......
+  0x00013020 7b1c4632 af9f9a92 cd3f0000 00000000 {.F2.....?......
+  0x00013030 b82a69cb 86efe7db d53f0000 00000000 .*i......?......
+  0x00013040 2d7f7176 647d9888 dd3f0000 00000000 -.qvd}...?......
+  0x00013050 4dda05ae de0ce8b6 e33f0000 00000000 M........?......
+  0x00013060 38c9463c 3c34fd8f e93f0000 00000000 8.F<<4...?......
+  0x00013070 be3e29d8 919e8188 ee3f0000 00000000 .>)......?......
+  0x00013080 8cf57042 092f7199 f23f0000 00000000 ..pB./q..?......
+  0x00013090 ca82344a 6cba51c1 f53f0000 00000000 ..4Jl.Q..?......
+  0x000130a0 8f3ddcd7 74a251f1 f73f0000 00000000 .=..t.Q..?......
+  0x000130b0 7b00c494 a13679db f83f0000 00000000 {....6y..?......
+  0x000130c0 397d1d4d ac82bef5 de3f0000 00000000 9}.M.....?......
+  0x000130d0 92cd79c3 56b206d7 e13f0000 00000000 ..y.V....?......
+  0x000130e0 8ad985d2 63b2bfad e63f0000 00000000 ....c....?......
+  0x000130f0 31bb6cc4 3c2778a5 e93f0000 00000000 1.l.<'x..?......
+  0x00013100 51f55525 10da41a7 ec3f0000 00000000 Q.U%..A..?......
+  0x00013110 cd00d912 a3ed58bc ef3f0000 00000000 ......X..?......
+  0x00013120 609483bf 6572bdda f03f0000 00000000 `...er...?......
+  0x00013130 f52af413 b90ad5c1 f43f0000 00000000 .*.......?......
+  0x00013140 861beed6 983683b9 f33f0000 00000000 .....6...?......
+  0x00013150 a8591e5a cf56efab f83f0000 00000000 .Y.Z.V...?......
+  0x00013160 38653c37 c3b9e4c6 f93f0000 00000000 8e<7.....?......
+  0x00013170 cae34408 07f05f9c fa3f0000 00000000 ..D..._..?......
+  0x00013180 3a908f2c fb187de4 fc3f0000 00000000 :..,..}..?......
+  0x00013190 123fcf15 19cf618f fd3f0000 00000000 .?....a..?......
+  0x000131a0 52b95d0e 9d988b89 fc3f0000 00000000 R.]......?......
+  0x000131b0 be119c75 1648a3c8 fe3f0000 00000000 ...u.H...?......
+  0x000131c0 63c2f718 689160a6 fe3f0000 00000000 c...h.`..?......
+  0x000131d0 2e94b12b 76fe28e3 fc3f0000 00000000 ...+v.(..?......
+  0x000131e0 d19dae86 4348ce81 fa3f0000 00000000 ....CH...?......
+  0x000131f0 c2a9a4cd c88ab189 ce3f0000 00000000 .........?......
+  0x00013200 a3fe7634 2d508ace d63f0000 00000000 ..v4-P...?......
+  0x00013210 03ba4a54 f5214b80 de3f0000 00000000 ..JT.!K..?......
+  0x00013220 6a2ab6b8 1b1fcaab e43f0000 00000000 j*.......?......
+  0x00013230 700dec10 28cf3c87 ea3f0000 00000000 p...(.<..?......
+  0x00013240 526eafb1 fca63580 ef3f0000 00000000 Rn....5..?......
+  0x00013250 4268a76b 56b41d90 f33f0000 00000000 Bh.kV....?......
+  0x00013260 22e833ef 1ac891b5 f63f0000 00000000 ".3......?......
+  0x00013270 fd92d307 bcd6a6e2 f83f0000 00000000 .........?......
+  0x00013280 e84790c1 0f5222ce f93f0000 00000000 .G...R"..?......
+  0x00013290 57c8a836 37bb2aa0 e2bf0000 00000000 W..67.*.........
+  0x000132a0 62e17d1d 9e1230b4 e53f0000 00000000 b.}...0..?......
+  0x000132b0 e81916a5 ad106ba1 e93f0000 00000000 ......k..?......
+  0x000132c0 1a6c884a a47622db ec3f0000 00000000 .l.J.v"..?......
+  0x000132d0 40bf3cbe 2b002f92 ee3f0000 00000000 @.<.+./..?......
+  0x000132e0 8e0f725e d7998bb0 f23f0000 00000000 ..r^.....?......
+  0x000132f0 6065c138 8a13bdd6 f23f0000 00000000 `e.8.....?......
+  0x00013300 9bc46ad7 935219cc f63f0000 00000000 ..j..R...?......
+  0x00013310 e419887f ec4b95c0 f83f0000 00000000 .....K...?......
+  0x00013320 6f686694 2677daf0 f63f0000 00000000 ohf.&w...?......
+  0x00013330 f06b54f0 ab5da5df fb3f0000 00000000 .kT..]...?......
+  0x00013340 94290d99 9dfcfc88 fd3f0000 00000000 .).......?......
+  0x00013350 b8c48e3a c2e6d1ce fc3f0000 00000000 ...:.....?......
+  0x00013360 318a3c16 88b8c3a2 fd3f0000 00000000 1.<......?......
+  0x00013370 64cc25c4 040d7e9f ff3f0000 00000000 d.%...~..?......
+  0x00013380 22cc354b 12bf98e8 fe3f0000 00000000 ".5K.....?......
+  0x00013390 56425c79 3e1f00cf fd3f0000 00000000 VB\y>....?......
+  0x000133a0 519cdfa6 dbf0abd1 fb3f0000 00000000 Q........?......
+  0x000133b0 816e715b 8af25fba f83f0000 00000000 .nq[.._..?......
+  0x000133c0 3f743c8c 17afa4a1 d13f0000 00000000 ?t<......?......
+  0x000133d0 5eae5a52 a30677f2 d93f0000 00000000 ^.ZR..w..?......
+  0x000133e0 b79bb38a fbb69b96 e13f0000 00000000 .........?......
+  0x000133f0 c386c69d d178abc9 e73f0000 00000000 .....x...?......
+  0x00013400 e06642c2 9697c29e ed3f0000 00000000 .fB......?......
+  0x00013410 358424ba 8b7f8296 f23f0000 00000000 5.$......?......
+  0x00013420 a7fb8921 01d32ea9 f63f0000 00000000 ...!.....?......
+  0x00013430 df80366c 6c9b26d5 f93f0000 00000000 ..6ll.&..?......
+  0x00013440 e84f3266 f6870985 fc3f0000 00000000 .O2f.....?......
+  0x00013450 87bfffe9 fef1fcf1 fc3f0000 00000000 .........?......
+  0x00013460 ae9133d3 bddf859b d43f0000 00000000 ..3......?......
+  0x00013470 855acdbc 9ccf48e9 dc3f0000 00000000 .Z....H..?......
+  0x00013480 6e7eb697 15dee790 e43f0000 00000000 n~.......?......
+  0x00013490 465a470a 42af08c2 ea3f0000 00000000 FZG.B....?......
+  0x000134a0 6f3edcb1 91babf98 f03f0000 00000000 o>.......?......
+  0x000134b0 6987d362 129bcf90 f53f0000 00000000 i..b.....?......
+  0x000134c0 d7fd0b52 c9eec6a2 f93f0000 00000000 ...R.....?......
+  0x000134d0 c1038362 cc8814cd fc3f0000 00000000 ...b.....?......
+  0x000134e0 c5d7837a 4c5ad3e8 ff3f0000 00000000 ...zLZ...?......
+  0x000134f0 c950ccea af2267f3 e33f0000 00000000 .P..."g..?......
+  0x00013500 8a776cf1 d8e756a7 e73f0000 00000000 .wl...V..?......
+  0x00013510 eaa65a7e cfe4598d ea3f0000 00000000 ..Z~..Y..?......
+  0x00013520 1c385072 c2f57895 ee3f0000 00000000 .8Pr..x..?......
+  0x00013530 1b6ce209 a71b47df ee3f0000 00000000 .l....G..?......
+  0x00013540 2a68c453 b5c0abf5 f23f0000 00000000 *h.S.....?......
+  0x00013550 a9bf9242 06e3dd9d f53f0000 00000000 ...B.....?......
+  0x00013560 4fa484e2 be2493d9 f43f0000 00000000 O....$...?......
+  0x00013570 14c18951 4c2dfcaa f83f0000 00000000 ...QL-...?......
+  0x00013580 22ad9f9a 28a5f5a8 fa3f0000 00000000 "...(....?......
+  0x00013590 0fc3d033 b8a20f8a fb3f0000 00000000 ...3.....?......
+  0x000135a0 c36b4188 e2cfa3bf f93f0000 00000000 .kA......?......
+  0x000135b0 09656323 9bb9a8fe fb3f0000 00000000 .ec#.....?......
+  0x000135c0 06083645 e74f1898 fd3f0000 00000000 ..6E.O...?......
+  0x000135d0 097331f0 6cd8bbb9 fd3f0000 00000000 .s1.l....?......
+  0x000135e0 12cb323d 4064a891 fd3f0000 00000000 ..2=@d...?......
+  0x000135f0 3e860ec9 14328698 fc3f0000 00000000 >....2...?......
+  0x00013600 b2c274e3 76e5d0cf fa3f0000 00000000 ..t.v....?......
+  0x00013610 113a9476 fa8196a7 f83f0000 00000000 .:.v.....?......
+  0x00013620 a40ea966 c9a5c3f3 f43f0000 00000000 ...f.....?......
+  0x00013630 5b947a77 3496a2ff d93f0000 00000000 [.zw4....?......
+  0x00013640 44ef9b59 a7f0b9bf db3f0000 00000000 D..Y.....?......
+  0x00013650 43d1a362 43764d8a e23f0000 00000000 C..bCvM..?......
+  0x00013660 0dafe47c 917673d1 e33f0000 00000000 ...|.vs..?......
+  0x00013670 e5883a67 87ee5bed e83f0000 00000000 ..:g..[..?......
+  0x00013680 f59ef6b2 365a63b6 ea3f0000 00000000 ....6Zc..?......
+  0x00013690 653a4481 36b936ce ee3f0000 00000000 e:D.6.6..?......
+  0x000136a0 b780efe9 345748a2 f03f0000 00000000 ....4WH..?......
+  0x000136b0 e35f24ab 335059c0 f33f0000 00000000 ._$.3PY..?......
+  0x000136c0 87334749 e156dd9d f53f0000 00000000 .3GI.V...?......
+  0x000136d0 46774eda 7bebc5ba f73f0000 00000000 FwN.{....?......
+  0x000136e0 9ea1cb52 a68baca6 f93f0000 00000000 ...R.....?......
+  0x000136f0 fb0b7cda 79d7aea2 fa3f0000 00000000 ..|.y....?......
+  0x00013700 ddf116e4 9da6adb2 fc3f0000 00000000 .........?......
+  0x00013710 f64370a4 036afad3 fa3f0000 00000000 .Cp..j...?......
+  0x00013720 64813e7c 5f4396a3 fe3f0000 00000000 d.>|_C...?......
+  0x00013730 48b52c01 f4af77bb fd3f0000 00000000 H.,...w..?......
+  0x00013740 0270b138 909b4fc4 fe3f0000 00000000 .p.8..O..?......
+  0x00013750 7dbb1d9c e6f518a9 cd3f0000 00000000 }........?......
+  0x00013760 3c992cea d970a5fd d53f0000 00000000 <.,..p...?......
+  0x00013770 df5bd91b adb78d9d dd3f0000 00000000 .[.......?......
+  0x00013780 8445b918 df47f8d2 e33f0000 00000000 .E...G...?......
+  0x00013790 48b906c2 ded414a6 e93f0000 00000000 H........?......
+  0x000137a0 3f4dcac4 8b56739d ee3f0000 00000000 ?M...Vs..?......
+  0x000137b0 33a79161 0b1cfcb0 f23f0000 00000000 3..a.....?......
+  0x000137c0 da29262f 60f4fade f53f0000 00000000 .)&/`....?......
+  0x000137d0 f44b6218 71192c8b f83f0000 00000000 .Kb.q.,..?......
+  0x000137e0 fb5de815 fdba25fd f83f0000 00000000 .]....%..?......
+  0x000137f0 69bdcca5 1823598f e4bf0000 00000000 i....#Y.........
+  0x00013800 784b2622 6bfddbfa e63f0000 00000000 xK&"k....?......
+  0x00013810 64b154e7 83c656ff ea3f0000 00000000 d.T...V..?......
+  0x00013820 a6e4aece 606dc7fe ed3f0000 00000000 ....`m...?......
+  0x00013830 945e40a8 10c47f84 f03f0000 00000000 .^@......?......
+  0x00013840 5c4597e7 e2f019b5 f33f0000 00000000 \E.......?......
+  0x00013850 fca5e902 6ce8cfd8 f03f0000 00000000 ....l....?......
+  0x00013860 50f03034 4f1748cd f73f0000 00000000 P.04O.H..?......
+  0x00013870 e973152e b8d9b8c5 f83f0000 00000000 .s.......?......
+  0x00013880 75b30a5a 2ce8d98a fa3f0000 00000000 u..Z,....?......
+  0x00013890 3df0ed62 ed482f99 fc3f0000 00000000 =..b.H/..?......
+  0x000138a0 b61c2cb1 2055c783 fc3f0000 00000000 ..,. U...?......
+  0x000138b0 4f1c1044 e52fa591 fd3f0000 00000000 O..D./...?......
+  0x000138c0 d8d4a9af bbada1da fe3f0000 00000000 .........?......
+  0x000138d0 034c29cd c0a835a2 fe3f0000 00000000 .L)...5..?......
+  0x000138e0 05450867 51e7dddb fc3f0000 00000000 .E.gQ....?......
+  0x000138f0 e24ec075 38bf46fb f93f0000 00000000 .N.u8.F..?......
+  0x00013900 83db892b 53f5adaa d33f0000 00000000 ...+S....?......
+  0x00013910 85ef4c44 28fc58bd db3f0000 00000000 ..LD(.X..?......
+  0x00013920 59cda902 449d20aa e23f0000 00000000 Y...D. ..?......
+  0x00013930 3c7451e7 932b10a0 e83f0000 00000000 <tQ..+...?......
+  0x00013940 c1731ee9 d4e357aa ed3f0000 00000000 .s....W..?......
+  0x00013950 9972d289 9f36bece f13f0000 00000000 .r...6...?......
+  0x00013960 ebf9a544 2126fb88 f53f0000 00000000 ...D!&...?......
+  0x00013970 7287751d 735989b0 f73f0000 00000000 r.u.sY...?......
+  0x00013980 7d10a760 5cb387a3 f83f0000 00000000 }..`\....?......
+  0x00013990 90efbe34 0c0f8482 e73f0000 00000000 ...4.....?......
+  0x000139a0 82cd56bb ed90d492 ea3f0000 00000000 ..V......?......
+  0x000139b0 8783798e a265648d ed3f0000 00000000 ..y..ed..?......
+  0x000139c0 44340299 64d93edc f03f0000 00000000 D4..d.>..?......
+  0x000139d0 ef65877c 8487378b e63f0000 00000000 .e.|..7..?......
+  0x000139e0 e21ad34d 635950c1 f53f0000 00000000 ...McYP..?......
+  0x000139f0 c64283d0 78c21f8d f73f0000 00000000 .B..x....?......
+  0x00013a00 3794e4b7 a39ae987 f83f0000 00000000 7........?......
+  0x00013a10 c0e90686 b484148a fb3f0000 00000000 .........?......
+  0x00013a20 362da058 63450c83 fc3f0000 00000000 6-.XcE...?......
+  0x00013a30 858e53fb 6a816fdf f73f0000 00000000 ..S.j.o..?......
+  0x00013a40 7426a251 efe366f0 fd3f0000 00000000 t&.Q..f..?......
+  0x00013a50 6b01f602 a212a991 ff3f0000 00000000 k........?......
+  0x00013a60 1fe472d3 42335bcd fe3f0000 00000000 ..r.B3[..?......
+  0x00013a70 4a5bb467 0d6147b4 fd3f0000 00000000 J[.g.aG..?......
+  0x00013a80 cd36c43f 7100c5b5 fb3f0000 00000000 .6.?q....?......
+  0x00013a90 b6302055 0fab92a1 f83f0000 00000000 .0 U.....?......
+  0x00013aa0 d538b271 67d39fea d53f0000 00000000 .8.qg....?......
+  0x00013ab0 86db1061 43a72482 de3f0000 00000000 ...aC.$..?......
+  0x00013ac0 3e110860 0c87dde9 e43f0000 00000000 >..`.....?......
+  0x00013ad0 912c658f b1d207dc ea3f0000 00000000 .,e......?......
+  0x00013ae0 3a15b596 198329ea ef3f0000 00000000 :.....)..?......
+  0x00013af0 45616b1f fd76198e f43f0000 00000000 Eak..v...?......
+  0x00013b00 a07b7d61 36ff4cbc f73f0000 00000000 .{}a6.L..?......
+  0x00013b10 d1ef288f 14f6acf2 f93f0000 00000000 ..(......?......
+  0x00013b20 638283e9 7cddcbe0 fa3f0000 00000000 c...|....?......
+  0x00013b30 3e83356f fb26edee e9bf0000 00000000 >.5o.&..........
+  0x00013b40 3bca74dc cc0a43a4 ed3f0000 00000000 ;.t...C..?......
+  0x00013b50 3bca74dc cc0a43a4 ee3f0000 00000000 ;.t...C..?......
+  0x00013b60 e9239175 76f2209f f33f0000 00000000 .#.uv. ..?......
+  0x00013b70 e27c9ca2 8410618f f53f0000 00000000 .|....a..?......
+  0x00013b80 d95fa047 17784fd6 f53f0000 00000000 ._.G.xO..?......
+  0x00013b90 011c2dba 732695b3 f93f0000 00000000 ..-.s&...?......
+  0x00013ba0 7af6402a 0ccc8f83 fb3f0000 00000000 z.@*.....?......
+  0x00013bb0 8b877aa4 884b5285 fb3f0000 00000000 ..z..KR..?......
+  0x00013bc0 6e9bb55a 76bdacde fb3f0000 00000000 n..Zv....?......
+  0x00013bd0 ce9a7255 5f5900ff fd3f0000 00000000 ..rU_Y...?......
+  0x00013be0 c10d6dbc c54c2fe5 fe3f0000 00000000 ..m..L/..?......
+  0x00013bf0 4d2cc8d5 fcc828c1 fe3f0000 00000000 M,....(..?......
+  0x00013c00 e94ce641 7d3c97c6 fd3f0000 00000000 .L.A}<...?......
+  0x00013c10 6e10aaf3 25fd2686 fc3f0000 00000000 n...%.&..?......
+  0x00013c20 c86b80ca 87e1b2d7 f93f0000 00000000 .k.......?......
+  0x00013c30 d71f4693 a82fdf9c f63f0000 00000000 ..F../...?......
+  0x00013c40 71baa30a 309771f0 d93f0000 00000000 q...0.q..?......
+  0x00013c50 6bd1e6a5 dc015f85 e23f0000 00000000 k....._..?......
+  0x00013c60 dbeadad6 1e79aaef e83f0000 00000000 .....y...?......
+  0x00013c70 974f0841 72ec7ce1 ee3f0000 00000000 .O.Ar.|..?......
+  0x00013c80 f4a8a751 a457f8ef f33f0000 00000000 ...Q.W...?......
+  0x00013c90 0cd330a7 70bc9f91 f83f0000 00000000 ..0.p....?......
+  0x00013ca0 5517d425 78a0f8c0 fb3f0000 00000000 U..%x....?......
+  0x00013cb0 f1e8fdd8 32d9b1f8 fd3f0000 00000000 ....2....?......
+  0x00013cc0 ee02577f fd395fe6 fe3f0000 00000000 ..W..9_..?......
+  0x00013cd0 454d1fe7 16af4399 e23f0000 00000000 EM....C..?......
+  0x00013ce0 9620e7a0 dc9a94bf e43f0000 00000000 . .......?......
+  0x00013cf0 2c26aee9 637dcaba e93f0000 00000000 ,&..c}...?......
+  0x00013d00 c02128ae 6a6676f5 eb3f0000 00000000 .!(.jfv..?......
+  0x00013d10 d6ed27fe 696311a3 ef3f0000 00000000 ..'.ic...?......
+  0x00013d20 350b7c6d ae96c7ea f13f0000 00000000 5.|m.....?......
+  0x00013d30 7ba4b711 5e3d9ee9 f33f0000 00000000 {...^=...?......
+  0x00013d40 15e0e0ed 005610ce f63f0000 00000000 .....V...?......
+  0x00013d50 5af002e5 376e31b9 f63f0000 00000000 Z...7n1..?......
+  0x00013d60 312d096c 9aba32a6 fa3f0000 00000000 1-.l..2..?......
+  0x00013d70 b3e17d6a a36f6989 fa3f0000 00000000 ..}j.oi..?......
+  0x00013d80 9d6ba4a9 23d626c7 fc3f0000 00000000 .k..#.&..?......
+  0x00013d90 7f689ec8 aeab26cd fd3f0000 00000000 .h....&..?......
+  0x00013da0 66cdfe59 42385d9d fb3f0000 00000000 f..YB8]..?......
+  0x00013db0 b36c8ff7 f4a0889d ff3f0000 00000000 .l.......?......
+  0x00013dc0 e0477335 32c9eaa4 fe3f0000 00000000 .Gs52....?......
+  0x00013dd0 19d3f55d 5b07ef83 fc3f0000 00000000 ...][....?......
+  0x00013de0 6055f5e4 40f3ac9f d33f0000 00000000 `U..@....?......
+  0x00013df0 b62a00fe dbdd23b1 db3f0000 00000000 .*....#..?......
+  0x00013e00 35ba3773 07b8289f e23f0000 00000000 5.7s..(..?......
+  0x00013e10 588d7ffc ae61be95 e83f0000 00000000 X....a...?......
+  0x00013e20 82b0b005 4a6e5c9f ed3f0000 00000000 ....Jn\..?......
+  0x00013e30 1f4d2241 4afd69c1 f13f0000 00000000 .M"AJ.i..?......
+  0x00013e40 ba9f8181 a4522680 f53f0000 00000000 .....R&..?......
+  0x00013e50 b8d5aec9 6eac27a5 f73f0000 00000000 ....n.'..?......
+  0x00013e60 9ba1687e 13b1fc98 f83f0000 00000000 ..h~.....?......
+  0x00013e70 a4a3561c 240a61db e0bf0000 00000000 ..V.$.a.........
+  0x00013e80 1978e19f 682bcdf6 e33f0000 00000000 .x..h+...?......
+  0x00013e90 ec508f64 38cc17dd e73f0000 00000000 .P.d8....?......
+  0x00013ea0 b2c4e2f3 0fc21296 eb3f0000 00000000 .........?......
+  0x00013eb0 ed43be78 10e4f6dc ec3f0000 00000000 .C.x.....?......
+  0x00013ec0 120b9b07 02457afd f03f0000 00000000 .....Ez..?......
+  0x00013ed0 6608332c 00711bf1 f03f0000 00000000 f.3,.q...?......
+  0x00013ee0 84eb0005 709468a4 f53f0000 00000000 ....p.h..?......
+  0x00013ef0 9dc22ff7 7c45eb88 f73f0000 00000000 ../.|E...?......
+  0x00013f00 14b4c812 53dfa9ac f73f0000 00000000 ....S....?......
+  0x00013f10 bf9f4730 2f349bd7 fa3f0000 00000000 ..G0/4...?......
+  0x00013f20 a715f48e 6c364abf fb3f0000 00000000 ....l6J..?......
+  0x00013f30 a873fcd2 1c7c23d9 fa3f0000 00000000 .s...|#..?......
+  0x00013f40 ece0aad0 278f6480 fe3f0000 00000000 ....'.d..?......
+  0x00013f50 81fc5b0c a469d58e ff3f0000 00000000 ..[..i...?......
+  0x00013f60 b1315262 b7afd0c7 fe3f0000 00000000 .1Rb.....?......
+  0x00013f70 5b9b208c c382daae fd3f0000 00000000 [. ......?......
+  0x00013f80 3929e092 6a951bb0 fb3f0000 00000000 9)..j....?......
+  0x00013f90 f97955f4 ec4b8a9c f83f0000 00000000 .yU..K...?......
+  0x00013fa0 d5226dca b8e460f0 cc3f0000 00000000 ."m...`..?......
+  0x00013fb0 20dad197 8aab48b4 d53f0000 00000000  .....H..?......
+  0x00013fc0 836beb84 5be7f7df dc3f0000 00000000 .k..[....?......
+  0x00013fd0 7fdba7e3 f667f395 e33f0000 00000000 .....g...?......
+  0x00013fe0 e2e50d0e 694817ec e83f0000 00000000 ....iH...?......
+  0x00013ff0 6a07dd13 8767d2df ed3f0000 00000000 j....g...?......
+  0x00014000 5737c882 a73097fb f13f0000 00000000 W7...0...?......
+  0x00014010 9841b4c1 e4c97c9e f53f0000 00000000 .A....|..?......
+  0x00014020 50e5358d 94b0d6c5 f73f0000 00000000 P.5......?......
+  0x00014030 be14e8be c2e5edb3 f83f0000 00000000 .........?......
+  0x00014040 39655154 82cedcbc e33f0000 00000000 9eQT.....?......
+  0x00014050 97f5f799 f9cdd781 e73f0000 00000000 .........?......
+  0x00014060 9089ee09 da1f5bdb e93f0000 00000000 ......[..?......
+  0x00014070 11f80ee7 a186f5e7 ed3f0000 00000000 .........?......
+  0x00014080 74f8c5ad a49fe5db ed3f0000 00000000 t........?......
+  0x00014090 186f8bcb cad923ea f23f0000 00000000 .o....#..?......
+  0x000140a0 1008e762 9fdebcf8 f43f0000 00000000 ...b.....?......
+  0x000140b0 8e9c7a28 481215e1 f43f0000 00000000 ..z(H....?......
+  0x000140c0 7403f03a 29a2e081 f93f0000 00000000 t..:)....?......
+  0x000140d0 1331e2f7 f9095ab5 fa3f0000 00000000 .1....Z..?......
+  0x000140e0 bc40994a a7f8b7cc f93f0000 00000000 .@.J.....?......
+  0x000140f0 21ffd410 70dfb4a5 fc3f0000 00000000 !...p....?......
+  0x00014100 cc730db2 7cce378b fe3f0000 00000000 .s..|.7..?......
+  0x00014110 cfc5c751 11d1d4ea fe3f0000 00000000 ...Q.....?......
+  0x00014120 54ddc6c9 70cfffbe fe3f0000 00000000 T...p....?......
+  0x00014130 a31ac244 e6584bc3 fd3f0000 00000000 ...D.XK..?......
+  0x00014140 546c5a74 d4499683 fc3f0000 00000000 TlZt.I...?......
+  0x00014150 104a79e4 10b25fd3 f93f0000 00000000 .Jy..._..?......
+  0x00014160 af7b6fbd ddf5b999 f63f0000 00000000 .{o......?......
+  0x00014170 584c99c1 f1f434b4 cf3f0000 00000000 XL....4..?......
+  0x00014180 42f93251 b5b72787 d83f0000 00000000 B.2Q..'..?......
+  0x00014190 38db87f8 708fe7a7 df3f0000 00000000 8...p....?......
+  0x000141a0 51fa9adc b283d4e0 e53f0000 00000000 Q........?......
+  0x000141b0 c7b84d9b b919feb0 eb3f0000 00000000 ..M......?......
+  0x000141c0 075933ea a472cba7 f03f0000 00000000 .Y3..r...?......
+  0x000141d0 14b1e3b3 80c29cbc f43f0000 00000000 .........?......
+  0x000141e0 104f902a 2630a1ed f73f0000 00000000 .O.*&0...?......
+  0x000141f0 f4ceb5a2 efca5094 fa3f0000 00000000 ......P..?......
+  0x00014200 cf404725 d1aae386 fb3f0000 00000000 .@G%.....?......
+  0x00014210 a66719f1 988a01fa e6bf0000 00000000 .g..............
+  0x00014220 36a4e443 9c4021cb ea3f0000 00000000 6..C.@!..?......
+  0x00014230 107f1540 a1d1d084 eb3f0000 00000000 ...@.....?......
+  0x00014240 4ecb703d b2edb1e7 f03f0000 00000000 N.p=.....?......
+  0x00014250 0cd515c5 e714e486 f33f0000 00000000 .........?......
+  0x00014260 2ca6515b ade358e1 f23f0000 00000000 ,.Q[..X..?......
+  0x00014270 1f33e7bf 6d50dcbd f73f0000 00000000 .3..mP...?......
+  0x00014280 063bb0a7 f4033db4 f93f0000 00000000 .;....=..?......
+  0x00014290 77213fc6 f6a6a583 fa3f0000 00000000 w!?......?......
+  0x000142a0 504e9d14 af668b8a fa3f0000 00000000 PN...f...?......
+  0x000142b0 6ed0f54d e062a488 fd3f0000 00000000 n..M.b...?......
+  0x000142c0 e5140d23 60a141a7 fe3f0000 00000000 ...#`.A..?......
+  0x000142d0 ed16b229 e26c8c89 ff3f0000 00000000 ...).l...?......
+  0x000142e0 1ea9c622 7ffbbdd6 fe3f0000 00000000 ...".....?......
+  0x000142f0 f47cad0e 67b411f4 fd3f0000 00000000 .|..g....?......
+  0x00014300 848db08a db96b8c5 fc3f0000 00000000 .........?......
+  0x00014310 c61a7bbe 118e13d9 fa3f0000 00000000 ..{......?......
+  0x00014320 b702899b 88461491 f83f0000 00000000 .....F...?......
+  0x00014330 44c81ed3 bb1b8fb2 f43f0000 00000000 D........?......
+  0x00014340 671b2170 28467493 d43f0000 00000000 g.!p(Ft..?......
+  0x00014350 1aa931a8 3c692edd dc3f0000 00000000 ..1.<i...?......
+  0x00014360 ce786951 16486389 e43f0000 00000000 .xiQ.Hc..?......
+  0x00014370 1aa3ac98 7d98f7b7 ea3f0000 00000000 ....}....?......
+  0x00014380 52d5d918 e1f8d290 f03f0000 00000000 R........?......
+  0x00014390 f6dae78c 4f474c89 f53f0000 00000000 ....OGL..?......
+  0x000143a0 3e59aa34 6afc549a f93f0000 00000000 >Y.4j.T..?......
+  0x000143b0 079bf6a1 8bbb70c2 fc3f0000 00000000 ......p..?......
+  0x000143c0 af277a1a 5fe6b7f2 fe3f0000 00000000 .'z._....?......
+  0x000143d0 a7fe1f3a f60bbfdc ff3f0000 00000000 ...:.....?......
+  0x000143e0 0da28a08 76671c8b de3f0000 00000000 ....vg...?......
+  0x000143f0 969bf28e 0eb571f3 e03f0000 00000000 ......q..?......
+  0x00014400 260914e8 4c2ab6c4 e53f0000 00000000 &...L*...?......
+  0x00014410 bab10034 548056bb e83f0000 00000000 ...4T.V..?......
+  0x00014420 2b31f153 ef490dc0 eb3f0000 00000000 +1.S.I...?......
+  0x00014430 696d5e41 0ed697d7 ee3f0000 00000000 im^A.....?......
+  0x00014440 ef9b9734 6711e782 f03f0000 00000000 ...4g....?......
+  0x00014450 de567afc 96c4d1e2 f33f0000 00000000 .Vz......?......
+  0x00014460 954abd8a deb80fa3 f23f0000 00000000 .J.......?......
+  0x00014470 2b8b53cf aff085d4 f73f0000 00000000 +.S......?......
+  0x00014480 f304bbde f69b68e6 f83f0000 00000000 ......h..?......
+  0x00014490 effe281d a2c1f4eb f93f0000 00000000 ..(......?......
+  0x000144a0 eda145ce cb8da790 fc3f0000 00000000 ..E......?......
+  0x000144b0 7c297ce2 51e2ccf3 fb3f0000 00000000 |)|.Q....?......
+  0x000144c0 462c7259 c9687a95 fd3f0000 00000000 F,rY.hz..?......
+  0x000144d0 03366f84 f1aa70db fe3f0000 00000000 .6o...p..?......
+  0x000144e0 d01ffc55 770608a2 fe3f0000 00000000 ...Uw....?......
+  0x000144f0 ac3779d6 500b8edb fc3f0000 00000000 .7y.P....?......
+  0x00014500 7bf66587 a57aebfa f93f0000 00000000 {.e..z...?......
+  0x00014510 3835dbb8 5b1403d4 cb3f0000 00000000 85..[....?......
+  0x00014520 ea67a4ca 444f029f d43f0000 00000000 .g..DO...?......
+  0x00014530 388edeed 89d689c5 db3f0000 00000000 8........?......
+  0x00014540 cd477f69 a9674184 e23f0000 00000000 .G.i.gA..?......
+  0x00014550 cab96630 c5fe3ad0 e73f0000 00000000 ..f0..:..?......
+  0x00014560 779bbf89 8fc368c5 ec3f0000 00000000 w.....h..?......
+  0x00014570 fbcc5043 dfa8e6dd f03f0000 00000000 ..PC.....?......
+  0x00014580 f8857666 5ee5c88b f43f0000 00000000 ..vf^....?......
+  0x00014590 e4211711 5a007eae f63f0000 00000000 .!..Z.~..?......
+  0x000145a0 3ebbc256 b83fb29e f73f0000 00000000 >..V.?...?......
+  0x000145b0 29c3a66a 717282c2 e8bf0000 00000000 )..jqr..........
+  0x000145c0 2ca652f9 adaeb985 ec3f0000 00000000 ,.R......?......
+  0x000145d0 2ca652f9 adaeb985 ed3f0000 00000000 ,.R......?......
+  0x000145e0 fb108889 38e18b81 f23f0000 00000000 ....8....?......
+  0x000145f0 ba980f81 8b703bc5 f33f0000 00000000 .....p;..?......
+  0x00014600 2aceab10 0d17d5ba f53f0000 00000000 *........?......
+  0x00014610 d9bb9601 90a203bb f83f0000 00000000 .........?......
+  0x00014620 3ffc1f2d 0f45b4bd f93f0000 00000000 ?..-.E...?......
+  0x00014630 258f9f6a acae90b9 f93f0000 00000000 %..j.....?......
+  0x00014640 40951a6c 2a8ba8e9 fc3f0000 00000000 @..l*....?......
+  0x00014650 0f1b3c6e c40a3d9a fe3f0000 00000000 ..<n..=..?......
+  0x00014660 6a8ca1f1 92bf2af2 fe3f0000 00000000 j.....*..?......
+  0x00014670 2f799298 d08629bc fe3f0000 00000000 /y....)..?......
+  0x00014680 d3c04390 a4e7f4be fd3f0000 00000000 ..C......?......
+  0x00014690 0d108399 25773580 fc3f0000 00000000 ....%w5..?......
+  0x000146a0 6209d2e4 1043adcd f93f0000 00000000 b....C...?......
+  0x000146b0 8def5249 0c489595 f63f0000 00000000 ..RI.H...?......
+  0x000146c0 056ae6b2 2a6ca9b7 d53f0000 00000000 .j..*l...?......
+  0x000146d0 9d9d775e fff3bfcb dd3f0000 00000000 ..w^.....?......
+  0x000146e0 35438a1f dd5311b7 e43f0000 00000000 5C...S...?......
+  0x000146f0 4efa7df2 c4e93cac ea3f0000 00000000 N.}...<..?......
+  0x00014700 d14d9939 c1ce4cb7 ef3f0000 00000000 .M.9..L..?......
+  0x00014710 8b140e0b 88e777de f33f0000 00000000 ......w..?......
+  0x00014720 92bf4a36 1e706693 f73f0000 00000000 ..J6.pf..?......
+  0x00014730 904b60a0 5edcf6bd f93f0000 00000000 .K`.^....?......
+  0x00014740 39759e6b 81f3f7af fa3f0000 00000000 9u.k.....?......
+  0x00014750 84703972 55575bc4 eb3f0000 00000000 .p9rUW[..?......
+  0x00014760 6babce6c f5368a9f ef3f0000 00000000 k..l.6...?......
+  0x00014770 7442f2c3 6aeccfab f03f0000 00000000 tB..j....?......
+  0x00014780 fed534bf 16f0988b f43f0000 00000000 ..4......?......
+  0x00014790 068e2b85 c9a4cc83 f73f0000 00000000 ..+......?......
+  0x000147a0 f18779fd ae9c28b0 f83f0000 00000000 ..y...(..?......
+  0x000147b0 6babce6c f5368a9f f13f0000 00000000 k..l.6...?......
+  0x000147c0 a7d7341c 7598a9b9 fb3f0000 00000000 ..4.u....?......
+  0x000147d0 8a7592fd 212406aa fd3f0000 00000000 .u..!$...?......
+  0x000147e0 fd2f60bd a4fd20b2 fe3f0000 00000000 ./`... ..?......
+  0x000147f0 2643c8dd 24135185 ff3f0000 00000000 &C..$.Q..?......
+  0x00014800 2299710f 3feaa4cc fe3f0000 00000000 ".q.?....?......
+  0x00014810 713acace ed4068e6 fd3f0000 00000000 q:...@h..?......
+  0x00014820 99b56e66 373eb0b9 fc3f0000 00000000 ..nf7>...?......
+  0x00014830 db2a40a3 f7f554cb fa3f0000 00000000 .*@...T..?......
+  0x00014840 3286c0d5 c31bc187 f83f0000 00000000 2........?......
+  0x00014850 3ee0b1df 7a0e15a7 f43f0000 00000000 >...z....?......
+  0x00014860 039106bd b1a9abca d93f0000 00000000 .........?......
+  0x00014870 df48b32d 4170d6e0 e13f0000 00000000 .H.-Ap...?......
+  0x00014880 9307d635 89d303ca e83f0000 00000000 ...5.....?......
+  0x00014890 94457683 7f7810be ee3f0000 00000000 .Ev..x...?......
+  0x000148a0 6a1378cd 637645ca f33f0000 00000000 j.x.cvE..?......
+  0x000148b0 3620147b b0597ef5 f73f0000 00000000 6 .{.Y~..?......
+  0x000148c0 6d86ee7a dde6a7a2 fb3f0000 00000000 m..z.....?......
+  0x000148d0 dec96072 0117a0d1 fd3f0000 00000000 ..`r.....?......
+  0x000148e0 a3c5b451 985a2ec2 fe3f0000 00000000 ...Q.Z...?......
+  0x000148f0 577fff9f a5424594 e63f0000 00000000 W....BE..?......
+  0x00014900 416fff53 faeacda6 e93f0000 00000000 Ao.S.....?......
+  0x00014910 481faac2 885da0a0 ec3f0000 00000000 H....]...?......
+  0x00014920 e226ff7d 77e034fa ef3f0000 00000000 .&.}w.4..?......
+  0x00014930 2b2bccdd ecce43ba ed3f0000 00000000 ++....C..?......
+  0x00014940 6e9cdf84 885fc0e8 f43f0000 00000000 n...._...?......
+  0x00014950 147dfb3b e9709d9f f63f0000 00000000 .}.;.p...?......
+  0x00014960 1e2fb06c 7ffa61c9 f73f0000 00000000 ./.l..a..?......
+  0x00014970 460cc672 53ec86aa fa3f0000 00000000 F..rS....?......
+  0x00014980 67da6229 593c02ec fa3f0000 00000000 g.b)Y<...?......
+  0x00014990 173b1b60 73c37ed9 fb3f0000 00000000 .;.`s.~..?......
+  0x000149a0 326ff693 9afb418a fe3f0000 00000000 2o....A..?......
+  0x000149b0 76ca4b80 9dea528b ff3f0000 00000000 v.K...R..?......
+  0x000149c0 6185569e 8b95e7c0 fe3f0000 00000000 a.V......?......
+  0x000149d0 80490b10 0e4013a8 fd3f0000 00000000 .I...@...?......
+  0x000149e0 6aae5b19 69b607a9 fb3f0000 00000000 j.[.i....?......
+  0x000149f0 5ef06d4f 96be3f96 f83f0000 00000000 ^.mO..?..?......
+  0x00014a00 3b9ef20e 8506ccbf d33f0000 00000000 ;........?......
+  0x00014a10 8a27959c 3b57c6d4 db3f0000 00000000 .'..;W...?......
+  0x00014a20 503dc2a8 8f312dbf e23f0000 00000000 P=...1-..?......
+  0x00014a30 b1b9f6bd 20faddb3 e83f0000 00000000 .... ....?......
+  0x00014a40 d63d4b98 ea4e6bbf ed3f0000 00000000 .=K..Nk..?......
+  0x00014a50 da8ac412 508c52e8 f13f0000 00000000 ....P.R..?......
+  0x00014a60 d8e168f6 96dbed99 f53f0000 00000000 ..h......?......
+  0x00014a70 7fcc18a3 0aee60c6 f73f0000 00000000 ......`..?......
+  0x00014a80 096e097d 5c51c3b7 f83f0000 00000000 .n.}\Q...?......
+  0x00014a90 79b31a8d ac5002df e5bf0000 00000000 y....P..........
+  0x00014aa0 d2b1a532 8ce131b5 e93f0000 00000000 ...2..1..?......
+  0x00014ab0 b05eec55 b775f2ec e93f0000 00000000 .^.U.u...?......
+  0x00014ac0 d3fec4e9 43e5acce ef3f0000 00000000 ....C....?......
+  0x00014ad0 089f13f5 27f3e6d3 f13f0000 00000000 ....'....?......
+  0x00014ae0 0164292c da8dae8f f33f0000 00000000 .d),.....?......
+  0x00014af0 a24f667d 4b3899d9 f63f0000 00000000 .Of}K8...?......
+  0x00014b00 78b0efda eb300e9a f83f0000 00000000 x....0...?......
+  0x00014b10 45b02f7d 8d4927f2 f53f0000 00000000 E./}.I'..?......
+  0x00014b20 c9682162 5b1ee2bd fb3f0000 00000000 .h!b[....?......
+  0x00014b30 80d92717 c73bd9aa fd3f0000 00000000 ..'..;...?......
+  0x00014b40 73ebccd8 0f6354b2 fe3f0000 00000000 s....cT..?......
+  0x00014b50 30539a3e 08294385 ff3f0000 00000000 0S.>.)C..?......
+  0x00014b60 96bf0d1b 38da86cc fe3f0000 00000000 ....8....?......
+  0x00014b70 b42cb153 340642e6 fd3f0000 00000000 .,.S4.B..?......
+  0x00014b80 d0a8f612 29c08fb9 fc3f0000 00000000 ....)....?......
+  0x00014b90 b37aca46 688130cb fa3f0000 00000000 .z.Fh.0..?......
+  0x00014ba0 b441e360 678aa887 f83f0000 00000000 .A.`g....?......
+  0x00014bb0 a29fdc4f bad1f6a6 f43f0000 00000000 ...O.....?......
+  0x00014bc0 0c91391f 64316d90 d03f0000 00000000 ..9.d1m..?......
+  0x00014bd0 9259d62e 16caa3d8 d83f0000 00000000 .Y.......?......
+  0x00014be0 fbdc6fef 121d9186 e03f0000 00000000 ..o......?......
+  0x00014bf0 16b44787 479630b4 e63f0000 00000000 ..G.G.0..?......
+  0x00014c00 43efbe01 45b7d98d ec3f0000 00000000 C...E....?......
+  0x00014c10 724a260c 36957a86 f13f0000 00000000 rJ&.6.z..?......
+  0x00014c20 506f0177 9bc02997 f53f0000 00000000 Po.w..)..?......
+  0x00014c30 d56c1550 27ac72be f83f0000 00000000 .l.P'.r..?......
+  0x00014c40 4be980bc 0212bced fa3f0000 00000000 K........?......
+  0x00014c50 f4900677 30b636d8 fb3f0000 00000000 ...w0.6..?......
+  0x00014c60 a301c6ee 2eccc3c5 e83f0000 00000000 .........?......
+  0x00014c70 89a1d9ff 6b8f67b9 ec3f0000 00000000 ....k.g..?......
+  0x00014c80 1a096d88 2f8ddf84 ee3f0000 00000000 ..m./....?......
+  0x00014c90 85b2848a ed2579b7 f13f0000 00000000 .....%y..?......
+  0x00014ca0 36b0fdca 5fc697d6 f43f0000 00000000 6..._....?......
+  0x00014cb0 9847db5b 421c70b1 f63f0000 00000000 .G.[B.p..?......
+  0x00014cc0 771c594f 1199ae92 f53f0000 00000000 w.YO.....?......
+  0x00014cd0 5b3b497f 8820abd1 f93f0000 00000000 [;I.. ...?......
+  0x00014ce0 06d1780c cc9609f6 fb3f0000 00000000 ..x......?......
+  0x00014cf0 12e4098f 374936a1 fd3f0000 00000000 ....7I6..?......
+  0x00014d00 f65711bc 1601a292 fe3f0000 00000000 .W.......?......
+  0x00014d10 9d90955a 5d25f7c5 fe3f0000 00000000 ...Z]%...?......
+  0x00014d20 c24b298c ee69c6cb fe3f0000 00000000 .K)..i...?......
+  0x00014d30 c91a95e1 644c51a1 fe3f0000 00000000 ....dLQ..?......
+  0x00014d40 5d6b5136 136bb4c3 fd3f0000 00000000 ]kQ6.k...?......
+  0x00014d50 da6602ae 01591ab3 fc3f0000 00000000 .f...Y...?......
+  0x00014d60 03197f82 a036bdef fa3f0000 00000000 .....6...?......
+  0x00014d70 70f96f94 6118c2dd f83f0000 00000000 p.o.a....?......
+  0x00014d80 2ac60f52 ead8a6fd f53f0000 00000000 *..R.....?......
+  0x00014d90 e39c3ba3 27eb4787 f23f0000 00000000 ..;.'.G..?......
+  0x00014da0 2efd6b6f a0729df3 e23f0000 00000000 ..ko.r...?......
+  0x00014db0 0f3e9a4c ce3e7ca7 e63f0000 00000000 .>.L.>|..?......
+  0x00014dc0 b20b0ad6 3b6f798d e93f0000 00000000 ....;oy..?......
+  0x00014dd0 6f1b179b 19509a95 ed3f0000 00000000 o....P...?......
+  0x00014de0 47f0f76a 84bd36e5 ec3f0000 00000000 G..j..6..?......
+  0x00014df0 b90450f6 55725da0 f23f0000 00000000 ..P.Ur]..?......
+  0x00014e00 426d214e 8a59c5a1 f43f0000 00000000 Bm!N.Y...?......
+  0x00014e10 7e9f84a4 5028e9df f43f0000 00000000 ~...P(...?......
+  0x00014e20 eb1a3e7e 5bbbe4b9 f83f0000 00000000 ..>~[....?......
+  0x00014e30 1d9865a7 0691b1d5 f93f0000 00000000 ..e......?......
+  0x00014e40 c649e4b8 e5d0d7e9 f83f0000 00000000 .I.......?......
+  0x00014e50 2dfdae90 315cb2dc fc3f0000 00000000 -...1\...?......
+  0x00014e60 520187c4 a6514497 fe3f0000 00000000 R....QD..?......
+  0x00014e70 e79b2cf1 3d5eb0f0 fe3f0000 00000000 ..,.=^...?......
+  0x00014e80 827a4e38 b100bebc fe3f0000 00000000 .zN8.....?......
+  0x00014e90 64eed518 3b78d8bf fd3f0000 00000000 d...;x...?......
+  0x00014ea0 be1d1085 81e1e680 fc3f0000 00000000 .........?......
+  0x00014eb0 13e2cd1a d28cd8ce f93f0000 00000000 .........?......
+  0x00014ec0 5447c42a 0df26e96 f63f0000 00000000 TG.*..n..?......
+  0x00014ed0 7aa38db4 26c191b9 cd3f0000 00000000 z...&....?......
+  0x00014ee0 9b3a6a07 dd502d8b d63f0000 00000000 .:j..P-..?......
+  0x00014ef0 1f301e16 dda3e6ac dd3f0000 00000000 .0.......?......
+  0x00014f00 e3475202 6a3f85e7 e33f0000 00000000 .GR.j?...?......
+  0x00014f10 b27f3cd6 7e6942b6 e93f0000 00000000 ..<.~iB..?......
+  0x00014f20 113f8d8e e8b0c9ac ee3f0000 00000000 .?.......?......
+  0x00014f30 b36ba661 ed9639c2 f23f0000 00000000 .k.a..9..?......
+  0x00014f40 f7a9f9bf 3b6db3f4 f53f0000 00000000 ....;m...?......
+  0x00014f50 faa9497d 5da5ba98 f83f0000 00000000 ..I}]....?......
+  0x00014f60 9a963c44 923de78a f93f0000 00000000 ..<D.=...?......
+  0x00014f70 6a47bb8c 33efe7b8 ecbf0000 00000000 jG..3...........
+  0x00014f80 f492ef53 407059ad f03f0000 00000000 ...S@pY..?......
+  0x00014f90 036261f9 28000fe9 f23f0000 00000000 .ba.(....?......
+  0x00014fa0 37aef33e 30140382 f33f0000 00000000 7..>0....?......
+  0x00014fb0 7ea30b68 7a88e1d6 f63f0000 00000000 ~..hz....?......
+  0x00014fc0 47e00cf6 9e461fb6 f93f0000 00000000 G....F...?......
+  0x00014fd0 87ea13bd 298c2f9f fb3f0000 00000000 ....)./..?......
+  0x00014fe0 9815a33c 9be503bc fc3f0000 00000000 ...<.....?......
+  0x00014ff0 30bf209c 5c39bba2 fd3f0000 00000000 0. .\9...?......
+  0x00015000 d13c8aaf 4249d6d5 fd3f0000 00000000 .<..BI...?......
+  0x00015010 1b851b00 294ca9d8 fd3f0000 00000000 ....)L...?......
+  0x00015020 b0519743 0e3ae2a9 fd3f0000 00000000 .Q.C.:...?......
+  0x00015030 507cced4 722fe3cc fc3f0000 00000000 P|..r/...?......
+  0x00015040 cd4b77aa e6fad5ba fb3f0000 00000000 .Kw......?......
+  0x00015050 74af8163 7edf90f9 f93f0000 00000000 t..c~....?......
+  0x00015060 cf8c4009 0d3d97e6 f73f0000 00000000 ..@..=...?......
+  0x00015070 6982d33f 0658d183 f53f0000 00000000 i..?.X...?......
+  0x00015080 4ebe0333 8f089b8c f13f0000 00000000 N..3.....?......
+  0x00015090 70bc5549 1beefcfc ea3f0000 00000000 p.UI.....?......
+  0x000150a0 1ba9952b 76818dcd ee3f0000 00000000 ...+v....?......
+  0x000150b0 e2042be0 57505ddd ef3f0000 00000000 ..+.WP]..?......
+  0x000150c0 f8f32266 47d1dbb3 f33f0000 00000000 .."fG....?......
+  0x000150d0 1d5cdeae 0830399c f63f0000 00000000 .\...09..?......
+  0x000150e0 64f1ba5e fc1ba48a f73f0000 00000000 d..^.....?......
+  0x000150f0 2aab016f b06d1584 f93f0000 00000000 *..o.m...?......
+  0x00015100 5a2107c9 86a60cf1 fb3f0000 00000000 Z!.......?......
+  0x00015110 0537e48b 0be96eb9 fd3f0000 00000000 .7....n..?......
+  0x00015120 71f3e43b 326c10b7 fe3f0000 00000000 q..;2l...?......
+  0x00015130 65ea113c 9ccf6c83 ff3f0000 00000000 e..<..l..?......
+  0x00015140 3d25c853 823c25c8 fe3f0000 00000000 =%.S.<%..?......
+  0x00015150 8a1873f8 f41955e0 fd3f0000 00000000 ..s...U..?......
+  0x00015160 639e3248 700158b4 fc3f0000 00000000 c.2Hp.X..?......
+  0x00015170 0c0bc8dd 50df3ac5 fa3f0000 00000000 ....P.:..?......
+  0x00015180 dd93bd94 cf859d83 f83f0000 00000000 .........?......
+  0x00015190 e87a5fa3 75f3fca1 f43f0000 00000000 .z_.u....?......
+  0x000151a0 7c221fea 95e43daa d73f0000 00000000 |"....=..?......
+  0x000151b0 428aba4f 96a9dcbc df3f0000 00000000 B..O.....?......
+  0x000151c0 b440f99d 54e9b0a9 e63f0000 00000000 .@..T....?......
+  0x000151d0 f8427b31 4b13a79f ec3f0000 00000000 .B{1K....?......
+  0x000151e0 54409f7c 9a0be8a9 f13f0000 00000000 T@.|.....?......
+  0x000151f0 621cecd3 227836ce f53f0000 00000000 b..."x6..?......
+  0x00015200 eca205df 9c35a188 f93f0000 00000000 .....5...?......
+  0x00015210 b2c5c913 3c7015b0 fb3f0000 00000000 ....<p...?......
+  0x00015220 92ca90bf 56541ca3 fc3f0000 00000000 ....VT...?......
+  0x00015230 b46ff021 829c24f0 e8bf0000 00000000 .o.!..$.........
+  0x00015240 af760f44 4ae626ff ec3f0000 00000000 .v.DJ.&..?......
+  0x00015250 8cd1596d 33393ec6 ef3f0000 00000000 ..Ym39>..?......
+  0x00015260 0aad1e89 7780279a f03f0000 00000000 ....w.'..?......
+  0x00015270 dd1197e6 6033a7cc f33f0000 00000000 ....`3...?......
+  0x00015280 1b7e73ee ac43a1d3 f63f0000 00000000 .~s..C...?......
+  0x00015290 0a9ef7f6 a92a30db f83f0000 00000000 .....*0..?......
+  0x000152a0 0d423d12 a82f229a fa3f0000 00000000 .B=../"..?......
+  0x000152b0 b4790dbc 6780d0a0 fb3f0000 00000000 .y..g....?......
+  0x000152c0 6a8c6195 a01d8981 fc3f0000 00000000 j.a......?......
+  0x000152d0 6304689a 50c36ca4 fc3f0000 00000000 c.h.P.l..?......
+  0x000152e0 849d16d3 86620ba6 fc3f0000 00000000 .....b...?......
+  0x000152f0 cef4a086 9b95af85 fc3f0000 00000000 .........?......
+  0x00015300 8c6583a0 70f4dbaa fb3f0000 00000000 .e..p....?......
+  0x00015310 cc4c5393 ac8e53ab fa3f0000 00000000 .LS...S..?......
+  0x00015320 f32a7782 92000584 f93f0000 00000000 .*w......?......
+  0x00015330 b7fc09e1 e7260a97 f73f0000 00000000 .....&...?......
+  0x00015340 cfde6148 57ddcdf1 f43f0000 00000000 ..aHW....?......
+  0x00015350 d6fd8310 a1dfdcf1 f13f0000 00000000 .........?......
+  0x00015360 8d94d65a 5bb4a2e3 ed3f0000 00000000 ...Z[....?......
+  0x00015370 a30e4e04 65b6e0ab e83f0000 00000000 ..N.e....?......
+  0x00015380 b92d09b4 feaa22a1 ec3f0000 00000000 .-...."..?......
+  0x00015390 ace3c8bd 17f5f5e6 ed3f0000 00000000 .........?......
+  0x000153a0 956a7eb7 36f9749f f13f0000 00000000 .j~.6.t..?......
+  0x000153b0 a6541b11 42abf2ad f43f0000 00000000 .T..B....?......
+  0x000153c0 00cefdac 5e7f42d6 f53f0000 00000000 ....^.B..?......
+  0x000153d0 e23c2c6e 0c6eea84 f73f0000 00000000 .<,n.n...?......
+  0x000153e0 608379ed f2eb5eb4 fa3f0000 00000000 `.y...^..?......
+  0x000153f0 9d24d28f 8334dcad fc3f0000 00000000 .$...4...?......
+  0x00015400 cfd671c9 f19dbfd5 fd3f0000 00000000 ..q......?......
+  0x00015410 d99eaabd 23f6cdbc fe3f0000 00000000 ....#....?......
+  0x00015420 1b888052 ab69f3fa fe3f0000 00000000 ...R.i...?......
+  0x00015430 c1db12dd c52b91c9 fe3f0000 00000000 .....+...?......
+  0x00015440 499dafa4 b7e6b9f3 fd3f0000 00000000 I........?......
+  0x00015450 ff8ccd3f 91619ade fc3f0000 00000000 ...?.a...?......
+  0x00015460 bfc3c33c 9bf5ce94 fb3f0000 00000000 ...<.....?......
+  0x00015470 08873396 8acf8f89 f93f0000 00000000 ..3......?......
+  0x00015480 8ea0ec7b 6e6d4e9d f63f0000 00000000 ...{nmN..?......
+  0x00015490 75de73c8 641fcba7 f23f0000 00000000 u.s.d....?......
+  0x000154a0 d5ef5ba4 d05ae9b9 d23f0000 00000000 ..[..Z...?......
+  0x000154b0 e0f3447b 1c046f8b db3f0000 00000000 ..D{..o..?......
+  0x000154c0 17810382 934238ad e23f0000 00000000 .....B8..?......
+  0x000154d0 95e25537 2d8af2e7 e83f0000 00000000 ..U7-....?......
+  0x000154e0 ae4e853c 297398b6 ee3f0000 00000000 .N.<)s...?......
+  0x000154f0 9288308c f4411bad f33f0000 00000000 ..0..A...?......
+  0x00015500 abf1514c 9a4695c2 f73f0000 00000000 ..QL.F...?......
+  0x00015510 c1926159 d1f026f5 fa3f0000 00000000 ..aY..&..?......
+  0x00015520 3707c924 5abe0299 fd3f0000 00000000 7..$Z....?......
+  0x00015530 02d09842 bdcf288b fe3f0000 00000000 ...B..(..?......
+  0x00015540 702592b0 3a95c9ca e73f0000 00000000 p%..:....?......
+  0x00015550 758cadb1 3561cff0 eb3f0000 00000000 u...5a...?......
+  0x00015560 029ff133 aea67487 ef3f0000 00000000 ...3..t..?......
+  0x00015570 ed4b96c9 7641e5bf f13f0000 00000000 .K..vA...?......
+  0x00015580 ed4b96c9 7641e5bf f33f0000 00000000 .K..vA...?......
+  0x00015590 f2b83017 19f1eb8f f53f0000 00000000 ..0......?......
+  0x000155a0 708263f0 4799e8a7 f63f0000 00000000 p.c.G....?......
+  0x000155b0 b11dca83 3045ea9b f73f0000 00000000 ....0E...?......
+  0x000155c0 892cafc5 c867dfe9 f73f0000 00000000 .,...g...?......
+  0x000155d0 8df023ce c114ec8e f83f0000 00000000 ..#......?......
   0x000155e0 00000000 00000080 00000000 00000000 ................
   0x000155f0 00000000 0000e03f 00000000 00003043 .......?......0C
-  0x00015600 00000000 0000f03f 00000000 00000080 .......?........
+  0x00015600 00000000 0000f03f ffffffff ffffff7f .......?........
   0x00015610 00000000 00005940                   ......Y@
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,12 +1,12 @@
 
 Hex dump of section '.eh_frame_hdr':
   0x00015618 011b033b 8c000000 10000000 08bafeff ...;............
   0x00015628 a8000000 18bbfeff d0000000 e8bbfeff ................
-  0x00015638 e8000000 58bcfeff fc000000 28bdfeff ....X.......(...
-  0x00015648 10010000 08bffeff 24010000 38c2feff ........$...8...
-  0x00015658 38010000 c8c7feff 54010000 b8d0feff 8.......T.......
-  0x00015668 70010000 48defeff 90010000 c8f1feff p...H...........
-  0x00015678 b0010000 580effff d0010000 4835ffff ....X.......H5..
-  0x00015688 f0010000 3864ffff 10020000 9864ffff ....8d.......d..
-  0x00015698 24020000 9865ffff 38020000          $....e..8...
+  0x00015638 e8000000 48bcfeff fc000000 18bdfeff ....H...........
+  0x00015648 10010000 d8befeff 24010000 f8c1feff ........$.......
+  0x00015658 38010000 68c7feff 54010000 28d0feff 8...h...T...(...
+  0x00015668 70010000 78ddfeff 90010000 c8f0feff p...x...........
+  0x00015678 b0010000 680dffff d0010000 4834ffff ....h.......H4..
+  0x00015688 f0010000 0863ffff 10020000 6863ffff .....c......hc..
+  0x00015698 24020000 6864ffff 38020000          $...hd..8...
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -2,34 +2,34 @@
 Hex dump of section '.eh_frame':
   0x000156a8 14000000 00000000 017a5200 01781001 .........zR..x..
   0x000156b8 1b0c0708 90010000 24000000 1c000000 ........$.......
   0x000156c8 58b9feff 10010000 000e1046 0e184a0f X..........F..J.
   0x000156d8 0b770880 003f1a3b 2a332422 00000000 .w...?.;*3$"....
   0x000156e8 14000000 44000000 40bafeff 08000000 ....D...@.......
   0x000156f8 00000000 00000000 10000000 5c000000 ............\...
-  0x00015708 f8bafeff 68000000 00000000 10000000 ....h...........
-  0x00015718 70000000 54bbfeff cc000000 00000000 p...T...........
-  0x00015728 10000000 84000000 10bcfeff dd010000 ................
-  0x00015738 00000000 10000000 98000000 dcbdfeff ................
-  0x00015748 29030000 00000000 18000000 ac000000 )...............
-  0x00015758 f8c0feff 81050000 00440e48 0343050a .........D.H.C..
-  0x00015768 0e08490b 18000000 c8000000 6cc6feff ..I.........l...
-  0x00015778 eb080000 00440e68 03ab080a 0e08410b .....D.h......A.
-  0x00015788 1c000000 e4000000 40cffeff 8d0d0000 ........@.......
-  0x00015798 00470ea8 01033f0d 0a0e084a 0b000000 .G....?....J....
-  0x000157a8 1c000000 04010000 b0dcfeff 7f130000 ................
-  0x000157b8 00470e88 02032a13 0a0e0847 0b000000 .G....*....G....
-  0x000157c8 1c000000 24010000 10f0feff 871c0000 ....$...........
-  0x000157d8 00470ec8 02032b1c 0a0e0846 0b000000 .G....+....F....
-  0x000157e8 1c000000 44010000 800cffff e5260000 ....D........&..
-  0x000157f8 00470ef8 02037c26 0a0e0845 0b000000 .G....|&...E....
-  0x00015808 1c000000 64010000 5033ffff e12e0000 ....d...P3......
-  0x00015818 00470ee8 0303642e 0a0e0845 0b000000 .G....d....E....
-  0x00015828 10000000 84010000 2062ffff 5e000000 ........ b..^...
-  0x00015838 00000000 10000000 98010000 6c62ffff ............lb..
+  0x00015708 f8bafeff 5f000000 00000000 10000000 ...._...........
+  0x00015718 70000000 44bbfeff c2000000 00000000 p...D...........
+  0x00015728 10000000 84000000 00bcfeff b1010000 ................
+  0x00015738 00000000 10000000 98000000 acbdfeff ................
+  0x00015748 13030000 00000000 18000000 ac000000 ................
+  0x00015758 b8c0feff 63050000 00440e28 033b050a ....c....D.(.;..
+  0x00015768 0e08410b 18000000 c8000000 0cc6feff ..A.............
+  0x00015778 bd080000 00440e58 0388080a 0e08440b .....D.X......D.
+  0x00015788 1c000000 e4000000 b0cefeff 450d0000 ............E...
+  0x00015798 00470ea8 0103060d 0a0e0843 0b000000 .G.........C....
+  0x000157a8 1c000000 04010000 e0dbfeff 4f130000 ............O...
+  0x000157b8 00470ee8 01030d13 0a0e0844 0b000000 .G.........D....
+  0x000157c8 1c000000 24010000 10effeff 9b1c0000 ....$...........
+  0x000157d8 00470eb8 0203431c 0a0e0846 0b000000 .G....C....F....
+  0x000157e8 1c000000 44010000 900bffff df260000 ....D........&..
+  0x000157f8 00470ee8 02037f26 0a0e084a 0b000000 .G.....&...J....
+  0x00015808 1c000000 64010000 5032ffff bd2e0000 ....d...P2......
+  0x00015818 00470ed8 0303462e 0a0e0843 0b000000 .G....F....C....
+  0x00015828 10000000 84010000 f060ffff 5e000000 .........`..^...
+  0x00015838 00000000 10000000 98010000 3c61ffff ............<a..
   0x00015848 f4000000 00000000 4c000000 ac010000 ........L.......
-  0x00015858 5863ffff e2060000 00420e10 8f02460e Xc.......B....F.
+  0x00015858 2862ffff f6050000 00420e10 8f02460e (b.......B....F.
   0x00015868 188e0342 0e208d04 420e288c 05410e30 ...B. ..B.(..A.0
-  0x00015878 8606410e 38830747 0ef00103 ee040a0e ..A.8..G........
+  0x00015878 8606410e 38830747 0ee00103 8c040a0e ..A.8..G........
   0x00015888 38410e30 410e2842 0e20420e 18420e10 8A.0A.(B. B..B..
-  0x00015898 420e0843 0b000000 00000000          B..C........
+  0x00015898 420e0845 0b000000 00000000          B..E........
```

#### readelf --wide --decompress --hex-dump=.init_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.init_array':
-  0x00016e10 f0110000 00000000                   ........
+  0x00016df8 f0110000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.fini_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.fini_array':
-  0x00016e18 b0110000 00000000                   ........
+  0x00016e00 b0110000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.got {}

```diff
@@ -1,5 +1,5 @@
 
 Hex dump of section '.got':
-  0x00016fe0 00000000 00000000 00000000 00000000 ................
-  0x00016ff0 00000000 00000000 00000000 00000000 ................
+  0x00016fc8 00000000 00000000 00000000 00000000 ................
+  0x00016fd8 00000000 00000000 00000000 00000000 ................
```

#### readelf --wide --decompress --hex-dump=.got.plt {}

```diff
@@ -1,14 +1,14 @@
 
 Hex dump of section '.got.plt':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
-  0x00017000 206e0100 00000000 00000000 00000000  n..............
-  0x00017010 00000000 00000000 36100000 00000000 ........6.......
-  0x00017020 46100000 00000000 56100000 00000000 F.......V.......
-  0x00017030 66100000 00000000 76100000 00000000 f.......v.......
-  0x00017040 86100000 00000000 96100000 00000000 ................
-  0x00017050 a6100000 00000000 b6100000 00000000 ................
-  0x00017060 c6100000 00000000 d6100000 00000000 ................
-  0x00017070 e6100000 00000000 f6100000 00000000 ................
-  0x00017080 06110000 00000000 16110000 00000000 ................
-  0x00017090 26110000 00000000                   &.......
+  0x00016fe8 086e0100 00000000 00000000 00000000 .n..............
+  0x00016ff8 00000000 00000000 36100000 00000000 ........6.......
+  0x00017008 46100000 00000000 56100000 00000000 F.......V.......
+  0x00017018 66100000 00000000 76100000 00000000 f.......v.......
+  0x00017028 86100000 00000000 96100000 00000000 ................
+  0x00017038 a6100000 00000000 b6100000 00000000 ................
+  0x00017048 c6100000 00000000 d6100000 00000000 ................
+  0x00017058 e6100000 00000000 f6100000 00000000 ................
+  0x00017068 06110000 00000000 16110000 00000000 ................
+  0x00017078 26110000 00000000                   &.......
```

#### readelf --wide --decompress --hex-dump=.data {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.data':
-  0x00017098 98700100 00000000                   .p......
+  0x00017080 80700100 00000000                   .p......
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Debian 10.2.1-6) 10.2.1 20210110
+  [     0]  GCC: (Debian 12.2.0-14) 12.2.0
```

### Comparing `lpsd-1.0.3/lpsd/wrapper.py` & `lpsd-1.0.4/lpsd/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 For the core part of the algorithm it uses an C implementation by M. Hewitson/G.Heinzel.
 Additionally a pure python implementation is provided.
 It depends on the packages numpy and ctypes.
 Ref: Improved spectrum estimation from digitized time series
 on a logarithmic frequency axis
 https://doi.org/10.1016/j.measurement.2005.10.010
 """
+
 from typing import Union
 from pandas import DataFrame
 
 from ._lcsd import LCSD
 
 
 def lcsd(data: DataFrame, *args, **kwargs) -> DataFrame:
```

### Comparing `lpsd-1.0.3/pyproject.toml` & `lpsd-1.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "lpsd"
-version = "1.0.3"
+version = "1.0.4"
 description = "Python and C implementation for logarithmical power spectral density (LPSD) calculation."
 authors = ["Christoph Bode <christoph.bode@aei.mpg.de>",
     "Gerhard Heinzel",
     "Christian Darsow-Fromm <cdarsowf@physnet.uni-hamburg.de>",
     "Artem Basalaev <artem.basalaev@physikDOTuni-hamburg.de>"]
 maintainers = ["Christian Darsow-Fromm <cdarsowf@physnet.uni-hamburg.de>"]
 readme = "README.md"
 repository = "https://gitlab.com/uhh-gwd/lpsd"
 documentation = "https://gitlab.com/uhh-gwd/lpsd/-/blob/main/README.md"
 include = ["**/*.so"]
 exclude = ["**/*.h", "**/*.c"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-pandas = ">=1.0,<2.0"
+python = ">=3.8,<3.14"
+pandas = ">=1.0,<3.0"
 numpy = ">=1.18,<2.0"
 scipy = ">=1.5,<2.0"
 importlib-metadata = {version = "^1.1.3", python = "<=3.7"}
 
 [tool.poetry.dev-dependencies]
-black = "^22.3.0"
-pytest = "^7.1.2"
-pytest-cov = "^4.0.0"
-pre-commit = "^2.15.0"
-mypy = "^0.991"
-pylint = "^2.15.9"
+black = "^24.3.0"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+pre-commit = "^3.5.0"
+mypy = "^1.9.0"
+pylint = "^3.1.0"
 isort = "^5.10.1"
 pytest-watch = "^4.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lpsd-1.0.3/PKG-INFO` & `lpsd-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: lpsd
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python and C implementation for logarithmical power spectral density (LPSD) calculation.
 Home-page: https://gitlab.com/uhh-gwd/lpsd
 Author: Christoph Bode
 Author-email: christoph.bode@aei.mpg.de
 Maintainer: Christian Darsow-Fromm
 Maintainer-email: cdarsowf@physnet.uni-hamburg.de
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<3.14
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: importlib-metadata (>=1.1.3,<2.0.0) ; python_full_version <= "3.7.0"
 Requires-Dist: numpy (>=1.18,<2.0)
-Requires-Dist: pandas (>=1.0,<2.0)
+Requires-Dist: pandas (>=1.0,<3.0)
 Requires-Dist: scipy (>=1.5,<2.0)
 Project-URL: Documentation, https://gitlab.com/uhh-gwd/lpsd/-/blob/main/README.md
 Project-URL: Repository, https://gitlab.com/uhh-gwd/lpsd
 Description-Content-Type: text/markdown
 
 # Python 3 LPSD algorithm
```

