# Comparing `tmp/upp-0.2.0.tar.gz` & `tmp/upp-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upp-0.2.0.tar", last modified: Mon Mar 25 19:02:59 2024, max compression
+gzip compressed data, was "upp-0.2.1.tar", last modified: Mon Apr  8 15:37:55 2024, max compression
```

## Comparing `upp-0.2.0.tar` & `upp-0.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-03-25 19:02:59.246757 upp-0.2.0/
--rw-r--r--   0 samir     (1000) samir     (1000)     1225 2021-01-04 17:42:38.000000 upp-0.2.0/.gitignore
--rw-r--r--   0 samir     (1000) samir     (1000)    35149 2019-02-20 19:25:43.000000 upp-0.2.0/LICENSE
--rw-r--r--   0 samir     (1000) samir     (1000)     7956 2024-03-25 19:02:59.246757 upp-0.2.0/PKG-INFO
--rw-r--r--   0 samir     (1000) samir     (1000)     7252 2024-03-25 18:35:38.000000 upp-0.2.0/README.md
--rw-r--r--   0 samir     (1000) samir     (1000)       38 2024-03-25 19:02:59.246757 upp-0.2.0/setup.cfg
--rw-r--r--   0 samir     (1000) samir     (1000)     1054 2024-03-25 18:40:07.000000 upp-0.2.0/setup.py
-drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-03-25 19:02:59.243424 upp-0.2.0/src/
-drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-03-25 19:02:59.243424 upp-0.2.0/src/upp/
--rw-r--r--   0 samir     (1000) samir     (1000)        0 2020-03-27 07:44:19.000000 upp-0.2.0/src/upp/__init__.py
-drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-03-25 19:02:59.243424 upp-0.2.0/src/upp/atom_gen/
--rw-r--r--   0 samir     (1000) samir     (1000)     3582 2024-03-25 15:46:08.000000 upp-0.2.0/src/upp/atom_gen/README.md
--rw-r--r--   0 samir     (1000) samir     (1000)        0 2021-08-15 09:31:23.000000 upp-0.2.0/src/upp/atom_gen/__init__.py
--rw-r--r--   0 samir     (1000) samir     (1000)     8599 2024-03-25 16:25:09.000000 upp-0.2.0/src/upp/atom_gen/atombios.py
--rw-r--r--   0 samir     (1000) samir     (1000)    30254 2024-03-25 16:25:20.000000 upp-0.2.0/src/upp/atom_gen/pptable_v1_0.py
--rw-r--r--   0 samir     (1000) samir     (1000)    31364 2024-03-25 16:25:45.000000 upp-0.2.0/src/upp/atom_gen/smu_v11_0_7_navi20.py
--rw-rw-r--   0 samir     (1000) samir     (1000)    25359 2024-03-25 16:25:40.000000 upp-0.2.0/src/upp/atom_gen/smu_v11_0_navi10.py
--rw-r--r--   0 samir     (1000) samir     (1000)    39447 2024-03-25 16:25:49.000000 upp-0.2.0/src/upp/atom_gen/smu_v13_0_7_navi30.py
--rw-rw-r--   0 samir     (1000) samir     (1000)    30177 2024-03-25 16:25:31.000000 upp-0.2.0/src/upp/atom_gen/vega10_pptable.py
--rw-rw-r--   0 samir     (1000) samir     (1000)    22595 2024-03-25 16:25:35.000000 upp-0.2.0/src/upp/atom_gen/vega20_pptable.py
--rw-r--r--   0 samir     (1000) samir     (1000)    34943 2024-03-25 18:23:43.000000 upp-0.2.0/src/upp/decode.py
--rwxr-xr-x   0 samir     (1000) samir     (1000)    16881 2024-03-25 18:27:25.000000 upp-0.2.0/src/upp/upp.py
-drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-03-25 19:02:59.246757 upp-0.2.0/src/upp.egg-info/
--rw-r--r--   0 samir     (1000) samir     (1000)     7956 2024-03-25 19:02:59.000000 upp-0.2.0/src/upp.egg-info/PKG-INFO
--rw-r--r--   0 samir     (1000) samir     (1000)     1231 2024-03-25 19:02:59.000000 upp-0.2.0/src/upp.egg-info/SOURCES.txt
--rw-r--r--   0 samir     (1000) samir     (1000)        1 2024-03-25 19:02:59.000000 upp-0.2.0/src/upp.egg-info/dependency_links.txt
--rw-r--r--   0 samir     (1000) samir     (1000)       37 2024-03-25 19:02:59.000000 upp-0.2.0/src/upp.egg-info/entry_points.txt
--rw-r--r--   0 samir     (1000) samir     (1000)       17 2024-03-25 19:02:59.000000 upp-0.2.0/src/upp.egg-info/requires.txt
--rw-r--r--   0 samir     (1000) samir     (1000)       17 2024-03-25 19:02:59.000000 upp-0.2.0/src/upp.egg-info/top_level.txt
-drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-03-25 19:02:59.246757 upp-0.2.0/test/
--rw-rw-r--   0 samir     (1000) samir     (1000)     8888 2021-06-03 18:56:29.000000 upp-0.2.0/test/AMD.RX480.8192.160603.rom.dump
--rw-rw-r--   0 samir     (1000) samir     (1000)    26376 2021-06-03 18:56:43.000000 upp-0.2.0/test/AMD.RX480.8192.160603.rom.rawdump
--rw-rw-r--   0 samir     (1000) samir     (1000)       91 2021-01-04 17:30:40.000000 upp-0.2.0/test/AMD.RX5700XT.8192.190616.rom.check
--rw-rw-r--   0 samir     (1000) samir     (1000)    16270 2021-01-04 17:25:18.000000 upp-0.2.0/test/AMD.RX5700XT.8192.190616.rom.dump
--rw-rw-r--   0 samir     (1000) samir     (1000)    44626 2021-01-04 17:25:20.000000 upp-0.2.0/test/AMD.RX5700XT.8192.190616.rom.rawdump
--rw-rw-r--   0 samir     (1000) samir     (1000)    24169 2021-06-03 19:05:56.000000 upp-0.2.0/test/AMD.RX6900.16384.201104.rom.dump
--rw-rw-r--   0 samir     (1000) samir     (1000)    65751 2024-03-25 16:24:27.000000 upp-0.2.0/test/AMD.RX6900.16384.201104.rom.rawdump
--rw-r--r--   0 samir     (1000) samir     (1000)    45635 2024-03-25 18:13:40.000000 upp-0.2.0/test/AMD.RX7900XTX.24576.230323.rom.dump
--rw-r--r--   0 samir     (1000) samir     (1000)   110096 2024-03-25 18:32:04.000000 upp-0.2.0/test/AMD.RX7900XTX.24576.230323.rom.rawdump
--rw-rw-r--   0 samir     (1000) samir     (1000)     7718 2021-01-04 17:25:18.000000 upp-0.2.0/test/AMD.RXVega64.8176.170719.rom.dump
--rw-rw-r--   0 samir     (1000) samir     (1000)    21669 2021-01-04 17:25:20.000000 upp-0.2.0/test/AMD.RXVega64.8176.170719.rom.rawdump
--rw-r--r--   0 samir     (1000) samir     (1000)     6722 2022-07-03 10:14:53.000000 upp-0.2.0/test/AMD.RXVegaFrontier.16384.170628.rom.dump
--rw-r--r--   0 samir     (1000) samir     (1000)    19177 2022-07-03 10:18:33.000000 upp-0.2.0/test/AMD.RXVegaFrontier.16384.170628.rom.rawdump
--rw-rw-r--   0 samir     (1000) samir     (1000)    16605 2021-01-04 17:25:18.000000 upp-0.2.0/test/AMD.RadeonVII.16384.190116.rom.dump
--rw-rw-r--   0 samir     (1000) samir     (1000)    41443 2021-01-04 17:25:20.000000 upp-0.2.0/test/AMD.RadeonVII.16384.190116.rom.rawdump
--rw-r--r--   0 samir     (1000) samir     (1000)     2726 2024-03-23 09:43:45.000000 upp-0.2.0/test/navi23.mpt
--rwxrwxr-x   0 samir     (1000) samir     (1000)     3991 2024-03-25 18:46:45.000000 upp-0.2.0/test/test.sh
+drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-04-08 15:37:55.832385 upp-0.2.1/
+-rw-r--r--   0 samir     (1000) samir     (1000)     1225 2021-01-04 17:42:38.000000 upp-0.2.1/.gitignore
+-rw-r--r--   0 samir     (1000) samir     (1000)    35149 2019-02-20 19:25:43.000000 upp-0.2.1/LICENSE
+-rw-r--r--   0 samir     (1000) samir     (1000)     7956 2024-04-08 15:37:55.832385 upp-0.2.1/PKG-INFO
+-rw-r--r--   0 samir     (1000) samir     (1000)     7252 2024-03-25 18:35:38.000000 upp-0.2.1/README.md
+-rw-r--r--   0 samir     (1000) samir     (1000)       38 2024-04-08 15:37:55.835718 upp-0.2.1/setup.cfg
+-rw-r--r--   0 samir     (1000) samir     (1000)     1054 2024-04-08 15:16:53.000000 upp-0.2.1/setup.py
+drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-04-08 15:37:55.829051 upp-0.2.1/src/
+drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-04-08 15:37:55.832385 upp-0.2.1/src/upp/
+-rw-r--r--   0 samir     (1000) samir     (1000)        0 2020-03-27 07:44:19.000000 upp-0.2.1/src/upp/__init__.py
+drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-04-08 15:37:55.832385 upp-0.2.1/src/upp/atom_gen/
+-rw-r--r--   0 samir     (1000) samir     (1000)     3582 2024-03-25 15:46:08.000000 upp-0.2.1/src/upp/atom_gen/README.md
+-rw-r--r--   0 samir     (1000) samir     (1000)        0 2021-08-15 09:31:23.000000 upp-0.2.1/src/upp/atom_gen/__init__.py
+-rw-r--r--   0 samir     (1000) samir     (1000)     8599 2024-03-25 16:25:09.000000 upp-0.2.1/src/upp/atom_gen/atombios.py
+-rw-r--r--   0 samir     (1000) samir     (1000)    30254 2024-03-25 16:25:20.000000 upp-0.2.1/src/upp/atom_gen/pptable_v1_0.py
+-rw-r--r--   0 samir     (1000) samir     (1000)    31364 2024-04-01 12:39:06.000000 upp-0.2.1/src/upp/atom_gen/smu_v11_0_7_navi20.py
+-rw-rw-r--   0 samir     (1000) samir     (1000)    25359 2024-03-25 16:25:40.000000 upp-0.2.1/src/upp/atom_gen/smu_v11_0_navi10.py
+-rw-r--r--   0 samir     (1000) samir     (1000)    39447 2024-03-25 16:25:49.000000 upp-0.2.1/src/upp/atom_gen/smu_v13_0_7_navi30.py
+-rw-rw-r--   0 samir     (1000) samir     (1000)    30177 2024-03-25 16:25:31.000000 upp-0.2.1/src/upp/atom_gen/vega10_pptable.py
+-rw-rw-r--   0 samir     (1000) samir     (1000)    22595 2024-03-25 16:25:35.000000 upp-0.2.1/src/upp/atom_gen/vega20_pptable.py
+-rw-r--r--   0 samir     (1000) samir     (1000)    38974 2024-04-08 15:10:39.000000 upp-0.2.1/src/upp/decode.py
+-rwxr-xr-x   0 samir     (1000) samir     (1000)    16881 2024-03-25 18:27:25.000000 upp-0.2.1/src/upp/upp.py
+drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-04-08 15:37:55.832385 upp-0.2.1/src/upp.egg-info/
+-rw-r--r--   0 samir     (1000) samir     (1000)     7956 2024-04-08 15:37:55.000000 upp-0.2.1/src/upp.egg-info/PKG-INFO
+-rw-r--r--   0 samir     (1000) samir     (1000)     1231 2024-04-08 15:37:55.000000 upp-0.2.1/src/upp.egg-info/SOURCES.txt
+-rw-r--r--   0 samir     (1000) samir     (1000)        1 2024-04-08 15:37:55.000000 upp-0.2.1/src/upp.egg-info/dependency_links.txt
+-rw-r--r--   0 samir     (1000) samir     (1000)       37 2024-04-08 15:37:55.000000 upp-0.2.1/src/upp.egg-info/entry_points.txt
+-rw-r--r--   0 samir     (1000) samir     (1000)       17 2024-04-08 15:37:55.000000 upp-0.2.1/src/upp.egg-info/requires.txt
+-rw-r--r--   0 samir     (1000) samir     (1000)       17 2024-04-08 15:37:55.000000 upp-0.2.1/src/upp.egg-info/top_level.txt
+drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-04-08 15:37:55.832385 upp-0.2.1/test/
+-rw-rw-r--   0 samir     (1000) samir     (1000)     8888 2021-06-03 18:56:29.000000 upp-0.2.1/test/AMD.RX480.8192.160603.rom.dump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    30539 2024-04-08 14:54:40.000000 upp-0.2.1/test/AMD.RX480.8192.160603.rom.rawdump
+-rw-rw-r--   0 samir     (1000) samir     (1000)       91 2021-01-04 17:30:40.000000 upp-0.2.1/test/AMD.RX5700XT.8192.190616.rom.check
+-rw-rw-r--   0 samir     (1000) samir     (1000)    17367 2024-04-08 15:13:17.000000 upp-0.2.1/test/AMD.RX5700XT.8192.190616.rom.dump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    51669 2024-04-08 15:15:25.000000 upp-0.2.1/test/AMD.RX5700XT.8192.190616.rom.rawdump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    25867 2024-04-08 14:58:34.000000 upp-0.2.1/test/AMD.RX6900.16384.201104.rom.dump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    76184 2024-04-08 15:04:05.000000 upp-0.2.1/test/AMD.RX6900.16384.201104.rom.rawdump
+-rw-r--r--   0 samir     (1000) samir     (1000)    47367 2024-04-08 15:06:00.000000 upp-0.2.1/test/AMD.RX7900XTX.24576.230323.rom.dump
+-rw-r--r--   0 samir     (1000) samir     (1000)   127547 2024-04-08 15:07:25.000000 upp-0.2.1/test/AMD.RX7900XTX.24576.230323.rom.rawdump
+-rw-rw-r--   0 samir     (1000) samir     (1000)     7718 2021-01-04 17:25:18.000000 upp-0.2.1/test/AMD.RXVega64.8176.170719.rom.dump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    25072 2024-04-08 14:55:09.000000 upp-0.2.1/test/AMD.RXVega64.8176.170719.rom.rawdump
+-rw-r--r--   0 samir     (1000) samir     (1000)     6722 2022-07-03 10:14:53.000000 upp-0.2.1/test/AMD.RXVegaFrontier.16384.170628.rom.dump
+-rw-r--r--   0 samir     (1000) samir     (1000)    22180 2024-04-08 14:55:12.000000 upp-0.2.1/test/AMD.RXVegaFrontier.16384.170628.rom.rawdump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    16605 2021-01-04 17:25:18.000000 upp-0.2.1/test/AMD.RadeonVII.16384.190116.rom.dump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    48006 2024-04-08 14:51:07.000000 upp-0.2.1/test/AMD.RadeonVII.16384.190116.rom.rawdump
+-rw-r--r--   0 samir     (1000) samir     (1000)     2726 2024-03-23 09:43:45.000000 upp-0.2.1/test/navi23.mpt
+-rwxrwxr-x   0 samir     (1000) samir     (1000)     3991 2024-03-25 18:46:45.000000 upp-0.2.1/test/test.sh
```

### Comparing `upp-0.2.0/.gitignore` & `upp-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/LICENSE` & `upp-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/PKG-INFO` & `upp-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upp
-Version: 0.2.0
+Version: 0.2.1
 Summary: Uplift Power Play
 Home-page: https://github.com/sibradzic/upp
 Author: Samir Ibradžić
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `upp-0.2.0/README.md` & `upp-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/setup.py` & `upp-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='upp',
-    version='0.2.0',
+    version='0.2.1',
     author='Samir Ibradžić',
     description='Uplift Power Play',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sibradzic/upp',
     package_dir={'': 'src'},
     packages=['upp', 'upp/atom_gen'],
```

### Comparing `upp-0.2.0/src/upp/atom_gen/README.md` & `upp-0.2.1/src/upp/atom_gen/README.md`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/src/upp/atom_gen/atombios.py` & `upp-0.2.1/src/upp/atom_gen/atombios.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/src/upp/atom_gen/pptable_v1_0.py` & `upp-0.2.1/src/upp/atom_gen/pptable_v1_0.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/src/upp/atom_gen/smu_v11_0_7_navi20.py` & `upp-0.2.1/src/upp/atom_gen/smu_v11_0_7_navi20.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/src/upp/atom_gen/smu_v11_0_navi10.py` & `upp-0.2.1/src/upp/atom_gen/smu_v11_0_navi10.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/src/upp/atom_gen/smu_v13_0_7_navi30.py` & `upp-0.2.1/src/upp/atom_gen/smu_v13_0_7_navi30.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/src/upp/atom_gen/vega10_pptable.py` & `upp-0.2.1/src/upp/atom_gen/vega10_pptable.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/src/upp/atom_gen/vega20_pptable.py` & `upp-0.2.1/src/upp/atom_gen/vega20_pptable.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/src/upp/decode.py` & `upp-0.2.1/src/upp/decode.py`

 * *Files 8% similar despite different names*

```diff
@@ -241,27 +241,34 @@
     print('Shifting checksum by {}...'.format(new_checksum))
     rom_bytes[0x21] = (rom_bytes[0x21] - new_checksum) & 0xff
     _write_binary_file(output_rom, rom_bytes)
 
     return True
 
 
-def validate_pp(header, length, rawdump):
+def validate_pp(header, rawbytes, rawdump):
     """
     Validates PowerPlay master table header
     """
 
     pp_frev = header.ucTableFormatRevision
     pp_crev = header.ucTableContentRevision
     pp_len = header.usStructureSize
+    rw_len = len(rawbytes)
 
-    if pp_len != length:
+    if pp_len != rw_len and pp_frev in [20, 21, 22] and rw_len == 4095:
+        msg = 'WARNING: Trying to work around rev {}.{} table truncated ' + \
+              'at 0x{:04x}, setting all missing values to zeroes.'
+        print(msg.format(pp_frev, pp_crev, rw_len))
+        rawbytes.extend(bytearray(pp_len-rw_len))
+        rw_len = len(rawbytes)
+    if pp_len != rw_len:
         msg = 'ERROR: Header length ({}) differs from file length ({}). ' + \
               'Is this a valid PowerPlay table?'
-        print(msg.format(pp_len, length))
+        print(msg.format(pp_len, rw_len))
         return None
     if rawdump:
         msg = 'PowerPlay table rev {}.{} size {} bytes'
         print(msg.format(pp_frev, pp_crev, pp_len))
     return pp_frev, pp_crev
 
 
@@ -296,21 +303,23 @@
             if is_i_plus1_big:
                 indices.append(i+1)
         i = i + 1
 
     return indices
 
 
-def _print_raw_value(offset, symbol, rawbytes, name, value):
+def _print_raw_value(offset, symbol, rawbytes, name, desc, value):
     hexval = _bytes2hex(rawbytes)
-    raw_msg = ' 0x{:04x} ({:04n}) {} {:>8} {:32s}:{: n}'
+    raw_msg = ' 0x{:04x} ({:04n}) {} {:>8} {:42s}:{: n}'
     # Polaris variable names have small-caps prefixes that we don't want
     big_caps = _get_bigcap_indices(name)
     if big_caps:
         name = name[big_caps[0]:]
+    if desc:
+        name = name + ' ' + desc
     print(raw_msg.format(offset, offset, symbol, hexval, name, value))
 
 
 def _get_ofst_cstruct(module, name, header_bytes, debug=False):
     """
     Resolves C structure name and its size from parent table's name
 
@@ -513,16 +522,16 @@
 
     """
 
     # Init decoded data dictionary
     if decoded is None:
         decoded = odict()
         if rawdump:
-            print(' Offset (dec.) t Raw val. Variable name ' + ' '*18 +
-                  'Decoded value\n' + '-'*71)
+            print(' Offset (dec.) t Raw val. Variable name ' + ' '*24 +
+                  'Decoded value\n' + '-'*78)
 
     # Here we parse data items in C Arrays (all items are same type)
     if issubclass(type(data), ctypes.Array):
         d_size = meta['size'] // len(data)
         d_offset = meta['ofs']
         index = 0
 
@@ -534,17 +543,21 @@
                 if parent_name in float_arrays:
                     d_symbol = 'f'
                     d_value = struct.unpack(d_symbol, d_bytes)[0]
                 child_key = index
                 decoded[child_key] = {'value':  d_value,
                                       'offset': d_offset,
                                       'type':   d_symbol}
+                desc = ''
+                if 'desc' in meta and index < len(meta['desc']) - 1:
+                    desc = meta['desc'][index]
+                    decoded[child_key]['desc'] = desc
                 if rawdump:
                     _print_raw_value(d_offset, d_symbol, d_bytes,
-                                     parent_name, d_value)
+                                     parent_name, desc, d_value)
                 d_offset += d_size
                 index += 1
 
         # Other types are recursed back into this very same function
         else:
             for item in data:
                 if debug:
@@ -565,15 +578,15 @@
     elif issubclass(type(data), ctypes.Structure):
         for name, ctyp_cls in data._fields_:
             d_value = getattr(data, name)
             d_meta = getattr(type(data), name)
             d_size = d_meta.size
             if name.startswith(('uc', 'us', 'ul')):
                 name = name[2:]
-            if not meta:
+            if 'ofs' not in meta:
                 d_offset = d_meta.offset
             else:
                 d_offset = meta['ofs'] + d_meta.offset
 
             # Base types parsed as is, exception are floats & offset tables
             if ctyp_cls in primitives:
                 d_symbol = ctyp_cls._type_
@@ -583,15 +596,15 @@
                 else:
                     d_bytes = d_value.to_bytes(d_size, 'little')
                 if ctyp_cls == ctypes.c_uint and name in float_fields:
                     d_symbol = 'f'
                     d_value = struct.unpack(d_symbol, d_bytes)[0]
                 if rawdump:
                     _print_raw_value(d_offset, d_symbol, d_bytes,
-                                     name, d_value)
+                                     name, '', d_value)
                 # Check if this is a pointer to an offset-ed table:
                 if not name.endswith(('ArrayOffset',
                                       'TableOffset',
                                       'ControllerOffset')):
                     decoded[name] = {'value':  d_value,
                                      'offset': d_offset,
                                      'type':   d_symbol}
@@ -625,14 +638,22 @@
 
             # Other types are recursed back into this very same function
             else:
                 if debug:
                     msg = 'DEBUG: Recursive dive from {} struct into "{}"'
                     print(msg.format(parent_name, name))
                 r_meta = {'ofs': d_offset, 'size': d_size}
+                if 'enum' in meta:
+                    if name in meta['enum']:
+                        r_meta['enum'] = {name: meta['enum'][name]}
+                    if parent_name in meta['enum'] and name in ['min', 'max']:
+                        r_meta['desc'] = meta['enum'][parent_name]['enum']
+                    if parent_name in meta['enum'] and name in ['cap']:
+                        r_meta['desc'] = meta['enum'][parent_name]['cap']
+
                 decoded[name] = odict()
                 build_data_tree(d_value, raw, decoded[name], name, r_meta,
                                 rawdump, debug)
                 if debug:
                     print('DEBUG: End of recursion into "{}"'.format(name))
 
     else:
@@ -643,15 +664,16 @@
 
 def select_pp_struct(rawbytes, rawdump=False, debug=False):
     """
     Selects appropriate variant of ctype data structures for conversion
     """
 
     pp_header = common_hdr.from_buffer(rawbytes[:4])
-    pp_ver = validate_pp(pp_header, len(rawbytes), rawdump)
+    pp_ver = validate_pp(pp_header, rawbytes, rawdump)
+    enum_structs = {}
 
     # Polaris aka RX470/RX480/RX570/RX580/RX590
     if pp_ver == (7, 1):
         gpugen = 'Polaris'
         from upp.atom_gen import pptable_v1_0 as pp_struct
         ctypes_strct = pp_struct.struct__ATOM_Tonga_POWERPLAYTABLE
     # Vega 10 aka Vega 56/64
@@ -665,45 +687,105 @@
         from upp.atom_gen import vega20_pptable as pp_struct
         ctypes_strct = pp_struct.struct__ATOM_VEGA20_POWERPLAYTABLE
     # Navi 10 aka RX5700/RX5600(XT,M), Navi 14 aka RX5500/RX5300(XT,M)
     elif pp_ver == (12, 0):
         gpugen = 'Navi 10 or 14'
         from upp.atom_gen import smu_v11_0_navi10 as pp_struct
         ctypes_strct = pp_struct.struct_smu_11_0_powerplay_table
+        enum_structs = {
+            'power_saving_clock': {
+                'prefix': 'SMU_11_0_PPCLOCK_',
+                'struct': pp_struct.SMU_11_0_PPCLOCK_ID__enumvalues
+            },
+            'overdrive_table': {
+                'prefix': 'SMU_11_0_ODSETTING_',
+                'struct': pp_struct.SMU_11_0_ODSETTING_ID__enumvalues,
+                'cappfx': 'SMU_11_0_ODCAP_',
+                'capstr': pp_struct.SMU_11_0_ODFEATURE_CAP__enumvalues,
+            }
+        }
     # Navi 12 aka PRO V520
     elif pp_ver == (14, 0):
         gpugen = 'Navi 12'
         from upp.atom_gen import smu_v11_0_navi10 as pp_struct
         ctypes_strct = pp_struct.struct_smu_11_0_powerplay_table
     # Navi 21 (Sienna Cichlid) aka RX6900XT/RX6800(XT)
     # Navi 22 (Navy Flounder) aka RX6700(XT)/RX6800M
     # Navi 23 (Dimgrey Cavefish) aka RX6600(XT)/RX6600M
     # Navi 24 (Beige Goby) aka RX6500(XT)/RX6400
     elif ((pp_ver[0] in [15, 16, 18, 19]) and pp_ver[1] == 0):
         gpugen = 'Navi 2x'
         from upp.atom_gen import smu_v11_0_7_navi20 as pp_struct
         ctypes_strct = pp_struct.struct_smu_11_0_7_powerplay_table
+        enum_structs = {
+            'power_saving_clock': {
+                'prefix': 'SMU_11_0_7_PPCLOCK_',
+                'struct': pp_struct.SMU_11_0_7_PPCLOCK_ID__enumvalues
+            },
+            'overdrive_table': {
+                'prefix': 'SMU_11_0_7_ODSETTING_',
+                'struct': pp_struct.SMU_11_0_7_ODSETTING_ID__enumvalues,
+                'cappfx': 'SMU_11_0_7_ODCAP_',
+                'capstr': pp_struct.SMU_11_0_7_ODFEATURE_CAP__enumvalues,
+            }
+        }
     # Navi 31, 32, 33
     elif ((pp_ver[0] in [20, 21, 22]) and pp_ver[1] == 0):
         gpugen = 'Navi 3x'
         from upp.atom_gen import smu_v13_0_7_navi30 as pp_struct
         ctypes_strct = pp_struct.struct_smu_13_0_7_powerplay_table
+        enum_structs = {
+            'power_saving_clock': {
+                'prefix': 'SMU_13_0_7_PPCLOCK_',
+                'struct': pp_struct.SMU_13_0_7_PPCLOCK_ID__enumvalues
+            },
+            'overdrive_table': {
+                'prefix': 'SMU_13_0_7_ODSETTING_',
+                'struct': pp_struct.SMU_13_0_7_ODSETTING_ID__enumvalues,
+                'cappfx': 'SMU_13_0_7_ODCAP_',
+                'capstr': pp_struct.SMU_13_0_7_ODFEATURE_CAP__enumvalues,
+            }
+        }
     elif pp_ver is not None:
         msg = 'Can not decode PowerPlay table version {}.{}'
         print(msg.format(pp_ver[0], pp_ver[1]))
         return None
     else:
         return None
 
+    # Unpack and sanitize enm_structs, if any
+    if enum_structs:
+        for tbl in enum_structs:
+            prefix = enum_structs[tbl].pop('prefix')
+            for enum in enum_structs[tbl]['struct']:
+                txt = enum_structs[tbl]['struct'][enum]
+                enum_structs[tbl]['struct'][enum] = txt.replace(prefix, '')
+            enum_structs[tbl]['enum'] = enum_structs[tbl]['struct']
+            enum_structs[tbl].pop('struct')
+            if 'capstr' in enum_structs[tbl]:
+                cappfx = enum_structs[tbl].pop('cappfx')
+                for cap in enum_structs[tbl]['capstr']:
+                    cpt = enum_structs[tbl]['capstr'][cap]
+                    enum_structs[tbl]['capstr'][cap] = cpt.replace(cappfx, '')
+                enum_structs[tbl]['cap'] = enum_structs[tbl]['capstr']
+                enum_structs[tbl].pop('capstr')
+        if debug:
+            print('DEBUG: unpacked enumeration data:')
+            for table in enum_structs:
+                print('  min/max enum in', table, enum_structs[tbl]['enum'])
+                if 'cap' in enum_structs[table]:
+                    print('  cap enum in', table, enum_structs[tbl]['cap'])
+
     if debug:
         print('DEBUG: This is a', gpugen,
               'PP table, using', pp_struct.__name__)
 
     data = decode_pp_table(rawbytes, ctypes_strct)
-    data_dict = build_data_tree(data, rawbytes, rawdump=rawdump, debug=debug)
+    data_dict = build_data_tree(data, rawbytes, meta={'enum': enum_structs},
+                                rawdump=rawdump, debug=debug)
     return data_dict
 
 
 def dump_pp_table(pp_bin_file, data_dict=None, indent=0, parent='',
                   rawdump=False, debug=False):
     """
     Prints all decoded PowerPlay parameters and their values to console
@@ -720,15 +802,20 @@
             name = str(parent) + ' ' + str(member)
         if data_dict[member] is None:
             print('{}{}: UNUSED'.format(' '*indent, member))
         elif 'value' in data_dict[member]:
             msg = '{}{}: {}'
             if data_dict[member]['type'] == 'f':
                 msg = '{}{}:{: n}'
-            print(msg.format(' '*indent, name, data_dict[member]['value']))
+            desc = ''
+            if 'desc' in data_dict[member]:
+                desc = '(' + data_dict[member]['desc'] + ')'
+                msg = '{}{}: {} {}'
+            print(msg.format(' '*indent, name,
+                             data_dict[member]['value'], desc))
         else:
             print('{}{}:'.format(' '*indent, name))
             dump_pp_table(None, data_dict[member], indent+2, parent=member)
 
 
 def get_value(pp_bin_file, var_path, data_dict=None, debug=False):
     """
```

### Comparing `upp-0.2.0/src/upp/upp.py` & `upp-0.2.1/src/upp/upp.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/src/upp.egg-info/PKG-INFO` & `upp-0.2.1/src/upp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upp
-Version: 0.2.0
+Version: 0.2.1
 Summary: Uplift Power Play
 Home-page: https://github.com/sibradzic/upp
 Author: Samir Ibradžić
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `upp-0.2.0/src/upp.egg-info/SOURCES.txt` & `upp-0.2.1/src/upp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/test/AMD.RX480.8192.160603.rom.dump` & `upp-0.2.1/test/AMD.RX480.8192.160603.rom.dump`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/test/AMD.RX480.8192.160603.rom.rawdump` & `upp-0.2.1/test/AMD.RX480.8192.160603.rom.rawdump`

 * *Files 0% similar despite different names*

```diff
@@ -1,418 +1,418 @@
 PowerPlay table rev 7.1 size 820 bytes
- Offset (dec.) t Raw val. Variable name                   Decoded value
------------------------------------------------------------------------
- 0x0000 (0000) H     3403 StructureSize                   : 820
- 0x0002 (0002) B       07 TableFormatRevision             : 7
- 0x0003 (0003) B       01 TableContentRevision            : 1
- 0x0004 (0004) B       00 TableRevision                   : 0
- 0x0005 (0005) H     4d00 TableSize                       : 77
- 0x0007 (0007) I 0a060000 GoldenPPID                      : 1546
- 0x000b (0011) I 3b240000 GoldenRevision                  : 9275
- 0x000f (0015) H     1900 FormatID                        : 25
- 0x0011 (0017) H     0000 VoltageTime                     : 0
- 0x0013 (0019) I 00800201 PlatformCaps                    : 16941056
- 0x0017 (0023) I 400d0300 MaxODEngineClock                : 200000
- 0x001b (0027) I e86e0300 MaxODMemoryClock                : 225000
- 0x001f (0031) H     3200 PowerControlLimit               : 50
- 0x0021 (0033) H     3200 UlvVoltageOffset                : 50
- 0x0023 (0035) H     4d00 StateArrayOffset                : 77
- 0x004d (0077) B       01 RevId                           : 1
- 0x004e (0078) B       02 NumEntries                      : 2
- 0x004f (0079) B       00 EngineClockIndexHigh            : 0
- 0x0050 (0080) B       00 EngineClockIndexLow             : 0
- 0x0051 (0081) B       00 MemoryClockIndexHigh            : 0
- 0x0052 (0082) B       00 MemoryClockIndexLow             : 0
- 0x0053 (0083) B       00 PCIEGenLow                      : 0
- 0x0054 (0084) B       00 PCIEGenHigh                     : 0
- 0x0055 (0085) B       00 PCIELaneLow                     : 0
- 0x0056 (0086) B       00 PCIELaneHigh                    : 0
- 0x0057 (0087) H     0800 Classification                  : 8
- 0x0059 (0089) I 00000000 CapsAndSettings                 : 0
- 0x005d (0093) H     0000 Classification2                 : 0
- 0x005f (0095) B       00 Unused                          : 0
- 0x0060 (0096) B       00 Unused                          : 0
- 0x0061 (0097) B       00 Unused                          : 0
- 0x0062 (0098) B       00 Unused                          : 0
- 0x0063 (0099) B       07 EngineClockIndexHigh            : 7
- 0x0064 (0100) B       00 EngineClockIndexLow             : 0
- 0x0065 (0101) B       01 MemoryClockIndexHigh            : 1
- 0x0066 (0102) B       00 MemoryClockIndexLow             : 0
- 0x0067 (0103) B       00 PCIEGenLow                      : 0
- 0x0068 (0104) B       00 PCIEGenHigh                     : 0
- 0x0069 (0105) B       00 PCIELaneLow                     : 0
- 0x006a (0106) B       00 PCIELaneHigh                    : 0
- 0x006b (0107) H     0500 Classification                  : 5
- 0x006d (0109) I 00000000 CapsAndSettings                 : 0
- 0x0071 (0113) H     0000 Classification2                 : 0
- 0x0073 (0115) B       00 Unused                          : 0
- 0x0074 (0116) B       00 Unused                          : 0
- 0x0075 (0117) B       00 Unused                          : 0
- 0x0076 (0118) B       00 Unused                          : 0
- 0x0025 (0037) H     9402 FanTableOffset                  : 660
- 0x0294 (0660) B       09 RevId                           : 9
- 0x0295 (0661) B       03 THyst                           : 3
- 0x0296 (0662) H     a00f TMin                            : 4000
- 0x0298 (0664) H     6419 TMed                            : 6500
- 0x029a (0666) H     3421 THigh                           : 8500
- 0x029c (0668) H     d007 PWMMin                          : 2000
- 0x029e (0670) H     a00f PWMMed                          : 4000
- 0x02a0 (0672) H     7017 PWMHigh                         : 6000
- 0x02a2 (0674) H     942a TMax                            : 10900
- 0x02a4 (0676) B       01 FanControlMode                  : 1
- 0x02a5 (0677) H     6400 FanPWMMax                       : 100
- 0x02a7 (0679) H     e412 FanOutputSensitivity            : 4836
- 0x02a9 (0681) H     9808 FanRPMMax                       : 2200
- 0x02ab (0683) I 78630100 MinFanSCLKAcousticLimit         : 91000
- 0x02af (0687) B       50 TargetTemperature               : 80
- 0x02b0 (0688) B       14 MinimumPWMLimit                 : 20
- 0x02b1 (0689) H     6400 FanGainEdge                     : 100
- 0x02b3 (0691) H     6400 FanGainHotspot                  : 100
- 0x02b5 (0693) H     6400 FanGainLiquid                   : 100
- 0x02b7 (0695) H     6400 FanGainVrVddc                   : 100
- 0x02b9 (0697) H     6400 FanGainVrMvdd                   : 100
- 0x02bb (0699) H     6400 FanGainPlx                      : 100
- 0x02bd (0701) H     6400 FanGainHbm                      : 100
- 0x02bf (0703) B       00 EnableZeroRPM                   : 0
- 0x02c0 (0704) B       32 FanStopTemperature              : 50
- 0x02c1 (0705) B       3c FanStartTemperature             : 60
- 0x02c2 (0706) H     0000 Reserved                        : 0
- 0x0027 (0039) H     8b02 ThermalControllerOffset         : 651
- 0x028b (0651) B       01 RevId                           : 1
- 0x028c (0652) B       17 Type                            : 23
- 0x028d (0653) B       00 I2cLine                         : 0
- 0x028e (0654) B       00 I2cAddress                      : 0
- 0x028f (0655) B       02 FanParameters                   : 2
- 0x0290 (0656) B       00 FanMinRPM                       : 0
- 0x0291 (0657) B       34 FanMaxRPM                       : 52
- 0x0292 (0658) B       00 Reserved                        : 0
- 0x0293 (0659) B       00 Flags                           : 0
- 0x0029 (0041) H     0000 Reserv                          : 0
- 0x002b (0043) H     b501 MclkDependencyTableOffset       : 437
- 0x01b5 (0437) B       00 RevId                           : 0
- 0x01b6 (0438) B       02 NumEntries                      : 2
- 0x01b7 (0439) B       00 VddcInd                         : 0
- 0x01b8 (0440) H     5203 Vddci                           : 850
- 0x01ba (0442) H     0000 VddgfxOffset                    : 0
- 0x01bc (0444) H     e803 Mvdd                            : 1000
- 0x01be (0446) I 30750000 Mclk                            : 30000
- 0x01c2 (0450) H     0000 Reserved                        : 0
- 0x01c4 (0452) B       0f VddcInd                         : 15
- 0x01c5 (0453) H     b603 Vddci                           : 950
- 0x01c7 (0455) H     0000 VddgfxOffset                    : 0
- 0x01c9 (0457) H     e803 Mvdd                            : 1000
- 0x01cb (0459) I 400d0300 Mclk                            : 200000
- 0x01cf (0463) H     0000 Reserved                        : 0
- 0x002d (0045) H     3b01 SclkDependencyTableOffset       : 315
- 0x013b (0315) B       01 RevId                           : 1
- 0x013c (0316) B       08 NumEntries                      : 8
- 0x013d (0317) B       00 VddInd                          : 0
- 0x013e (0318) H     0000 VddcOffset                      : 0
- 0x0140 (0320) I 30750000 Sclk                            : 30000
- 0x0144 (0324) H     0000 EdcCurrent                      : 0
- 0x0146 (0326) B       00 ReliabilityTemperature          : 0
- 0x0147 (0327) B       80 CKSVOffsetandDisable            : 128
- 0x0148 (0328) I 00000000 SclkOffset                      : 0
- 0x014c (0332) B       01 VddInd                          : 1
- 0x014d (0333) H     e6ff VddcOffset                      : 65510
- 0x014f (0335) I 80ed0000 Sclk                            : 60800
- 0x0153 (0339) H     0000 EdcCurrent                      : 0
- 0x0155 (0341) B       00 ReliabilityTemperature          : 0
- 0x0156 (0342) B       00 CKSVOffsetandDisable            : 0
- 0x0157 (0343) I 00000000 SclkOffset                      : 0
- 0x015b (0347) B       02 VddInd                          : 2
- 0x015c (0348) H     e6ff VddcOffset                      : 65510
- 0x015e (0350) I 78630100 Sclk                            : 91000
- 0x0162 (0354) H     0000 EdcCurrent                      : 0
- 0x0164 (0356) B       00 ReliabilityTemperature          : 0
- 0x0165 (0357) B       00 CKSVOffsetandDisable            : 0
- 0x0166 (0358) I 88130000 SclkOffset                      : 5000
- 0x016a (0362) B       03 VddInd                          : 3
- 0x016b (0363) H     e6ff VddcOffset                      : 65510
- 0x016d (0365) I b4a40100 Sclk                            : 107700
- 0x0171 (0369) H     0000 EdcCurrent                      : 0
- 0x0173 (0371) B       00 ReliabilityTemperature          : 0
- 0x0174 (0372) B       00 CKSVOffsetandDisable            : 0
- 0x0175 (0373) I 00000000 SclkOffset                      : 0
- 0x0179 (0377) B       04 VddInd                          : 4
- 0x017a (0378) H     e6ff VddcOffset                      : 65510
- 0x017c (0380) I 44bf0100 Sclk                            : 114500
- 0x0180 (0384) H     0000 EdcCurrent                      : 0
- 0x0182 (0386) B       00 ReliabilityTemperature          : 0
- 0x0183 (0387) B       00 CKSVOffsetandDisable            : 0
- 0x0184 (0388) I 00000000 SclkOffset                      : 0
- 0x0188 (0392) B       05 VddInd                          : 5
- 0x0189 (0393) H     e6ff VddcOffset                      : 65510
- 0x018b (0395) I 3cd10100 Sclk                            : 119100
- 0x018f (0399) H     0000 EdcCurrent                      : 0
- 0x0191 (0401) B       00 ReliabilityTemperature          : 0
- 0x0192 (0402) B       00 CKSVOffsetandDisable            : 0
- 0x0193 (0403) I 00000000 SclkOffset                      : 0
- 0x0197 (0407) B       06 VddInd                          : 6
- 0x0198 (0408) H     e6ff VddcOffset                      : 65510
- 0x019a (0410) I d0e20100 Sclk                            : 123600
- 0x019e (0414) H     0000 EdcCurrent                      : 0
- 0x01a0 (0416) B       00 ReliabilityTemperature          : 0
- 0x01a1 (0417) B       00 CKSVOffsetandDisable            : 0
- 0x01a2 (0418) I 00000000 SclkOffset                      : 0
- 0x01a6 (0422) B       07 VddInd                          : 7
- 0x01a7 (0423) H     0000 VddcOffset                      : 0
- 0x01a9 (0425) I 88ee0100 Sclk                            : 126600
- 0x01ad (0429) H     0000 EdcCurrent                      : 0
- 0x01af (0431) B       00 ReliabilityTemperature          : 0
- 0x01b0 (0432) B       00 CKSVOffsetandDisable            : 0
- 0x01b1 (0433) I 00000000 SclkOffset                      : 0
- 0x002f (0047) H     7700 VddcLookupTableOffset           : 119
- 0x0077 (0119) B       00 RevId                           : 0
- 0x0078 (0120) B       10 NumEntries                      : 16
- 0x0079 (0121) H     2003 Vdd                             : 800
- 0x007b (0123) H     0000 CACLow                          : 0
- 0x007d (0125) H     0000 CACMid                          : 0
- 0x007f (0127) H     0000 CACHigh                         : 0
- 0x0081 (0129) H     02ff Vdd                             : 65282
- 0x0083 (0131) H     0000 CACLow                          : 0
- 0x0085 (0133) H     0000 CACMid                          : 0
- 0x0087 (0135) H     0000 CACHigh                         : 0
- 0x0089 (0137) H     03ff Vdd                             : 65283
- 0x008b (0139) H     0000 CACLow                          : 0
- 0x008d (0141) H     0000 CACMid                          : 0
- 0x008f (0143) H     0000 CACHigh                         : 0
- 0x0091 (0145) H     04ff Vdd                             : 65284
- 0x0093 (0147) H     0000 CACLow                          : 0
- 0x0095 (0149) H     0000 CACMid                          : 0
- 0x0097 (0151) H     0000 CACHigh                         : 0
- 0x0099 (0153) H     05ff Vdd                             : 65285
- 0x009b (0155) H     0000 CACLow                          : 0
- 0x009d (0157) H     0000 CACMid                          : 0
- 0x009f (0159) H     0000 CACHigh                         : 0
- 0x00a1 (0161) H     06ff Vdd                             : 65286
- 0x00a3 (0163) H     0000 CACLow                          : 0
- 0x00a5 (0165) H     0000 CACMid                          : 0
- 0x00a7 (0167) H     0000 CACHigh                         : 0
- 0x00a9 (0169) H     07ff Vdd                             : 65287
- 0x00ab (0171) H     0000 CACLow                          : 0
- 0x00ad (0173) H     0000 CACMid                          : 0
- 0x00af (0175) H     0000 CACHigh                         : 0
- 0x00b1 (0177) H     08ff Vdd                             : 65288
- 0x00b3 (0179) H     0000 CACLow                          : 0
- 0x00b5 (0181) H     0000 CACMid                          : 0
- 0x00b7 (0183) H     0000 CACHigh                         : 0
- 0x00b9 (0185) H     5203 Vdd                             : 850
- 0x00bb (0187) H     0000 CACLow                          : 0
- 0x00bd (0189) H     0000 CACMid                          : 0
- 0x00bf (0191) H     0000 CACHigh                         : 0
- 0x00c1 (0193) H     8403 Vdd                             : 900
- 0x00c3 (0195) H     0000 CACLow                          : 0
- 0x00c5 (0197) H     0000 CACMid                          : 0
- 0x00c7 (0199) H     0000 CACHigh                         : 0
- 0x00c9 (0201) H     b603 Vdd                             : 950
- 0x00cb (0203) H     0000 CACLow                          : 0
- 0x00cd (0205) H     0000 CACMid                          : 0
- 0x00cf (0207) H     0000 CACHigh                         : 0
- 0x00d1 (0209) H     e803 Vdd                             : 1000
- 0x00d3 (0211) H     0000 CACLow                          : 0
- 0x00d5 (0213) H     0000 CACMid                          : 0
- 0x00d7 (0215) H     0000 CACHigh                         : 0
- 0x00d9 (0217) H     1a04 Vdd                             : 1050
- 0x00db (0219) H     0000 CACLow                          : 0
- 0x00dd (0221) H     0000 CACMid                          : 0
- 0x00df (0223) H     0000 CACHigh                         : 0
- 0x00e1 (0225) H     4c04 Vdd                             : 1100
- 0x00e3 (0227) H     0000 CACLow                          : 0
- 0x00e5 (0229) H     0000 CACMid                          : 0
- 0x00e7 (0231) H     0000 CACHigh                         : 0
- 0x00e9 (0233) H     7e04 Vdd                             : 1150
- 0x00eb (0235) H     0000 CACLow                          : 0
- 0x00ed (0237) H     0000 CACMid                          : 0
- 0x00ef (0239) H     0000 CACHigh                         : 0
- 0x00f1 (0241) H     cf03 Vdd                             : 975
- 0x00f3 (0243) H     0000 CACLow                          : 0
- 0x00f5 (0245) H     0000 CACMid                          : 0
- 0x00f7 (0247) H     0000 CACHigh                         : 0
- 0x0031 (0049) H     f900 VddgfxLookupTableOffset         : 249
- 0x00f9 (0249) B       00 RevId                           : 0
- 0x00fa (0250) B       08 NumEntries                      : 8
- 0x00fb (0251) H     8403 Vdd                             : 900
- 0x00fd (0253) H     0000 CACLow                          : 0
- 0x00ff (0255) H     0000 CACMid                          : 0
- 0x0101 (0257) H     0000 CACHigh                         : 0
- 0x0103 (0259) H     02ff Vdd                             : 65282
- 0x0105 (0261) H     0000 CACLow                          : 0
- 0x0107 (0263) H     0000 CACMid                          : 0
- 0x0109 (0265) H     0000 CACHigh                         : 0
- 0x010b (0267) H     03ff Vdd                             : 65283
- 0x010d (0269) H     0000 CACLow                          : 0
- 0x010f (0271) H     0000 CACMid                          : 0
- 0x0111 (0273) H     0000 CACHigh                         : 0
- 0x0113 (0275) H     04ff Vdd                             : 65284
- 0x0115 (0277) H     0000 CACLow                          : 0
- 0x0117 (0279) H     0000 CACMid                          : 0
- 0x0119 (0281) H     0000 CACHigh                         : 0
- 0x011b (0283) H     05ff Vdd                             : 65285
- 0x011d (0285) H     0000 CACLow                          : 0
- 0x011f (0287) H     0000 CACMid                          : 0
- 0x0121 (0289) H     0000 CACHigh                         : 0
- 0x0123 (0291) H     06ff Vdd                             : 65286
- 0x0125 (0293) H     0000 CACLow                          : 0
- 0x0127 (0295) H     0000 CACMid                          : 0
- 0x0129 (0297) H     0000 CACHigh                         : 0
- 0x012b (0299) H     07ff Vdd                             : 65287
- 0x012d (0301) H     0000 CACLow                          : 0
- 0x012f (0303) H     0000 CACMid                          : 0
- 0x0131 (0305) H     0000 CACHigh                         : 0
- 0x0133 (0307) H     08ff Vdd                             : 65288
- 0x0135 (0309) H     0000 CACLow                          : 0
- 0x0137 (0311) H     0000 CACMid                          : 0
- 0x0139 (0313) H     0000 CACHigh                         : 0
- 0x0033 (0051) H     d101 MMDependencyTableOffset         : 465
- 0x01d1 (0465) B       00 RevId                           : 0
- 0x01d2 (0466) B       08 NumEntries                      : 8
- 0x01d3 (0467) B       00 VddcInd                         : 0
- 0x01d4 (0468) H     0000 VddgfxOffset                    : 0
- 0x01d6 (0470) I 90e20000 DClk                            : 58000
- 0x01da (0474) I f8240100 VClk                            : 75000
- 0x01de (0478) I 18f60000 EClk                            : 63000
- 0x01e2 (0482) I 00000000 AClk                            : 0
- 0x01e6 (0486) I a8de0000 SAMUClk                         : 57000
- 0x01ea (0490) B       08 VddcInd                         : 8
- 0x01eb (0491) H     b4ff VddgfxOffset                    : 65460
- 0x01ed (0493) I 18f60000 DClk                            : 63000
- 0x01f1 (0497) I 80380100 VClk                            : 80000
- 0x01f5 (0501) I 880d0100 EClk                            : 69000
- 0x01f9 (0505) I 00000000 AClk                            : 0
- 0x01fd (0509) I 00fa0000 SAMUClk                         : 64000
- 0x0201 (0513) B       09 VddcInd                         : 9
- 0x0202 (0514) H     9bff VddgfxOffset                    : 65435
- 0x0204 (0516) I a0090100 DClk                            : 68000
- 0x0208 (0520) I 084c0100 VClk                            : 85000
- 0x020c (0524) I f8240100 EClk                            : 75000
- 0x0210 (0528) I 00000000 AClk                            : 0
- 0x0214 (0532) I 70110100 SAMUClk                         : 70000
- 0x0218 (0536) B       0a VddcInd                         : 10
- 0x0219 (0537) H     82ff VddgfxOffset                    : 65410
- 0x021b (0539) I 281d0100 DClk                            : 73000
- 0x021f (0543) I a85b0100 VClk                            : 89000
- 0x0223 (0547) I 683c0100 EClk                            : 81000
- 0x0227 (0551) I 00000000 AClk                            : 0
- 0x022b (0555) I e0280100 SAMUClk                         : 76000
- 0x022f (0559) B       0b VddcInd                         : 11
- 0x0230 (0560) H     69ff VddgfxOffset                    : 65385
- 0x0232 (0562) I c82c0100 DClk                            : 77000
- 0x0236 (0566) I 60670100 VClk                            : 92000
- 0x023a (0570) I f04f0100 EClk                            : 86000
- 0x023e (0574) I 00000000 AClk                            : 0
- 0x0242 (0578) I 683c0100 SAMUClk                         : 81000
- 0x0246 (0582) B       0c VddcInd                         : 12
- 0x0247 (0583) H     37ff VddgfxOffset                    : 65335
- 0x0249 (0585) I 80380100 DClk                            : 80000
- 0x024d (0589) I 18730100 VClk                            : 95000
- 0x0251 (0593) I 78630100 EClk                            : 91000
- 0x0255 (0597) I 00000000 AClk                            : 0
- 0x0259 (0601) I 084c0100 SAMUClk                         : 85000
- 0x025d (0605) B       0d VddcInd                         : 13
- 0x025e (0606) H     05ff VddgfxOffset                    : 65285
- 0x0260 (0608) I 38440100 DClk                            : 83000
- 0x0264 (0612) I d07e0100 VClk                            : 98000
- 0x0268 (0616) I 00770100 EClk                            : 96000
- 0x026c (0620) I 00000000 AClk                            : 0
- 0x0270 (0624) I c0570100 SAMUClk                         : 88000
- 0x0274 (0628) B       0e VddcInd                         : 14
- 0x0275 (0629) H     0000 VddgfxOffset                    : 0
- 0x0277 (0631) I f04f0100 DClk                            : 86000
- 0x027b (0635) I a0860100 VClk                            : 100000
- 0x027f (0639) I a0860100 EClk                            : 100000
- 0x0283 (0643) I 00000000 AClk                            : 0
- 0x0287 (0647) I 78630100 SAMUClk                         : 91000
- 0x0035 (0053) H     f902 VCEStateTableOffset             : 761
- 0x02f9 (0761) B       01 RevId                           : 1
- 0x02fa (0762) B       06 NumEntries                      : 6
- 0x02fb (0763) B       00 VCEClockIndex                   : 0
- 0x02fc (0764) B       00 Flag                            : 0
- 0x02fd (0765) B       01 SCLKIndex                       : 1
- 0x02fe (0766) B       01 MCLKIndex                       : 1
- 0x02ff (0767) B       00 VCEClockIndex                   : 0
- 0x0300 (0768) B       01 Flag                            : 1
- 0x0301 (0769) B       01 SCLKIndex                       : 1
- 0x0302 (0770) B       01 MCLKIndex                       : 1
- 0x0303 (0771) B       00 VCEClockIndex                   : 0
- 0x0304 (0772) B       02 Flag                            : 2
- 0x0305 (0773) B       01 SCLKIndex                       : 1
- 0x0306 (0774) B       01 MCLKIndex                       : 1
- 0x0307 (0775) B       00 VCEClockIndex                   : 0
- 0x0308 (0776) B       02 Flag                            : 2
- 0x0309 (0777) B       01 SCLKIndex                       : 1
- 0x030a (0778) B       01 MCLKIndex                       : 1
- 0x030b (0779) B       00 VCEClockIndex                   : 0
- 0x030c (0780) B       02 Flag                            : 2
- 0x030d (0781) B       01 SCLKIndex                       : 1
- 0x030e (0782) B       01 MCLKIndex                       : 1
- 0x030f (0783) B       00 VCEClockIndex                   : 0
- 0x0310 (0784) B       02 Flag                            : 2
- 0x0311 (0785) B       01 SCLKIndex                       : 1
- 0x0312 (0786) B       01 MCLKIndex                       : 1
- 0x0037 (0055) H     0000 PPMTableOffset                  : 0
- 0x0039 (0057) H     c402 PowerTuneTableOffset            : 708
- 0x02c4 (0708) B       04 RevId                           : 4
- 0x02c5 (0709) H     6e00 TDP                             : 110
- 0x02c7 (0711) H     0000 ConfigurableTDP                 : 0
- 0x02c9 (0713) H     6b00 TDC                             : 107
- 0x02cb (0715) H     6e00 BatteryPowerLimit               : 110
- 0x02cd (0717) H     6e00 SmallPowerLimit                 : 110
- 0x02cf (0719) H     0000 LowCACLeakage                   : 0
- 0x02d1 (0721) H     0000 HighCACLeakage                  : 0
- 0x02d3 (0723) H     6e00 MaximumPowerDeliveryLimit       : 110
- 0x02d5 (0725) H     5a00 TjMax                           : 90
- 0x02d7 (0727) H     0000 PowerTuneDataSetID              : 0
- 0x02d9 (0729) H     0000 EDCLimit                        : 0
- 0x02db (0731) H     5e00 SoftwareShutdownTemp            : 94
- 0x02dd (0733) H     0200 ClockStretchAmount              : 2
- 0x02df (0735) H     6900 TemperatureLimitHotspot         : 105
- 0x02e1 (0737) H     5000 TemperatureLimitLiquid1         : 80
- 0x02e3 (0739) H     5000 TemperatureLimitLiquid2         : 80
- 0x02e5 (0741) H     7300 TemperatureLimitVrVddc          : 115
- 0x02e7 (0743) H     7300 TemperatureLimitVrMvdd          : 115
- 0x02e9 (0745) H     5f00 TemperatureLimitPlx             : 95
- 0x02eb (0747) B       00 Liquid1_I2C_address             : 0
- 0x02ec (0748) B       00 Liquid2_I2C_address             : 0
- 0x02ed (0749) B       90 Liquid_I2C_Line                 : 144
- 0x02ee (0750) B       10 Vr_I2C_address                  : 16
- 0x02ef (0751) B       96 Vr_I2C_Line                     : 150
- 0x02f0 (0752) B       00 Plx_I2C_address                 : 0
- 0x02f1 (0753) B       90 Plx_I2C_Line                    : 144
- 0x02f2 (0754) H     0000 BoostPowerLimit                 : 0
- 0x02f4 (0756) B       06 CKS_LDO_REFSEL                  : 6
- 0x02f5 (0757) B       00 HotSpotOnly                     : 0
- 0x02f6 (0758) B       00 Reserve                         : 0
- 0x02f7 (0759) H     0000 Reserve                         : 0
- 0x003b (0059) H     0000 HardLimitTableOffset            : 0
- 0x003d (0061) H     1303 PCIETableOffset                 : 787
- 0x0313 (0787) B       01 RevId                           : 1
- 0x0314 (0788) B       03 NumEntries                      : 3
- 0x0315 (0789) B       00 PCIEGenSpeed                    : 0
- 0x0316 (0790) B       10 PCIELaneWidth                   : 16
- 0x0317 (0791) B       00 Reserved                        : 0
- 0x0318 (0792) B       00 Reserved                        : 0
- 0x0319 (0793) I 00000000 PCIE_Sclk                       : 0
- 0x031d (0797) B       00 PCIEGenSpeed                    : 0
- 0x031e (0798) B       10 PCIELaneWidth                   : 16
- 0x031f (0799) B       00 Reserved                        : 0
- 0x0320 (0800) B       00 Reserved                        : 0
- 0x0321 (0801) I 00000000 PCIE_Sclk                       : 0
- 0x0325 (0805) B       02 PCIEGenSpeed                    : 2
- 0x0326 (0806) B       10 PCIELaneWidth                   : 16
- 0x0327 (0807) B       00 Reserved                        : 0
- 0x0328 (0808) B       00 Reserved                        : 0
- 0x0329 (0809) I 00000000 PCIE_Sclk                       : 0
- 0x003f (0063) H     2d03 GPIOTableOffset                 : 813
- 0x032d (0813) B       00 RevId                           : 0
- 0x032e (0814) B       01 VRHotTriggeredSclkDpmIndex      : 1
- 0x032f (0815) B       00 Reserve                         : 0
- 0x0330 (0816) B       00 Reserve                         : 0
- 0x0331 (0817) B       00 Reserve                         : 0
- 0x0332 (0818) B       00 Reserve                         : 0
- 0x0333 (0819) B       00 Reserve                         : 0
- 0x0041 (0065) H     0000 Reserved                        : 0
- 0x0043 (0067) H     0000 Reserved                        : 0
- 0x0045 (0069) H     0000 Reserved                        : 0
- 0x0047 (0071) H     0000 Reserved                        : 0
- 0x0049 (0073) H     0000 Reserved                        : 0
- 0x004b (0075) H     0000 Reserved                        : 0
+ Offset (dec.) t Raw val. Variable name                         Decoded value
+------------------------------------------------------------------------------
+ 0x0000 (0000) H     3403 StructureSize                             : 820
+ 0x0002 (0002) B       07 TableFormatRevision                       : 7
+ 0x0003 (0003) B       01 TableContentRevision                      : 1
+ 0x0004 (0004) B       00 TableRevision                             : 0
+ 0x0005 (0005) H     4d00 TableSize                                 : 77
+ 0x0007 (0007) I 0a060000 GoldenPPID                                : 1546
+ 0x000b (0011) I 3b240000 GoldenRevision                            : 9275
+ 0x000f (0015) H     1900 FormatID                                  : 25
+ 0x0011 (0017) H     0000 VoltageTime                               : 0
+ 0x0013 (0019) I 00800201 PlatformCaps                              : 16941056
+ 0x0017 (0023) I 400d0300 MaxODEngineClock                          : 200000
+ 0x001b (0027) I e86e0300 MaxODMemoryClock                          : 225000
+ 0x001f (0031) H     3200 PowerControlLimit                         : 50
+ 0x0021 (0033) H     3200 UlvVoltageOffset                          : 50
+ 0x0023 (0035) H     4d00 StateArrayOffset                          : 77
+ 0x004d (0077) B       01 RevId                                     : 1
+ 0x004e (0078) B       02 NumEntries                                : 2
+ 0x004f (0079) B       00 EngineClockIndexHigh                      : 0
+ 0x0050 (0080) B       00 EngineClockIndexLow                       : 0
+ 0x0051 (0081) B       00 MemoryClockIndexHigh                      : 0
+ 0x0052 (0082) B       00 MemoryClockIndexLow                       : 0
+ 0x0053 (0083) B       00 PCIEGenLow                                : 0
+ 0x0054 (0084) B       00 PCIEGenHigh                               : 0
+ 0x0055 (0085) B       00 PCIELaneLow                               : 0
+ 0x0056 (0086) B       00 PCIELaneHigh                              : 0
+ 0x0057 (0087) H     0800 Classification                            : 8
+ 0x0059 (0089) I 00000000 CapsAndSettings                           : 0
+ 0x005d (0093) H     0000 Classification2                           : 0
+ 0x005f (0095) B       00 Unused                                    : 0
+ 0x0060 (0096) B       00 Unused                                    : 0
+ 0x0061 (0097) B       00 Unused                                    : 0
+ 0x0062 (0098) B       00 Unused                                    : 0
+ 0x0063 (0099) B       07 EngineClockIndexHigh                      : 7
+ 0x0064 (0100) B       00 EngineClockIndexLow                       : 0
+ 0x0065 (0101) B       01 MemoryClockIndexHigh                      : 1
+ 0x0066 (0102) B       00 MemoryClockIndexLow                       : 0
+ 0x0067 (0103) B       00 PCIEGenLow                                : 0
+ 0x0068 (0104) B       00 PCIEGenHigh                               : 0
+ 0x0069 (0105) B       00 PCIELaneLow                               : 0
+ 0x006a (0106) B       00 PCIELaneHigh                              : 0
+ 0x006b (0107) H     0500 Classification                            : 5
+ 0x006d (0109) I 00000000 CapsAndSettings                           : 0
+ 0x0071 (0113) H     0000 Classification2                           : 0
+ 0x0073 (0115) B       00 Unused                                    : 0
+ 0x0074 (0116) B       00 Unused                                    : 0
+ 0x0075 (0117) B       00 Unused                                    : 0
+ 0x0076 (0118) B       00 Unused                                    : 0
+ 0x0025 (0037) H     9402 FanTableOffset                            : 660
+ 0x0294 (0660) B       09 RevId                                     : 9
+ 0x0295 (0661) B       03 THyst                                     : 3
+ 0x0296 (0662) H     a00f TMin                                      : 4000
+ 0x0298 (0664) H     6419 TMed                                      : 6500
+ 0x029a (0666) H     3421 THigh                                     : 8500
+ 0x029c (0668) H     d007 PWMMin                                    : 2000
+ 0x029e (0670) H     a00f PWMMed                                    : 4000
+ 0x02a0 (0672) H     7017 PWMHigh                                   : 6000
+ 0x02a2 (0674) H     942a TMax                                      : 10900
+ 0x02a4 (0676) B       01 FanControlMode                            : 1
+ 0x02a5 (0677) H     6400 FanPWMMax                                 : 100
+ 0x02a7 (0679) H     e412 FanOutputSensitivity                      : 4836
+ 0x02a9 (0681) H     9808 FanRPMMax                                 : 2200
+ 0x02ab (0683) I 78630100 MinFanSCLKAcousticLimit                   : 91000
+ 0x02af (0687) B       50 TargetTemperature                         : 80
+ 0x02b0 (0688) B       14 MinimumPWMLimit                           : 20
+ 0x02b1 (0689) H     6400 FanGainEdge                               : 100
+ 0x02b3 (0691) H     6400 FanGainHotspot                            : 100
+ 0x02b5 (0693) H     6400 FanGainLiquid                             : 100
+ 0x02b7 (0695) H     6400 FanGainVrVddc                             : 100
+ 0x02b9 (0697) H     6400 FanGainVrMvdd                             : 100
+ 0x02bb (0699) H     6400 FanGainPlx                                : 100
+ 0x02bd (0701) H     6400 FanGainHbm                                : 100
+ 0x02bf (0703) B       00 EnableZeroRPM                             : 0
+ 0x02c0 (0704) B       32 FanStopTemperature                        : 50
+ 0x02c1 (0705) B       3c FanStartTemperature                       : 60
+ 0x02c2 (0706) H     0000 Reserved                                  : 0
+ 0x0027 (0039) H     8b02 ThermalControllerOffset                   : 651
+ 0x028b (0651) B       01 RevId                                     : 1
+ 0x028c (0652) B       17 Type                                      : 23
+ 0x028d (0653) B       00 I2cLine                                   : 0
+ 0x028e (0654) B       00 I2cAddress                                : 0
+ 0x028f (0655) B       02 FanParameters                             : 2
+ 0x0290 (0656) B       00 FanMinRPM                                 : 0
+ 0x0291 (0657) B       34 FanMaxRPM                                 : 52
+ 0x0292 (0658) B       00 Reserved                                  : 0
+ 0x0293 (0659) B       00 Flags                                     : 0
+ 0x0029 (0041) H     0000 Reserv                                    : 0
+ 0x002b (0043) H     b501 MclkDependencyTableOffset                 : 437
+ 0x01b5 (0437) B       00 RevId                                     : 0
+ 0x01b6 (0438) B       02 NumEntries                                : 2
+ 0x01b7 (0439) B       00 VddcInd                                   : 0
+ 0x01b8 (0440) H     5203 Vddci                                     : 850
+ 0x01ba (0442) H     0000 VddgfxOffset                              : 0
+ 0x01bc (0444) H     e803 Mvdd                                      : 1000
+ 0x01be (0446) I 30750000 Mclk                                      : 30000
+ 0x01c2 (0450) H     0000 Reserved                                  : 0
+ 0x01c4 (0452) B       0f VddcInd                                   : 15
+ 0x01c5 (0453) H     b603 Vddci                                     : 950
+ 0x01c7 (0455) H     0000 VddgfxOffset                              : 0
+ 0x01c9 (0457) H     e803 Mvdd                                      : 1000
+ 0x01cb (0459) I 400d0300 Mclk                                      : 200000
+ 0x01cf (0463) H     0000 Reserved                                  : 0
+ 0x002d (0045) H     3b01 SclkDependencyTableOffset                 : 315
+ 0x013b (0315) B       01 RevId                                     : 1
+ 0x013c (0316) B       08 NumEntries                                : 8
+ 0x013d (0317) B       00 VddInd                                    : 0
+ 0x013e (0318) H     0000 VddcOffset                                : 0
+ 0x0140 (0320) I 30750000 Sclk                                      : 30000
+ 0x0144 (0324) H     0000 EdcCurrent                                : 0
+ 0x0146 (0326) B       00 ReliabilityTemperature                    : 0
+ 0x0147 (0327) B       80 CKSVOffsetandDisable                      : 128
+ 0x0148 (0328) I 00000000 SclkOffset                                : 0
+ 0x014c (0332) B       01 VddInd                                    : 1
+ 0x014d (0333) H     e6ff VddcOffset                                : 65510
+ 0x014f (0335) I 80ed0000 Sclk                                      : 60800
+ 0x0153 (0339) H     0000 EdcCurrent                                : 0
+ 0x0155 (0341) B       00 ReliabilityTemperature                    : 0
+ 0x0156 (0342) B       00 CKSVOffsetandDisable                      : 0
+ 0x0157 (0343) I 00000000 SclkOffset                                : 0
+ 0x015b (0347) B       02 VddInd                                    : 2
+ 0x015c (0348) H     e6ff VddcOffset                                : 65510
+ 0x015e (0350) I 78630100 Sclk                                      : 91000
+ 0x0162 (0354) H     0000 EdcCurrent                                : 0
+ 0x0164 (0356) B       00 ReliabilityTemperature                    : 0
+ 0x0165 (0357) B       00 CKSVOffsetandDisable                      : 0
+ 0x0166 (0358) I 88130000 SclkOffset                                : 5000
+ 0x016a (0362) B       03 VddInd                                    : 3
+ 0x016b (0363) H     e6ff VddcOffset                                : 65510
+ 0x016d (0365) I b4a40100 Sclk                                      : 107700
+ 0x0171 (0369) H     0000 EdcCurrent                                : 0
+ 0x0173 (0371) B       00 ReliabilityTemperature                    : 0
+ 0x0174 (0372) B       00 CKSVOffsetandDisable                      : 0
+ 0x0175 (0373) I 00000000 SclkOffset                                : 0
+ 0x0179 (0377) B       04 VddInd                                    : 4
+ 0x017a (0378) H     e6ff VddcOffset                                : 65510
+ 0x017c (0380) I 44bf0100 Sclk                                      : 114500
+ 0x0180 (0384) H     0000 EdcCurrent                                : 0
+ 0x0182 (0386) B       00 ReliabilityTemperature                    : 0
+ 0x0183 (0387) B       00 CKSVOffsetandDisable                      : 0
+ 0x0184 (0388) I 00000000 SclkOffset                                : 0
+ 0x0188 (0392) B       05 VddInd                                    : 5
+ 0x0189 (0393) H     e6ff VddcOffset                                : 65510
+ 0x018b (0395) I 3cd10100 Sclk                                      : 119100
+ 0x018f (0399) H     0000 EdcCurrent                                : 0
+ 0x0191 (0401) B       00 ReliabilityTemperature                    : 0
+ 0x0192 (0402) B       00 CKSVOffsetandDisable                      : 0
+ 0x0193 (0403) I 00000000 SclkOffset                                : 0
+ 0x0197 (0407) B       06 VddInd                                    : 6
+ 0x0198 (0408) H     e6ff VddcOffset                                : 65510
+ 0x019a (0410) I d0e20100 Sclk                                      : 123600
+ 0x019e (0414) H     0000 EdcCurrent                                : 0
+ 0x01a0 (0416) B       00 ReliabilityTemperature                    : 0
+ 0x01a1 (0417) B       00 CKSVOffsetandDisable                      : 0
+ 0x01a2 (0418) I 00000000 SclkOffset                                : 0
+ 0x01a6 (0422) B       07 VddInd                                    : 7
+ 0x01a7 (0423) H     0000 VddcOffset                                : 0
+ 0x01a9 (0425) I 88ee0100 Sclk                                      : 126600
+ 0x01ad (0429) H     0000 EdcCurrent                                : 0
+ 0x01af (0431) B       00 ReliabilityTemperature                    : 0
+ 0x01b0 (0432) B       00 CKSVOffsetandDisable                      : 0
+ 0x01b1 (0433) I 00000000 SclkOffset                                : 0
+ 0x002f (0047) H     7700 VddcLookupTableOffset                     : 119
+ 0x0077 (0119) B       00 RevId                                     : 0
+ 0x0078 (0120) B       10 NumEntries                                : 16
+ 0x0079 (0121) H     2003 Vdd                                       : 800
+ 0x007b (0123) H     0000 CACLow                                    : 0
+ 0x007d (0125) H     0000 CACMid                                    : 0
+ 0x007f (0127) H     0000 CACHigh                                   : 0
+ 0x0081 (0129) H     02ff Vdd                                       : 65282
+ 0x0083 (0131) H     0000 CACLow                                    : 0
+ 0x0085 (0133) H     0000 CACMid                                    : 0
+ 0x0087 (0135) H     0000 CACHigh                                   : 0
+ 0x0089 (0137) H     03ff Vdd                                       : 65283
+ 0x008b (0139) H     0000 CACLow                                    : 0
+ 0x008d (0141) H     0000 CACMid                                    : 0
+ 0x008f (0143) H     0000 CACHigh                                   : 0
+ 0x0091 (0145) H     04ff Vdd                                       : 65284
+ 0x0093 (0147) H     0000 CACLow                                    : 0
+ 0x0095 (0149) H     0000 CACMid                                    : 0
+ 0x0097 (0151) H     0000 CACHigh                                   : 0
+ 0x0099 (0153) H     05ff Vdd                                       : 65285
+ 0x009b (0155) H     0000 CACLow                                    : 0
+ 0x009d (0157) H     0000 CACMid                                    : 0
+ 0x009f (0159) H     0000 CACHigh                                   : 0
+ 0x00a1 (0161) H     06ff Vdd                                       : 65286
+ 0x00a3 (0163) H     0000 CACLow                                    : 0
+ 0x00a5 (0165) H     0000 CACMid                                    : 0
+ 0x00a7 (0167) H     0000 CACHigh                                   : 0
+ 0x00a9 (0169) H     07ff Vdd                                       : 65287
+ 0x00ab (0171) H     0000 CACLow                                    : 0
+ 0x00ad (0173) H     0000 CACMid                                    : 0
+ 0x00af (0175) H     0000 CACHigh                                   : 0
+ 0x00b1 (0177) H     08ff Vdd                                       : 65288
+ 0x00b3 (0179) H     0000 CACLow                                    : 0
+ 0x00b5 (0181) H     0000 CACMid                                    : 0
+ 0x00b7 (0183) H     0000 CACHigh                                   : 0
+ 0x00b9 (0185) H     5203 Vdd                                       : 850
+ 0x00bb (0187) H     0000 CACLow                                    : 0
+ 0x00bd (0189) H     0000 CACMid                                    : 0
+ 0x00bf (0191) H     0000 CACHigh                                   : 0
+ 0x00c1 (0193) H     8403 Vdd                                       : 900
+ 0x00c3 (0195) H     0000 CACLow                                    : 0
+ 0x00c5 (0197) H     0000 CACMid                                    : 0
+ 0x00c7 (0199) H     0000 CACHigh                                   : 0
+ 0x00c9 (0201) H     b603 Vdd                                       : 950
+ 0x00cb (0203) H     0000 CACLow                                    : 0
+ 0x00cd (0205) H     0000 CACMid                                    : 0
+ 0x00cf (0207) H     0000 CACHigh                                   : 0
+ 0x00d1 (0209) H     e803 Vdd                                       : 1000
+ 0x00d3 (0211) H     0000 CACLow                                    : 0
+ 0x00d5 (0213) H     0000 CACMid                                    : 0
+ 0x00d7 (0215) H     0000 CACHigh                                   : 0
+ 0x00d9 (0217) H     1a04 Vdd                                       : 1050
+ 0x00db (0219) H     0000 CACLow                                    : 0
+ 0x00dd (0221) H     0000 CACMid                                    : 0
+ 0x00df (0223) H     0000 CACHigh                                   : 0
+ 0x00e1 (0225) H     4c04 Vdd                                       : 1100
+ 0x00e3 (0227) H     0000 CACLow                                    : 0
+ 0x00e5 (0229) H     0000 CACMid                                    : 0
+ 0x00e7 (0231) H     0000 CACHigh                                   : 0
+ 0x00e9 (0233) H     7e04 Vdd                                       : 1150
+ 0x00eb (0235) H     0000 CACLow                                    : 0
+ 0x00ed (0237) H     0000 CACMid                                    : 0
+ 0x00ef (0239) H     0000 CACHigh                                   : 0
+ 0x00f1 (0241) H     cf03 Vdd                                       : 975
+ 0x00f3 (0243) H     0000 CACLow                                    : 0
+ 0x00f5 (0245) H     0000 CACMid                                    : 0
+ 0x00f7 (0247) H     0000 CACHigh                                   : 0
+ 0x0031 (0049) H     f900 VddgfxLookupTableOffset                   : 249
+ 0x00f9 (0249) B       00 RevId                                     : 0
+ 0x00fa (0250) B       08 NumEntries                                : 8
+ 0x00fb (0251) H     8403 Vdd                                       : 900
+ 0x00fd (0253) H     0000 CACLow                                    : 0
+ 0x00ff (0255) H     0000 CACMid                                    : 0
+ 0x0101 (0257) H     0000 CACHigh                                   : 0
+ 0x0103 (0259) H     02ff Vdd                                       : 65282
+ 0x0105 (0261) H     0000 CACLow                                    : 0
+ 0x0107 (0263) H     0000 CACMid                                    : 0
+ 0x0109 (0265) H     0000 CACHigh                                   : 0
+ 0x010b (0267) H     03ff Vdd                                       : 65283
+ 0x010d (0269) H     0000 CACLow                                    : 0
+ 0x010f (0271) H     0000 CACMid                                    : 0
+ 0x0111 (0273) H     0000 CACHigh                                   : 0
+ 0x0113 (0275) H     04ff Vdd                                       : 65284
+ 0x0115 (0277) H     0000 CACLow                                    : 0
+ 0x0117 (0279) H     0000 CACMid                                    : 0
+ 0x0119 (0281) H     0000 CACHigh                                   : 0
+ 0x011b (0283) H     05ff Vdd                                       : 65285
+ 0x011d (0285) H     0000 CACLow                                    : 0
+ 0x011f (0287) H     0000 CACMid                                    : 0
+ 0x0121 (0289) H     0000 CACHigh                                   : 0
+ 0x0123 (0291) H     06ff Vdd                                       : 65286
+ 0x0125 (0293) H     0000 CACLow                                    : 0
+ 0x0127 (0295) H     0000 CACMid                                    : 0
+ 0x0129 (0297) H     0000 CACHigh                                   : 0
+ 0x012b (0299) H     07ff Vdd                                       : 65287
+ 0x012d (0301) H     0000 CACLow                                    : 0
+ 0x012f (0303) H     0000 CACMid                                    : 0
+ 0x0131 (0305) H     0000 CACHigh                                   : 0
+ 0x0133 (0307) H     08ff Vdd                                       : 65288
+ 0x0135 (0309) H     0000 CACLow                                    : 0
+ 0x0137 (0311) H     0000 CACMid                                    : 0
+ 0x0139 (0313) H     0000 CACHigh                                   : 0
+ 0x0033 (0051) H     d101 MMDependencyTableOffset                   : 465
+ 0x01d1 (0465) B       00 RevId                                     : 0
+ 0x01d2 (0466) B       08 NumEntries                                : 8
+ 0x01d3 (0467) B       00 VddcInd                                   : 0
+ 0x01d4 (0468) H     0000 VddgfxOffset                              : 0
+ 0x01d6 (0470) I 90e20000 DClk                                      : 58000
+ 0x01da (0474) I f8240100 VClk                                      : 75000
+ 0x01de (0478) I 18f60000 EClk                                      : 63000
+ 0x01e2 (0482) I 00000000 AClk                                      : 0
+ 0x01e6 (0486) I a8de0000 SAMUClk                                   : 57000
+ 0x01ea (0490) B       08 VddcInd                                   : 8
+ 0x01eb (0491) H     b4ff VddgfxOffset                              : 65460
+ 0x01ed (0493) I 18f60000 DClk                                      : 63000
+ 0x01f1 (0497) I 80380100 VClk                                      : 80000
+ 0x01f5 (0501) I 880d0100 EClk                                      : 69000
+ 0x01f9 (0505) I 00000000 AClk                                      : 0
+ 0x01fd (0509) I 00fa0000 SAMUClk                                   : 64000
+ 0x0201 (0513) B       09 VddcInd                                   : 9
+ 0x0202 (0514) H     9bff VddgfxOffset                              : 65435
+ 0x0204 (0516) I a0090100 DClk                                      : 68000
+ 0x0208 (0520) I 084c0100 VClk                                      : 85000
+ 0x020c (0524) I f8240100 EClk                                      : 75000
+ 0x0210 (0528) I 00000000 AClk                                      : 0
+ 0x0214 (0532) I 70110100 SAMUClk                                   : 70000
+ 0x0218 (0536) B       0a VddcInd                                   : 10
+ 0x0219 (0537) H     82ff VddgfxOffset                              : 65410
+ 0x021b (0539) I 281d0100 DClk                                      : 73000
+ 0x021f (0543) I a85b0100 VClk                                      : 89000
+ 0x0223 (0547) I 683c0100 EClk                                      : 81000
+ 0x0227 (0551) I 00000000 AClk                                      : 0
+ 0x022b (0555) I e0280100 SAMUClk                                   : 76000
+ 0x022f (0559) B       0b VddcInd                                   : 11
+ 0x0230 (0560) H     69ff VddgfxOffset                              : 65385
+ 0x0232 (0562) I c82c0100 DClk                                      : 77000
+ 0x0236 (0566) I 60670100 VClk                                      : 92000
+ 0x023a (0570) I f04f0100 EClk                                      : 86000
+ 0x023e (0574) I 00000000 AClk                                      : 0
+ 0x0242 (0578) I 683c0100 SAMUClk                                   : 81000
+ 0x0246 (0582) B       0c VddcInd                                   : 12
+ 0x0247 (0583) H     37ff VddgfxOffset                              : 65335
+ 0x0249 (0585) I 80380100 DClk                                      : 80000
+ 0x024d (0589) I 18730100 VClk                                      : 95000
+ 0x0251 (0593) I 78630100 EClk                                      : 91000
+ 0x0255 (0597) I 00000000 AClk                                      : 0
+ 0x0259 (0601) I 084c0100 SAMUClk                                   : 85000
+ 0x025d (0605) B       0d VddcInd                                   : 13
+ 0x025e (0606) H     05ff VddgfxOffset                              : 65285
+ 0x0260 (0608) I 38440100 DClk                                      : 83000
+ 0x0264 (0612) I d07e0100 VClk                                      : 98000
+ 0x0268 (0616) I 00770100 EClk                                      : 96000
+ 0x026c (0620) I 00000000 AClk                                      : 0
+ 0x0270 (0624) I c0570100 SAMUClk                                   : 88000
+ 0x0274 (0628) B       0e VddcInd                                   : 14
+ 0x0275 (0629) H     0000 VddgfxOffset                              : 0
+ 0x0277 (0631) I f04f0100 DClk                                      : 86000
+ 0x027b (0635) I a0860100 VClk                                      : 100000
+ 0x027f (0639) I a0860100 EClk                                      : 100000
+ 0x0283 (0643) I 00000000 AClk                                      : 0
+ 0x0287 (0647) I 78630100 SAMUClk                                   : 91000
+ 0x0035 (0053) H     f902 VCEStateTableOffset                       : 761
+ 0x02f9 (0761) B       01 RevId                                     : 1
+ 0x02fa (0762) B       06 NumEntries                                : 6
+ 0x02fb (0763) B       00 VCEClockIndex                             : 0
+ 0x02fc (0764) B       00 Flag                                      : 0
+ 0x02fd (0765) B       01 SCLKIndex                                 : 1
+ 0x02fe (0766) B       01 MCLKIndex                                 : 1
+ 0x02ff (0767) B       00 VCEClockIndex                             : 0
+ 0x0300 (0768) B       01 Flag                                      : 1
+ 0x0301 (0769) B       01 SCLKIndex                                 : 1
+ 0x0302 (0770) B       01 MCLKIndex                                 : 1
+ 0x0303 (0771) B       00 VCEClockIndex                             : 0
+ 0x0304 (0772) B       02 Flag                                      : 2
+ 0x0305 (0773) B       01 SCLKIndex                                 : 1
+ 0x0306 (0774) B       01 MCLKIndex                                 : 1
+ 0x0307 (0775) B       00 VCEClockIndex                             : 0
+ 0x0308 (0776) B       02 Flag                                      : 2
+ 0x0309 (0777) B       01 SCLKIndex                                 : 1
+ 0x030a (0778) B       01 MCLKIndex                                 : 1
+ 0x030b (0779) B       00 VCEClockIndex                             : 0
+ 0x030c (0780) B       02 Flag                                      : 2
+ 0x030d (0781) B       01 SCLKIndex                                 : 1
+ 0x030e (0782) B       01 MCLKIndex                                 : 1
+ 0x030f (0783) B       00 VCEClockIndex                             : 0
+ 0x0310 (0784) B       02 Flag                                      : 2
+ 0x0311 (0785) B       01 SCLKIndex                                 : 1
+ 0x0312 (0786) B       01 MCLKIndex                                 : 1
+ 0x0037 (0055) H     0000 PPMTableOffset                            : 0
+ 0x0039 (0057) H     c402 PowerTuneTableOffset                      : 708
+ 0x02c4 (0708) B       04 RevId                                     : 4
+ 0x02c5 (0709) H     6e00 TDP                                       : 110
+ 0x02c7 (0711) H     0000 ConfigurableTDP                           : 0
+ 0x02c9 (0713) H     6b00 TDC                                       : 107
+ 0x02cb (0715) H     6e00 BatteryPowerLimit                         : 110
+ 0x02cd (0717) H     6e00 SmallPowerLimit                           : 110
+ 0x02cf (0719) H     0000 LowCACLeakage                             : 0
+ 0x02d1 (0721) H     0000 HighCACLeakage                            : 0
+ 0x02d3 (0723) H     6e00 MaximumPowerDeliveryLimit                 : 110
+ 0x02d5 (0725) H     5a00 TjMax                                     : 90
+ 0x02d7 (0727) H     0000 PowerTuneDataSetID                        : 0
+ 0x02d9 (0729) H     0000 EDCLimit                                  : 0
+ 0x02db (0731) H     5e00 SoftwareShutdownTemp                      : 94
+ 0x02dd (0733) H     0200 ClockStretchAmount                        : 2
+ 0x02df (0735) H     6900 TemperatureLimitHotspot                   : 105
+ 0x02e1 (0737) H     5000 TemperatureLimitLiquid1                   : 80
+ 0x02e3 (0739) H     5000 TemperatureLimitLiquid2                   : 80
+ 0x02e5 (0741) H     7300 TemperatureLimitVrVddc                    : 115
+ 0x02e7 (0743) H     7300 TemperatureLimitVrMvdd                    : 115
+ 0x02e9 (0745) H     5f00 TemperatureLimitPlx                       : 95
+ 0x02eb (0747) B       00 Liquid1_I2C_address                       : 0
+ 0x02ec (0748) B       00 Liquid2_I2C_address                       : 0
+ 0x02ed (0749) B       90 Liquid_I2C_Line                           : 144
+ 0x02ee (0750) B       10 Vr_I2C_address                            : 16
+ 0x02ef (0751) B       96 Vr_I2C_Line                               : 150
+ 0x02f0 (0752) B       00 Plx_I2C_address                           : 0
+ 0x02f1 (0753) B       90 Plx_I2C_Line                              : 144
+ 0x02f2 (0754) H     0000 BoostPowerLimit                           : 0
+ 0x02f4 (0756) B       06 CKS_LDO_REFSEL                            : 6
+ 0x02f5 (0757) B       00 HotSpotOnly                               : 0
+ 0x02f6 (0758) B       00 Reserve                                   : 0
+ 0x02f7 (0759) H     0000 Reserve                                   : 0
+ 0x003b (0059) H     0000 HardLimitTableOffset                      : 0
+ 0x003d (0061) H     1303 PCIETableOffset                           : 787
+ 0x0313 (0787) B       01 RevId                                     : 1
+ 0x0314 (0788) B       03 NumEntries                                : 3
+ 0x0315 (0789) B       00 PCIEGenSpeed                              : 0
+ 0x0316 (0790) B       10 PCIELaneWidth                             : 16
+ 0x0317 (0791) B       00 Reserved                                  : 0
+ 0x0318 (0792) B       00 Reserved                                  : 0
+ 0x0319 (0793) I 00000000 PCIE_Sclk                                 : 0
+ 0x031d (0797) B       00 PCIEGenSpeed                              : 0
+ 0x031e (0798) B       10 PCIELaneWidth                             : 16
+ 0x031f (0799) B       00 Reserved                                  : 0
+ 0x0320 (0800) B       00 Reserved                                  : 0
+ 0x0321 (0801) I 00000000 PCIE_Sclk                                 : 0
+ 0x0325 (0805) B       02 PCIEGenSpeed                              : 2
+ 0x0326 (0806) B       10 PCIELaneWidth                             : 16
+ 0x0327 (0807) B       00 Reserved                                  : 0
+ 0x0328 (0808) B       00 Reserved                                  : 0
+ 0x0329 (0809) I 00000000 PCIE_Sclk                                 : 0
+ 0x003f (0063) H     2d03 GPIOTableOffset                           : 813
+ 0x032d (0813) B       00 RevId                                     : 0
+ 0x032e (0814) B       01 VRHotTriggeredSclkDpmIndex                : 1
+ 0x032f (0815) B       00 Reserve                                   : 0
+ 0x0330 (0816) B       00 Reserve                                   : 0
+ 0x0331 (0817) B       00 Reserve                                   : 0
+ 0x0332 (0818) B       00 Reserve                                   : 0
+ 0x0333 (0819) B       00 Reserve                                   : 0
+ 0x0041 (0065) H     0000 Reserved                                  : 0
+ 0x0043 (0067) H     0000 Reserved                                  : 0
+ 0x0045 (0069) H     0000 Reserved                                  : 0
+ 0x0047 (0071) H     0000 Reserved                                  : 0
+ 0x0049 (0073) H     0000 Reserved                                  : 0
+ 0x004b (0075) H     0000 Reserved                                  : 0
```

### Comparing `upp-0.2.0/test/AMD.RX5700XT.8192.190616.rom.dump` & `upp-0.2.1/test/AMD.RX5700XT.8192.190616.rom.dump`

 * *Files 21% similar despite different names*

```diff
@@ -26,41 +26,41 @@
   revision: 1
   reserve:
     reserve 0: 0
     reserve 1: 0
     reserve 2: 0
   count: 10
   max:
-    max 0: 2100
-    max 1: 1267
-    max 2: 1086
-    max 3: 1267
-    max 4: 1267
-    max 5: 875
-    max 6: 1267
-    max 7: 1284
-    max 8: 1284
-    max 9: 810
+    max 0: 2100 (GFXCLK)
+    max 1: 1267 (VCLK)
+    max 2: 1086 (DCLK)
+    max 3: 1267 (ECLK)
+    max 4: 1267 (SOCCLK)
+    max 5: 875 (UCLK)
+    max 6: 1267 (DCEFCLK)
+    max 7: 1284 (DISPCLK)
+    max 8: 1284 (PIXCLK)
+    max 9: 810 (PHYCLK)
     max 10: 0
     max 11: 0
     max 12: 0
     max 13: 0
     max 14: 0
     max 15: 0
   min:
-    min 0: 300
-    min 1: 100
-    min 2: 100
-    min 3: 100
-    min 4: 507
-    min 5: 100
-    min 6: 507
-    min 7: 308
-    min 8: 300
-    min 9: 300
+    min 0: 300 (GFXCLK)
+    min 1: 100 (VCLK)
+    min 2: 100 (DCLK)
+    min 3: 100 (ECLK)
+    min 4: 507 (SOCCLK)
+    min 5: 100 (UCLK)
+    min 6: 507 (DCEFCLK)
+    min 7: 308 (DISPCLK)
+    min 8: 300 (PIXCLK)
+    min 9: 300 (PHYCLK)
     min 10: 0
     min 11: 0
     min 12: 0
     min 13: 0
     min 14: 0
     min 15: 0
 overdrive_table:
@@ -68,28 +68,28 @@
   reserve:
     reserve 0: 0
     reserve 1: 0
     reserve 2: 0
   feature_count: 14
   setting_count: 30
   cap:
-    cap 0: 1
-    cap 1: 1
-    cap 2: 1
-    cap 3: 1
-    cap 4: 1
-    cap 5: 1
-    cap 6: 1
-    cap 7: 1
-    cap 8: 1
-    cap 9: 0
-    cap 10: 1
-    cap 11: 1
-    cap 12: 1
-    cap 13: 1
+    cap 0: 1 (GFXCLK_LIMITS)
+    cap 1: 1 (GFXCLK_CURVE)
+    cap 2: 1 (UCLK_MAX)
+    cap 3: 1 (POWER_LIMIT)
+    cap 4: 1 (FAN_ACOUSTIC_LIMIT)
+    cap 5: 1 (FAN_SPEED_MIN)
+    cap 6: 1 (TEMPERATURE_FAN)
+    cap 7: 1 (TEMPERATURE_SYSTEM)
+    cap 8: 1 (MEMORY_TIMING_TUNE)
+    cap 9: 0 (FAN_ZERO_RPM_CONTROL)
+    cap 10: 1 (AUTO_UV_ENGINE)
+    cap 11: 1 (AUTO_OC_ENGINE)
+    cap 12: 1 (AUTO_OC_MEMORY)
+    cap 13: 1 (FAN_CURVE)
     cap 14: 0
     cap 15: 0
     cap 16: 0
     cap 17: 0
     cap 18: 0
     cap 19: 0
     cap 20: 0
@@ -101,66 +101,66 @@
     cap 26: 0
     cap 27: 0
     cap 28: 0
     cap 29: 0
     cap 30: 0
     cap 31: 0
   max:
-    max 0: 2150
-    max 1: 2150
-    max 2: 2150
-    max 3: 1200
-    max 4: 2150
-    max 5: 1200
-    max 6: 2150
-    max 7: 1200
-    max 8: 950
-    max 9: 50
-    max 10: 4950
-    max 11: 4950
-    max 12: 100
-    max 13: 110
-    max 14: 2
-    max 15: 0
-    max 16: 1
-    max 17: 1
-    max 18: 1
+    max 0: 2150 (GFXCLKFMAX)
+    max 1: 2150 (GFXCLKFMIN)
+    max 2: 2150 (VDDGFXCURVEFREQ_P1)
+    max 3: 1200 (VDDGFXCURVEVOLTAGE_P1)
+    max 4: 2150 (VDDGFXCURVEFREQ_P2)
+    max 5: 1200 (VDDGFXCURVEVOLTAGE_P2)
+    max 6: 2150 (VDDGFXCURVEFREQ_P3)
+    max 7: 1200 (VDDGFXCURVEVOLTAGE_P3)
+    max 8: 950 (UCLKFMAX)
+    max 9: 50 (POWERPERCENTAGE)
+    max 10: 4950 (FANRPMMIN)
+    max 11: 4950 (FANRPMACOUSTICLIMIT)
+    max 12: 100 (FANTARGETTEMPERATURE)
+    max 13: 110 (OPERATINGTEMPMAX)
+    max 14: 2 (ACTIMING)
+    max 15: 0 (FAN_ZERO_RPM_CONTROL)
+    max 16: 1 (AUTOUVENGINE)
+    max 17: 1 (AUTOOCENGINE)
+    max 18: 1 (AUTOOCMEMORY)
     max 19: 100
     max 20: 100
     max 21: 100
     max 22: 100
     max 23: 100
     max 24: 100
     max 25: 100
     max 26: 100
     max 27: 100
     max 28: 100
     max 29: 0
     max 30: 0
     max 31: 0
   min:
-    min 0: 800
-    min 1: 800
-    min 2: 800
-    min 3: 750
-    min 4: 800
-    min 5: 750
-    min 6: 800
-    min 7: 750
-    min 8: 625
-    min 9: 50
-    min 10: 1100
-    min 11: 1100
-    min 12: 25
-    min 13: 50
-    min 14: 0
-    min 15: 0
-    min 16: 0
-    min 17: 0
-    min 18: 0
+    min 0: 800 (GFXCLKFMAX)
+    min 1: 800 (GFXCLKFMIN)
+    min 2: 800 (VDDGFXCURVEFREQ_P1)
+    min 3: 750 (VDDGFXCURVEVOLTAGE_P1)
+    min 4: 800 (VDDGFXCURVEFREQ_P2)
+    min 5: 750 (VDDGFXCURVEVOLTAGE_P2)
+    min 6: 800 (VDDGFXCURVEFREQ_P3)
+    min 7: 750 (VDDGFXCURVEVOLTAGE_P3)
+    min 8: 625 (UCLKFMAX)
+    min 9: 50 (POWERPERCENTAGE)
+    min 10: 1100 (FANRPMMIN)
+    min 11: 1100 (FANRPMACOUSTICLIMIT)
+    min 12: 25 (FANTARGETTEMPERATURE)
+    min 13: 50 (OPERATINGTEMPMAX)
+    min 14: 0 (ACTIMING)
+    min 15: 0 (FAN_ZERO_RPM_CONTROL)
+    min 16: 0 (AUTOUVENGINE)
+    min 17: 0 (AUTOOCENGINE)
+    min 18: 0 (AUTOOCMEMORY)
     min 19: 25
     min 20: 10
     min 21: 25
     min 22: 10
     min 23: 25
     min 24: 10
     min 25: 25
```

### Comparing `upp-0.2.0/test/AMD.RX5700XT.8192.190616.rom.rawdump` & `upp-0.2.1/test/AMD.RadeonVII.16384.190116.rom.rawdump`

 * *Files 7% similar despite different names*

```diff
@@ -1,706 +1,658 @@
-PowerPlay table rev 12.0 size 1674 bytes
- Offset (dec.) t Raw val. Variable name                   Decoded value
------------------------------------------------------------------------
- 0x0000 (0000) H     8a06 structuresize                   : 1674
- 0x0002 (0002) B       0c format_revision                 : 12
- 0x0003 (0003) B       00 content_revision                : 0
- 0x0004 (0004) B       01 table_revision                  : 1
- 0x0005 (0005) H     e201 table_size                      : 482
- 0x0007 (0007) I c7080000 golden_pp_id                    : 2247
- 0x000b (0011) I 20380000 golden_revision                 : 14368
- 0x000f (0015) H     7d00 format_id                       : 125
- 0x0011 (0017) I 08000000 platform_caps                   : 8
- 0x0015 (0021) B       1b thermal_controller_type         : 27
- 0x0016 (0022) H     0000 small_power_limit1              : 0
- 0x0018 (0024) H     0000 small_power_limit2              : 0
- 0x001a (0026) H     0000 boost_power_limit               : 0
- 0x001c (0028) H     0000 od_turbo_power_limit            : 0
- 0x001e (0030) H     0000 od_power_save_power_limit       : 0
- 0x0020 (0032) H     7600 software_shutdown_temp          : 118
- 0x0022 (0034) H     0000 reserve                         : 0
- 0x0024 (0036) H     0000 reserve                         : 0
- 0x0026 (0038) H     0000 reserve                         : 0
- 0x0028 (0040) H     0000 reserve                         : 0
- 0x002a (0042) H     0000 reserve                         : 0
- 0x002c (0044) H     0000 reserve                         : 0
- 0x002e (0046) B       01 revision                        : 1
- 0x002f (0047) B       00 reserve                         : 0
- 0x0030 (0048) B       00 reserve                         : 0
- 0x0031 (0049) B       00 reserve                         : 0
- 0x0032 (0050) I 0a000000 count                           : 10
- 0x0036 (0054) I 34080000 max                             : 2100
- 0x003a (0058) I f3040000 max                             : 1267
- 0x003e (0062) I 3e040000 max                             : 1086
- 0x0042 (0066) I f3040000 max                             : 1267
- 0x0046 (0070) I f3040000 max                             : 1267
- 0x004a (0074) I 6b030000 max                             : 875
- 0x004e (0078) I f3040000 max                             : 1267
- 0x0052 (0082) I 04050000 max                             : 1284
- 0x0056 (0086) I 04050000 max                             : 1284
- 0x005a (0090) I 2a030000 max                             : 810
- 0x005e (0094) I 00000000 max                             : 0
- 0x0062 (0098) I 00000000 max                             : 0
- 0x0066 (0102) I 00000000 max                             : 0
- 0x006a (0106) I 00000000 max                             : 0
- 0x006e (0110) I 00000000 max                             : 0
- 0x0072 (0114) I 00000000 max                             : 0
- 0x0076 (0118) I 2c010000 min                             : 300
- 0x007a (0122) I 64000000 min                             : 100
- 0x007e (0126) I 64000000 min                             : 100
- 0x0082 (0130) I 64000000 min                             : 100
- 0x0086 (0134) I fb010000 min                             : 507
- 0x008a (0138) I 64000000 min                             : 100
- 0x008e (0142) I fb010000 min                             : 507
- 0x0092 (0146) I 34010000 min                             : 308
- 0x0096 (0150) I 2c010000 min                             : 300
- 0x009a (0154) I 2c010000 min                             : 300
- 0x009e (0158) I 00000000 min                             : 0
- 0x00a2 (0162) I 00000000 min                             : 0
- 0x00a6 (0166) I 00000000 min                             : 0
- 0x00aa (0170) I 00000000 min                             : 0
- 0x00ae (0174) I 00000000 min                             : 0
- 0x00b2 (0178) I 00000000 min                             : 0
- 0x00b6 (0182) B       80 revision                        : 128
- 0x00b7 (0183) B       00 reserve                         : 0
- 0x00b8 (0184) B       00 reserve                         : 0
- 0x00b9 (0185) B       00 reserve                         : 0
- 0x00ba (0186) I 0e000000 feature_count                   : 14
- 0x00be (0190) I 1e000000 setting_count                   : 30
- 0x00c2 (0194) B       01 cap                             : 1
- 0x00c3 (0195) B       01 cap                             : 1
- 0x00c4 (0196) B       01 cap                             : 1
- 0x00c5 (0197) B       01 cap                             : 1
- 0x00c6 (0198) B       01 cap                             : 1
- 0x00c7 (0199) B       01 cap                             : 1
- 0x00c8 (0200) B       01 cap                             : 1
- 0x00c9 (0201) B       01 cap                             : 1
- 0x00ca (0202) B       01 cap                             : 1
- 0x00cb (0203) B       00 cap                             : 0
- 0x00cc (0204) B       01 cap                             : 1
- 0x00cd (0205) B       01 cap                             : 1
- 0x00ce (0206) B       01 cap                             : 1
- 0x00cf (0207) B       01 cap                             : 1
- 0x00d0 (0208) B       00 cap                             : 0
- 0x00d1 (0209) B       00 cap                             : 0
- 0x00d2 (0210) B       00 cap                             : 0
- 0x00d3 (0211) B       00 cap                             : 0
- 0x00d4 (0212) B       00 cap                             : 0
- 0x00d5 (0213) B       00 cap                             : 0
- 0x00d6 (0214) B       00 cap                             : 0
- 0x00d7 (0215) B       00 cap                             : 0
- 0x00d8 (0216) B       00 cap                             : 0
- 0x00d9 (0217) B       00 cap                             : 0
- 0x00da (0218) B       00 cap                             : 0
- 0x00db (0219) B       00 cap                             : 0
- 0x00dc (0220) B       00 cap                             : 0
- 0x00dd (0221) B       00 cap                             : 0
- 0x00de (0222) B       00 cap                             : 0
- 0x00df (0223) B       00 cap                             : 0
- 0x00e0 (0224) B       00 cap                             : 0
- 0x00e1 (0225) B       00 cap                             : 0
- 0x00e2 (0226) I 66080000 max                             : 2150
- 0x00e6 (0230) I 66080000 max                             : 2150
- 0x00ea (0234) I 66080000 max                             : 2150
- 0x00ee (0238) I b0040000 max                             : 1200
- 0x00f2 (0242) I 66080000 max                             : 2150
- 0x00f6 (0246) I b0040000 max                             : 1200
- 0x00fa (0250) I 66080000 max                             : 2150
- 0x00fe (0254) I b0040000 max                             : 1200
- 0x0102 (0258) I b6030000 max                             : 950
- 0x0106 (0262) I 32000000 max                             : 50
- 0x010a (0266) I 56130000 max                             : 4950
- 0x010e (0270) I 56130000 max                             : 4950
- 0x0112 (0274) I 64000000 max                             : 100
- 0x0116 (0278) I 6e000000 max                             : 110
- 0x011a (0282) I 02000000 max                             : 2
- 0x011e (0286) I 00000000 max                             : 0
- 0x0122 (0290) I 01000000 max                             : 1
- 0x0126 (0294) I 01000000 max                             : 1
- 0x012a (0298) I 01000000 max                             : 1
- 0x012e (0302) I 64000000 max                             : 100
- 0x0132 (0306) I 64000000 max                             : 100
- 0x0136 (0310) I 64000000 max                             : 100
- 0x013a (0314) I 64000000 max                             : 100
- 0x013e (0318) I 64000000 max                             : 100
- 0x0142 (0322) I 64000000 max                             : 100
- 0x0146 (0326) I 64000000 max                             : 100
- 0x014a (0330) I 64000000 max                             : 100
- 0x014e (0334) I 64000000 max                             : 100
- 0x0152 (0338) I 64000000 max                             : 100
- 0x0156 (0342) I 00000000 max                             : 0
- 0x015a (0346) I 00000000 max                             : 0
- 0x015e (0350) I 00000000 max                             : 0
- 0x0162 (0354) I 20030000 min                             : 800
- 0x0166 (0358) I 20030000 min                             : 800
- 0x016a (0362) I 20030000 min                             : 800
- 0x016e (0366) I ee020000 min                             : 750
- 0x0172 (0370) I 20030000 min                             : 800
- 0x0176 (0374) I ee020000 min                             : 750
- 0x017a (0378) I 20030000 min                             : 800
- 0x017e (0382) I ee020000 min                             : 750
- 0x0182 (0386) I 71020000 min                             : 625
- 0x0186 (0390) I 32000000 min                             : 50
- 0x018a (0394) I 4c040000 min                             : 1100
- 0x018e (0398) I 4c040000 min                             : 1100
- 0x0192 (0402) I 19000000 min                             : 25
- 0x0196 (0406) I 32000000 min                             : 50
- 0x019a (0410) I 00000000 min                             : 0
- 0x019e (0414) I 00000000 min                             : 0
- 0x01a2 (0418) I 00000000 min                             : 0
- 0x01a6 (0422) I 00000000 min                             : 0
- 0x01aa (0426) I 00000000 min                             : 0
- 0x01ae (0430) I 19000000 min                             : 25
- 0x01b2 (0434) I 0a000000 min                             : 10
- 0x01b6 (0438) I 19000000 min                             : 25
- 0x01ba (0442) I 0a000000 min                             : 10
- 0x01be (0446) I 19000000 min                             : 25
- 0x01c2 (0450) I 0a000000 min                             : 10
- 0x01c6 (0454) I 19000000 min                             : 25
- 0x01ca (0458) I 0a000000 min                             : 10
- 0x01ce (0462) I 19000000 min                             : 25
- 0x01d2 (0466) I 0a000000 min                             : 10
- 0x01d6 (0470) I 00000000 min                             : 0
- 0x01da (0474) I 00000000 min                             : 0
- 0x01de (0478) I 00000000 min                             : 0
- 0x01e2 (0482) I 08000000 Version                         : 8
- 0x01e6 (0486) I ffafdfb3 FeaturesToRun                   : 3017781247
- 0x01ea (0490) I 23060000 FeaturesToRun                   : 1571
- 0x01ee (0494) H     b400 SocketPowerLimitAc              : 180
- 0x01f0 (0496) H     0000 SocketPowerLimitAc              : 0
- 0x01f2 (0498) H     0000 SocketPowerLimitAc              : 0
- 0x01f4 (0500) H     0000 SocketPowerLimitAc              : 0
- 0x01f6 (0502) H     0000 SocketPowerLimitAcTau           : 0
- 0x01f8 (0504) H     0000 SocketPowerLimitAcTau           : 0
- 0x01fa (0506) H     0000 SocketPowerLimitAcTau           : 0
- 0x01fc (0508) H     0000 SocketPowerLimitAcTau           : 0
- 0x01fe (0510) H     b400 SocketPowerLimitDc              : 180
- 0x0200 (0512) H     0000 SocketPowerLimitDc              : 0
- 0x0202 (0514) H     0000 SocketPowerLimitDc              : 0
- 0x0204 (0516) H     0000 SocketPowerLimitDc              : 0
- 0x0206 (0518) H     0000 SocketPowerLimitDcTau           : 0
- 0x0208 (0520) H     0000 SocketPowerLimitDcTau           : 0
- 0x020a (0522) H     0000 SocketPowerLimitDcTau           : 0
- 0x020c (0524) H     0000 SocketPowerLimitDcTau           : 0
- 0x020e (0526) H     0e00 TdcLimitSoc                     : 14
- 0x0210 (0528) H     0000 TdcLimitSocTau                  : 0
- 0x0212 (0530) H     aa00 TdcLimitGfx                     : 170
- 0x0214 (0532) H     0000 TdcLimitGfxTau                  : 0
- 0x0216 (0534) H     6400 TedgeLimit                      : 100
- 0x0218 (0536) H     6e00 ThotspotLimit                   : 110
- 0x021a (0538) H     6900 TmemLimit                       : 105
- 0x021c (0540) H     7300 Tvr_gfxLimit                    : 115
- 0x021e (0542) H     7300 Tvr_mem0Limit                   : 115
- 0x0220 (0544) H     7300 Tvr_mem1Limit                   : 115
- 0x0222 (0546) H     7300 Tvr_socLimit                    : 115
- 0x0224 (0548) H     0000 Tliquid0Limit                   : 0
- 0x0226 (0550) H     0000 Tliquid1Limit                   : 0
- 0x0228 (0552) H     0000 TplxLimit                       : 0
- 0x022a (0554) I 00000000 FitLimit                        : 0
- 0x022e (0558) H     0000 PpmPowerLimit                   : 0
- 0x0230 (0560) H     0000 PpmTemperatureThreshold         : 0
- 0x0232 (0562) I fe700000 ThrottlerControlMask            : 28926
- 0x0236 (0566) I 01000000 FwDStateMask                    : 1
- 0x023a (0570) H     6400 UlvVoltageOffsetSoc             : 100
- 0x023c (0572) H     6400 UlvVoltageOffsetGfx             : 100
- 0x023e (0574) B       00 GceaLinkMgrIdleThreshold        : 0
- 0x023f (0575) B       00 RlcUlvParams                    : 0
- 0x0240 (0576) B       00 RlcUlvParams                    : 0
- 0x0241 (0577) B       00 RlcUlvParams                    : 0
- 0x0242 (0578) B       00 UlvSmnclkDid                    : 0
- 0x0243 (0579) B       00 UlvMp1clkDid                    : 0
- 0x0244 (0580) B       00 UlvGfxclkBypass                 : 0
- 0x0245 (0581) B       00 Padding234                      : 0
- 0x0246 (0582) H     540b MinVoltageUlvGfx                : 2900
- 0x0248 (0584) H     540b MinVoltageUlvSoc                : 2900
- 0x024a (0586) H     b80b MinVoltageGfx                   : 3000
- 0x024c (0588) H     b80b MinVoltageSoc                   : 3000
- 0x024e (0590) H     c012 MaxVoltageGfx                   : 4800
- 0x0250 (0592) H     c012 MaxVoltageSoc                   : 4800
- 0x0252 (0594) H     4c00 LoadLineResistanceGfx           : 76
- 0x0254 (0596) H     0000 LoadLineResistanceSoc           : 0
- 0x0256 (0598) B       01 VoltageMode                     : 1
- 0x0257 (0599) B       00 SnapToDiscrete                  : 0
- 0x0258 (0600) B       02 NumDiscreteLevels               : 2
- 0x0259 (0601) B       00 Padding                         : 0
- 0x025a (0602) f 00000000 m                               : 0
- 0x025e (0606) f 00000000 b                               : 0
- 0x0262 (0610) f 8126823e a                               : 0.2542
- 0x0266 (0614) f a4705dbe b                               :-0.21625
- 0x026a (0618) f b51a323f c                               : 0.69572
- 0x026e (0622) B       01 VoltageMode                     : 1
- 0x026f (0623) B       00 SnapToDiscrete                  : 0
- 0x0270 (0624) B       02 NumDiscreteLevels               : 2
- 0x0271 (0625) B       00 Padding                         : 0
- 0x0272 (0626) f 0000803f m                               : 1
- 0x0276 (0630) f 00000000 b                               : 0
- 0x027a (0634) f f1ba5e3e a                               : 0.21751
- 0x027e (0638) f abb26fbd b                               :-0.05852
- 0x0282 (0642) f 45f5363f c                               : 0.71468
- 0x0286 (0646) B       01 VoltageMode                     : 1
- 0x0287 (0647) B       01 SnapToDiscrete                  : 1
- 0x0288 (0648) B       04 NumDiscreteLevels               : 4
- 0x0289 (0649) B       00 Padding                         : 0
- 0x028a (0650) f 0000803f m                               : 1
- 0x028e (0654) f 00000000 b                               : 0
- 0x0292 (0658) f f1ba5e3e a                               : 0.21751
- 0x0296 (0662) f abb26fbd b                               :-0.05852
- 0x029a (0666) f 45f5363f c                               : 0.71468
- 0x029e (0670) B       01 VoltageMode                     : 1
- 0x029f (0671) B       00 SnapToDiscrete                  : 0
- 0x02a0 (0672) B       02 NumDiscreteLevels               : 2
- 0x02a1 (0673) B       00 Padding                         : 0
- 0x02a2 (0674) f d8f0243f m                               : 0.6443
- 0x02a6 (0678) f 35ef083f b                               : 0.5349
- 0x02aa (0682) f 00000000 a                               : 0
- 0x02ae (0686) f d42bc53e b                               : 0.3851
- 0x02b2 (0690) f 575b113f c                               : 0.5678
- 0x02b6 (0694) B       01 VoltageMode                     : 1
- 0x02b7 (0695) B       00 SnapToDiscrete                  : 0
- 0x02b8 (0696) B       02 NumDiscreteLevels               : 2
- 0x02b9 (0697) B       00 Padding                         : 0
- 0x02ba (0698) f 0a68023f m                               : 0.5094
- 0x02be (0702) f 14ae173f b                               : 0.5925
- 0x02c2 (0706) f 00000000 a                               : 0
- 0x02c6 (0710) f 8351a93e b                               : 0.3307
- 0x02ca (0714) f 3789113f c                               : 0.5685
- 0x02ce (0718) B       01 VoltageMode                     : 1
- 0x02cf (0719) B       00 SnapToDiscrete                  : 0
- 0x02d0 (0720) B       02 NumDiscreteLevels               : 2
- 0x02d1 (0721) B       00 Padding                         : 0
- 0x02d2 (0722) f 9cc4a03f m                               : 1.256
- 0x02d6 (0726) f 8e06b0be b                               :-0.3438
- 0x02da (0730) f 00000000 a                               : 0
- 0x02de (0734) f e3c7083f b                               : 0.5343
- 0x02e2 (0738) f ec2f7b3e c                               : 0.2453
- 0x02e6 (0742) B       01 VoltageMode                     : 1
- 0x02e7 (0743) B       00 SnapToDiscrete                  : 0
- 0x02e8 (0744) B       02 NumDiscreteLevels               : 2
- 0x02e9 (0745) B       00 Padding                         : 0
- 0x02ea (0746) f 6154523f m                               : 0.8216
- 0x02ee (0750) f d7346f3c b                               : 0.0146
- 0x02f2 (0754) f 00000000 a                               : 0
- 0x02f6 (0758) f fd87f43e b                               : 0.4776
- 0x02fa (0762) f ca54813e c                               : 0.2526
- 0x02fe (0766) B       02 VoltageMode                     : 2
- 0x02ff (0767) B       00 SnapToDiscrete                  : 0
- 0x0300 (0768) B       02 NumDiscreteLevels               : 2
- 0x0301 (0769) B       00 Padding                         : 0
- 0x0302 (0770) f 00000000 m                               : 0
- 0x0306 (0774) f 00000000 b                               : 0
- 0x030a (0778) f 00000000 a                               : 0
- 0x030e (0782) f 00000000 b                               : 0
- 0x0312 (0786) f 00000000 c                               : 0
- 0x0316 (0790) B       02 VoltageMode                     : 2
- 0x0317 (0791) B       00 SnapToDiscrete                  : 0
- 0x0318 (0792) B       02 NumDiscreteLevels               : 2
- 0x0319 (0793) B       00 Padding                         : 0
- 0x031a (0794) f 00000000 m                               : 0
- 0x031e (0798) f 00000000 b                               : 0
- 0x0322 (0802) f 00000000 a                               : 0
- 0x0326 (0806) f 00000000 b                               : 0
- 0x032a (0810) f 00000000 c                               : 0
- 0x032e (0814) H     2c01 FreqTableGfx                    : 300
- 0x0330 (0816) H     3408 FreqTableGfx                    : 2100
- 0x0332 (0818) H     7805 FreqTableGfx                    : 1400
- 0x0334 (0820) H     7805 FreqTableGfx                    : 1400
- 0x0336 (0822) H     7805 FreqTableGfx                    : 1400
- 0x0338 (0824) H     7805 FreqTableGfx                    : 1400
- 0x033a (0826) H     7805 FreqTableGfx                    : 1400
- 0x033c (0828) H     7805 FreqTableGfx                    : 1400
- 0x033e (0830) H     7805 FreqTableGfx                    : 1400
- 0x0340 (0832) H     7805 FreqTableGfx                    : 1400
- 0x0342 (0834) H     7805 FreqTableGfx                    : 1400
- 0x0344 (0836) H     7805 FreqTableGfx                    : 1400
- 0x0346 (0838) H     7805 FreqTableGfx                    : 1400
- 0x0348 (0840) H     7805 FreqTableGfx                    : 1400
- 0x034a (0842) H     7805 FreqTableGfx                    : 1400
- 0x034c (0844) H     7805 FreqTableGfx                    : 1400
- 0x034e (0846) H     6400 FreqTableVclk                   : 100
- 0x0350 (0848) H     f304 FreqTableVclk                   : 1267
- 0x0352 (0850) H     f304 FreqTableVclk                   : 1267
- 0x0354 (0852) H     f304 FreqTableVclk                   : 1267
- 0x0356 (0854) H     f304 FreqTableVclk                   : 1267
- 0x0358 (0856) H     f304 FreqTableVclk                   : 1267
- 0x035a (0858) H     f304 FreqTableVclk                   : 1267
- 0x035c (0860) H     f304 FreqTableVclk                   : 1267
- 0x035e (0862) H     6400 FreqTableDclk                   : 100
- 0x0360 (0864) H     3e04 FreqTableDclk                   : 1086
- 0x0362 (0866) H     3e04 FreqTableDclk                   : 1086
- 0x0364 (0868) H     3e04 FreqTableDclk                   : 1086
- 0x0366 (0870) H     3e04 FreqTableDclk                   : 1086
- 0x0368 (0872) H     3e04 FreqTableDclk                   : 1086
- 0x036a (0874) H     3e04 FreqTableDclk                   : 1086
- 0x036c (0876) H     3e04 FreqTableDclk                   : 1086
- 0x036e (0878) H     fb01 FreqTableSocclk                 : 507
- 0x0370 (0880) H     f304 FreqTableSocclk                 : 1267
- 0x0372 (0882) H     b603 FreqTableSocclk                 : 950
- 0x0374 (0884) H     b603 FreqTableSocclk                 : 950
- 0x0376 (0886) H     b603 FreqTableSocclk                 : 950
- 0x0378 (0888) H     b603 FreqTableSocclk                 : 950
- 0x037a (0890) H     b603 FreqTableSocclk                 : 950
- 0x037c (0892) H     b603 FreqTableSocclk                 : 950
- 0x037e (0894) H     6400 FreqTableUclk                   : 100
- 0x0380 (0896) H     f401 FreqTableUclk                   : 500
- 0x0382 (0898) H     7102 FreqTableUclk                   : 625
- 0x0384 (0900) H     6b03 FreqTableUclk                   : 875
- 0x0386 (0902) H     fb01 FreqTableDcefclk                : 507
- 0x0388 (0904) H     f304 FreqTableDcefclk                : 1267
- 0x038a (0906) H     f304 FreqTableDcefclk                : 1267
- 0x038c (0908) H     f304 FreqTableDcefclk                : 1267
- 0x038e (0910) H     f304 FreqTableDcefclk                : 1267
- 0x0390 (0912) H     f304 FreqTableDcefclk                : 1267
- 0x0392 (0914) H     f304 FreqTableDcefclk                : 1267
- 0x0394 (0916) H     f304 FreqTableDcefclk                : 1267
- 0x0396 (0918) H     3401 FreqTableDispclk                : 308
- 0x0398 (0920) H     0405 FreqTableDispclk                : 1284
- 0x039a (0922) H     0405 FreqTableDispclk                : 1284
- 0x039c (0924) H     0405 FreqTableDispclk                : 1284
- 0x039e (0926) H     0405 FreqTableDispclk                : 1284
- 0x03a0 (0928) H     0405 FreqTableDispclk                : 1284
- 0x03a2 (0930) H     0405 FreqTableDispclk                : 1284
- 0x03a4 (0932) H     0405 FreqTableDispclk                : 1284
- 0x03a6 (0934) H     2c01 FreqTablePixclk                 : 300
- 0x03a8 (0936) H     0405 FreqTablePixclk                 : 1284
- 0x03aa (0938) H     a404 FreqTablePixclk                 : 1188
- 0x03ac (0940) H     a404 FreqTablePixclk                 : 1188
- 0x03ae (0942) H     a404 FreqTablePixclk                 : 1188
- 0x03b0 (0944) H     a404 FreqTablePixclk                 : 1188
- 0x03b2 (0946) H     a404 FreqTablePixclk                 : 1188
- 0x03b4 (0948) H     a404 FreqTablePixclk                 : 1188
- 0x03b6 (0950) H     2c01 FreqTablePhyclk                 : 300
- 0x03b8 (0952) H     2a03 FreqTablePhyclk                 : 810
- 0x03ba (0954) H     2a03 FreqTablePhyclk                 : 810
- 0x03bc (0956) H     2a03 FreqTablePhyclk                 : 810
- 0x03be (0958) H     2a03 FreqTablePhyclk                 : 810
- 0x03c0 (0960) H     2a03 FreqTablePhyclk                 : 810
- 0x03c2 (0962) H     2a03 FreqTablePhyclk                 : 810
- 0x03c4 (0964) H     2a03 FreqTablePhyclk                 : 810
- 0x03c6 (0966) I d001d001 Paddingclks                     : 30409168
- 0x03ca (0970) I d001d001 Paddingclks                     : 30409168
- 0x03ce (0974) I d001d001 Paddingclks                     : 30409168
- 0x03d2 (0978) I d001d001 Paddingclks                     : 30409168
- 0x03d6 (0982) I d001d001 Paddingclks                     : 30409168
- 0x03da (0986) I d001d001 Paddingclks                     : 30409168
- 0x03de (0990) I d001d001 Paddingclks                     : 30409168
- 0x03e2 (0994) I d001d001 Paddingclks                     : 30409168
- 0x03e6 (0998) I d001d001 Paddingclks                     : 30409168
- 0x03ea (1002) I d001d001 Paddingclks                     : 30409168
- 0x03ee (1006) I d001d001 Paddingclks                     : 30409168
- 0x03f2 (1010) I d001d001 Paddingclks                     : 30409168
- 0x03f6 (1014) I d001d001 Paddingclks                     : 30409168
- 0x03fa (1018) I d001d001 Paddingclks                     : 30409168
- 0x03fe (1022) I d001d001 Paddingclks                     : 30409168
- 0x0402 (1026) I d001d001 Paddingclks                     : 30409168
- 0x0406 (1030) H     3408 DcModeMaxFreq                   : 2100
- 0x0408 (1032) H     f304 DcModeMaxFreq                   : 1267
- 0x040a (1034) H     6b03 DcModeMaxFreq                   : 875
- 0x040c (1036) H     3e04 DcModeMaxFreq                   : 1086
- 0x040e (1038) H     f304 DcModeMaxFreq                   : 1267
- 0x0410 (1040) H     f304 DcModeMaxFreq                   : 1267
- 0x0412 (1042) H     0405 DcModeMaxFreq                   : 1284
- 0x0414 (1044) H     0405 DcModeMaxFreq                   : 1284
- 0x0416 (1046) H     2a03 DcModeMaxFreq                   : 810
- 0x0418 (1048) H     d001 Padding8_Clks                   : 464
- 0x041a (1050) B       00 FreqTableUclkDiv                : 0
- 0x041b (1051) B       03 FreqTableUclkDiv                : 3
- 0x041c (1052) B       03 FreqTableUclkDiv                : 3
- 0x041d (1053) B       03 FreqTableUclkDiv                : 3
- 0x041e (1054) H     3001 Mp0clkFreq                      : 304
- 0x0420 (1056) H     fb01 Mp0clkFreq                      : 507
- 0x0422 (1058) H     b80b Mp0DpmVoltage                   : 3000
- 0x0424 (1060) H     b80b Mp0DpmVoltage                   : 3000
- 0x0426 (1062) H     8c0a MemVddciVoltage                 : 2700
- 0x0428 (1064) H     480d MemVddciVoltage                 : 3400
- 0x042a (1066) H     480d MemVddciVoltage                 : 3400
- 0x042c (1068) H     480d MemVddciVoltage                 : 3400
- 0x042e (1070) H     8813 MemMvddVoltage                  : 5000
- 0x0430 (1072) H     1815 MemMvddVoltage                  : 5400
- 0x0432 (1074) H     1815 MemMvddVoltage                  : 5400
- 0x0434 (1076) H     1815 MemMvddVoltage                  : 5400
- 0x0436 (1078) H     2003 GfxclkFgfxoffEntry              : 800
- 0x0438 (1080) H     2003 GfxclkFinit                     : 800
- 0x043a (1082) H     2003 GfxclkFidle                     : 800
- 0x043c (1084) H     0000 GfxclkSlewRate                  : 0
- 0x043e (1086) H     0000 GfxclkFopt                      : 0
- 0x0440 (1088) B       d0 Padding567                      : 208
- 0x0441 (1089) B       01 Padding567                      : 1
- 0x0442 (1090) H     0000 GfxclkDsMaxFreq                 : 0
- 0x0444 (1092) B       01 GfxclkSource                    : 1
- 0x0445 (1093) B       02 Padding456                      : 2
- 0x0446 (1094) B       00 LowestUclkReservedForUlv        : 0
- 0x0447 (1095) B       00 Uclk                            : 0
- 0x0448 (1096) B       5b Uclk                            : 91
- 0x0449 (1097) B       00 Uclk                            : 0
- 0x044a (1098) B       00 MemoryType                      : 0
- 0x044b (1099) B       10 MemoryChannels                  : 16
- 0x044c (1100) B       00 PaddingMem                      : 0
- 0x044d (1101) B       00 PaddingMem                      : 0
- 0x044e (1102) B       00 PcieGenSpeed                    : 0
- 0x044f (1103) B       03 PcieGenSpeed                    : 3
- 0x0450 (1104) B       06 PcieLaneCount                   : 6
- 0x0451 (1105) B       06 PcieLaneCount                   : 6
- 0x0452 (1106) H     6b02 LclkFreq                        : 619
- 0x0454 (1108) H     6b02 LclkFreq                        : 619
- 0x0456 (1110) H     0000 EnableTdpm                      : 0
- 0x0458 (1112) H     0000 TdpmHighHystTemperature         : 0
- 0x045a (1114) H     0000 TdpmLowHystTemperature          : 0
- 0x045c (1116) H     0000 GfxclkFreqHighTempLimit         : 0
- 0x045e (1118) H     0000 FanStopTemp                     : 0
- 0x0460 (1120) H     0000 FanStartTemp                    : 0
- 0x0462 (1122) H     9001 FanGainEdge                     : 400
- 0x0464 (1124) H     9001 FanGainHotspot                  : 400
- 0x0466 (1126) H     9001 FanGainLiquid0                  : 400
- 0x0468 (1128) H     9001 FanGainLiquid1                  : 400
- 0x046a (1130) H     9001 FanGainVrGfx                    : 400
- 0x046c (1132) H     9001 FanGainVrSoc                    : 400
- 0x046e (1134) H     9001 FanGainVrMem0                   : 400
- 0x0470 (1136) H     9001 FanGainVrMem1                   : 400
- 0x0472 (1138) H     9001 FanGainPlx                      : 400
- 0x0474 (1140) H     9001 FanGainMem                      : 400
- 0x0476 (1142) H     1400 FanPwmMin                       : 20
- 0x0478 (1144) H     3408 FanAcousticLimitRpm             : 2100
- 0x047a (1146) H     3408 FanThrottlingRpm                : 2100
- 0x047c (1148) H     5613 FanMaximumRpm                   : 4950
- 0x047e (1150) H     5a00 FanTargetTemperature            : 90
- 0x0480 (1152) H     2003 FanTargetGfxclk                 : 800
- 0x0482 (1154) B       01 FanTempInputSelect              : 1
- 0x0483 (1155) B       00 FanPadding                      : 0
- 0x0484 (1156) B       00 FanZeroRpmEnable                : 0
- 0x0485 (1157) B       02 FanTachEdgePerRev               : 2
- 0x0486 (1158) h     0000 FuzzyFan_ErrorSetDelta          : 0
- 0x0488 (1160) h     0000 FuzzyFan_ErrorRateSetDelta      : 0
- 0x048a (1162) h     0000 FuzzyFan_PwmSetDelta            : 0
- 0x048c (1164) H     0000 FuzzyFan_Reserved               : 0
- 0x048e (1166) B       00 OverrideAvfsGb                  : 0
- 0x048f (1167) B       00 OverrideAvfsGb                  : 0
- 0x0490 (1168) B       00 Padding8_Avfs                   : 0
- 0x0491 (1169) B       00 Padding8_Avfs                   : 0
- 0x0492 (1170) f 47e6913c a                               : 0.01781
- 0x0496 (1174) f aca841bd b                               :-0.04728
- 0x049a (1178) f 13445d3d c                               : 0.05402
- 0x049e (1182) f 00000000 a                               : 0
- 0x04a2 (1186) f 00000000 b                               : 0
- 0x04a6 (1190) f 8fc2f53c c                               : 0.03
- 0x04aa (1194) f 00000000 a                               : 0
- 0x04ae (1198) f 00000000 b                               : 0
- 0x04b2 (1202) f 00000000 c                               : 0
- 0x04b6 (1206) f 4bc8c73d a                               : 0.09755
- 0x04ba (1210) f 9834463d b                               : 0.04839
- 0x04be (1214) f 7042a1bd c                               :-0.07874
- 0x04c2 (1218) f af5a193b a                               : 0.00234
- 0x04c6 (1222) f 8ca11cbb b                               :-0.00239
- 0x04ca (1226) f f836bd3d c                               : 0.09239
- 0x04ce (1230) f 00000000 m                               : 0
- 0x04d2 (1234) f 00000000 b                               : 0
- 0x04d6 (1238) f 00000000 m                               : 0
- 0x04da (1242) f 00000000 b                               : 0
- 0x04de (1246) f 00000000 a                               : 0
- 0x04e2 (1250) f 00000000 b                               : 0
- 0x04e6 (1254) f 00000000 c                               : 0
- 0x04ea (1258) f 00000000 a                               : 0
- 0x04ee (1262) f 00000000 b                               : 0
- 0x04f2 (1266) f 00000000 c                               : 0
- 0x04f6 (1270) H     a000 DcTol                           : 160
- 0x04f8 (1272) H     a000 DcTol                           : 160
- 0x04fa (1274) B       01 DcBtcEnabled                    : 1
- 0x04fb (1275) B       01 DcBtcEnabled                    : 1
- 0x04fc (1276) B       00 Padding8_GfxBtc                 : 0
- 0x04fd (1277) B       00 Padding8_GfxBtc                 : 0
- 0x04fe (1278) H     0000 DcBtcMin                        : 0
- 0x0500 (1280) H     0000 DcBtcMin                        : 0
- 0x0502 (1282) H     a000 DcBtcMax                        : 160
- 0x0504 (1284) H     a000 DcBtcMax                        : 160
- 0x0506 (1286) I 00020000 DebugOverrides                  : 512
- 0x050a (1290) f 00000000 a                               : 0
- 0x050e (1294) f 00000000 b                               : 0
- 0x0512 (1298) f 00000000 c                               : 0
- 0x0516 (1302) f 00000000 a                               : 0
- 0x051a (1306) f 00000000 b                               : 0
- 0x051e (1310) f 00000000 c                               : 0
- 0x0522 (1314) f 00000000 a                               : 0
- 0x0526 (1318) f 00000000 b                               : 0
- 0x052a (1322) f 00000000 c                               : 0
- 0x052e (1326) f 00000000 a                               : 0
- 0x0532 (1330) f 00000000 b                               : 0
- 0x0536 (1334) f 00000000 c                               : 0
- 0x053a (1338) B       01 TotalPowerConfig                : 1
- 0x053b (1339) B       00 TotalPowerSpare1                : 0
- 0x053c (1340) H     0000 TotalPowerSpare2                : 0
- 0x053e (1342) H     0000 PccThresholdLow                 : 0
- 0x0540 (1344) H     0000 PccThresholdHigh                : 0
- 0x0542 (1346) I 00000000 MGpuFanBoostLimitRpm            : 0
- 0x0546 (1350) I 00000000 PaddingAPCC                     : 0
- 0x054a (1354) I 00000000 PaddingAPCC                     : 0
- 0x054e (1358) I 00000000 PaddingAPCC                     : 0
- 0x0552 (1362) I 00000000 PaddingAPCC                     : 0
- 0x0556 (1366) I 00000000 PaddingAPCC                     : 0
- 0x055a (1370) H     0000 VDDGFX_TVmin                    : 0
- 0x055c (1372) H     0000 VDDSOC_TVmin                    : 0
- 0x055e (1374) H     0000 VDDGFX_Vmin_HiTemp              : 0
- 0x0560 (1376) H     0000 VDDGFX_Vmin_LoTemp              : 0
- 0x0562 (1378) H     0000 VDDSOC_Vmin_HiTemp              : 0
- 0x0564 (1380) H     0000 VDDSOC_Vmin_LoTemp              : 0
- 0x0566 (1382) H     0000 VDDGFX_TVminHystersis           : 0
- 0x0568 (1384) H     0000 VDDSOC_TVminHystersis           : 0
- 0x056a (1386) I 00000000 BtcConfig                       : 0
- 0x056e (1390) H     a901 SsFmin                          : 425
- 0x0570 (1392) H     8700 SsFmin                          : 135
- 0x0572 (1394) H     8700 SsFmin                          : 135
- 0x0574 (1396) H     0000 SsFmin                          : 0
- 0x0576 (1398) H     0000 SsFmin                          : 0
- 0x0578 (1400) H     0000 SsFmin                          : 0
- 0x057a (1402) H     0000 SsFmin                          : 0
- 0x057c (1404) H     0000 SsFmin                          : 0
- 0x057e (1406) H     0000 SsFmin                          : 0
- 0x0580 (1408) H     0000 SsFmin                          : 0
- 0x0582 (1410) H     1900 DcBtcGb                         : 25
- 0x0584 (1412) H     1900 DcBtcGb                         : 25
- 0x0586 (1414) I 00000000 Reserved                        : 0
- 0x058a (1418) I 00000000 Reserved                        : 0
- 0x058e (1422) I 00000000 Reserved                        : 0
- 0x0592 (1426) I 00000000 Reserved                        : 0
- 0x0596 (1430) I 00000000 Reserved                        : 0
- 0x059a (1434) I 00000000 Reserved                        : 0
- 0x059e (1438) I 00000000 Reserved                        : 0
- 0x05a2 (1442) I 00000000 Reserved                        : 0
- 0x05a6 (1446) B       00 Enabled                         : 0
- 0x05a7 (1447) B       00 Speed                           : 0
- 0x05a8 (1448) B       00 Padding                         : 0
- 0x05a9 (1449) B       00 Padding                         : 0
- 0x05aa (1450) I 00000000 SlaveAddress                    : 0
- 0x05ae (1454) B       00 ControllerPort                  : 0
- 0x05af (1455) B       00 ControllerName                  : 0
- 0x05b0 (1456) B       00 ThermalThrotter                 : 0
- 0x05b1 (1457) B       00 I2cProtocol                     : 0
- 0x05b2 (1458) B       00 Enabled                         : 0
- 0x05b3 (1459) B       00 Speed                           : 0
- 0x05b4 (1460) B       00 Padding                         : 0
- 0x05b5 (1461) B       00 Padding                         : 0
- 0x05b6 (1462) I 00000000 SlaveAddress                    : 0
- 0x05ba (1466) B       00 ControllerPort                  : 0
- 0x05bb (1467) B       00 ControllerName                  : 0
- 0x05bc (1468) B       00 ThermalThrotter                 : 0
- 0x05bd (1469) B       00 I2cProtocol                     : 0
- 0x05be (1470) B       00 Enabled                         : 0
- 0x05bf (1471) B       00 Speed                           : 0
- 0x05c0 (1472) B       00 Padding                         : 0
- 0x05c1 (1473) B       00 Padding                         : 0
- 0x05c2 (1474) I 00000000 SlaveAddress                    : 0
- 0x05c6 (1478) B       00 ControllerPort                  : 0
- 0x05c7 (1479) B       00 ControllerName                  : 0
- 0x05c8 (1480) B       00 ThermalThrotter                 : 0
- 0x05c9 (1481) B       00 I2cProtocol                     : 0
- 0x05ca (1482) B       00 Enabled                         : 0
- 0x05cb (1483) B       00 Speed                           : 0
- 0x05cc (1484) B       00 Padding                         : 0
- 0x05cd (1485) B       00 Padding                         : 0
- 0x05ce (1486) I 00000000 SlaveAddress                    : 0
- 0x05d2 (1490) B       00 ControllerPort                  : 0
- 0x05d3 (1491) B       00 ControllerName                  : 0
- 0x05d4 (1492) B       00 ThermalThrotter                 : 0
- 0x05d5 (1493) B       00 I2cProtocol                     : 0
- 0x05d6 (1494) B       00 Enabled                         : 0
- 0x05d7 (1495) B       00 Speed                           : 0
- 0x05d8 (1496) B       00 Padding                         : 0
- 0x05d9 (1497) B       00 Padding                         : 0
- 0x05da (1498) I 00000000 SlaveAddress                    : 0
- 0x05de (1502) B       00 ControllerPort                  : 0
- 0x05df (1503) B       00 ControllerName                  : 0
- 0x05e0 (1504) B       00 ThermalThrotter                 : 0
- 0x05e1 (1505) B       00 I2cProtocol                     : 0
- 0x05e2 (1506) B       00 Enabled                         : 0
- 0x05e3 (1507) B       00 Speed                           : 0
- 0x05e4 (1508) B       00 Padding                         : 0
- 0x05e5 (1509) B       00 Padding                         : 0
- 0x05e6 (1510) I 00000000 SlaveAddress                    : 0
- 0x05ea (1514) B       00 ControllerPort                  : 0
- 0x05eb (1515) B       00 ControllerName                  : 0
- 0x05ec (1516) B       00 ThermalThrotter                 : 0
- 0x05ed (1517) B       00 I2cProtocol                     : 0
- 0x05ee (1518) B       00 Enabled                         : 0
- 0x05ef (1519) B       00 Speed                           : 0
- 0x05f0 (1520) B       00 Padding                         : 0
- 0x05f1 (1521) B       00 Padding                         : 0
- 0x05f2 (1522) I 00000000 SlaveAddress                    : 0
- 0x05f6 (1526) B       00 ControllerPort                  : 0
- 0x05f7 (1527) B       00 ControllerName                  : 0
- 0x05f8 (1528) B       00 ThermalThrotter                 : 0
- 0x05f9 (1529) B       00 I2cProtocol                     : 0
- 0x05fa (1530) B       00 Enabled                         : 0
- 0x05fb (1531) B       00 Speed                           : 0
- 0x05fc (1532) B       00 Padding                         : 0
- 0x05fd (1533) B       00 Padding                         : 0
- 0x05fe (1534) I 00000000 SlaveAddress                    : 0
- 0x0602 (1538) B       00 ControllerPort                  : 0
- 0x0603 (1539) B       00 ControllerName                  : 0
- 0x0604 (1540) B       00 ThermalThrotter                 : 0
- 0x0605 (1541) B       00 I2cProtocol                     : 0
- 0x0606 (1542) H     0000 MaxVoltageStepGfx               : 0
- 0x0608 (1544) H     0000 MaxVoltageStepSoc               : 0
- 0x060a (1546) B       00 VddGfxVrMapping                 : 0
- 0x060b (1547) B       00 VddSocVrMapping                 : 0
- 0x060c (1548) B       00 VddMem0VrMapping                : 0
- 0x060d (1549) B       00 VddMem1VrMapping                : 0
- 0x060e (1550) B       00 GfxUlvPhaseSheddingMask         : 0
- 0x060f (1551) B       00 SocUlvPhaseSheddingMask         : 0
- 0x0610 (1552) B       00 ExternalSensorPresent           : 0
- 0x0611 (1553) B       00 Padding8_V                      : 0
- 0x0612 (1554) H     0000 GfxMaxCurrent                   : 0
- 0x0614 (1556) b       00 GfxOffset                       : 0
- 0x0615 (1557) B       00 Padding_TelemetryGfx            : 0
- 0x0616 (1558) H     0000 SocMaxCurrent                   : 0
- 0x0618 (1560) b       00 SocOffset                       : 0
- 0x0619 (1561) B       00 Padding_TelemetrySoc            : 0
- 0x061a (1562) H     0000 Mem0MaxCurrent                  : 0
- 0x061c (1564) b       00 Mem0Offset                      : 0
- 0x061d (1565) B       00 Padding_TelemetryMem0           : 0
- 0x061e (1566) H     0000 Mem1MaxCurrent                  : 0
- 0x0620 (1568) b       00 Mem1Offset                      : 0
- 0x0621 (1569) B       00 Padding_TelemetryMem1           : 0
- 0x0622 (1570) B       00 AcDcGpio                        : 0
- 0x0623 (1571) B       00 AcDcPolarity                    : 0
- 0x0624 (1572) B       00 VR0HotGpio                      : 0
- 0x0625 (1573) B       00 VR0HotPolarity                  : 0
- 0x0626 (1574) B       00 VR1HotGpio                      : 0
- 0x0627 (1575) B       00 VR1HotPolarity                  : 0
- 0x0628 (1576) B       00 GthrGpio                        : 0
- 0x0629 (1577) B       00 GthrPolarity                    : 0
- 0x062a (1578) B       00 LedPin0                         : 0
- 0x062b (1579) B       00 LedPin1                         : 0
- 0x062c (1580) B       00 LedPin2                         : 0
- 0x062d (1581) B       00 padding8_4                      : 0
- 0x062e (1582) B       00 PllGfxclkSpreadEnabled          : 0
- 0x062f (1583) B       00 PllGfxclkSpreadPercent          : 0
- 0x0630 (1584) H     0000 PllGfxclkSpreadFreq             : 0
- 0x0632 (1586) B       00 DfllGfxclkSpreadEnabled         : 0
- 0x0633 (1587) B       00 DfllGfxclkSpreadPercent         : 0
- 0x0634 (1588) H     0000 DfllGfxclkSpreadFreq            : 0
- 0x0636 (1590) B       00 UclkSpreadEnabled               : 0
- 0x0637 (1591) B       00 UclkSpreadPercent               : 0
- 0x0638 (1592) H     0000 UclkSpreadFreq                  : 0
- 0x063a (1594) B       00 SoclkSpreadEnabled              : 0
- 0x063b (1595) B       00 SocclkSpreadPercent             : 0
- 0x063c (1596) H     0000 SocclkSpreadFreq                : 0
- 0x063e (1598) H     0000 TotalBoardPower                 : 0
- 0x0640 (1600) H     0000 BoardPadding                    : 0
- 0x0642 (1602) I 00000000 MvddRatio                       : 0
- 0x0646 (1606) B       00 RenesesLoadLineEnabled          : 0
- 0x0647 (1607) B       00 GfxLoadlineResistance           : 0
- 0x0648 (1608) B       00 SocLoadlineResistance           : 0
- 0x0649 (1609) B       00 Padding8_Loadline               : 0
- 0x064a (1610) I 00000000 BoardReserved                   : 0
- 0x064e (1614) I 00000000 BoardReserved                   : 0
- 0x0652 (1618) I 00000000 BoardReserved                   : 0
- 0x0656 (1622) I 00000000 BoardReserved                   : 0
- 0x065a (1626) I 00000000 BoardReserved                   : 0
- 0x065e (1630) I 00000000 BoardReserved                   : 0
- 0x0662 (1634) I 00000000 BoardReserved                   : 0
- 0x0666 (1638) I 00000000 BoardReserved                   : 0
- 0x066a (1642) I 00000000 MmHubPadding                    : 0
- 0x066e (1646) I 00000000 MmHubPadding                    : 0
- 0x0672 (1650) I 00000000 MmHubPadding                    : 0
- 0x0676 (1654) I 00000000 MmHubPadding                    : 0
- 0x067a (1658) I 00000000 MmHubPadding                    : 0
- 0x067e (1662) I 00000000 MmHubPadding                    : 0
- 0x0682 (1666) I 00000000 MmHubPadding                    : 0
- 0x0686 (1670) I 00000000 MmHubPadding                    : 0
+PowerPlay table rev 11.0 size 1730 bytes
+ Offset (dec.) t Raw val. Variable name                         Decoded value
+------------------------------------------------------------------------------
+ 0x0000 (0000) H     c206 structuresize                             : 1730
+ 0x0002 (0002) B       0b format_revision                           : 11
+ 0x0003 (0003) B       00 content_revision                          : 0
+ 0x0004 (0004) B       02 TableRevision                             : 2
+ 0x0005 (0005) H     c206 TableSize                                 : 1730
+ 0x0007 (0007) I 34080000 GoldenPPID                                : 2100
+ 0x000b (0011) I a4350000 GoldenRevision                            : 13732
+ 0x000f (0015) H     7c00 FormatID                                  : 124
+ 0x0011 (0017) I 09000000 PlatformCaps                              : 9
+ 0x0015 (0021) B       1a ThermalControllerType                     : 26
+ 0x0016 (0022) H     fa00 SmallPowerLimit1                          : 250
+ 0x0018 (0024) H     fa00 SmallPowerLimit2                          : 250
+ 0x001a (0026) H     fa00 BoostPowerLimit                           : 250
+ 0x001c (0028) H     0000 ODTurboPowerLimit                         : 0
+ 0x001e (0030) H     0000 ODPowerSavePowerLimit                     : 0
+ 0x0020 (0032) H     7600 SoftwareShutdownTemp                      : 118
+ 0x0022 (0034) B       01 TableRevision                             : 1
+ 0x0023 (0035) I 0b000000 PowerSavingClockCount                     : 11
+ 0x0027 (0039) I 09070000 PowerSavingClockMax                       : 1801
+ 0x002b (0043) I 6e040000 PowerSavingClockMax                       : 1134
+ 0x002f (0047) I cc030000 PowerSavingClockMax                       : 972
+ 0x0033 (0051) I cc030000 PowerSavingClockMax                       : 972
+ 0x0037 (0055) I cc030000 PowerSavingClockMax                       : 972
+ 0x003b (0059) I e8030000 PowerSavingClockMax                       : 1000
+ 0x003f (0063) I c9040000 PowerSavingClockMax                       : 1225
+ 0x0043 (0067) I 6e040000 PowerSavingClockMax                       : 1134
+ 0x0047 (0071) I 6e040000 PowerSavingClockMax                       : 1134
+ 0x004b (0075) I 34040000 PowerSavingClockMax                       : 1076
+ 0x004f (0079) I 2a030000 PowerSavingClockMax                       : 810
+ 0x0053 (0083) I 00000000 PowerSavingClockMax                       : 0
+ 0x0057 (0087) I 00000000 PowerSavingClockMax                       : 0
+ 0x005b (0091) I 00000000 PowerSavingClockMax                       : 0
+ 0x005f (0095) I 00000000 PowerSavingClockMax                       : 0
+ 0x0063 (0099) I 00000000 PowerSavingClockMax                       : 0
+ 0x0067 (0103) I bc020000 PowerSavingClockMin                       : 700
+ 0x006b (0107) I 66010000 PowerSavingClockMin                       : 358
+ 0x006f (0111) I 36010000 PowerSavingClockMin                       : 310
+ 0x0073 (0115) I 36010000 PowerSavingClockMin                       : 310
+ 0x0077 (0119) I 36010000 PowerSavingClockMin                       : 310
+ 0x007b (0123) I 5e010000 PowerSavingClockMin                       : 350
+ 0x007f (0127) I 26020000 PowerSavingClockMin                       : 550
+ 0x0083 (0131) I 66010000 PowerSavingClockMin                       : 358
+ 0x0087 (0135) I 66010000 PowerSavingClockMin                       : 358
+ 0x008b (0139) I 93000000 PowerSavingClockMin                       : 147
+ 0x008f (0143) I 0e010000 PowerSavingClockMin                       : 270
+ 0x0093 (0147) I 00000000 PowerSavingClockMin                       : 0
+ 0x0097 (0151) I 00000000 PowerSavingClockMin                       : 0
+ 0x009b (0155) I 00000000 PowerSavingClockMin                       : 0
+ 0x009f (0159) I 00000000 PowerSavingClockMin                       : 0
+ 0x00a3 (0163) I 00000000 PowerSavingClockMin                       : 0
+ 0x00a7 (0167) B       01 ODTableRevision                           : 1
+ 0x00a8 (0168) I 0e000000 ODFeatureCount                            : 14
+ 0x00ac (0172) B       01 ODFeatureCapabilities                     : 1
+ 0x00ad (0173) B       01 ODFeatureCapabilities                     : 1
+ 0x00ae (0174) B       01 ODFeatureCapabilities                     : 1
+ 0x00af (0175) B       01 ODFeatureCapabilities                     : 1
+ 0x00b0 (0176) B       01 ODFeatureCapabilities                     : 1
+ 0x00b1 (0177) B       01 ODFeatureCapabilities                     : 1
+ 0x00b2 (0178) B       01 ODFeatureCapabilities                     : 1
+ 0x00b3 (0179) B       01 ODFeatureCapabilities                     : 1
+ 0x00b4 (0180) B       01 ODFeatureCapabilities                     : 1
+ 0x00b5 (0181) B       00 ODFeatureCapabilities                     : 0
+ 0x00b6 (0182) B       01 ODFeatureCapabilities                     : 1
+ 0x00b7 (0183) B       01 ODFeatureCapabilities                     : 1
+ 0x00b8 (0184) B       01 ODFeatureCapabilities                     : 1
+ 0x00b9 (0185) B       01 ODFeatureCapabilities                     : 1
+ 0x00ba (0186) B       00 ODFeatureCapabilities                     : 0
+ 0x00bb (0187) B       00 ODFeatureCapabilities                     : 0
+ 0x00bc (0188) B       00 ODFeatureCapabilities                     : 0
+ 0x00bd (0189) B       00 ODFeatureCapabilities                     : 0
+ 0x00be (0190) B       00 ODFeatureCapabilities                     : 0
+ 0x00bf (0191) B       00 ODFeatureCapabilities                     : 0
+ 0x00c0 (0192) B       00 ODFeatureCapabilities                     : 0
+ 0x00c1 (0193) B       00 ODFeatureCapabilities                     : 0
+ 0x00c2 (0194) B       00 ODFeatureCapabilities                     : 0
+ 0x00c3 (0195) B       00 ODFeatureCapabilities                     : 0
+ 0x00c4 (0196) B       00 ODFeatureCapabilities                     : 0
+ 0x00c5 (0197) B       00 ODFeatureCapabilities                     : 0
+ 0x00c6 (0198) B       00 ODFeatureCapabilities                     : 0
+ 0x00c7 (0199) B       00 ODFeatureCapabilities                     : 0
+ 0x00c8 (0200) B       00 ODFeatureCapabilities                     : 0
+ 0x00c9 (0201) B       00 ODFeatureCapabilities                     : 0
+ 0x00ca (0202) B       00 ODFeatureCapabilities                     : 0
+ 0x00cb (0203) B       00 ODFeatureCapabilities                     : 0
+ 0x00cc (0204) I 1d000000 ODSettingCount                            : 29
+ 0x00d0 (0208) I 98080000 ODSettingsMax                             : 2200
+ 0x00d4 (0212) I 98080000 ODSettingsMax                             : 2200
+ 0x00d8 (0216) I 98080000 ODSettingsMax                             : 2200
+ 0x00dc (0220) I c2040000 ODSettingsMax                             : 1218
+ 0x00e0 (0224) I 98080000 ODSettingsMax                             : 2200
+ 0x00e4 (0228) I c2040000 ODSettingsMax                             : 1218
+ 0x00e8 (0232) I 98080000 ODSettingsMax                             : 2200
+ 0x00ec (0236) I c2040000 ODSettingsMax                             : 1218
+ 0x00f0 (0240) I b0040000 ODSettingsMax                             : 1200
+ 0x00f4 (0244) I 14000000 ODSettingsMax                             : 20
+ 0x00f8 (0248) I 0a0f0000 ODSettingsMax                             : 3850
+ 0x00fc (0252) I 0a0f0000 ODSettingsMax                             : 3850
+ 0x0100 (0256) I 5f000000 ODSettingsMax                             : 95
+ 0x0104 (0260) I 6e000000 ODSettingsMax                             : 110
+ 0x0108 (0264) I 02000000 ODSettingsMax                             : 2
+ 0x010c (0268) I 00000000 ODSettingsMax                             : 0
+ 0x0110 (0272) I 01000000 ODSettingsMax                             : 1
+ 0x0114 (0276) I 01000000 ODSettingsMax                             : 1
+ 0x0118 (0280) I 01000000 ODSettingsMax                             : 1
+ 0x011c (0284) I 5f000000 ODSettingsMax                             : 95
+ 0x0120 (0288) I 64000000 ODSettingsMax                             : 100
+ 0x0124 (0292) I 5f000000 ODSettingsMax                             : 95
+ 0x0128 (0296) I 64000000 ODSettingsMax                             : 100
+ 0x012c (0300) I 5f000000 ODSettingsMax                             : 95
+ 0x0130 (0304) I 64000000 ODSettingsMax                             : 100
+ 0x0134 (0308) I 5f000000 ODSettingsMax                             : 95
+ 0x0138 (0312) I 64000000 ODSettingsMax                             : 100
+ 0x013c (0316) I 5f000000 ODSettingsMax                             : 95
+ 0x0140 (0320) I 64000000 ODSettingsMax                             : 100
+ 0x0144 (0324) I 00000000 ODSettingsMax                             : 0
+ 0x0148 (0328) I 00000000 ODSettingsMax                             : 0
+ 0x014c (0332) I 00000000 ODSettingsMax                             : 0
+ 0x0150 (0336) I 28030000 ODSettingsMin                             : 808
+ 0x0154 (0340) I 28030000 ODSettingsMin                             : 808
+ 0x0158 (0344) I 28030000 ODSettingsMin                             : 808
+ 0x015c (0348) I e2020000 ODSettingsMin                             : 738
+ 0x0160 (0352) I 28030000 ODSettingsMin                             : 808
+ 0x0164 (0356) I e2020000 ODSettingsMin                             : 738
+ 0x0168 (0360) I 28030000 ODSettingsMin                             : 808
+ 0x016c (0364) I e2020000 ODSettingsMin                             : 738
+ 0x0170 (0368) I 5e010000 ODSettingsMin                             : 350
+ 0x0174 (0372) I 14000000 ODSettingsMin                             : 20
+ 0x0178 (0376) I c2010000 ODSettingsMin                             : 450
+ 0x017c (0380) I c2010000 ODSettingsMin                             : 450
+ 0x0180 (0384) I 19000000 ODSettingsMin                             : 25
+ 0x0184 (0388) I 32000000 ODSettingsMin                             : 50
+ 0x0188 (0392) I 00000000 ODSettingsMin                             : 0
+ 0x018c (0396) I 00000000 ODSettingsMin                             : 0
+ 0x0190 (0400) I 00000000 ODSettingsMin                             : 0
+ 0x0194 (0404) I 00000000 ODSettingsMin                             : 0
+ 0x0198 (0408) I 00000000 ODSettingsMin                             : 0
+ 0x019c (0412) I 19000000 ODSettingsMin                             : 25
+ 0x01a0 (0416) I 14000000 ODSettingsMin                             : 20
+ 0x01a4 (0420) I 19000000 ODSettingsMin                             : 25
+ 0x01a8 (0424) I 14000000 ODSettingsMin                             : 20
+ 0x01ac (0428) I 19000000 ODSettingsMin                             : 25
+ 0x01b0 (0432) I 14000000 ODSettingsMin                             : 20
+ 0x01b4 (0436) I 19000000 ODSettingsMin                             : 25
+ 0x01b8 (0440) I 14000000 ODSettingsMin                             : 20
+ 0x01bc (0444) I 19000000 ODSettingsMin                             : 25
+ 0x01c0 (0448) I 14000000 ODSettingsMin                             : 20
+ 0x01c4 (0452) I 00000000 ODSettingsMin                             : 0
+ 0x01c8 (0456) I 00000000 ODSettingsMin                             : 0
+ 0x01cc (0460) I 00000000 ODSettingsMin                             : 0
+ 0x01d0 (0464) H     0000 Reserve                                   : 0
+ 0x01d2 (0466) H     0000 Reserve                                   : 0
+ 0x01d4 (0468) H     0000 Reserve                                   : 0
+ 0x01d6 (0470) H     0000 Reserve                                   : 0
+ 0x01d8 (0472) H     0000 Reserve                                   : 0
+ 0x01da (0474) I 03000000 Version                                   : 3
+ 0x01de (0478) I ffeff439 FeaturesToRun                             : 972353535
+ 0x01e2 (0482) I 00000000 FeaturesToRun                             : 0
+ 0x01e6 (0486) H     fa00 SocketPowerLimitAc0                       : 250
+ 0x01e8 (0488) H     0000 SocketPowerLimitAc0Tau                    : 0
+ 0x01ea (0490) H     0000 SocketPowerLimitAc1                       : 0
+ 0x01ec (0492) H     0000 SocketPowerLimitAc1Tau                    : 0
+ 0x01ee (0494) H     0000 SocketPowerLimitAc2                       : 0
+ 0x01f0 (0496) H     0000 SocketPowerLimitAc2Tau                    : 0
+ 0x01f2 (0498) H     0000 SocketPowerLimitAc3                       : 0
+ 0x01f4 (0500) H     0000 SocketPowerLimitAc3Tau                    : 0
+ 0x01f6 (0502) H     fa00 SocketPowerLimitDc                        : 250
+ 0x01f8 (0504) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x01fa (0506) H     3200 TdcLimitSoc                               : 50
+ 0x01fc (0508) H     0000 TdcLimitSocTau                            : 0
+ 0x01fe (0510) H     4a01 TdcLimitGfx                               : 330
+ 0x0200 (0512) H     0000 TdcLimitGfxTau                            : 0
+ 0x0202 (0514) H     6400 TedgeLimit                                : 100
+ 0x0204 (0516) H     6e00 ThotspotLimit                             : 110
+ 0x0206 (0518) H     5e00 ThbmLimit                                 : 94
+ 0x0208 (0520) H     7300 Tvr_gfxLimit                              : 115
+ 0x020a (0522) H     7300 Tvr_memLimit                              : 115
+ 0x020c (0524) H     ffff Tliquid1Limit                             : 65535
+ 0x020e (0526) H     ffff Tliquid2Limit                             : 65535
+ 0x0210 (0528) H     ffff TplxLimit                                 : 65535
+ 0x0212 (0530) I 00000000 FitLimit                                  : 0
+ 0x0216 (0534) H     0000 PpmPowerLimit                             : 0
+ 0x0218 (0536) H     0000 PpmTemperatureThreshold                   : 0
+ 0x021a (0538) B       01 MemoryOnPackage                           : 1
+ 0x021b (0539) B       00 padding8_limits                           : 0
+ 0x021c (0540) H     7300 Tvr_SocLimit                              : 115
+ 0x021e (0542) H     0000 UlvVoltageOffsetSoc                       : 0
+ 0x0220 (0544) H     0000 UlvVoltageOffsetGfx                       : 0
+ 0x0222 (0546) B       00 UlvSmnclkDid                              : 0
+ 0x0223 (0547) B       00 UlvMp1clkDid                              : 0
+ 0x0224 (0548) B       00 UlvGfxclkBypass                           : 0
+ 0x0225 (0549) B       00 Padding234                                : 0
+ 0x0226 (0550) H     860b MinVoltageGfx                             : 2950
+ 0x0228 (0552) H     220b MinVoltageSoc                             : 2850
+ 0x022a (0554) H     0b13 MaxVoltageGfx                             : 4875
+ 0x022c (0556) H     4312 MaxVoltageSoc                             : 4675
+ 0x022e (0558) H     2600 LoadLineResistanceGfx                     : 38
+ 0x0230 (0560) H     0000 LoadLineResistanceSoc                     : 0
+ 0x0232 (0562) B       01 VoltageMode                               : 1
+ 0x0233 (0563) B       01 SnapToDiscrete                            : 1
+ 0x0234 (0564) B       09 NumDiscreteLevels                         : 9
+ 0x0235 (0565) B       00 padding                                   : 0
+ 0x0236 (0566) f 00000000 m                                         : 0
+ 0x023a (0570) f 00000000 b                                         : 0
+ 0x023e (0574) f 5bb1bf3e a                                         : 0.3744
+ 0x0242 (0578) f ec51f8be b                                         :-0.485
+ 0x0246 (0582) f 6519523f c                                         : 0.8207
+ 0x024a (0586) B       00 VoltageMode                               : 0
+ 0x024b (0587) B       01 SnapToDiscrete                            : 1
+ 0x024c (0588) B       08 NumDiscreteLevels                         : 8
+ 0x024d (0589) B       00 padding                                   : 0
+ 0x024e (0590) f 643b9f3f m                                         : 1.244
+ 0x0252 (0594) f 16dea5bd b                                         :-0.08099
+ 0x0256 (0598) f 00000000 a                                         : 0
+ 0x025a (0602) f 00000000 b                                         : 0
+ 0x025e (0606) f 00000000 c                                         : 0
+ 0x0262 (0610) B       00 VoltageMode                               : 0
+ 0x0263 (0611) B       01 SnapToDiscrete                            : 1
+ 0x0264 (0612) B       08 NumDiscreteLevels                         : 8
+ 0x0265 (0613) B       00 padding                                   : 0
+ 0x0266 (0614) f 355e9a3f m                                         : 1.206
+ 0x026a (0618) f 8f362e3e b                                         : 0.17013
+ 0x026e (0622) f 00000000 a                                         : 0
+ 0x0272 (0626) f 00000000 b                                         : 0
+ 0x0276 (0630) f 00000000 c                                         : 0
+ 0x027a (0634) B       00 VoltageMode                               : 0
+ 0x027b (0635) B       01 SnapToDiscrete                            : 1
+ 0x027c (0636) B       08 NumDiscreteLevels                         : 8
+ 0x027d (0637) B       00 padding                                   : 0
+ 0x027e (0638) f 696fb03f m                                         : 1.3784
+ 0x0282 (0642) f 4833163d b                                         : 0.03667
+ 0x0286 (0646) f 00000000 a                                         : 0
+ 0x028a (0650) f 00000000 b                                         : 0
+ 0x028e (0654) f 00000000 c                                         : 0
+ 0x0292 (0658) B       00 VoltageMode                               : 0
+ 0x0293 (0659) B       01 SnapToDiscrete                            : 1
+ 0x0294 (0660) B       08 NumDiscreteLevels                         : 8
+ 0x0295 (0661) B       00 padding                                   : 0
+ 0x0296 (0662) f e561a13f m                                         : 1.2608
+ 0x029a (0666) f 12f758bd b                                         :-0.05297
+ 0x029e (0670) f 00000000 a                                         : 0
+ 0x02a2 (0674) f 00000000 b                                         : 0
+ 0x02a6 (0678) f 00000000 c                                         : 0
+ 0x02aa (0682) B       00 VoltageMode                               : 0
+ 0x02ab (0683) B       01 SnapToDiscrete                            : 1
+ 0x02ac (0684) B       03 NumDiscreteLevels                         : 3
+ 0x02ad (0685) B       00 padding                                   : 0
+ 0x02ae (0686) f b515833f m                                         : 1.0241
+ 0x02b2 (0690) f c2dd193e b                                         : 0.15026
+ 0x02b6 (0694) f 00000000 a                                         : 0
+ 0x02ba (0698) f 00000000 b                                         : 0
+ 0x02be (0702) f 00000000 c                                         : 0
+ 0x02c2 (0706) B       00 VoltageMode                               : 0
+ 0x02c3 (0707) B       01 SnapToDiscrete                            : 1
+ 0x02c4 (0708) B       08 NumDiscreteLevels                         : 8
+ 0x02c5 (0709) B       00 padding                                   : 0
+ 0x02c6 (0710) f 8638863f m                                         : 1.0486
+ 0x02ca (0714) f 0ebe303e b                                         : 0.1726
+ 0x02ce (0718) f 00000000 a                                         : 0
+ 0x02d2 (0722) f 00000000 b                                         : 0
+ 0x02d6 (0726) f 00000000 c                                         : 0
+ 0x02da (0730) B       00 VoltageMode                               : 0
+ 0x02db (0731) B       01 SnapToDiscrete                            : 1
+ 0x02dc (0732) B       08 NumDiscreteLevels                         : 8
+ 0x02dd (0733) B       00 padding                                   : 0
+ 0x02de (0734) f 83c05a3f m                                         : 0.8545
+ 0x02e2 (0738) f 4da1f33d b                                         : 0.11896
+ 0x02e6 (0742) f 00000000 a                                         : 0
+ 0x02ea (0746) f 00000000 b                                         : 0
+ 0x02ee (0750) f 00000000 c                                         : 0
+ 0x02f2 (0754) B       02 VoltageMode                               : 2
+ 0x02f3 (0755) B       01 SnapToDiscrete                            : 1
+ 0x02f4 (0756) B       08 NumDiscreteLevels                         : 8
+ 0x02f5 (0757) B       00 padding                                   : 0
+ 0x02f6 (0758) f 00000000 m                                         : 0
+ 0x02fa (0762) f 00000000 b                                         : 0
+ 0x02fe (0766) f a4708d3f a                                         : 1.105
+ 0x0302 (0770) f e41485bf b                                         :-1.0397
+ 0x0306 (0774) f d5e7323f c                                         : 0.69885
+ 0x030a (0778) B       02 VoltageMode                               : 2
+ 0x030b (0779) B       01 SnapToDiscrete                            : 1
+ 0x030c (0780) B       03 NumDiscreteLevels                         : 3
+ 0x030d (0781) B       00 padding                                   : 0
+ 0x030e (0782) f 00000000 m                                         : 0
+ 0x0312 (0786) f 00000000 b                                         : 0
+ 0x0316 (0790) f 00000000 a                                         : 0
+ 0x031a (0794) f 00000000 b                                         : 0
+ 0x031e (0798) f d5e7323f c                                         : 0.69885
+ 0x0322 (0802) B       01 VoltageMode                               : 1
+ 0x0323 (0803) B       01 SnapToDiscrete                            : 1
+ 0x0324 (0804) B       08 NumDiscreteLevels                         : 8
+ 0x0325 (0805) B       00 padding                                   : 0
+ 0x0326 (0806) f 0000803f m                                         : 1
+ 0x032a (0810) f 00000000 b                                         : 0
+ 0x032e (0814) f d191fc3e a                                         : 0.4933
+ 0x0332 (0818) f 1f852bbf b                                         :-0.67
+ 0x0336 (0822) f 3277753f c                                         : 0.95885
+ 0x033a (0826) H     bc02 FreqTableGfx                              : 700
+ 0x033c (0828) H     2803 FreqTableGfx                              : 808
+ 0x033e (0830) H     6e04 FreqTableGfx                              : 1134
+ 0x0340 (0832) H     5c05 FreqTableGfx                              : 1372
+ 0x0342 (0834) H     0a06 FreqTableGfx                              : 1546
+ 0x0344 (0836) H     9306 FreqTableGfx                              : 1683
+ 0x0346 (0838) H     d506 FreqTableGfx                              : 1749
+ 0x0348 (0840) H     ed06 FreqTableGfx                              : 1773
+ 0x034a (0842) H     0907 FreqTableGfx                              : 1801
+ 0x034c (0844) H     0000 FreqTableGfx                              : 0
+ 0x034e (0846) H     0000 FreqTableGfx                              : 0
+ 0x0350 (0848) H     0000 FreqTableGfx                              : 0
+ 0x0352 (0850) H     0000 FreqTableGfx                              : 0
+ 0x0354 (0852) H     0000 FreqTableGfx                              : 0
+ 0x0356 (0854) H     0000 FreqTableGfx                              : 0
+ 0x0358 (0856) H     0000 FreqTableGfx                              : 0
+ 0x035a (0858) H     6601 FreqTableVclk                             : 358
+ 0x035c (0860) H     e601 FreqTableVclk                             : 486
+ 0x035e (0862) H     6b02 FreqTableVclk                             : 619
+ 0x0360 (0864) H     f402 FreqTableVclk                             : 756
+ 0x0362 (0866) H     5203 FreqTableVclk                             : 850
+ 0x0364 (0868) H     cc03 FreqTableVclk                             : 972
+ 0x0366 (0870) H     6e04 FreqTableVclk                             : 1134
+ 0x0368 (0872) H     6e04 FreqTableVclk                             : 1134
+ 0x036a (0874) H     3601 FreqTableDclk                             : 310
+ 0x036c (0876) H     9001 FreqTableDclk                             : 400
+ 0x036e (0878) H     0c02 FreqTableDclk                             : 524
+ 0x0370 (0880) H     6b02 FreqTableDclk                             : 619
+ 0x0372 (0882) H     a802 FreqTableDclk                             : 680
+ 0x0374 (0884) H     f402 FreqTableDclk                             : 756
+ 0x0376 (0886) H     5203 FreqTableDclk                             : 850
+ 0x0378 (0888) H     cc03 FreqTableDclk                             : 972
+ 0x037a (0890) H     3601 FreqTableEclk                             : 310
+ 0x037c (0892) H     9001 FreqTableEclk                             : 400
+ 0x037e (0894) H     0c02 FreqTableEclk                             : 524
+ 0x0380 (0896) H     6b02 FreqTableEclk                             : 619
+ 0x0382 (0898) H     a802 FreqTableEclk                             : 680
+ 0x0384 (0900) H     f402 FreqTableEclk                             : 756
+ 0x0386 (0902) H     5203 FreqTableEclk                             : 850
+ 0x0388 (0904) H     cc03 FreqTableEclk                             : 972
+ 0x038a (0906) H     3601 FreqTableSocclk                           : 310
+ 0x038c (0908) H     0c02 FreqTableSocclk                           : 524
+ 0x038e (0910) H     3702 FreqTableSocclk                           : 567
+ 0x0390 (0912) H     6b02 FreqTableSocclk                           : 619
+ 0x0392 (0914) H     a802 FreqTableSocclk                           : 680
+ 0x0394 (0916) H     f402 FreqTableSocclk                           : 756
+ 0x0396 (0918) H     5203 FreqTableSocclk                           : 850
+ 0x0398 (0920) H     cc03 FreqTableSocclk                           : 972
+ 0x039a (0922) H     5e01 FreqTableUclk                             : 350
+ 0x039c (0924) H     2003 FreqTableUclk                             : 800
+ 0x039e (0926) H     e803 FreqTableUclk                             : 1000
+ 0x03a0 (0928) H     e803 FreqTableUclk                             : 1000
+ 0x03a2 (0930) H     2602 FreqTableFclk                             : 550
+ 0x03a4 (0932) H     6202 FreqTableFclk                             : 610
+ 0x03a6 (0934) H     b202 FreqTableFclk                             : 690
+ 0x03a8 (0936) H     f802 FreqTableFclk                             : 760
+ 0x03aa (0938) H     6603 FreqTableFclk                             : 870
+ 0x03ac (0940) H     c003 FreqTableFclk                             : 960
+ 0x03ae (0942) H     3804 FreqTableFclk                             : 1080
+ 0x03b0 (0944) H     c904 FreqTableFclk                             : 1225
+ 0x03b2 (0946) H     6601 FreqTableDcefclk                          : 358
+ 0x03b4 (0948) H     c601 FreqTableDcefclk                          : 454
+ 0x03b6 (0950) H     3702 FreqTableDcefclk                          : 567
+ 0x03b8 (0952) H     a802 FreqTableDcefclk                          : 680
+ 0x03ba (0954) H     f402 FreqTableDcefclk                          : 756
+ 0x03bc (0956) H     5203 FreqTableDcefclk                          : 850
+ 0x03be (0958) H     cc03 FreqTableDcefclk                          : 972
+ 0x03c0 (0960) H     6e04 FreqTableDcefclk                          : 1134
+ 0x03c2 (0962) H     6601 FreqTableDispclk                          : 358
+ 0x03c4 (0964) H     c601 FreqTableDispclk                          : 454
+ 0x03c6 (0966) H     3702 FreqTableDispclk                          : 567
+ 0x03c8 (0968) H     a802 FreqTableDispclk                          : 680
+ 0x03ca (0970) H     f402 FreqTableDispclk                          : 756
+ 0x03cc (0972) H     5203 FreqTableDispclk                          : 850
+ 0x03ce (0974) H     cc03 FreqTableDispclk                          : 972
+ 0x03d0 (0976) H     6e04 FreqTableDispclk                          : 1134
+ 0x03d2 (0978) H     9300 FreqTablePixclk                           : 147
+ 0x03d4 (0980) H     f200 FreqTablePixclk                           : 242
+ 0x03d6 (0982) H     5801 FreqTablePixclk                           : 344
+ 0x03d8 (0984) H     e401 FreqTablePixclk                           : 484
+ 0x03da (0986) H     1502 FreqTablePixclk                           : 533
+ 0x03dc (0988) H     aa03 FreqTablePixclk                           : 938
+ 0x03de (0990) H     1304 FreqTablePixclk                           : 1043
+ 0x03e0 (0992) H     3404 FreqTablePixclk                           : 1076
+ 0x03e2 (0994) H     0e01 FreqTablePhyclk                           : 270
+ 0x03e4 (0996) H     1c02 FreqTablePhyclk                           : 540
+ 0x03e6 (0998) H     2a03 FreqTablePhyclk                           : 810
+ 0x03e8 (1000) H     0000 FreqTablePhyclk                           : 0
+ 0x03ea (1002) H     0000 FreqTablePhyclk                           : 0
+ 0x03ec (1004) H     0000 FreqTablePhyclk                           : 0
+ 0x03ee (1006) H     0000 FreqTablePhyclk                           : 0
+ 0x03f0 (1008) H     0000 FreqTablePhyclk                           : 0
+ 0x03f2 (1010) H     0907 DcModeMaxFreq                             : 1801
+ 0x03f4 (1012) H     6e04 DcModeMaxFreq                             : 1134
+ 0x03f6 (1014) H     cc03 DcModeMaxFreq                             : 972
+ 0x03f8 (1016) H     cc03 DcModeMaxFreq                             : 972
+ 0x03fa (1018) H     cc03 DcModeMaxFreq                             : 972
+ 0x03fc (1020) H     e803 DcModeMaxFreq                             : 1000
+ 0x03fe (1022) H     6e04 DcModeMaxFreq                             : 1134
+ 0x0400 (1024) H     6e04 DcModeMaxFreq                             : 1134
+ 0x0402 (1026) H     3404 DcModeMaxFreq                             : 1076
+ 0x0404 (1028) H     2a03 DcModeMaxFreq                             : 810
+ 0x0406 (1030) H     c904 DcModeMaxFreq                             : 1225
+ 0x0408 (1032) H     0000 Padding8_Clks                             : 0
+ 0x040a (1034) H     c800 Mp0clkFreq                                : 200
+ 0x040c (1036) H     2c01 Mp0clkFreq                                : 300
+ 0x040e (1038) H     6009 Mp0DpmVoltage                             : 2400
+ 0x0410 (1040) H     f00a Mp0DpmVoltage                             : 2800
+ 0x0412 (1042) H     2803 GfxclkFidle                               : 808
+ 0x0414 (1044) H     0000 GfxclkSlewRate                            : 0
+ 0x0416 (1046) H     0000 CksEnableFreq                             : 0
+ 0x0418 (1048) H     0000 Padding789                                : 0
+ 0x041a (1050) f 00000000 a                                         : 0
+ 0x041e (1054) f 00000000 b                                         : 0
+ 0x0422 (1058) f 00000000 c                                         : 0
+ 0x0426 (1062) B       00 Padding567                                : 0
+ 0x0427 (1063) B       00 Padding567                                : 0
+ 0x0428 (1064) B       00 Padding567                                : 0
+ 0x0429 (1065) B       00 Padding567                                : 0
+ 0x042a (1066) H     0907 GfxclkDsMaxFreq                           : 1801
+ 0x042c (1068) B       01 GfxclkSource                              : 1
+ 0x042d (1069) B       00 Padding456                                : 0
+ 0x042e (1070) B       00 LowestUclkReservedForUlv                  : 0
+ 0x042f (1071) B       00 Padding8_Uclk                             : 0
+ 0x0430 (1072) B       00 Padding8_Uclk                             : 0
+ 0x0431 (1073) B       00 Padding8_Uclk                             : 0
+ 0x0432 (1074) B       00 PcieGenSpeed                              : 0
+ 0x0433 (1075) B       02 PcieGenSpeed                              : 2
+ 0x0434 (1076) B       06 PcieLaneCount                             : 6
+ 0x0435 (1077) B       06 PcieLaneCount                             : 6
+ 0x0436 (1078) H     5000 LclkFreq                                  : 80
+ 0x0438 (1080) H     3401 LclkFreq                                  : 308
+ 0x043a (1082) H     0000 EnableTdpm                                : 0
+ 0x043c (1084) H     0000 TdpmHighHystTemperature                   : 0
+ 0x043e (1086) H     0000 TdpmLowHystTemperature                    : 0
+ 0x0440 (1088) H     0000 GfxclkFreqHighTempLimit                   : 0
+ 0x0442 (1090) H     0000 FanStopTemp                               : 0
+ 0x0444 (1092) H     0000 FanStartTemp                              : 0
+ 0x0446 (1094) H     9001 FanGainEdge                               : 400
+ 0x0448 (1096) H     9001 FanGainHotspot                            : 400
+ 0x044a (1098) H     9001 FanGainLiquid                             : 400
+ 0x044c (1100) H     9001 FanGainVrGfx                              : 400
+ 0x044e (1102) H     9001 FanGainVrSoc                              : 400
+ 0x0450 (1104) H     9001 FanGainPlx                                : 400
+ 0x0452 (1106) H     9001 FanGainHbm                                : 400
+ 0x0454 (1108) H     1400 FanPwmMin                                 : 20
+ 0x0456 (1110) H     540b FanAcousticLimitRpm                       : 2900
+ 0x0458 (1112) H     540b FanThrottlingRpm                          : 2900
+ 0x045a (1114) H     0a0f FanMaximumRpm                             : 3850
+ 0x045c (1116) H     5f00 FanTargetTemperature                      : 95
+ 0x045e (1118) H     0000 FanTargetGfxclk                           : 0
+ 0x0460 (1120) B       00 FanZeroRpmEnable                          : 0
+ 0x0461 (1121) B       02 FanTachEdgePerRev                         : 2
+ 0x0462 (1122) h     0000 FuzzyFan_ErrorSetDelta                    : 0
+ 0x0464 (1124) h     0000 FuzzyFan_ErrorRateSetDelta                : 0
+ 0x0466 (1126) h     0000 FuzzyFan_PwmSetDelta                      : 0
+ 0x0468 (1128) H     0000 FuzzyFan_Reserved                         : 0
+ 0x046a (1130) B       00 OverrideAvfsGb                            : 0
+ 0x046b (1131) B       01 OverrideAvfsGb                            : 1
+ 0x046c (1132) B       00 Padding8_Avfs                             : 0
+ 0x046d (1133) B       00 Padding8_Avfs                             : 0
+ 0x046e (1134) f 00000000 a                                         : 0
+ 0x0472 (1138) f 508d973c b                                         : 0.0185
+ 0x0476 (1142) f 0ad7a33b c                                         : 0.005
+ 0x047a (1146) f 00000000 a                                         : 0
+ 0x047e (1150) f eab2983c b                                         : 0.01864
+ 0x0482 (1154) f 87a2403d c                                         : 0.04703
+ 0x0486 (1158) f 00000000 a                                         : 0
+ 0x048a (1162) f 00000000 b                                         : 0
+ 0x048e (1166) f 00000000 c                                         : 0
+ 0x0492 (1170) f 00000000 a                                         : 0
+ 0x0496 (1174) f 00000000 b                                         : 0
+ 0x049a (1178) f 00000000 c                                         : 0
+ 0x049e (1182) f 00000000 a                                         : 0
+ 0x04a2 (1186) f 00000000 b                                         : 0
+ 0x04a6 (1190) f 00000000 c                                         : 0
+ 0x04aa (1194) f 00000000 a                                         : 0
+ 0x04ae (1198) f 00000000 b                                         : 0
+ 0x04b2 (1202) f 00000000 c                                         : 0
+ 0x04b6 (1206) f 00000000 m                                         : 0
+ 0x04ba (1210) f 00000000 b                                         : 0
+ 0x04be (1214) f 00000000 m                                         : 0
+ 0x04c2 (1218) f 00000000 b                                         : 0
+ 0x04c6 (1222) f 00000000 a                                         : 0
+ 0x04ca (1226) f 00000000 b                                         : 0
+ 0x04ce (1230) f 00000000 c                                         : 0
+ 0x04d2 (1234) f 00000000 a                                         : 0
+ 0x04d6 (1238) f 00000000 b                                         : 0
+ 0x04da (1242) f 00000000 c                                         : 0
+ 0x04de (1246) H     0000 DcTol                                     : 0
+ 0x04e0 (1248) H     a000 DcTol                                     : 160
+ 0x04e2 (1250) B       01 DcBtcEnabled                              : 1
+ 0x04e3 (1251) B       00 DcBtcEnabled                              : 0
+ 0x04e4 (1252) B       00 Padding8_GfxBtc                           : 0
+ 0x04e5 (1253) B       00 Padding8_GfxBtc                           : 0
+ 0x04e6 (1254) h     0000 DcBtcMin                                  : 0
+ 0x04e8 (1256) h     0000 DcBtcMin                                  : 0
+ 0x04ea (1258) H     a000 DcBtcMax                                  : 160
+ 0x04ec (1260) H     0000 DcBtcMax                                  : 0
+ 0x04ee (1262) B       08 XgmiLinkSpeed                             : 8
+ 0x04ef (1263) B       10 XgmiLinkSpeed                             : 16
+ 0x04f0 (1264) B       02 XgmiLinkWidth                             : 2
+ 0x04f1 (1265) B       10 XgmiLinkWidth                             : 16
+ 0x04f2 (1266) H     1a04 XgmiFclkFreq                              : 1050
+ 0x04f4 (1268) H     4c04 XgmiFclkFreq                              : 1100
+ 0x04f6 (1270) H     e803 XgmiUclkFreq                              : 1000
+ 0x04f8 (1272) H     e803 XgmiUclkFreq                              : 1000
+ 0x04fa (1274) H     e803 XgmiSocclkFreq                            : 1000
+ 0x04fc (1276) H     e803 XgmiSocclkFreq                            : 1000
+ 0x04fe (1278) H     0000 XgmiSocVoltage                            : 0
+ 0x0500 (1280) H     0000 XgmiSocVoltage                            : 0
+ 0x0502 (1282) I 00000000 DebugOverrides                            : 0
+ 0x0506 (1286) f 00000000 a                                         : 0
+ 0x050a (1290) f 00000000 b                                         : 0
+ 0x050e (1294) f 00000000 c                                         : 0
+ 0x0512 (1298) f 00000000 a                                         : 0
+ 0x0516 (1302) f 00000000 b                                         : 0
+ 0x051a (1306) f 00000000 c                                         : 0
+ 0x051e (1310) f 00000000 a                                         : 0
+ 0x0522 (1314) f 00000000 b                                         : 0
+ 0x0526 (1318) f 00000000 c                                         : 0
+ 0x052a (1322) f 00000000 a                                         : 0
+ 0x052e (1326) f 00000000 b                                         : 0
+ 0x0532 (1330) f 00000000 c                                         : 0
+ 0x0536 (1334) H     860b MinVoltageUlvGfx                          : 2950
+ 0x0538 (1336) H     220b MinVoltageUlvSoc                          : 2850
+ 0x053a (1338) H     540b MGpuFanBoostLimitRpm                      : 2900
+ 0x053c (1340) H     0000 Fan                                       : 0
+ 0x053e (1342) H     9001 FanGainVrMem0                             : 400
+ 0x0540 (1344) H     9001 FanGainVrMem1                             : 400
+ 0x0542 (1346) H     3800 DcBtcGb                                   : 56
+ 0x0544 (1348) H     0000 DcBtcGb                                   : 0
+ 0x0546 (1350) I 00000000 Reserved                                  : 0
+ 0x054a (1354) I 00000000 Reserved                                  : 0
+ 0x054e (1358) I 00000000 Reserved                                  : 0
+ 0x0552 (1362) I 00000000 Reserved                                  : 0
+ 0x0556 (1366) I 00000000 Reserved                                  : 0
+ 0x055a (1370) I 00000000 Reserved                                  : 0
+ 0x055e (1374) I 00000000 Reserved                                  : 0
+ 0x0562 (1378) I 00000000 Reserved                                  : 0
+ 0x0566 (1382) I 00000000 Reserved                                  : 0
+ 0x056a (1386) I 00000000 Reserved                                  : 0
+ 0x056e (1390) I 00000000 Reserved                                  : 0
+ 0x0572 (1394) I 00000000 Padding32                                 : 0
+ 0x0576 (1398) I 00000000 Padding32                                 : 0
+ 0x057a (1402) I 00000000 Padding32                                 : 0
+ 0x057e (1406) H     0000 MaxVoltageStepGfx                         : 0
+ 0x0580 (1408) H     0000 MaxVoltageStepSoc                         : 0
+ 0x0582 (1410) B       00 VddGfxVrMapping                           : 0
+ 0x0583 (1411) B       00 VddSocVrMapping                           : 0
+ 0x0584 (1412) B       00 VddMem0VrMapping                          : 0
+ 0x0585 (1413) B       00 VddMem1VrMapping                          : 0
+ 0x0586 (1414) B       00 GfxUlvPhaseSheddingMask                   : 0
+ 0x0587 (1415) B       00 SocUlvPhaseSheddingMask                   : 0
+ 0x0588 (1416) B       00 ExternalSensorPresent                     : 0
+ 0x0589 (1417) B       00 Padding8_V                                : 0
+ 0x058a (1418) H     0000 GfxMaxCurrent                             : 0
+ 0x058c (1420) b       00 GfxOffset                                 : 0
+ 0x058d (1421) B       00 Padding_TelemetryGfx                      : 0
+ 0x058e (1422) H     0000 SocMaxCurrent                             : 0
+ 0x0590 (1424) b       00 SocOffset                                 : 0
+ 0x0591 (1425) B       00 Padding_TelemetrySoc                      : 0
+ 0x0592 (1426) H     0000 Mem0MaxCurrent                            : 0
+ 0x0594 (1428) b       00 Mem0Offset                                : 0
+ 0x0595 (1429) B       00 Padding_TelemetryMem0                     : 0
+ 0x0596 (1430) H     0000 Mem1MaxCurrent                            : 0
+ 0x0598 (1432) b       00 Mem1Offset                                : 0
+ 0x0599 (1433) B       00 Padding_TelemetryMem1                     : 0
+ 0x059a (1434) B       00 AcDcGpio                                  : 0
+ 0x059b (1435) B       00 AcDcPolarity                              : 0
+ 0x059c (1436) B       00 VR0HotGpio                                : 0
+ 0x059d (1437) B       00 VR0HotPolarity                            : 0
+ 0x059e (1438) B       00 VR1HotGpio                                : 0
+ 0x059f (1439) B       00 VR1HotPolarity                            : 0
+ 0x05a0 (1440) B       00 Padding1                                  : 0
+ 0x05a1 (1441) B       00 Padding2                                  : 0
+ 0x05a2 (1442) B       00 LedPin0                                   : 0
+ 0x05a3 (1443) B       00 LedPin1                                   : 0
+ 0x05a4 (1444) B       00 LedPin2                                   : 0
+ 0x05a5 (1445) B       00 padding8_4                                : 0
+ 0x05a6 (1446) B       00 PllGfxclkSpreadEnabled                    : 0
+ 0x05a7 (1447) B       00 PllGfxclkSpreadPercent                    : 0
+ 0x05a8 (1448) H     0000 PllGfxclkSpreadFreq                       : 0
+ 0x05aa (1450) B       00 UclkSpreadEnabled                         : 0
+ 0x05ab (1451) B       00 UclkSpreadPercent                         : 0
+ 0x05ac (1452) H     0000 UclkSpreadFreq                            : 0
+ 0x05ae (1454) B       00 FclkSpreadEnabled                         : 0
+ 0x05af (1455) B       00 FclkSpreadPercent                         : 0
+ 0x05b0 (1456) H     0000 FclkSpreadFreq                            : 0
+ 0x05b2 (1458) B       00 FllGfxclkSpreadEnabled                    : 0
+ 0x05b3 (1459) B       00 FllGfxclkSpreadPercent                    : 0
+ 0x05b4 (1460) H     0000 FllGfxclkSpreadFreq                       : 0
+ 0x05b6 (1462) I 00000000 Enabled                                   : 0
+ 0x05ba (1466) I 00000000 SlaveAddress                              : 0
+ 0x05be (1470) I 00000000 ControllerPort                            : 0
+ 0x05c2 (1474) I 00000000 ControllerName                            : 0
+ 0x05c6 (1478) I 00000000 ThermalThrottler                          : 0
+ 0x05ca (1482) I 00000000 I2cProtocol                               : 0
+ 0x05ce (1486) I 00000000 I2cSpeed                                  : 0
+ 0x05d2 (1490) I 00000000 Enabled                                   : 0
+ 0x05d6 (1494) I 00000000 SlaveAddress                              : 0
+ 0x05da (1498) I 00000000 ControllerPort                            : 0
+ 0x05de (1502) I 00000000 ControllerName                            : 0
+ 0x05e2 (1506) I 00000000 ThermalThrottler                          : 0
+ 0x05e6 (1510) I 00000000 I2cProtocol                               : 0
+ 0x05ea (1514) I 00000000 I2cSpeed                                  : 0
+ 0x05ee (1518) I 00000000 Enabled                                   : 0
+ 0x05f2 (1522) I 00000000 SlaveAddress                              : 0
+ 0x05f6 (1526) I 00000000 ControllerPort                            : 0
+ 0x05fa (1530) I 00000000 ControllerName                            : 0
+ 0x05fe (1534) I 00000000 ThermalThrottler                          : 0
+ 0x0602 (1538) I 00000000 I2cProtocol                               : 0
+ 0x0606 (1542) I 00000000 I2cSpeed                                  : 0
+ 0x060a (1546) I 00000000 Enabled                                   : 0
+ 0x060e (1550) I 00000000 SlaveAddress                              : 0
+ 0x0612 (1554) I 00000000 ControllerPort                            : 0
+ 0x0616 (1558) I 00000000 ControllerName                            : 0
+ 0x061a (1562) I 00000000 ThermalThrottler                          : 0
+ 0x061e (1566) I 00000000 I2cProtocol                               : 0
+ 0x0622 (1570) I 00000000 I2cSpeed                                  : 0
+ 0x0626 (1574) I 00000000 Enabled                                   : 0
+ 0x062a (1578) I 00000000 SlaveAddress                              : 0
+ 0x062e (1582) I 00000000 ControllerPort                            : 0
+ 0x0632 (1586) I 00000000 ControllerName                            : 0
+ 0x0636 (1590) I 00000000 ThermalThrottler                          : 0
+ 0x063a (1594) I 00000000 I2cProtocol                               : 0
+ 0x063e (1598) I 00000000 I2cSpeed                                  : 0
+ 0x0642 (1602) I 00000000 Enabled                                   : 0
+ 0x0646 (1606) I 00000000 SlaveAddress                              : 0
+ 0x064a (1610) I 00000000 ControllerPort                            : 0
+ 0x064e (1614) I 00000000 ControllerName                            : 0
+ 0x0652 (1618) I 00000000 ThermalThrottler                          : 0
+ 0x0656 (1622) I 00000000 I2cProtocol                               : 0
+ 0x065a (1626) I 00000000 I2cSpeed                                  : 0
+ 0x065e (1630) I 00000000 Enabled                                   : 0
+ 0x0662 (1634) I 00000000 SlaveAddress                              : 0
+ 0x0666 (1638) I 00000000 ControllerPort                            : 0
+ 0x066a (1642) I 00000000 ControllerName                            : 0
+ 0x066e (1646) I 00000000 ThermalThrottler                          : 0
+ 0x0672 (1650) I 00000000 I2cProtocol                               : 0
+ 0x0676 (1654) I 00000000 I2cSpeed                                  : 0
+ 0x067a (1658) I 00000000 BoardReserved                             : 0
+ 0x067e (1662) I 00000000 BoardReserved                             : 0
+ 0x0682 (1666) I 00000000 BoardReserved                             : 0
+ 0x0686 (1670) I 00000000 BoardReserved                             : 0
+ 0x068a (1674) I 00000000 BoardReserved                             : 0
+ 0x068e (1678) I 00000000 BoardReserved                             : 0
+ 0x0692 (1682) I 00000000 BoardReserved                             : 0
+ 0x0696 (1686) I 00000000 BoardReserved                             : 0
+ 0x069a (1690) I 00000000 BoardReserved                             : 0
+ 0x069e (1694) I 00000000 BoardReserved                             : 0
+ 0x06a2 (1698) I 00000000 MmHubPadding                              : 0
+ 0x06a6 (1702) I 00000000 MmHubPadding                              : 0
+ 0x06aa (1706) I 00000000 MmHubPadding                              : 0
+ 0x06ae (1710) I 00000000 MmHubPadding                              : 0
+ 0x06b2 (1714) I 00000000 MmHubPadding                              : 0
+ 0x06b6 (1718) I 00000000 MmHubPadding                              : 0
+ 0x06ba (1722) I 00000000 MmHubPadding                              : 0
+ 0x06be (1726) I 00000000 MmHubPadding                              : 0
```

### Comparing `upp-0.2.0/test/AMD.RX6900.16384.201104.rom.dump` & `upp-0.2.1/test/AMD.RX6900.16384.201104.rom.dump`

 * *Files 14% similar despite different names*

```diff
@@ -26,72 +26,72 @@
   revision: 1
   reserve:
     reserve 0: 0
     reserve 1: 0
     reserve 2: 0
   count: 13
   max:
-    max 0: 2660
-    max 1: 1200
-    max 2: 1000
-    max 3: 1940
-    max 4: 1266
-    max 5: 1477
-    max 6: 1266
-    max 7: 1477
-    max 8: 1200
-    max 9: 1217
-    max 10: 1217
-    max 11: 810
-    max 12: 1217
+    max 0: 2660 (GFXCLK)
+    max 1: 1200 (SOCCLK)
+    max 2: 1000 (UCLK)
+    max 3: 1940 (FCLK)
+    max 4: 1266 (DCLK_0)
+    max 5: 1477 (VCLK_0)
+    max 6: 1266 (DCLK_1)
+    max 7: 1477 (VCLK_1)
+    max 8: 1200 (DCEFCLK)
+    max 9: 1217 (DISPCLK)
+    max 10: 1217 (PIXCLK)
+    max 11: 810 (PHYCLK)
+    max 12: 1217 (DTBCLK)
     max 13: 0
     max 14: 0
     max 15: 0
   min:
-    min 0: 500
-    min 1: 480
-    min 2: 97
-    min 3: 550
-    min 4: 317
-    min 5: 363
-    min 6: 317
-    min 7: 363
-    min 8: 418
-    min 9: 487
-    min 10: 487
-    min 11: 300
-    min 12: 487
+    min 0: 500 (GFXCLK)
+    min 1: 480 (SOCCLK)
+    min 2: 97 (UCLK)
+    min 3: 550 (FCLK)
+    min 4: 317 (DCLK_0)
+    min 5: 363 (VCLK_0)
+    min 6: 317 (DCLK_1)
+    min 7: 363 (VCLK_1)
+    min 8: 418 (DCEFCLK)
+    min 9: 487 (DISPCLK)
+    min 10: 487 (PIXCLK)
+    min 11: 300 (PHYCLK)
+    min 12: 487 (DTBCLK)
     min 13: 0
     min 14: 0
     min 15: 0
 overdrive_table:
   revision: 129
   reserve:
     reserve 0: 0
     reserve 1: 0
     reserve 2: 0
   feature_count: 16
   setting_count: 30
   cap:
-    cap 0: 1
-    cap 1: 1
-    cap 2: 1
-    cap 3: 1
-    cap 4: 1
-    cap 5: 1
-    cap 6: 1
-    cap 7: 1
-    cap 8: 1
-    cap 9: 1
-    cap 10: 1
-    cap 11: 1
-    cap 12: 1
-    cap 13: 1
-    cap 14: 0
-    cap 15: 1
+    cap 0: 1 (GFXCLK_LIMITS)
+    cap 1: 1 (GFXCLK_CURVE)
+    cap 2: 1 (UCLK_LIMITS)
+    cap 3: 1 (POWER_LIMIT)
+    cap 4: 1 (FAN_ACOUSTIC_LIMIT)
+    cap 5: 1 (FAN_SPEED_MIN)
+    cap 6: 1 (TEMPERATURE_FAN)
+    cap 7: 1 (TEMPERATURE_SYSTEM)
+    cap 8: 1 (MEMORY_TIMING_TUNE)
+    cap 9: 1 (FAN_ZERO_RPM_CONTROL)
+    cap 10: 1 (AUTO_UV_ENGINE)
+    cap 11: 1 (AUTO_OC_ENGINE)
+    cap 12: 1 (AUTO_OC_MEMORY)
+    cap 13: 1 (FAN_CURVE)
+    cap 14: 0 (SMU_11_0_ODCAP_AUTO_FAN_ACOUSTIC_LIMIT)
+    cap 15: 1 (POWER_MODE)
     cap 16: 0
     cap 17: 0
     cap 18: 0
     cap 19: 0
     cap 20: 0
     cap 21: 0
     cap 22: 0
@@ -101,44 +101,44 @@
     cap 26: 0
     cap 27: 0
     cap 28: 0
     cap 29: 0
     cap 30: 0
     cap 31: 0
   max:
-    max 0: 3000
-    max 1: 3000
-    max 2: 0
-    max 3: 0
-    max 4: 0
-    max 5: 3000
-    max 6: 1075
-    max 7: 1075
-    max 8: 15
-    max 9: 3300
-    max 10: 3300
-    max 11: 100
-    max 12: 110
-    max 13: 1
-    max 14: 1
-    max 15: 1
-    max 16: 1
-    max 17: 1
-    max 18: 100
-    max 19: 100
-    max 20: 100
-    max 21: 100
-    max 22: 100
-    max 23: 100
-    max 24: 100
-    max 25: 100
-    max 26: 100
-    max 27: 100
-    max 28: 0
-    max 29: 1
+    max 0: 3000 (GFXCLKFMAX)
+    max 1: 3000 (GFXCLKFMIN)
+    max 2: 0 (CUSTOM_GFX_VF_CURVE_A)
+    max 3: 0 (CUSTOM_GFX_VF_CURVE_B)
+    max 4: 0 (CUSTOM_GFX_VF_CURVE_C)
+    max 5: 3000 (CUSTOM_CURVE_VFT_FMIN)
+    max 6: 1075 (UCLKFMIN)
+    max 7: 1075 (UCLKFMAX)
+    max 8: 15 (POWERPERCENTAGE)
+    max 9: 3300 (FANRPMMIN)
+    max 10: 3300 (FANRPMACOUSTICLIMIT)
+    max 11: 100 (FANTARGETTEMPERATURE)
+    max 12: 110 (OPERATINGTEMPMAX)
+    max 13: 1 (ACTIMING)
+    max 14: 1 (FAN_ZERO_RPM_CONTROL)
+    max 15: 1 (AUTOUVENGINE)
+    max 16: 1 (AUTOOCENGINE)
+    max 17: 1 (AUTOOCMEMORY)
+    max 18: 100 (FAN_CURVE_TEMPERATURE_1)
+    max 19: 100 (FAN_CURVE_SPEED_1)
+    max 20: 100 (FAN_CURVE_TEMPERATURE_2)
+    max 21: 100 (FAN_CURVE_SPEED_2)
+    max 22: 100 (FAN_CURVE_TEMPERATURE_3)
+    max 23: 100 (FAN_CURVE_SPEED_3)
+    max 24: 100 (FAN_CURVE_TEMPERATURE_4)
+    max 25: 100 (FAN_CURVE_SPEED_4)
+    max 26: 100 (FAN_CURVE_TEMPERATURE_5)
+    max 27: 100 (FAN_CURVE_SPEED_5)
+    max 28: 0 (AUTO_FAN_ACOUSTIC_LIMIT)
+    max 29: 1 (POWER_MODE)
     max 30: 0
     max 31: 0
     max 32: 0
     max 33: 0
     max 34: 0
     max 35: 0
     max 36: 0
@@ -166,44 +166,44 @@
     max 58: 0
     max 59: 0
     max 60: 0
     max 61: 0
     max 62: 0
     max 63: 0
   min:
-    min 0: 500
-    min 1: 500
-    min 2: 0
-    min 3: 0
-    min 4: 0
-    min 5: 500
-    min 6: 674
-    min 7: 674
-    min 8: 10
-    min 9: 250
-    min 10: 1000
-    min 11: 25
-    min 12: 50
-    min 13: 0
-    min 14: 0
-    min 15: 0
-    min 16: 0
-    min 17: 0
-    min 18: 25
-    min 19: 10
-    min 20: 25
-    min 21: 10
-    min 22: 25
-    min 23: 10
-    min 24: 25
-    min 25: 10
-    min 26: 25
-    min 27: 10
-    min 28: 0
-    min 29: 0
+    min 0: 500 (GFXCLKFMAX)
+    min 1: 500 (GFXCLKFMIN)
+    min 2: 0 (CUSTOM_GFX_VF_CURVE_A)
+    min 3: 0 (CUSTOM_GFX_VF_CURVE_B)
+    min 4: 0 (CUSTOM_GFX_VF_CURVE_C)
+    min 5: 500 (CUSTOM_CURVE_VFT_FMIN)
+    min 6: 674 (UCLKFMIN)
+    min 7: 674 (UCLKFMAX)
+    min 8: 10 (POWERPERCENTAGE)
+    min 9: 250 (FANRPMMIN)
+    min 10: 1000 (FANRPMACOUSTICLIMIT)
+    min 11: 25 (FANTARGETTEMPERATURE)
+    min 12: 50 (OPERATINGTEMPMAX)
+    min 13: 0 (ACTIMING)
+    min 14: 0 (FAN_ZERO_RPM_CONTROL)
+    min 15: 0 (AUTOUVENGINE)
+    min 16: 0 (AUTOOCENGINE)
+    min 17: 0 (AUTOOCMEMORY)
+    min 18: 25 (FAN_CURVE_TEMPERATURE_1)
+    min 19: 10 (FAN_CURVE_SPEED_1)
+    min 20: 25 (FAN_CURVE_TEMPERATURE_2)
+    min 21: 10 (FAN_CURVE_SPEED_2)
+    min 22: 25 (FAN_CURVE_TEMPERATURE_3)
+    min 23: 10 (FAN_CURVE_SPEED_3)
+    min 24: 25 (FAN_CURVE_TEMPERATURE_4)
+    min 25: 10 (FAN_CURVE_SPEED_4)
+    min 26: 25 (FAN_CURVE_TEMPERATURE_5)
+    min 27: 10 (FAN_CURVE_SPEED_5)
+    min 28: 0 (AUTO_FAN_ACOUSTIC_LIMIT)
+    min 29: 0 (POWER_MODE)
     min 30: 0
     min 31: 0
     min 32: 0
     min 33: 0
     min 34: 0
     min 35: 0
     min 36: 0
```

### Comparing `upp-0.2.0/test/AMD.RX6900.16384.201104.rom.rawdump` & `upp-0.2.1/test/AMD.RX6900.16384.201104.rom.rawdump`

 * *Files 17% similar despite different names*

```diff
@@ -1,1045 +1,1045 @@
 PowerPlay table rev 15.0 size 2470 bytes
- Offset (dec.) t Raw val. Variable name                   Decoded value
------------------------------------------------------------------------
- 0x0000 (0000) H     a609 structuresize                   : 2470
- 0x0002 (0002) B       0f format_revision                 : 15
- 0x0003 (0003) B       00 content_revision                : 0
- 0x0004 (0004) B       02 table_revision                  : 2
- 0x0005 (0005) H     2203 table_size                      : 802
- 0x0007 (0007) I af090000 golden_pp_id                    : 2479
- 0x000b (0011) I 77400000 golden_revision                 : 16503
- 0x000f (0015) H     8000 format_id                       : 128
- 0x0011 (0017) I 18000000 platform_caps                   : 24
- 0x0015 (0021) B       1c thermal_controller_type         : 28
- 0x0016 (0022) H     0000 small_power_limit1              : 0
- 0x0018 (0024) H     0000 small_power_limit2              : 0
- 0x001a (0026) H     0000 boost_power_limit               : 0
- 0x001c (0028) H     7600 software_shutdown_temp          : 118
- 0x001e (0030) H     0000 reserve                         : 0
- 0x0020 (0032) H     0000 reserve                         : 0
- 0x0022 (0034) H     0000 reserve                         : 0
- 0x0024 (0036) H     0000 reserve                         : 0
- 0x0026 (0038) H     0000 reserve                         : 0
- 0x0028 (0040) H     0000 reserve                         : 0
- 0x002a (0042) H     0100 reserve                         : 1
- 0x002c (0044) H     0000 reserve                         : 0
- 0x002e (0046) B       01 revision                        : 1
- 0x002f (0047) B       00 reserve                         : 0
- 0x0030 (0048) B       00 reserve                         : 0
- 0x0031 (0049) B       00 reserve                         : 0
- 0x0032 (0050) I 0d000000 count                           : 13
- 0x0036 (0054) I 640a0000 max                             : 2660
- 0x003a (0058) I b0040000 max                             : 1200
- 0x003e (0062) I e8030000 max                             : 1000
- 0x0042 (0066) I 94070000 max                             : 1940
- 0x0046 (0070) I f2040000 max                             : 1266
- 0x004a (0074) I c5050000 max                             : 1477
- 0x004e (0078) I f2040000 max                             : 1266
- 0x0052 (0082) I c5050000 max                             : 1477
- 0x0056 (0086) I b0040000 max                             : 1200
- 0x005a (0090) I c1040000 max                             : 1217
- 0x005e (0094) I c1040000 max                             : 1217
- 0x0062 (0098) I 2a030000 max                             : 810
- 0x0066 (0102) I c1040000 max                             : 1217
- 0x006a (0106) I 00000000 max                             : 0
- 0x006e (0110) I 00000000 max                             : 0
- 0x0072 (0114) I 00000000 max                             : 0
- 0x0076 (0118) I f4010000 min                             : 500
- 0x007a (0122) I e0010000 min                             : 480
- 0x007e (0126) I 61000000 min                             : 97
- 0x0082 (0130) I 26020000 min                             : 550
- 0x0086 (0134) I 3d010000 min                             : 317
- 0x008a (0138) I 6b010000 min                             : 363
- 0x008e (0142) I 3d010000 min                             : 317
- 0x0092 (0146) I 6b010000 min                             : 363
- 0x0096 (0150) I a2010000 min                             : 418
- 0x009a (0154) I e7010000 min                             : 487
- 0x009e (0158) I e7010000 min                             : 487
- 0x00a2 (0162) I 2c010000 min                             : 300
- 0x00a6 (0166) I e7010000 min                             : 487
- 0x00aa (0170) I 00000000 min                             : 0
- 0x00ae (0174) I 00000000 min                             : 0
- 0x00b2 (0178) I 00000000 min                             : 0
- 0x00b6 (0182) B       81 revision                        : 129
- 0x00b7 (0183) B       00 reserve                         : 0
- 0x00b8 (0184) B       00 reserve                         : 0
- 0x00b9 (0185) B       00 reserve                         : 0
- 0x00ba (0186) I 10000000 feature_count                   : 16
- 0x00be (0190) I 1e000000 setting_count                   : 30
- 0x00c2 (0194) B       01 cap                             : 1
- 0x00c3 (0195) B       01 cap                             : 1
- 0x00c4 (0196) B       01 cap                             : 1
- 0x00c5 (0197) B       01 cap                             : 1
- 0x00c6 (0198) B       01 cap                             : 1
- 0x00c7 (0199) B       01 cap                             : 1
- 0x00c8 (0200) B       01 cap                             : 1
- 0x00c9 (0201) B       01 cap                             : 1
- 0x00ca (0202) B       01 cap                             : 1
- 0x00cb (0203) B       01 cap                             : 1
- 0x00cc (0204) B       01 cap                             : 1
- 0x00cd (0205) B       01 cap                             : 1
- 0x00ce (0206) B       01 cap                             : 1
- 0x00cf (0207) B       01 cap                             : 1
- 0x00d0 (0208) B       00 cap                             : 0
- 0x00d1 (0209) B       01 cap                             : 1
- 0x00d2 (0210) B       00 cap                             : 0
- 0x00d3 (0211) B       00 cap                             : 0
- 0x00d4 (0212) B       00 cap                             : 0
- 0x00d5 (0213) B       00 cap                             : 0
- 0x00d6 (0214) B       00 cap                             : 0
- 0x00d7 (0215) B       00 cap                             : 0
- 0x00d8 (0216) B       00 cap                             : 0
- 0x00d9 (0217) B       00 cap                             : 0
- 0x00da (0218) B       00 cap                             : 0
- 0x00db (0219) B       00 cap                             : 0
- 0x00dc (0220) B       00 cap                             : 0
- 0x00dd (0221) B       00 cap                             : 0
- 0x00de (0222) B       00 cap                             : 0
- 0x00df (0223) B       00 cap                             : 0
- 0x00e0 (0224) B       00 cap                             : 0
- 0x00e1 (0225) B       00 cap                             : 0
- 0x00e2 (0226) I b80b0000 max                             : 3000
- 0x00e6 (0230) I b80b0000 max                             : 3000
- 0x00ea (0234) I 00000000 max                             : 0
- 0x00ee (0238) I 00000000 max                             : 0
- 0x00f2 (0242) I 00000000 max                             : 0
- 0x00f6 (0246) I b80b0000 max                             : 3000
- 0x00fa (0250) I 33040000 max                             : 1075
- 0x00fe (0254) I 33040000 max                             : 1075
- 0x0102 (0258) I 0f000000 max                             : 15
- 0x0106 (0262) I e40c0000 max                             : 3300
- 0x010a (0266) I e40c0000 max                             : 3300
- 0x010e (0270) I 64000000 max                             : 100
- 0x0112 (0274) I 6e000000 max                             : 110
- 0x0116 (0278) I 01000000 max                             : 1
- 0x011a (0282) I 01000000 max                             : 1
- 0x011e (0286) I 01000000 max                             : 1
- 0x0122 (0290) I 01000000 max                             : 1
- 0x0126 (0294) I 01000000 max                             : 1
- 0x012a (0298) I 64000000 max                             : 100
- 0x012e (0302) I 64000000 max                             : 100
- 0x0132 (0306) I 64000000 max                             : 100
- 0x0136 (0310) I 64000000 max                             : 100
- 0x013a (0314) I 64000000 max                             : 100
- 0x013e (0318) I 64000000 max                             : 100
- 0x0142 (0322) I 64000000 max                             : 100
- 0x0146 (0326) I 64000000 max                             : 100
- 0x014a (0330) I 64000000 max                             : 100
- 0x014e (0334) I 64000000 max                             : 100
- 0x0152 (0338) I 00000000 max                             : 0
- 0x0156 (0342) I 01000000 max                             : 1
- 0x015a (0346) I 00000000 max                             : 0
- 0x015e (0350) I 00000000 max                             : 0
- 0x0162 (0354) I 00000000 max                             : 0
- 0x0166 (0358) I 00000000 max                             : 0
- 0x016a (0362) I 00000000 max                             : 0
- 0x016e (0366) I 00000000 max                             : 0
- 0x0172 (0370) I 00000000 max                             : 0
- 0x0176 (0374) I 00000000 max                             : 0
- 0x017a (0378) I 00000000 max                             : 0
- 0x017e (0382) I 00000000 max                             : 0
- 0x0182 (0386) I 00000000 max                             : 0
- 0x0186 (0390) I 00000000 max                             : 0
- 0x018a (0394) I 00000000 max                             : 0
- 0x018e (0398) I 00000000 max                             : 0
- 0x0192 (0402) I 00000000 max                             : 0
- 0x0196 (0406) I 00000000 max                             : 0
- 0x019a (0410) I 00000000 max                             : 0
- 0x019e (0414) I 00000000 max                             : 0
- 0x01a2 (0418) I 00000000 max                             : 0
- 0x01a6 (0422) I 00000000 max                             : 0
- 0x01aa (0426) I 00000000 max                             : 0
- 0x01ae (0430) I 00000000 max                             : 0
- 0x01b2 (0434) I 00000000 max                             : 0
- 0x01b6 (0438) I 00000000 max                             : 0
- 0x01ba (0442) I 00000000 max                             : 0
- 0x01be (0446) I 00000000 max                             : 0
- 0x01c2 (0450) I 00000000 max                             : 0
- 0x01c6 (0454) I 00000000 max                             : 0
- 0x01ca (0458) I 00000000 max                             : 0
- 0x01ce (0462) I 00000000 max                             : 0
- 0x01d2 (0466) I 00000000 max                             : 0
- 0x01d6 (0470) I 00000000 max                             : 0
- 0x01da (0474) I 00000000 max                             : 0
- 0x01de (0478) I 00000000 max                             : 0
- 0x01e2 (0482) I f4010000 min                             : 500
- 0x01e6 (0486) I f4010000 min                             : 500
- 0x01ea (0490) I 00000000 min                             : 0
- 0x01ee (0494) I 00000000 min                             : 0
- 0x01f2 (0498) I 00000000 min                             : 0
- 0x01f6 (0502) I f4010000 min                             : 500
- 0x01fa (0506) I a2020000 min                             : 674
- 0x01fe (0510) I a2020000 min                             : 674
- 0x0202 (0514) I 0a000000 min                             : 10
- 0x0206 (0518) I fa000000 min                             : 250
- 0x020a (0522) I e8030000 min                             : 1000
- 0x020e (0526) I 19000000 min                             : 25
- 0x0212 (0530) I 32000000 min                             : 50
- 0x0216 (0534) I 00000000 min                             : 0
- 0x021a (0538) I 00000000 min                             : 0
- 0x021e (0542) I 00000000 min                             : 0
- 0x0222 (0546) I 00000000 min                             : 0
- 0x0226 (0550) I 00000000 min                             : 0
- 0x022a (0554) I 19000000 min                             : 25
- 0x022e (0558) I 0a000000 min                             : 10
- 0x0232 (0562) I 19000000 min                             : 25
- 0x0236 (0566) I 0a000000 min                             : 10
- 0x023a (0570) I 19000000 min                             : 25
- 0x023e (0574) I 0a000000 min                             : 10
- 0x0242 (0578) I 19000000 min                             : 25
- 0x0246 (0582) I 0a000000 min                             : 10
- 0x024a (0586) I 19000000 min                             : 25
- 0x024e (0590) I 0a000000 min                             : 10
- 0x0252 (0594) I 00000000 min                             : 0
- 0x0256 (0598) I 00000000 min                             : 0
- 0x025a (0602) I 00000000 min                             : 0
- 0x025e (0606) I 00000000 min                             : 0
- 0x0262 (0610) I 00000000 min                             : 0
- 0x0266 (0614) I 00000000 min                             : 0
- 0x026a (0618) I 00000000 min                             : 0
- 0x026e (0622) I 00000000 min                             : 0
- 0x0272 (0626) I 00000000 min                             : 0
- 0x0276 (0630) I 00000000 min                             : 0
- 0x027a (0634) I 00000000 min                             : 0
- 0x027e (0638) I 00000000 min                             : 0
- 0x0282 (0642) I 00000000 min                             : 0
- 0x0286 (0646) I 00000000 min                             : 0
- 0x028a (0650) I 00000000 min                             : 0
- 0x028e (0654) I 00000000 min                             : 0
- 0x0292 (0658) I 00000000 min                             : 0
- 0x0296 (0662) I 00000000 min                             : 0
- 0x029a (0666) I 00000000 min                             : 0
- 0x029e (0670) I 00000000 min                             : 0
- 0x02a2 (0674) I 00000000 min                             : 0
- 0x02a6 (0678) I 00000000 min                             : 0
- 0x02aa (0682) I 00000000 min                             : 0
- 0x02ae (0686) I 00000000 min                             : 0
- 0x02b2 (0690) I 00000000 min                             : 0
- 0x02b6 (0694) I 00000000 min                             : 0
- 0x02ba (0698) I 00000000 min                             : 0
- 0x02be (0702) I 00000000 min                             : 0
- 0x02c2 (0706) I 00000000 min                             : 0
- 0x02c6 (0710) I 00000000 min                             : 0
- 0x02ca (0714) I 00000000 min                             : 0
- 0x02ce (0718) I 00000000 min                             : 0
- 0x02d2 (0722) I 00000000 min                             : 0
- 0x02d6 (0726) I 00000000 min                             : 0
- 0x02da (0730) I 00000000 min                             : 0
- 0x02de (0734) I 00000000 min                             : 0
- 0x02e2 (0738) h     0600 pm_setting                      : 6
- 0x02e4 (0740) h     0000 pm_setting                      : 0
- 0x02e6 (0742) h     0600 pm_setting                      : 6
- 0x02e8 (0744) h     0600 pm_setting                      : 6
- 0x02ea (0746) h     5f00 pm_setting                      : 95
- 0x02ec (0748) h     5f00 pm_setting                      : 95
- 0x02ee (0750) h     5f00 pm_setting                      : 95
- 0x02f0 (0752) h     5f00 pm_setting                      : 95
- 0x02f2 (0754) h     7206 pm_setting                      : 1650
- 0x02f4 (0756) h     7206 pm_setting                      : 1650
- 0x02f6 (0758) h     d606 pm_setting                      : 1750
- 0x02f8 (0760) h     d606 pm_setting                      : 1750
- 0x02fa (0762) h     d007 pm_setting                      : 2000
- 0x02fc (0764) h     d007 pm_setting                      : 2000
- 0x02fe (0766) h     ca08 pm_setting                      : 2250
- 0x0300 (0768) h     ca08 pm_setting                      : 2250
- 0x0302 (0770) h     0000 pm_setting                      : 0
- 0x0304 (0772) h     0000 pm_setting                      : 0
- 0x0306 (0774) h     0000 pm_setting                      : 0
- 0x0308 (0776) h     0000 pm_setting                      : 0
- 0x030a (0778) h     0000 pm_setting                      : 0
- 0x030c (0780) h     0000 pm_setting                      : 0
- 0x030e (0782) h     0000 pm_setting                      : 0
- 0x0310 (0784) h     0000 pm_setting                      : 0
- 0x0312 (0786) h     0000 pm_setting                      : 0
- 0x0314 (0788) h     0000 pm_setting                      : 0
- 0x0316 (0790) h     0000 pm_setting                      : 0
- 0x0318 (0792) h     0000 pm_setting                      : 0
- 0x031a (0794) h     0000 pm_setting                      : 0
- 0x031c (0796) h     0000 pm_setting                      : 0
- 0x031e (0798) h     0000 pm_setting                      : 0
- 0x0320 (0800) h     0000 pm_setting                      : 0
- 0x0322 (0802) I 06000000 Version                         : 6
- 0x0326 (0806) I fffd7fa3 FeaturesToRun                   : 2743074303
- 0x032a (0810) I 63370000 FeaturesToRun                   : 14179
- 0x032e (0814) H     ff00 SocketPowerLimitAc              : 255
- 0x0330 (0816) H     0000 SocketPowerLimitAc              : 0
- 0x0332 (0818) H     0000 SocketPowerLimitAc              : 0
- 0x0334 (0820) H     0000 SocketPowerLimitAc              : 0
- 0x0336 (0822) H     0000 SocketPowerLimitAcTau           : 0
- 0x0338 (0824) H     0000 SocketPowerLimitAcTau           : 0
- 0x033a (0826) H     0000 SocketPowerLimitAcTau           : 0
- 0x033c (0828) H     0000 SocketPowerLimitAcTau           : 0
- 0x033e (0830) H     ff00 SocketPowerLimitDc              : 255
- 0x0340 (0832) H     0000 SocketPowerLimitDc              : 0
- 0x0342 (0834) H     0000 SocketPowerLimitDc              : 0
- 0x0344 (0836) H     0000 SocketPowerLimitDc              : 0
- 0x0346 (0838) H     0000 SocketPowerLimitDcTau           : 0
- 0x0348 (0840) H     0000 SocketPowerLimitDcTau           : 0
- 0x034a (0842) H     0000 SocketPowerLimitDcTau           : 0
- 0x034c (0844) H     0000 SocketPowerLimitDcTau           : 0
- 0x034e (0846) H     4001 TdcLimit                        : 320
- 0x0350 (0848) H     3700 TdcLimit                        : 55
- 0x0352 (0850) H     0000 TdcLimitTau                     : 0
- 0x0354 (0852) H     0000 TdcLimitTau                     : 0
- 0x0356 (0854) H     6400 TemperatureLimit                : 100
- 0x0358 (0856) H     6e00 TemperatureLimit                : 110
- 0x035a (0858) H     6400 TemperatureLimit                : 100
- 0x035c (0860) H     7300 TemperatureLimit                : 115
- 0x035e (0862) H     7300 TemperatureLimit                : 115
- 0x0360 (0864) H     7300 TemperatureLimit                : 115
- 0x0362 (0866) H     7300 TemperatureLimit                : 115
- 0x0364 (0868) H     0000 TemperatureLimit                : 0
- 0x0366 (0870) H     0000 TemperatureLimit                : 0
- 0x0368 (0872) H     0000 TemperatureLimit                : 0
- 0x036a (0874) I 00000000 FitLimit                        : 0
- 0x036e (0878) B       01 TotalPowerConfig                : 1
- 0x036f (0879) B       00 TotalPowerPadding               : 0
- 0x0370 (0880) B       00 TotalPowerPadding               : 0
- 0x0371 (0881) B       00 TotalPowerPadding               : 0
- 0x0372 (0882) I 0a000000 ApccPlusResidencyLimit          : 10
- 0x0376 (0886) H     0000 SmnclkDpmFreq                   : 0
- 0x0378 (0888) H     0000 SmnclkDpmFreq                   : 0
- 0x037a (0890) H     0000 SmnclkDpmVoltage                : 0
- 0x037c (0892) H     0000 SmnclkDpmVoltage                : 0
- 0x037e (0894) I 00000000 PaddingAPCC                     : 0
- 0x0382 (0898) H     0000 PerPartDroopVsetGfxDfll         : 0
- 0x0384 (0900) H     0000 PerPartDroopVsetGfxDfll         : 0
- 0x0386 (0902) H     0000 PerPartDroopVsetGfxDfll         : 0
- 0x0388 (0904) H     0000 PerPartDroopVsetGfxDfll         : 0
- 0x038a (0906) H     0000 PerPartDroopVsetGfxDfll         : 0
- 0x038c (0908) H     0000 PaddingPerPartDroop             : 0
- 0x038e (0910) I fe380000 ThrottlerControlMask            : 14590
- 0x0392 (0914) I 730f0000 FwDStateMask                    : 3955
- 0x0396 (0918) H     6400 UlvVoltageOffsetSoc             : 100
- 0x0398 (0920) H     6400 UlvVoltageOffsetGfx             : 100
- 0x039a (0922) H     1c0c MinVoltageUlvGfx                : 3100
- 0x039c (0924) H     800c MinVoltageUlvSoc                : 3200
- 0x039e (0926) H     0000 SocLIVmin                       : 0
- 0x03a0 (0928) H     0000 PaddingLIVmin                   : 0
- 0x03a2 (0930) B       00 GceaLinkMgrIdleThreshold        : 0
- 0x03a3 (0931) B       00 RlcUlvParams                    : 0
- 0x03a4 (0932) B       00 RlcUlvParams                    : 0
- 0x03a5 (0933) B       00 RlcUlvParams                    : 0
- 0x03a6 (0934) H     e40c MinVoltageGfx                   : 3300
- 0x03a8 (0936) H     e40c MinVoltageSoc                   : 3300
- 0x03aa (0938) H     5c12 MaxVoltageGfx                   : 4700
- 0x03ac (0940) H     f811 MaxVoltageSoc                   : 4600
- 0x03ae (0942) H     4000 LoadLineResistanceGfx           : 64
- 0x03b0 (0944) H     0001 LoadLineResistanceSoc           : 256
- 0x03b2 (0946) H     3200 VDDGFX_TVmin                    : 50
- 0x03b4 (0948) H     3c00 VDDSOC_TVmin                    : 60
- 0x03b6 (0950) H     800c VDDGFX_Vmin_HiTemp              : 3200
- 0x03b8 (0952) H     800c VDDGFX_Vmin_LoTemp              : 3200
- 0x03ba (0954) H     800c VDDSOC_Vmin_HiTemp              : 3200
- 0x03bc (0956) H     800c VDDSOC_Vmin_LoTemp              : 3200
- 0x03be (0958) H     1400 VDDGFX_TVminHystersis           : 20
- 0x03c0 (0960) H     1400 VDDSOC_TVminHystersis           : 20
- 0x03c2 (0962) B       00 VoltageMode                     : 0
- 0x03c3 (0963) B       00 SnapToDiscrete                  : 0
- 0x03c4 (0964) B       02 NumDiscreteLevels               : 2
- 0x03c5 (0965) B       00 Padding                         : 0
- 0x03c6 (0966) f 0000803f m                               : 1
- 0x03ca (0970) f 00000000 b                               : 0
- 0x03ce (0974) f b537b83e a                               : 0.3598
- 0x03d2 (0978) f ef1b67bf b                               :-0.90277
- 0x03d6 (0982) f 4f40a73f c                               : 1.30665
- 0x03da (0986) H     8b04 SsFmin                          : 1163
- 0x03dc (0988) H     0000 Padding16                       : 0
- 0x03de (0990) B       00 VoltageMode                     : 0
- 0x03df (0991) B       00 SnapToDiscrete                  : 0
- 0x03e0 (0992) B       02 NumDiscreteLevels               : 2
- 0x03e1 (0993) B       00 Padding                         : 0
- 0x03e2 (0994) f ee7c8f3f m                               : 1.121
- 0x03e6 (0998) f a69b843e b                               : 0.259
- 0x03ea (1002) f 44349a3e a                               : 0.30118
- 0x03ee (1006) f 43ad09be b                               :-0.13445
- 0x03f2 (1010) f 3d0f363f c                               : 0.71117
- 0x03f6 (1014) H     f100 SsFmin                          : 241
- 0x03f8 (1016) H     0000 Padding16                       : 0
- 0x03fa (1018) B       00 VoltageMode                     : 0
- 0x03fb (1019) B       01 SnapToDiscrete                  : 1
- 0x03fc (1020) B       04 NumDiscreteLevels               : 4
- 0x03fd (1021) B       00 Padding                         : 0
- 0x03fe (1022) f cdccac3f m                               : 1.35
- 0x0402 (1026) f e3a59bbd b                               :-0.076
- 0x0406 (1030) f 6f81e43e a                               : 0.4463
- 0x040a (1034) f caa6ccbe b                               :-0.39971
- 0x040e (1038) f 0421493f c                               : 0.78566
- 0x0412 (1042) H     c001 SsFmin                          : 448
- 0x0414 (1044) H     0000 Padding16                       : 0
- 0x0416 (1046) B       00 VoltageMode                     : 0
- 0x0417 (1047) B       00 SnapToDiscrete                  : 0
- 0x0418 (1048) B       02 NumDiscreteLevels               : 2
- 0x0419 (1049) B       00 Padding                         : 0
- 0x041a (1050) f 0000803f m                               : 1
- 0x041e (1054) f 00000000 b                               : 0
- 0x0422 (1058) f 72c47a3e a                               : 0.24489
- 0x0426 (1062) f 4c8984be b                               :-0.25886
- 0x042a (1066) f dcba433f c                               : 0.76457
- 0x042e (1070) H     1102 SsFmin                          : 529
- 0x0430 (1072) H     0000 Padding16                       : 0
- 0x0432 (1074) B       00 VoltageMode                     : 0
- 0x0433 (1075) B       00 SnapToDiscrete                  : 0
- 0x0434 (1076) B       02 NumDiscreteLevels               : 2
- 0x0435 (1077) B       00 Padding                         : 0
- 0x0436 (1078) f 098aaf3f m                               : 1.3714
- 0x043a (1082) f 295c0fbd b                               :-0.035
- 0x043e (1086) f 85ceeb3e a                               : 0.46056
- 0x0442 (1090) f 10ccc1be b                               :-0.37851
- 0x0446 (1094) f 4720463f c                               : 0.77393
- 0x044a (1098) H     9b01 SsFmin                          : 411
- 0x044c (1100) H     0000 Padding16                       : 0
- 0x044e (1102) B       00 VoltageMode                     : 0
- 0x044f (1103) B       00 SnapToDiscrete                  : 0
- 0x0450 (1104) B       02 NumDiscreteLevels               : 2
- 0x0451 (1105) B       00 Padding                         : 0
- 0x0452 (1106) f 6ade893f m                               : 1.0771
- 0x0456 (1110) f b81e053e b                               : 0.13
- 0x045a (1114) f 8e75913e a                               : 0.2841
- 0x045e (1118) f 284957be b                               :-0.21024
- 0x0462 (1122) f e42c3c3f c                               : 0.73506
- 0x0466 (1126) H     7301 SsFmin                          : 371
- 0x0468 (1128) H     0000 Padding16                       : 0
- 0x046a (1130) B       00 VoltageMode                     : 0
- 0x046b (1131) B       00 SnapToDiscrete                  : 0
- 0x046c (1132) B       02 NumDiscreteLevels               : 2
- 0x046d (1133) B       00 Padding                         : 0
- 0x046e (1134) f 098aaf3f m                               : 1.3714
- 0x0472 (1138) f 295c0fbd b                               :-0.035
- 0x0476 (1142) f 85ceeb3e a                               : 0.46056
- 0x047a (1146) f 10ccc1be b                               :-0.37851
- 0x047e (1150) f 4720463f c                               : 0.77393
- 0x0482 (1154) H     9b01 SsFmin                          : 411
- 0x0484 (1156) H     0000 Padding16                       : 0
- 0x0486 (1158) B       00 VoltageMode                     : 0
- 0x0487 (1159) B       00 SnapToDiscrete                  : 0
- 0x0488 (1160) B       02 NumDiscreteLevels               : 2
- 0x0489 (1161) B       00 Padding                         : 0
- 0x048a (1162) f 6ade893f m                               : 1.0771
- 0x048e (1166) f b81e053e b                               : 0.13
- 0x0492 (1170) f 8e75913e a                               : 0.2841
- 0x0496 (1174) f 284957be b                               :-0.21024
- 0x049a (1178) f e42c3c3f c                               : 0.73506
- 0x049e (1182) H     7301 SsFmin                          : 371
- 0x04a0 (1184) H     0000 Padding16                       : 0
- 0x04a2 (1186) B       00 VoltageMode                     : 0
- 0x04a3 (1187) B       00 SnapToDiscrete                  : 0
- 0x04a4 (1188) B       02 NumDiscreteLevels               : 2
- 0x04a5 (1189) B       00 Padding                         : 0
- 0x04a6 (1190) f 7d3f953f m                               : 1.166
- 0x04aa (1194) f dd24063e b                               : 0.131
- 0x04ae (1198) f 1d77aa3e a                               : 0.33294
- 0x04b2 (1202) f ee7768be b                               :-0.22702
- 0x04b6 (1206) f c91f3c3f c                               : 0.73486
- 0x04ba (1210) H     5501 SsFmin                          : 341
- 0x04bc (1212) H     0000 Padding16                       : 0
- 0x04be (1214) B       00 VoltageMode                     : 0
- 0x04bf (1215) B       00 SnapToDiscrete                  : 0
- 0x04c0 (1216) B       02 NumDiscreteLevels               : 2
- 0x04c1 (1217) B       00 Padding                         : 0
- 0x04c2 (1218) f 6abc743f m                               : 0.956
- 0x04c6 (1222) f ae47613e b                               : 0.22
- 0x04ca (1226) f 732e653e a                               : 0.22381
- 0x04ce (1230) f 52ed13be b                               :-0.14446
- 0x04d2 (1234) f d72f383f c                               : 0.71948
- 0x04d6 (1238) H     4301 SsFmin                          : 323
- 0x04d8 (1240) H     0000 Padding16                       : 0
- 0x04da (1242) B       00 VoltageMode                     : 0
- 0x04db (1243) B       00 SnapToDiscrete                  : 0
- 0x04dc (1244) B       02 NumDiscreteLevels               : 2
- 0x04dd (1245) B       00 Padding                         : 0
- 0x04de (1246) f 6abc743f m                               : 0.956
- 0x04e2 (1250) f ae47613e b                               : 0.22
- 0x04e6 (1254) f 732e653e a                               : 0.22381
- 0x04ea (1258) f 52ed13be b                               :-0.14446
- 0x04ee (1262) f d72f383f c                               : 0.71948
- 0x04f2 (1266) H     4301 SsFmin                          : 323
- 0x04f4 (1268) H     0000 Padding16                       : 0
- 0x04f6 (1270) B       00 VoltageMode                     : 0
- 0x04f7 (1271) B       00 SnapToDiscrete                  : 0
- 0x04f8 (1272) B       02 NumDiscreteLevels               : 2
- 0x04f9 (1273) B       00 Padding                         : 0
- 0x04fa (1274) f 0e2d123f m                               : 0.571
- 0x04fe (1278) f 9a99d93e b                               : 0.425
- 0x0502 (1282) f 2783a33d a                               : 0.07984
- 0x0506 (1286) f 8d28edbc b                               :-0.02895
- 0x050a (1290) f e7e3323f c                               : 0.69879
- 0x050e (1294) H     b600 SsFmin                          : 182
- 0x0510 (1296) H     0000 Padding16                       : 0
- 0x0512 (1298) B       00 VoltageMode                     : 0
- 0x0513 (1299) B       00 SnapToDiscrete                  : 0
- 0x0514 (1300) B       02 NumDiscreteLevels               : 2
- 0x0515 (1301) B       00 Padding                         : 0
- 0x0516 (1302) f 6abc743f m                               : 0.956
- 0x051a (1306) f ae47613e b                               : 0.22
- 0x051e (1310) f 732e653e a                               : 0.22381
- 0x0522 (1314) f 52ed13be b                               :-0.14446
- 0x0526 (1318) f d72f383f c                               : 0.71948
- 0x052a (1322) H     4301 SsFmin                          : 323
- 0x052c (1324) H     0000 Padding16                       : 0
- 0x052e (1326) H     f401 FreqTableGfx                    : 500
- 0x0530 (1328) H     640a FreqTableGfx                    : 2660
- 0x0532 (1330) H     0000 FreqTableGfx                    : 0
- 0x0534 (1332) H     0000 FreqTableGfx                    : 0
- 0x0536 (1334) H     0000 FreqTableGfx                    : 0
- 0x0538 (1336) H     0000 FreqTableGfx                    : 0
- 0x053a (1338) H     0000 FreqTableGfx                    : 0
- 0x053c (1340) H     0000 FreqTableGfx                    : 0
- 0x053e (1342) H     0000 FreqTableGfx                    : 0
- 0x0540 (1344) H     0000 FreqTableGfx                    : 0
- 0x0542 (1346) H     0000 FreqTableGfx                    : 0
- 0x0544 (1348) H     0000 FreqTableGfx                    : 0
- 0x0546 (1350) H     0000 FreqTableGfx                    : 0
- 0x0548 (1352) H     0000 FreqTableGfx                    : 0
- 0x054a (1354) H     0000 FreqTableGfx                    : 0
- 0x054c (1356) H     0000 FreqTableGfx                    : 0
- 0x054e (1358) H     6b01 FreqTableVclk                   : 363
- 0x0550 (1360) H     c505 FreqTableVclk                   : 1477
- 0x0552 (1362) H     0000 FreqTableVclk                   : 0
- 0x0554 (1364) H     0000 FreqTableVclk                   : 0
- 0x0556 (1366) H     0000 FreqTableVclk                   : 0
- 0x0558 (1368) H     0000 FreqTableVclk                   : 0
- 0x055a (1370) H     0000 FreqTableVclk                   : 0
- 0x055c (1372) H     0000 FreqTableVclk                   : 0
- 0x055e (1374) H     3d01 FreqTableDclk                   : 317
- 0x0560 (1376) H     f204 FreqTableDclk                   : 1266
- 0x0562 (1378) H     0000 FreqTableDclk                   : 0
- 0x0564 (1380) H     0000 FreqTableDclk                   : 0
- 0x0566 (1382) H     0000 FreqTableDclk                   : 0
- 0x0568 (1384) H     0000 FreqTableDclk                   : 0
- 0x056a (1386) H     0000 FreqTableDclk                   : 0
- 0x056c (1388) H     0000 FreqTableDclk                   : 0
- 0x056e (1390) H     e001 FreqTableSocclk                 : 480
- 0x0570 (1392) H     b004 FreqTableSocclk                 : 1200
- 0x0572 (1394) H     0000 FreqTableSocclk                 : 0
- 0x0574 (1396) H     0000 FreqTableSocclk                 : 0
- 0x0576 (1398) H     0000 FreqTableSocclk                 : 0
- 0x0578 (1400) H     0000 FreqTableSocclk                 : 0
- 0x057a (1402) H     0000 FreqTableSocclk                 : 0
- 0x057c (1404) H     0000 FreqTableSocclk                 : 0
- 0x057e (1406) H     6100 FreqTableUclk                   : 97
- 0x0580 (1408) H     c901 FreqTableUclk                   : 457
- 0x0582 (1410) H     a202 FreqTableUclk                   : 674
- 0x0584 (1412) H     e803 FreqTableUclk                   : 1000
- 0x0586 (1414) H     a201 FreqTableDcefclk                : 418
- 0x0588 (1416) H     b004 FreqTableDcefclk                : 1200
- 0x058a (1418) H     0000 FreqTableDcefclk                : 0
- 0x058c (1420) H     0000 FreqTableDcefclk                : 0
- 0x058e (1422) H     0000 FreqTableDcefclk                : 0
- 0x0590 (1424) H     0000 FreqTableDcefclk                : 0
- 0x0592 (1426) H     0000 FreqTableDcefclk                : 0
- 0x0594 (1428) H     0000 FreqTableDcefclk                : 0
- 0x0596 (1430) H     e701 FreqTableDispclk                : 487
- 0x0598 (1432) H     c104 FreqTableDispclk                : 1217
- 0x059a (1434) H     0000 FreqTableDispclk                : 0
- 0x059c (1436) H     0000 FreqTableDispclk                : 0
- 0x059e (1438) H     0000 FreqTableDispclk                : 0
- 0x05a0 (1440) H     0000 FreqTableDispclk                : 0
- 0x05a2 (1442) H     0000 FreqTableDispclk                : 0
- 0x05a4 (1444) H     0000 FreqTableDispclk                : 0
- 0x05a6 (1446) H     e701 FreqTablePixclk                 : 487
- 0x05a8 (1448) H     c104 FreqTablePixclk                 : 1217
- 0x05aa (1450) H     0000 FreqTablePixclk                 : 0
- 0x05ac (1452) H     0000 FreqTablePixclk                 : 0
- 0x05ae (1454) H     0000 FreqTablePixclk                 : 0
- 0x05b0 (1456) H     0000 FreqTablePixclk                 : 0
- 0x05b2 (1458) H     0000 FreqTablePixclk                 : 0
- 0x05b4 (1460) H     0000 FreqTablePixclk                 : 0
- 0x05b6 (1462) H     2c01 FreqTablePhyclk                 : 300
- 0x05b8 (1464) H     2a03 FreqTablePhyclk                 : 810
- 0x05ba (1466) H     0000 FreqTablePhyclk                 : 0
- 0x05bc (1468) H     0000 FreqTablePhyclk                 : 0
- 0x05be (1470) H     0000 FreqTablePhyclk                 : 0
- 0x05c0 (1472) H     0000 FreqTablePhyclk                 : 0
- 0x05c2 (1474) H     0000 FreqTablePhyclk                 : 0
- 0x05c4 (1476) H     0000 FreqTablePhyclk                 : 0
- 0x05c6 (1478) H     e701 FreqTableDtbclk                 : 487
- 0x05c8 (1480) H     c104 FreqTableDtbclk                 : 1217
- 0x05ca (1482) H     0000 FreqTableDtbclk                 : 0
- 0x05cc (1484) H     0000 FreqTableDtbclk                 : 0
- 0x05ce (1486) H     0000 FreqTableDtbclk                 : 0
- 0x05d0 (1488) H     0000 FreqTableDtbclk                 : 0
- 0x05d2 (1490) H     0000 FreqTableDtbclk                 : 0
- 0x05d4 (1492) H     0000 FreqTableDtbclk                 : 0
- 0x05d6 (1494) H     2602 FreqTableFclk                   : 550
- 0x05d8 (1496) H     9407 FreqTableFclk                   : 1940
- 0x05da (1498) H     0000 FreqTableFclk                   : 0
- 0x05dc (1500) H     0000 FreqTableFclk                   : 0
- 0x05de (1502) H     0000 FreqTableFclk                   : 0
- 0x05e0 (1504) H     0000 FreqTableFclk                   : 0
- 0x05e2 (1506) H     0000 FreqTableFclk                   : 0
- 0x05e4 (1508) H     0000 FreqTableFclk                   : 0
- 0x05e6 (1510) I 00000000 Paddingclks                     : 0
- 0x05ea (1514) f 00000000 a                               : 0
- 0x05ee (1518) f 00000000 b                               : 0
- 0x05f2 (1522) f 00000000 c                               : 0
- 0x05f6 (1526) f 00000000 a                               : 0
- 0x05fa (1530) f 00000000 b                               : 0
- 0x05fe (1534) f 00000000 c                               : 0
- 0x0602 (1538) f 00000000 a                               : 0
- 0x0606 (1542) f 00000000 b                               : 0
- 0x060a (1546) f 00000000 c                               : 0
- 0x060e (1550) f 00000000 a                               : 0
- 0x0612 (1554) f 00000000 b                               : 0
- 0x0616 (1558) f 00000000 c                               : 0
- 0x061a (1562) f 00000000 a                               : 0
- 0x061e (1566) f 00000000 b                               : 0
- 0x0622 (1570) f 00000000 c                               : 0
- 0x0626 (1574) I 640a0000 DcModeMaxFreq                   : 2660
- 0x062a (1578) I b0040000 DcModeMaxFreq                   : 1200
- 0x062e (1582) I e8030000 DcModeMaxFreq                   : 1000
- 0x0632 (1586) I 94070000 DcModeMaxFreq                   : 1940
- 0x0636 (1590) I f2040000 DcModeMaxFreq                   : 1266
- 0x063a (1594) I c5050000 DcModeMaxFreq                   : 1477
- 0x063e (1598) I f2040000 DcModeMaxFreq                   : 1266
- 0x0642 (1602) I c5050000 DcModeMaxFreq                   : 1477
- 0x0646 (1606) I b0040000 DcModeMaxFreq                   : 1200
- 0x064a (1610) I c1040000 DcModeMaxFreq                   : 1217
- 0x064e (1614) I c1040000 DcModeMaxFreq                   : 1217
- 0x0652 (1618) I 2a030000 DcModeMaxFreq                   : 810
- 0x0656 (1622) I c1040000 DcModeMaxFreq                   : 1217
- 0x065a (1626) B       00 FreqTableUclkDiv                : 0
- 0x065b (1627) B       02 FreqTableUclkDiv                : 2
- 0x065c (1628) B       03 FreqTableUclkDiv                : 3
- 0x065d (1629) B       03 FreqTableUclkDiv                : 3
- 0x065e (1630) H     7805 FclkBoostFreq                   : 1400
- 0x0660 (1632) H     0000 FclkParamPadding                : 0
- 0x0662 (1634) H     4c01 Mp0clkFreq                      : 332
- 0x0664 (1636) H     fa01 Mp0clkFreq                      : 506
- 0x0666 (1638) H     f00a Mp0DpmVoltage                   : 2800
- 0x0668 (1640) H     800c Mp0DpmVoltage                   : 3200
- 0x066a (1642) H     8c0a MemVddciVoltage                 : 2700
- 0x066c (1644) H     800c MemVddciVoltage                 : 3200
- 0x066e (1646) H     480d MemVddciVoltage                 : 3400
- 0x0670 (1648) H     480d MemVddciVoltage                 : 3400
- 0x0672 (1650) H     8813 MemMvddVoltage                  : 5000
- 0x0674 (1652) H     1815 MemMvddVoltage                  : 5400
- 0x0676 (1654) H     1815 MemMvddVoltage                  : 5400
- 0x0678 (1656) H     1815 MemMvddVoltage                  : 5400
- 0x067a (1658) H     f401 GfxclkFgfxoffEntry              : 500
- 0x067c (1660) H     2003 GfxclkFinit                     : 800
- 0x067e (1662) H     f401 GfxclkFidle                     : 500
- 0x0680 (1664) B       01 GfxclkSource                    : 1
- 0x0681 (1665) B       00 GfxclkPadding                   : 0
- 0x0682 (1666) B       01 GfxGpoSubFeatureMask            : 1
- 0x0683 (1667) B       02 GfxGpoEnabledWorkPolicyMask     : 2
- 0x0684 (1668) B       5d GfxGpoDisabledWorkPolicyMask    : 93
- 0x0685 (1669) B       00 GfxGpoPadding                   : 0
- 0x0686 (1670) I 01000000 GfxGpoVotingAllow               : 1
- 0x068a (1674) I 00000000 GfxGpoPadding32                 : 0
- 0x068e (1678) I 00000000 GfxGpoPadding32                 : 0
- 0x0692 (1682) I 00000000 GfxGpoPadding32                 : 0
- 0x0696 (1686) I 00000000 GfxGpoPadding32                 : 0
- 0x069a (1690) H     0000 GfxDcsFopt                      : 0
- 0x069c (1692) H     0000 GfxDcsFclkFopt                  : 0
- 0x069e (1694) H     0000 GfxDcsUclkFopt                  : 0
- 0x06a0 (1696) H     0000 DcsGfxOffVoltage                : 0
- 0x06a2 (1698) H     0000 DcsMinGfxOffTime                : 0
- 0x06a4 (1700) H     0000 DcsMaxGfxOffTime                : 0
- 0x06a6 (1702) I 00000000 DcsMinCreditAccum               : 0
- 0x06aa (1706) H     0000 DcsExitHysteresis               : 0
- 0x06ac (1708) H     0000 DcsTimeout                      : 0
- 0x06ae (1710) I 00000000 DcsParamPadding                 : 0
- 0x06b2 (1714) I 00000000 DcsParamPadding                 : 0
- 0x06b6 (1718) I 00000000 DcsParamPadding                 : 0
- 0x06ba (1722) I 00000000 DcsParamPadding                 : 0
- 0x06be (1726) I 00000000 DcsParamPadding                 : 0
- 0x06c2 (1730) H     2a16 FlopsPerByteTable               : 5674
- 0x06c4 (1732) H     d715 FlopsPerByteTable               : 5591
- 0x06c6 (1734) H     8415 FlopsPerByteTable               : 5508
- 0x06c8 (1736) H     3015 FlopsPerByteTable               : 5424
- 0x06ca (1738) H     dd14 FlopsPerByteTable               : 5341
- 0x06cc (1740) H     8a14 FlopsPerByteTable               : 5258
- 0x06ce (1742) H     3614 FlopsPerByteTable               : 5174
- 0x06d0 (1744) H     e313 FlopsPerByteTable               : 5091
- 0x06d2 (1746) H     9013 FlopsPerByteTable               : 5008
- 0x06d4 (1748) H     3d13 FlopsPerByteTable               : 4925
- 0x06d6 (1750) H     e912 FlopsPerByteTable               : 4841
- 0x06d8 (1752) H     9612 FlopsPerByteTable               : 4758
- 0x06da (1754) H     b111 FlopsPerByteTable               : 4529
- 0x06dc (1756) H     cc10 FlopsPerByteTable               : 4300
- 0x06de (1758) H     e70f FlopsPerByteTable               : 4071
- 0x06e0 (1760) H     020f FlopsPerByteTable               : 3842
- 0x06e2 (1762) B       00 LowestUclkReservedForUlv        : 0
- 0x06e3 (1763) B       00 PaddingMem                      : 0
- 0x06e4 (1764) B       00 PaddingMem                      : 0
- 0x06e5 (1765) B       00 PaddingMem                      : 0
- 0x06e6 (1766) B       03 UclkDpmPstates                  : 3
- 0x06e7 (1767) B       02 UclkDpmPstates                  : 2
- 0x06e8 (1768) B       01 UclkDpmPstates                  : 1
- 0x06e9 (1769) B       00 UclkDpmPstates                  : 0
- 0x06ea (1770) H     0000 Fmin                            : 0
- 0x06ec (1772) H     0000 Fmax                            : 0
- 0x06ee (1774) H     0000 Fmin                            : 0
- 0x06f0 (1776) H     0000 Fmax                            : 0
- 0x06f2 (1778) H     0000 UclkDpmMidstepFreq              : 0
- 0x06f4 (1780) H     0000 UclkMidstepPadding              : 0
- 0x06f6 (1782) B       00 PcieGenSpeed                    : 0
- 0x06f7 (1783) B       03 PcieGenSpeed                    : 3
- 0x06f8 (1784) B       01 PcieLaneCount                   : 1
- 0x06f9 (1785) B       06 PcieLaneCount                   : 6
- 0x06fa (1786) H     3601 LclkFreq                        : 310
- 0x06fc (1788) H     6b02 LclkFreq                        : 619
- 0x06fe (1790) H     3700 FanStopTemp                     : 55
- 0x0700 (1792) H     4600 FanStartTemp                    : 70
- 0x0702 (1794) H     9001 FanGain                         : 400
- 0x0704 (1796) H     9001 FanGain                         : 400
- 0x0706 (1798) H     9001 FanGain                         : 400
- 0x0708 (1800) H     9001 FanGain                         : 400
- 0x070a (1802) H     9001 FanGain                         : 400
- 0x070c (1804) H     9001 FanGain                         : 400
- 0x070e (1806) H     9001 FanGain                         : 400
- 0x0710 (1808) H     9001 FanGain                         : 400
- 0x0712 (1810) H     9001 FanGain                         : 400
- 0x0714 (1812) H     9001 FanGain                         : 400
- 0x0716 (1814) H     1900 FanPwmMin                       : 25
- 0x0718 (1816) H     7206 FanAcousticLimitRpm             : 1650
- 0x071a (1818) H     d007 FanThrottlingRpm                : 2000
- 0x071c (1820) H     e40c FanMaximumRpm                   : 3300
- 0x071e (1822) H     0000 MGpuFanBoostLimitRpm            : 0
- 0x0720 (1824) H     5f00 FanTargetTemperature            : 95
- 0x0722 (1826) H     f401 FanTargetGfxclk                 : 500
- 0x0724 (1828) H     0000 FanPadding16                    : 0
- 0x0726 (1830) B       01 FanTempInputSelect              : 1
- 0x0727 (1831) B       00 FanPadding                      : 0
- 0x0728 (1832) B       01 FanZeroRpmEnable                : 1
- 0x0729 (1833) B       02 FanTachEdgePerRev               : 2
- 0x072a (1834) h     0000 FuzzyFan_ErrorSetDelta          : 0
- 0x072c (1836) h     0000 FuzzyFan_ErrorRateSetDelta      : 0
- 0x072e (1838) h     0000 FuzzyFan_PwmSetDelta            : 0
- 0x0730 (1840) H     0000 FuzzyFan_Reserved               : 0
- 0x0732 (1842) B       00 OverrideAvfsGb                  : 0
- 0x0733 (1843) B       00 OverrideAvfsGb                  : 0
- 0x0734 (1844) B       01 BtcGbGfxDfllModelSelect         : 1
- 0x0735 (1845) B       00 Padding8_Avfs                   : 0
- 0x0736 (1846) f 00000000 a                               : 0
- 0x073a (1850) f 00000000 b                               : 0
- 0x073e (1854) f 00000000 c                               : 0
- 0x0742 (1858) f 00000000 a                               : 0
- 0x0746 (1862) f 00000000 b                               : 0
- 0x074a (1866) f 00000000 c                               : 0
- 0x074e (1870) f 0d54863d a                               : 0.06559
- 0x0752 (1874) f bc05d2bd b                               :-0.10255
- 0x0756 (1878) f 1f80143e c                               : 0.14502
- 0x075a (1882) f 00000000 a                               : 0
- 0x075e (1886) f 00000000 b                               : 0
- 0x0762 (1890) f 00000000 c                               : 0
- 0x0766 (1894) f 00000000 a                               : 0
- 0x076a (1898) f 00000000 b                               : 0
- 0x076e (1902) f 00000000 c                               : 0
- 0x0772 (1906) f 00000000 m                               : 0
- 0x0776 (1910) f 00000000 b                               : 0
- 0x077a (1914) f 00000000 m                               : 0
- 0x077e (1918) f 00000000 b                               : 0
- 0x0782 (1922) f 9a99993e Fset                            : 0.3
- 0x0786 (1926) f 0000c03f Fset                            : 1.5
- 0x078a (1930) f 33331340 Fset                            : 2.3
- 0x078e (1934) f 00002040 Fset                            : 2.5
- 0x0792 (1938) f 66664640 Fset                            : 3.1
- 0x0796 (1942) f 0ad7233d Vdroop                          : 0.04
- 0x079a (1946) f dd24863d Vdroop                          : 0.0655
- 0x079e (1950) f a245b63d Vdroop                          : 0.089
- 0x07a2 (1954) f 39b4c83d Vdroop                          : 0.098
- 0x07a6 (1958) f c74bb73e Vdroop                          : 0.358
- 0x07aa (1962) f 7593983d a                               : 0.0745
- 0x07ae (1966) f 2fdd84be b                               :-0.2595
- 0x07b2 (1970) f a3927a3e c                               : 0.2447
- 0x07b6 (1974) f e56121bd a                               :-0.0394
- 0x07ba (1978) f 04568e3e b                               : 0.278
- 0x07be (1982) f c5722bbe c                               :-0.16743
- 0x07c2 (1986) H     c000 DcTol                           : 192
- 0x07c4 (1988) H     c000 DcTol                           : 192
- 0x07c6 (1990) B       01 DcBtcEnabled                    : 1
- 0x07c7 (1991) B       01 DcBtcEnabled                    : 1
- 0x07c8 (1992) B       00 Padding8_GfxBtc                 : 0
- 0x07c9 (1993) B       00 Padding8_GfxBtc                 : 0
- 0x07ca (1994) H     0000 DcBtcMin                        : 0
- 0x07cc (1996) H     0000 DcBtcMin                        : 0
- 0x07ce (1998) H     c000 DcBtcMax                        : 192
- 0x07d0 (2000) H     c000 DcBtcMax                        : 192
- 0x07d2 (2002) H     1900 DcBtcGb                         : 25
- 0x07d4 (2004) H     1900 DcBtcGb                         : 25
- 0x07d6 (2006) B       00 XgmiDpmPstates                  : 0
- 0x07d7 (2007) B       00 XgmiDpmPstates                  : 0
- 0x07d8 (2008) B       00 XgmiDpmSpare                    : 0
- 0x07d9 (2009) B       00 XgmiDpmSpare                    : 0
- 0x07da (2010) I 00000000 DebugOverrides                  : 0
- 0x07de (2014) f 00000000 a                               : 0
- 0x07e2 (2018) f 00000000 b                               : 0
- 0x07e6 (2022) f 00000000 c                               : 0
- 0x07ea (2026) f 00000000 a                               : 0
- 0x07ee (2030) f 00000000 b                               : 0
- 0x07f2 (2034) f 00000000 c                               : 0
- 0x07f6 (2038) f 00000000 a                               : 0
- 0x07fa (2042) f 00000000 b                               : 0
- 0x07fe (2046) f 00000000 c                               : 0
- 0x0802 (2050) f 00000000 a                               : 0
- 0x0806 (2054) f 00000000 b                               : 0
- 0x080a (2058) f 00000000 c                               : 0
- 0x080e (2062) B       00 CustomerVariant                 : 0
- 0x080f (2063) B       01 VcBtcEnabled                    : 1
- 0x0810 (2064) H     3b0b VcBtcVminT0                     : 2875
- 0x0812 (2066) H     4501 VcBtcFixedVminAgingOffset       : 325
- 0x0814 (2068) H     0000 VcBtcVmin2PsmDegrationGb        : 0
- 0x0816 (2070) f 3480373b VcBtcPsmA                       : 0.0028
- 0x081a (2074) f 9fabcd3e VcBtcPsmB                       : 0.4017
- 0x081e (2078) f ed0d3e3c VcBtcVminA                      : 0.0116
- 0x0822 (2082) f 7593f83e VcBtcVminB                      : 0.4855
- 0x0826 (2086) H     0000 LedGpio                         : 0
- 0x0828 (2088) H     0100 GfxPowerStagesGpio              : 1
- 0x082a (2090) I 00000000 SkuReserved                     : 0
- 0x082e (2094) I 00000000 SkuReserved                     : 0
- 0x0832 (2098) I 00000000 SkuReserved                     : 0
- 0x0836 (2102) I 00000000 SkuReserved                     : 0
- 0x083a (2106) I 00000000 SkuReserved                     : 0
- 0x083e (2110) I 00000000 SkuReserved                     : 0
- 0x0842 (2114) I 00000000 SkuReserved                     : 0
- 0x0846 (2118) I 00000000 SkuReserved                     : 0
- 0x084a (2122) I 00000000 GamingClk                       : 0
- 0x084e (2126) I 00000000 GamingClk                       : 0
- 0x0852 (2130) I 00000000 GamingClk                       : 0
- 0x0856 (2134) I 00000000 GamingClk                       : 0
- 0x085a (2138) I 00000000 GamingClk                       : 0
- 0x085e (2142) I 00000000 GamingClk                       : 0
- 0x0862 (2146) B       00 Enabled                         : 0
- 0x0863 (2147) B       00 Speed                           : 0
- 0x0864 (2148) B       00 SlaveAddress                    : 0
- 0x0865 (2149) B       00 ControllerPort                  : 0
- 0x0866 (2150) B       00 ControllerName                  : 0
- 0x0867 (2151) B       00 ThermalThrotter                 : 0
- 0x0868 (2152) B       00 I2cProtocol                     : 0
- 0x0869 (2153) B       00 PaddingConfig                   : 0
- 0x086a (2154) B       00 Enabled                         : 0
- 0x086b (2155) B       00 Speed                           : 0
- 0x086c (2156) B       00 SlaveAddress                    : 0
- 0x086d (2157) B       00 ControllerPort                  : 0
- 0x086e (2158) B       00 ControllerName                  : 0
- 0x086f (2159) B       00 ThermalThrotter                 : 0
- 0x0870 (2160) B       00 I2cProtocol                     : 0
- 0x0871 (2161) B       00 PaddingConfig                   : 0
- 0x0872 (2162) B       00 Enabled                         : 0
- 0x0873 (2163) B       00 Speed                           : 0
- 0x0874 (2164) B       00 SlaveAddress                    : 0
- 0x0875 (2165) B       00 ControllerPort                  : 0
- 0x0876 (2166) B       00 ControllerName                  : 0
- 0x0877 (2167) B       00 ThermalThrotter                 : 0
- 0x0878 (2168) B       00 I2cProtocol                     : 0
- 0x0879 (2169) B       00 PaddingConfig                   : 0
- 0x087a (2170) B       00 Enabled                         : 0
- 0x087b (2171) B       00 Speed                           : 0
- 0x087c (2172) B       00 SlaveAddress                    : 0
- 0x087d (2173) B       00 ControllerPort                  : 0
- 0x087e (2174) B       00 ControllerName                  : 0
- 0x087f (2175) B       00 ThermalThrotter                 : 0
- 0x0880 (2176) B       00 I2cProtocol                     : 0
- 0x0881 (2177) B       00 PaddingConfig                   : 0
- 0x0882 (2178) B       00 Enabled                         : 0
- 0x0883 (2179) B       00 Speed                           : 0
- 0x0884 (2180) B       00 SlaveAddress                    : 0
- 0x0885 (2181) B       00 ControllerPort                  : 0
- 0x0886 (2182) B       00 ControllerName                  : 0
- 0x0887 (2183) B       00 ThermalThrotter                 : 0
- 0x0888 (2184) B       00 I2cProtocol                     : 0
- 0x0889 (2185) B       00 PaddingConfig                   : 0
- 0x088a (2186) B       00 Enabled                         : 0
- 0x088b (2187) B       00 Speed                           : 0
- 0x088c (2188) B       00 SlaveAddress                    : 0
- 0x088d (2189) B       00 ControllerPort                  : 0
- 0x088e (2190) B       00 ControllerName                  : 0
- 0x088f (2191) B       00 ThermalThrotter                 : 0
- 0x0890 (2192) B       00 I2cProtocol                     : 0
- 0x0891 (2193) B       00 PaddingConfig                   : 0
- 0x0892 (2194) B       00 Enabled                         : 0
- 0x0893 (2195) B       00 Speed                           : 0
- 0x0894 (2196) B       00 SlaveAddress                    : 0
- 0x0895 (2197) B       00 ControllerPort                  : 0
- 0x0896 (2198) B       00 ControllerName                  : 0
- 0x0897 (2199) B       00 ThermalThrotter                 : 0
- 0x0898 (2200) B       00 I2cProtocol                     : 0
- 0x0899 (2201) B       00 PaddingConfig                   : 0
- 0x089a (2202) B       00 Enabled                         : 0
- 0x089b (2203) B       00 Speed                           : 0
- 0x089c (2204) B       00 SlaveAddress                    : 0
- 0x089d (2205) B       00 ControllerPort                  : 0
- 0x089e (2206) B       00 ControllerName                  : 0
- 0x089f (2207) B       00 ThermalThrotter                 : 0
- 0x08a0 (2208) B       00 I2cProtocol                     : 0
- 0x08a1 (2209) B       00 PaddingConfig                   : 0
- 0x08a2 (2210) B       00 Enabled                         : 0
- 0x08a3 (2211) B       00 Speed                           : 0
- 0x08a4 (2212) B       00 SlaveAddress                    : 0
- 0x08a5 (2213) B       00 ControllerPort                  : 0
- 0x08a6 (2214) B       00 ControllerName                  : 0
- 0x08a7 (2215) B       00 ThermalThrotter                 : 0
- 0x08a8 (2216) B       00 I2cProtocol                     : 0
- 0x08a9 (2217) B       00 PaddingConfig                   : 0
- 0x08aa (2218) B       00 Enabled                         : 0
- 0x08ab (2219) B       00 Speed                           : 0
- 0x08ac (2220) B       00 SlaveAddress                    : 0
- 0x08ad (2221) B       00 ControllerPort                  : 0
- 0x08ae (2222) B       00 ControllerName                  : 0
- 0x08af (2223) B       00 ThermalThrotter                 : 0
- 0x08b0 (2224) B       00 I2cProtocol                     : 0
- 0x08b1 (2225) B       00 PaddingConfig                   : 0
- 0x08b2 (2226) B       00 Enabled                         : 0
- 0x08b3 (2227) B       00 Speed                           : 0
- 0x08b4 (2228) B       00 SlaveAddress                    : 0
- 0x08b5 (2229) B       00 ControllerPort                  : 0
- 0x08b6 (2230) B       00 ControllerName                  : 0
- 0x08b7 (2231) B       00 ThermalThrotter                 : 0
- 0x08b8 (2232) B       00 I2cProtocol                     : 0
- 0x08b9 (2233) B       00 PaddingConfig                   : 0
- 0x08ba (2234) B       00 Enabled                         : 0
- 0x08bb (2235) B       00 Speed                           : 0
- 0x08bc (2236) B       00 SlaveAddress                    : 0
- 0x08bd (2237) B       00 ControllerPort                  : 0
- 0x08be (2238) B       00 ControllerName                  : 0
- 0x08bf (2239) B       00 ThermalThrotter                 : 0
- 0x08c0 (2240) B       00 I2cProtocol                     : 0
- 0x08c1 (2241) B       00 PaddingConfig                   : 0
- 0x08c2 (2242) B       00 Enabled                         : 0
- 0x08c3 (2243) B       00 Speed                           : 0
- 0x08c4 (2244) B       00 SlaveAddress                    : 0
- 0x08c5 (2245) B       00 ControllerPort                  : 0
- 0x08c6 (2246) B       00 ControllerName                  : 0
- 0x08c7 (2247) B       00 ThermalThrotter                 : 0
- 0x08c8 (2248) B       00 I2cProtocol                     : 0
- 0x08c9 (2249) B       00 PaddingConfig                   : 0
- 0x08ca (2250) B       00 Enabled                         : 0
- 0x08cb (2251) B       00 Speed                           : 0
- 0x08cc (2252) B       00 SlaveAddress                    : 0
- 0x08cd (2253) B       00 ControllerPort                  : 0
- 0x08ce (2254) B       00 ControllerName                  : 0
- 0x08cf (2255) B       00 ThermalThrotter                 : 0
- 0x08d0 (2256) B       00 I2cProtocol                     : 0
- 0x08d1 (2257) B       00 PaddingConfig                   : 0
- 0x08d2 (2258) B       00 Enabled                         : 0
- 0x08d3 (2259) B       00 Speed                           : 0
- 0x08d4 (2260) B       00 SlaveAddress                    : 0
- 0x08d5 (2261) B       00 ControllerPort                  : 0
- 0x08d6 (2262) B       00 ControllerName                  : 0
- 0x08d7 (2263) B       00 ThermalThrotter                 : 0
- 0x08d8 (2264) B       00 I2cProtocol                     : 0
- 0x08d9 (2265) B       00 PaddingConfig                   : 0
- 0x08da (2266) B       00 Enabled                         : 0
- 0x08db (2267) B       00 Speed                           : 0
- 0x08dc (2268) B       00 SlaveAddress                    : 0
- 0x08dd (2269) B       00 ControllerPort                  : 0
- 0x08de (2270) B       00 ControllerName                  : 0
- 0x08df (2271) B       00 ThermalThrotter                 : 0
- 0x08e0 (2272) B       00 I2cProtocol                     : 0
- 0x08e1 (2273) B       00 PaddingConfig                   : 0
- 0x08e2 (2274) B       00 GpioScl                         : 0
- 0x08e3 (2275) B       00 GpioSda                         : 0
- 0x08e4 (2276) B       00 FchUsbPdSlaveAddr               : 0
- 0x08e5 (2277) B       00 I2cSpare                        : 0
- 0x08e6 (2278) B       00 VddGfxVrMapping                 : 0
- 0x08e7 (2279) B       00 VddSocVrMapping                 : 0
- 0x08e8 (2280) B       00 VddMem0VrMapping                : 0
- 0x08e9 (2281) B       00 VddMem1VrMapping                : 0
- 0x08ea (2282) B       00 GfxUlvPhaseSheddingMask         : 0
- 0x08eb (2283) B       00 SocUlvPhaseSheddingMask         : 0
- 0x08ec (2284) B       00 VddciUlvPhaseSheddingMask       : 0
- 0x08ed (2285) B       00 MvddUlvPhaseSheddingMask        : 0
- 0x08ee (2286) H     0000 GfxMaxCurrent                   : 0
- 0x08f0 (2288) b       00 GfxOffset                       : 0
- 0x08f1 (2289) B       00 Padding_TelemetryGfx            : 0
- 0x08f2 (2290) H     0000 SocMaxCurrent                   : 0
- 0x08f4 (2292) b       00 SocOffset                       : 0
- 0x08f5 (2293) B       00 Padding_TelemetrySoc            : 0
- 0x08f6 (2294) H     0000 Mem0MaxCurrent                  : 0
- 0x08f8 (2296) b       00 Mem0Offset                      : 0
- 0x08f9 (2297) B       00 Padding_TelemetryMem0           : 0
- 0x08fa (2298) H     0000 Mem1MaxCurrent                  : 0
- 0x08fc (2300) b       00 Mem1Offset                      : 0
- 0x08fd (2301) B       00 Padding_TelemetryMem1           : 0
- 0x08fe (2302) I 00000000 MvddRatio                       : 0
- 0x0902 (2306) B       00 AcDcGpio                        : 0
- 0x0903 (2307) B       00 AcDcPolarity                    : 0
- 0x0904 (2308) B       00 VR0HotGpio                      : 0
- 0x0905 (2309) B       00 VR0HotPolarity                  : 0
- 0x0906 (2310) B       00 VR1HotGpio                      : 0
- 0x0907 (2311) B       00 VR1HotPolarity                  : 0
- 0x0908 (2312) B       00 GthrGpio                        : 0
- 0x0909 (2313) B       00 GthrPolarity                    : 0
- 0x090a (2314) B       00 LedPin0                         : 0
- 0x090b (2315) B       00 LedPin1                         : 0
- 0x090c (2316) B       00 LedPin2                         : 0
- 0x090d (2317) B       00 LedEnableMask                   : 0
- 0x090e (2318) B       00 LedPcie                         : 0
- 0x090f (2319) B       00 LedError                        : 0
- 0x0910 (2320) B       00 LedSpare1                       : 0
- 0x0911 (2321) B       01 LedSpare1                       : 1
- 0x0912 (2322) B       00 PllGfxclkSpreadEnabled          : 0
- 0x0913 (2323) B       00 PllGfxclkSpreadPercent          : 0
- 0x0914 (2324) H     0000 PllGfxclkSpreadFreq             : 0
- 0x0916 (2326) B       00 DfllGfxclkSpreadEnabled         : 0
- 0x0917 (2327) B       00 DfllGfxclkSpreadPercent         : 0
- 0x0918 (2328) H     0000 DfllGfxclkSpreadFreq            : 0
- 0x091a (2330) H     0000 UclkSpreadPadding               : 0
- 0x091c (2332) H     0000 UclkSpreadFreq                  : 0
- 0x091e (2334) B       00 FclkSpreadEnabled               : 0
- 0x091f (2335) B       00 FclkSpreadPercent               : 0
- 0x0920 (2336) H     0000 FclkSpreadFreq                  : 0
- 0x0922 (2338) I 00000000 MemoryChannelEnabled            : 0
- 0x0926 (2342) B       00 DramBitWidth                    : 0
- 0x0927 (2343) B       00 PaddingMem1                     : 0
- 0x0928 (2344) B       00 PaddingMem1                     : 0
- 0x0929 (2345) B       00 PaddingMem1                     : 0
- 0x092a (2346) H     0000 TotalBoardPower                 : 0
- 0x092c (2348) H     0000 BoardPowerPadding               : 0
- 0x092e (2350) B       00 XgmiLinkSpeed                   : 0
- 0x092f (2351) B       00 XgmiLinkSpeed                   : 0
- 0x0930 (2352) B       00 XgmiLinkSpeed                   : 0
- 0x0931 (2353) B       00 XgmiLinkSpeed                   : 0
- 0x0932 (2354) B       00 XgmiLinkWidth                   : 0
- 0x0933 (2355) B       00 XgmiLinkWidth                   : 0
- 0x0934 (2356) B       00 XgmiLinkWidth                   : 0
- 0x0935 (2357) B       00 XgmiLinkWidth                   : 0
- 0x0936 (2358) H     0000 XgmiFclkFreq                    : 0
- 0x0938 (2360) H     0000 XgmiFclkFreq                    : 0
- 0x093a (2362) H     0000 XgmiFclkFreq                    : 0
- 0x093c (2364) H     0000 XgmiFclkFreq                    : 0
- 0x093e (2366) H     0000 XgmiSocVoltage                  : 0
- 0x0940 (2368) H     0000 XgmiSocVoltage                  : 0
- 0x0942 (2370) H     0000 XgmiSocVoltage                  : 0
- 0x0944 (2372) H     0000 XgmiSocVoltage                  : 0
- 0x0946 (2374) B       00 HsrEnabled                      : 0
- 0x0947 (2375) B       00 VddqOffEnabled                  : 0
- 0x0948 (2376) B       00 PaddingUmcFlags                 : 0
- 0x0949 (2377) B       00 PaddingUmcFlags                 : 0
- 0x094a (2378) B       00 UclkSpreadPercent               : 0
- 0x094b (2379) B       00 UclkSpreadPercent               : 0
- 0x094c (2380) B       00 UclkSpreadPercent               : 0
- 0x094d (2381) B       00 UclkSpreadPercent               : 0
- 0x094e (2382) B       00 UclkSpreadPercent               : 0
- 0x094f (2383) B       00 UclkSpreadPercent               : 0
- 0x0950 (2384) B       00 UclkSpreadPercent               : 0
- 0x0951 (2385) B       00 UclkSpreadPercent               : 0
- 0x0952 (2386) B       00 UclkSpreadPercent               : 0
- 0x0953 (2387) B       00 UclkSpreadPercent               : 0
- 0x0954 (2388) B       00 UclkSpreadPercent               : 0
- 0x0955 (2389) B       00 UclkSpreadPercent               : 0
- 0x0956 (2390) B       00 UclkSpreadPercent               : 0
- 0x0957 (2391) B       00 UclkSpreadPercent               : 0
- 0x0958 (2392) B       00 UclkSpreadPercent               : 0
- 0x0959 (2393) B       00 UclkSpreadPercent               : 0
- 0x095a (2394) I 00000000 BoardReserved                   : 0
- 0x095e (2398) I 00000000 BoardReserved                   : 0
- 0x0962 (2402) I 00000000 BoardReserved                   : 0
- 0x0966 (2406) I 00000000 BoardReserved                   : 0
- 0x096a (2410) I 00000000 BoardReserved                   : 0
- 0x096e (2414) I 00000000 BoardReserved                   : 0
- 0x0972 (2418) I 00000000 BoardReserved                   : 0
- 0x0976 (2422) I 00000000 BoardReserved                   : 0
- 0x097a (2426) I 00000000 BoardReserved                   : 0
- 0x097e (2430) I 00000000 BoardReserved                   : 0
- 0x0982 (2434) I 00000000 BoardReserved                   : 0
- 0x0986 (2438) I 00000000 MmHubPadding                    : 0
- 0x098a (2442) I 00000000 MmHubPadding                    : 0
- 0x098e (2446) I 00000000 MmHubPadding                    : 0
- 0x0992 (2450) I 00000000 MmHubPadding                    : 0
- 0x0996 (2454) I 00000000 MmHubPadding                    : 0
- 0x099a (2458) I 00000000 MmHubPadding                    : 0
- 0x099e (2462) I 00000000 MmHubPadding                    : 0
- 0x09a2 (2466) I 00001e06 MmHubPadding                    : 102629376
+ Offset (dec.) t Raw val. Variable name                         Decoded value
+------------------------------------------------------------------------------
+ 0x0000 (0000) H     a609 structuresize                             : 2470
+ 0x0002 (0002) B       0f format_revision                           : 15
+ 0x0003 (0003) B       00 content_revision                          : 0
+ 0x0004 (0004) B       02 table_revision                            : 2
+ 0x0005 (0005) H     2203 table_size                                : 802
+ 0x0007 (0007) I af090000 golden_pp_id                              : 2479
+ 0x000b (0011) I 77400000 golden_revision                           : 16503
+ 0x000f (0015) H     8000 format_id                                 : 128
+ 0x0011 (0017) I 18000000 platform_caps                             : 24
+ 0x0015 (0021) B       1c thermal_controller_type                   : 28
+ 0x0016 (0022) H     0000 small_power_limit1                        : 0
+ 0x0018 (0024) H     0000 small_power_limit2                        : 0
+ 0x001a (0026) H     0000 boost_power_limit                         : 0
+ 0x001c (0028) H     7600 software_shutdown_temp                    : 118
+ 0x001e (0030) H     0000 reserve                                   : 0
+ 0x0020 (0032) H     0000 reserve                                   : 0
+ 0x0022 (0034) H     0000 reserve                                   : 0
+ 0x0024 (0036) H     0000 reserve                                   : 0
+ 0x0026 (0038) H     0000 reserve                                   : 0
+ 0x0028 (0040) H     0000 reserve                                   : 0
+ 0x002a (0042) H     0100 reserve                                   : 1
+ 0x002c (0044) H     0000 reserve                                   : 0
+ 0x002e (0046) B       01 revision                                  : 1
+ 0x002f (0047) B       00 reserve                                   : 0
+ 0x0030 (0048) B       00 reserve                                   : 0
+ 0x0031 (0049) B       00 reserve                                   : 0
+ 0x0032 (0050) I 0d000000 count                                     : 13
+ 0x0036 (0054) I 640a0000 max GFXCLK                                : 2660
+ 0x003a (0058) I b0040000 max SOCCLK                                : 1200
+ 0x003e (0062) I e8030000 max UCLK                                  : 1000
+ 0x0042 (0066) I 94070000 max FCLK                                  : 1940
+ 0x0046 (0070) I f2040000 max DCLK_0                                : 1266
+ 0x004a (0074) I c5050000 max VCLK_0                                : 1477
+ 0x004e (0078) I f2040000 max DCLK_1                                : 1266
+ 0x0052 (0082) I c5050000 max VCLK_1                                : 1477
+ 0x0056 (0086) I b0040000 max DCEFCLK                               : 1200
+ 0x005a (0090) I c1040000 max DISPCLK                               : 1217
+ 0x005e (0094) I c1040000 max PIXCLK                                : 1217
+ 0x0062 (0098) I 2a030000 max PHYCLK                                : 810
+ 0x0066 (0102) I c1040000 max DTBCLK                                : 1217
+ 0x006a (0106) I 00000000 max                                       : 0
+ 0x006e (0110) I 00000000 max                                       : 0
+ 0x0072 (0114) I 00000000 max                                       : 0
+ 0x0076 (0118) I f4010000 min GFXCLK                                : 500
+ 0x007a (0122) I e0010000 min SOCCLK                                : 480
+ 0x007e (0126) I 61000000 min UCLK                                  : 97
+ 0x0082 (0130) I 26020000 min FCLK                                  : 550
+ 0x0086 (0134) I 3d010000 min DCLK_0                                : 317
+ 0x008a (0138) I 6b010000 min VCLK_0                                : 363
+ 0x008e (0142) I 3d010000 min DCLK_1                                : 317
+ 0x0092 (0146) I 6b010000 min VCLK_1                                : 363
+ 0x0096 (0150) I a2010000 min DCEFCLK                               : 418
+ 0x009a (0154) I e7010000 min DISPCLK                               : 487
+ 0x009e (0158) I e7010000 min PIXCLK                                : 487
+ 0x00a2 (0162) I 2c010000 min PHYCLK                                : 300
+ 0x00a6 (0166) I e7010000 min DTBCLK                                : 487
+ 0x00aa (0170) I 00000000 min                                       : 0
+ 0x00ae (0174) I 00000000 min                                       : 0
+ 0x00b2 (0178) I 00000000 min                                       : 0
+ 0x00b6 (0182) B       81 revision                                  : 129
+ 0x00b7 (0183) B       00 reserve                                   : 0
+ 0x00b8 (0184) B       00 reserve                                   : 0
+ 0x00b9 (0185) B       00 reserve                                   : 0
+ 0x00ba (0186) I 10000000 feature_count                             : 16
+ 0x00be (0190) I 1e000000 setting_count                             : 30
+ 0x00c2 (0194) B       01 cap GFXCLK_LIMITS                         : 1
+ 0x00c3 (0195) B       01 cap GFXCLK_CURVE                          : 1
+ 0x00c4 (0196) B       01 cap UCLK_LIMITS                           : 1
+ 0x00c5 (0197) B       01 cap POWER_LIMIT                           : 1
+ 0x00c6 (0198) B       01 cap FAN_ACOUSTIC_LIMIT                    : 1
+ 0x00c7 (0199) B       01 cap FAN_SPEED_MIN                         : 1
+ 0x00c8 (0200) B       01 cap TEMPERATURE_FAN                       : 1
+ 0x00c9 (0201) B       01 cap TEMPERATURE_SYSTEM                    : 1
+ 0x00ca (0202) B       01 cap MEMORY_TIMING_TUNE                    : 1
+ 0x00cb (0203) B       01 cap FAN_ZERO_RPM_CONTROL                  : 1
+ 0x00cc (0204) B       01 cap AUTO_UV_ENGINE                        : 1
+ 0x00cd (0205) B       01 cap AUTO_OC_ENGINE                        : 1
+ 0x00ce (0206) B       01 cap AUTO_OC_MEMORY                        : 1
+ 0x00cf (0207) B       01 cap FAN_CURVE                             : 1
+ 0x00d0 (0208) B       00 cap SMU_11_0_ODCAP_AUTO_FAN_ACOUSTIC_LIMIT: 0
+ 0x00d1 (0209) B       01 cap POWER_MODE                            : 1
+ 0x00d2 (0210) B       00 cap                                       : 0
+ 0x00d3 (0211) B       00 cap                                       : 0
+ 0x00d4 (0212) B       00 cap                                       : 0
+ 0x00d5 (0213) B       00 cap                                       : 0
+ 0x00d6 (0214) B       00 cap                                       : 0
+ 0x00d7 (0215) B       00 cap                                       : 0
+ 0x00d8 (0216) B       00 cap                                       : 0
+ 0x00d9 (0217) B       00 cap                                       : 0
+ 0x00da (0218) B       00 cap                                       : 0
+ 0x00db (0219) B       00 cap                                       : 0
+ 0x00dc (0220) B       00 cap                                       : 0
+ 0x00dd (0221) B       00 cap                                       : 0
+ 0x00de (0222) B       00 cap                                       : 0
+ 0x00df (0223) B       00 cap                                       : 0
+ 0x00e0 (0224) B       00 cap                                       : 0
+ 0x00e1 (0225) B       00 cap                                       : 0
+ 0x00e2 (0226) I b80b0000 max GFXCLKFMAX                            : 3000
+ 0x00e6 (0230) I b80b0000 max GFXCLKFMIN                            : 3000
+ 0x00ea (0234) I 00000000 max CUSTOM_GFX_VF_CURVE_A                 : 0
+ 0x00ee (0238) I 00000000 max CUSTOM_GFX_VF_CURVE_B                 : 0
+ 0x00f2 (0242) I 00000000 max CUSTOM_GFX_VF_CURVE_C                 : 0
+ 0x00f6 (0246) I b80b0000 max CUSTOM_CURVE_VFT_FMIN                 : 3000
+ 0x00fa (0250) I 33040000 max UCLKFMIN                              : 1075
+ 0x00fe (0254) I 33040000 max UCLKFMAX                              : 1075
+ 0x0102 (0258) I 0f000000 max POWERPERCENTAGE                       : 15
+ 0x0106 (0262) I e40c0000 max FANRPMMIN                             : 3300
+ 0x010a (0266) I e40c0000 max FANRPMACOUSTICLIMIT                   : 3300
+ 0x010e (0270) I 64000000 max FANTARGETTEMPERATURE                  : 100
+ 0x0112 (0274) I 6e000000 max OPERATINGTEMPMAX                      : 110
+ 0x0116 (0278) I 01000000 max ACTIMING                              : 1
+ 0x011a (0282) I 01000000 max FAN_ZERO_RPM_CONTROL                  : 1
+ 0x011e (0286) I 01000000 max AUTOUVENGINE                          : 1
+ 0x0122 (0290) I 01000000 max AUTOOCENGINE                          : 1
+ 0x0126 (0294) I 01000000 max AUTOOCMEMORY                          : 1
+ 0x012a (0298) I 64000000 max FAN_CURVE_TEMPERATURE_1               : 100
+ 0x012e (0302) I 64000000 max FAN_CURVE_SPEED_1                     : 100
+ 0x0132 (0306) I 64000000 max FAN_CURVE_TEMPERATURE_2               : 100
+ 0x0136 (0310) I 64000000 max FAN_CURVE_SPEED_2                     : 100
+ 0x013a (0314) I 64000000 max FAN_CURVE_TEMPERATURE_3               : 100
+ 0x013e (0318) I 64000000 max FAN_CURVE_SPEED_3                     : 100
+ 0x0142 (0322) I 64000000 max FAN_CURVE_TEMPERATURE_4               : 100
+ 0x0146 (0326) I 64000000 max FAN_CURVE_SPEED_4                     : 100
+ 0x014a (0330) I 64000000 max FAN_CURVE_TEMPERATURE_5               : 100
+ 0x014e (0334) I 64000000 max FAN_CURVE_SPEED_5                     : 100
+ 0x0152 (0338) I 00000000 max AUTO_FAN_ACOUSTIC_LIMIT               : 0
+ 0x0156 (0342) I 01000000 max POWER_MODE                            : 1
+ 0x015a (0346) I 00000000 max                                       : 0
+ 0x015e (0350) I 00000000 max                                       : 0
+ 0x0162 (0354) I 00000000 max                                       : 0
+ 0x0166 (0358) I 00000000 max                                       : 0
+ 0x016a (0362) I 00000000 max                                       : 0
+ 0x016e (0366) I 00000000 max                                       : 0
+ 0x0172 (0370) I 00000000 max                                       : 0
+ 0x0176 (0374) I 00000000 max                                       : 0
+ 0x017a (0378) I 00000000 max                                       : 0
+ 0x017e (0382) I 00000000 max                                       : 0
+ 0x0182 (0386) I 00000000 max                                       : 0
+ 0x0186 (0390) I 00000000 max                                       : 0
+ 0x018a (0394) I 00000000 max                                       : 0
+ 0x018e (0398) I 00000000 max                                       : 0
+ 0x0192 (0402) I 00000000 max                                       : 0
+ 0x0196 (0406) I 00000000 max                                       : 0
+ 0x019a (0410) I 00000000 max                                       : 0
+ 0x019e (0414) I 00000000 max                                       : 0
+ 0x01a2 (0418) I 00000000 max                                       : 0
+ 0x01a6 (0422) I 00000000 max                                       : 0
+ 0x01aa (0426) I 00000000 max                                       : 0
+ 0x01ae (0430) I 00000000 max                                       : 0
+ 0x01b2 (0434) I 00000000 max                                       : 0
+ 0x01b6 (0438) I 00000000 max                                       : 0
+ 0x01ba (0442) I 00000000 max                                       : 0
+ 0x01be (0446) I 00000000 max                                       : 0
+ 0x01c2 (0450) I 00000000 max                                       : 0
+ 0x01c6 (0454) I 00000000 max                                       : 0
+ 0x01ca (0458) I 00000000 max                                       : 0
+ 0x01ce (0462) I 00000000 max                                       : 0
+ 0x01d2 (0466) I 00000000 max                                       : 0
+ 0x01d6 (0470) I 00000000 max                                       : 0
+ 0x01da (0474) I 00000000 max                                       : 0
+ 0x01de (0478) I 00000000 max                                       : 0
+ 0x01e2 (0482) I f4010000 min GFXCLKFMAX                            : 500
+ 0x01e6 (0486) I f4010000 min GFXCLKFMIN                            : 500
+ 0x01ea (0490) I 00000000 min CUSTOM_GFX_VF_CURVE_A                 : 0
+ 0x01ee (0494) I 00000000 min CUSTOM_GFX_VF_CURVE_B                 : 0
+ 0x01f2 (0498) I 00000000 min CUSTOM_GFX_VF_CURVE_C                 : 0
+ 0x01f6 (0502) I f4010000 min CUSTOM_CURVE_VFT_FMIN                 : 500
+ 0x01fa (0506) I a2020000 min UCLKFMIN                              : 674
+ 0x01fe (0510) I a2020000 min UCLKFMAX                              : 674
+ 0x0202 (0514) I 0a000000 min POWERPERCENTAGE                       : 10
+ 0x0206 (0518) I fa000000 min FANRPMMIN                             : 250
+ 0x020a (0522) I e8030000 min FANRPMACOUSTICLIMIT                   : 1000
+ 0x020e (0526) I 19000000 min FANTARGETTEMPERATURE                  : 25
+ 0x0212 (0530) I 32000000 min OPERATINGTEMPMAX                      : 50
+ 0x0216 (0534) I 00000000 min ACTIMING                              : 0
+ 0x021a (0538) I 00000000 min FAN_ZERO_RPM_CONTROL                  : 0
+ 0x021e (0542) I 00000000 min AUTOUVENGINE                          : 0
+ 0x0222 (0546) I 00000000 min AUTOOCENGINE                          : 0
+ 0x0226 (0550) I 00000000 min AUTOOCMEMORY                          : 0
+ 0x022a (0554) I 19000000 min FAN_CURVE_TEMPERATURE_1               : 25
+ 0x022e (0558) I 0a000000 min FAN_CURVE_SPEED_1                     : 10
+ 0x0232 (0562) I 19000000 min FAN_CURVE_TEMPERATURE_2               : 25
+ 0x0236 (0566) I 0a000000 min FAN_CURVE_SPEED_2                     : 10
+ 0x023a (0570) I 19000000 min FAN_CURVE_TEMPERATURE_3               : 25
+ 0x023e (0574) I 0a000000 min FAN_CURVE_SPEED_3                     : 10
+ 0x0242 (0578) I 19000000 min FAN_CURVE_TEMPERATURE_4               : 25
+ 0x0246 (0582) I 0a000000 min FAN_CURVE_SPEED_4                     : 10
+ 0x024a (0586) I 19000000 min FAN_CURVE_TEMPERATURE_5               : 25
+ 0x024e (0590) I 0a000000 min FAN_CURVE_SPEED_5                     : 10
+ 0x0252 (0594) I 00000000 min AUTO_FAN_ACOUSTIC_LIMIT               : 0
+ 0x0256 (0598) I 00000000 min POWER_MODE                            : 0
+ 0x025a (0602) I 00000000 min                                       : 0
+ 0x025e (0606) I 00000000 min                                       : 0
+ 0x0262 (0610) I 00000000 min                                       : 0
+ 0x0266 (0614) I 00000000 min                                       : 0
+ 0x026a (0618) I 00000000 min                                       : 0
+ 0x026e (0622) I 00000000 min                                       : 0
+ 0x0272 (0626) I 00000000 min                                       : 0
+ 0x0276 (0630) I 00000000 min                                       : 0
+ 0x027a (0634) I 00000000 min                                       : 0
+ 0x027e (0638) I 00000000 min                                       : 0
+ 0x0282 (0642) I 00000000 min                                       : 0
+ 0x0286 (0646) I 00000000 min                                       : 0
+ 0x028a (0650) I 00000000 min                                       : 0
+ 0x028e (0654) I 00000000 min                                       : 0
+ 0x0292 (0658) I 00000000 min                                       : 0
+ 0x0296 (0662) I 00000000 min                                       : 0
+ 0x029a (0666) I 00000000 min                                       : 0
+ 0x029e (0670) I 00000000 min                                       : 0
+ 0x02a2 (0674) I 00000000 min                                       : 0
+ 0x02a6 (0678) I 00000000 min                                       : 0
+ 0x02aa (0682) I 00000000 min                                       : 0
+ 0x02ae (0686) I 00000000 min                                       : 0
+ 0x02b2 (0690) I 00000000 min                                       : 0
+ 0x02b6 (0694) I 00000000 min                                       : 0
+ 0x02ba (0698) I 00000000 min                                       : 0
+ 0x02be (0702) I 00000000 min                                       : 0
+ 0x02c2 (0706) I 00000000 min                                       : 0
+ 0x02c6 (0710) I 00000000 min                                       : 0
+ 0x02ca (0714) I 00000000 min                                       : 0
+ 0x02ce (0718) I 00000000 min                                       : 0
+ 0x02d2 (0722) I 00000000 min                                       : 0
+ 0x02d6 (0726) I 00000000 min                                       : 0
+ 0x02da (0730) I 00000000 min                                       : 0
+ 0x02de (0734) I 00000000 min                                       : 0
+ 0x02e2 (0738) h     0600 pm_setting                                : 6
+ 0x02e4 (0740) h     0000 pm_setting                                : 0
+ 0x02e6 (0742) h     0600 pm_setting                                : 6
+ 0x02e8 (0744) h     0600 pm_setting                                : 6
+ 0x02ea (0746) h     5f00 pm_setting                                : 95
+ 0x02ec (0748) h     5f00 pm_setting                                : 95
+ 0x02ee (0750) h     5f00 pm_setting                                : 95
+ 0x02f0 (0752) h     5f00 pm_setting                                : 95
+ 0x02f2 (0754) h     7206 pm_setting                                : 1650
+ 0x02f4 (0756) h     7206 pm_setting                                : 1650
+ 0x02f6 (0758) h     d606 pm_setting                                : 1750
+ 0x02f8 (0760) h     d606 pm_setting                                : 1750
+ 0x02fa (0762) h     d007 pm_setting                                : 2000
+ 0x02fc (0764) h     d007 pm_setting                                : 2000
+ 0x02fe (0766) h     ca08 pm_setting                                : 2250
+ 0x0300 (0768) h     ca08 pm_setting                                : 2250
+ 0x0302 (0770) h     0000 pm_setting                                : 0
+ 0x0304 (0772) h     0000 pm_setting                                : 0
+ 0x0306 (0774) h     0000 pm_setting                                : 0
+ 0x0308 (0776) h     0000 pm_setting                                : 0
+ 0x030a (0778) h     0000 pm_setting                                : 0
+ 0x030c (0780) h     0000 pm_setting                                : 0
+ 0x030e (0782) h     0000 pm_setting                                : 0
+ 0x0310 (0784) h     0000 pm_setting                                : 0
+ 0x0312 (0786) h     0000 pm_setting                                : 0
+ 0x0314 (0788) h     0000 pm_setting                                : 0
+ 0x0316 (0790) h     0000 pm_setting                                : 0
+ 0x0318 (0792) h     0000 pm_setting                                : 0
+ 0x031a (0794) h     0000 pm_setting                                : 0
+ 0x031c (0796) h     0000 pm_setting                                : 0
+ 0x031e (0798) h     0000 pm_setting                                : 0
+ 0x0320 (0800) h     0000 pm_setting                                : 0
+ 0x0322 (0802) I 06000000 Version                                   : 6
+ 0x0326 (0806) I fffd7fa3 FeaturesToRun                             : 2743074303
+ 0x032a (0810) I 63370000 FeaturesToRun                             : 14179
+ 0x032e (0814) H     ff00 SocketPowerLimitAc                        : 255
+ 0x0330 (0816) H     0000 SocketPowerLimitAc                        : 0
+ 0x0332 (0818) H     0000 SocketPowerLimitAc                        : 0
+ 0x0334 (0820) H     0000 SocketPowerLimitAc                        : 0
+ 0x0336 (0822) H     0000 SocketPowerLimitAcTau                     : 0
+ 0x0338 (0824) H     0000 SocketPowerLimitAcTau                     : 0
+ 0x033a (0826) H     0000 SocketPowerLimitAcTau                     : 0
+ 0x033c (0828) H     0000 SocketPowerLimitAcTau                     : 0
+ 0x033e (0830) H     ff00 SocketPowerLimitDc                        : 255
+ 0x0340 (0832) H     0000 SocketPowerLimitDc                        : 0
+ 0x0342 (0834) H     0000 SocketPowerLimitDc                        : 0
+ 0x0344 (0836) H     0000 SocketPowerLimitDc                        : 0
+ 0x0346 (0838) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x0348 (0840) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x034a (0842) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x034c (0844) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x034e (0846) H     4001 TdcLimit                                  : 320
+ 0x0350 (0848) H     3700 TdcLimit                                  : 55
+ 0x0352 (0850) H     0000 TdcLimitTau                               : 0
+ 0x0354 (0852) H     0000 TdcLimitTau                               : 0
+ 0x0356 (0854) H     6400 TemperatureLimit                          : 100
+ 0x0358 (0856) H     6e00 TemperatureLimit                          : 110
+ 0x035a (0858) H     6400 TemperatureLimit                          : 100
+ 0x035c (0860) H     7300 TemperatureLimit                          : 115
+ 0x035e (0862) H     7300 TemperatureLimit                          : 115
+ 0x0360 (0864) H     7300 TemperatureLimit                          : 115
+ 0x0362 (0866) H     7300 TemperatureLimit                          : 115
+ 0x0364 (0868) H     0000 TemperatureLimit                          : 0
+ 0x0366 (0870) H     0000 TemperatureLimit                          : 0
+ 0x0368 (0872) H     0000 TemperatureLimit                          : 0
+ 0x036a (0874) I 00000000 FitLimit                                  : 0
+ 0x036e (0878) B       01 TotalPowerConfig                          : 1
+ 0x036f (0879) B       00 TotalPowerPadding                         : 0
+ 0x0370 (0880) B       00 TotalPowerPadding                         : 0
+ 0x0371 (0881) B       00 TotalPowerPadding                         : 0
+ 0x0372 (0882) I 0a000000 ApccPlusResidencyLimit                    : 10
+ 0x0376 (0886) H     0000 SmnclkDpmFreq                             : 0
+ 0x0378 (0888) H     0000 SmnclkDpmFreq                             : 0
+ 0x037a (0890) H     0000 SmnclkDpmVoltage                          : 0
+ 0x037c (0892) H     0000 SmnclkDpmVoltage                          : 0
+ 0x037e (0894) I 00000000 PaddingAPCC                               : 0
+ 0x0382 (0898) H     0000 PerPartDroopVsetGfxDfll                   : 0
+ 0x0384 (0900) H     0000 PerPartDroopVsetGfxDfll                   : 0
+ 0x0386 (0902) H     0000 PerPartDroopVsetGfxDfll                   : 0
+ 0x0388 (0904) H     0000 PerPartDroopVsetGfxDfll                   : 0
+ 0x038a (0906) H     0000 PerPartDroopVsetGfxDfll                   : 0
+ 0x038c (0908) H     0000 PaddingPerPartDroop                       : 0
+ 0x038e (0910) I fe380000 ThrottlerControlMask                      : 14590
+ 0x0392 (0914) I 730f0000 FwDStateMask                              : 3955
+ 0x0396 (0918) H     6400 UlvVoltageOffsetSoc                       : 100
+ 0x0398 (0920) H     6400 UlvVoltageOffsetGfx                       : 100
+ 0x039a (0922) H     1c0c MinVoltageUlvGfx                          : 3100
+ 0x039c (0924) H     800c MinVoltageUlvSoc                          : 3200
+ 0x039e (0926) H     0000 SocLIVmin                                 : 0
+ 0x03a0 (0928) H     0000 PaddingLIVmin                             : 0
+ 0x03a2 (0930) B       00 GceaLinkMgrIdleThreshold                  : 0
+ 0x03a3 (0931) B       00 RlcUlvParams                              : 0
+ 0x03a4 (0932) B       00 RlcUlvParams                              : 0
+ 0x03a5 (0933) B       00 RlcUlvParams                              : 0
+ 0x03a6 (0934) H     e40c MinVoltageGfx                             : 3300
+ 0x03a8 (0936) H     e40c MinVoltageSoc                             : 3300
+ 0x03aa (0938) H     5c12 MaxVoltageGfx                             : 4700
+ 0x03ac (0940) H     f811 MaxVoltageSoc                             : 4600
+ 0x03ae (0942) H     4000 LoadLineResistanceGfx                     : 64
+ 0x03b0 (0944) H     0001 LoadLineResistanceSoc                     : 256
+ 0x03b2 (0946) H     3200 VDDGFX_TVmin                              : 50
+ 0x03b4 (0948) H     3c00 VDDSOC_TVmin                              : 60
+ 0x03b6 (0950) H     800c VDDGFX_Vmin_HiTemp                        : 3200
+ 0x03b8 (0952) H     800c VDDGFX_Vmin_LoTemp                        : 3200
+ 0x03ba (0954) H     800c VDDSOC_Vmin_HiTemp                        : 3200
+ 0x03bc (0956) H     800c VDDSOC_Vmin_LoTemp                        : 3200
+ 0x03be (0958) H     1400 VDDGFX_TVminHystersis                     : 20
+ 0x03c0 (0960) H     1400 VDDSOC_TVminHystersis                     : 20
+ 0x03c2 (0962) B       00 VoltageMode                               : 0
+ 0x03c3 (0963) B       00 SnapToDiscrete                            : 0
+ 0x03c4 (0964) B       02 NumDiscreteLevels                         : 2
+ 0x03c5 (0965) B       00 Padding                                   : 0
+ 0x03c6 (0966) f 0000803f m                                         : 1
+ 0x03ca (0970) f 00000000 b                                         : 0
+ 0x03ce (0974) f b537b83e a                                         : 0.3598
+ 0x03d2 (0978) f ef1b67bf b                                         :-0.90277
+ 0x03d6 (0982) f 4f40a73f c                                         : 1.30665
+ 0x03da (0986) H     8b04 SsFmin                                    : 1163
+ 0x03dc (0988) H     0000 Padding16                                 : 0
+ 0x03de (0990) B       00 VoltageMode                               : 0
+ 0x03df (0991) B       00 SnapToDiscrete                            : 0
+ 0x03e0 (0992) B       02 NumDiscreteLevels                         : 2
+ 0x03e1 (0993) B       00 Padding                                   : 0
+ 0x03e2 (0994) f ee7c8f3f m                                         : 1.121
+ 0x03e6 (0998) f a69b843e b                                         : 0.259
+ 0x03ea (1002) f 44349a3e a                                         : 0.30118
+ 0x03ee (1006) f 43ad09be b                                         :-0.13445
+ 0x03f2 (1010) f 3d0f363f c                                         : 0.71117
+ 0x03f6 (1014) H     f100 SsFmin                                    : 241
+ 0x03f8 (1016) H     0000 Padding16                                 : 0
+ 0x03fa (1018) B       00 VoltageMode                               : 0
+ 0x03fb (1019) B       01 SnapToDiscrete                            : 1
+ 0x03fc (1020) B       04 NumDiscreteLevels                         : 4
+ 0x03fd (1021) B       00 Padding                                   : 0
+ 0x03fe (1022) f cdccac3f m                                         : 1.35
+ 0x0402 (1026) f e3a59bbd b                                         :-0.076
+ 0x0406 (1030) f 6f81e43e a                                         : 0.4463
+ 0x040a (1034) f caa6ccbe b                                         :-0.39971
+ 0x040e (1038) f 0421493f c                                         : 0.78566
+ 0x0412 (1042) H     c001 SsFmin                                    : 448
+ 0x0414 (1044) H     0000 Padding16                                 : 0
+ 0x0416 (1046) B       00 VoltageMode                               : 0
+ 0x0417 (1047) B       00 SnapToDiscrete                            : 0
+ 0x0418 (1048) B       02 NumDiscreteLevels                         : 2
+ 0x0419 (1049) B       00 Padding                                   : 0
+ 0x041a (1050) f 0000803f m                                         : 1
+ 0x041e (1054) f 00000000 b                                         : 0
+ 0x0422 (1058) f 72c47a3e a                                         : 0.24489
+ 0x0426 (1062) f 4c8984be b                                         :-0.25886
+ 0x042a (1066) f dcba433f c                                         : 0.76457
+ 0x042e (1070) H     1102 SsFmin                                    : 529
+ 0x0430 (1072) H     0000 Padding16                                 : 0
+ 0x0432 (1074) B       00 VoltageMode                               : 0
+ 0x0433 (1075) B       00 SnapToDiscrete                            : 0
+ 0x0434 (1076) B       02 NumDiscreteLevels                         : 2
+ 0x0435 (1077) B       00 Padding                                   : 0
+ 0x0436 (1078) f 098aaf3f m                                         : 1.3714
+ 0x043a (1082) f 295c0fbd b                                         :-0.035
+ 0x043e (1086) f 85ceeb3e a                                         : 0.46056
+ 0x0442 (1090) f 10ccc1be b                                         :-0.37851
+ 0x0446 (1094) f 4720463f c                                         : 0.77393
+ 0x044a (1098) H     9b01 SsFmin                                    : 411
+ 0x044c (1100) H     0000 Padding16                                 : 0
+ 0x044e (1102) B       00 VoltageMode                               : 0
+ 0x044f (1103) B       00 SnapToDiscrete                            : 0
+ 0x0450 (1104) B       02 NumDiscreteLevels                         : 2
+ 0x0451 (1105) B       00 Padding                                   : 0
+ 0x0452 (1106) f 6ade893f m                                         : 1.0771
+ 0x0456 (1110) f b81e053e b                                         : 0.13
+ 0x045a (1114) f 8e75913e a                                         : 0.2841
+ 0x045e (1118) f 284957be b                                         :-0.21024
+ 0x0462 (1122) f e42c3c3f c                                         : 0.73506
+ 0x0466 (1126) H     7301 SsFmin                                    : 371
+ 0x0468 (1128) H     0000 Padding16                                 : 0
+ 0x046a (1130) B       00 VoltageMode                               : 0
+ 0x046b (1131) B       00 SnapToDiscrete                            : 0
+ 0x046c (1132) B       02 NumDiscreteLevels                         : 2
+ 0x046d (1133) B       00 Padding                                   : 0
+ 0x046e (1134) f 098aaf3f m                                         : 1.3714
+ 0x0472 (1138) f 295c0fbd b                                         :-0.035
+ 0x0476 (1142) f 85ceeb3e a                                         : 0.46056
+ 0x047a (1146) f 10ccc1be b                                         :-0.37851
+ 0x047e (1150) f 4720463f c                                         : 0.77393
+ 0x0482 (1154) H     9b01 SsFmin                                    : 411
+ 0x0484 (1156) H     0000 Padding16                                 : 0
+ 0x0486 (1158) B       00 VoltageMode                               : 0
+ 0x0487 (1159) B       00 SnapToDiscrete                            : 0
+ 0x0488 (1160) B       02 NumDiscreteLevels                         : 2
+ 0x0489 (1161) B       00 Padding                                   : 0
+ 0x048a (1162) f 6ade893f m                                         : 1.0771
+ 0x048e (1166) f b81e053e b                                         : 0.13
+ 0x0492 (1170) f 8e75913e a                                         : 0.2841
+ 0x0496 (1174) f 284957be b                                         :-0.21024
+ 0x049a (1178) f e42c3c3f c                                         : 0.73506
+ 0x049e (1182) H     7301 SsFmin                                    : 371
+ 0x04a0 (1184) H     0000 Padding16                                 : 0
+ 0x04a2 (1186) B       00 VoltageMode                               : 0
+ 0x04a3 (1187) B       00 SnapToDiscrete                            : 0
+ 0x04a4 (1188) B       02 NumDiscreteLevels                         : 2
+ 0x04a5 (1189) B       00 Padding                                   : 0
+ 0x04a6 (1190) f 7d3f953f m                                         : 1.166
+ 0x04aa (1194) f dd24063e b                                         : 0.131
+ 0x04ae (1198) f 1d77aa3e a                                         : 0.33294
+ 0x04b2 (1202) f ee7768be b                                         :-0.22702
+ 0x04b6 (1206) f c91f3c3f c                                         : 0.73486
+ 0x04ba (1210) H     5501 SsFmin                                    : 341
+ 0x04bc (1212) H     0000 Padding16                                 : 0
+ 0x04be (1214) B       00 VoltageMode                               : 0
+ 0x04bf (1215) B       00 SnapToDiscrete                            : 0
+ 0x04c0 (1216) B       02 NumDiscreteLevels                         : 2
+ 0x04c1 (1217) B       00 Padding                                   : 0
+ 0x04c2 (1218) f 6abc743f m                                         : 0.956
+ 0x04c6 (1222) f ae47613e b                                         : 0.22
+ 0x04ca (1226) f 732e653e a                                         : 0.22381
+ 0x04ce (1230) f 52ed13be b                                         :-0.14446
+ 0x04d2 (1234) f d72f383f c                                         : 0.71948
+ 0x04d6 (1238) H     4301 SsFmin                                    : 323
+ 0x04d8 (1240) H     0000 Padding16                                 : 0
+ 0x04da (1242) B       00 VoltageMode                               : 0
+ 0x04db (1243) B       00 SnapToDiscrete                            : 0
+ 0x04dc (1244) B       02 NumDiscreteLevels                         : 2
+ 0x04dd (1245) B       00 Padding                                   : 0
+ 0x04de (1246) f 6abc743f m                                         : 0.956
+ 0x04e2 (1250) f ae47613e b                                         : 0.22
+ 0x04e6 (1254) f 732e653e a                                         : 0.22381
+ 0x04ea (1258) f 52ed13be b                                         :-0.14446
+ 0x04ee (1262) f d72f383f c                                         : 0.71948
+ 0x04f2 (1266) H     4301 SsFmin                                    : 323
+ 0x04f4 (1268) H     0000 Padding16                                 : 0
+ 0x04f6 (1270) B       00 VoltageMode                               : 0
+ 0x04f7 (1271) B       00 SnapToDiscrete                            : 0
+ 0x04f8 (1272) B       02 NumDiscreteLevels                         : 2
+ 0x04f9 (1273) B       00 Padding                                   : 0
+ 0x04fa (1274) f 0e2d123f m                                         : 0.571
+ 0x04fe (1278) f 9a99d93e b                                         : 0.425
+ 0x0502 (1282) f 2783a33d a                                         : 0.07984
+ 0x0506 (1286) f 8d28edbc b                                         :-0.02895
+ 0x050a (1290) f e7e3323f c                                         : 0.69879
+ 0x050e (1294) H     b600 SsFmin                                    : 182
+ 0x0510 (1296) H     0000 Padding16                                 : 0
+ 0x0512 (1298) B       00 VoltageMode                               : 0
+ 0x0513 (1299) B       00 SnapToDiscrete                            : 0
+ 0x0514 (1300) B       02 NumDiscreteLevels                         : 2
+ 0x0515 (1301) B       00 Padding                                   : 0
+ 0x0516 (1302) f 6abc743f m                                         : 0.956
+ 0x051a (1306) f ae47613e b                                         : 0.22
+ 0x051e (1310) f 732e653e a                                         : 0.22381
+ 0x0522 (1314) f 52ed13be b                                         :-0.14446
+ 0x0526 (1318) f d72f383f c                                         : 0.71948
+ 0x052a (1322) H     4301 SsFmin                                    : 323
+ 0x052c (1324) H     0000 Padding16                                 : 0
+ 0x052e (1326) H     f401 FreqTableGfx                              : 500
+ 0x0530 (1328) H     640a FreqTableGfx                              : 2660
+ 0x0532 (1330) H     0000 FreqTableGfx                              : 0
+ 0x0534 (1332) H     0000 FreqTableGfx                              : 0
+ 0x0536 (1334) H     0000 FreqTableGfx                              : 0
+ 0x0538 (1336) H     0000 FreqTableGfx                              : 0
+ 0x053a (1338) H     0000 FreqTableGfx                              : 0
+ 0x053c (1340) H     0000 FreqTableGfx                              : 0
+ 0x053e (1342) H     0000 FreqTableGfx                              : 0
+ 0x0540 (1344) H     0000 FreqTableGfx                              : 0
+ 0x0542 (1346) H     0000 FreqTableGfx                              : 0
+ 0x0544 (1348) H     0000 FreqTableGfx                              : 0
+ 0x0546 (1350) H     0000 FreqTableGfx                              : 0
+ 0x0548 (1352) H     0000 FreqTableGfx                              : 0
+ 0x054a (1354) H     0000 FreqTableGfx                              : 0
+ 0x054c (1356) H     0000 FreqTableGfx                              : 0
+ 0x054e (1358) H     6b01 FreqTableVclk                             : 363
+ 0x0550 (1360) H     c505 FreqTableVclk                             : 1477
+ 0x0552 (1362) H     0000 FreqTableVclk                             : 0
+ 0x0554 (1364) H     0000 FreqTableVclk                             : 0
+ 0x0556 (1366) H     0000 FreqTableVclk                             : 0
+ 0x0558 (1368) H     0000 FreqTableVclk                             : 0
+ 0x055a (1370) H     0000 FreqTableVclk                             : 0
+ 0x055c (1372) H     0000 FreqTableVclk                             : 0
+ 0x055e (1374) H     3d01 FreqTableDclk                             : 317
+ 0x0560 (1376) H     f204 FreqTableDclk                             : 1266
+ 0x0562 (1378) H     0000 FreqTableDclk                             : 0
+ 0x0564 (1380) H     0000 FreqTableDclk                             : 0
+ 0x0566 (1382) H     0000 FreqTableDclk                             : 0
+ 0x0568 (1384) H     0000 FreqTableDclk                             : 0
+ 0x056a (1386) H     0000 FreqTableDclk                             : 0
+ 0x056c (1388) H     0000 FreqTableDclk                             : 0
+ 0x056e (1390) H     e001 FreqTableSocclk                           : 480
+ 0x0570 (1392) H     b004 FreqTableSocclk                           : 1200
+ 0x0572 (1394) H     0000 FreqTableSocclk                           : 0
+ 0x0574 (1396) H     0000 FreqTableSocclk                           : 0
+ 0x0576 (1398) H     0000 FreqTableSocclk                           : 0
+ 0x0578 (1400) H     0000 FreqTableSocclk                           : 0
+ 0x057a (1402) H     0000 FreqTableSocclk                           : 0
+ 0x057c (1404) H     0000 FreqTableSocclk                           : 0
+ 0x057e (1406) H     6100 FreqTableUclk                             : 97
+ 0x0580 (1408) H     c901 FreqTableUclk                             : 457
+ 0x0582 (1410) H     a202 FreqTableUclk                             : 674
+ 0x0584 (1412) H     e803 FreqTableUclk                             : 1000
+ 0x0586 (1414) H     a201 FreqTableDcefclk                          : 418
+ 0x0588 (1416) H     b004 FreqTableDcefclk                          : 1200
+ 0x058a (1418) H     0000 FreqTableDcefclk                          : 0
+ 0x058c (1420) H     0000 FreqTableDcefclk                          : 0
+ 0x058e (1422) H     0000 FreqTableDcefclk                          : 0
+ 0x0590 (1424) H     0000 FreqTableDcefclk                          : 0
+ 0x0592 (1426) H     0000 FreqTableDcefclk                          : 0
+ 0x0594 (1428) H     0000 FreqTableDcefclk                          : 0
+ 0x0596 (1430) H     e701 FreqTableDispclk                          : 487
+ 0x0598 (1432) H     c104 FreqTableDispclk                          : 1217
+ 0x059a (1434) H     0000 FreqTableDispclk                          : 0
+ 0x059c (1436) H     0000 FreqTableDispclk                          : 0
+ 0x059e (1438) H     0000 FreqTableDispclk                          : 0
+ 0x05a0 (1440) H     0000 FreqTableDispclk                          : 0
+ 0x05a2 (1442) H     0000 FreqTableDispclk                          : 0
+ 0x05a4 (1444) H     0000 FreqTableDispclk                          : 0
+ 0x05a6 (1446) H     e701 FreqTablePixclk                           : 487
+ 0x05a8 (1448) H     c104 FreqTablePixclk                           : 1217
+ 0x05aa (1450) H     0000 FreqTablePixclk                           : 0
+ 0x05ac (1452) H     0000 FreqTablePixclk                           : 0
+ 0x05ae (1454) H     0000 FreqTablePixclk                           : 0
+ 0x05b0 (1456) H     0000 FreqTablePixclk                           : 0
+ 0x05b2 (1458) H     0000 FreqTablePixclk                           : 0
+ 0x05b4 (1460) H     0000 FreqTablePixclk                           : 0
+ 0x05b6 (1462) H     2c01 FreqTablePhyclk                           : 300
+ 0x05b8 (1464) H     2a03 FreqTablePhyclk                           : 810
+ 0x05ba (1466) H     0000 FreqTablePhyclk                           : 0
+ 0x05bc (1468) H     0000 FreqTablePhyclk                           : 0
+ 0x05be (1470) H     0000 FreqTablePhyclk                           : 0
+ 0x05c0 (1472) H     0000 FreqTablePhyclk                           : 0
+ 0x05c2 (1474) H     0000 FreqTablePhyclk                           : 0
+ 0x05c4 (1476) H     0000 FreqTablePhyclk                           : 0
+ 0x05c6 (1478) H     e701 FreqTableDtbclk                           : 487
+ 0x05c8 (1480) H     c104 FreqTableDtbclk                           : 1217
+ 0x05ca (1482) H     0000 FreqTableDtbclk                           : 0
+ 0x05cc (1484) H     0000 FreqTableDtbclk                           : 0
+ 0x05ce (1486) H     0000 FreqTableDtbclk                           : 0
+ 0x05d0 (1488) H     0000 FreqTableDtbclk                           : 0
+ 0x05d2 (1490) H     0000 FreqTableDtbclk                           : 0
+ 0x05d4 (1492) H     0000 FreqTableDtbclk                           : 0
+ 0x05d6 (1494) H     2602 FreqTableFclk                             : 550
+ 0x05d8 (1496) H     9407 FreqTableFclk                             : 1940
+ 0x05da (1498) H     0000 FreqTableFclk                             : 0
+ 0x05dc (1500) H     0000 FreqTableFclk                             : 0
+ 0x05de (1502) H     0000 FreqTableFclk                             : 0
+ 0x05e0 (1504) H     0000 FreqTableFclk                             : 0
+ 0x05e2 (1506) H     0000 FreqTableFclk                             : 0
+ 0x05e4 (1508) H     0000 FreqTableFclk                             : 0
+ 0x05e6 (1510) I 00000000 Paddingclks                               : 0
+ 0x05ea (1514) f 00000000 a                                         : 0
+ 0x05ee (1518) f 00000000 b                                         : 0
+ 0x05f2 (1522) f 00000000 c                                         : 0
+ 0x05f6 (1526) f 00000000 a                                         : 0
+ 0x05fa (1530) f 00000000 b                                         : 0
+ 0x05fe (1534) f 00000000 c                                         : 0
+ 0x0602 (1538) f 00000000 a                                         : 0
+ 0x0606 (1542) f 00000000 b                                         : 0
+ 0x060a (1546) f 00000000 c                                         : 0
+ 0x060e (1550) f 00000000 a                                         : 0
+ 0x0612 (1554) f 00000000 b                                         : 0
+ 0x0616 (1558) f 00000000 c                                         : 0
+ 0x061a (1562) f 00000000 a                                         : 0
+ 0x061e (1566) f 00000000 b                                         : 0
+ 0x0622 (1570) f 00000000 c                                         : 0
+ 0x0626 (1574) I 640a0000 DcModeMaxFreq                             : 2660
+ 0x062a (1578) I b0040000 DcModeMaxFreq                             : 1200
+ 0x062e (1582) I e8030000 DcModeMaxFreq                             : 1000
+ 0x0632 (1586) I 94070000 DcModeMaxFreq                             : 1940
+ 0x0636 (1590) I f2040000 DcModeMaxFreq                             : 1266
+ 0x063a (1594) I c5050000 DcModeMaxFreq                             : 1477
+ 0x063e (1598) I f2040000 DcModeMaxFreq                             : 1266
+ 0x0642 (1602) I c5050000 DcModeMaxFreq                             : 1477
+ 0x0646 (1606) I b0040000 DcModeMaxFreq                             : 1200
+ 0x064a (1610) I c1040000 DcModeMaxFreq                             : 1217
+ 0x064e (1614) I c1040000 DcModeMaxFreq                             : 1217
+ 0x0652 (1618) I 2a030000 DcModeMaxFreq                             : 810
+ 0x0656 (1622) I c1040000 DcModeMaxFreq                             : 1217
+ 0x065a (1626) B       00 FreqTableUclkDiv                          : 0
+ 0x065b (1627) B       02 FreqTableUclkDiv                          : 2
+ 0x065c (1628) B       03 FreqTableUclkDiv                          : 3
+ 0x065d (1629) B       03 FreqTableUclkDiv                          : 3
+ 0x065e (1630) H     7805 FclkBoostFreq                             : 1400
+ 0x0660 (1632) H     0000 FclkParamPadding                          : 0
+ 0x0662 (1634) H     4c01 Mp0clkFreq                                : 332
+ 0x0664 (1636) H     fa01 Mp0clkFreq                                : 506
+ 0x0666 (1638) H     f00a Mp0DpmVoltage                             : 2800
+ 0x0668 (1640) H     800c Mp0DpmVoltage                             : 3200
+ 0x066a (1642) H     8c0a MemVddciVoltage                           : 2700
+ 0x066c (1644) H     800c MemVddciVoltage                           : 3200
+ 0x066e (1646) H     480d MemVddciVoltage                           : 3400
+ 0x0670 (1648) H     480d MemVddciVoltage                           : 3400
+ 0x0672 (1650) H     8813 MemMvddVoltage                            : 5000
+ 0x0674 (1652) H     1815 MemMvddVoltage                            : 5400
+ 0x0676 (1654) H     1815 MemMvddVoltage                            : 5400
+ 0x0678 (1656) H     1815 MemMvddVoltage                            : 5400
+ 0x067a (1658) H     f401 GfxclkFgfxoffEntry                        : 500
+ 0x067c (1660) H     2003 GfxclkFinit                               : 800
+ 0x067e (1662) H     f401 GfxclkFidle                               : 500
+ 0x0680 (1664) B       01 GfxclkSource                              : 1
+ 0x0681 (1665) B       00 GfxclkPadding                             : 0
+ 0x0682 (1666) B       01 GfxGpoSubFeatureMask                      : 1
+ 0x0683 (1667) B       02 GfxGpoEnabledWorkPolicyMask               : 2
+ 0x0684 (1668) B       5d GfxGpoDisabledWorkPolicyMask              : 93
+ 0x0685 (1669) B       00 GfxGpoPadding                             : 0
+ 0x0686 (1670) I 01000000 GfxGpoVotingAllow                         : 1
+ 0x068a (1674) I 00000000 GfxGpoPadding32                           : 0
+ 0x068e (1678) I 00000000 GfxGpoPadding32                           : 0
+ 0x0692 (1682) I 00000000 GfxGpoPadding32                           : 0
+ 0x0696 (1686) I 00000000 GfxGpoPadding32                           : 0
+ 0x069a (1690) H     0000 GfxDcsFopt                                : 0
+ 0x069c (1692) H     0000 GfxDcsFclkFopt                            : 0
+ 0x069e (1694) H     0000 GfxDcsUclkFopt                            : 0
+ 0x06a0 (1696) H     0000 DcsGfxOffVoltage                          : 0
+ 0x06a2 (1698) H     0000 DcsMinGfxOffTime                          : 0
+ 0x06a4 (1700) H     0000 DcsMaxGfxOffTime                          : 0
+ 0x06a6 (1702) I 00000000 DcsMinCreditAccum                         : 0
+ 0x06aa (1706) H     0000 DcsExitHysteresis                         : 0
+ 0x06ac (1708) H     0000 DcsTimeout                                : 0
+ 0x06ae (1710) I 00000000 DcsParamPadding                           : 0
+ 0x06b2 (1714) I 00000000 DcsParamPadding                           : 0
+ 0x06b6 (1718) I 00000000 DcsParamPadding                           : 0
+ 0x06ba (1722) I 00000000 DcsParamPadding                           : 0
+ 0x06be (1726) I 00000000 DcsParamPadding                           : 0
+ 0x06c2 (1730) H     2a16 FlopsPerByteTable                         : 5674
+ 0x06c4 (1732) H     d715 FlopsPerByteTable                         : 5591
+ 0x06c6 (1734) H     8415 FlopsPerByteTable                         : 5508
+ 0x06c8 (1736) H     3015 FlopsPerByteTable                         : 5424
+ 0x06ca (1738) H     dd14 FlopsPerByteTable                         : 5341
+ 0x06cc (1740) H     8a14 FlopsPerByteTable                         : 5258
+ 0x06ce (1742) H     3614 FlopsPerByteTable                         : 5174
+ 0x06d0 (1744) H     e313 FlopsPerByteTable                         : 5091
+ 0x06d2 (1746) H     9013 FlopsPerByteTable                         : 5008
+ 0x06d4 (1748) H     3d13 FlopsPerByteTable                         : 4925
+ 0x06d6 (1750) H     e912 FlopsPerByteTable                         : 4841
+ 0x06d8 (1752) H     9612 FlopsPerByteTable                         : 4758
+ 0x06da (1754) H     b111 FlopsPerByteTable                         : 4529
+ 0x06dc (1756) H     cc10 FlopsPerByteTable                         : 4300
+ 0x06de (1758) H     e70f FlopsPerByteTable                         : 4071
+ 0x06e0 (1760) H     020f FlopsPerByteTable                         : 3842
+ 0x06e2 (1762) B       00 LowestUclkReservedForUlv                  : 0
+ 0x06e3 (1763) B       00 PaddingMem                                : 0
+ 0x06e4 (1764) B       00 PaddingMem                                : 0
+ 0x06e5 (1765) B       00 PaddingMem                                : 0
+ 0x06e6 (1766) B       03 UclkDpmPstates                            : 3
+ 0x06e7 (1767) B       02 UclkDpmPstates                            : 2
+ 0x06e8 (1768) B       01 UclkDpmPstates                            : 1
+ 0x06e9 (1769) B       00 UclkDpmPstates                            : 0
+ 0x06ea (1770) H     0000 Fmin                                      : 0
+ 0x06ec (1772) H     0000 Fmax                                      : 0
+ 0x06ee (1774) H     0000 Fmin                                      : 0
+ 0x06f0 (1776) H     0000 Fmax                                      : 0
+ 0x06f2 (1778) H     0000 UclkDpmMidstepFreq                        : 0
+ 0x06f4 (1780) H     0000 UclkMidstepPadding                        : 0
+ 0x06f6 (1782) B       00 PcieGenSpeed                              : 0
+ 0x06f7 (1783) B       03 PcieGenSpeed                              : 3
+ 0x06f8 (1784) B       01 PcieLaneCount                             : 1
+ 0x06f9 (1785) B       06 PcieLaneCount                             : 6
+ 0x06fa (1786) H     3601 LclkFreq                                  : 310
+ 0x06fc (1788) H     6b02 LclkFreq                                  : 619
+ 0x06fe (1790) H     3700 FanStopTemp                               : 55
+ 0x0700 (1792) H     4600 FanStartTemp                              : 70
+ 0x0702 (1794) H     9001 FanGain                                   : 400
+ 0x0704 (1796) H     9001 FanGain                                   : 400
+ 0x0706 (1798) H     9001 FanGain                                   : 400
+ 0x0708 (1800) H     9001 FanGain                                   : 400
+ 0x070a (1802) H     9001 FanGain                                   : 400
+ 0x070c (1804) H     9001 FanGain                                   : 400
+ 0x070e (1806) H     9001 FanGain                                   : 400
+ 0x0710 (1808) H     9001 FanGain                                   : 400
+ 0x0712 (1810) H     9001 FanGain                                   : 400
+ 0x0714 (1812) H     9001 FanGain                                   : 400
+ 0x0716 (1814) H     1900 FanPwmMin                                 : 25
+ 0x0718 (1816) H     7206 FanAcousticLimitRpm                       : 1650
+ 0x071a (1818) H     d007 FanThrottlingRpm                          : 2000
+ 0x071c (1820) H     e40c FanMaximumRpm                             : 3300
+ 0x071e (1822) H     0000 MGpuFanBoostLimitRpm                      : 0
+ 0x0720 (1824) H     5f00 FanTargetTemperature                      : 95
+ 0x0722 (1826) H     f401 FanTargetGfxclk                           : 500
+ 0x0724 (1828) H     0000 FanPadding16                              : 0
+ 0x0726 (1830) B       01 FanTempInputSelect                        : 1
+ 0x0727 (1831) B       00 FanPadding                                : 0
+ 0x0728 (1832) B       01 FanZeroRpmEnable                          : 1
+ 0x0729 (1833) B       02 FanTachEdgePerRev                         : 2
+ 0x072a (1834) h     0000 FuzzyFan_ErrorSetDelta                    : 0
+ 0x072c (1836) h     0000 FuzzyFan_ErrorRateSetDelta                : 0
+ 0x072e (1838) h     0000 FuzzyFan_PwmSetDelta                      : 0
+ 0x0730 (1840) H     0000 FuzzyFan_Reserved                         : 0
+ 0x0732 (1842) B       00 OverrideAvfsGb                            : 0
+ 0x0733 (1843) B       00 OverrideAvfsGb                            : 0
+ 0x0734 (1844) B       01 BtcGbGfxDfllModelSelect                   : 1
+ 0x0735 (1845) B       00 Padding8_Avfs                             : 0
+ 0x0736 (1846) f 00000000 a                                         : 0
+ 0x073a (1850) f 00000000 b                                         : 0
+ 0x073e (1854) f 00000000 c                                         : 0
+ 0x0742 (1858) f 00000000 a                                         : 0
+ 0x0746 (1862) f 00000000 b                                         : 0
+ 0x074a (1866) f 00000000 c                                         : 0
+ 0x074e (1870) f 0d54863d a                                         : 0.06559
+ 0x0752 (1874) f bc05d2bd b                                         :-0.10255
+ 0x0756 (1878) f 1f80143e c                                         : 0.14502
+ 0x075a (1882) f 00000000 a                                         : 0
+ 0x075e (1886) f 00000000 b                                         : 0
+ 0x0762 (1890) f 00000000 c                                         : 0
+ 0x0766 (1894) f 00000000 a                                         : 0
+ 0x076a (1898) f 00000000 b                                         : 0
+ 0x076e (1902) f 00000000 c                                         : 0
+ 0x0772 (1906) f 00000000 m                                         : 0
+ 0x0776 (1910) f 00000000 b                                         : 0
+ 0x077a (1914) f 00000000 m                                         : 0
+ 0x077e (1918) f 00000000 b                                         : 0
+ 0x0782 (1922) f 9a99993e Fset                                      : 0.3
+ 0x0786 (1926) f 0000c03f Fset                                      : 1.5
+ 0x078a (1930) f 33331340 Fset                                      : 2.3
+ 0x078e (1934) f 00002040 Fset                                      : 2.5
+ 0x0792 (1938) f 66664640 Fset                                      : 3.1
+ 0x0796 (1942) f 0ad7233d Vdroop                                    : 0.04
+ 0x079a (1946) f dd24863d Vdroop                                    : 0.0655
+ 0x079e (1950) f a245b63d Vdroop                                    : 0.089
+ 0x07a2 (1954) f 39b4c83d Vdroop                                    : 0.098
+ 0x07a6 (1958) f c74bb73e Vdroop                                    : 0.358
+ 0x07aa (1962) f 7593983d a                                         : 0.0745
+ 0x07ae (1966) f 2fdd84be b                                         :-0.2595
+ 0x07b2 (1970) f a3927a3e c                                         : 0.2447
+ 0x07b6 (1974) f e56121bd a                                         :-0.0394
+ 0x07ba (1978) f 04568e3e b                                         : 0.278
+ 0x07be (1982) f c5722bbe c                                         :-0.16743
+ 0x07c2 (1986) H     c000 DcTol                                     : 192
+ 0x07c4 (1988) H     c000 DcTol                                     : 192
+ 0x07c6 (1990) B       01 DcBtcEnabled                              : 1
+ 0x07c7 (1991) B       01 DcBtcEnabled                              : 1
+ 0x07c8 (1992) B       00 Padding8_GfxBtc                           : 0
+ 0x07c9 (1993) B       00 Padding8_GfxBtc                           : 0
+ 0x07ca (1994) H     0000 DcBtcMin                                  : 0
+ 0x07cc (1996) H     0000 DcBtcMin                                  : 0
+ 0x07ce (1998) H     c000 DcBtcMax                                  : 192
+ 0x07d0 (2000) H     c000 DcBtcMax                                  : 192
+ 0x07d2 (2002) H     1900 DcBtcGb                                   : 25
+ 0x07d4 (2004) H     1900 DcBtcGb                                   : 25
+ 0x07d6 (2006) B       00 XgmiDpmPstates                            : 0
+ 0x07d7 (2007) B       00 XgmiDpmPstates                            : 0
+ 0x07d8 (2008) B       00 XgmiDpmSpare                              : 0
+ 0x07d9 (2009) B       00 XgmiDpmSpare                              : 0
+ 0x07da (2010) I 00000000 DebugOverrides                            : 0
+ 0x07de (2014) f 00000000 a                                         : 0
+ 0x07e2 (2018) f 00000000 b                                         : 0
+ 0x07e6 (2022) f 00000000 c                                         : 0
+ 0x07ea (2026) f 00000000 a                                         : 0
+ 0x07ee (2030) f 00000000 b                                         : 0
+ 0x07f2 (2034) f 00000000 c                                         : 0
+ 0x07f6 (2038) f 00000000 a                                         : 0
+ 0x07fa (2042) f 00000000 b                                         : 0
+ 0x07fe (2046) f 00000000 c                                         : 0
+ 0x0802 (2050) f 00000000 a                                         : 0
+ 0x0806 (2054) f 00000000 b                                         : 0
+ 0x080a (2058) f 00000000 c                                         : 0
+ 0x080e (2062) B       00 CustomerVariant                           : 0
+ 0x080f (2063) B       01 VcBtcEnabled                              : 1
+ 0x0810 (2064) H     3b0b VcBtcVminT0                               : 2875
+ 0x0812 (2066) H     4501 VcBtcFixedVminAgingOffset                 : 325
+ 0x0814 (2068) H     0000 VcBtcVmin2PsmDegrationGb                  : 0
+ 0x0816 (2070) f 3480373b VcBtcPsmA                                 : 0.0028
+ 0x081a (2074) f 9fabcd3e VcBtcPsmB                                 : 0.4017
+ 0x081e (2078) f ed0d3e3c VcBtcVminA                                : 0.0116
+ 0x0822 (2082) f 7593f83e VcBtcVminB                                : 0.4855
+ 0x0826 (2086) H     0000 LedGpio                                   : 0
+ 0x0828 (2088) H     0100 GfxPowerStagesGpio                        : 1
+ 0x082a (2090) I 00000000 SkuReserved                               : 0
+ 0x082e (2094) I 00000000 SkuReserved                               : 0
+ 0x0832 (2098) I 00000000 SkuReserved                               : 0
+ 0x0836 (2102) I 00000000 SkuReserved                               : 0
+ 0x083a (2106) I 00000000 SkuReserved                               : 0
+ 0x083e (2110) I 00000000 SkuReserved                               : 0
+ 0x0842 (2114) I 00000000 SkuReserved                               : 0
+ 0x0846 (2118) I 00000000 SkuReserved                               : 0
+ 0x084a (2122) I 00000000 GamingClk                                 : 0
+ 0x084e (2126) I 00000000 GamingClk                                 : 0
+ 0x0852 (2130) I 00000000 GamingClk                                 : 0
+ 0x0856 (2134) I 00000000 GamingClk                                 : 0
+ 0x085a (2138) I 00000000 GamingClk                                 : 0
+ 0x085e (2142) I 00000000 GamingClk                                 : 0
+ 0x0862 (2146) B       00 Enabled                                   : 0
+ 0x0863 (2147) B       00 Speed                                     : 0
+ 0x0864 (2148) B       00 SlaveAddress                              : 0
+ 0x0865 (2149) B       00 ControllerPort                            : 0
+ 0x0866 (2150) B       00 ControllerName                            : 0
+ 0x0867 (2151) B       00 ThermalThrotter                           : 0
+ 0x0868 (2152) B       00 I2cProtocol                               : 0
+ 0x0869 (2153) B       00 PaddingConfig                             : 0
+ 0x086a (2154) B       00 Enabled                                   : 0
+ 0x086b (2155) B       00 Speed                                     : 0
+ 0x086c (2156) B       00 SlaveAddress                              : 0
+ 0x086d (2157) B       00 ControllerPort                            : 0
+ 0x086e (2158) B       00 ControllerName                            : 0
+ 0x086f (2159) B       00 ThermalThrotter                           : 0
+ 0x0870 (2160) B       00 I2cProtocol                               : 0
+ 0x0871 (2161) B       00 PaddingConfig                             : 0
+ 0x0872 (2162) B       00 Enabled                                   : 0
+ 0x0873 (2163) B       00 Speed                                     : 0
+ 0x0874 (2164) B       00 SlaveAddress                              : 0
+ 0x0875 (2165) B       00 ControllerPort                            : 0
+ 0x0876 (2166) B       00 ControllerName                            : 0
+ 0x0877 (2167) B       00 ThermalThrotter                           : 0
+ 0x0878 (2168) B       00 I2cProtocol                               : 0
+ 0x0879 (2169) B       00 PaddingConfig                             : 0
+ 0x087a (2170) B       00 Enabled                                   : 0
+ 0x087b (2171) B       00 Speed                                     : 0
+ 0x087c (2172) B       00 SlaveAddress                              : 0
+ 0x087d (2173) B       00 ControllerPort                            : 0
+ 0x087e (2174) B       00 ControllerName                            : 0
+ 0x087f (2175) B       00 ThermalThrotter                           : 0
+ 0x0880 (2176) B       00 I2cProtocol                               : 0
+ 0x0881 (2177) B       00 PaddingConfig                             : 0
+ 0x0882 (2178) B       00 Enabled                                   : 0
+ 0x0883 (2179) B       00 Speed                                     : 0
+ 0x0884 (2180) B       00 SlaveAddress                              : 0
+ 0x0885 (2181) B       00 ControllerPort                            : 0
+ 0x0886 (2182) B       00 ControllerName                            : 0
+ 0x0887 (2183) B       00 ThermalThrotter                           : 0
+ 0x0888 (2184) B       00 I2cProtocol                               : 0
+ 0x0889 (2185) B       00 PaddingConfig                             : 0
+ 0x088a (2186) B       00 Enabled                                   : 0
+ 0x088b (2187) B       00 Speed                                     : 0
+ 0x088c (2188) B       00 SlaveAddress                              : 0
+ 0x088d (2189) B       00 ControllerPort                            : 0
+ 0x088e (2190) B       00 ControllerName                            : 0
+ 0x088f (2191) B       00 ThermalThrotter                           : 0
+ 0x0890 (2192) B       00 I2cProtocol                               : 0
+ 0x0891 (2193) B       00 PaddingConfig                             : 0
+ 0x0892 (2194) B       00 Enabled                                   : 0
+ 0x0893 (2195) B       00 Speed                                     : 0
+ 0x0894 (2196) B       00 SlaveAddress                              : 0
+ 0x0895 (2197) B       00 ControllerPort                            : 0
+ 0x0896 (2198) B       00 ControllerName                            : 0
+ 0x0897 (2199) B       00 ThermalThrotter                           : 0
+ 0x0898 (2200) B       00 I2cProtocol                               : 0
+ 0x0899 (2201) B       00 PaddingConfig                             : 0
+ 0x089a (2202) B       00 Enabled                                   : 0
+ 0x089b (2203) B       00 Speed                                     : 0
+ 0x089c (2204) B       00 SlaveAddress                              : 0
+ 0x089d (2205) B       00 ControllerPort                            : 0
+ 0x089e (2206) B       00 ControllerName                            : 0
+ 0x089f (2207) B       00 ThermalThrotter                           : 0
+ 0x08a0 (2208) B       00 I2cProtocol                               : 0
+ 0x08a1 (2209) B       00 PaddingConfig                             : 0
+ 0x08a2 (2210) B       00 Enabled                                   : 0
+ 0x08a3 (2211) B       00 Speed                                     : 0
+ 0x08a4 (2212) B       00 SlaveAddress                              : 0
+ 0x08a5 (2213) B       00 ControllerPort                            : 0
+ 0x08a6 (2214) B       00 ControllerName                            : 0
+ 0x08a7 (2215) B       00 ThermalThrotter                           : 0
+ 0x08a8 (2216) B       00 I2cProtocol                               : 0
+ 0x08a9 (2217) B       00 PaddingConfig                             : 0
+ 0x08aa (2218) B       00 Enabled                                   : 0
+ 0x08ab (2219) B       00 Speed                                     : 0
+ 0x08ac (2220) B       00 SlaveAddress                              : 0
+ 0x08ad (2221) B       00 ControllerPort                            : 0
+ 0x08ae (2222) B       00 ControllerName                            : 0
+ 0x08af (2223) B       00 ThermalThrotter                           : 0
+ 0x08b0 (2224) B       00 I2cProtocol                               : 0
+ 0x08b1 (2225) B       00 PaddingConfig                             : 0
+ 0x08b2 (2226) B       00 Enabled                                   : 0
+ 0x08b3 (2227) B       00 Speed                                     : 0
+ 0x08b4 (2228) B       00 SlaveAddress                              : 0
+ 0x08b5 (2229) B       00 ControllerPort                            : 0
+ 0x08b6 (2230) B       00 ControllerName                            : 0
+ 0x08b7 (2231) B       00 ThermalThrotter                           : 0
+ 0x08b8 (2232) B       00 I2cProtocol                               : 0
+ 0x08b9 (2233) B       00 PaddingConfig                             : 0
+ 0x08ba (2234) B       00 Enabled                                   : 0
+ 0x08bb (2235) B       00 Speed                                     : 0
+ 0x08bc (2236) B       00 SlaveAddress                              : 0
+ 0x08bd (2237) B       00 ControllerPort                            : 0
+ 0x08be (2238) B       00 ControllerName                            : 0
+ 0x08bf (2239) B       00 ThermalThrotter                           : 0
+ 0x08c0 (2240) B       00 I2cProtocol                               : 0
+ 0x08c1 (2241) B       00 PaddingConfig                             : 0
+ 0x08c2 (2242) B       00 Enabled                                   : 0
+ 0x08c3 (2243) B       00 Speed                                     : 0
+ 0x08c4 (2244) B       00 SlaveAddress                              : 0
+ 0x08c5 (2245) B       00 ControllerPort                            : 0
+ 0x08c6 (2246) B       00 ControllerName                            : 0
+ 0x08c7 (2247) B       00 ThermalThrotter                           : 0
+ 0x08c8 (2248) B       00 I2cProtocol                               : 0
+ 0x08c9 (2249) B       00 PaddingConfig                             : 0
+ 0x08ca (2250) B       00 Enabled                                   : 0
+ 0x08cb (2251) B       00 Speed                                     : 0
+ 0x08cc (2252) B       00 SlaveAddress                              : 0
+ 0x08cd (2253) B       00 ControllerPort                            : 0
+ 0x08ce (2254) B       00 ControllerName                            : 0
+ 0x08cf (2255) B       00 ThermalThrotter                           : 0
+ 0x08d0 (2256) B       00 I2cProtocol                               : 0
+ 0x08d1 (2257) B       00 PaddingConfig                             : 0
+ 0x08d2 (2258) B       00 Enabled                                   : 0
+ 0x08d3 (2259) B       00 Speed                                     : 0
+ 0x08d4 (2260) B       00 SlaveAddress                              : 0
+ 0x08d5 (2261) B       00 ControllerPort                            : 0
+ 0x08d6 (2262) B       00 ControllerName                            : 0
+ 0x08d7 (2263) B       00 ThermalThrotter                           : 0
+ 0x08d8 (2264) B       00 I2cProtocol                               : 0
+ 0x08d9 (2265) B       00 PaddingConfig                             : 0
+ 0x08da (2266) B       00 Enabled                                   : 0
+ 0x08db (2267) B       00 Speed                                     : 0
+ 0x08dc (2268) B       00 SlaveAddress                              : 0
+ 0x08dd (2269) B       00 ControllerPort                            : 0
+ 0x08de (2270) B       00 ControllerName                            : 0
+ 0x08df (2271) B       00 ThermalThrotter                           : 0
+ 0x08e0 (2272) B       00 I2cProtocol                               : 0
+ 0x08e1 (2273) B       00 PaddingConfig                             : 0
+ 0x08e2 (2274) B       00 GpioScl                                   : 0
+ 0x08e3 (2275) B       00 GpioSda                                   : 0
+ 0x08e4 (2276) B       00 FchUsbPdSlaveAddr                         : 0
+ 0x08e5 (2277) B       00 I2cSpare                                  : 0
+ 0x08e6 (2278) B       00 VddGfxVrMapping                           : 0
+ 0x08e7 (2279) B       00 VddSocVrMapping                           : 0
+ 0x08e8 (2280) B       00 VddMem0VrMapping                          : 0
+ 0x08e9 (2281) B       00 VddMem1VrMapping                          : 0
+ 0x08ea (2282) B       00 GfxUlvPhaseSheddingMask                   : 0
+ 0x08eb (2283) B       00 SocUlvPhaseSheddingMask                   : 0
+ 0x08ec (2284) B       00 VddciUlvPhaseSheddingMask                 : 0
+ 0x08ed (2285) B       00 MvddUlvPhaseSheddingMask                  : 0
+ 0x08ee (2286) H     0000 GfxMaxCurrent                             : 0
+ 0x08f0 (2288) b       00 GfxOffset                                 : 0
+ 0x08f1 (2289) B       00 Padding_TelemetryGfx                      : 0
+ 0x08f2 (2290) H     0000 SocMaxCurrent                             : 0
+ 0x08f4 (2292) b       00 SocOffset                                 : 0
+ 0x08f5 (2293) B       00 Padding_TelemetrySoc                      : 0
+ 0x08f6 (2294) H     0000 Mem0MaxCurrent                            : 0
+ 0x08f8 (2296) b       00 Mem0Offset                                : 0
+ 0x08f9 (2297) B       00 Padding_TelemetryMem0                     : 0
+ 0x08fa (2298) H     0000 Mem1MaxCurrent                            : 0
+ 0x08fc (2300) b       00 Mem1Offset                                : 0
+ 0x08fd (2301) B       00 Padding_TelemetryMem1                     : 0
+ 0x08fe (2302) I 00000000 MvddRatio                                 : 0
+ 0x0902 (2306) B       00 AcDcGpio                                  : 0
+ 0x0903 (2307) B       00 AcDcPolarity                              : 0
+ 0x0904 (2308) B       00 VR0HotGpio                                : 0
+ 0x0905 (2309) B       00 VR0HotPolarity                            : 0
+ 0x0906 (2310) B       00 VR1HotGpio                                : 0
+ 0x0907 (2311) B       00 VR1HotPolarity                            : 0
+ 0x0908 (2312) B       00 GthrGpio                                  : 0
+ 0x0909 (2313) B       00 GthrPolarity                              : 0
+ 0x090a (2314) B       00 LedPin0                                   : 0
+ 0x090b (2315) B       00 LedPin1                                   : 0
+ 0x090c (2316) B       00 LedPin2                                   : 0
+ 0x090d (2317) B       00 LedEnableMask                             : 0
+ 0x090e (2318) B       00 LedPcie                                   : 0
+ 0x090f (2319) B       00 LedError                                  : 0
+ 0x0910 (2320) B       00 LedSpare1                                 : 0
+ 0x0911 (2321) B       01 LedSpare1                                 : 1
+ 0x0912 (2322) B       00 PllGfxclkSpreadEnabled                    : 0
+ 0x0913 (2323) B       00 PllGfxclkSpreadPercent                    : 0
+ 0x0914 (2324) H     0000 PllGfxclkSpreadFreq                       : 0
+ 0x0916 (2326) B       00 DfllGfxclkSpreadEnabled                   : 0
+ 0x0917 (2327) B       00 DfllGfxclkSpreadPercent                   : 0
+ 0x0918 (2328) H     0000 DfllGfxclkSpreadFreq                      : 0
+ 0x091a (2330) H     0000 UclkSpreadPadding                         : 0
+ 0x091c (2332) H     0000 UclkSpreadFreq                            : 0
+ 0x091e (2334) B       00 FclkSpreadEnabled                         : 0
+ 0x091f (2335) B       00 FclkSpreadPercent                         : 0
+ 0x0920 (2336) H     0000 FclkSpreadFreq                            : 0
+ 0x0922 (2338) I 00000000 MemoryChannelEnabled                      : 0
+ 0x0926 (2342) B       00 DramBitWidth                              : 0
+ 0x0927 (2343) B       00 PaddingMem1                               : 0
+ 0x0928 (2344) B       00 PaddingMem1                               : 0
+ 0x0929 (2345) B       00 PaddingMem1                               : 0
+ 0x092a (2346) H     0000 TotalBoardPower                           : 0
+ 0x092c (2348) H     0000 BoardPowerPadding                         : 0
+ 0x092e (2350) B       00 XgmiLinkSpeed                             : 0
+ 0x092f (2351) B       00 XgmiLinkSpeed                             : 0
+ 0x0930 (2352) B       00 XgmiLinkSpeed                             : 0
+ 0x0931 (2353) B       00 XgmiLinkSpeed                             : 0
+ 0x0932 (2354) B       00 XgmiLinkWidth                             : 0
+ 0x0933 (2355) B       00 XgmiLinkWidth                             : 0
+ 0x0934 (2356) B       00 XgmiLinkWidth                             : 0
+ 0x0935 (2357) B       00 XgmiLinkWidth                             : 0
+ 0x0936 (2358) H     0000 XgmiFclkFreq                              : 0
+ 0x0938 (2360) H     0000 XgmiFclkFreq                              : 0
+ 0x093a (2362) H     0000 XgmiFclkFreq                              : 0
+ 0x093c (2364) H     0000 XgmiFclkFreq                              : 0
+ 0x093e (2366) H     0000 XgmiSocVoltage                            : 0
+ 0x0940 (2368) H     0000 XgmiSocVoltage                            : 0
+ 0x0942 (2370) H     0000 XgmiSocVoltage                            : 0
+ 0x0944 (2372) H     0000 XgmiSocVoltage                            : 0
+ 0x0946 (2374) B       00 HsrEnabled                                : 0
+ 0x0947 (2375) B       00 VddqOffEnabled                            : 0
+ 0x0948 (2376) B       00 PaddingUmcFlags                           : 0
+ 0x0949 (2377) B       00 PaddingUmcFlags                           : 0
+ 0x094a (2378) B       00 UclkSpreadPercent                         : 0
+ 0x094b (2379) B       00 UclkSpreadPercent                         : 0
+ 0x094c (2380) B       00 UclkSpreadPercent                         : 0
+ 0x094d (2381) B       00 UclkSpreadPercent                         : 0
+ 0x094e (2382) B       00 UclkSpreadPercent                         : 0
+ 0x094f (2383) B       00 UclkSpreadPercent                         : 0
+ 0x0950 (2384) B       00 UclkSpreadPercent                         : 0
+ 0x0951 (2385) B       00 UclkSpreadPercent                         : 0
+ 0x0952 (2386) B       00 UclkSpreadPercent                         : 0
+ 0x0953 (2387) B       00 UclkSpreadPercent                         : 0
+ 0x0954 (2388) B       00 UclkSpreadPercent                         : 0
+ 0x0955 (2389) B       00 UclkSpreadPercent                         : 0
+ 0x0956 (2390) B       00 UclkSpreadPercent                         : 0
+ 0x0957 (2391) B       00 UclkSpreadPercent                         : 0
+ 0x0958 (2392) B       00 UclkSpreadPercent                         : 0
+ 0x0959 (2393) B       00 UclkSpreadPercent                         : 0
+ 0x095a (2394) I 00000000 BoardReserved                             : 0
+ 0x095e (2398) I 00000000 BoardReserved                             : 0
+ 0x0962 (2402) I 00000000 BoardReserved                             : 0
+ 0x0966 (2406) I 00000000 BoardReserved                             : 0
+ 0x096a (2410) I 00000000 BoardReserved                             : 0
+ 0x096e (2414) I 00000000 BoardReserved                             : 0
+ 0x0972 (2418) I 00000000 BoardReserved                             : 0
+ 0x0976 (2422) I 00000000 BoardReserved                             : 0
+ 0x097a (2426) I 00000000 BoardReserved                             : 0
+ 0x097e (2430) I 00000000 BoardReserved                             : 0
+ 0x0982 (2434) I 00000000 BoardReserved                             : 0
+ 0x0986 (2438) I 00000000 MmHubPadding                              : 0
+ 0x098a (2442) I 00000000 MmHubPadding                              : 0
+ 0x098e (2446) I 00000000 MmHubPadding                              : 0
+ 0x0992 (2450) I 00000000 MmHubPadding                              : 0
+ 0x0996 (2454) I 00000000 MmHubPadding                              : 0
+ 0x099a (2458) I 00000000 MmHubPadding                              : 0
+ 0x099e (2462) I 00000000 MmHubPadding                              : 0
+ 0x09a2 (2466) I 00001e06 MmHubPadding                              : 102629376
```

### Comparing `upp-0.2.0/test/AMD.RX7900XTX.24576.230323.rom.dump` & `upp-0.2.1/test/AMD.RX7900XTX.24576.230323.rom.dump`

 * *Files 2% similar despite different names*

```diff
@@ -67,30 +67,30 @@
   reserve:
     reserve 0: 0
     reserve 1: 0
     reserve 2: 0
   feature_count: 22
   setting_count: 41
   cap:
-    cap 0: 1
-    cap 1: 1
-    cap 2: 1
-    cap 3: 1
-    cap 4: 1
-    cap 5: 1
-    cap 6: 1
-    cap 7: 1
-    cap 8: 1
-    cap 9: 1
-    cap 10: 1
-    cap 11: 1
-    cap 12: 1
-    cap 13: 0
-    cap 14: 1
-    cap 15: 0
+    cap 0: 1 (GFXCLK_LIMITS)
+    cap 1: 1 (UCLK_LIMITS)
+    cap 2: 1 (POWER_LIMIT)
+    cap 3: 1 (FAN_ACOUSTIC_LIMIT)
+    cap 4: 1 (FAN_SPEED_MIN)
+    cap 5: 1 (TEMPERATURE_FAN)
+    cap 6: 1 (TEMPERATURE_SYSTEM)
+    cap 7: 1 (MEMORY_TIMING_TUNE)
+    cap 8: 1 (FAN_ZERO_RPM_CONTROL)
+    cap 9: 1 (AUTO_UV_ENGINE)
+    cap 10: 1 (AUTO_OC_ENGINE)
+    cap 11: 1 (AUTO_OC_MEMORY)
+    cap 12: 1 (FAN_CURVE)
+    cap 13: 0 (AUTO_FAN_ACOUSTIC_LIMIT)
+    cap 14: 1 (POWER_MODE)
+    cap 15: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET)
     cap 16: 0
     cap 17: 1
     cap 18: 0
     cap 19: 0
     cap 20: 0
     cap 21: 0
     cap 22: 0
@@ -100,46 +100,46 @@
     cap 26: 0
     cap 27: 0
     cap 28: 0
     cap 29: 0
     cap 30: 0
     cap 31: 0
   max:
-    max 0: 5000
-    max 1: 5000
-    max 2: 1500
-    max 3: 1500
-    max 4: 15
-    max 5: 3300
-    max 6: 3300
-    max 7: 105
-    max 8: 110
-    max 9: 1
-    max 10: 1
-    max 11: 1
-    max 12: 1
-    max 13: 1
-    max 14: 100
-    max 15: 100
-    max 16: 100
-    max 17: 100
-    max 18: 100
-    max 19: 100
-    max 20: 100
-    max 21: 100
-    max 22: 100
-    max 23: 100
-    max 24: 0
-    max 25: 1
-    max 26: 0
-    max 27: 0
-    max 28: 0
-    max 29: 0
-    max 30: 0
-    max 31: 0
+    max 0: 5000 (GFXCLKFMAX)
+    max 1: 5000 (GFXCLKFMIN)
+    max 2: 1500 (UCLKFMIN)
+    max 3: 1500 (UCLKFMAX)
+    max 4: 15 (POWERPERCENTAGE)
+    max 5: 3300 (FANRPMMIN)
+    max 6: 3300 (FANRPMACOUSTICLIMIT)
+    max 7: 105 (FANTARGETTEMPERATURE)
+    max 8: 110 (OPERATINGTEMPMAX)
+    max 9: 1 (ACTIMING)
+    max 10: 1 (FAN_ZERO_RPM_CONTROL)
+    max 11: 1 (AUTOUVENGINE)
+    max 12: 1 (AUTOOCENGINE)
+    max 13: 1 (AUTOOCMEMORY)
+    max 14: 100 (FAN_CURVE_TEMPERATURE_1)
+    max 15: 100 (FAN_CURVE_SPEED_1)
+    max 16: 100 (FAN_CURVE_TEMPERATURE_2)
+    max 17: 100 (FAN_CURVE_SPEED_2)
+    max 18: 100 (FAN_CURVE_TEMPERATURE_3)
+    max 19: 100 (FAN_CURVE_SPEED_3)
+    max 20: 100 (FAN_CURVE_TEMPERATURE_4)
+    max 21: 100 (FAN_CURVE_SPEED_4)
+    max 22: 100 (FAN_CURVE_TEMPERATURE_5)
+    max 23: 100 (FAN_CURVE_SPEED_5)
+    max 24: 0 (AUTO_FAN_ACOUSTIC_LIMIT)
+    max 25: 1 (POWER_MODE)
+    max 26: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_1)
+    max 27: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_2)
+    max 28: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_3)
+    max 29: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_4)
+    max 30: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_5)
+    max 31: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_6)
     max 32: 0
     max 33: 0
     max 34: 0
     max 35: 0
     max 36: 0
     max 37: 0
     max 38: 0
@@ -165,46 +165,46 @@
     max 58: 0
     max 59: 0
     max 60: 0
     max 61: 0
     max 62: 0
     max 63: 0
   min:
-    min 0: 500
-    min 1: 500
-    min 2: 97
-    min 3: 97
-    min 4: 10
-    min 5: 500
-    min 6: 500
-    min 7: 25
-    min 8: 50
-    min 9: 0
-    min 10: 0
-    min 11: 0
-    min 12: 0
-    min 13: 0
-    min 14: 25
-    min 15: 15
-    min 16: 25
-    min 17: 15
-    min 18: 25
-    min 19: 15
-    min 20: 25
-    min 21: 15
-    min 22: 25
-    min 23: 15
-    min 24: 0
-    min 25: 0
-    min 26: 0
-    min 27: 0
-    min 28: 0
-    min 29: 0
-    min 30: 0
-    min 31: 0
+    min 0: 500 (GFXCLKFMAX)
+    min 1: 500 (GFXCLKFMIN)
+    min 2: 97 (UCLKFMIN)
+    min 3: 97 (UCLKFMAX)
+    min 4: 10 (POWERPERCENTAGE)
+    min 5: 500 (FANRPMMIN)
+    min 6: 500 (FANRPMACOUSTICLIMIT)
+    min 7: 25 (FANTARGETTEMPERATURE)
+    min 8: 50 (OPERATINGTEMPMAX)
+    min 9: 0 (ACTIMING)
+    min 10: 0 (FAN_ZERO_RPM_CONTROL)
+    min 11: 0 (AUTOUVENGINE)
+    min 12: 0 (AUTOOCENGINE)
+    min 13: 0 (AUTOOCMEMORY)
+    min 14: 25 (FAN_CURVE_TEMPERATURE_1)
+    min 15: 15 (FAN_CURVE_SPEED_1)
+    min 16: 25 (FAN_CURVE_TEMPERATURE_2)
+    min 17: 15 (FAN_CURVE_SPEED_2)
+    min 18: 25 (FAN_CURVE_TEMPERATURE_3)
+    min 19: 15 (FAN_CURVE_SPEED_3)
+    min 20: 25 (FAN_CURVE_TEMPERATURE_4)
+    min 21: 15 (FAN_CURVE_SPEED_4)
+    min 22: 25 (FAN_CURVE_TEMPERATURE_5)
+    min 23: 15 (FAN_CURVE_SPEED_5)
+    min 24: 0 (AUTO_FAN_ACOUSTIC_LIMIT)
+    min 25: 0 (POWER_MODE)
+    min 26: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_1)
+    min 27: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_2)
+    min 28: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_3)
+    min 29: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_4)
+    min 30: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_5)
+    min 31: 0 (PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_6)
     min 32: 0
     min 33: 10
     min 34: 0
     min 35: 0
     min 36: 0
     min 37: 0
     min 38: 0
```

### Comparing `upp-0.2.0/test/AMD.RX7900XTX.24576.230323.rom.rawdump` & `upp-0.2.1/test/AMD.RX7900XTX.24576.230323.rom.rawdump`

 * *Files 5% similar despite different names*

```diff
@@ -1,1749 +1,1749 @@
 PowerPlay table rev 20.0 size 5424 bytes
- Offset (dec.) t Raw val. Variable name                   Decoded value
------------------------------------------------------------------------
- 0x0000 (0000) H     3015 structuresize                   : 5424
- 0x0002 (0002) B       14 format_revision                 : 20
- 0x0003 (0003) B       00 content_revision                : 0
- 0x0004 (0004) B       03 table_revision                  : 3
- 0x0005 (0005) B       00 padding                         : 0
- 0x0006 (0006) H     4003 table_size                      : 832
- 0x0008 (0008) I 3c0f0000 golden_pp_id                    : 3900
- 0x000c (0012) I 11540000 golden_revision                 : 21521
- 0x0010 (0016) H     8500 format_id                       : 133
- 0x0012 (0018) I 08000000 platform_caps                   : 8
- 0x0016 (0022) B       1d thermal_controller_type         : 29
- 0x0017 (0023) H     0000 small_power_limit1              : 0
- 0x0019 (0025) H     0000 small_power_limit2              : 0
- 0x001b (0027) H     0000 boost_power_limit               : 0
- 0x001d (0029) H     7600 software_shutdown_temp          : 118
- 0x001f (0031) I 00000000 reserve                         : 0
- 0x0023 (0035) I 00000000 reserve                         : 0
- 0x0027 (0039) I 00000000 reserve                         : 0
- 0x002b (0043) I 00000000 reserve                         : 0
- 0x002f (0047) I 00000000 reserve                         : 0
- 0x0033 (0051) I 00000000 reserve                         : 0
- 0x0037 (0055) I 00000000 reserve                         : 0
- 0x003b (0059) I 00000000 reserve                         : 0
- 0x003f (0063) I 00000000 reserve                         : 0
- 0x0043 (0067) I 00000000 reserve                         : 0
- 0x0047 (0071) I 00000000 reserve                         : 0
- 0x004b (0075) I 00000000 reserve                         : 0
- 0x004f (0079) I 00000000 reserve                         : 0
- 0x0053 (0083) I 00000000 reserve                         : 0
- 0x0057 (0087) I 00000000 reserve                         : 0
- 0x005b (0091) I 00000000 reserve                         : 0
- 0x005f (0095) I 00000000 reserve                         : 0
- 0x0063 (0099) I 00000000 reserve                         : 0
- 0x0067 (0103) I 00000000 reserve                         : 0
- 0x006b (0107) I 00000000 reserve                         : 0
- 0x006f (0111) I 00000000 reserve                         : 0
- 0x0073 (0115) I 00000000 reserve                         : 0
- 0x0077 (0119) I 00000000 reserve                         : 0
- 0x007b (0123) I 00000000 reserve                         : 0
- 0x007f (0127) I 00000000 reserve                         : 0
- 0x0083 (0131) I 00000000 reserve                         : 0
- 0x0087 (0135) I 00000000 reserve                         : 0
- 0x008b (0139) I 00000000 reserve                         : 0
- 0x008f (0143) I 00000000 reserve                         : 0
- 0x0093 (0147) I 00000000 reserve                         : 0
- 0x0097 (0151) I 00000000 reserve                         : 0
- 0x009b (0155) I 00000000 reserve                         : 0
- 0x009f (0159) I 00000000 reserve                         : 0
- 0x00a3 (0163) I 00000000 reserve                         : 0
- 0x00a7 (0167) I 00000000 reserve                         : 0
- 0x00ab (0171) I 00000000 reserve                         : 0
- 0x00af (0175) I 00000000 reserve                         : 0
- 0x00b3 (0179) I 00000000 reserve                         : 0
- 0x00b7 (0183) I 00000000 reserve                         : 0
- 0x00bb (0187) I 00000000 reserve                         : 0
- 0x00bf (0191) I 00000000 reserve                         : 0
- 0x00c3 (0195) I 00000000 reserve                         : 0
- 0x00c7 (0199) I 00000000 reserve                         : 0
- 0x00cb (0203) I 00000000 reserve                         : 0
- 0x00cf (0207) I 00000000 reserve                         : 0
- 0x00d3 (0211) B       83 revision                        : 131
- 0x00d4 (0212) B       00 reserve                         : 0
- 0x00d5 (0213) B       00 reserve                         : 0
- 0x00d6 (0214) B       00 reserve                         : 0
- 0x00d7 (0215) I 16000000 feature_count                   : 22
- 0x00db (0219) I 29000000 setting_count                   : 41
- 0x00df (0223) B       01 cap                             : 1
- 0x00e0 (0224) B       01 cap                             : 1
- 0x00e1 (0225) B       01 cap                             : 1
- 0x00e2 (0226) B       01 cap                             : 1
- 0x00e3 (0227) B       01 cap                             : 1
- 0x00e4 (0228) B       01 cap                             : 1
- 0x00e5 (0229) B       01 cap                             : 1
- 0x00e6 (0230) B       01 cap                             : 1
- 0x00e7 (0231) B       01 cap                             : 1
- 0x00e8 (0232) B       01 cap                             : 1
- 0x00e9 (0233) B       01 cap                             : 1
- 0x00ea (0234) B       01 cap                             : 1
- 0x00eb (0235) B       01 cap                             : 1
- 0x00ec (0236) B       00 cap                             : 0
- 0x00ed (0237) B       01 cap                             : 1
- 0x00ee (0238) B       00 cap                             : 0
- 0x00ef (0239) B       00 cap                             : 0
- 0x00f0 (0240) B       01 cap                             : 1
- 0x00f1 (0241) B       00 cap                             : 0
- 0x00f2 (0242) B       00 cap                             : 0
- 0x00f3 (0243) B       00 cap                             : 0
- 0x00f4 (0244) B       00 cap                             : 0
- 0x00f5 (0245) B       00 cap                             : 0
- 0x00f6 (0246) B       00 cap                             : 0
- 0x00f7 (0247) B       00 cap                             : 0
- 0x00f8 (0248) B       00 cap                             : 0
- 0x00f9 (0249) B       00 cap                             : 0
- 0x00fa (0250) B       00 cap                             : 0
- 0x00fb (0251) B       00 cap                             : 0
- 0x00fc (0252) B       00 cap                             : 0
- 0x00fd (0253) B       00 cap                             : 0
- 0x00fe (0254) B       00 cap                             : 0
- 0x00ff (0255) I 88130000 max                             : 5000
- 0x0103 (0259) I 88130000 max                             : 5000
- 0x0107 (0263) I dc050000 max                             : 1500
- 0x010b (0267) I dc050000 max                             : 1500
- 0x010f (0271) I 0f000000 max                             : 15
- 0x0113 (0275) I e40c0000 max                             : 3300
- 0x0117 (0279) I e40c0000 max                             : 3300
- 0x011b (0283) I 69000000 max                             : 105
- 0x011f (0287) I 6e000000 max                             : 110
- 0x0123 (0291) I 01000000 max                             : 1
- 0x0127 (0295) I 01000000 max                             : 1
- 0x012b (0299) I 01000000 max                             : 1
- 0x012f (0303) I 01000000 max                             : 1
- 0x0133 (0307) I 01000000 max                             : 1
- 0x0137 (0311) I 64000000 max                             : 100
- 0x013b (0315) I 64000000 max                             : 100
- 0x013f (0319) I 64000000 max                             : 100
- 0x0143 (0323) I 64000000 max                             : 100
- 0x0147 (0327) I 64000000 max                             : 100
- 0x014b (0331) I 64000000 max                             : 100
- 0x014f (0335) I 64000000 max                             : 100
- 0x0153 (0339) I 64000000 max                             : 100
- 0x0157 (0343) I 64000000 max                             : 100
- 0x015b (0347) I 64000000 max                             : 100
- 0x015f (0351) I 00000000 max                             : 0
- 0x0163 (0355) I 01000000 max                             : 1
- 0x0167 (0359) I 00000000 max                             : 0
- 0x016b (0363) I 00000000 max                             : 0
- 0x016f (0367) I 00000000 max                             : 0
- 0x0173 (0371) I 00000000 max                             : 0
- 0x0177 (0375) I 00000000 max                             : 0
- 0x017b (0379) I 00000000 max                             : 0
- 0x017f (0383) I 00000000 max                             : 0
- 0x0183 (0387) I 00000000 max                             : 0
- 0x0187 (0391) I 00000000 max                             : 0
- 0x018b (0395) I 00000000 max                             : 0
- 0x018f (0399) I 00000000 max                             : 0
- 0x0193 (0403) I 00000000 max                             : 0
- 0x0197 (0407) I 00000000 max                             : 0
- 0x019b (0411) I 00000000 max                             : 0
- 0x019f (0415) I 00000000 max                             : 0
- 0x01a3 (0419) I 00000000 max                             : 0
- 0x01a7 (0423) I 00000000 max                             : 0
- 0x01ab (0427) I 00000000 max                             : 0
- 0x01af (0431) I 00000000 max                             : 0
- 0x01b3 (0435) I 00000000 max                             : 0
- 0x01b7 (0439) I 00000000 max                             : 0
- 0x01bb (0443) I 00000000 max                             : 0
- 0x01bf (0447) I 00000000 max                             : 0
- 0x01c3 (0451) I 00000000 max                             : 0
- 0x01c7 (0455) I 00000000 max                             : 0
- 0x01cb (0459) I 00000000 max                             : 0
- 0x01cf (0463) I 00000000 max                             : 0
- 0x01d3 (0467) I 00000000 max                             : 0
- 0x01d7 (0471) I 00000000 max                             : 0
- 0x01db (0475) I 00000000 max                             : 0
- 0x01df (0479) I 00000000 max                             : 0
- 0x01e3 (0483) I 00000000 max                             : 0
- 0x01e7 (0487) I 00000000 max                             : 0
- 0x01eb (0491) I 00000000 max                             : 0
- 0x01ef (0495) I 00000000 max                             : 0
- 0x01f3 (0499) I 00000000 max                             : 0
- 0x01f7 (0503) I 00000000 max                             : 0
- 0x01fb (0507) I 00000000 max                             : 0
- 0x01ff (0511) I f4010000 min                             : 500
- 0x0203 (0515) I f4010000 min                             : 500
- 0x0207 (0519) I 61000000 min                             : 97
- 0x020b (0523) I 61000000 min                             : 97
- 0x020f (0527) I 0a000000 min                             : 10
- 0x0213 (0531) I f4010000 min                             : 500
- 0x0217 (0535) I f4010000 min                             : 500
- 0x021b (0539) I 19000000 min                             : 25
- 0x021f (0543) I 32000000 min                             : 50
- 0x0223 (0547) I 00000000 min                             : 0
- 0x0227 (0551) I 00000000 min                             : 0
- 0x022b (0555) I 00000000 min                             : 0
- 0x022f (0559) I 00000000 min                             : 0
- 0x0233 (0563) I 00000000 min                             : 0
- 0x0237 (0567) I 19000000 min                             : 25
- 0x023b (0571) I 0f000000 min                             : 15
- 0x023f (0575) I 19000000 min                             : 25
- 0x0243 (0579) I 0f000000 min                             : 15
- 0x0247 (0583) I 19000000 min                             : 25
- 0x024b (0587) I 0f000000 min                             : 15
- 0x024f (0591) I 19000000 min                             : 25
- 0x0253 (0595) I 0f000000 min                             : 15
- 0x0257 (0599) I 19000000 min                             : 25
- 0x025b (0603) I 0f000000 min                             : 15
- 0x025f (0607) I 00000000 min                             : 0
- 0x0263 (0611) I 00000000 min                             : 0
- 0x0267 (0615) I 00000000 min                             : 0
- 0x026b (0619) I 00000000 min                             : 0
- 0x026f (0623) I 00000000 min                             : 0
- 0x0273 (0627) I 00000000 min                             : 0
- 0x0277 (0631) I 00000000 min                             : 0
- 0x027b (0635) I 00000000 min                             : 0
- 0x027f (0639) I 00000000 min                             : 0
- 0x0283 (0643) I 0a000000 min                             : 10
- 0x0287 (0647) I 00000000 min                             : 0
- 0x028b (0651) I 00000000 min                             : 0
- 0x028f (0655) I 00000000 min                             : 0
- 0x0293 (0659) I 00000000 min                             : 0
- 0x0297 (0663) I 00000000 min                             : 0
- 0x029b (0667) I 00000000 min                             : 0
- 0x029f (0671) I 00000000 min                             : 0
- 0x02a3 (0675) I 00000000 min                             : 0
- 0x02a7 (0679) I 00000000 min                             : 0
- 0x02ab (0683) I 00000000 min                             : 0
- 0x02af (0687) I 00000000 min                             : 0
- 0x02b3 (0691) I 00000000 min                             : 0
- 0x02b7 (0695) I 00000000 min                             : 0
- 0x02bb (0699) I 00000000 min                             : 0
- 0x02bf (0703) I 00000000 min                             : 0
- 0x02c3 (0707) I 00000000 min                             : 0
- 0x02c7 (0711) I 00000000 min                             : 0
- 0x02cb (0715) I 00000000 min                             : 0
- 0x02cf (0719) I 00000000 min                             : 0
- 0x02d3 (0723) I 00000000 min                             : 0
- 0x02d7 (0727) I 00000000 min                             : 0
- 0x02db (0731) I 00000000 min                             : 0
- 0x02df (0735) I 00000000 min                             : 0
- 0x02e3 (0739) I 00000000 min                             : 0
- 0x02e7 (0743) I 00000000 min                             : 0
- 0x02eb (0747) I 00000000 min                             : 0
- 0x02ef (0751) I 00000000 min                             : 0
- 0x02f3 (0755) I 00000000 min                             : 0
- 0x02f7 (0759) I 00000000 min                             : 0
- 0x02fb (0763) I 00000000 min                             : 0
- 0x02ff (0767) h     0000 pm_setting                      : 0
- 0x0301 (0769) h     0000 pm_setting                      : 0
- 0x0303 (0771) h     0000 pm_setting                      : 0
- 0x0305 (0773) h     0a00 pm_setting                      : 10
- 0x0307 (0775) h     6900 pm_setting                      : 105
- 0x0309 (0777) h     5f00 pm_setting                      : 95
- 0x030b (0779) h     0000 pm_setting                      : 0
- 0x030d (0781) h     4b00 pm_setting                      : 75
- 0x030f (0783) h     0e06 pm_setting                      : 1550
- 0x0311 (0785) h     a406 pm_setting                      : 1700
- 0x0313 (0787) h     0000 pm_setting                      : 0
- 0x0315 (0789) h     b80b pm_setting                      : 3000
- 0x0317 (0791) h     0e06 pm_setting                      : 1550
- 0x0319 (0793) h     b80b pm_setting                      : 3000
- 0x031b (0795) h     0000 pm_setting                      : 0
- 0x031d (0797) h     b80b pm_setting                      : 3000
- 0x031f (0799) h     0000 pm_setting                      : 0
- 0x0321 (0801) h     0000 pm_setting                      : 0
- 0x0323 (0803) h     0000 pm_setting                      : 0
- 0x0325 (0805) h     0000 pm_setting                      : 0
- 0x0327 (0807) h     0000 pm_setting                      : 0
- 0x0329 (0809) h     0000 pm_setting                      : 0
- 0x032b (0811) h     0000 pm_setting                      : 0
- 0x032d (0813) h     0000 pm_setting                      : 0
- 0x032f (0815) h     0000 pm_setting                      : 0
- 0x0331 (0817) h     0000 pm_setting                      : 0
- 0x0333 (0819) h     0000 pm_setting                      : 0
- 0x0335 (0821) h     0000 pm_setting                      : 0
- 0x0337 (0823) h     0000 pm_setting                      : 0
- 0x0339 (0825) h     0000 pm_setting                      : 0
- 0x033b (0827) h     0000 pm_setting                      : 0
- 0x033d (0829) h     0000 pm_setting                      : 0
- 0x033f (0831) B       00 padding1                        : 0
- 0x0340 (0832) I 29000000 Version                         : 41
- 0x0344 (0836) I ffffff71 FeaturesToRun                   : 1912602623
- 0x0348 (0840) I b8eb0300 FeaturesToRun                   : 256952
- 0x034c (0844) B       01 TotalPowerConfig                : 1
- 0x034d (0845) B       00 CustomerVariant                 : 0
- 0x034e (0846) B       04 MemoryTemperatureTypeMask       : 4
- 0x034f (0847) B       00 SmartShiftVersion               : 0
- 0x0350 (0848) H     4701 SocketPowerLimitAc              : 327
- 0x0352 (0850) H     b004 SocketPowerLimitAc              : 1200
- 0x0354 (0852) H     0000 SocketPowerLimitAc              : 0
- 0x0356 (0854) H     0000 SocketPowerLimitAc              : 0
- 0x0358 (0856) H     0000 SocketPowerLimitDc              : 0
- 0x035a (0858) H     0000 SocketPowerLimitDc              : 0
- 0x035c (0860) H     0000 SocketPowerLimitDc              : 0
- 0x035e (0862) H     0000 SocketPowerLimitDc              : 0
- 0x0360 (0864) H     0000 SocketPowerLimitSmartShift2     : 0
- 0x0362 (0866) B       00 EnableLegacyPptLimit            : 0
- 0x0363 (0867) B       00 UseInputTelemetry               : 0
- 0x0364 (0868) B       00 SmartShiftMinReportedPptinDcs   : 0
- 0x0365 (0869) B       00 PaddingPpt                      : 0
- 0x0366 (0870) H     3b01 VrTdcLimit                      : 315
- 0x0368 (0872) H     5200 VrTdcLimit                      : 82
- 0x036a (0874) H     5600 VrTdcLimit                      : 86
- 0x036c (0876) H     c001 PlatformTdcLimit                : 448
- 0x036e (0878) H     5200 PlatformTdcLimit                : 82
- 0x0370 (0880) H     5600 PlatformTdcLimit                : 86
- 0x0372 (0882) H     6400 TemperatureLimit                : 100
- 0x0374 (0884) H     6e00 TemperatureLimit                : 110
- 0x0376 (0886) H     6e00 TemperatureLimit                : 110
- 0x0378 (0888) H     6e00 TemperatureLimit                : 110
- 0x037a (0890) H     6c00 TemperatureLimit                : 108
- 0x037c (0892) H     7300 TemperatureLimit                : 115
- 0x037e (0894) H     7300 TemperatureLimit                : 115
- 0x0380 (0896) H     7300 TemperatureLimit                : 115
- 0x0382 (0898) H     7300 TemperatureLimit                : 115
- 0x0384 (0900) H     7300 TemperatureLimit                : 115
- 0x0386 (0902) H     0000 TemperatureLimit                : 0
- 0x0388 (0904) H     0000 TemperatureLimit                : 0
- 0x038a (0906) H     0000 TemperatureLimit                : 0
- 0x038c (0908) H     7800 HwCtfTempLimit                  : 120
- 0x038e (0910) H     0000 PaddingInfra                    : 0
- 0x0390 (0912) I 00000000 FitControllerFailureRateLimit   : 0
- 0x0394 (0916) I 00000000 FitControllerGfxDutyCycle       : 0
- 0x0398 (0920) I 00000000 FitControllerSocDutyCycle       : 0
- 0x039c (0924) I 00000000 FitControllerSocOffset          : 0
- 0x03a0 (0928) I 00000000 GfxApccPlusResidencyLimit       : 0
- 0x03a4 (0932) I f2e30300 ThrottlerControlMask            : 254962
- 0x03a8 (0936) I ffff9b01 FwDStateMask                    : 27000831
- 0x03ac (0940) H     6400 UlvVoltageOffset                : 100
- 0x03ae (0942) H     6400 UlvVoltageOffset                : 100
- 0x03b0 (0944) H     6400 UlvVoltageOffsetU               : 100
- 0x03b2 (0946) H     6400 DeepUlvVoltageOffsetSoc         : 100
- 0x03b4 (0948) H     f811 DefaultMaxVoltage               : 4600
- 0x03b6 (0950) H     c012 DefaultMaxVoltage               : 4800
- 0x03b8 (0952) H     f811 BoostMaxVoltage                 : 4600
- 0x03ba (0954) H     c012 BoostMaxVoltage                 : 4800
- 0x03bc (0956) h     0500 VminTempHystersis               : 5
- 0x03be (0958) h     0500 VminTempHystersis               : 5
- 0x03c0 (0960) h     3700 VminTempThreshold               : 55
- 0x03c2 (0962) h     3700 VminTempThreshold               : 55
- 0x03c4 (0964) H     f00a Vmin_Hot_T0                     : 2800
- 0x03c6 (0966) H     f00a Vmin_Hot_T0                     : 2800
- 0x03c8 (0968) H     f00a Vmin_Cold_T0                    : 2800
- 0x03ca (0970) H     f00a Vmin_Cold_T0                    : 2800
- 0x03cc (0972) H     f00a Vmin_Hot_Eol                    : 2800
- 0x03ce (0974) H     f00a Vmin_Hot_Eol                    : 2800
- 0x03d0 (0976) H     f00a Vmin_Cold_Eol                   : 2800
- 0x03d2 (0978) H     f00a Vmin_Cold_Eol                   : 2800
- 0x03d4 (0980) H     0000 Vmin_Aging_Offset               : 0
- 0x03d6 (0982) H     0000 Vmin_Aging_Offset               : 0
- 0x03d8 (0984) H     0000 Spare_Vmin_Plat_Offset_Hot      : 0
- 0x03da (0986) H     0000 Spare_Vmin_Plat_Offset_Hot      : 0
- 0x03dc (0988) H     0000 Spare_Vmin_Plat_Offset_Cold     : 0
- 0x03de (0990) H     0000 Spare_Vmin_Plat_Offset_Cold     : 0
- 0x03e0 (0992) H     0000 VcBtcFixedVminAgingOffset       : 0
- 0x03e2 (0994) H     0000 VcBtcFixedVminAgingOffset       : 0
- 0x03e4 (0996) H     0000 VcBtcVmin2PsmDegrationGb        : 0
- 0x03e6 (0998) H     0000 VcBtcVmin2PsmDegrationGb        : 0
- 0x03e8 (1000) f 00000000 VcBtcPsmA                       : 0
- 0x03ec (1004) f 00000000 VcBtcPsmA                       : 0
- 0x03f0 (1008) f 00000000 VcBtcPsmB                       : 0
- 0x03f4 (1012) f 00000000 VcBtcPsmB                       : 0
- 0x03f8 (1016) f 00000000 VcBtcVminA                      : 0
- 0x03fc (1020) f 00000000 VcBtcVminA                      : 0
- 0x0400 (1024) f 00000000 VcBtcVminB                      : 0
- 0x0404 (1028) f 00000000 VcBtcVminB                      : 0
- 0x0408 (1032) B       01 PerPartVminEnabled              : 1
- 0x0409 (1033) B       00 PerPartVminEnabled              : 0
- 0x040a (1034) B       00 VcBtcEnabled                    : 0
- 0x040b (1035) B       00 VcBtcEnabled                    : 0
- 0x040c (1036) H     6400 SocketPowerLimitAcTau           : 100
- 0x040e (1038) H     0a00 SocketPowerLimitAcTau           : 10
- 0x0410 (1040) H     0000 SocketPowerLimitAcTau           : 0
- 0x0412 (1042) H     0000 SocketPowerLimitAcTau           : 0
- 0x0414 (1044) H     0000 SocketPowerLimitDcTau           : 0
- 0x0416 (1046) H     0000 SocketPowerLimitDcTau           : 0
- 0x0418 (1048) H     0000 SocketPowerLimitDcTau           : 0
- 0x041a (1050) H     0000 SocketPowerLimitDcTau           : 0
- 0x041c (1052) f 00000000 a                               : 0
- 0x0420 (1056) f 9a99993d b                               : 0.075
- 0x0424 (1060) f 0ad723bc c                               :-0.01
- 0x0428 (1064) I 00000000 SpareVmin                       : 0
- 0x042c (1068) I 00000000 SpareVmin                       : 0
- 0x0430 (1072) I 00000000 SpareVmin                       : 0
- 0x0434 (1076) I 00000000 SpareVmin                       : 0
- 0x0438 (1080) I 00000000 SpareVmin                       : 0
- 0x043c (1084) I 00000000 SpareVmin                       : 0
- 0x0440 (1088) I 00000200 SpareVmin                       : 131072
- 0x0444 (1092) I 00000000 SpareVmin                       : 0
- 0x0448 (1096) I 00000000 SpareVmin                       : 0
- 0x044c (1100) B       00 Padding                         : 0
- 0x044d (1101) B       00 SnapToDiscrete                  : 0
- 0x044e (1102) B       02 NumDiscreteLevels               : 2
- 0x044f (1103) B       03 CalculateFopt                   : 3
- 0x0450 (1104) f 0000803f m                               : 1
- 0x0454 (1108) f 00000000 b                               : 0
- 0x0458 (1112) I 00000000 Padding3                        : 0
- 0x045c (1116) I 00000000 Padding3                        : 0
- 0x0460 (1120) I 00000000 Padding3                        : 0
- 0x0464 (1124) H     0000 Padding4                        : 0
- 0x0466 (1126) H     0000 FoptimalDc                      : 0
- 0x0468 (1128) H     f401 FoptimalAc                      : 500
- 0x046a (1130) H     0000 Padding2                        : 0
- 0x046c (1132) B       00 Padding                         : 0
- 0x046d (1133) B       00 SnapToDiscrete                  : 0
- 0x046e (1134) B       02 NumDiscreteLevels               : 2
- 0x046f (1135) B       00 CalculateFopt                   : 0
- 0x0470 (1136) f 6210a83f m                               : 1.313
- 0x0474 (1140) f f0a7463e b                               : 0.194
- 0x0478 (1144) I 00000000 Padding3                        : 0
- 0x047c (1148) I 00000000 Padding3                        : 0
- 0x0480 (1152) I 00010400 Padding3                        : 262400
- 0x0484 (1156) H     0000 Padding4                        : 0
- 0x0486 (1158) H     0000 FoptimalDc                      : 0
- 0x0488 (1160) H     0000 FoptimalAc                      : 0
- 0x048a (1162) H     0000 Padding2                        : 0
- 0x048c (1164) B       00 Padding                         : 0
- 0x048d (1165) B       01 SnapToDiscrete                  : 1
- 0x048e (1166) B       04 NumDiscreteLevels               : 4
- 0x048f (1167) B       00 CalculateFopt                   : 0
- 0x0490 (1168) f aaf1c23f m                               : 1.523
- 0x0494 (1172) f a60ac63d b                               : 0.0967
- 0x0498 (1176) I 00000000 Padding3                        : 0
- 0x049c (1180) I 00000000 Padding3                        : 0
- 0x04a0 (1184) I 00000000 Padding3                        : 0
- 0x04a4 (1188) H     0000 Padding4                        : 0
- 0x04a6 (1190) H     0000 FoptimalDc                      : 0
- 0x04a8 (1192) H     0000 FoptimalAc                      : 0
- 0x04aa (1194) H     0000 Padding2                        : 0
- 0x04ac (1196) B       00 Padding                         : 0
- 0x04ad (1197) B       01 SnapToDiscrete                  : 1
- 0x04ae (1198) B       08 NumDiscreteLevels               : 8
- 0x04af (1199) B       03 CalculateFopt                   : 3
- 0x04b0 (1200) f 0000803f m                               : 1
- 0x04b4 (1204) f 00000000 b                               : 0
- 0x04b8 (1208) I 00000000 Padding3                        : 0
- 0x04bc (1212) I 00000000 Padding3                        : 0
- 0x04c0 (1216) I 00000000 Padding3                        : 0
- 0x04c4 (1220) H     0000 Padding4                        : 0
- 0x04c6 (1222) H     0000 FoptimalDc                      : 0
- 0x04c8 (1224) H     fc08 FoptimalAc                      : 2300
- 0x04ca (1226) H     0000 Padding2                        : 0
- 0x04cc (1228) B       00 Padding                         : 0
- 0x04cd (1229) B       00 SnapToDiscrete                  : 0
- 0x04ce (1230) B       02 NumDiscreteLevels               : 2
- 0x04cf (1231) B       00 CalculateFopt                   : 0
- 0x04d0 (1232) f 789c823f m                               : 1.0204
- 0x04d4 (1236) f a01aaf3e b                               : 0.342
- 0x04d8 (1240) I 00000000 Padding3                        : 0
- 0x04dc (1244) I 00000000 Padding3                        : 0
- 0x04e0 (1248) I 00000000 Padding3                        : 0
- 0x04e4 (1252) H     0000 Padding4                        : 0
- 0x04e6 (1254) H     0000 FoptimalDc                      : 0
- 0x04e8 (1256) H     0000 FoptimalAc                      : 0
- 0x04ea (1258) H     0000 Padding2                        : 0
- 0x04ec (1260) B       00 Padding                         : 0
- 0x04ed (1261) B       00 SnapToDiscrete                  : 0
- 0x04ee (1262) B       02 NumDiscreteLevels               : 2
- 0x04ef (1263) B       00 CalculateFopt                   : 0
- 0x04f0 (1264) f 508d673f m                               : 0.9045
- 0x04f4 (1268) f b7d140be b                               :-0.1883
- 0x04f8 (1272) I 00000000 Padding3                        : 0
- 0x04fc (1276) I 00000000 Padding3                        : 0
- 0x0500 (1280) I 00000000 Padding3                        : 0
- 0x0504 (1284) H     0000 Padding4                        : 0
- 0x0506 (1286) H     0000 FoptimalDc                      : 0
- 0x0508 (1288) H     0000 FoptimalAc                      : 0
- 0x050a (1290) H     0000 Padding2                        : 0
- 0x050c (1292) B       00 Padding                         : 0
- 0x050d (1293) B       00 SnapToDiscrete                  : 0
- 0x050e (1294) B       02 NumDiscreteLevels               : 2
- 0x050f (1295) B       00 CalculateFopt                   : 0
- 0x0510 (1296) f 789c823f m                               : 1.0204
- 0x0514 (1300) f a01aaf3e b                               : 0.342
- 0x0518 (1304) I 00000000 Padding3                        : 0
- 0x051c (1308) I 00000000 Padding3                        : 0
- 0x0520 (1312) I 00000000 Padding3                        : 0
- 0x0524 (1316) H     0000 Padding4                        : 0
- 0x0526 (1318) H     0000 FoptimalDc                      : 0
- 0x0528 (1320) H     0000 FoptimalAc                      : 0
- 0x052a (1322) H     0000 Padding2                        : 0
- 0x052c (1324) B       00 Padding                         : 0
- 0x052d (1325) B       00 SnapToDiscrete                  : 0
- 0x052e (1326) B       02 NumDiscreteLevels               : 2
- 0x052f (1327) B       00 CalculateFopt                   : 0
- 0x0530 (1328) f 508d673f m                               : 0.9045
- 0x0534 (1332) f b7d140be b                               :-0.1883
- 0x0538 (1336) I 00000000 Padding3                        : 0
- 0x053c (1340) I 00000000 Padding3                        : 0
- 0x0540 (1344) I 00000000 Padding3                        : 0
- 0x0544 (1348) H     0000 Padding4                        : 0
- 0x0546 (1350) H     0000 FoptimalDc                      : 0
- 0x0548 (1352) H     0000 FoptimalAc                      : 0
- 0x054a (1354) H     0000 Padding2                        : 0
- 0x054c (1356) B       00 Padding                         : 0
- 0x054d (1357) B       00 SnapToDiscrete                  : 0
- 0x054e (1358) B       02 NumDiscreteLevels               : 2
- 0x054f (1359) B       00 CalculateFopt                   : 0
- 0x0550 (1360) f fed4483f m                               : 0.7845
- 0x0554 (1364) f dbf93e3f b                               : 0.746
- 0x0558 (1368) I 00000000 Padding3                        : 0
- 0x055c (1372) I 00000000 Padding3                        : 0
- 0x0560 (1376) I 00000000 Padding3                        : 0
- 0x0564 (1380) H     0000 Padding4                        : 0
- 0x0566 (1382) H     0000 FoptimalDc                      : 0
- 0x0568 (1384) H     0000 FoptimalAc                      : 0
- 0x056a (1386) H     0000 Padding2                        : 0
- 0x056c (1388) B       00 Padding                         : 0
- 0x056d (1389) B       00 SnapToDiscrete                  : 0
- 0x056e (1390) B       02 NumDiscreteLevels               : 2
- 0x056f (1391) B       00 CalculateFopt                   : 0
- 0x0570 (1392) f fed4483f m                               : 0.7845
- 0x0574 (1396) f dbf93e3f b                               : 0.746
- 0x0578 (1400) I 00000000 Padding3                        : 0
- 0x057c (1404) I 00000000 Padding3                        : 0
- 0x0580 (1408) I 00000000 Padding3                        : 0
- 0x0584 (1412) H     0000 Padding4                        : 0
- 0x0586 (1414) H     0000 FoptimalDc                      : 0
- 0x0588 (1416) H     0000 FoptimalAc                      : 0
- 0x058a (1418) H     0000 Padding2                        : 0
- 0x058c (1420) B       00 Padding                         : 0
- 0x058d (1421) B       00 SnapToDiscrete                  : 0
- 0x058e (1422) B       02 NumDiscreteLevels               : 2
- 0x058f (1423) B       00 CalculateFopt                   : 0
- 0x0590 (1424) f 986ea23f m                               : 1.269
- 0x0594 (1428) f 1283403e b                               : 0.188
- 0x0598 (1432) I 00000000 Padding3                        : 0
- 0x059c (1436) I 00000000 Padding3                        : 0
- 0x05a0 (1440) I 00000000 Padding3                        : 0
- 0x05a4 (1444) H     0000 Padding4                        : 0
- 0x05a6 (1446) H     0000 FoptimalDc                      : 0
- 0x05a8 (1448) H     0000 FoptimalAc                      : 0
- 0x05aa (1450) H     0000 Padding2                        : 0
- 0x05ac (1452) B       00 Padding                         : 0
- 0x05ad (1453) B       00 SnapToDiscrete                  : 0
- 0x05ae (1454) B       02 NumDiscreteLevels               : 2
- 0x05af (1455) B       00 CalculateFopt                   : 0
- 0x05b0 (1456) f f2d28d3f m                               : 1.108
- 0x05b4 (1460) f 7b140e3f b                               : 0.555
- 0x05b8 (1464) I 00000000 Padding3                        : 0
- 0x05bc (1468) I 00000000 Padding3                        : 0
- 0x05c0 (1472) I 00000000 Padding3                        : 0
- 0x05c4 (1476) H     0000 Padding4                        : 0
- 0x05c6 (1478) H     0000 FoptimalDc                      : 0
- 0x05c8 (1480) H     0000 FoptimalAc                      : 0
- 0x05ca (1482) H     0000 Padding2                        : 0
- 0x05cc (1484) B       00 Padding                         : 0
- 0x05cd (1485) B       00 SnapToDiscrete                  : 0
- 0x05ce (1486) B       02 NumDiscreteLevels               : 2
- 0x05cf (1487) B       00 CalculateFopt                   : 0
- 0x05d0 (1488) f 986ea23f m                               : 1.269
- 0x05d4 (1492) f 1283403e b                               : 0.188
- 0x05d8 (1496) I 00000000 Padding3                        : 0
- 0x05dc (1500) I 00000000 Padding3                        : 0
- 0x05e0 (1504) I f401d007 Padding3                        : 131072500
- 0x05e4 (1508) H     0000 Padding4                        : 0
- 0x05e6 (1510) H     0000 FoptimalDc                      : 0
- 0x05e8 (1512) H     0000 FoptimalAc                      : 0
- 0x05ea (1514) H     0000 Padding2                        : 0
- 0x05ec (1516) H     f401 FreqTableGfx                    : 500
- 0x05ee (1518) H     920c FreqTableGfx                    : 3218
- 0x05f0 (1520) H     0000 FreqTableGfx                    : 0
- 0x05f2 (1522) H     0000 FreqTableGfx                    : 0
- 0x05f4 (1524) H     0000 FreqTableGfx                    : 0
- 0x05f6 (1526) H     0000 FreqTableGfx                    : 0
- 0x05f8 (1528) H     0000 FreqTableGfx                    : 0
- 0x05fa (1530) H     0000 FreqTableGfx                    : 0
- 0x05fc (1532) H     0000 FreqTableGfx                    : 0
- 0x05fe (1534) H     0000 FreqTableGfx                    : 0
- 0x0600 (1536) H     0000 FreqTableGfx                    : 0
- 0x0602 (1538) H     0000 FreqTableGfx                    : 0
- 0x0604 (1540) H     0000 FreqTableGfx                    : 0
- 0x0606 (1542) H     0000 FreqTableGfx                    : 0
- 0x0608 (1544) H     0000 FreqTableGfx                    : 0
- 0x060a (1546) H     0000 FreqTableGfx                    : 0
- 0x060c (1548) H     0102 FreqTableVclk                   : 513
- 0x060e (1550) H     760b FreqTableVclk                   : 2934
- 0x0610 (1552) H     0000 FreqTableVclk                   : 0
- 0x0612 (1554) H     0000 FreqTableVclk                   : 0
- 0x0614 (1556) H     0000 FreqTableVclk                   : 0
- 0x0616 (1558) H     0000 FreqTableVclk                   : 0
- 0x0618 (1560) H     0000 FreqTableVclk                   : 0
- 0x061a (1562) H     0000 FreqTableVclk                   : 0
- 0x061c (1564) H     0102 FreqTableDclk                   : 513
- 0x061e (1566) H     9808 FreqTableDclk                   : 2200
- 0x0620 (1568) H     0000 FreqTableDclk                   : 0
- 0x0622 (1570) H     0000 FreqTableDclk                   : 0
- 0x0624 (1572) H     0000 FreqTableDclk                   : 0
- 0x0626 (1574) H     0000 FreqTableDclk                   : 0
- 0x0628 (1576) H     0000 FreqTableDclk                   : 0
- 0x062a (1578) H     0000 FreqTableDclk                   : 0
- 0x062c (1580) H     f401 FreqTableSocclk                 : 500
- 0x062e (1582) H     dc05 FreqTableSocclk                 : 1500
- 0x0630 (1584) H     6100 FreqTableSocclk                 : 97
- 0x0632 (1586) H     c901 FreqTableSocclk                 : 457
- 0x0634 (1588) H     ad02 FreqTableSocclk                 : 685
- 0x0636 (1590) H     e803 FreqTableSocclk                 : 1000
- 0x0638 (1592) H     0000 FreqTableSocclk                 : 0
- 0x063a (1594) H     0000 FreqTableSocclk                 : 0
- 0x063c (1596) H     6100 FreqTableUclk                   : 97
- 0x063e (1598) H     c901 FreqTableUclk                   : 457
- 0x0640 (1600) H     0503 FreqTableUclk                   : 773
- 0x0642 (1602) H     e204 FreqTableUclk                   : 1250
- 0x0644 (1604) H     9400 FreqTableDispclk                : 148
- 0x0646 (1606) H     6608 FreqTableDispclk                : 2150
- 0x0648 (1608) H     0000 FreqTableDispclk                : 0
- 0x064a (1610) H     0000 FreqTableDispclk                : 0
- 0x064c (1612) H     0000 FreqTableDispclk                : 0
- 0x064e (1614) H     0000 FreqTableDispclk                : 0
- 0x0650 (1616) H     0000 FreqTableDispclk                : 0
- 0x0652 (1618) H     0000 FreqTableDispclk                : 0
- 0x0654 (1620) H     9400 FreqTableDppClk                 : 148
- 0x0656 (1622) H     6608 FreqTableDppClk                 : 2150
- 0x0658 (1624) H     0000 FreqTableDppClk                 : 0
- 0x065a (1626) H     0000 FreqTableDppClk                 : 0
- 0x065c (1628) H     0000 FreqTableDppClk                 : 0
- 0x065e (1630) H     0000 FreqTableDppClk                 : 0
- 0x0660 (1632) H     0000 FreqTableDppClk                 : 0
- 0x0662 (1634) H     0000 FreqTableDppClk                 : 0
- 0x0664 (1636) H     cd02 FreqTableDprefclk               : 717
- 0x0666 (1638) H     cd02 FreqTableDprefclk               : 717
- 0x0668 (1640) H     0000 FreqTableDprefclk               : 0
- 0x066a (1642) H     0000 FreqTableDprefclk               : 0
- 0x066c (1644) H     0000 FreqTableDprefclk               : 0
- 0x066e (1646) H     0000 FreqTableDprefclk               : 0
- 0x0670 (1648) H     0000 FreqTableDprefclk               : 0
- 0x0672 (1650) H     0000 FreqTableDprefclk               : 0
- 0x0674 (1652) H     9400 FreqTableDcfclk                 : 148
- 0x0676 (1654) H     1c06 FreqTableDcfclk                 : 1564
- 0x0678 (1656) H     0000 FreqTableDcfclk                 : 0
- 0x067a (1658) H     0000 FreqTableDcfclk                 : 0
- 0x067c (1660) H     0000 FreqTableDcfclk                 : 0
- 0x067e (1662) H     0000 FreqTableDcfclk                 : 0
- 0x0680 (1664) H     0000 FreqTableDcfclk                 : 0
- 0x0682 (1666) H     0000 FreqTableDcfclk                 : 0
- 0x0684 (1668) H     9400 FreqTableDtbclk                 : 148
- 0x0686 (1670) H     1c06 FreqTableDtbclk                 : 1564
- 0x0688 (1672) H     0000 FreqTableDtbclk                 : 0
- 0x068a (1674) H     0000 FreqTableDtbclk                 : 0
- 0x068c (1676) H     0000 FreqTableDtbclk                 : 0
- 0x068e (1678) H     0000 FreqTableDtbclk                 : 0
- 0x0690 (1680) H     0000 FreqTableDtbclk                 : 0
- 0x0692 (1682) H     0000 FreqTableDtbclk                 : 0
- 0x0694 (1684) H     5802 FreqTableFclk                   : 600
- 0x0696 (1686) H     e803 FreqTableFclk                   : 1000
- 0x0698 (1688) H     b004 FreqTableFclk                   : 1200
- 0x069a (1690) H     4006 FreqTableFclk                   : 1600
- 0x069c (1692) H     d007 FreqTableFclk                   : 2000
- 0x069e (1694) H     9808 FreqTableFclk                   : 2200
- 0x06a0 (1696) H     ca08 FreqTableFclk                   : 2250
- 0x06a2 (1698) H     fc08 FreqTableFclk                   : 2300
- 0x06a4 (1700) I 920c0000 DcModeMaxFreq                   : 3218
- 0x06a8 (1704) I dc050000 DcModeMaxFreq                   : 1500
- 0x06ac (1708) I e2040000 DcModeMaxFreq                   : 1250
- 0x06b0 (1712) I fc080000 DcModeMaxFreq                   : 2300
- 0x06b4 (1716) I 98080000 DcModeMaxFreq                   : 2200
- 0x06b8 (1720) I 760b0000 DcModeMaxFreq                   : 2934
- 0x06bc (1724) I 98080000 DcModeMaxFreq                   : 2200
- 0x06c0 (1728) I 760b0000 DcModeMaxFreq                   : 2934
- 0x06c4 (1732) I 66080000 DcModeMaxFreq                   : 2150
- 0x06c8 (1736) I 66080000 DcModeMaxFreq                   : 2150
- 0x06cc (1740) I cd020000 DcModeMaxFreq                   : 717
- 0x06d0 (1744) I 1c060000 DcModeMaxFreq                   : 1564
- 0x06d4 (1748) I 1c060000 DcModeMaxFreq                   : 1564
- 0x06d8 (1752) H     f401 Mp0clkFreq                      : 500
- 0x06da (1754) H     bc02 Mp0clkFreq                      : 700
- 0x06dc (1756) H     f00a Mp0DpmVoltage                   : 2800
- 0x06de (1758) H     800c Mp0DpmVoltage                   : 3200
- 0x06e0 (1760) B       00 GfxclkSpare                     : 0
- 0x06e1 (1761) B       00 GfxclkSpare                     : 0
- 0x06e2 (1762) H     0000 GfxclkFreqCap                   : 0
- 0x06e4 (1764) H     2003 GfxclkFgfxoffEntry              : 800
- 0x06e6 (1766) H     b004 GfxclkFgfxoffExitImu            : 1200
- 0x06e8 (1768) H     2003 GfxclkFgfxoffExitRlc            : 800
- 0x06ea (1770) H     fa00 GfxclkThrottleClock             : 250
- 0x06ec (1772) B       01 EnableGfxPowerStagesGpio        : 1
- 0x06ed (1773) B       00 GfxIdlePadding                  : 0
- 0x06ee (1774) B       01 SmsRepairWRCKClkDivEn           : 1
- 0x06ef (1775) B       04 SmsRepairWRCKClkDivVal          : 4
- 0x06f0 (1776) B       01 GfxOffEntryEarlyMGCGEn          : 1
- 0x06f1 (1777) B       00 GfxOffEntryForceCGCGEn          : 0
- 0x06f2 (1778) B       00 GfxOffEntryForceCGCGDelayEn     : 0
- 0x06f3 (1779) B       00 GfxOffEntryForceCGCGDelayVal    : 0
- 0x06f4 (1780) H     1405 GfxclkFreqGfxUlv                : 1300
- 0x06f6 (1782) B       00 GfxIdlePadding2                 : 0
- 0x06f7 (1783) B       00 GfxIdlePadding2                 : 0
- 0x06f8 (1784) I 60ea0000 GfxOffEntryHysteresis           : 60000
- 0x06fc (1788) I 00000000 GfxoffSpare                     : 0
- 0x0700 (1792) I 00000000 GfxoffSpare                     : 0
- 0x0704 (1796) I 00000000 GfxoffSpare                     : 0
- 0x0708 (1800) I 00000000 GfxoffSpare                     : 0
- 0x070c (1804) I 00000000 GfxoffSpare                     : 0
- 0x0710 (1808) I 00000000 GfxoffSpare                     : 0
- 0x0714 (1812) I 00000000 GfxoffSpare                     : 0
- 0x0718 (1816) I 00000000 GfxoffSpare                     : 0
- 0x071c (1820) I 00000000 GfxoffSpare                     : 0
- 0x0720 (1824) I 00000000 GfxoffSpare                     : 0
- 0x0724 (1828) I 00000000 GfxoffSpare                     : 0
- 0x0728 (1832) I 00000000 GfxoffSpare                     : 0
- 0x072c (1836) I 00000000 GfxoffSpare                     : 0
- 0x0730 (1840) I 00000000 GfxoffSpare                     : 0
- 0x0734 (1844) I 00000000 GfxoffSpare                     : 0
- 0x0738 (1848) I 0000803f DfllBtcMasterScalerM            : 1065353216
+ Offset (dec.) t Raw val. Variable name                         Decoded value
+------------------------------------------------------------------------------
+ 0x0000 (0000) H     3015 structuresize                             : 5424
+ 0x0002 (0002) B       14 format_revision                           : 20
+ 0x0003 (0003) B       00 content_revision                          : 0
+ 0x0004 (0004) B       03 table_revision                            : 3
+ 0x0005 (0005) B       00 padding                                   : 0
+ 0x0006 (0006) H     4003 table_size                                : 832
+ 0x0008 (0008) I 3c0f0000 golden_pp_id                              : 3900
+ 0x000c (0012) I 11540000 golden_revision                           : 21521
+ 0x0010 (0016) H     8500 format_id                                 : 133
+ 0x0012 (0018) I 08000000 platform_caps                             : 8
+ 0x0016 (0022) B       1d thermal_controller_type                   : 29
+ 0x0017 (0023) H     0000 small_power_limit1                        : 0
+ 0x0019 (0025) H     0000 small_power_limit2                        : 0
+ 0x001b (0027) H     0000 boost_power_limit                         : 0
+ 0x001d (0029) H     7600 software_shutdown_temp                    : 118
+ 0x001f (0031) I 00000000 reserve                                   : 0
+ 0x0023 (0035) I 00000000 reserve                                   : 0
+ 0x0027 (0039) I 00000000 reserve                                   : 0
+ 0x002b (0043) I 00000000 reserve                                   : 0
+ 0x002f (0047) I 00000000 reserve                                   : 0
+ 0x0033 (0051) I 00000000 reserve                                   : 0
+ 0x0037 (0055) I 00000000 reserve                                   : 0
+ 0x003b (0059) I 00000000 reserve                                   : 0
+ 0x003f (0063) I 00000000 reserve                                   : 0
+ 0x0043 (0067) I 00000000 reserve                                   : 0
+ 0x0047 (0071) I 00000000 reserve                                   : 0
+ 0x004b (0075) I 00000000 reserve                                   : 0
+ 0x004f (0079) I 00000000 reserve                                   : 0
+ 0x0053 (0083) I 00000000 reserve                                   : 0
+ 0x0057 (0087) I 00000000 reserve                                   : 0
+ 0x005b (0091) I 00000000 reserve                                   : 0
+ 0x005f (0095) I 00000000 reserve                                   : 0
+ 0x0063 (0099) I 00000000 reserve                                   : 0
+ 0x0067 (0103) I 00000000 reserve                                   : 0
+ 0x006b (0107) I 00000000 reserve                                   : 0
+ 0x006f (0111) I 00000000 reserve                                   : 0
+ 0x0073 (0115) I 00000000 reserve                                   : 0
+ 0x0077 (0119) I 00000000 reserve                                   : 0
+ 0x007b (0123) I 00000000 reserve                                   : 0
+ 0x007f (0127) I 00000000 reserve                                   : 0
+ 0x0083 (0131) I 00000000 reserve                                   : 0
+ 0x0087 (0135) I 00000000 reserve                                   : 0
+ 0x008b (0139) I 00000000 reserve                                   : 0
+ 0x008f (0143) I 00000000 reserve                                   : 0
+ 0x0093 (0147) I 00000000 reserve                                   : 0
+ 0x0097 (0151) I 00000000 reserve                                   : 0
+ 0x009b (0155) I 00000000 reserve                                   : 0
+ 0x009f (0159) I 00000000 reserve                                   : 0
+ 0x00a3 (0163) I 00000000 reserve                                   : 0
+ 0x00a7 (0167) I 00000000 reserve                                   : 0
+ 0x00ab (0171) I 00000000 reserve                                   : 0
+ 0x00af (0175) I 00000000 reserve                                   : 0
+ 0x00b3 (0179) I 00000000 reserve                                   : 0
+ 0x00b7 (0183) I 00000000 reserve                                   : 0
+ 0x00bb (0187) I 00000000 reserve                                   : 0
+ 0x00bf (0191) I 00000000 reserve                                   : 0
+ 0x00c3 (0195) I 00000000 reserve                                   : 0
+ 0x00c7 (0199) I 00000000 reserve                                   : 0
+ 0x00cb (0203) I 00000000 reserve                                   : 0
+ 0x00cf (0207) I 00000000 reserve                                   : 0
+ 0x00d3 (0211) B       83 revision                                  : 131
+ 0x00d4 (0212) B       00 reserve                                   : 0
+ 0x00d5 (0213) B       00 reserve                                   : 0
+ 0x00d6 (0214) B       00 reserve                                   : 0
+ 0x00d7 (0215) I 16000000 feature_count                             : 22
+ 0x00db (0219) I 29000000 setting_count                             : 41
+ 0x00df (0223) B       01 cap GFXCLK_LIMITS                         : 1
+ 0x00e0 (0224) B       01 cap UCLK_LIMITS                           : 1
+ 0x00e1 (0225) B       01 cap POWER_LIMIT                           : 1
+ 0x00e2 (0226) B       01 cap FAN_ACOUSTIC_LIMIT                    : 1
+ 0x00e3 (0227) B       01 cap FAN_SPEED_MIN                         : 1
+ 0x00e4 (0228) B       01 cap TEMPERATURE_FAN                       : 1
+ 0x00e5 (0229) B       01 cap TEMPERATURE_SYSTEM                    : 1
+ 0x00e6 (0230) B       01 cap MEMORY_TIMING_TUNE                    : 1
+ 0x00e7 (0231) B       01 cap FAN_ZERO_RPM_CONTROL                  : 1
+ 0x00e8 (0232) B       01 cap AUTO_UV_ENGINE                        : 1
+ 0x00e9 (0233) B       01 cap AUTO_OC_ENGINE                        : 1
+ 0x00ea (0234) B       01 cap AUTO_OC_MEMORY                        : 1
+ 0x00eb (0235) B       01 cap FAN_CURVE                             : 1
+ 0x00ec (0236) B       00 cap AUTO_FAN_ACOUSTIC_LIMIT               : 0
+ 0x00ed (0237) B       01 cap POWER_MODE                            : 1
+ 0x00ee (0238) B       00 cap PER_ZONE_GFX_VOLTAGE_OFFSET           : 0
+ 0x00ef (0239) B       00 cap                                       : 0
+ 0x00f0 (0240) B       01 cap                                       : 1
+ 0x00f1 (0241) B       00 cap                                       : 0
+ 0x00f2 (0242) B       00 cap                                       : 0
+ 0x00f3 (0243) B       00 cap                                       : 0
+ 0x00f4 (0244) B       00 cap                                       : 0
+ 0x00f5 (0245) B       00 cap                                       : 0
+ 0x00f6 (0246) B       00 cap                                       : 0
+ 0x00f7 (0247) B       00 cap                                       : 0
+ 0x00f8 (0248) B       00 cap                                       : 0
+ 0x00f9 (0249) B       00 cap                                       : 0
+ 0x00fa (0250) B       00 cap                                       : 0
+ 0x00fb (0251) B       00 cap                                       : 0
+ 0x00fc (0252) B       00 cap                                       : 0
+ 0x00fd (0253) B       00 cap                                       : 0
+ 0x00fe (0254) B       00 cap                                       : 0
+ 0x00ff (0255) I 88130000 max GFXCLKFMAX                            : 5000
+ 0x0103 (0259) I 88130000 max GFXCLKFMIN                            : 5000
+ 0x0107 (0263) I dc050000 max UCLKFMIN                              : 1500
+ 0x010b (0267) I dc050000 max UCLKFMAX                              : 1500
+ 0x010f (0271) I 0f000000 max POWERPERCENTAGE                       : 15
+ 0x0113 (0275) I e40c0000 max FANRPMMIN                             : 3300
+ 0x0117 (0279) I e40c0000 max FANRPMACOUSTICLIMIT                   : 3300
+ 0x011b (0283) I 69000000 max FANTARGETTEMPERATURE                  : 105
+ 0x011f (0287) I 6e000000 max OPERATINGTEMPMAX                      : 110
+ 0x0123 (0291) I 01000000 max ACTIMING                              : 1
+ 0x0127 (0295) I 01000000 max FAN_ZERO_RPM_CONTROL                  : 1
+ 0x012b (0299) I 01000000 max AUTOUVENGINE                          : 1
+ 0x012f (0303) I 01000000 max AUTOOCENGINE                          : 1
+ 0x0133 (0307) I 01000000 max AUTOOCMEMORY                          : 1
+ 0x0137 (0311) I 64000000 max FAN_CURVE_TEMPERATURE_1               : 100
+ 0x013b (0315) I 64000000 max FAN_CURVE_SPEED_1                     : 100
+ 0x013f (0319) I 64000000 max FAN_CURVE_TEMPERATURE_2               : 100
+ 0x0143 (0323) I 64000000 max FAN_CURVE_SPEED_2                     : 100
+ 0x0147 (0327) I 64000000 max FAN_CURVE_TEMPERATURE_3               : 100
+ 0x014b (0331) I 64000000 max FAN_CURVE_SPEED_3                     : 100
+ 0x014f (0335) I 64000000 max FAN_CURVE_TEMPERATURE_4               : 100
+ 0x0153 (0339) I 64000000 max FAN_CURVE_SPEED_4                     : 100
+ 0x0157 (0343) I 64000000 max FAN_CURVE_TEMPERATURE_5               : 100
+ 0x015b (0347) I 64000000 max FAN_CURVE_SPEED_5                     : 100
+ 0x015f (0351) I 00000000 max AUTO_FAN_ACOUSTIC_LIMIT               : 0
+ 0x0163 (0355) I 01000000 max POWER_MODE                            : 1
+ 0x0167 (0359) I 00000000 max PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_1   : 0
+ 0x016b (0363) I 00000000 max PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_2   : 0
+ 0x016f (0367) I 00000000 max PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_3   : 0
+ 0x0173 (0371) I 00000000 max PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_4   : 0
+ 0x0177 (0375) I 00000000 max PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_5   : 0
+ 0x017b (0379) I 00000000 max PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_6   : 0
+ 0x017f (0383) I 00000000 max                                       : 0
+ 0x0183 (0387) I 00000000 max                                       : 0
+ 0x0187 (0391) I 00000000 max                                       : 0
+ 0x018b (0395) I 00000000 max                                       : 0
+ 0x018f (0399) I 00000000 max                                       : 0
+ 0x0193 (0403) I 00000000 max                                       : 0
+ 0x0197 (0407) I 00000000 max                                       : 0
+ 0x019b (0411) I 00000000 max                                       : 0
+ 0x019f (0415) I 00000000 max                                       : 0
+ 0x01a3 (0419) I 00000000 max                                       : 0
+ 0x01a7 (0423) I 00000000 max                                       : 0
+ 0x01ab (0427) I 00000000 max                                       : 0
+ 0x01af (0431) I 00000000 max                                       : 0
+ 0x01b3 (0435) I 00000000 max                                       : 0
+ 0x01b7 (0439) I 00000000 max                                       : 0
+ 0x01bb (0443) I 00000000 max                                       : 0
+ 0x01bf (0447) I 00000000 max                                       : 0
+ 0x01c3 (0451) I 00000000 max                                       : 0
+ 0x01c7 (0455) I 00000000 max                                       : 0
+ 0x01cb (0459) I 00000000 max                                       : 0
+ 0x01cf (0463) I 00000000 max                                       : 0
+ 0x01d3 (0467) I 00000000 max                                       : 0
+ 0x01d7 (0471) I 00000000 max                                       : 0
+ 0x01db (0475) I 00000000 max                                       : 0
+ 0x01df (0479) I 00000000 max                                       : 0
+ 0x01e3 (0483) I 00000000 max                                       : 0
+ 0x01e7 (0487) I 00000000 max                                       : 0
+ 0x01eb (0491) I 00000000 max                                       : 0
+ 0x01ef (0495) I 00000000 max                                       : 0
+ 0x01f3 (0499) I 00000000 max                                       : 0
+ 0x01f7 (0503) I 00000000 max                                       : 0
+ 0x01fb (0507) I 00000000 max                                       : 0
+ 0x01ff (0511) I f4010000 min GFXCLKFMAX                            : 500
+ 0x0203 (0515) I f4010000 min GFXCLKFMIN                            : 500
+ 0x0207 (0519) I 61000000 min UCLKFMIN                              : 97
+ 0x020b (0523) I 61000000 min UCLKFMAX                              : 97
+ 0x020f (0527) I 0a000000 min POWERPERCENTAGE                       : 10
+ 0x0213 (0531) I f4010000 min FANRPMMIN                             : 500
+ 0x0217 (0535) I f4010000 min FANRPMACOUSTICLIMIT                   : 500
+ 0x021b (0539) I 19000000 min FANTARGETTEMPERATURE                  : 25
+ 0x021f (0543) I 32000000 min OPERATINGTEMPMAX                      : 50
+ 0x0223 (0547) I 00000000 min ACTIMING                              : 0
+ 0x0227 (0551) I 00000000 min FAN_ZERO_RPM_CONTROL                  : 0
+ 0x022b (0555) I 00000000 min AUTOUVENGINE                          : 0
+ 0x022f (0559) I 00000000 min AUTOOCENGINE                          : 0
+ 0x0233 (0563) I 00000000 min AUTOOCMEMORY                          : 0
+ 0x0237 (0567) I 19000000 min FAN_CURVE_TEMPERATURE_1               : 25
+ 0x023b (0571) I 0f000000 min FAN_CURVE_SPEED_1                     : 15
+ 0x023f (0575) I 19000000 min FAN_CURVE_TEMPERATURE_2               : 25
+ 0x0243 (0579) I 0f000000 min FAN_CURVE_SPEED_2                     : 15
+ 0x0247 (0583) I 19000000 min FAN_CURVE_TEMPERATURE_3               : 25
+ 0x024b (0587) I 0f000000 min FAN_CURVE_SPEED_3                     : 15
+ 0x024f (0591) I 19000000 min FAN_CURVE_TEMPERATURE_4               : 25
+ 0x0253 (0595) I 0f000000 min FAN_CURVE_SPEED_4                     : 15
+ 0x0257 (0599) I 19000000 min FAN_CURVE_TEMPERATURE_5               : 25
+ 0x025b (0603) I 0f000000 min FAN_CURVE_SPEED_5                     : 15
+ 0x025f (0607) I 00000000 min AUTO_FAN_ACOUSTIC_LIMIT               : 0
+ 0x0263 (0611) I 00000000 min POWER_MODE                            : 0
+ 0x0267 (0615) I 00000000 min PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_1   : 0
+ 0x026b (0619) I 00000000 min PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_2   : 0
+ 0x026f (0623) I 00000000 min PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_3   : 0
+ 0x0273 (0627) I 00000000 min PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_4   : 0
+ 0x0277 (0631) I 00000000 min PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_5   : 0
+ 0x027b (0635) I 00000000 min PER_ZONE_GFX_VOLTAGE_OFFSET_POINT_6   : 0
+ 0x027f (0639) I 00000000 min                                       : 0
+ 0x0283 (0643) I 0a000000 min                                       : 10
+ 0x0287 (0647) I 00000000 min                                       : 0
+ 0x028b (0651) I 00000000 min                                       : 0
+ 0x028f (0655) I 00000000 min                                       : 0
+ 0x0293 (0659) I 00000000 min                                       : 0
+ 0x0297 (0663) I 00000000 min                                       : 0
+ 0x029b (0667) I 00000000 min                                       : 0
+ 0x029f (0671) I 00000000 min                                       : 0
+ 0x02a3 (0675) I 00000000 min                                       : 0
+ 0x02a7 (0679) I 00000000 min                                       : 0
+ 0x02ab (0683) I 00000000 min                                       : 0
+ 0x02af (0687) I 00000000 min                                       : 0
+ 0x02b3 (0691) I 00000000 min                                       : 0
+ 0x02b7 (0695) I 00000000 min                                       : 0
+ 0x02bb (0699) I 00000000 min                                       : 0
+ 0x02bf (0703) I 00000000 min                                       : 0
+ 0x02c3 (0707) I 00000000 min                                       : 0
+ 0x02c7 (0711) I 00000000 min                                       : 0
+ 0x02cb (0715) I 00000000 min                                       : 0
+ 0x02cf (0719) I 00000000 min                                       : 0
+ 0x02d3 (0723) I 00000000 min                                       : 0
+ 0x02d7 (0727) I 00000000 min                                       : 0
+ 0x02db (0731) I 00000000 min                                       : 0
+ 0x02df (0735) I 00000000 min                                       : 0
+ 0x02e3 (0739) I 00000000 min                                       : 0
+ 0x02e7 (0743) I 00000000 min                                       : 0
+ 0x02eb (0747) I 00000000 min                                       : 0
+ 0x02ef (0751) I 00000000 min                                       : 0
+ 0x02f3 (0755) I 00000000 min                                       : 0
+ 0x02f7 (0759) I 00000000 min                                       : 0
+ 0x02fb (0763) I 00000000 min                                       : 0
+ 0x02ff (0767) h     0000 pm_setting                                : 0
+ 0x0301 (0769) h     0000 pm_setting                                : 0
+ 0x0303 (0771) h     0000 pm_setting                                : 0
+ 0x0305 (0773) h     0a00 pm_setting                                : 10
+ 0x0307 (0775) h     6900 pm_setting                                : 105
+ 0x0309 (0777) h     5f00 pm_setting                                : 95
+ 0x030b (0779) h     0000 pm_setting                                : 0
+ 0x030d (0781) h     4b00 pm_setting                                : 75
+ 0x030f (0783) h     0e06 pm_setting                                : 1550
+ 0x0311 (0785) h     a406 pm_setting                                : 1700
+ 0x0313 (0787) h     0000 pm_setting                                : 0
+ 0x0315 (0789) h     b80b pm_setting                                : 3000
+ 0x0317 (0791) h     0e06 pm_setting                                : 1550
+ 0x0319 (0793) h     b80b pm_setting                                : 3000
+ 0x031b (0795) h     0000 pm_setting                                : 0
+ 0x031d (0797) h     b80b pm_setting                                : 3000
+ 0x031f (0799) h     0000 pm_setting                                : 0
+ 0x0321 (0801) h     0000 pm_setting                                : 0
+ 0x0323 (0803) h     0000 pm_setting                                : 0
+ 0x0325 (0805) h     0000 pm_setting                                : 0
+ 0x0327 (0807) h     0000 pm_setting                                : 0
+ 0x0329 (0809) h     0000 pm_setting                                : 0
+ 0x032b (0811) h     0000 pm_setting                                : 0
+ 0x032d (0813) h     0000 pm_setting                                : 0
+ 0x032f (0815) h     0000 pm_setting                                : 0
+ 0x0331 (0817) h     0000 pm_setting                                : 0
+ 0x0333 (0819) h     0000 pm_setting                                : 0
+ 0x0335 (0821) h     0000 pm_setting                                : 0
+ 0x0337 (0823) h     0000 pm_setting                                : 0
+ 0x0339 (0825) h     0000 pm_setting                                : 0
+ 0x033b (0827) h     0000 pm_setting                                : 0
+ 0x033d (0829) h     0000 pm_setting                                : 0
+ 0x033f (0831) B       00 padding1                                  : 0
+ 0x0340 (0832) I 29000000 Version                                   : 41
+ 0x0344 (0836) I ffffff71 FeaturesToRun                             : 1912602623
+ 0x0348 (0840) I b8eb0300 FeaturesToRun                             : 256952
+ 0x034c (0844) B       01 TotalPowerConfig                          : 1
+ 0x034d (0845) B       00 CustomerVariant                           : 0
+ 0x034e (0846) B       04 MemoryTemperatureTypeMask                 : 4
+ 0x034f (0847) B       00 SmartShiftVersion                         : 0
+ 0x0350 (0848) H     4701 SocketPowerLimitAc                        : 327
+ 0x0352 (0850) H     b004 SocketPowerLimitAc                        : 1200
+ 0x0354 (0852) H     0000 SocketPowerLimitAc                        : 0
+ 0x0356 (0854) H     0000 SocketPowerLimitAc                        : 0
+ 0x0358 (0856) H     0000 SocketPowerLimitDc                        : 0
+ 0x035a (0858) H     0000 SocketPowerLimitDc                        : 0
+ 0x035c (0860) H     0000 SocketPowerLimitDc                        : 0
+ 0x035e (0862) H     0000 SocketPowerLimitDc                        : 0
+ 0x0360 (0864) H     0000 SocketPowerLimitSmartShift2               : 0
+ 0x0362 (0866) B       00 EnableLegacyPptLimit                      : 0
+ 0x0363 (0867) B       00 UseInputTelemetry                         : 0
+ 0x0364 (0868) B       00 SmartShiftMinReportedPptinDcs             : 0
+ 0x0365 (0869) B       00 PaddingPpt                                : 0
+ 0x0366 (0870) H     3b01 VrTdcLimit                                : 315
+ 0x0368 (0872) H     5200 VrTdcLimit                                : 82
+ 0x036a (0874) H     5600 VrTdcLimit                                : 86
+ 0x036c (0876) H     c001 PlatformTdcLimit                          : 448
+ 0x036e (0878) H     5200 PlatformTdcLimit                          : 82
+ 0x0370 (0880) H     5600 PlatformTdcLimit                          : 86
+ 0x0372 (0882) H     6400 TemperatureLimit                          : 100
+ 0x0374 (0884) H     6e00 TemperatureLimit                          : 110
+ 0x0376 (0886) H     6e00 TemperatureLimit                          : 110
+ 0x0378 (0888) H     6e00 TemperatureLimit                          : 110
+ 0x037a (0890) H     6c00 TemperatureLimit                          : 108
+ 0x037c (0892) H     7300 TemperatureLimit                          : 115
+ 0x037e (0894) H     7300 TemperatureLimit                          : 115
+ 0x0380 (0896) H     7300 TemperatureLimit                          : 115
+ 0x0382 (0898) H     7300 TemperatureLimit                          : 115
+ 0x0384 (0900) H     7300 TemperatureLimit                          : 115
+ 0x0386 (0902) H     0000 TemperatureLimit                          : 0
+ 0x0388 (0904) H     0000 TemperatureLimit                          : 0
+ 0x038a (0906) H     0000 TemperatureLimit                          : 0
+ 0x038c (0908) H     7800 HwCtfTempLimit                            : 120
+ 0x038e (0910) H     0000 PaddingInfra                              : 0
+ 0x0390 (0912) I 00000000 FitControllerFailureRateLimit             : 0
+ 0x0394 (0916) I 00000000 FitControllerGfxDutyCycle                 : 0
+ 0x0398 (0920) I 00000000 FitControllerSocDutyCycle                 : 0
+ 0x039c (0924) I 00000000 FitControllerSocOffset                    : 0
+ 0x03a0 (0928) I 00000000 GfxApccPlusResidencyLimit                 : 0
+ 0x03a4 (0932) I f2e30300 ThrottlerControlMask                      : 254962
+ 0x03a8 (0936) I ffff9b01 FwDStateMask                              : 27000831
+ 0x03ac (0940) H     6400 UlvVoltageOffset                          : 100
+ 0x03ae (0942) H     6400 UlvVoltageOffset                          : 100
+ 0x03b0 (0944) H     6400 UlvVoltageOffsetU                         : 100
+ 0x03b2 (0946) H     6400 DeepUlvVoltageOffsetSoc                   : 100
+ 0x03b4 (0948) H     f811 DefaultMaxVoltage                         : 4600
+ 0x03b6 (0950) H     c012 DefaultMaxVoltage                         : 4800
+ 0x03b8 (0952) H     f811 BoostMaxVoltage                           : 4600
+ 0x03ba (0954) H     c012 BoostMaxVoltage                           : 4800
+ 0x03bc (0956) h     0500 VminTempHystersis                         : 5
+ 0x03be (0958) h     0500 VminTempHystersis                         : 5
+ 0x03c0 (0960) h     3700 VminTempThreshold                         : 55
+ 0x03c2 (0962) h     3700 VminTempThreshold                         : 55
+ 0x03c4 (0964) H     f00a Vmin_Hot_T0                               : 2800
+ 0x03c6 (0966) H     f00a Vmin_Hot_T0                               : 2800
+ 0x03c8 (0968) H     f00a Vmin_Cold_T0                              : 2800
+ 0x03ca (0970) H     f00a Vmin_Cold_T0                              : 2800
+ 0x03cc (0972) H     f00a Vmin_Hot_Eol                              : 2800
+ 0x03ce (0974) H     f00a Vmin_Hot_Eol                              : 2800
+ 0x03d0 (0976) H     f00a Vmin_Cold_Eol                             : 2800
+ 0x03d2 (0978) H     f00a Vmin_Cold_Eol                             : 2800
+ 0x03d4 (0980) H     0000 Vmin_Aging_Offset                         : 0
+ 0x03d6 (0982) H     0000 Vmin_Aging_Offset                         : 0
+ 0x03d8 (0984) H     0000 Spare_Vmin_Plat_Offset_Hot                : 0
+ 0x03da (0986) H     0000 Spare_Vmin_Plat_Offset_Hot                : 0
+ 0x03dc (0988) H     0000 Spare_Vmin_Plat_Offset_Cold               : 0
+ 0x03de (0990) H     0000 Spare_Vmin_Plat_Offset_Cold               : 0
+ 0x03e0 (0992) H     0000 VcBtcFixedVminAgingOffset                 : 0
+ 0x03e2 (0994) H     0000 VcBtcFixedVminAgingOffset                 : 0
+ 0x03e4 (0996) H     0000 VcBtcVmin2PsmDegrationGb                  : 0
+ 0x03e6 (0998) H     0000 VcBtcVmin2PsmDegrationGb                  : 0
+ 0x03e8 (1000) f 00000000 VcBtcPsmA                                 : 0
+ 0x03ec (1004) f 00000000 VcBtcPsmA                                 : 0
+ 0x03f0 (1008) f 00000000 VcBtcPsmB                                 : 0
+ 0x03f4 (1012) f 00000000 VcBtcPsmB                                 : 0
+ 0x03f8 (1016) f 00000000 VcBtcVminA                                : 0
+ 0x03fc (1020) f 00000000 VcBtcVminA                                : 0
+ 0x0400 (1024) f 00000000 VcBtcVminB                                : 0
+ 0x0404 (1028) f 00000000 VcBtcVminB                                : 0
+ 0x0408 (1032) B       01 PerPartVminEnabled                        : 1
+ 0x0409 (1033) B       00 PerPartVminEnabled                        : 0
+ 0x040a (1034) B       00 VcBtcEnabled                              : 0
+ 0x040b (1035) B       00 VcBtcEnabled                              : 0
+ 0x040c (1036) H     6400 SocketPowerLimitAcTau                     : 100
+ 0x040e (1038) H     0a00 SocketPowerLimitAcTau                     : 10
+ 0x0410 (1040) H     0000 SocketPowerLimitAcTau                     : 0
+ 0x0412 (1042) H     0000 SocketPowerLimitAcTau                     : 0
+ 0x0414 (1044) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x0416 (1046) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x0418 (1048) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x041a (1050) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x041c (1052) f 00000000 a                                         : 0
+ 0x0420 (1056) f 9a99993d b                                         : 0.075
+ 0x0424 (1060) f 0ad723bc c                                         :-0.01
+ 0x0428 (1064) I 00000000 SpareVmin                                 : 0
+ 0x042c (1068) I 00000000 SpareVmin                                 : 0
+ 0x0430 (1072) I 00000000 SpareVmin                                 : 0
+ 0x0434 (1076) I 00000000 SpareVmin                                 : 0
+ 0x0438 (1080) I 00000000 SpareVmin                                 : 0
+ 0x043c (1084) I 00000000 SpareVmin                                 : 0
+ 0x0440 (1088) I 00000200 SpareVmin                                 : 131072
+ 0x0444 (1092) I 00000000 SpareVmin                                 : 0
+ 0x0448 (1096) I 00000000 SpareVmin                                 : 0
+ 0x044c (1100) B       00 Padding                                   : 0
+ 0x044d (1101) B       00 SnapToDiscrete                            : 0
+ 0x044e (1102) B       02 NumDiscreteLevels                         : 2
+ 0x044f (1103) B       03 CalculateFopt                             : 3
+ 0x0450 (1104) f 0000803f m                                         : 1
+ 0x0454 (1108) f 00000000 b                                         : 0
+ 0x0458 (1112) I 00000000 Padding3                                  : 0
+ 0x045c (1116) I 00000000 Padding3                                  : 0
+ 0x0460 (1120) I 00000000 Padding3                                  : 0
+ 0x0464 (1124) H     0000 Padding4                                  : 0
+ 0x0466 (1126) H     0000 FoptimalDc                                : 0
+ 0x0468 (1128) H     f401 FoptimalAc                                : 500
+ 0x046a (1130) H     0000 Padding2                                  : 0
+ 0x046c (1132) B       00 Padding                                   : 0
+ 0x046d (1133) B       00 SnapToDiscrete                            : 0
+ 0x046e (1134) B       02 NumDiscreteLevels                         : 2
+ 0x046f (1135) B       00 CalculateFopt                             : 0
+ 0x0470 (1136) f 6210a83f m                                         : 1.313
+ 0x0474 (1140) f f0a7463e b                                         : 0.194
+ 0x0478 (1144) I 00000000 Padding3                                  : 0
+ 0x047c (1148) I 00000000 Padding3                                  : 0
+ 0x0480 (1152) I 00010400 Padding3                                  : 262400
+ 0x0484 (1156) H     0000 Padding4                                  : 0
+ 0x0486 (1158) H     0000 FoptimalDc                                : 0
+ 0x0488 (1160) H     0000 FoptimalAc                                : 0
+ 0x048a (1162) H     0000 Padding2                                  : 0
+ 0x048c (1164) B       00 Padding                                   : 0
+ 0x048d (1165) B       01 SnapToDiscrete                            : 1
+ 0x048e (1166) B       04 NumDiscreteLevels                         : 4
+ 0x048f (1167) B       00 CalculateFopt                             : 0
+ 0x0490 (1168) f aaf1c23f m                                         : 1.523
+ 0x0494 (1172) f a60ac63d b                                         : 0.0967
+ 0x0498 (1176) I 00000000 Padding3                                  : 0
+ 0x049c (1180) I 00000000 Padding3                                  : 0
+ 0x04a0 (1184) I 00000000 Padding3                                  : 0
+ 0x04a4 (1188) H     0000 Padding4                                  : 0
+ 0x04a6 (1190) H     0000 FoptimalDc                                : 0
+ 0x04a8 (1192) H     0000 FoptimalAc                                : 0
+ 0x04aa (1194) H     0000 Padding2                                  : 0
+ 0x04ac (1196) B       00 Padding                                   : 0
+ 0x04ad (1197) B       01 SnapToDiscrete                            : 1
+ 0x04ae (1198) B       08 NumDiscreteLevels                         : 8
+ 0x04af (1199) B       03 CalculateFopt                             : 3
+ 0x04b0 (1200) f 0000803f m                                         : 1
+ 0x04b4 (1204) f 00000000 b                                         : 0
+ 0x04b8 (1208) I 00000000 Padding3                                  : 0
+ 0x04bc (1212) I 00000000 Padding3                                  : 0
+ 0x04c0 (1216) I 00000000 Padding3                                  : 0
+ 0x04c4 (1220) H     0000 Padding4                                  : 0
+ 0x04c6 (1222) H     0000 FoptimalDc                                : 0
+ 0x04c8 (1224) H     fc08 FoptimalAc                                : 2300
+ 0x04ca (1226) H     0000 Padding2                                  : 0
+ 0x04cc (1228) B       00 Padding                                   : 0
+ 0x04cd (1229) B       00 SnapToDiscrete                            : 0
+ 0x04ce (1230) B       02 NumDiscreteLevels                         : 2
+ 0x04cf (1231) B       00 CalculateFopt                             : 0
+ 0x04d0 (1232) f 789c823f m                                         : 1.0204
+ 0x04d4 (1236) f a01aaf3e b                                         : 0.342
+ 0x04d8 (1240) I 00000000 Padding3                                  : 0
+ 0x04dc (1244) I 00000000 Padding3                                  : 0
+ 0x04e0 (1248) I 00000000 Padding3                                  : 0
+ 0x04e4 (1252) H     0000 Padding4                                  : 0
+ 0x04e6 (1254) H     0000 FoptimalDc                                : 0
+ 0x04e8 (1256) H     0000 FoptimalAc                                : 0
+ 0x04ea (1258) H     0000 Padding2                                  : 0
+ 0x04ec (1260) B       00 Padding                                   : 0
+ 0x04ed (1261) B       00 SnapToDiscrete                            : 0
+ 0x04ee (1262) B       02 NumDiscreteLevels                         : 2
+ 0x04ef (1263) B       00 CalculateFopt                             : 0
+ 0x04f0 (1264) f 508d673f m                                         : 0.9045
+ 0x04f4 (1268) f b7d140be b                                         :-0.1883
+ 0x04f8 (1272) I 00000000 Padding3                                  : 0
+ 0x04fc (1276) I 00000000 Padding3                                  : 0
+ 0x0500 (1280) I 00000000 Padding3                                  : 0
+ 0x0504 (1284) H     0000 Padding4                                  : 0
+ 0x0506 (1286) H     0000 FoptimalDc                                : 0
+ 0x0508 (1288) H     0000 FoptimalAc                                : 0
+ 0x050a (1290) H     0000 Padding2                                  : 0
+ 0x050c (1292) B       00 Padding                                   : 0
+ 0x050d (1293) B       00 SnapToDiscrete                            : 0
+ 0x050e (1294) B       02 NumDiscreteLevels                         : 2
+ 0x050f (1295) B       00 CalculateFopt                             : 0
+ 0x0510 (1296) f 789c823f m                                         : 1.0204
+ 0x0514 (1300) f a01aaf3e b                                         : 0.342
+ 0x0518 (1304) I 00000000 Padding3                                  : 0
+ 0x051c (1308) I 00000000 Padding3                                  : 0
+ 0x0520 (1312) I 00000000 Padding3                                  : 0
+ 0x0524 (1316) H     0000 Padding4                                  : 0
+ 0x0526 (1318) H     0000 FoptimalDc                                : 0
+ 0x0528 (1320) H     0000 FoptimalAc                                : 0
+ 0x052a (1322) H     0000 Padding2                                  : 0
+ 0x052c (1324) B       00 Padding                                   : 0
+ 0x052d (1325) B       00 SnapToDiscrete                            : 0
+ 0x052e (1326) B       02 NumDiscreteLevels                         : 2
+ 0x052f (1327) B       00 CalculateFopt                             : 0
+ 0x0530 (1328) f 508d673f m                                         : 0.9045
+ 0x0534 (1332) f b7d140be b                                         :-0.1883
+ 0x0538 (1336) I 00000000 Padding3                                  : 0
+ 0x053c (1340) I 00000000 Padding3                                  : 0
+ 0x0540 (1344) I 00000000 Padding3                                  : 0
+ 0x0544 (1348) H     0000 Padding4                                  : 0
+ 0x0546 (1350) H     0000 FoptimalDc                                : 0
+ 0x0548 (1352) H     0000 FoptimalAc                                : 0
+ 0x054a (1354) H     0000 Padding2                                  : 0
+ 0x054c (1356) B       00 Padding                                   : 0
+ 0x054d (1357) B       00 SnapToDiscrete                            : 0
+ 0x054e (1358) B       02 NumDiscreteLevels                         : 2
+ 0x054f (1359) B       00 CalculateFopt                             : 0
+ 0x0550 (1360) f fed4483f m                                         : 0.7845
+ 0x0554 (1364) f dbf93e3f b                                         : 0.746
+ 0x0558 (1368) I 00000000 Padding3                                  : 0
+ 0x055c (1372) I 00000000 Padding3                                  : 0
+ 0x0560 (1376) I 00000000 Padding3                                  : 0
+ 0x0564 (1380) H     0000 Padding4                                  : 0
+ 0x0566 (1382) H     0000 FoptimalDc                                : 0
+ 0x0568 (1384) H     0000 FoptimalAc                                : 0
+ 0x056a (1386) H     0000 Padding2                                  : 0
+ 0x056c (1388) B       00 Padding                                   : 0
+ 0x056d (1389) B       00 SnapToDiscrete                            : 0
+ 0x056e (1390) B       02 NumDiscreteLevels                         : 2
+ 0x056f (1391) B       00 CalculateFopt                             : 0
+ 0x0570 (1392) f fed4483f m                                         : 0.7845
+ 0x0574 (1396) f dbf93e3f b                                         : 0.746
+ 0x0578 (1400) I 00000000 Padding3                                  : 0
+ 0x057c (1404) I 00000000 Padding3                                  : 0
+ 0x0580 (1408) I 00000000 Padding3                                  : 0
+ 0x0584 (1412) H     0000 Padding4                                  : 0
+ 0x0586 (1414) H     0000 FoptimalDc                                : 0
+ 0x0588 (1416) H     0000 FoptimalAc                                : 0
+ 0x058a (1418) H     0000 Padding2                                  : 0
+ 0x058c (1420) B       00 Padding                                   : 0
+ 0x058d (1421) B       00 SnapToDiscrete                            : 0
+ 0x058e (1422) B       02 NumDiscreteLevels                         : 2
+ 0x058f (1423) B       00 CalculateFopt                             : 0
+ 0x0590 (1424) f 986ea23f m                                         : 1.269
+ 0x0594 (1428) f 1283403e b                                         : 0.188
+ 0x0598 (1432) I 00000000 Padding3                                  : 0
+ 0x059c (1436) I 00000000 Padding3                                  : 0
+ 0x05a0 (1440) I 00000000 Padding3                                  : 0
+ 0x05a4 (1444) H     0000 Padding4                                  : 0
+ 0x05a6 (1446) H     0000 FoptimalDc                                : 0
+ 0x05a8 (1448) H     0000 FoptimalAc                                : 0
+ 0x05aa (1450) H     0000 Padding2                                  : 0
+ 0x05ac (1452) B       00 Padding                                   : 0
+ 0x05ad (1453) B       00 SnapToDiscrete                            : 0
+ 0x05ae (1454) B       02 NumDiscreteLevels                         : 2
+ 0x05af (1455) B       00 CalculateFopt                             : 0
+ 0x05b0 (1456) f f2d28d3f m                                         : 1.108
+ 0x05b4 (1460) f 7b140e3f b                                         : 0.555
+ 0x05b8 (1464) I 00000000 Padding3                                  : 0
+ 0x05bc (1468) I 00000000 Padding3                                  : 0
+ 0x05c0 (1472) I 00000000 Padding3                                  : 0
+ 0x05c4 (1476) H     0000 Padding4                                  : 0
+ 0x05c6 (1478) H     0000 FoptimalDc                                : 0
+ 0x05c8 (1480) H     0000 FoptimalAc                                : 0
+ 0x05ca (1482) H     0000 Padding2                                  : 0
+ 0x05cc (1484) B       00 Padding                                   : 0
+ 0x05cd (1485) B       00 SnapToDiscrete                            : 0
+ 0x05ce (1486) B       02 NumDiscreteLevels                         : 2
+ 0x05cf (1487) B       00 CalculateFopt                             : 0
+ 0x05d0 (1488) f 986ea23f m                                         : 1.269
+ 0x05d4 (1492) f 1283403e b                                         : 0.188
+ 0x05d8 (1496) I 00000000 Padding3                                  : 0
+ 0x05dc (1500) I 00000000 Padding3                                  : 0
+ 0x05e0 (1504) I f401d007 Padding3                                  : 131072500
+ 0x05e4 (1508) H     0000 Padding4                                  : 0
+ 0x05e6 (1510) H     0000 FoptimalDc                                : 0
+ 0x05e8 (1512) H     0000 FoptimalAc                                : 0
+ 0x05ea (1514) H     0000 Padding2                                  : 0
+ 0x05ec (1516) H     f401 FreqTableGfx                              : 500
+ 0x05ee (1518) H     920c FreqTableGfx                              : 3218
+ 0x05f0 (1520) H     0000 FreqTableGfx                              : 0
+ 0x05f2 (1522) H     0000 FreqTableGfx                              : 0
+ 0x05f4 (1524) H     0000 FreqTableGfx                              : 0
+ 0x05f6 (1526) H     0000 FreqTableGfx                              : 0
+ 0x05f8 (1528) H     0000 FreqTableGfx                              : 0
+ 0x05fa (1530) H     0000 FreqTableGfx                              : 0
+ 0x05fc (1532) H     0000 FreqTableGfx                              : 0
+ 0x05fe (1534) H     0000 FreqTableGfx                              : 0
+ 0x0600 (1536) H     0000 FreqTableGfx                              : 0
+ 0x0602 (1538) H     0000 FreqTableGfx                              : 0
+ 0x0604 (1540) H     0000 FreqTableGfx                              : 0
+ 0x0606 (1542) H     0000 FreqTableGfx                              : 0
+ 0x0608 (1544) H     0000 FreqTableGfx                              : 0
+ 0x060a (1546) H     0000 FreqTableGfx                              : 0
+ 0x060c (1548) H     0102 FreqTableVclk                             : 513
+ 0x060e (1550) H     760b FreqTableVclk                             : 2934
+ 0x0610 (1552) H     0000 FreqTableVclk                             : 0
+ 0x0612 (1554) H     0000 FreqTableVclk                             : 0
+ 0x0614 (1556) H     0000 FreqTableVclk                             : 0
+ 0x0616 (1558) H     0000 FreqTableVclk                             : 0
+ 0x0618 (1560) H     0000 FreqTableVclk                             : 0
+ 0x061a (1562) H     0000 FreqTableVclk                             : 0
+ 0x061c (1564) H     0102 FreqTableDclk                             : 513
+ 0x061e (1566) H     9808 FreqTableDclk                             : 2200
+ 0x0620 (1568) H     0000 FreqTableDclk                             : 0
+ 0x0622 (1570) H     0000 FreqTableDclk                             : 0
+ 0x0624 (1572) H     0000 FreqTableDclk                             : 0
+ 0x0626 (1574) H     0000 FreqTableDclk                             : 0
+ 0x0628 (1576) H     0000 FreqTableDclk                             : 0
+ 0x062a (1578) H     0000 FreqTableDclk                             : 0
+ 0x062c (1580) H     f401 FreqTableSocclk                           : 500
+ 0x062e (1582) H     dc05 FreqTableSocclk                           : 1500
+ 0x0630 (1584) H     6100 FreqTableSocclk                           : 97
+ 0x0632 (1586) H     c901 FreqTableSocclk                           : 457
+ 0x0634 (1588) H     ad02 FreqTableSocclk                           : 685
+ 0x0636 (1590) H     e803 FreqTableSocclk                           : 1000
+ 0x0638 (1592) H     0000 FreqTableSocclk                           : 0
+ 0x063a (1594) H     0000 FreqTableSocclk                           : 0
+ 0x063c (1596) H     6100 FreqTableUclk                             : 97
+ 0x063e (1598) H     c901 FreqTableUclk                             : 457
+ 0x0640 (1600) H     0503 FreqTableUclk                             : 773
+ 0x0642 (1602) H     e204 FreqTableUclk                             : 1250
+ 0x0644 (1604) H     9400 FreqTableDispclk                          : 148
+ 0x0646 (1606) H     6608 FreqTableDispclk                          : 2150
+ 0x0648 (1608) H     0000 FreqTableDispclk                          : 0
+ 0x064a (1610) H     0000 FreqTableDispclk                          : 0
+ 0x064c (1612) H     0000 FreqTableDispclk                          : 0
+ 0x064e (1614) H     0000 FreqTableDispclk                          : 0
+ 0x0650 (1616) H     0000 FreqTableDispclk                          : 0
+ 0x0652 (1618) H     0000 FreqTableDispclk                          : 0
+ 0x0654 (1620) H     9400 FreqTableDppClk                           : 148
+ 0x0656 (1622) H     6608 FreqTableDppClk                           : 2150
+ 0x0658 (1624) H     0000 FreqTableDppClk                           : 0
+ 0x065a (1626) H     0000 FreqTableDppClk                           : 0
+ 0x065c (1628) H     0000 FreqTableDppClk                           : 0
+ 0x065e (1630) H     0000 FreqTableDppClk                           : 0
+ 0x0660 (1632) H     0000 FreqTableDppClk                           : 0
+ 0x0662 (1634) H     0000 FreqTableDppClk                           : 0
+ 0x0664 (1636) H     cd02 FreqTableDprefclk                         : 717
+ 0x0666 (1638) H     cd02 FreqTableDprefclk                         : 717
+ 0x0668 (1640) H     0000 FreqTableDprefclk                         : 0
+ 0x066a (1642) H     0000 FreqTableDprefclk                         : 0
+ 0x066c (1644) H     0000 FreqTableDprefclk                         : 0
+ 0x066e (1646) H     0000 FreqTableDprefclk                         : 0
+ 0x0670 (1648) H     0000 FreqTableDprefclk                         : 0
+ 0x0672 (1650) H     0000 FreqTableDprefclk                         : 0
+ 0x0674 (1652) H     9400 FreqTableDcfclk                           : 148
+ 0x0676 (1654) H     1c06 FreqTableDcfclk                           : 1564
+ 0x0678 (1656) H     0000 FreqTableDcfclk                           : 0
+ 0x067a (1658) H     0000 FreqTableDcfclk                           : 0
+ 0x067c (1660) H     0000 FreqTableDcfclk                           : 0
+ 0x067e (1662) H     0000 FreqTableDcfclk                           : 0
+ 0x0680 (1664) H     0000 FreqTableDcfclk                           : 0
+ 0x0682 (1666) H     0000 FreqTableDcfclk                           : 0
+ 0x0684 (1668) H     9400 FreqTableDtbclk                           : 148
+ 0x0686 (1670) H     1c06 FreqTableDtbclk                           : 1564
+ 0x0688 (1672) H     0000 FreqTableDtbclk                           : 0
+ 0x068a (1674) H     0000 FreqTableDtbclk                           : 0
+ 0x068c (1676) H     0000 FreqTableDtbclk                           : 0
+ 0x068e (1678) H     0000 FreqTableDtbclk                           : 0
+ 0x0690 (1680) H     0000 FreqTableDtbclk                           : 0
+ 0x0692 (1682) H     0000 FreqTableDtbclk                           : 0
+ 0x0694 (1684) H     5802 FreqTableFclk                             : 600
+ 0x0696 (1686) H     e803 FreqTableFclk                             : 1000
+ 0x0698 (1688) H     b004 FreqTableFclk                             : 1200
+ 0x069a (1690) H     4006 FreqTableFclk                             : 1600
+ 0x069c (1692) H     d007 FreqTableFclk                             : 2000
+ 0x069e (1694) H     9808 FreqTableFclk                             : 2200
+ 0x06a0 (1696) H     ca08 FreqTableFclk                             : 2250
+ 0x06a2 (1698) H     fc08 FreqTableFclk                             : 2300
+ 0x06a4 (1700) I 920c0000 DcModeMaxFreq                             : 3218
+ 0x06a8 (1704) I dc050000 DcModeMaxFreq                             : 1500
+ 0x06ac (1708) I e2040000 DcModeMaxFreq                             : 1250
+ 0x06b0 (1712) I fc080000 DcModeMaxFreq                             : 2300
+ 0x06b4 (1716) I 98080000 DcModeMaxFreq                             : 2200
+ 0x06b8 (1720) I 760b0000 DcModeMaxFreq                             : 2934
+ 0x06bc (1724) I 98080000 DcModeMaxFreq                             : 2200
+ 0x06c0 (1728) I 760b0000 DcModeMaxFreq                             : 2934
+ 0x06c4 (1732) I 66080000 DcModeMaxFreq                             : 2150
+ 0x06c8 (1736) I 66080000 DcModeMaxFreq                             : 2150
+ 0x06cc (1740) I cd020000 DcModeMaxFreq                             : 717
+ 0x06d0 (1744) I 1c060000 DcModeMaxFreq                             : 1564
+ 0x06d4 (1748) I 1c060000 DcModeMaxFreq                             : 1564
+ 0x06d8 (1752) H     f401 Mp0clkFreq                                : 500
+ 0x06da (1754) H     bc02 Mp0clkFreq                                : 700
+ 0x06dc (1756) H     f00a Mp0DpmVoltage                             : 2800
+ 0x06de (1758) H     800c Mp0DpmVoltage                             : 3200
+ 0x06e0 (1760) B       00 GfxclkSpare                               : 0
+ 0x06e1 (1761) B       00 GfxclkSpare                               : 0
+ 0x06e2 (1762) H     0000 GfxclkFreqCap                             : 0
+ 0x06e4 (1764) H     2003 GfxclkFgfxoffEntry                        : 800
+ 0x06e6 (1766) H     b004 GfxclkFgfxoffExitImu                      : 1200
+ 0x06e8 (1768) H     2003 GfxclkFgfxoffExitRlc                      : 800
+ 0x06ea (1770) H     fa00 GfxclkThrottleClock                       : 250
+ 0x06ec (1772) B       01 EnableGfxPowerStagesGpio                  : 1
+ 0x06ed (1773) B       00 GfxIdlePadding                            : 0
+ 0x06ee (1774) B       01 SmsRepairWRCKClkDivEn                     : 1
+ 0x06ef (1775) B       04 SmsRepairWRCKClkDivVal                    : 4
+ 0x06f0 (1776) B       01 GfxOffEntryEarlyMGCGEn                    : 1
+ 0x06f1 (1777) B       00 GfxOffEntryForceCGCGEn                    : 0
+ 0x06f2 (1778) B       00 GfxOffEntryForceCGCGDelayEn               : 0
+ 0x06f3 (1779) B       00 GfxOffEntryForceCGCGDelayVal              : 0
+ 0x06f4 (1780) H     1405 GfxclkFreqGfxUlv                          : 1300
+ 0x06f6 (1782) B       00 GfxIdlePadding2                           : 0
+ 0x06f7 (1783) B       00 GfxIdlePadding2                           : 0
+ 0x06f8 (1784) I 60ea0000 GfxOffEntryHysteresis                     : 60000
+ 0x06fc (1788) I 00000000 GfxoffSpare                               : 0
+ 0x0700 (1792) I 00000000 GfxoffSpare                               : 0
+ 0x0704 (1796) I 00000000 GfxoffSpare                               : 0
+ 0x0708 (1800) I 00000000 GfxoffSpare                               : 0
+ 0x070c (1804) I 00000000 GfxoffSpare                               : 0
+ 0x0710 (1808) I 00000000 GfxoffSpare                               : 0
+ 0x0714 (1812) I 00000000 GfxoffSpare                               : 0
+ 0x0718 (1816) I 00000000 GfxoffSpare                               : 0
+ 0x071c (1820) I 00000000 GfxoffSpare                               : 0
+ 0x0720 (1824) I 00000000 GfxoffSpare                               : 0
+ 0x0724 (1828) I 00000000 GfxoffSpare                               : 0
+ 0x0728 (1832) I 00000000 GfxoffSpare                               : 0
+ 0x072c (1836) I 00000000 GfxoffSpare                               : 0
+ 0x0730 (1840) I 00000000 GfxoffSpare                               : 0
+ 0x0734 (1844) I 00000000 GfxoffSpare                               : 0
+ 0x0738 (1848) I 0000803f DfllBtcMasterScalerM                      : 1065353216
 ERROR: Unexpected data structure: <class 'int'>
- 0x0740 (1856) I cdcc8c3f DfllBtcSlaveScalerM             : 1066192077
+ 0x0740 (1856) I cdcc8c3f DfllBtcSlaveScalerM                       : 1066192077
 ERROR: Unexpected data structure: <class 'int'>
- 0x0748 (1864) I 64006400 DfllPccAsWaitCtrl               : 6553700
- 0x074c (1868) I 2f841f00 DfllPccAsStepCtrl               : 2065455
- 0x0750 (1872) I 713d8a3f GfxGpoSpare                     : 1066024305
- 0x0754 (1876) I 00000000 GfxGpoSpare                     : 0
- 0x0758 (1880) I 00000000 GfxGpoSpare                     : 0
- 0x075c (1884) I 00000000 GfxGpoSpare                     : 0
- 0x0760 (1888) I 00000000 GfxGpoSpare                     : 0
- 0x0764 (1892) I 00000000 GfxGpoSpare                     : 0
- 0x0768 (1896) I 00000000 GfxGpoSpare                     : 0
- 0x076c (1900) I 00000000 GfxGpoSpare                     : 0
- 0x0770 (1904) I 00000000 GfxGpoSpare                     : 0
- 0x0774 (1908) I 00000000 GfxGpoSpare                     : 0
- 0x0778 (1912) H     0000 DcsGfxOffVoltage                : 0
- 0x077a (1914) H     0000 PaddingDcs                      : 0
- 0x077c (1916) H     0000 DcsMinGfxOffTime                : 0
- 0x077e (1918) H     0000 DcsMaxGfxOffTime                : 0
- 0x0780 (1920) I 00000000 DcsMinCreditAccum               : 0
- 0x0784 (1924) H     0000 DcsExitHysteresis               : 0
- 0x0786 (1926) H     0000 DcsTimeout                      : 0
- 0x0788 (1928) I 00000000 DcsSpare                        : 0
- 0x078c (1932) I 00000000 DcsSpare                        : 0
- 0x0790 (1936) I 00000000 DcsSpare                        : 0
- 0x0794 (1940) I 00000000 DcsSpare                        : 0
- 0x0798 (1944) I 00000000 DcsSpare                        : 0
- 0x079c (1948) I 00000000 DcsSpare                        : 0
- 0x07a0 (1952) I 00000000 DcsSpare                        : 0
- 0x07a4 (1956) I 00000000 DcsSpare                        : 0
- 0x07a8 (1960) I 00000000 DcsSpare                        : 0
- 0x07ac (1964) I 00000000 DcsSpare                        : 0
- 0x07b0 (1968) I 00000000 DcsSpare                        : 0
- 0x07b4 (1972) I 00000000 DcsSpare                        : 0
- 0x07b8 (1976) I 00000000 DcsSpare                        : 0
- 0x07bc (1980) I 00000000 DcsSpare                        : 0
- 0x07c0 (1984) H     6400 ShadowFreqTableUclk             : 100
- 0x07c2 (1986) H     b601 ShadowFreqTableUclk             : 438
- 0x07c4 (1988) H     db02 ShadowFreqTableUclk             : 731
- 0x07c6 (1990) H     a304 ShadowFreqTableUclk             : 1187
- 0x07c8 (1992) B       01 UseStrobeModeOptimizations      : 1
- 0x07c9 (1993) B       0a PaddingMem                      : 10
- 0x07ca (1994) B       f0 PaddingMem                      : 240
- 0x07cb (1995) B       0a PaddingMem                      : 10
- 0x07cc (1996) B       03 UclkDpmPstates                  : 3
- 0x07cd (1997) B       02 UclkDpmPstates                  : 2
- 0x07ce (1998) B       01 UclkDpmPstates                  : 1
- 0x07cf (1999) B       00 UclkDpmPstates                  : 0
- 0x07d0 (2000) B       00 FreqTableUclkDiv                : 0
- 0x07d1 (2001) B       02 FreqTableUclkDiv                : 2
- 0x07d2 (2002) B       03 FreqTableUclkDiv                : 3
- 0x07d3 (2003) B       03 FreqTableUclkDiv                : 3
- 0x07d4 (2004) H     8c0a MemVmempVoltage                 : 2700
- 0x07d6 (2006) H     f00a MemVmempVoltage                 : 2800
- 0x07d8 (2008) H     b80b MemVmempVoltage                 : 3000
- 0x07da (2010) H     800c MemVmempVoltage                 : 3200
- 0x07dc (2012) H     8813 MemVddioVoltage                 : 5000
- 0x07de (2014) H     1815 MemVddioVoltage                 : 5400
- 0x07e0 (2016) H     1815 MemVddioVoltage                 : 5400
- 0x07e2 (2018) H     1815 MemVddioVoltage                 : 5400
- 0x07e4 (2020) B       00 FclkDpmUPstates                 : 0
- 0x07e5 (2021) B       01 FclkDpmUPstates                 : 1
- 0x07e6 (2022) B       02 FclkDpmUPstates                 : 2
- 0x07e7 (2023) B       03 FclkDpmUPstates                 : 3
- 0x07e8 (2024) B       04 FclkDpmUPstates                 : 4
- 0x07e9 (2025) B       05 FclkDpmUPstates                 : 5
- 0x07ea (2026) B       06 FclkDpmUPstates                 : 6
- 0x07eb (2027) B       07 FclkDpmUPstates                 : 7
- 0x07ec (2028) H     b80b FclkDpmVddU                     : 3000
- 0x07ee (2030) H     b80b FclkDpmVddU                     : 3000
- 0x07f0 (2032) H     b80b FclkDpmVddU                     : 3000
- 0x07f2 (2034) H     b80b FclkDpmVddU                     : 3000
- 0x07f4 (2036) H     b80b FclkDpmVddU                     : 3000
- 0x07f6 (2038) H     480d FclkDpmVddU                     : 3400
- 0x07f8 (2040) H     480d FclkDpmVddU                     : 3400
- 0x07fa (2042) H     480d FclkDpmVddU                     : 3400
- 0x07fc (2044) H     6009 FclkDpmUSpeed                   : 2400
- 0x07fe (2046) H     a00f FclkDpmUSpeed                   : 4000
- 0x0800 (2048) H     c012 FclkDpmUSpeed                   : 4800
- 0x0802 (2050) H     0019 FclkDpmUSpeed                   : 6400
- 0x0804 (2052) H     401f FclkDpmUSpeed                   : 8000
- 0x0806 (2054) H     6022 FclkDpmUSpeed                   : 8800
- 0x0808 (2056) H     2823 FclkDpmUSpeed                   : 9000
- 0x080a (2058) H     f023 FclkDpmUSpeed                   : 9200
- 0x080c (2060) H     0000 FclkDpmDisallowPstateFreq       : 0
- 0x080e (2062) H     0000 PaddingFclk                     : 0
- 0x0810 (2064) B       00 PcieGenSpeed                    : 0
- 0x0811 (2065) B       01 PcieGenSpeed                    : 1
- 0x0812 (2066) B       03 PcieGenSpeed                    : 3
- 0x0813 (2067) B       01 PcieLaneCount                   : 1
- 0x0814 (2068) B       03 PcieLaneCount                   : 3
- 0x0815 (2069) B       06 PcieLaneCount                   : 6
- 0x0816 (2070) H     4e00 LclkFreq                        : 78
- 0x0818 (2072) H     9c00 LclkFreq                        : 156
- 0x081a (2074) H     6f02 LclkFreq                        : 623
- 0x081c (2076) H     0000 FanStopTemp                     : 0
- 0x081e (2078) H     3200 FanStopTemp                     : 50
- 0x0820 (2080) H     3200 FanStopTemp                     : 50
- 0x0822 (2082) H     3200 FanStopTemp                     : 50
- 0x0824 (2084) H     3c00 FanStopTemp                     : 60
- 0x0826 (2086) H     3200 FanStopTemp                     : 50
- 0x0828 (2088) H     3200 FanStopTemp                     : 50
- 0x082a (2090) H     3200 FanStopTemp                     : 50
- 0x082c (2092) H     3200 FanStopTemp                     : 50
- 0x082e (2094) H     3200 FanStopTemp                     : 50
- 0x0830 (2096) H     0000 FanStopTemp                     : 0
- 0x0832 (2098) H     0000 FanStopTemp                     : 0
- 0x0834 (2100) H     0000 FanStopTemp                     : 0
- 0x0836 (2102) H     0000 FanStartTemp                    : 0
- 0x0838 (2104) H     3c00 FanStartTemp                    : 60
- 0x083a (2106) H     3c00 FanStartTemp                    : 60
- 0x083c (2108) H     3c00 FanStartTemp                    : 60
- 0x083e (2110) H     4600 FanStartTemp                    : 70
- 0x0840 (2112) H     3c00 FanStartTemp                    : 60
- 0x0842 (2114) H     3c00 FanStartTemp                    : 60
- 0x0844 (2116) H     3c00 FanStartTemp                    : 60
- 0x0846 (2118) H     3c00 FanStartTemp                    : 60
- 0x0848 (2120) H     3c00 FanStartTemp                    : 60
- 0x084a (2122) H     0000 FanStartTemp                    : 0
- 0x084c (2124) H     0000 FanStartTemp                    : 0
- 0x084e (2126) H     0000 FanStartTemp                    : 0
- 0x0850 (2128) H     0000 FanGain                         : 0
- 0x0852 (2130) H     9001 FanGain                         : 400
- 0x0854 (2132) H     9001 FanGain                         : 400
- 0x0856 (2134) H     9001 FanGain                         : 400
- 0x0858 (2136) H     9001 FanGain                         : 400
- 0x085a (2138) H     9001 FanGain                         : 400
- 0x085c (2140) H     9001 FanGain                         : 400
- 0x085e (2142) H     9001 FanGain                         : 400
- 0x0860 (2144) H     9001 FanGain                         : 400
- 0x0862 (2146) H     9001 FanGain                         : 400
- 0x0864 (2148) H     0000 FanGain                         : 0
- 0x0866 (2150) H     0000 FanGain                         : 0
- 0x0868 (2152) H     0000 FanGain                         : 0
- 0x086a (2154) H     2413 FanGainPadding                  : 4900
- 0x086c (2156) H     0f00 FanPwmMin                       : 15
- 0x086e (2158) H     4006 AcousticTargetRpmThreshold      : 1600
- 0x0870 (2160) H     e40c AcousticLimitRpmThreshold       : 3300
- 0x0872 (2162) H     e40c FanMaximumRpm                   : 3300
- 0x0874 (2164) H     b80b MGpuAcousticLimitRpmThreshold   : 3000
- 0x0876 (2166) H     f401 FanTargetGfxclk                 : 500
- 0x0878 (2168) I f2030000 TempInputSelectMask             : 1010
- 0x087c (2172) B       01 FanZeroRpmEnable                : 1
- 0x087d (2173) B       02 FanTachEdgePerRev               : 2
- 0x087e (2174) H     0000 FanTargetTemperature            : 0
- 0x0880 (2176) H     5200 FanTargetTemperature            : 82
- 0x0882 (2178) H     5200 FanTargetTemperature            : 82
- 0x0884 (2180) H     5200 FanTargetTemperature            : 82
- 0x0886 (2182) H     5a00 FanTargetTemperature            : 90
- 0x0888 (2184) H     6400 FanTargetTemperature            : 100
- 0x088a (2186) H     6400 FanTargetTemperature            : 100
- 0x088c (2188) H     6400 FanTargetTemperature            : 100
- 0x088e (2190) H     6400 FanTargetTemperature            : 100
- 0x0890 (2192) H     6400 FanTargetTemperature            : 100
- 0x0892 (2194) H     0000 FanTargetTemperature            : 0
- 0x0894 (2196) H     0000 FanTargetTemperature            : 0
- 0x0896 (2198) H     0000 FanTargetTemperature            : 0
- 0x0898 (2200) h     0000 FuzzyFan_ErrorSetDelta          : 0
- 0x089a (2202) h     0000 FuzzyFan_ErrorRateSetDelta      : 0
- 0x089c (2204) h     0000 FuzzyFan_PwmSetDelta            : 0
- 0x089e (2206) H     7d00 FuzzyFan_Reserved               : 125
- 0x08a0 (2208) H     0000 FwCtfLimit                      : 0
- 0x08a2 (2210) H     7600 FwCtfLimit                      : 118
- 0x08a4 (2212) H     7600 FwCtfLimit                      : 118
- 0x08a6 (2214) H     7600 FwCtfLimit                      : 118
- 0x08a8 (2216) H     7100 FwCtfLimit                      : 113
- 0x08aa (2218) H     7d00 FwCtfLimit                      : 125
- 0x08ac (2220) H     7d00 FwCtfLimit                      : 125
- 0x08ae (2222) H     7d00 FwCtfLimit                      : 125
- 0x08b0 (2224) H     7d00 FwCtfLimit                      : 125
- 0x08b2 (2226) H     7d00 FwCtfLimit                      : 125
- 0x08b4 (2228) H     0000 FwCtfLimit                      : 0
- 0x08b6 (2230) H     0000 FwCtfLimit                      : 0
- 0x08b8 (2232) H     0000 FwCtfLimit                      : 0
- 0x08ba (2234) H     e803 IntakeTempEnableRPM             : 1000
- 0x08bc (2236) h     c800 IntakeTempOffsetTemp            : 200
- 0x08be (2238) H     2d00 IntakeTempReleaseTemp           : 45
- 0x08c0 (2240) H     b80b IntakeTempHighIntakeAcousticLimit: 3000
- 0x08c2 (2242) H     6400 IntakeTempAcouticLimitReleaseRate: 100
- 0x08c4 (2244) h     ecff FanAbnormalTempLimitOffset      :-20
- 0x08c6 (2246) H     fa00 FanStalledTriggerRpm            : 250
- 0x08c8 (2248) H     5500 FanAbnormalTriggerRpmCoeff      : 85
- 0x08ca (2250) H     0000 FanAbnormalDetectionEnable      : 0
- 0x08cc (2252) B       01 FanIntakeSensorSupport          : 1
- 0x08cd (2253) B       00 FanIntakePadding                : 0
- 0x08ce (2254) B       00 FanIntakePadding                : 0
- 0x08cf (2255) B       00 FanIntakePadding                : 0
- 0x08d0 (2256) I 00000000 FanSpare                        : 0
- 0x08d4 (2260) I 00000000 FanSpare                        : 0
- 0x08d8 (2264) I 00000000 FanSpare                        : 0
- 0x08dc (2268) I 00000000 FanSpare                        : 0
- 0x08e0 (2272) I 00000000 FanSpare                        : 0
- 0x08e4 (2276) I 00000000 FanSpare                        : 0
- 0x08e8 (2280) I 00000000 FanSpare                        : 0
- 0x08ec (2284) I 00000000 FanSpare                        : 0
- 0x08f0 (2288) I 00000000 FanSpare                        : 0
- 0x08f4 (2292) I 00000000 FanSpare                        : 0
- 0x08f8 (2296) I 00000000 FanSpare                        : 0
- 0x08fc (2300) I 00000000 FanSpare                        : 0
- 0x0900 (2304) I 00000000 FanSpare                        : 0
- 0x0904 (2308) B       00 OverrideGfxAvfsFuses            : 0
- 0x0905 (2309) B       00 GfxAvfsPadding                  : 0
- 0x0906 (2310) B       00 GfxAvfsPadding                  : 0
- 0x0907 (2311) B       00 GfxAvfsPadding                  : 0
- 0x0908 (2312) I 00000001 L2HwRtAvfsFuses                 : 16777216
- 0x090c (2316) I 00000001 L2HwRtAvfsFuses                 : 16777216
- 0x0910 (2320) I 00000001 L2HwRtAvfsFuses                 : 16777216
- 0x0914 (2324) I 00000001 L2HwRtAvfsFuses                 : 16777216
- 0x0918 (2328) I 00000001 L2HwRtAvfsFuses                 : 16777216
- 0x091c (2332) I 40050002 L2HwRtAvfsFuses                 : 33555776
- 0x0920 (2336) I 00100000 L2HwRtAvfsFuses                 : 4096
- 0x0924 (2340) I 40050002 L2HwRtAvfsFuses                 : 33555776
- 0x0928 (2344) I 00100000 L2HwRtAvfsFuses                 : 4096
- 0x092c (2348) I 40050002 L2HwRtAvfsFuses                 : 33555776
- 0x0930 (2352) I 00100000 L2HwRtAvfsFuses                 : 4096
- 0x0934 (2356) I 40050002 L2HwRtAvfsFuses                 : 33555776
- 0x0938 (2360) I 00100000 L2HwRtAvfsFuses                 : 4096
- 0x093c (2364) I 40050002 L2HwRtAvfsFuses                 : 33555776
- 0x0940 (2368) I 00100000 L2HwRtAvfsFuses                 : 4096
- 0x0944 (2372) I e7001301 L2HwRtAvfsFuses                 : 18022631
- 0x0948 (2376) I 34013101 L2HwRtAvfsFuses                 : 19988788
- 0x094c (2380) I 80015801 L2HwRtAvfsFuses                 : 22544768
- 0x0950 (2384) I cd018b01 L2HwRtAvfsFuses                 : 25887181
- 0x0954 (2388) I 00000000 L2HwRtAvfsFuses                 : 0
- 0x0958 (2392) I 00000000 L2HwRtAvfsFuses                 : 0
- 0x095c (2396) I 00000000 L2HwRtAvfsFuses                 : 0
- 0x0960 (2400) I 00000000 L2HwRtAvfsFuses                 : 0
- 0x0964 (2404) I 00000000 L2HwRtAvfsFuses                 : 0
- 0x0968 (2408) I 00000000 L2HwRtAvfsFuses                 : 0
- 0x096c (2412) I 00000000 L2HwRtAvfsFuses                 : 0
- 0x0970 (2416) I 00000000 L2HwRtAvfsFuses                 : 0
- 0x0974 (2420) I 00000000 L2HwRtAvfsFuses                 : 0
- 0x0978 (2424) I 10801080 L2HwRtAvfsFuses                 : 2148565008
- 0x097c (2428) I 10801080 L2HwRtAvfsFuses                 : 2148565008
- 0x0980 (2432) I 10800000 L2HwRtAvfsFuses                 : 32784
- 0x0984 (2436) I ffff0000 L2HwRtAvfsFuses                 : 65535
- 0x0988 (2440) I 00000001 SeHwRtAvfsFuses                 : 16777216
- 0x098c (2444) I 00000001 SeHwRtAvfsFuses                 : 16777216
- 0x0990 (2448) I 00000001 SeHwRtAvfsFuses                 : 16777216
- 0x0994 (2452) I 00000001 SeHwRtAvfsFuses                 : 16777216
- 0x0998 (2456) I 00000001 SeHwRtAvfsFuses                 : 16777216
- 0x099c (2460) I 40050002 SeHwRtAvfsFuses                 : 33555776
- 0x09a0 (2464) I 00100000 SeHwRtAvfsFuses                 : 4096
- 0x09a4 (2468) I 40050002 SeHwRtAvfsFuses                 : 33555776
- 0x09a8 (2472) I 00100000 SeHwRtAvfsFuses                 : 4096
- 0x09ac (2476) I 40050002 SeHwRtAvfsFuses                 : 33555776
- 0x09b0 (2480) I 00100000 SeHwRtAvfsFuses                 : 4096
- 0x09b4 (2484) I 40050002 SeHwRtAvfsFuses                 : 33555776
- 0x09b8 (2488) I 00100000 SeHwRtAvfsFuses                 : 4096
- 0x09bc (2492) I 40050002 SeHwRtAvfsFuses                 : 33555776
- 0x09c0 (2496) I 00100000 SeHwRtAvfsFuses                 : 4096
- 0x09c4 (2500) I e7001301 SeHwRtAvfsFuses                 : 18022631
- 0x09c8 (2504) I 34013101 SeHwRtAvfsFuses                 : 19988788
- 0x09cc (2508) I 80015801 SeHwRtAvfsFuses                 : 22544768
- 0x09d0 (2512) I cd018b01 SeHwRtAvfsFuses                 : 25887181
- 0x09d4 (2516) I 00000000 SeHwRtAvfsFuses                 : 0
- 0x09d8 (2520) I 00000000 SeHwRtAvfsFuses                 : 0
- 0x09dc (2524) I 00000000 SeHwRtAvfsFuses                 : 0
- 0x09e0 (2528) I 00000000 SeHwRtAvfsFuses                 : 0
- 0x09e4 (2532) I 00000000 SeHwRtAvfsFuses                 : 0
- 0x09e8 (2536) I 00000000 SeHwRtAvfsFuses                 : 0
- 0x09ec (2540) I 00000000 SeHwRtAvfsFuses                 : 0
- 0x09f0 (2544) I 00000000 SeHwRtAvfsFuses                 : 0
- 0x09f4 (2548) I 00000000 SeHwRtAvfsFuses                 : 0
- 0x09f8 (2552) I 10801080 SeHwRtAvfsFuses                 : 2148565008
- 0x09fc (2556) I 10801080 SeHwRtAvfsFuses                 : 2148565008
- 0x0a00 (2560) I 10800000 SeHwRtAvfsFuses                 : 32784
- 0x0a04 (2564) I ffff0000 SeHwRtAvfsFuses                 : 65535
- 0x0a08 (2568) I bc020000 CommonRtAvfs                    : 700
- 0x0a0c (2572) I bc020000 CommonRtAvfs                    : 700
- 0x0a10 (2576) I bc020000 CommonRtAvfs                    : 700
- 0x0a14 (2580) I bc020000 CommonRtAvfs                    : 700
- 0x0a18 (2584) I bc020000 CommonRtAvfs                    : 700
- 0x0a1c (2588) I bc020000 CommonRtAvfs                    : 700
- 0x0a20 (2592) I bc020000 CommonRtAvfs                    : 700
- 0x0a24 (2596) I bc020000 CommonRtAvfs                    : 700
- 0x0a28 (2600) I 00000000 CommonRtAvfs                    : 0
- 0x0a2c (2604) I aa020000 CommonRtAvfs                    : 682
- 0x0a30 (2608) I aa020000 CommonRtAvfs                    : 682
- 0x0a34 (2612) I aa020000 CommonRtAvfs                    : 682
- 0x0a38 (2616) I aa020000 CommonRtAvfs                    : 682
- 0x0a3c (2620) I 00000000 L2FwRtAvfsFuses                 : 0
- 0x0a40 (2624) I 00000000 L2FwRtAvfsFuses                 : 0
- 0x0a44 (2628) I 00000000 L2FwRtAvfsFuses                 : 0
- 0x0a48 (2632) I 00000000 L2FwRtAvfsFuses                 : 0
- 0x0a4c (2636) I 00000000 L2FwRtAvfsFuses                 : 0
- 0x0a50 (2640) I 00000000 L2FwRtAvfsFuses                 : 0
- 0x0a54 (2644) I 00000000 L2FwRtAvfsFuses                 : 0
- 0x0a58 (2648) I 00000000 L2FwRtAvfsFuses                 : 0
- 0x0a5c (2652) I 00000000 L2FwRtAvfsFuses                 : 0
- 0x0a60 (2656) I 00000000 L2FwRtAvfsFuses                 : 0
- 0x0a64 (2660) I 00000000 L2FwRtAvfsFuses                 : 0
- 0x0a68 (2664) I 00000000 L2FwRtAvfsFuses                 : 0
- 0x0a6c (2668) I 32000000 L2FwRtAvfsFuses                 : 50
- 0x0a70 (2672) I b80b0000 L2FwRtAvfsFuses                 : 3000
- 0x0a74 (2676) I 02060000 L2FwRtAvfsFuses                 : 1538
- 0x0a78 (2680) I 02060000 L2FwRtAvfsFuses                 : 1538
- 0x0a7c (2684) I 02060000 L2FwRtAvfsFuses                 : 1538
- 0x0a80 (2688) I 02060000 L2FwRtAvfsFuses                 : 1538
- 0x0a84 (2692) I 02060000 L2FwRtAvfsFuses                 : 1538
- 0x0a88 (2696) I 00000000 SeFwRtAvfsFuses                 : 0
- 0x0a8c (2700) I 00000000 SeFwRtAvfsFuses                 : 0
- 0x0a90 (2704) I 00000000 SeFwRtAvfsFuses                 : 0
- 0x0a94 (2708) I 00000000 SeFwRtAvfsFuses                 : 0
- 0x0a98 (2712) I 00000000 SeFwRtAvfsFuses                 : 0
- 0x0a9c (2716) I 00000000 SeFwRtAvfsFuses                 : 0
- 0x0aa0 (2720) I 00000000 SeFwRtAvfsFuses                 : 0
- 0x0aa4 (2724) I 00000000 SeFwRtAvfsFuses                 : 0
- 0x0aa8 (2728) I 00000000 SeFwRtAvfsFuses                 : 0
- 0x0aac (2732) I 00000000 SeFwRtAvfsFuses                 : 0
- 0x0ab0 (2736) I 00000000 SeFwRtAvfsFuses                 : 0
- 0x0ab4 (2740) I 00000000 SeFwRtAvfsFuses                 : 0
- 0x0ab8 (2744) I 32000000 SeFwRtAvfsFuses                 : 50
- 0x0abc (2748) I b80b0000 SeFwRtAvfsFuses                 : 3000
- 0x0ac0 (2752) I 02060000 SeFwRtAvfsFuses                 : 1538
- 0x0ac4 (2756) I 02060000 SeFwRtAvfsFuses                 : 1538
- 0x0ac8 (2760) I 02060000 SeFwRtAvfsFuses                 : 1538
- 0x0acc (2764) I 02060000 SeFwRtAvfsFuses                 : 1538
- 0x0ad0 (2768) I 02060000 SeFwRtAvfsFuses                 : 1538
- 0x0ad4 (2772) f 00000000 Droop_PWL_F                     : 0
- 0x0ad8 (2776) f 00000040 Droop_PWL_F                     : 2
- 0x0adc (2780) f 00002040 Droop_PWL_F                     : 2.5
- 0x0ae0 (2784) f 00004040 Droop_PWL_F                     : 3
- 0x0ae4 (2788) f 00006040 Droop_PWL_F                     : 3.5
- 0x0ae8 (2792) f df32a73d Droop_PWL_a                     : 0.08164
- 0x0aec (2796) f df32a73d Droop_PWL_a                     : 0.08164
- 0x0af0 (2800) f df32a73d Droop_PWL_a                     : 0.08164
- 0x0af4 (2804) f df32a73d Droop_PWL_a                     : 0.08164
- 0x0af8 (2808) f df32a73d Droop_PWL_a                     : 0.08164
- 0x0afc (2812) f 1c42953d Droop_PWL_b                     : 0.07288
- 0x0b00 (2816) f 1c42953d Droop_PWL_b                     : 0.07288
- 0x0b04 (2820) f 7250c23d Droop_PWL_b                     : 0.09488
- 0x0b08 (2824) f 1c42953d Droop_PWL_b                     : 0.07288
- 0x0b0c (2828) f 1c42953d Droop_PWL_b                     : 0.07288
- 0x0b10 (2832) f 0d8ed2bd Droop_PWL_c                     :-0.10281
- 0x0b14 (2836) f 0d8ed2bd Droop_PWL_c                     :-0.10281
- 0x0b18 (2840) f a0e002be Droop_PWL_c                     :-0.12781
- 0x0b1c (2844) f f2ea1cbd Droop_PWL_c                     :-0.03831
- 0x0b20 (2848) f f2ea1cbd Droop_PWL_c                     :-0.03831
- 0x0b24 (2852) I 0ad7233c Static_PWL_Offset               : 1008981770
- 0x0b28 (2856) I 0ad7233c Static_PWL_Offset               : 1008981770
- 0x0b2c (2860) I 0ad7233c Static_PWL_Offset               : 1008981770
- 0x0b30 (2864) I 0ad7233c Static_PWL_Offset               : 1008981770
- 0x0b34 (2868) I 0ad7233c Static_PWL_Offset               : 1008981770
- 0x0b38 (2872) I 00000000 GbV_dT_vmin                     : 0
- 0x0b3c (2876) I 00000000 GbV_dT_vmax                     : 0
- 0x0b40 (2880) I 58020000 V2F_vmin_range_low              : 600
- 0x0b44 (2884) I bc020000 V2F_vmin_range_high             : 700
- 0x0b48 (2888) I 4c040000 V2F_vmax_range_low              : 1100
- 0x0b4c (2892) I b0040000 V2F_vmax_range_high             : 1200
- 0x0b50 (2896) B       00 DcBtcEnabled                    : 0
- 0x0b51 (2897) B       00 Padding                         : 0
- 0x0b52 (2898) B       00 Padding                         : 0
- 0x0b53 (2899) B       00 Padding                         : 0
- 0x0b54 (2900) H     1800 DcTol                           : 24
- 0x0b56 (2902) H     0000 DcBtcGb                         : 0
- 0x0b58 (2904) H     0000 DcBtcMin                        : 0
- 0x0b5a (2906) H     0000 DcBtcMax                        : 0
- 0x0b5c (2908) f 00000000 m                               : 0
- 0x0b60 (2912) f 00000000 b                               : 0
- 0x0b64 (2916) I 00000000 GfxAvfsSpare                    : 0
- 0x0b68 (2920) I 00000000 GfxAvfsSpare                    : 0
- 0x0b6c (2924) I 00000000 GfxAvfsSpare                    : 0
- 0x0b70 (2928) I 00000000 GfxAvfsSpare                    : 0
- 0x0b74 (2932) I 00000000 GfxAvfsSpare                    : 0
- 0x0b78 (2936) I 00000000 GfxAvfsSpare                    : 0
- 0x0b7c (2940) I 00000000 GfxAvfsSpare                    : 0
- 0x0b80 (2944) I 00000000 GfxAvfsSpare                    : 0
- 0x0b84 (2948) I 00000000 GfxAvfsSpare                    : 0
- 0x0b88 (2952) I 00000000 GfxAvfsSpare                    : 0
- 0x0b8c (2956) I 00000000 GfxAvfsSpare                    : 0
- 0x0b90 (2960) I 00000000 GfxAvfsSpare                    : 0
- 0x0b94 (2964) I 00000000 GfxAvfsSpare                    : 0
- 0x0b98 (2968) I 00000000 GfxAvfsSpare                    : 0
- 0x0b9c (2972) I 00000000 GfxAvfsSpare                    : 0
- 0x0ba0 (2976) I 00000000 GfxAvfsSpare                    : 0
- 0x0ba4 (2980) I 00000000 GfxAvfsSpare                    : 0
- 0x0ba8 (2984) I 00000000 GfxAvfsSpare                    : 0
- 0x0bac (2988) I 00000000 GfxAvfsSpare                    : 0
- 0x0bb0 (2992) I 00000000 GfxAvfsSpare                    : 0
- 0x0bb4 (2996) I 00000000 GfxAvfsSpare                    : 0
- 0x0bb8 (3000) I 00000000 GfxAvfsSpare                    : 0
- 0x0bbc (3004) I 00000000 GfxAvfsSpare                    : 0
- 0x0bc0 (3008) I 00000000 GfxAvfsSpare                    : 0
- 0x0bc4 (3012) I 00000000 GfxAvfsSpare                    : 0
- 0x0bc8 (3016) I 00000000 GfxAvfsSpare                    : 0
- 0x0bcc (3020) I 00000000 GfxAvfsSpare                    : 0
- 0x0bd0 (3024) I 00000000 GfxAvfsSpare                    : 0
- 0x0bd4 (3028) I 00000000 GfxAvfsSpare                    : 0
- 0x0bd8 (3032) I 00000000 GfxAvfsSpare                    : 0
- 0x0bdc (3036) I 00000000 GfxAvfsSpare                    : 0
- 0x0be0 (3040) I 00000000 GfxAvfsSpare                    : 0
- 0x0be4 (3044) B       00 OverrideSocAvfsFuses            : 0
- 0x0be5 (3045) B       01 MinSocAvfsRevision              : 1
- 0x0be6 (3046) B       00 SocAvfsPadding                  : 0
- 0x0be7 (3047) B       00 SocAvfsPadding                  : 0
- 0x0be8 (3048) H     0000 AvfsTemp                        : 0
- 0x0bea (3050) H     5500 AvfsTemp                        : 85
- 0x0bec (3052) H     2c01 VftFMin                         : 300
- 0x0bee (3054) H     f00a VInversion                      : 2800
- 0x0bf0 (3056) f dcd7013d a                               : 0.0317
- 0x0bf4 (3060) f 399c793d b                               : 0.06094
- 0x0bf8 (3064) f 5e80ed3e c                               : 0.46387
- 0x0bfc (3068) f d8b6283d a                               : 0.04119
- 0x0c00 (3072) f e223623d b                               : 0.05521
- 0x0c04 (3076) f a1dbdb3e c                               : 0.42941
- 0x0c08 (3080) f 00000000 a                               : 0
- 0x0c0c (3084) f 00000000 b                               : 0
- 0x0c10 (3088) f a69b443d c                               : 0.048
- 0x0c14 (3092) f 00000000 a                               : 0
- 0x0c18 (3096) f 00000000 b                               : 0
- 0x0c1c (3100) f 00000000 c                               : 0
- 0x0c20 (3104) H     0000 AvfsTemp                        : 0
- 0x0c22 (3106) H     5500 AvfsTemp                        : 85
- 0x0c24 (3108) H     2c01 VftFMin                         : 300
- 0x0c26 (3110) H     f00a VInversion                      : 2800
- 0x0c28 (3112) f dcd7013d a                               : 0.0317
- 0x0c2c (3116) f 399c793d b                               : 0.06094
- 0x0c30 (3120) f 5e80ed3e c                               : 0.46387
- 0x0c34 (3124) f d8b6283d a                               : 0.04119
- 0x0c38 (3128) f e223623d b                               : 0.05521
- 0x0c3c (3132) f a1dbdb3e c                               : 0.42941
- 0x0c40 (3136) f 00000000 a                               : 0
- 0x0c44 (3140) f 00000000 b                               : 0
- 0x0c48 (3144) f a69b443d c                               : 0.048
- 0x0c4c (3148) f 00000000 a                               : 0
- 0x0c50 (3152) f 00000000 b                               : 0
- 0x0c54 (3156) f 00000000 c                               : 0
- 0x0c58 (3160) H     0000 AvfsTemp                        : 0
- 0x0c5a (3162) H     5500 AvfsTemp                        : 85
- 0x0c5c (3164) H     2c01 VftFMin                         : 300
- 0x0c5e (3166) H     f00a VInversion                      : 2800
- 0x0c60 (3168) f dcd7013d a                               : 0.0317
- 0x0c64 (3172) f 399c793d b                               : 0.06094
- 0x0c68 (3176) f 5e80ed3e c                               : 0.46387
- 0x0c6c (3180) f d8b6283d a                               : 0.04119
- 0x0c70 (3184) f e223623d b                               : 0.05521
- 0x0c74 (3188) f a1dbdb3e c                               : 0.42941
- 0x0c78 (3192) f 00000000 a                               : 0
- 0x0c7c (3196) f 00000000 b                               : 0
- 0x0c80 (3200) f a69b443d c                               : 0.048
- 0x0c84 (3204) f 00000000 a                               : 0
- 0x0c88 (3208) f 00000000 b                               : 0
- 0x0c8c (3212) f 00000000 c                               : 0
- 0x0c90 (3216) f 0000c03f a                               : 1.5
- 0x0c94 (3220) f e4839ebd b                               :-0.0774
- 0x0c98 (3224) f 9cc440bf c                               :-0.753
- 0x0c9c (3228) f 0000c03f a                               : 1.5
- 0x0ca0 (3232) f e4839ebd b                               :-0.0774
- 0x0ca4 (3236) f 9cc440bf c                               :-0.753
- 0x0ca8 (3240) f 0000c03f a                               : 1.5
- 0x0cac (3244) f e4839ebd b                               :-0.0774
- 0x0cb0 (3248) f 9cc440bf c                               :-0.753
- 0x0cb4 (3252) f 00000000 m                               : 0
- 0x0cb8 (3256) f 00000000 b                               : 0
- 0x0cbc (3260) f 00000000 m                               : 0
- 0x0cc0 (3264) f 00000000 b                               : 0
- 0x0cc4 (3268) f 00000000 m                               : 0
- 0x0cc8 (3272) f 00000000 b                               : 0
- 0x0ccc (3276) f 00000000 a                               : 0
- 0x0cd0 (3280) f 00000000 b                               : 0
- 0x0cd4 (3284) f 00000000 c                               : 0
- 0x0cd8 (3288) f 00000000 a                               : 0
- 0x0cdc (3292) f 00000000 b                               : 0
- 0x0ce0 (3296) f 00000000 c                               : 0
- 0x0ce4 (3300) f 00000000 a                               : 0
- 0x0ce8 (3304) f 00000000 b                               : 0
- 0x0cec (3308) f 00000000 c                               : 0
- 0x0cf0 (3312) B       01 DcBtcEnabled                    : 1
- 0x0cf1 (3313) B       00 Padding                         : 0
- 0x0cf2 (3314) B       00 Padding                         : 0
- 0x0cf3 (3315) B       00 Padding                         : 0
- 0x0cf4 (3316) H     b400 DcTol                           : 180
- 0x0cf6 (3318) H     1800 DcBtcGb                         : 24
- 0x0cf8 (3320) H     0000 DcBtcMin                        : 0
- 0x0cfa (3322) H     b400 DcBtcMax                        : 180
- 0x0cfc (3324) f 00002040 m                               : 2.5
- 0x0d00 (3328) f 00000000 b                               : 0
- 0x0d04 (3332) B       01 DcBtcEnabled                    : 1
- 0x0d05 (3333) B       00 Padding                         : 0
- 0x0d06 (3334) B       00 Padding                         : 0
- 0x0d07 (3335) B       00 Padding                         : 0
- 0x0d08 (3336) H     b400 DcTol                           : 180
- 0x0d0a (3338) H     1800 DcBtcGb                         : 24
- 0x0d0c (3340) H     0000 DcBtcMin                        : 0
- 0x0d0e (3342) H     b400 DcBtcMax                        : 180
- 0x0d10 (3344) f 00009040 m                               : 4.5
- 0x0d14 (3348) f 00000000 b                               : 0
- 0x0d18 (3352) B       00 DcBtcEnabled                    : 0
- 0x0d19 (3353) B       00 Padding                         : 0
- 0x0d1a (3354) B       00 Padding                         : 0
- 0x0d1b (3355) B       00 Padding                         : 0
- 0x0d1c (3356) H     0000 DcTol                           : 0
- 0x0d1e (3358) H     0000 DcBtcGb                         : 0
- 0x0d20 (3360) H     0000 DcBtcMin                        : 0
- 0x0d22 (3362) H     0000 DcBtcMax                        : 0
- 0x0d24 (3364) f 00000000 m                               : 0
- 0x0d28 (3368) f 00000000 b                               : 0
- 0x0d2c (3372) I 00000000 SocAvfsSpare                    : 0
- 0x0d30 (3376) I 00000000 SocAvfsSpare                    : 0
- 0x0d34 (3380) I 00000000 SocAvfsSpare                    : 0
- 0x0d38 (3384) I 00000000 SocAvfsSpare                    : 0
- 0x0d3c (3388) I 00000000 SocAvfsSpare                    : 0
- 0x0d40 (3392) I 00000000 SocAvfsSpare                    : 0
- 0x0d44 (3396) I 00000000 SocAvfsSpare                    : 0
- 0x0d48 (3400) I 00000000 SocAvfsSpare                    : 0
- 0x0d4c (3404) I 00000000 SocAvfsSpare                    : 0
- 0x0d50 (3408) I 00000000 SocAvfsSpare                    : 0
- 0x0d54 (3412) I 00000000 SocAvfsSpare                    : 0
- 0x0d58 (3416) I 00000000 SocAvfsSpare                    : 0
- 0x0d5c (3420) I 00000000 SocAvfsSpare                    : 0
- 0x0d60 (3424) I 00000000 SocAvfsSpare                    : 0
- 0x0d64 (3428) I 00000000 SocAvfsSpare                    : 0
- 0x0d68 (3432) I 00000000 SocAvfsSpare                    : 0
- 0x0d6c (3436) I 00000000 SocAvfsSpare                    : 0
- 0x0d70 (3440) I 00000000 SocAvfsSpare                    : 0
- 0x0d74 (3444) I 00000000 SocAvfsSpare                    : 0
- 0x0d78 (3448) I 00000000 SocAvfsSpare                    : 0
- 0x0d7c (3452) I 00000000 SocAvfsSpare                    : 0
- 0x0d80 (3456) I 00000000 SocAvfsSpare                    : 0
- 0x0d84 (3460) I 00000000 SocAvfsSpare                    : 0
- 0x0d88 (3464) I 00000000 SocAvfsSpare                    : 0
- 0x0d8c (3468) I 00000000 SocAvfsSpare                    : 0
- 0x0d90 (3472) I 00000000 SocAvfsSpare                    : 0
- 0x0d94 (3476) I 00000000 SocAvfsSpare                    : 0
- 0x0d98 (3480) I 00000000 SocAvfsSpare                    : 0
- 0x0d9c (3484) I 00000000 SocAvfsSpare                    : 0
- 0x0da0 (3488) I 00000000 SocAvfsSpare                    : 0
- 0x0da4 (3492) I 00000000 SocAvfsSpare                    : 0
- 0x0da8 (3496) I 00000000 SocAvfsSpare                    : 0
- 0x0dac (3500) H     b004 InitGfxclk_bypass               : 1200
- 0x0dae (3502) H     5802 InitSocclk                      : 600
- 0x0db0 (3504) H     d002 InitMp0clk                      : 720
- 0x0db2 (3506) H     f401 InitMpioclk                     : 500
- 0x0db4 (3508) H     f401 InitSmnclk                      : 500
- 0x0db6 (3510) H     e803 InitUcpclk                      : 1000
- 0x0db8 (3512) H     9001 InitCsrclk                      : 400
- 0x0dba (3514) H     cd02 InitDprefclk                    : 717
- 0x0dbc (3516) H     9602 InitDcfclk                      : 662
- 0x0dbe (3518) H     0000 InitDtbclk                      : 0
- 0x0dc0 (3520) H     0102 InitDclk                        : 513
- 0x0dc2 (3522) H     0102 InitVclk                        : 513
- 0x0dc4 (3524) H     a002 InitUsbdfsclk                   : 672
- 0x0dc6 (3526) H     fd01 InitMp1clk                      : 509
- 0x0dc8 (3528) H     6f02 InitLclk                        : 623
- 0x0dca (3530) H     9001 InitBaco400clk_bypass           : 400
- 0x0dcc (3532) H     b004 InitBaco1200clk_bypass          : 1200
- 0x0dce (3534) H     bc02 InitBaco700clk_bypass           : 700
- 0x0dd0 (3536) H     e803 InitFclk                        : 1000
- 0x0dd2 (3538) H     0000 InitGfxclk_clkb                 : 0
- 0x0dd4 (3540) B       00 InitUclkDPMState                : 0
- 0x0dd5 (3541) B       00 Padding                         : 0
- 0x0dd6 (3542) B       00 Padding                         : 0
- 0x0dd7 (3543) B       00 Padding                         : 0
- 0x0dd8 (3544) I 94110000 InitVcoFreqPll0                 : 4500
- 0x0ddc (3548) I cc100000 InitVcoFreqPll1                 : 4300
- 0x0de0 (3552) I 00000000 InitVcoFreqPll2                 : 0
- 0x0de4 (3556) I 04100000 InitVcoFreqPll3                 : 4100
- 0x0de8 (3560) I a00f0000 InitVcoFreqPll4                 : 4000
- 0x0dec (3564) I 68100000 InitVcoFreqPll5                 : 4200
- 0x0df0 (3568) I 00000000 InitVcoFreqPll6                 : 0
- 0x0df4 (3572) H     0000 InitGfx                         : 0
- 0x0df6 (3574) H     800c InitSoc                         : 3200
- 0x0df8 (3576) H     480d InitU                           : 3400
- 0x0dfa (3578) H     0000 Padding2                        : 0
- 0x0dfc (3580) I 00000000 Spare                           : 0
- 0x0e00 (3584) I 00000000 Spare                           : 0
- 0x0e04 (3588) I 00000000 Spare                           : 0
- 0x0e08 (3592) I 00000000 Spare                           : 0
- 0x0e0c (3596) I 00000000 Spare                           : 0
- 0x0e10 (3600) I 00000000 Spare                           : 0
- 0x0e14 (3604) I 00000000 Spare                           : 0
- 0x0e18 (3608) I 00000000 Spare                           : 0
- 0x0e1c (3612) H     1b08 BaseClockAc                     : 2075
- 0x0e1e (3614) H     d309 GameClockAc                     : 2515
- 0x0e20 (3616) H     390a BoostClockAc                    : 2617
- 0x0e22 (3618) H     0000 BaseClockDc                     : 0
- 0x0e24 (3620) H     0000 GameClockDc                     : 0
- 0x0e26 (3622) H     0000 BoostClockDc                    : 0
- 0x0e28 (3624) I 00000000 Reserved                        : 0
- 0x0e2c (3628) I 00000000 Reserved                        : 0
- 0x0e30 (3632) I 00000000 Reserved                        : 0
- 0x0e34 (3636) I 00000000 Reserved                        : 0
- 0x0e38 (3640) H     5e01 Power                           : 350
- 0x0e3a (3642) H     0000 Power                           : 0
- 0x0e3c (3644) H     b004 Power                           : 1200
- 0x0e3e (3646) H     0000 Power                           : 0
- 0x0e40 (3648) H     0000 Power                           : 0
- 0x0e42 (3650) H     0000 Power                           : 0
- 0x0e44 (3652) H     0000 Power                           : 0
- 0x0e46 (3654) H     0000 Power                           : 0
- 0x0e48 (3656) H     c001 Tdc                             : 448
- 0x0e4a (3658) H     5200 Tdc                             : 82
- 0x0e4c (3660) H     5600 Tdc                             : 86
- 0x0e4e (3662) H     6400 Temperature                     : 100
- 0x0e50 (3664) H     6e00 Temperature                     : 110
- 0x0e52 (3666) H     6e00 Temperature                     : 110
- 0x0e54 (3668) H     6e00 Temperature                     : 110
- 0x0e56 (3670) H     6e00 Temperature                     : 110
- 0x0e58 (3672) H     7300 Temperature                     : 115
- 0x0e5a (3674) H     7300 Temperature                     : 115
- 0x0e5c (3676) H     7300 Temperature                     : 115
- 0x0e5e (3678) H     7300 Temperature                     : 115
- 0x0e60 (3680) H     7300 Temperature                     : 115
- 0x0e62 (3682) H     0000 Temperature                     : 0
- 0x0e64 (3684) H     0000 Temperature                     : 0
- 0x0e66 (3686) H     0000 Temperature                     : 0
- 0x0e68 (3688) B       00 PwmLimitMin                     : 0
- 0x0e69 (3689) B       ff PwmLimitMax                     : 255
- 0x0e6a (3690) B       6e FanTargetTemperature            : 110
- 0x0e6b (3691) B       00 Spare1                          : 0
- 0x0e6c (3692) H     f401 AcousticTargetRpmThresholdMin   : 500
- 0x0e6e (3694) H     7017 AcousticTargetRpmThresholdMax   : 6000
- 0x0e70 (3696) H     f401 AcousticLimitRpmThresholdMin    : 500
- 0x0e72 (3698) H     7017 AcousticLimitRpmThresholdMax    : 6000
- 0x0e74 (3700) H     0000 PccLimitMin                     : 0
- 0x0e76 (3702) H     c201 PccLimitMax                     : 450
- 0x0e78 (3704) H     1900 FanStopTempMin                  : 25
- 0x0e7a (3706) H     6400 FanStopTempMax                  : 100
- 0x0e7c (3708) H     1900 FanStartTempMin                 : 25
- 0x0e7e (3710) H     6400 FanStartTempMax                 : 100
- 0x0e80 (3712) H     0000 PowerMinPpt0                    : 0
- 0x0e82 (3714) H     0000 PowerMinPpt0                    : 0
- 0x0e84 (3716) I 00000000 Spare                           : 0
- 0x0e88 (3720) I 00000000 Spare                           : 0
- 0x0e8c (3724) I 00000000 Spare                           : 0
- 0x0e90 (3728) I 00000000 Spare                           : 0
- 0x0e94 (3732) I 00000000 Spare                           : 0
- 0x0e98 (3736) I 00000000 Spare                           : 0
- 0x0e9c (3740) I 00000000 Spare                           : 0
- 0x0ea0 (3744) I 00000000 Spare                           : 0
- 0x0ea4 (3748) I 00000000 Spare                           : 0
- 0x0ea8 (3752) I 00000000 Spare                           : 0
- 0x0eac (3756) I 00000000 Spare                           : 0
- 0x0eb0 (3760) I cd070000 FeatureCtrlMask                 : 1997
- 0x0eb4 (3764) h     3efe VoltageOffsetPerZoneBoundary    :-450
- 0x0eb6 (3766) H     0000 Reserved1                       : 0
- 0x0eb8 (3768) H     0000 Reserved2                       : 0
- 0x0eba (3770) h     f401 GfxclkFmin                      : 500
- 0x0ebc (3772) h     f401 GfxclkFmax                      : 500
- 0x0ebe (3774) H     6100 UclkFmin                        : 97
- 0x0ec0 (3776) H     6100 UclkFmax                        : 97
- 0x0ec2 (3778) h     f6ff Ppt                             :-10
- 0x0ec4 (3780) h     f6ff Tdc                             :-10
- 0x0ec6 (3782) B       0f FanLinearPwmPoints              : 15
- 0x0ec7 (3783) B       19 FanLinearTempPoints             : 25
- 0x0ec8 (3784) H     0f00 FanMinimumPwm                   : 15
- 0x0eca (3786) H     f401 AcousticTargetRpmThreshold      : 500
- 0x0ecc (3788) H     f401 AcousticLimitRpmThreshold       : 500
- 0x0ece (3790) H     1900 FanTargetTemperature            : 25
- 0x0ed0 (3792) B       00 FanZeroRpmEnable                : 0
- 0x0ed1 (3793) B       19 FanZeroRpmStopTemp              : 25
- 0x0ed2 (3794) B       00 FanMode                         : 0
- 0x0ed3 (3795) B       32 MaxOpTemp                       : 50
- 0x0ed4 (3796) B       00 Padding                         : 0
- 0x0ed5 (3797) B       00 Padding                         : 0
- 0x0ed6 (3798) B       00 Padding                         : 0
- 0x0ed7 (3799) B       00 Padding                         : 0
- 0x0ed8 (3800) I 00000000 Spare                           : 0
- 0x0edc (3804) I 00000000 Spare                           : 0
- 0x0ee0 (3808) I 00000000 Spare                           : 0
- 0x0ee4 (3812) I 00000000 Spare                           : 0
- 0x0ee8 (3816) I 00000000 Spare                           : 0
- 0x0eec (3820) I 00000000 Spare                           : 0
- 0x0ef0 (3824) I 00000000 Spare                           : 0
- 0x0ef4 (3828) I 00000000 Spare                           : 0
- 0x0ef8 (3832) I 00000000 Spare                           : 0
- 0x0efc (3836) I 00000000 Spare                           : 0
- 0x0f00 (3840) I 00000000 Spare                           : 0
- 0x0f04 (3844) I 00000000 Spare                           : 0
- 0x0f08 (3848) I cd070000 FeatureCtrlMask                 : 1997
- 0x0f0c (3852) h     0000 VoltageOffsetPerZoneBoundary    : 0
- 0x0f0e (3854) H     0000 Reserved1                       : 0
- 0x0f10 (3856) H     0000 Reserved2                       : 0
- 0x0f12 (3858) h     8813 GfxclkFmin                      : 5000
- 0x0f14 (3860) h     8813 GfxclkFmax                      : 5000
- 0x0f16 (3862) H     dc05 UclkFmin                        : 1500
- 0x0f18 (3864) H     dc05 UclkFmax                        : 1500
- 0x0f1a (3866) h     0f00 Ppt                             : 15
- 0x0f1c (3868) h     0000 Tdc                             : 0
- 0x0f1e (3870) B       64 FanLinearPwmPoints              : 100
- 0x0f1f (3871) B       64 FanLinearTempPoints             : 100
- 0x0f20 (3872) H     6400 FanMinimumPwm                   : 100
- 0x0f22 (3874) H     e40c AcousticTargetRpmThreshold      : 3300
- 0x0f24 (3876) H     e40c AcousticLimitRpmThreshold       : 3300
- 0x0f26 (3878) H     6900 FanTargetTemperature            : 105
- 0x0f28 (3880) B       01 FanZeroRpmEnable                : 1
- 0x0f29 (3881) B       64 FanZeroRpmStopTemp              : 100
- 0x0f2a (3882) B       01 FanMode                         : 1
- 0x0f2b (3883) B       6e MaxOpTemp                       : 110
- 0x0f2c (3884) B       00 Padding                         : 0
- 0x0f2d (3885) B       00 Padding                         : 0
- 0x0f2e (3886) B       00 Padding                         : 0
- 0x0f2f (3887) B       00 Padding                         : 0
- 0x0f30 (3888) I 00000000 Spare                           : 0
- 0x0f34 (3892) I 00000000 Spare                           : 0
- 0x0f38 (3896) I 00000000 Spare                           : 0
- 0x0f3c (3900) I 00000000 Spare                           : 0
- 0x0f40 (3904) I 00000000 Spare                           : 0
- 0x0f44 (3908) I 00000000 Spare                           : 0
- 0x0f48 (3912) I 00000000 Spare                           : 0
- 0x0f4c (3916) I 00000000 Spare                           : 0
- 0x0f50 (3920) I b0045802 Spare                           : 39322800
- 0x0f54 (3924) I d002f401 Spare                           : 32768720
- 0x0f58 (3928) I f401e803 Spare                           : 65536500
- 0x0f5c (3932) I 9001bc02 Spare                           : 45875600
- 0x0f60 (3936) I 00000000 FeatureCtrlMask                 : 0
- 0x0f64 (3940) h     0000 VoltageOffsetPerZoneBoundary    : 0
- 0x0f66 (3942) H     0000 Reserved1                       : 0
- 0x0f68 (3944) H     0000 Reserved2                       : 0
- 0x0f6a (3946) h     0000 GfxclkFmin                      : 0
- 0x0f6c (3948) h     0000 GfxclkFmax                      : 0
- 0x0f6e (3950) H     0000 UclkFmin                        : 0
- 0x0f70 (3952) H     0000 UclkFmax                        : 0
- 0x0f72 (3954) h     0000 Ppt                             : 0
- 0x0f74 (3956) h     0000 Tdc                             : 0
- 0x0f76 (3958) B       00 FanLinearPwmPoints              : 0
- 0x0f77 (3959) B       00 FanLinearTempPoints             : 0
- 0x0f78 (3960) H     0000 FanMinimumPwm                   : 0
- 0x0f7a (3962) H     0000 AcousticTargetRpmThreshold      : 0
- 0x0f7c (3964) H     0000 AcousticLimitRpmThreshold       : 0
- 0x0f7e (3966) H     0000 FanTargetTemperature            : 0
- 0x0f80 (3968) B       00 FanZeroRpmEnable                : 0
- 0x0f81 (3969) B       00 FanZeroRpmStopTemp              : 0
- 0x0f82 (3970) B       00 FanMode                         : 0
- 0x0f83 (3971) B       00 MaxOpTemp                       : 0
- 0x0f84 (3972) B       00 Padding                         : 0
- 0x0f85 (3973) B       00 Padding                         : 0
- 0x0f86 (3974) B       00 Padding                         : 0
- 0x0f87 (3975) B       00 Padding                         : 0
- 0x0f88 (3976) I 00000000 Spare                           : 0
- 0x0f8c (3980) I 00000000 Spare                           : 0
- 0x0f90 (3984) I 68100000 Spare                           : 4200
- 0x0f94 (3988) I 00000000 Spare                           : 0
- 0x0f98 (3992) I 0000bc02 Spare                           : 45875200
- 0x0f9c (3996) I ee020000 Spare                           : 750
- 0x0fa0 (4000) I 00000000 Spare                           : 0
- 0x0fa4 (4004) I 00000000 Spare                           : 0
- 0x0fa8 (4008) I 00000000 Spare                           : 0
- 0x0fac (4012) I 00000000 Spare                           : 0
- 0x0fb0 (4016) I 00000000 Spare                           : 0
- 0x0fb4 (4020) I 00000000 Spare                           : 0
- 0x0fb8 (4024) I 00000000 DebugOverrides                  : 0
- 0x0fbc (4028) B       01 TotalBoardPowerSupport          : 1
- 0x0fbd (4029) B       00 TotalBoardPowerPadding          : 0
- 0x0fbe (4030) B       00 TotalBoardPowerPadding          : 0
- 0x0fbf (4031) B       00 TotalBoardPowerPadding          : 0
- 0x0fc0 (4032) h     6d03 TotalIdleBoardPowerM            : 877
- 0x0fc2 (4034) h     0000 TotalIdleBoardPowerB            : 0
- 0x0fc4 (4036) h     9b04 TotalBoardPowerM                : 1179
- 0x0fc6 (4038) h     b30f TotalBoardPowerB                : 4019
- 0x0fc8 (4040) f 8f368ebd a                               :-0.06944
- 0x0fcc (4044) f 54553c42 b                               : 47.0833
- 0x0fd0 (4048) f 007daac5 c                               :-5455.62
- 0x0fd4 (4052) f 00000000 a                               : 0
- 0x0fd8 (4056) f 00000000 b                               : 0
- 0x0fdc (4060) f 00000000 c                               : 0
- 0x0fe0 (4064) f 3ecbf3bb a                               :-0.00744
- 0x0fe4 (4068) f 52550a41 b                               : 8.64583
- 0x0fe8 (4072) f 4af22f42 c                               : 43.9866
- 0x0fec (4076) f 00000000 a                               : 0
- 0x0ff0 (4080) f 00000000 b                               : 0
- 0x0ff4 (4084) f 00000000 c                               : 0
- 0x0ff8 (4088) f f7af2c3d a                               : 0.04216
- 0x0ffc (4092) f a92ab6c1 b                               :-22.7708
- 0x1000 (4096) f 9b98ad45 c                               : 5555.08
- 0x1004 (4100) f 00000000 a                               : 0
- 0x1008 (4104) f 00000000 b                               : 0
- 0x100c (4108) f 00000000 c                               : 0
- 0x1010 (4112) I 00000000 Spare                           : 0
- 0x1014 (4116) I 00000000 Spare                           : 0
- 0x1018 (4120) I 00000000 Spare                           : 0
- 0x101c (4124) I 00000000 Spare                           : 0
- 0x1020 (4128) I 00000000 Spare                           : 0
- 0x1024 (4132) I 00000000 Spare                           : 0
- 0x1028 (4136) I 00000000 Spare                           : 0
- 0x102c (4140) I 00000000 Spare                           : 0
- 0x1030 (4144) I 00000000 Spare                           : 0
- 0x1034 (4148) I 00000000 Spare                           : 0
- 0x1038 (4152) I 00000000 Spare                           : 0
- 0x103c (4156) I 00000000 Spare                           : 0
- 0x1040 (4160) I 00000000 Spare                           : 0
- 0x1044 (4164) I 00000000 Spare                           : 0
- 0x1048 (4168) I 00000000 Spare                           : 0
- 0x104c (4172) I 00000000 Spare                           : 0
- 0x1050 (4176) I 00000000 Spare                           : 0
- 0x1054 (4180) I 00000000 Spare                           : 0
- 0x1058 (4184) I 00000000 Spare                           : 0
- 0x105c (4188) I 00000000 Spare                           : 0
- 0x1060 (4192) I 00000000 Spare                           : 0
- 0x1064 (4196) I 00000000 Spare                           : 0
- 0x1068 (4200) I 00000000 Spare                           : 0
- 0x106c (4204) I 00000000 Spare                           : 0
- 0x1070 (4208) I 00000000 Spare                           : 0
- 0x1074 (4212) I 00000000 Spare                           : 0
- 0x1078 (4216) I 00000000 Spare                           : 0
- 0x107c (4220) I 00000000 Spare                           : 0
- 0x1080 (4224) I 00000000 Spare                           : 0
- 0x1084 (4228) I 00000000 Spare                           : 0
- 0x1088 (4232) I 00000000 Spare                           : 0
- 0x108c (4236) I 00000000 Spare                           : 0
- 0x1090 (4240) I 00000000 Spare                           : 0
- 0x1094 (4244) I 00000000 Spare                           : 0
- 0x1098 (4248) I 00000000 Spare                           : 0
- 0x109c (4252) I 00000000 Spare                           : 0
- 0x10a0 (4256) I 00000000 Spare                           : 0
- 0x10a4 (4260) I 00000000 Spare                           : 0
- 0x10a8 (4264) I 00000000 Spare                           : 0
- 0x10ac (4268) I 00000000 Spare                           : 0
- 0x10b0 (4272) I 00000000 Spare                           : 0
- 0x10b4 (4276) I 00000000 Spare                           : 0
- 0x10b8 (4280) I 00000000 Spare                           : 0
- 0x10bc (4284) I 00000000 MmHubPadding                    : 0
- 0x10c0 (4288) I 00000000 MmHubPadding                    : 0
- 0x10c4 (4292) I 00000000 MmHubPadding                    : 0
- 0x10c8 (4296) I 00000000 MmHubPadding                    : 0
- 0x10cc (4300) I 00000000 MmHubPadding                    : 0
- 0x10d0 (4304) I 00000000 MmHubPadding                    : 0
- 0x10d4 (4308) I 00000000 MmHubPadding                    : 0
- 0x10d8 (4312) I 00000000 MmHubPadding                    : 0
- 0x10dc (4316) I 26000000 Version                         : 38
- 0x10e0 (4320) B       00 Enabled                         : 0
- 0x10e1 (4321) B       00 Speed                           : 0
- 0x10e2 (4322) B       00 SlaveAddress                    : 0
- 0x10e3 (4323) B       00 ControllerPort                  : 0
- 0x10e4 (4324) B       00 ControllerName                  : 0
- 0x10e5 (4325) B       00 ThermalThrotter                 : 0
- 0x10e6 (4326) B       00 I2cProtocol                     : 0
- 0x10e7 (4327) B       00 PaddingConfig                   : 0
- 0x10e8 (4328) B       00 Enabled                         : 0
- 0x10e9 (4329) B       00 Speed                           : 0
- 0x10ea (4330) B       00 SlaveAddress                    : 0
- 0x10eb (4331) B       00 ControllerPort                  : 0
- 0x10ec (4332) B       00 ControllerName                  : 0
- 0x10ed (4333) B       00 ThermalThrotter                 : 0
- 0x10ee (4334) B       00 I2cProtocol                     : 0
- 0x10ef (4335) B       00 PaddingConfig                   : 0
- 0x10f0 (4336) B       00 Enabled                         : 0
- 0x10f1 (4337) B       00 Speed                           : 0
- 0x10f2 (4338) B       00 SlaveAddress                    : 0
- 0x10f3 (4339) B       00 ControllerPort                  : 0
- 0x10f4 (4340) B       00 ControllerName                  : 0
- 0x10f5 (4341) B       00 ThermalThrotter                 : 0
- 0x10f6 (4342) B       00 I2cProtocol                     : 0
- 0x10f7 (4343) B       00 PaddingConfig                   : 0
- 0x10f8 (4344) B       00 Enabled                         : 0
- 0x10f9 (4345) B       00 Speed                           : 0
- 0x10fa (4346) B       00 SlaveAddress                    : 0
- 0x10fb (4347) B       00 ControllerPort                  : 0
- 0x10fc (4348) B       00 ControllerName                  : 0
- 0x10fd (4349) B       00 ThermalThrotter                 : 0
- 0x10fe (4350) B       00 I2cProtocol                     : 0
- 0x10ff (4351) B       00 PaddingConfig                   : 0
- 0x1100 (4352) B       00 Enabled                         : 0
- 0x1101 (4353) B       00 Speed                           : 0
- 0x1102 (4354) B       00 SlaveAddress                    : 0
- 0x1103 (4355) B       00 ControllerPort                  : 0
- 0x1104 (4356) B       00 ControllerName                  : 0
- 0x1105 (4357) B       00 ThermalThrotter                 : 0
- 0x1106 (4358) B       00 I2cProtocol                     : 0
- 0x1107 (4359) B       00 PaddingConfig                   : 0
- 0x1108 (4360) B       00 Enabled                         : 0
- 0x1109 (4361) B       00 Speed                           : 0
- 0x110a (4362) B       00 SlaveAddress                    : 0
- 0x110b (4363) B       00 ControllerPort                  : 0
- 0x110c (4364) B       00 ControllerName                  : 0
- 0x110d (4365) B       00 ThermalThrotter                 : 0
- 0x110e (4366) B       00 I2cProtocol                     : 0
- 0x110f (4367) B       00 PaddingConfig                   : 0
- 0x1110 (4368) B       00 Enabled                         : 0
- 0x1111 (4369) B       00 Speed                           : 0
- 0x1112 (4370) B       00 SlaveAddress                    : 0
- 0x1113 (4371) B       00 ControllerPort                  : 0
- 0x1114 (4372) B       00 ControllerName                  : 0
- 0x1115 (4373) B       00 ThermalThrotter                 : 0
- 0x1116 (4374) B       00 I2cProtocol                     : 0
- 0x1117 (4375) B       00 PaddingConfig                   : 0
- 0x1118 (4376) B       00 Enabled                         : 0
- 0x1119 (4377) B       00 Speed                           : 0
- 0x111a (4378) B       00 SlaveAddress                    : 0
- 0x111b (4379) B       00 ControllerPort                  : 0
- 0x111c (4380) B       00 ControllerName                  : 0
- 0x111d (4381) B       00 ThermalThrotter                 : 0
- 0x111e (4382) B       00 I2cProtocol                     : 0
- 0x111f (4383) B       00 PaddingConfig                   : 0
- 0x1120 (4384) B       00 VddGfxVrMapping                 : 0
- 0x1121 (4385) B       00 VddSocVrMapping                 : 0
- 0x1122 (4386) B       00 VddMem0VrMapping                : 0
- 0x1123 (4387) B       00 VddMem1VrMapping                : 0
- 0x1124 (4388) B       00 GfxUlvPhaseSheddingMask         : 0
- 0x1125 (4389) B       00 SocUlvPhaseSheddingMask         : 0
- 0x1126 (4390) B       00 VmempUlvPhaseSheddingMask       : 0
- 0x1127 (4391) B       00 VddioUlvPhaseSheddingMask       : 0
- 0x1128 (4392) B       00 SlaveAddrMapping                : 0
- 0x1129 (4393) B       00 SlaveAddrMapping                : 0
- 0x112a (4394) B       00 SlaveAddrMapping                : 0
- 0x112b (4395) B       00 SlaveAddrMapping                : 0
- 0x112c (4396) B       00 SlaveAddrMapping                : 0
- 0x112d (4397) B       00 VrPsiSupport                    : 0
- 0x112e (4398) B       00 VrPsiSupport                    : 0
- 0x112f (4399) B       00 VrPsiSupport                    : 0
- 0x1130 (4400) B       01 VrPsiSupport                    : 1
- 0x1131 (4401) B       00 VrPsiSupport                    : 0
- 0x1132 (4402) B       00 PaddingPsi                      : 0
- 0x1133 (4403) B       00 PaddingPsi                      : 0
- 0x1134 (4404) B       00 PaddingPsi                      : 0
- 0x1135 (4405) B       00 PaddingPsi                      : 0
- 0x1136 (4406) B       00 PaddingPsi                      : 0
- 0x1137 (4407) B       00 EnablePsi6                      : 0
- 0x1138 (4408) B       00 EnablePsi6                      : 0
- 0x1139 (4409) B       00 EnablePsi6                      : 0
- 0x113a (4410) B       00 EnablePsi6                      : 0
- 0x113b (4411) B       00 EnablePsi6                      : 0
- 0x113c (4412) b       00 Offset                          : 0
- 0x113d (4413) B       00 Padding                         : 0
- 0x113e (4414) H     0000 MaxCurrent                      : 0
- 0x1140 (4416) b       00 Offset                          : 0
- 0x1141 (4417) B       00 Padding                         : 0
- 0x1142 (4418) H     0000 MaxCurrent                      : 0
- 0x1144 (4420) b       00 Offset                          : 0
- 0x1145 (4421) B       00 Padding                         : 0
- 0x1146 (4422) H     0000 MaxCurrent                      : 0
- 0x1148 (4424) b       00 Offset                          : 0
- 0x1149 (4425) B       00 Padding                         : 0
- 0x114a (4426) H     0000 MaxCurrent                      : 0
- 0x114c (4428) b       00 Offset                          : 0
- 0x114d (4429) B       00 Padding                         : 0
- 0x114e (4430) H     0000 MaxCurrent                      : 0
- 0x1150 (4432) I 00000000 VoltageTelemetryRatio           : 0
- 0x1154 (4436) I 00000000 VoltageTelemetryRatio           : 0
- 0x1158 (4440) I 00000000 VoltageTelemetryRatio           : 0
- 0x115c (4444) I 00000000 VoltageTelemetryRatio           : 0
- 0x1160 (4448) I 00000000 VoltageTelemetryRatio           : 0
- 0x1164 (4452) B       00 DownSlewRateVr                  : 0
- 0x1165 (4453) B       00 DownSlewRateVr                  : 0
- 0x1166 (4454) B       00 DownSlewRateVr                  : 0
- 0x1167 (4455) B       00 DownSlewRateVr                  : 0
- 0x1168 (4456) B       00 DownSlewRateVr                  : 0
- 0x1169 (4457) B       00 LedOffGpio                      : 0
- 0x116a (4458) B       00 FanOffGpio                      : 0
- 0x116b (4459) B       00 GfxVrPowerStageOffGpio          : 0
- 0x116c (4460) B       00 AcDcGpio                        : 0
- 0x116d (4461) B       00 AcDcPolarity                    : 0
- 0x116e (4462) B       00 VR0HotGpio                      : 0
- 0x116f (4463) B       00 VR0HotPolarity                  : 0
- 0x1170 (4464) B       00 GthrGpio                        : 0
- 0x1171 (4465) B       00 GthrPolarity                    : 0
- 0x1172 (4466) B       00 LedPin0                         : 0
- 0x1173 (4467) B       00 LedPin1                         : 0
- 0x1174 (4468) B       00 LedPin2                         : 0
- 0x1175 (4469) B       00 LedEnableMask                   : 0
- 0x1176 (4470) B       00 LedPcie                         : 0
- 0x1177 (4471) B       00 LedError                        : 0
- 0x1178 (4472) B       00 UclkTrainingModeSpreadPercent   : 0
- 0x1179 (4473) B       00 UclkSpreadPadding               : 0
- 0x117a (4474) H     0000 UclkSpreadFreq                  : 0
- 0x117c (4476) B       00 UclkSpreadPercent               : 0
- 0x117d (4477) B       00 UclkSpreadPercent               : 0
- 0x117e (4478) B       00 UclkSpreadPercent               : 0
- 0x117f (4479) B       00 UclkSpreadPercent               : 0
- 0x1180 (4480) B       00 UclkSpreadPercent               : 0
- 0x1181 (4481) B       00 UclkSpreadPercent               : 0
- 0x1182 (4482) B       00 UclkSpreadPercent               : 0
- 0x1183 (4483) B       00 UclkSpreadPercent               : 0
- 0x1184 (4484) B       00 UclkSpreadPercent               : 0
- 0x1185 (4485) B       00 UclkSpreadPercent               : 0
- 0x1186 (4486) B       00 UclkSpreadPercent               : 0
- 0x1187 (4487) B       00 UclkSpreadPercent               : 0
- 0x1188 (4488) B       00 UclkSpreadPercent               : 0
- 0x1189 (4489) B       00 UclkSpreadPercent               : 0
- 0x118a (4490) B       00 UclkSpreadPercent               : 0
- 0x118b (4491) B       00 UclkSpreadPercent               : 0
- 0x118c (4492) B       00 FclkSpreadPadding               : 0
- 0x118d (4493) B       00 FclkSpreadPercent               : 0
- 0x118e (4494) H     0000 FclkSpreadFreq                  : 0
- 0x1190 (4496) B       00 DramWidth                       : 0
- 0x1191 (4497) B       00 PaddingMem1                     : 0
- 0x1192 (4498) B       00 PaddingMem1                     : 0
- 0x1193 (4499) B       00 PaddingMem1                     : 0
- 0x1194 (4500) B       00 PaddingMem1                     : 0
- 0x1195 (4501) B       00 PaddingMem1                     : 0
- 0x1196 (4502) B       00 PaddingMem1                     : 0
- 0x1197 (4503) B       00 PaddingMem1                     : 0
- 0x1198 (4504) B       00 HsrEnabled                      : 0
- 0x1199 (4505) B       00 VddqOffEnabled                  : 0
- 0x119a (4506) B       00 PaddingUmcFlags                 : 0
- 0x119b (4507) B       00 PaddingUmcFlags                 : 0
- 0x119c (4508) I 00000000 PostVoltageSetBacoDelay         : 0
- 0x11a0 (4512) I 00000000 BacoEntryDelay                  : 0
- 0x11a4 (4516) B       00 FuseWritePowerMuxPresent        : 0
- 0x11a5 (4517) B       00 FuseWritePadding                : 0
- 0x11a6 (4518) B       00 FuseWritePadding                : 0
- 0x11a7 (4519) B       00 FuseWritePadding                : 0
- 0x11a8 (4520) I 00000000 BoardSpare                      : 0
- 0x11ac (4524) I 00000000 BoardSpare                      : 0
- 0x11b0 (4528) I 00000000 BoardSpare                      : 0
- 0x11b4 (4532) I 00000000 BoardSpare                      : 0
- 0x11b8 (4536) I 00000000 BoardSpare                      : 0
- 0x11bc (4540) I 00000000 BoardSpare                      : 0
- 0x11c0 (4544) I 00000000 BoardSpare                      : 0
- 0x11c4 (4548) I 00000000 BoardSpare                      : 0
- 0x11c8 (4552) I 00000000 BoardSpare                      : 0
- 0x11cc (4556) I 00000000 BoardSpare                      : 0
- 0x11d0 (4560) I 00000000 BoardSpare                      : 0
- 0x11d4 (4564) I 00000000 BoardSpare                      : 0
- 0x11d8 (4568) I 00000000 BoardSpare                      : 0
- 0x11dc (4572) I 00000000 BoardSpare                      : 0
- 0x11e0 (4576) I 00000000 BoardSpare                      : 0
- 0x11e4 (4580) I 00000000 BoardSpare                      : 0
- 0x11e8 (4584) I 00000000 BoardSpare                      : 0
- 0x11ec (4588) I 00000000 BoardSpare                      : 0
- 0x11f0 (4592) I 00000000 BoardSpare                      : 0
- 0x11f4 (4596) I 00000000 BoardSpare                      : 0
- 0x11f8 (4600) I 00000000 BoardSpare                      : 0
- 0x11fc (4604) I 00000000 BoardSpare                      : 0
- 0x1200 (4608) I 00000000 BoardSpare                      : 0
- 0x1204 (4612) I 00000000 BoardSpare                      : 0
- 0x1208 (4616) I 00000000 BoardSpare                      : 0
- 0x120c (4620) I 00000000 BoardSpare                      : 0
- 0x1210 (4624) I 00000000 BoardSpare                      : 0
- 0x1214 (4628) I 00000000 BoardSpare                      : 0
- 0x1218 (4632) I 00000000 BoardSpare                      : 0
- 0x121c (4636) I 00000000 BoardSpare                      : 0
- 0x1220 (4640) I 00000000 BoardSpare                      : 0
- 0x1224 (4644) I 00000000 BoardSpare                      : 0
- 0x1228 (4648) I 00000000 BoardSpare                      : 0
- 0x122c (4652) I 00000000 BoardSpare                      : 0
- 0x1230 (4656) I 00000000 BoardSpare                      : 0
- 0x1234 (4660) I 00000000 BoardSpare                      : 0
- 0x1238 (4664) I 00000000 BoardSpare                      : 0
- 0x123c (4668) I 00000000 BoardSpare                      : 0
- 0x1240 (4672) I 00000000 BoardSpare                      : 0
- 0x1244 (4676) I 00000000 BoardSpare                      : 0
- 0x1248 (4680) I 00000000 BoardSpare                      : 0
- 0x124c (4684) I 00000000 BoardSpare                      : 0
- 0x1250 (4688) I 00000000 BoardSpare                      : 0
- 0x1254 (4692) I 00000000 BoardSpare                      : 0
- 0x1258 (4696) I 00000000 BoardSpare                      : 0
- 0x125c (4700) I 00000000 BoardSpare                      : 0
- 0x1260 (4704) I 00000000 BoardSpare                      : 0
- 0x1264 (4708) I 00000000 BoardSpare                      : 0
- 0x1268 (4712) I 00000000 BoardSpare                      : 0
- 0x126c (4716) I 00000000 BoardSpare                      : 0
- 0x1270 (4720) I 00000000 BoardSpare                      : 0
- 0x1274 (4724) I 00000000 BoardSpare                      : 0
- 0x1278 (4728) I 00000000 BoardSpare                      : 0
- 0x127c (4732) I 00000000 BoardSpare                      : 0
- 0x1280 (4736) I 00000000 BoardSpare                      : 0
- 0x1284 (4740) I 00000000 BoardSpare                      : 0
- 0x1288 (4744) I 00000000 BoardSpare                      : 0
- 0x128c (4748) I 00000000 BoardSpare                      : 0
- 0x1290 (4752) I 00000000 BoardSpare                      : 0
- 0x1294 (4756) I 00000000 BoardSpare                      : 0
- 0x1298 (4760) I 00000000 BoardSpare                      : 0
- 0x129c (4764) I 00000000 BoardSpare                      : 0
- 0x12a0 (4768) I 00000000 BoardSpare                      : 0
- 0x12a4 (4772) I 00000000 MmHubPadding                    : 0
- 0x12a8 (4776) I 00000000 MmHubPadding                    : 0
- 0x12ac (4780) I 00000000 MmHubPadding                    : 0
- 0x12b0 (4784) I 00000000 MmHubPadding                    : 0
- 0x12b4 (4788) I 00000000 MmHubPadding                    : 0
- 0x12b8 (4792) I 00000000 MmHubPadding                    : 0
- 0x12bc (4796) I 00000000 MmHubPadding                    : 0
- 0x12c0 (4800) I 00000000 MmHubPadding                    : 0
+ 0x0748 (1864) I 64006400 DfllPccAsWaitCtrl                         : 6553700
+ 0x074c (1868) I 2f841f00 DfllPccAsStepCtrl                         : 2065455
+ 0x0750 (1872) I 713d8a3f GfxGpoSpare                               : 1066024305
+ 0x0754 (1876) I 00000000 GfxGpoSpare                               : 0
+ 0x0758 (1880) I 00000000 GfxGpoSpare                               : 0
+ 0x075c (1884) I 00000000 GfxGpoSpare                               : 0
+ 0x0760 (1888) I 00000000 GfxGpoSpare                               : 0
+ 0x0764 (1892) I 00000000 GfxGpoSpare                               : 0
+ 0x0768 (1896) I 00000000 GfxGpoSpare                               : 0
+ 0x076c (1900) I 00000000 GfxGpoSpare                               : 0
+ 0x0770 (1904) I 00000000 GfxGpoSpare                               : 0
+ 0x0774 (1908) I 00000000 GfxGpoSpare                               : 0
+ 0x0778 (1912) H     0000 DcsGfxOffVoltage                          : 0
+ 0x077a (1914) H     0000 PaddingDcs                                : 0
+ 0x077c (1916) H     0000 DcsMinGfxOffTime                          : 0
+ 0x077e (1918) H     0000 DcsMaxGfxOffTime                          : 0
+ 0x0780 (1920) I 00000000 DcsMinCreditAccum                         : 0
+ 0x0784 (1924) H     0000 DcsExitHysteresis                         : 0
+ 0x0786 (1926) H     0000 DcsTimeout                                : 0
+ 0x0788 (1928) I 00000000 DcsSpare                                  : 0
+ 0x078c (1932) I 00000000 DcsSpare                                  : 0
+ 0x0790 (1936) I 00000000 DcsSpare                                  : 0
+ 0x0794 (1940) I 00000000 DcsSpare                                  : 0
+ 0x0798 (1944) I 00000000 DcsSpare                                  : 0
+ 0x079c (1948) I 00000000 DcsSpare                                  : 0
+ 0x07a0 (1952) I 00000000 DcsSpare                                  : 0
+ 0x07a4 (1956) I 00000000 DcsSpare                                  : 0
+ 0x07a8 (1960) I 00000000 DcsSpare                                  : 0
+ 0x07ac (1964) I 00000000 DcsSpare                                  : 0
+ 0x07b0 (1968) I 00000000 DcsSpare                                  : 0
+ 0x07b4 (1972) I 00000000 DcsSpare                                  : 0
+ 0x07b8 (1976) I 00000000 DcsSpare                                  : 0
+ 0x07bc (1980) I 00000000 DcsSpare                                  : 0
+ 0x07c0 (1984) H     6400 ShadowFreqTableUclk                       : 100
+ 0x07c2 (1986) H     b601 ShadowFreqTableUclk                       : 438
+ 0x07c4 (1988) H     db02 ShadowFreqTableUclk                       : 731
+ 0x07c6 (1990) H     a304 ShadowFreqTableUclk                       : 1187
+ 0x07c8 (1992) B       01 UseStrobeModeOptimizations                : 1
+ 0x07c9 (1993) B       0a PaddingMem                                : 10
+ 0x07ca (1994) B       f0 PaddingMem                                : 240
+ 0x07cb (1995) B       0a PaddingMem                                : 10
+ 0x07cc (1996) B       03 UclkDpmPstates                            : 3
+ 0x07cd (1997) B       02 UclkDpmPstates                            : 2
+ 0x07ce (1998) B       01 UclkDpmPstates                            : 1
+ 0x07cf (1999) B       00 UclkDpmPstates                            : 0
+ 0x07d0 (2000) B       00 FreqTableUclkDiv                          : 0
+ 0x07d1 (2001) B       02 FreqTableUclkDiv                          : 2
+ 0x07d2 (2002) B       03 FreqTableUclkDiv                          : 3
+ 0x07d3 (2003) B       03 FreqTableUclkDiv                          : 3
+ 0x07d4 (2004) H     8c0a MemVmempVoltage                           : 2700
+ 0x07d6 (2006) H     f00a MemVmempVoltage                           : 2800
+ 0x07d8 (2008) H     b80b MemVmempVoltage                           : 3000
+ 0x07da (2010) H     800c MemVmempVoltage                           : 3200
+ 0x07dc (2012) H     8813 MemVddioVoltage                           : 5000
+ 0x07de (2014) H     1815 MemVddioVoltage                           : 5400
+ 0x07e0 (2016) H     1815 MemVddioVoltage                           : 5400
+ 0x07e2 (2018) H     1815 MemVddioVoltage                           : 5400
+ 0x07e4 (2020) B       00 FclkDpmUPstates                           : 0
+ 0x07e5 (2021) B       01 FclkDpmUPstates                           : 1
+ 0x07e6 (2022) B       02 FclkDpmUPstates                           : 2
+ 0x07e7 (2023) B       03 FclkDpmUPstates                           : 3
+ 0x07e8 (2024) B       04 FclkDpmUPstates                           : 4
+ 0x07e9 (2025) B       05 FclkDpmUPstates                           : 5
+ 0x07ea (2026) B       06 FclkDpmUPstates                           : 6
+ 0x07eb (2027) B       07 FclkDpmUPstates                           : 7
+ 0x07ec (2028) H     b80b FclkDpmVddU                               : 3000
+ 0x07ee (2030) H     b80b FclkDpmVddU                               : 3000
+ 0x07f0 (2032) H     b80b FclkDpmVddU                               : 3000
+ 0x07f2 (2034) H     b80b FclkDpmVddU                               : 3000
+ 0x07f4 (2036) H     b80b FclkDpmVddU                               : 3000
+ 0x07f6 (2038) H     480d FclkDpmVddU                               : 3400
+ 0x07f8 (2040) H     480d FclkDpmVddU                               : 3400
+ 0x07fa (2042) H     480d FclkDpmVddU                               : 3400
+ 0x07fc (2044) H     6009 FclkDpmUSpeed                             : 2400
+ 0x07fe (2046) H     a00f FclkDpmUSpeed                             : 4000
+ 0x0800 (2048) H     c012 FclkDpmUSpeed                             : 4800
+ 0x0802 (2050) H     0019 FclkDpmUSpeed                             : 6400
+ 0x0804 (2052) H     401f FclkDpmUSpeed                             : 8000
+ 0x0806 (2054) H     6022 FclkDpmUSpeed                             : 8800
+ 0x0808 (2056) H     2823 FclkDpmUSpeed                             : 9000
+ 0x080a (2058) H     f023 FclkDpmUSpeed                             : 9200
+ 0x080c (2060) H     0000 FclkDpmDisallowPstateFreq                 : 0
+ 0x080e (2062) H     0000 PaddingFclk                               : 0
+ 0x0810 (2064) B       00 PcieGenSpeed                              : 0
+ 0x0811 (2065) B       01 PcieGenSpeed                              : 1
+ 0x0812 (2066) B       03 PcieGenSpeed                              : 3
+ 0x0813 (2067) B       01 PcieLaneCount                             : 1
+ 0x0814 (2068) B       03 PcieLaneCount                             : 3
+ 0x0815 (2069) B       06 PcieLaneCount                             : 6
+ 0x0816 (2070) H     4e00 LclkFreq                                  : 78
+ 0x0818 (2072) H     9c00 LclkFreq                                  : 156
+ 0x081a (2074) H     6f02 LclkFreq                                  : 623
+ 0x081c (2076) H     0000 FanStopTemp                               : 0
+ 0x081e (2078) H     3200 FanStopTemp                               : 50
+ 0x0820 (2080) H     3200 FanStopTemp                               : 50
+ 0x0822 (2082) H     3200 FanStopTemp                               : 50
+ 0x0824 (2084) H     3c00 FanStopTemp                               : 60
+ 0x0826 (2086) H     3200 FanStopTemp                               : 50
+ 0x0828 (2088) H     3200 FanStopTemp                               : 50
+ 0x082a (2090) H     3200 FanStopTemp                               : 50
+ 0x082c (2092) H     3200 FanStopTemp                               : 50
+ 0x082e (2094) H     3200 FanStopTemp                               : 50
+ 0x0830 (2096) H     0000 FanStopTemp                               : 0
+ 0x0832 (2098) H     0000 FanStopTemp                               : 0
+ 0x0834 (2100) H     0000 FanStopTemp                               : 0
+ 0x0836 (2102) H     0000 FanStartTemp                              : 0
+ 0x0838 (2104) H     3c00 FanStartTemp                              : 60
+ 0x083a (2106) H     3c00 FanStartTemp                              : 60
+ 0x083c (2108) H     3c00 FanStartTemp                              : 60
+ 0x083e (2110) H     4600 FanStartTemp                              : 70
+ 0x0840 (2112) H     3c00 FanStartTemp                              : 60
+ 0x0842 (2114) H     3c00 FanStartTemp                              : 60
+ 0x0844 (2116) H     3c00 FanStartTemp                              : 60
+ 0x0846 (2118) H     3c00 FanStartTemp                              : 60
+ 0x0848 (2120) H     3c00 FanStartTemp                              : 60
+ 0x084a (2122) H     0000 FanStartTemp                              : 0
+ 0x084c (2124) H     0000 FanStartTemp                              : 0
+ 0x084e (2126) H     0000 FanStartTemp                              : 0
+ 0x0850 (2128) H     0000 FanGain                                   : 0
+ 0x0852 (2130) H     9001 FanGain                                   : 400
+ 0x0854 (2132) H     9001 FanGain                                   : 400
+ 0x0856 (2134) H     9001 FanGain                                   : 400
+ 0x0858 (2136) H     9001 FanGain                                   : 400
+ 0x085a (2138) H     9001 FanGain                                   : 400
+ 0x085c (2140) H     9001 FanGain                                   : 400
+ 0x085e (2142) H     9001 FanGain                                   : 400
+ 0x0860 (2144) H     9001 FanGain                                   : 400
+ 0x0862 (2146) H     9001 FanGain                                   : 400
+ 0x0864 (2148) H     0000 FanGain                                   : 0
+ 0x0866 (2150) H     0000 FanGain                                   : 0
+ 0x0868 (2152) H     0000 FanGain                                   : 0
+ 0x086a (2154) H     2413 FanGainPadding                            : 4900
+ 0x086c (2156) H     0f00 FanPwmMin                                 : 15
+ 0x086e (2158) H     4006 AcousticTargetRpmThreshold                : 1600
+ 0x0870 (2160) H     e40c AcousticLimitRpmThreshold                 : 3300
+ 0x0872 (2162) H     e40c FanMaximumRpm                             : 3300
+ 0x0874 (2164) H     b80b MGpuAcousticLimitRpmThreshold             : 3000
+ 0x0876 (2166) H     f401 FanTargetGfxclk                           : 500
+ 0x0878 (2168) I f2030000 TempInputSelectMask                       : 1010
+ 0x087c (2172) B       01 FanZeroRpmEnable                          : 1
+ 0x087d (2173) B       02 FanTachEdgePerRev                         : 2
+ 0x087e (2174) H     0000 FanTargetTemperature                      : 0
+ 0x0880 (2176) H     5200 FanTargetTemperature                      : 82
+ 0x0882 (2178) H     5200 FanTargetTemperature                      : 82
+ 0x0884 (2180) H     5200 FanTargetTemperature                      : 82
+ 0x0886 (2182) H     5a00 FanTargetTemperature                      : 90
+ 0x0888 (2184) H     6400 FanTargetTemperature                      : 100
+ 0x088a (2186) H     6400 FanTargetTemperature                      : 100
+ 0x088c (2188) H     6400 FanTargetTemperature                      : 100
+ 0x088e (2190) H     6400 FanTargetTemperature                      : 100
+ 0x0890 (2192) H     6400 FanTargetTemperature                      : 100
+ 0x0892 (2194) H     0000 FanTargetTemperature                      : 0
+ 0x0894 (2196) H     0000 FanTargetTemperature                      : 0
+ 0x0896 (2198) H     0000 FanTargetTemperature                      : 0
+ 0x0898 (2200) h     0000 FuzzyFan_ErrorSetDelta                    : 0
+ 0x089a (2202) h     0000 FuzzyFan_ErrorRateSetDelta                : 0
+ 0x089c (2204) h     0000 FuzzyFan_PwmSetDelta                      : 0
+ 0x089e (2206) H     7d00 FuzzyFan_Reserved                         : 125
+ 0x08a0 (2208) H     0000 FwCtfLimit                                : 0
+ 0x08a2 (2210) H     7600 FwCtfLimit                                : 118
+ 0x08a4 (2212) H     7600 FwCtfLimit                                : 118
+ 0x08a6 (2214) H     7600 FwCtfLimit                                : 118
+ 0x08a8 (2216) H     7100 FwCtfLimit                                : 113
+ 0x08aa (2218) H     7d00 FwCtfLimit                                : 125
+ 0x08ac (2220) H     7d00 FwCtfLimit                                : 125
+ 0x08ae (2222) H     7d00 FwCtfLimit                                : 125
+ 0x08b0 (2224) H     7d00 FwCtfLimit                                : 125
+ 0x08b2 (2226) H     7d00 FwCtfLimit                                : 125
+ 0x08b4 (2228) H     0000 FwCtfLimit                                : 0
+ 0x08b6 (2230) H     0000 FwCtfLimit                                : 0
+ 0x08b8 (2232) H     0000 FwCtfLimit                                : 0
+ 0x08ba (2234) H     e803 IntakeTempEnableRPM                       : 1000
+ 0x08bc (2236) h     c800 IntakeTempOffsetTemp                      : 200
+ 0x08be (2238) H     2d00 IntakeTempReleaseTemp                     : 45
+ 0x08c0 (2240) H     b80b IntakeTempHighIntakeAcousticLimit         : 3000
+ 0x08c2 (2242) H     6400 IntakeTempAcouticLimitReleaseRate         : 100
+ 0x08c4 (2244) h     ecff FanAbnormalTempLimitOffset                :-20
+ 0x08c6 (2246) H     fa00 FanStalledTriggerRpm                      : 250
+ 0x08c8 (2248) H     5500 FanAbnormalTriggerRpmCoeff                : 85
+ 0x08ca (2250) H     0000 FanAbnormalDetectionEnable                : 0
+ 0x08cc (2252) B       01 FanIntakeSensorSupport                    : 1
+ 0x08cd (2253) B       00 FanIntakePadding                          : 0
+ 0x08ce (2254) B       00 FanIntakePadding                          : 0
+ 0x08cf (2255) B       00 FanIntakePadding                          : 0
+ 0x08d0 (2256) I 00000000 FanSpare                                  : 0
+ 0x08d4 (2260) I 00000000 FanSpare                                  : 0
+ 0x08d8 (2264) I 00000000 FanSpare                                  : 0
+ 0x08dc (2268) I 00000000 FanSpare                                  : 0
+ 0x08e0 (2272) I 00000000 FanSpare                                  : 0
+ 0x08e4 (2276) I 00000000 FanSpare                                  : 0
+ 0x08e8 (2280) I 00000000 FanSpare                                  : 0
+ 0x08ec (2284) I 00000000 FanSpare                                  : 0
+ 0x08f0 (2288) I 00000000 FanSpare                                  : 0
+ 0x08f4 (2292) I 00000000 FanSpare                                  : 0
+ 0x08f8 (2296) I 00000000 FanSpare                                  : 0
+ 0x08fc (2300) I 00000000 FanSpare                                  : 0
+ 0x0900 (2304) I 00000000 FanSpare                                  : 0
+ 0x0904 (2308) B       00 OverrideGfxAvfsFuses                      : 0
+ 0x0905 (2309) B       00 GfxAvfsPadding                            : 0
+ 0x0906 (2310) B       00 GfxAvfsPadding                            : 0
+ 0x0907 (2311) B       00 GfxAvfsPadding                            : 0
+ 0x0908 (2312) I 00000001 L2HwRtAvfsFuses                           : 16777216
+ 0x090c (2316) I 00000001 L2HwRtAvfsFuses                           : 16777216
+ 0x0910 (2320) I 00000001 L2HwRtAvfsFuses                           : 16777216
+ 0x0914 (2324) I 00000001 L2HwRtAvfsFuses                           : 16777216
+ 0x0918 (2328) I 00000001 L2HwRtAvfsFuses                           : 16777216
+ 0x091c (2332) I 40050002 L2HwRtAvfsFuses                           : 33555776
+ 0x0920 (2336) I 00100000 L2HwRtAvfsFuses                           : 4096
+ 0x0924 (2340) I 40050002 L2HwRtAvfsFuses                           : 33555776
+ 0x0928 (2344) I 00100000 L2HwRtAvfsFuses                           : 4096
+ 0x092c (2348) I 40050002 L2HwRtAvfsFuses                           : 33555776
+ 0x0930 (2352) I 00100000 L2HwRtAvfsFuses                           : 4096
+ 0x0934 (2356) I 40050002 L2HwRtAvfsFuses                           : 33555776
+ 0x0938 (2360) I 00100000 L2HwRtAvfsFuses                           : 4096
+ 0x093c (2364) I 40050002 L2HwRtAvfsFuses                           : 33555776
+ 0x0940 (2368) I 00100000 L2HwRtAvfsFuses                           : 4096
+ 0x0944 (2372) I e7001301 L2HwRtAvfsFuses                           : 18022631
+ 0x0948 (2376) I 34013101 L2HwRtAvfsFuses                           : 19988788
+ 0x094c (2380) I 80015801 L2HwRtAvfsFuses                           : 22544768
+ 0x0950 (2384) I cd018b01 L2HwRtAvfsFuses                           : 25887181
+ 0x0954 (2388) I 00000000 L2HwRtAvfsFuses                           : 0
+ 0x0958 (2392) I 00000000 L2HwRtAvfsFuses                           : 0
+ 0x095c (2396) I 00000000 L2HwRtAvfsFuses                           : 0
+ 0x0960 (2400) I 00000000 L2HwRtAvfsFuses                           : 0
+ 0x0964 (2404) I 00000000 L2HwRtAvfsFuses                           : 0
+ 0x0968 (2408) I 00000000 L2HwRtAvfsFuses                           : 0
+ 0x096c (2412) I 00000000 L2HwRtAvfsFuses                           : 0
+ 0x0970 (2416) I 00000000 L2HwRtAvfsFuses                           : 0
+ 0x0974 (2420) I 00000000 L2HwRtAvfsFuses                           : 0
+ 0x0978 (2424) I 10801080 L2HwRtAvfsFuses                           : 2148565008
+ 0x097c (2428) I 10801080 L2HwRtAvfsFuses                           : 2148565008
+ 0x0980 (2432) I 10800000 L2HwRtAvfsFuses                           : 32784
+ 0x0984 (2436) I ffff0000 L2HwRtAvfsFuses                           : 65535
+ 0x0988 (2440) I 00000001 SeHwRtAvfsFuses                           : 16777216
+ 0x098c (2444) I 00000001 SeHwRtAvfsFuses                           : 16777216
+ 0x0990 (2448) I 00000001 SeHwRtAvfsFuses                           : 16777216
+ 0x0994 (2452) I 00000001 SeHwRtAvfsFuses                           : 16777216
+ 0x0998 (2456) I 00000001 SeHwRtAvfsFuses                           : 16777216
+ 0x099c (2460) I 40050002 SeHwRtAvfsFuses                           : 33555776
+ 0x09a0 (2464) I 00100000 SeHwRtAvfsFuses                           : 4096
+ 0x09a4 (2468) I 40050002 SeHwRtAvfsFuses                           : 33555776
+ 0x09a8 (2472) I 00100000 SeHwRtAvfsFuses                           : 4096
+ 0x09ac (2476) I 40050002 SeHwRtAvfsFuses                           : 33555776
+ 0x09b0 (2480) I 00100000 SeHwRtAvfsFuses                           : 4096
+ 0x09b4 (2484) I 40050002 SeHwRtAvfsFuses                           : 33555776
+ 0x09b8 (2488) I 00100000 SeHwRtAvfsFuses                           : 4096
+ 0x09bc (2492) I 40050002 SeHwRtAvfsFuses                           : 33555776
+ 0x09c0 (2496) I 00100000 SeHwRtAvfsFuses                           : 4096
+ 0x09c4 (2500) I e7001301 SeHwRtAvfsFuses                           : 18022631
+ 0x09c8 (2504) I 34013101 SeHwRtAvfsFuses                           : 19988788
+ 0x09cc (2508) I 80015801 SeHwRtAvfsFuses                           : 22544768
+ 0x09d0 (2512) I cd018b01 SeHwRtAvfsFuses                           : 25887181
+ 0x09d4 (2516) I 00000000 SeHwRtAvfsFuses                           : 0
+ 0x09d8 (2520) I 00000000 SeHwRtAvfsFuses                           : 0
+ 0x09dc (2524) I 00000000 SeHwRtAvfsFuses                           : 0
+ 0x09e0 (2528) I 00000000 SeHwRtAvfsFuses                           : 0
+ 0x09e4 (2532) I 00000000 SeHwRtAvfsFuses                           : 0
+ 0x09e8 (2536) I 00000000 SeHwRtAvfsFuses                           : 0
+ 0x09ec (2540) I 00000000 SeHwRtAvfsFuses                           : 0
+ 0x09f0 (2544) I 00000000 SeHwRtAvfsFuses                           : 0
+ 0x09f4 (2548) I 00000000 SeHwRtAvfsFuses                           : 0
+ 0x09f8 (2552) I 10801080 SeHwRtAvfsFuses                           : 2148565008
+ 0x09fc (2556) I 10801080 SeHwRtAvfsFuses                           : 2148565008
+ 0x0a00 (2560) I 10800000 SeHwRtAvfsFuses                           : 32784
+ 0x0a04 (2564) I ffff0000 SeHwRtAvfsFuses                           : 65535
+ 0x0a08 (2568) I bc020000 CommonRtAvfs                              : 700
+ 0x0a0c (2572) I bc020000 CommonRtAvfs                              : 700
+ 0x0a10 (2576) I bc020000 CommonRtAvfs                              : 700
+ 0x0a14 (2580) I bc020000 CommonRtAvfs                              : 700
+ 0x0a18 (2584) I bc020000 CommonRtAvfs                              : 700
+ 0x0a1c (2588) I bc020000 CommonRtAvfs                              : 700
+ 0x0a20 (2592) I bc020000 CommonRtAvfs                              : 700
+ 0x0a24 (2596) I bc020000 CommonRtAvfs                              : 700
+ 0x0a28 (2600) I 00000000 CommonRtAvfs                              : 0
+ 0x0a2c (2604) I aa020000 CommonRtAvfs                              : 682
+ 0x0a30 (2608) I aa020000 CommonRtAvfs                              : 682
+ 0x0a34 (2612) I aa020000 CommonRtAvfs                              : 682
+ 0x0a38 (2616) I aa020000 CommonRtAvfs                              : 682
+ 0x0a3c (2620) I 00000000 L2FwRtAvfsFuses                           : 0
+ 0x0a40 (2624) I 00000000 L2FwRtAvfsFuses                           : 0
+ 0x0a44 (2628) I 00000000 L2FwRtAvfsFuses                           : 0
+ 0x0a48 (2632) I 00000000 L2FwRtAvfsFuses                           : 0
+ 0x0a4c (2636) I 00000000 L2FwRtAvfsFuses                           : 0
+ 0x0a50 (2640) I 00000000 L2FwRtAvfsFuses                           : 0
+ 0x0a54 (2644) I 00000000 L2FwRtAvfsFuses                           : 0
+ 0x0a58 (2648) I 00000000 L2FwRtAvfsFuses                           : 0
+ 0x0a5c (2652) I 00000000 L2FwRtAvfsFuses                           : 0
+ 0x0a60 (2656) I 00000000 L2FwRtAvfsFuses                           : 0
+ 0x0a64 (2660) I 00000000 L2FwRtAvfsFuses                           : 0
+ 0x0a68 (2664) I 00000000 L2FwRtAvfsFuses                           : 0
+ 0x0a6c (2668) I 32000000 L2FwRtAvfsFuses                           : 50
+ 0x0a70 (2672) I b80b0000 L2FwRtAvfsFuses                           : 3000
+ 0x0a74 (2676) I 02060000 L2FwRtAvfsFuses                           : 1538
+ 0x0a78 (2680) I 02060000 L2FwRtAvfsFuses                           : 1538
+ 0x0a7c (2684) I 02060000 L2FwRtAvfsFuses                           : 1538
+ 0x0a80 (2688) I 02060000 L2FwRtAvfsFuses                           : 1538
+ 0x0a84 (2692) I 02060000 L2FwRtAvfsFuses                           : 1538
+ 0x0a88 (2696) I 00000000 SeFwRtAvfsFuses                           : 0
+ 0x0a8c (2700) I 00000000 SeFwRtAvfsFuses                           : 0
+ 0x0a90 (2704) I 00000000 SeFwRtAvfsFuses                           : 0
+ 0x0a94 (2708) I 00000000 SeFwRtAvfsFuses                           : 0
+ 0x0a98 (2712) I 00000000 SeFwRtAvfsFuses                           : 0
+ 0x0a9c (2716) I 00000000 SeFwRtAvfsFuses                           : 0
+ 0x0aa0 (2720) I 00000000 SeFwRtAvfsFuses                           : 0
+ 0x0aa4 (2724) I 00000000 SeFwRtAvfsFuses                           : 0
+ 0x0aa8 (2728) I 00000000 SeFwRtAvfsFuses                           : 0
+ 0x0aac (2732) I 00000000 SeFwRtAvfsFuses                           : 0
+ 0x0ab0 (2736) I 00000000 SeFwRtAvfsFuses                           : 0
+ 0x0ab4 (2740) I 00000000 SeFwRtAvfsFuses                           : 0
+ 0x0ab8 (2744) I 32000000 SeFwRtAvfsFuses                           : 50
+ 0x0abc (2748) I b80b0000 SeFwRtAvfsFuses                           : 3000
+ 0x0ac0 (2752) I 02060000 SeFwRtAvfsFuses                           : 1538
+ 0x0ac4 (2756) I 02060000 SeFwRtAvfsFuses                           : 1538
+ 0x0ac8 (2760) I 02060000 SeFwRtAvfsFuses                           : 1538
+ 0x0acc (2764) I 02060000 SeFwRtAvfsFuses                           : 1538
+ 0x0ad0 (2768) I 02060000 SeFwRtAvfsFuses                           : 1538
+ 0x0ad4 (2772) f 00000000 Droop_PWL_F                               : 0
+ 0x0ad8 (2776) f 00000040 Droop_PWL_F                               : 2
+ 0x0adc (2780) f 00002040 Droop_PWL_F                               : 2.5
+ 0x0ae0 (2784) f 00004040 Droop_PWL_F                               : 3
+ 0x0ae4 (2788) f 00006040 Droop_PWL_F                               : 3.5
+ 0x0ae8 (2792) f df32a73d Droop_PWL_a                               : 0.08164
+ 0x0aec (2796) f df32a73d Droop_PWL_a                               : 0.08164
+ 0x0af0 (2800) f df32a73d Droop_PWL_a                               : 0.08164
+ 0x0af4 (2804) f df32a73d Droop_PWL_a                               : 0.08164
+ 0x0af8 (2808) f df32a73d Droop_PWL_a                               : 0.08164
+ 0x0afc (2812) f 1c42953d Droop_PWL_b                               : 0.07288
+ 0x0b00 (2816) f 1c42953d Droop_PWL_b                               : 0.07288
+ 0x0b04 (2820) f 7250c23d Droop_PWL_b                               : 0.09488
+ 0x0b08 (2824) f 1c42953d Droop_PWL_b                               : 0.07288
+ 0x0b0c (2828) f 1c42953d Droop_PWL_b                               : 0.07288
+ 0x0b10 (2832) f 0d8ed2bd Droop_PWL_c                               :-0.10281
+ 0x0b14 (2836) f 0d8ed2bd Droop_PWL_c                               :-0.10281
+ 0x0b18 (2840) f a0e002be Droop_PWL_c                               :-0.12781
+ 0x0b1c (2844) f f2ea1cbd Droop_PWL_c                               :-0.03831
+ 0x0b20 (2848) f f2ea1cbd Droop_PWL_c                               :-0.03831
+ 0x0b24 (2852) I 0ad7233c Static_PWL_Offset                         : 1008981770
+ 0x0b28 (2856) I 0ad7233c Static_PWL_Offset                         : 1008981770
+ 0x0b2c (2860) I 0ad7233c Static_PWL_Offset                         : 1008981770
+ 0x0b30 (2864) I 0ad7233c Static_PWL_Offset                         : 1008981770
+ 0x0b34 (2868) I 0ad7233c Static_PWL_Offset                         : 1008981770
+ 0x0b38 (2872) I 00000000 GbV_dT_vmin                               : 0
+ 0x0b3c (2876) I 00000000 GbV_dT_vmax                               : 0
+ 0x0b40 (2880) I 58020000 V2F_vmin_range_low                        : 600
+ 0x0b44 (2884) I bc020000 V2F_vmin_range_high                       : 700
+ 0x0b48 (2888) I 4c040000 V2F_vmax_range_low                        : 1100
+ 0x0b4c (2892) I b0040000 V2F_vmax_range_high                       : 1200
+ 0x0b50 (2896) B       00 DcBtcEnabled                              : 0
+ 0x0b51 (2897) B       00 Padding                                   : 0
+ 0x0b52 (2898) B       00 Padding                                   : 0
+ 0x0b53 (2899) B       00 Padding                                   : 0
+ 0x0b54 (2900) H     1800 DcTol                                     : 24
+ 0x0b56 (2902) H     0000 DcBtcGb                                   : 0
+ 0x0b58 (2904) H     0000 DcBtcMin                                  : 0
+ 0x0b5a (2906) H     0000 DcBtcMax                                  : 0
+ 0x0b5c (2908) f 00000000 m                                         : 0
+ 0x0b60 (2912) f 00000000 b                                         : 0
+ 0x0b64 (2916) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b68 (2920) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b6c (2924) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b70 (2928) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b74 (2932) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b78 (2936) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b7c (2940) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b80 (2944) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b84 (2948) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b88 (2952) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b8c (2956) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b90 (2960) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b94 (2964) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b98 (2968) I 00000000 GfxAvfsSpare                              : 0
+ 0x0b9c (2972) I 00000000 GfxAvfsSpare                              : 0
+ 0x0ba0 (2976) I 00000000 GfxAvfsSpare                              : 0
+ 0x0ba4 (2980) I 00000000 GfxAvfsSpare                              : 0
+ 0x0ba8 (2984) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bac (2988) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bb0 (2992) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bb4 (2996) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bb8 (3000) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bbc (3004) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bc0 (3008) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bc4 (3012) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bc8 (3016) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bcc (3020) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bd0 (3024) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bd4 (3028) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bd8 (3032) I 00000000 GfxAvfsSpare                              : 0
+ 0x0bdc (3036) I 00000000 GfxAvfsSpare                              : 0
+ 0x0be0 (3040) I 00000000 GfxAvfsSpare                              : 0
+ 0x0be4 (3044) B       00 OverrideSocAvfsFuses                      : 0
+ 0x0be5 (3045) B       01 MinSocAvfsRevision                        : 1
+ 0x0be6 (3046) B       00 SocAvfsPadding                            : 0
+ 0x0be7 (3047) B       00 SocAvfsPadding                            : 0
+ 0x0be8 (3048) H     0000 AvfsTemp                                  : 0
+ 0x0bea (3050) H     5500 AvfsTemp                                  : 85
+ 0x0bec (3052) H     2c01 VftFMin                                   : 300
+ 0x0bee (3054) H     f00a VInversion                                : 2800
+ 0x0bf0 (3056) f dcd7013d a                                         : 0.0317
+ 0x0bf4 (3060) f 399c793d b                                         : 0.06094
+ 0x0bf8 (3064) f 5e80ed3e c                                         : 0.46387
+ 0x0bfc (3068) f d8b6283d a                                         : 0.04119
+ 0x0c00 (3072) f e223623d b                                         : 0.05521
+ 0x0c04 (3076) f a1dbdb3e c                                         : 0.42941
+ 0x0c08 (3080) f 00000000 a                                         : 0
+ 0x0c0c (3084) f 00000000 b                                         : 0
+ 0x0c10 (3088) f a69b443d c                                         : 0.048
+ 0x0c14 (3092) f 00000000 a                                         : 0
+ 0x0c18 (3096) f 00000000 b                                         : 0
+ 0x0c1c (3100) f 00000000 c                                         : 0
+ 0x0c20 (3104) H     0000 AvfsTemp                                  : 0
+ 0x0c22 (3106) H     5500 AvfsTemp                                  : 85
+ 0x0c24 (3108) H     2c01 VftFMin                                   : 300
+ 0x0c26 (3110) H     f00a VInversion                                : 2800
+ 0x0c28 (3112) f dcd7013d a                                         : 0.0317
+ 0x0c2c (3116) f 399c793d b                                         : 0.06094
+ 0x0c30 (3120) f 5e80ed3e c                                         : 0.46387
+ 0x0c34 (3124) f d8b6283d a                                         : 0.04119
+ 0x0c38 (3128) f e223623d b                                         : 0.05521
+ 0x0c3c (3132) f a1dbdb3e c                                         : 0.42941
+ 0x0c40 (3136) f 00000000 a                                         : 0
+ 0x0c44 (3140) f 00000000 b                                         : 0
+ 0x0c48 (3144) f a69b443d c                                         : 0.048
+ 0x0c4c (3148) f 00000000 a                                         : 0
+ 0x0c50 (3152) f 00000000 b                                         : 0
+ 0x0c54 (3156) f 00000000 c                                         : 0
+ 0x0c58 (3160) H     0000 AvfsTemp                                  : 0
+ 0x0c5a (3162) H     5500 AvfsTemp                                  : 85
+ 0x0c5c (3164) H     2c01 VftFMin                                   : 300
+ 0x0c5e (3166) H     f00a VInversion                                : 2800
+ 0x0c60 (3168) f dcd7013d a                                         : 0.0317
+ 0x0c64 (3172) f 399c793d b                                         : 0.06094
+ 0x0c68 (3176) f 5e80ed3e c                                         : 0.46387
+ 0x0c6c (3180) f d8b6283d a                                         : 0.04119
+ 0x0c70 (3184) f e223623d b                                         : 0.05521
+ 0x0c74 (3188) f a1dbdb3e c                                         : 0.42941
+ 0x0c78 (3192) f 00000000 a                                         : 0
+ 0x0c7c (3196) f 00000000 b                                         : 0
+ 0x0c80 (3200) f a69b443d c                                         : 0.048
+ 0x0c84 (3204) f 00000000 a                                         : 0
+ 0x0c88 (3208) f 00000000 b                                         : 0
+ 0x0c8c (3212) f 00000000 c                                         : 0
+ 0x0c90 (3216) f 0000c03f a                                         : 1.5
+ 0x0c94 (3220) f e4839ebd b                                         :-0.0774
+ 0x0c98 (3224) f 9cc440bf c                                         :-0.753
+ 0x0c9c (3228) f 0000c03f a                                         : 1.5
+ 0x0ca0 (3232) f e4839ebd b                                         :-0.0774
+ 0x0ca4 (3236) f 9cc440bf c                                         :-0.753
+ 0x0ca8 (3240) f 0000c03f a                                         : 1.5
+ 0x0cac (3244) f e4839ebd b                                         :-0.0774
+ 0x0cb0 (3248) f 9cc440bf c                                         :-0.753
+ 0x0cb4 (3252) f 00000000 m                                         : 0
+ 0x0cb8 (3256) f 00000000 b                                         : 0
+ 0x0cbc (3260) f 00000000 m                                         : 0
+ 0x0cc0 (3264) f 00000000 b                                         : 0
+ 0x0cc4 (3268) f 00000000 m                                         : 0
+ 0x0cc8 (3272) f 00000000 b                                         : 0
+ 0x0ccc (3276) f 00000000 a                                         : 0
+ 0x0cd0 (3280) f 00000000 b                                         : 0
+ 0x0cd4 (3284) f 00000000 c                                         : 0
+ 0x0cd8 (3288) f 00000000 a                                         : 0
+ 0x0cdc (3292) f 00000000 b                                         : 0
+ 0x0ce0 (3296) f 00000000 c                                         : 0
+ 0x0ce4 (3300) f 00000000 a                                         : 0
+ 0x0ce8 (3304) f 00000000 b                                         : 0
+ 0x0cec (3308) f 00000000 c                                         : 0
+ 0x0cf0 (3312) B       01 DcBtcEnabled                              : 1
+ 0x0cf1 (3313) B       00 Padding                                   : 0
+ 0x0cf2 (3314) B       00 Padding                                   : 0
+ 0x0cf3 (3315) B       00 Padding                                   : 0
+ 0x0cf4 (3316) H     b400 DcTol                                     : 180
+ 0x0cf6 (3318) H     1800 DcBtcGb                                   : 24
+ 0x0cf8 (3320) H     0000 DcBtcMin                                  : 0
+ 0x0cfa (3322) H     b400 DcBtcMax                                  : 180
+ 0x0cfc (3324) f 00002040 m                                         : 2.5
+ 0x0d00 (3328) f 00000000 b                                         : 0
+ 0x0d04 (3332) B       01 DcBtcEnabled                              : 1
+ 0x0d05 (3333) B       00 Padding                                   : 0
+ 0x0d06 (3334) B       00 Padding                                   : 0
+ 0x0d07 (3335) B       00 Padding                                   : 0
+ 0x0d08 (3336) H     b400 DcTol                                     : 180
+ 0x0d0a (3338) H     1800 DcBtcGb                                   : 24
+ 0x0d0c (3340) H     0000 DcBtcMin                                  : 0
+ 0x0d0e (3342) H     b400 DcBtcMax                                  : 180
+ 0x0d10 (3344) f 00009040 m                                         : 4.5
+ 0x0d14 (3348) f 00000000 b                                         : 0
+ 0x0d18 (3352) B       00 DcBtcEnabled                              : 0
+ 0x0d19 (3353) B       00 Padding                                   : 0
+ 0x0d1a (3354) B       00 Padding                                   : 0
+ 0x0d1b (3355) B       00 Padding                                   : 0
+ 0x0d1c (3356) H     0000 DcTol                                     : 0
+ 0x0d1e (3358) H     0000 DcBtcGb                                   : 0
+ 0x0d20 (3360) H     0000 DcBtcMin                                  : 0
+ 0x0d22 (3362) H     0000 DcBtcMax                                  : 0
+ 0x0d24 (3364) f 00000000 m                                         : 0
+ 0x0d28 (3368) f 00000000 b                                         : 0
+ 0x0d2c (3372) I 00000000 SocAvfsSpare                              : 0
+ 0x0d30 (3376) I 00000000 SocAvfsSpare                              : 0
+ 0x0d34 (3380) I 00000000 SocAvfsSpare                              : 0
+ 0x0d38 (3384) I 00000000 SocAvfsSpare                              : 0
+ 0x0d3c (3388) I 00000000 SocAvfsSpare                              : 0
+ 0x0d40 (3392) I 00000000 SocAvfsSpare                              : 0
+ 0x0d44 (3396) I 00000000 SocAvfsSpare                              : 0
+ 0x0d48 (3400) I 00000000 SocAvfsSpare                              : 0
+ 0x0d4c (3404) I 00000000 SocAvfsSpare                              : 0
+ 0x0d50 (3408) I 00000000 SocAvfsSpare                              : 0
+ 0x0d54 (3412) I 00000000 SocAvfsSpare                              : 0
+ 0x0d58 (3416) I 00000000 SocAvfsSpare                              : 0
+ 0x0d5c (3420) I 00000000 SocAvfsSpare                              : 0
+ 0x0d60 (3424) I 00000000 SocAvfsSpare                              : 0
+ 0x0d64 (3428) I 00000000 SocAvfsSpare                              : 0
+ 0x0d68 (3432) I 00000000 SocAvfsSpare                              : 0
+ 0x0d6c (3436) I 00000000 SocAvfsSpare                              : 0
+ 0x0d70 (3440) I 00000000 SocAvfsSpare                              : 0
+ 0x0d74 (3444) I 00000000 SocAvfsSpare                              : 0
+ 0x0d78 (3448) I 00000000 SocAvfsSpare                              : 0
+ 0x0d7c (3452) I 00000000 SocAvfsSpare                              : 0
+ 0x0d80 (3456) I 00000000 SocAvfsSpare                              : 0
+ 0x0d84 (3460) I 00000000 SocAvfsSpare                              : 0
+ 0x0d88 (3464) I 00000000 SocAvfsSpare                              : 0
+ 0x0d8c (3468) I 00000000 SocAvfsSpare                              : 0
+ 0x0d90 (3472) I 00000000 SocAvfsSpare                              : 0
+ 0x0d94 (3476) I 00000000 SocAvfsSpare                              : 0
+ 0x0d98 (3480) I 00000000 SocAvfsSpare                              : 0
+ 0x0d9c (3484) I 00000000 SocAvfsSpare                              : 0
+ 0x0da0 (3488) I 00000000 SocAvfsSpare                              : 0
+ 0x0da4 (3492) I 00000000 SocAvfsSpare                              : 0
+ 0x0da8 (3496) I 00000000 SocAvfsSpare                              : 0
+ 0x0dac (3500) H     b004 InitGfxclk_bypass                         : 1200
+ 0x0dae (3502) H     5802 InitSocclk                                : 600
+ 0x0db0 (3504) H     d002 InitMp0clk                                : 720
+ 0x0db2 (3506) H     f401 InitMpioclk                               : 500
+ 0x0db4 (3508) H     f401 InitSmnclk                                : 500
+ 0x0db6 (3510) H     e803 InitUcpclk                                : 1000
+ 0x0db8 (3512) H     9001 InitCsrclk                                : 400
+ 0x0dba (3514) H     cd02 InitDprefclk                              : 717
+ 0x0dbc (3516) H     9602 InitDcfclk                                : 662
+ 0x0dbe (3518) H     0000 InitDtbclk                                : 0
+ 0x0dc0 (3520) H     0102 InitDclk                                  : 513
+ 0x0dc2 (3522) H     0102 InitVclk                                  : 513
+ 0x0dc4 (3524) H     a002 InitUsbdfsclk                             : 672
+ 0x0dc6 (3526) H     fd01 InitMp1clk                                : 509
+ 0x0dc8 (3528) H     6f02 InitLclk                                  : 623
+ 0x0dca (3530) H     9001 InitBaco400clk_bypass                     : 400
+ 0x0dcc (3532) H     b004 InitBaco1200clk_bypass                    : 1200
+ 0x0dce (3534) H     bc02 InitBaco700clk_bypass                     : 700
+ 0x0dd0 (3536) H     e803 InitFclk                                  : 1000
+ 0x0dd2 (3538) H     0000 InitGfxclk_clkb                           : 0
+ 0x0dd4 (3540) B       00 InitUclkDPMState                          : 0
+ 0x0dd5 (3541) B       00 Padding                                   : 0
+ 0x0dd6 (3542) B       00 Padding                                   : 0
+ 0x0dd7 (3543) B       00 Padding                                   : 0
+ 0x0dd8 (3544) I 94110000 InitVcoFreqPll0                           : 4500
+ 0x0ddc (3548) I cc100000 InitVcoFreqPll1                           : 4300
+ 0x0de0 (3552) I 00000000 InitVcoFreqPll2                           : 0
+ 0x0de4 (3556) I 04100000 InitVcoFreqPll3                           : 4100
+ 0x0de8 (3560) I a00f0000 InitVcoFreqPll4                           : 4000
+ 0x0dec (3564) I 68100000 InitVcoFreqPll5                           : 4200
+ 0x0df0 (3568) I 00000000 InitVcoFreqPll6                           : 0
+ 0x0df4 (3572) H     0000 InitGfx                                   : 0
+ 0x0df6 (3574) H     800c InitSoc                                   : 3200
+ 0x0df8 (3576) H     480d InitU                                     : 3400
+ 0x0dfa (3578) H     0000 Padding2                                  : 0
+ 0x0dfc (3580) I 00000000 Spare                                     : 0
+ 0x0e00 (3584) I 00000000 Spare                                     : 0
+ 0x0e04 (3588) I 00000000 Spare                                     : 0
+ 0x0e08 (3592) I 00000000 Spare                                     : 0
+ 0x0e0c (3596) I 00000000 Spare                                     : 0
+ 0x0e10 (3600) I 00000000 Spare                                     : 0
+ 0x0e14 (3604) I 00000000 Spare                                     : 0
+ 0x0e18 (3608) I 00000000 Spare                                     : 0
+ 0x0e1c (3612) H     1b08 BaseClockAc                               : 2075
+ 0x0e1e (3614) H     d309 GameClockAc                               : 2515
+ 0x0e20 (3616) H     390a BoostClockAc                              : 2617
+ 0x0e22 (3618) H     0000 BaseClockDc                               : 0
+ 0x0e24 (3620) H     0000 GameClockDc                               : 0
+ 0x0e26 (3622) H     0000 BoostClockDc                              : 0
+ 0x0e28 (3624) I 00000000 Reserved                                  : 0
+ 0x0e2c (3628) I 00000000 Reserved                                  : 0
+ 0x0e30 (3632) I 00000000 Reserved                                  : 0
+ 0x0e34 (3636) I 00000000 Reserved                                  : 0
+ 0x0e38 (3640) H     5e01 Power                                     : 350
+ 0x0e3a (3642) H     0000 Power                                     : 0
+ 0x0e3c (3644) H     b004 Power                                     : 1200
+ 0x0e3e (3646) H     0000 Power                                     : 0
+ 0x0e40 (3648) H     0000 Power                                     : 0
+ 0x0e42 (3650) H     0000 Power                                     : 0
+ 0x0e44 (3652) H     0000 Power                                     : 0
+ 0x0e46 (3654) H     0000 Power                                     : 0
+ 0x0e48 (3656) H     c001 Tdc                                       : 448
+ 0x0e4a (3658) H     5200 Tdc                                       : 82
+ 0x0e4c (3660) H     5600 Tdc                                       : 86
+ 0x0e4e (3662) H     6400 Temperature                               : 100
+ 0x0e50 (3664) H     6e00 Temperature                               : 110
+ 0x0e52 (3666) H     6e00 Temperature                               : 110
+ 0x0e54 (3668) H     6e00 Temperature                               : 110
+ 0x0e56 (3670) H     6e00 Temperature                               : 110
+ 0x0e58 (3672) H     7300 Temperature                               : 115
+ 0x0e5a (3674) H     7300 Temperature                               : 115
+ 0x0e5c (3676) H     7300 Temperature                               : 115
+ 0x0e5e (3678) H     7300 Temperature                               : 115
+ 0x0e60 (3680) H     7300 Temperature                               : 115
+ 0x0e62 (3682) H     0000 Temperature                               : 0
+ 0x0e64 (3684) H     0000 Temperature                               : 0
+ 0x0e66 (3686) H     0000 Temperature                               : 0
+ 0x0e68 (3688) B       00 PwmLimitMin                               : 0
+ 0x0e69 (3689) B       ff PwmLimitMax                               : 255
+ 0x0e6a (3690) B       6e FanTargetTemperature                      : 110
+ 0x0e6b (3691) B       00 Spare1                                    : 0
+ 0x0e6c (3692) H     f401 AcousticTargetRpmThresholdMin             : 500
+ 0x0e6e (3694) H     7017 AcousticTargetRpmThresholdMax             : 6000
+ 0x0e70 (3696) H     f401 AcousticLimitRpmThresholdMin              : 500
+ 0x0e72 (3698) H     7017 AcousticLimitRpmThresholdMax              : 6000
+ 0x0e74 (3700) H     0000 PccLimitMin                               : 0
+ 0x0e76 (3702) H     c201 PccLimitMax                               : 450
+ 0x0e78 (3704) H     1900 FanStopTempMin                            : 25
+ 0x0e7a (3706) H     6400 FanStopTempMax                            : 100
+ 0x0e7c (3708) H     1900 FanStartTempMin                           : 25
+ 0x0e7e (3710) H     6400 FanStartTempMax                           : 100
+ 0x0e80 (3712) H     0000 PowerMinPpt0                              : 0
+ 0x0e82 (3714) H     0000 PowerMinPpt0                              : 0
+ 0x0e84 (3716) I 00000000 Spare                                     : 0
+ 0x0e88 (3720) I 00000000 Spare                                     : 0
+ 0x0e8c (3724) I 00000000 Spare                                     : 0
+ 0x0e90 (3728) I 00000000 Spare                                     : 0
+ 0x0e94 (3732) I 00000000 Spare                                     : 0
+ 0x0e98 (3736) I 00000000 Spare                                     : 0
+ 0x0e9c (3740) I 00000000 Spare                                     : 0
+ 0x0ea0 (3744) I 00000000 Spare                                     : 0
+ 0x0ea4 (3748) I 00000000 Spare                                     : 0
+ 0x0ea8 (3752) I 00000000 Spare                                     : 0
+ 0x0eac (3756) I 00000000 Spare                                     : 0
+ 0x0eb0 (3760) I cd070000 FeatureCtrlMask                           : 1997
+ 0x0eb4 (3764) h     3efe VoltageOffsetPerZoneBoundary              :-450
+ 0x0eb6 (3766) H     0000 Reserved1                                 : 0
+ 0x0eb8 (3768) H     0000 Reserved2                                 : 0
+ 0x0eba (3770) h     f401 GfxclkFmin                                : 500
+ 0x0ebc (3772) h     f401 GfxclkFmax                                : 500
+ 0x0ebe (3774) H     6100 UclkFmin                                  : 97
+ 0x0ec0 (3776) H     6100 UclkFmax                                  : 97
+ 0x0ec2 (3778) h     f6ff Ppt                                       :-10
+ 0x0ec4 (3780) h     f6ff Tdc                                       :-10
+ 0x0ec6 (3782) B       0f FanLinearPwmPoints                        : 15
+ 0x0ec7 (3783) B       19 FanLinearTempPoints                       : 25
+ 0x0ec8 (3784) H     0f00 FanMinimumPwm                             : 15
+ 0x0eca (3786) H     f401 AcousticTargetRpmThreshold                : 500
+ 0x0ecc (3788) H     f401 AcousticLimitRpmThreshold                 : 500
+ 0x0ece (3790) H     1900 FanTargetTemperature                      : 25
+ 0x0ed0 (3792) B       00 FanZeroRpmEnable                          : 0
+ 0x0ed1 (3793) B       19 FanZeroRpmStopTemp                        : 25
+ 0x0ed2 (3794) B       00 FanMode                                   : 0
+ 0x0ed3 (3795) B       32 MaxOpTemp                                 : 50
+ 0x0ed4 (3796) B       00 Padding                                   : 0
+ 0x0ed5 (3797) B       00 Padding                                   : 0
+ 0x0ed6 (3798) B       00 Padding                                   : 0
+ 0x0ed7 (3799) B       00 Padding                                   : 0
+ 0x0ed8 (3800) I 00000000 Spare                                     : 0
+ 0x0edc (3804) I 00000000 Spare                                     : 0
+ 0x0ee0 (3808) I 00000000 Spare                                     : 0
+ 0x0ee4 (3812) I 00000000 Spare                                     : 0
+ 0x0ee8 (3816) I 00000000 Spare                                     : 0
+ 0x0eec (3820) I 00000000 Spare                                     : 0
+ 0x0ef0 (3824) I 00000000 Spare                                     : 0
+ 0x0ef4 (3828) I 00000000 Spare                                     : 0
+ 0x0ef8 (3832) I 00000000 Spare                                     : 0
+ 0x0efc (3836) I 00000000 Spare                                     : 0
+ 0x0f00 (3840) I 00000000 Spare                                     : 0
+ 0x0f04 (3844) I 00000000 Spare                                     : 0
+ 0x0f08 (3848) I cd070000 FeatureCtrlMask                           : 1997
+ 0x0f0c (3852) h     0000 VoltageOffsetPerZoneBoundary              : 0
+ 0x0f0e (3854) H     0000 Reserved1                                 : 0
+ 0x0f10 (3856) H     0000 Reserved2                                 : 0
+ 0x0f12 (3858) h     8813 GfxclkFmin                                : 5000
+ 0x0f14 (3860) h     8813 GfxclkFmax                                : 5000
+ 0x0f16 (3862) H     dc05 UclkFmin                                  : 1500
+ 0x0f18 (3864) H     dc05 UclkFmax                                  : 1500
+ 0x0f1a (3866) h     0f00 Ppt                                       : 15
+ 0x0f1c (3868) h     0000 Tdc                                       : 0
+ 0x0f1e (3870) B       64 FanLinearPwmPoints                        : 100
+ 0x0f1f (3871) B       64 FanLinearTempPoints                       : 100
+ 0x0f20 (3872) H     6400 FanMinimumPwm                             : 100
+ 0x0f22 (3874) H     e40c AcousticTargetRpmThreshold                : 3300
+ 0x0f24 (3876) H     e40c AcousticLimitRpmThreshold                 : 3300
+ 0x0f26 (3878) H     6900 FanTargetTemperature                      : 105
+ 0x0f28 (3880) B       01 FanZeroRpmEnable                          : 1
+ 0x0f29 (3881) B       64 FanZeroRpmStopTemp                        : 100
+ 0x0f2a (3882) B       01 FanMode                                   : 1
+ 0x0f2b (3883) B       6e MaxOpTemp                                 : 110
+ 0x0f2c (3884) B       00 Padding                                   : 0
+ 0x0f2d (3885) B       00 Padding                                   : 0
+ 0x0f2e (3886) B       00 Padding                                   : 0
+ 0x0f2f (3887) B       00 Padding                                   : 0
+ 0x0f30 (3888) I 00000000 Spare                                     : 0
+ 0x0f34 (3892) I 00000000 Spare                                     : 0
+ 0x0f38 (3896) I 00000000 Spare                                     : 0
+ 0x0f3c (3900) I 00000000 Spare                                     : 0
+ 0x0f40 (3904) I 00000000 Spare                                     : 0
+ 0x0f44 (3908) I 00000000 Spare                                     : 0
+ 0x0f48 (3912) I 00000000 Spare                                     : 0
+ 0x0f4c (3916) I 00000000 Spare                                     : 0
+ 0x0f50 (3920) I b0045802 Spare                                     : 39322800
+ 0x0f54 (3924) I d002f401 Spare                                     : 32768720
+ 0x0f58 (3928) I f401e803 Spare                                     : 65536500
+ 0x0f5c (3932) I 9001bc02 Spare                                     : 45875600
+ 0x0f60 (3936) I 00000000 FeatureCtrlMask                           : 0
+ 0x0f64 (3940) h     0000 VoltageOffsetPerZoneBoundary              : 0
+ 0x0f66 (3942) H     0000 Reserved1                                 : 0
+ 0x0f68 (3944) H     0000 Reserved2                                 : 0
+ 0x0f6a (3946) h     0000 GfxclkFmin                                : 0
+ 0x0f6c (3948) h     0000 GfxclkFmax                                : 0
+ 0x0f6e (3950) H     0000 UclkFmin                                  : 0
+ 0x0f70 (3952) H     0000 UclkFmax                                  : 0
+ 0x0f72 (3954) h     0000 Ppt                                       : 0
+ 0x0f74 (3956) h     0000 Tdc                                       : 0
+ 0x0f76 (3958) B       00 FanLinearPwmPoints                        : 0
+ 0x0f77 (3959) B       00 FanLinearTempPoints                       : 0
+ 0x0f78 (3960) H     0000 FanMinimumPwm                             : 0
+ 0x0f7a (3962) H     0000 AcousticTargetRpmThreshold                : 0
+ 0x0f7c (3964) H     0000 AcousticLimitRpmThreshold                 : 0
+ 0x0f7e (3966) H     0000 FanTargetTemperature                      : 0
+ 0x0f80 (3968) B       00 FanZeroRpmEnable                          : 0
+ 0x0f81 (3969) B       00 FanZeroRpmStopTemp                        : 0
+ 0x0f82 (3970) B       00 FanMode                                   : 0
+ 0x0f83 (3971) B       00 MaxOpTemp                                 : 0
+ 0x0f84 (3972) B       00 Padding                                   : 0
+ 0x0f85 (3973) B       00 Padding                                   : 0
+ 0x0f86 (3974) B       00 Padding                                   : 0
+ 0x0f87 (3975) B       00 Padding                                   : 0
+ 0x0f88 (3976) I 00000000 Spare                                     : 0
+ 0x0f8c (3980) I 00000000 Spare                                     : 0
+ 0x0f90 (3984) I 68100000 Spare                                     : 4200
+ 0x0f94 (3988) I 00000000 Spare                                     : 0
+ 0x0f98 (3992) I 0000bc02 Spare                                     : 45875200
+ 0x0f9c (3996) I ee020000 Spare                                     : 750
+ 0x0fa0 (4000) I 00000000 Spare                                     : 0
+ 0x0fa4 (4004) I 00000000 Spare                                     : 0
+ 0x0fa8 (4008) I 00000000 Spare                                     : 0
+ 0x0fac (4012) I 00000000 Spare                                     : 0
+ 0x0fb0 (4016) I 00000000 Spare                                     : 0
+ 0x0fb4 (4020) I 00000000 Spare                                     : 0
+ 0x0fb8 (4024) I 00000000 DebugOverrides                            : 0
+ 0x0fbc (4028) B       01 TotalBoardPowerSupport                    : 1
+ 0x0fbd (4029) B       00 TotalBoardPowerPadding                    : 0
+ 0x0fbe (4030) B       00 TotalBoardPowerPadding                    : 0
+ 0x0fbf (4031) B       00 TotalBoardPowerPadding                    : 0
+ 0x0fc0 (4032) h     6d03 TotalIdleBoardPowerM                      : 877
+ 0x0fc2 (4034) h     0000 TotalIdleBoardPowerB                      : 0
+ 0x0fc4 (4036) h     9b04 TotalBoardPowerM                          : 1179
+ 0x0fc6 (4038) h     b30f TotalBoardPowerB                          : 4019
+ 0x0fc8 (4040) f 8f368ebd a                                         :-0.06944
+ 0x0fcc (4044) f 54553c42 b                                         : 47.0833
+ 0x0fd0 (4048) f 007daac5 c                                         :-5455.62
+ 0x0fd4 (4052) f 00000000 a                                         : 0
+ 0x0fd8 (4056) f 00000000 b                                         : 0
+ 0x0fdc (4060) f 00000000 c                                         : 0
+ 0x0fe0 (4064) f 3ecbf3bb a                                         :-0.00744
+ 0x0fe4 (4068) f 52550a41 b                                         : 8.64583
+ 0x0fe8 (4072) f 4af22f42 c                                         : 43.9866
+ 0x0fec (4076) f 00000000 a                                         : 0
+ 0x0ff0 (4080) f 00000000 b                                         : 0
+ 0x0ff4 (4084) f 00000000 c                                         : 0
+ 0x0ff8 (4088) f f7af2c3d a                                         : 0.04216
+ 0x0ffc (4092) f a92ab6c1 b                                         :-22.7708
+ 0x1000 (4096) f 9b98ad45 c                                         : 5555.08
+ 0x1004 (4100) f 00000000 a                                         : 0
+ 0x1008 (4104) f 00000000 b                                         : 0
+ 0x100c (4108) f 00000000 c                                         : 0
+ 0x1010 (4112) I 00000000 Spare                                     : 0
+ 0x1014 (4116) I 00000000 Spare                                     : 0
+ 0x1018 (4120) I 00000000 Spare                                     : 0
+ 0x101c (4124) I 00000000 Spare                                     : 0
+ 0x1020 (4128) I 00000000 Spare                                     : 0
+ 0x1024 (4132) I 00000000 Spare                                     : 0
+ 0x1028 (4136) I 00000000 Spare                                     : 0
+ 0x102c (4140) I 00000000 Spare                                     : 0
+ 0x1030 (4144) I 00000000 Spare                                     : 0
+ 0x1034 (4148) I 00000000 Spare                                     : 0
+ 0x1038 (4152) I 00000000 Spare                                     : 0
+ 0x103c (4156) I 00000000 Spare                                     : 0
+ 0x1040 (4160) I 00000000 Spare                                     : 0
+ 0x1044 (4164) I 00000000 Spare                                     : 0
+ 0x1048 (4168) I 00000000 Spare                                     : 0
+ 0x104c (4172) I 00000000 Spare                                     : 0
+ 0x1050 (4176) I 00000000 Spare                                     : 0
+ 0x1054 (4180) I 00000000 Spare                                     : 0
+ 0x1058 (4184) I 00000000 Spare                                     : 0
+ 0x105c (4188) I 00000000 Spare                                     : 0
+ 0x1060 (4192) I 00000000 Spare                                     : 0
+ 0x1064 (4196) I 00000000 Spare                                     : 0
+ 0x1068 (4200) I 00000000 Spare                                     : 0
+ 0x106c (4204) I 00000000 Spare                                     : 0
+ 0x1070 (4208) I 00000000 Spare                                     : 0
+ 0x1074 (4212) I 00000000 Spare                                     : 0
+ 0x1078 (4216) I 00000000 Spare                                     : 0
+ 0x107c (4220) I 00000000 Spare                                     : 0
+ 0x1080 (4224) I 00000000 Spare                                     : 0
+ 0x1084 (4228) I 00000000 Spare                                     : 0
+ 0x1088 (4232) I 00000000 Spare                                     : 0
+ 0x108c (4236) I 00000000 Spare                                     : 0
+ 0x1090 (4240) I 00000000 Spare                                     : 0
+ 0x1094 (4244) I 00000000 Spare                                     : 0
+ 0x1098 (4248) I 00000000 Spare                                     : 0
+ 0x109c (4252) I 00000000 Spare                                     : 0
+ 0x10a0 (4256) I 00000000 Spare                                     : 0
+ 0x10a4 (4260) I 00000000 Spare                                     : 0
+ 0x10a8 (4264) I 00000000 Spare                                     : 0
+ 0x10ac (4268) I 00000000 Spare                                     : 0
+ 0x10b0 (4272) I 00000000 Spare                                     : 0
+ 0x10b4 (4276) I 00000000 Spare                                     : 0
+ 0x10b8 (4280) I 00000000 Spare                                     : 0
+ 0x10bc (4284) I 00000000 MmHubPadding                              : 0
+ 0x10c0 (4288) I 00000000 MmHubPadding                              : 0
+ 0x10c4 (4292) I 00000000 MmHubPadding                              : 0
+ 0x10c8 (4296) I 00000000 MmHubPadding                              : 0
+ 0x10cc (4300) I 00000000 MmHubPadding                              : 0
+ 0x10d0 (4304) I 00000000 MmHubPadding                              : 0
+ 0x10d4 (4308) I 00000000 MmHubPadding                              : 0
+ 0x10d8 (4312) I 00000000 MmHubPadding                              : 0
+ 0x10dc (4316) I 26000000 Version                                   : 38
+ 0x10e0 (4320) B       00 Enabled                                   : 0
+ 0x10e1 (4321) B       00 Speed                                     : 0
+ 0x10e2 (4322) B       00 SlaveAddress                              : 0
+ 0x10e3 (4323) B       00 ControllerPort                            : 0
+ 0x10e4 (4324) B       00 ControllerName                            : 0
+ 0x10e5 (4325) B       00 ThermalThrotter                           : 0
+ 0x10e6 (4326) B       00 I2cProtocol                               : 0
+ 0x10e7 (4327) B       00 PaddingConfig                             : 0
+ 0x10e8 (4328) B       00 Enabled                                   : 0
+ 0x10e9 (4329) B       00 Speed                                     : 0
+ 0x10ea (4330) B       00 SlaveAddress                              : 0
+ 0x10eb (4331) B       00 ControllerPort                            : 0
+ 0x10ec (4332) B       00 ControllerName                            : 0
+ 0x10ed (4333) B       00 ThermalThrotter                           : 0
+ 0x10ee (4334) B       00 I2cProtocol                               : 0
+ 0x10ef (4335) B       00 PaddingConfig                             : 0
+ 0x10f0 (4336) B       00 Enabled                                   : 0
+ 0x10f1 (4337) B       00 Speed                                     : 0
+ 0x10f2 (4338) B       00 SlaveAddress                              : 0
+ 0x10f3 (4339) B       00 ControllerPort                            : 0
+ 0x10f4 (4340) B       00 ControllerName                            : 0
+ 0x10f5 (4341) B       00 ThermalThrotter                           : 0
+ 0x10f6 (4342) B       00 I2cProtocol                               : 0
+ 0x10f7 (4343) B       00 PaddingConfig                             : 0
+ 0x10f8 (4344) B       00 Enabled                                   : 0
+ 0x10f9 (4345) B       00 Speed                                     : 0
+ 0x10fa (4346) B       00 SlaveAddress                              : 0
+ 0x10fb (4347) B       00 ControllerPort                            : 0
+ 0x10fc (4348) B       00 ControllerName                            : 0
+ 0x10fd (4349) B       00 ThermalThrotter                           : 0
+ 0x10fe (4350) B       00 I2cProtocol                               : 0
+ 0x10ff (4351) B       00 PaddingConfig                             : 0
+ 0x1100 (4352) B       00 Enabled                                   : 0
+ 0x1101 (4353) B       00 Speed                                     : 0
+ 0x1102 (4354) B       00 SlaveAddress                              : 0
+ 0x1103 (4355) B       00 ControllerPort                            : 0
+ 0x1104 (4356) B       00 ControllerName                            : 0
+ 0x1105 (4357) B       00 ThermalThrotter                           : 0
+ 0x1106 (4358) B       00 I2cProtocol                               : 0
+ 0x1107 (4359) B       00 PaddingConfig                             : 0
+ 0x1108 (4360) B       00 Enabled                                   : 0
+ 0x1109 (4361) B       00 Speed                                     : 0
+ 0x110a (4362) B       00 SlaveAddress                              : 0
+ 0x110b (4363) B       00 ControllerPort                            : 0
+ 0x110c (4364) B       00 ControllerName                            : 0
+ 0x110d (4365) B       00 ThermalThrotter                           : 0
+ 0x110e (4366) B       00 I2cProtocol                               : 0
+ 0x110f (4367) B       00 PaddingConfig                             : 0
+ 0x1110 (4368) B       00 Enabled                                   : 0
+ 0x1111 (4369) B       00 Speed                                     : 0
+ 0x1112 (4370) B       00 SlaveAddress                              : 0
+ 0x1113 (4371) B       00 ControllerPort                            : 0
+ 0x1114 (4372) B       00 ControllerName                            : 0
+ 0x1115 (4373) B       00 ThermalThrotter                           : 0
+ 0x1116 (4374) B       00 I2cProtocol                               : 0
+ 0x1117 (4375) B       00 PaddingConfig                             : 0
+ 0x1118 (4376) B       00 Enabled                                   : 0
+ 0x1119 (4377) B       00 Speed                                     : 0
+ 0x111a (4378) B       00 SlaveAddress                              : 0
+ 0x111b (4379) B       00 ControllerPort                            : 0
+ 0x111c (4380) B       00 ControllerName                            : 0
+ 0x111d (4381) B       00 ThermalThrotter                           : 0
+ 0x111e (4382) B       00 I2cProtocol                               : 0
+ 0x111f (4383) B       00 PaddingConfig                             : 0
+ 0x1120 (4384) B       00 VddGfxVrMapping                           : 0
+ 0x1121 (4385) B       00 VddSocVrMapping                           : 0
+ 0x1122 (4386) B       00 VddMem0VrMapping                          : 0
+ 0x1123 (4387) B       00 VddMem1VrMapping                          : 0
+ 0x1124 (4388) B       00 GfxUlvPhaseSheddingMask                   : 0
+ 0x1125 (4389) B       00 SocUlvPhaseSheddingMask                   : 0
+ 0x1126 (4390) B       00 VmempUlvPhaseSheddingMask                 : 0
+ 0x1127 (4391) B       00 VddioUlvPhaseSheddingMask                 : 0
+ 0x1128 (4392) B       00 SlaveAddrMapping                          : 0
+ 0x1129 (4393) B       00 SlaveAddrMapping                          : 0
+ 0x112a (4394) B       00 SlaveAddrMapping                          : 0
+ 0x112b (4395) B       00 SlaveAddrMapping                          : 0
+ 0x112c (4396) B       00 SlaveAddrMapping                          : 0
+ 0x112d (4397) B       00 VrPsiSupport                              : 0
+ 0x112e (4398) B       00 VrPsiSupport                              : 0
+ 0x112f (4399) B       00 VrPsiSupport                              : 0
+ 0x1130 (4400) B       01 VrPsiSupport                              : 1
+ 0x1131 (4401) B       00 VrPsiSupport                              : 0
+ 0x1132 (4402) B       00 PaddingPsi                                : 0
+ 0x1133 (4403) B       00 PaddingPsi                                : 0
+ 0x1134 (4404) B       00 PaddingPsi                                : 0
+ 0x1135 (4405) B       00 PaddingPsi                                : 0
+ 0x1136 (4406) B       00 PaddingPsi                                : 0
+ 0x1137 (4407) B       00 EnablePsi6                                : 0
+ 0x1138 (4408) B       00 EnablePsi6                                : 0
+ 0x1139 (4409) B       00 EnablePsi6                                : 0
+ 0x113a (4410) B       00 EnablePsi6                                : 0
+ 0x113b (4411) B       00 EnablePsi6                                : 0
+ 0x113c (4412) b       00 Offset                                    : 0
+ 0x113d (4413) B       00 Padding                                   : 0
+ 0x113e (4414) H     0000 MaxCurrent                                : 0
+ 0x1140 (4416) b       00 Offset                                    : 0
+ 0x1141 (4417) B       00 Padding                                   : 0
+ 0x1142 (4418) H     0000 MaxCurrent                                : 0
+ 0x1144 (4420) b       00 Offset                                    : 0
+ 0x1145 (4421) B       00 Padding                                   : 0
+ 0x1146 (4422) H     0000 MaxCurrent                                : 0
+ 0x1148 (4424) b       00 Offset                                    : 0
+ 0x1149 (4425) B       00 Padding                                   : 0
+ 0x114a (4426) H     0000 MaxCurrent                                : 0
+ 0x114c (4428) b       00 Offset                                    : 0
+ 0x114d (4429) B       00 Padding                                   : 0
+ 0x114e (4430) H     0000 MaxCurrent                                : 0
+ 0x1150 (4432) I 00000000 VoltageTelemetryRatio                     : 0
+ 0x1154 (4436) I 00000000 VoltageTelemetryRatio                     : 0
+ 0x1158 (4440) I 00000000 VoltageTelemetryRatio                     : 0
+ 0x115c (4444) I 00000000 VoltageTelemetryRatio                     : 0
+ 0x1160 (4448) I 00000000 VoltageTelemetryRatio                     : 0
+ 0x1164 (4452) B       00 DownSlewRateVr                            : 0
+ 0x1165 (4453) B       00 DownSlewRateVr                            : 0
+ 0x1166 (4454) B       00 DownSlewRateVr                            : 0
+ 0x1167 (4455) B       00 DownSlewRateVr                            : 0
+ 0x1168 (4456) B       00 DownSlewRateVr                            : 0
+ 0x1169 (4457) B       00 LedOffGpio                                : 0
+ 0x116a (4458) B       00 FanOffGpio                                : 0
+ 0x116b (4459) B       00 GfxVrPowerStageOffGpio                    : 0
+ 0x116c (4460) B       00 AcDcGpio                                  : 0
+ 0x116d (4461) B       00 AcDcPolarity                              : 0
+ 0x116e (4462) B       00 VR0HotGpio                                : 0
+ 0x116f (4463) B       00 VR0HotPolarity                            : 0
+ 0x1170 (4464) B       00 GthrGpio                                  : 0
+ 0x1171 (4465) B       00 GthrPolarity                              : 0
+ 0x1172 (4466) B       00 LedPin0                                   : 0
+ 0x1173 (4467) B       00 LedPin1                                   : 0
+ 0x1174 (4468) B       00 LedPin2                                   : 0
+ 0x1175 (4469) B       00 LedEnableMask                             : 0
+ 0x1176 (4470) B       00 LedPcie                                   : 0
+ 0x1177 (4471) B       00 LedError                                  : 0
+ 0x1178 (4472) B       00 UclkTrainingModeSpreadPercent             : 0
+ 0x1179 (4473) B       00 UclkSpreadPadding                         : 0
+ 0x117a (4474) H     0000 UclkSpreadFreq                            : 0
+ 0x117c (4476) B       00 UclkSpreadPercent                         : 0
+ 0x117d (4477) B       00 UclkSpreadPercent                         : 0
+ 0x117e (4478) B       00 UclkSpreadPercent                         : 0
+ 0x117f (4479) B       00 UclkSpreadPercent                         : 0
+ 0x1180 (4480) B       00 UclkSpreadPercent                         : 0
+ 0x1181 (4481) B       00 UclkSpreadPercent                         : 0
+ 0x1182 (4482) B       00 UclkSpreadPercent                         : 0
+ 0x1183 (4483) B       00 UclkSpreadPercent                         : 0
+ 0x1184 (4484) B       00 UclkSpreadPercent                         : 0
+ 0x1185 (4485) B       00 UclkSpreadPercent                         : 0
+ 0x1186 (4486) B       00 UclkSpreadPercent                         : 0
+ 0x1187 (4487) B       00 UclkSpreadPercent                         : 0
+ 0x1188 (4488) B       00 UclkSpreadPercent                         : 0
+ 0x1189 (4489) B       00 UclkSpreadPercent                         : 0
+ 0x118a (4490) B       00 UclkSpreadPercent                         : 0
+ 0x118b (4491) B       00 UclkSpreadPercent                         : 0
+ 0x118c (4492) B       00 FclkSpreadPadding                         : 0
+ 0x118d (4493) B       00 FclkSpreadPercent                         : 0
+ 0x118e (4494) H     0000 FclkSpreadFreq                            : 0
+ 0x1190 (4496) B       00 DramWidth                                 : 0
+ 0x1191 (4497) B       00 PaddingMem1                               : 0
+ 0x1192 (4498) B       00 PaddingMem1                               : 0
+ 0x1193 (4499) B       00 PaddingMem1                               : 0
+ 0x1194 (4500) B       00 PaddingMem1                               : 0
+ 0x1195 (4501) B       00 PaddingMem1                               : 0
+ 0x1196 (4502) B       00 PaddingMem1                               : 0
+ 0x1197 (4503) B       00 PaddingMem1                               : 0
+ 0x1198 (4504) B       00 HsrEnabled                                : 0
+ 0x1199 (4505) B       00 VddqOffEnabled                            : 0
+ 0x119a (4506) B       00 PaddingUmcFlags                           : 0
+ 0x119b (4507) B       00 PaddingUmcFlags                           : 0
+ 0x119c (4508) I 00000000 PostVoltageSetBacoDelay                   : 0
+ 0x11a0 (4512) I 00000000 BacoEntryDelay                            : 0
+ 0x11a4 (4516) B       00 FuseWritePowerMuxPresent                  : 0
+ 0x11a5 (4517) B       00 FuseWritePadding                          : 0
+ 0x11a6 (4518) B       00 FuseWritePadding                          : 0
+ 0x11a7 (4519) B       00 FuseWritePadding                          : 0
+ 0x11a8 (4520) I 00000000 BoardSpare                                : 0
+ 0x11ac (4524) I 00000000 BoardSpare                                : 0
+ 0x11b0 (4528) I 00000000 BoardSpare                                : 0
+ 0x11b4 (4532) I 00000000 BoardSpare                                : 0
+ 0x11b8 (4536) I 00000000 BoardSpare                                : 0
+ 0x11bc (4540) I 00000000 BoardSpare                                : 0
+ 0x11c0 (4544) I 00000000 BoardSpare                                : 0
+ 0x11c4 (4548) I 00000000 BoardSpare                                : 0
+ 0x11c8 (4552) I 00000000 BoardSpare                                : 0
+ 0x11cc (4556) I 00000000 BoardSpare                                : 0
+ 0x11d0 (4560) I 00000000 BoardSpare                                : 0
+ 0x11d4 (4564) I 00000000 BoardSpare                                : 0
+ 0x11d8 (4568) I 00000000 BoardSpare                                : 0
+ 0x11dc (4572) I 00000000 BoardSpare                                : 0
+ 0x11e0 (4576) I 00000000 BoardSpare                                : 0
+ 0x11e4 (4580) I 00000000 BoardSpare                                : 0
+ 0x11e8 (4584) I 00000000 BoardSpare                                : 0
+ 0x11ec (4588) I 00000000 BoardSpare                                : 0
+ 0x11f0 (4592) I 00000000 BoardSpare                                : 0
+ 0x11f4 (4596) I 00000000 BoardSpare                                : 0
+ 0x11f8 (4600) I 00000000 BoardSpare                                : 0
+ 0x11fc (4604) I 00000000 BoardSpare                                : 0
+ 0x1200 (4608) I 00000000 BoardSpare                                : 0
+ 0x1204 (4612) I 00000000 BoardSpare                                : 0
+ 0x1208 (4616) I 00000000 BoardSpare                                : 0
+ 0x120c (4620) I 00000000 BoardSpare                                : 0
+ 0x1210 (4624) I 00000000 BoardSpare                                : 0
+ 0x1214 (4628) I 00000000 BoardSpare                                : 0
+ 0x1218 (4632) I 00000000 BoardSpare                                : 0
+ 0x121c (4636) I 00000000 BoardSpare                                : 0
+ 0x1220 (4640) I 00000000 BoardSpare                                : 0
+ 0x1224 (4644) I 00000000 BoardSpare                                : 0
+ 0x1228 (4648) I 00000000 BoardSpare                                : 0
+ 0x122c (4652) I 00000000 BoardSpare                                : 0
+ 0x1230 (4656) I 00000000 BoardSpare                                : 0
+ 0x1234 (4660) I 00000000 BoardSpare                                : 0
+ 0x1238 (4664) I 00000000 BoardSpare                                : 0
+ 0x123c (4668) I 00000000 BoardSpare                                : 0
+ 0x1240 (4672) I 00000000 BoardSpare                                : 0
+ 0x1244 (4676) I 00000000 BoardSpare                                : 0
+ 0x1248 (4680) I 00000000 BoardSpare                                : 0
+ 0x124c (4684) I 00000000 BoardSpare                                : 0
+ 0x1250 (4688) I 00000000 BoardSpare                                : 0
+ 0x1254 (4692) I 00000000 BoardSpare                                : 0
+ 0x1258 (4696) I 00000000 BoardSpare                                : 0
+ 0x125c (4700) I 00000000 BoardSpare                                : 0
+ 0x1260 (4704) I 00000000 BoardSpare                                : 0
+ 0x1264 (4708) I 00000000 BoardSpare                                : 0
+ 0x1268 (4712) I 00000000 BoardSpare                                : 0
+ 0x126c (4716) I 00000000 BoardSpare                                : 0
+ 0x1270 (4720) I 00000000 BoardSpare                                : 0
+ 0x1274 (4724) I 00000000 BoardSpare                                : 0
+ 0x1278 (4728) I 00000000 BoardSpare                                : 0
+ 0x127c (4732) I 00000000 BoardSpare                                : 0
+ 0x1280 (4736) I 00000000 BoardSpare                                : 0
+ 0x1284 (4740) I 00000000 BoardSpare                                : 0
+ 0x1288 (4744) I 00000000 BoardSpare                                : 0
+ 0x128c (4748) I 00000000 BoardSpare                                : 0
+ 0x1290 (4752) I 00000000 BoardSpare                                : 0
+ 0x1294 (4756) I 00000000 BoardSpare                                : 0
+ 0x1298 (4760) I 00000000 BoardSpare                                : 0
+ 0x129c (4764) I 00000000 BoardSpare                                : 0
+ 0x12a0 (4768) I 00000000 BoardSpare                                : 0
+ 0x12a4 (4772) I 00000000 MmHubPadding                              : 0
+ 0x12a8 (4776) I 00000000 MmHubPadding                              : 0
+ 0x12ac (4780) I 00000000 MmHubPadding                              : 0
+ 0x12b0 (4784) I 00000000 MmHubPadding                              : 0
+ 0x12b4 (4788) I 00000000 MmHubPadding                              : 0
+ 0x12b8 (4792) I 00000000 MmHubPadding                              : 0
+ 0x12bc (4796) I 00000000 MmHubPadding                              : 0
+ 0x12c0 (4800) I 00000000 MmHubPadding                              : 0
```

### Comparing `upp-0.2.0/test/AMD.RXVega64.8176.170719.rom.dump` & `upp-0.2.1/test/AMD.RXVega64.8176.170719.rom.dump`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/test/AMD.RXVega64.8176.170719.rom.rawdump` & `upp-0.2.1/test/AMD.RXVega64.8176.170719.rom.rawdump`

 * *Files 0% similar despite different names*

```diff
@@ -1,342 +1,342 @@
 PowerPlay table rev 8.1 size 694 bytes
- Offset (dec.) t Raw val. Variable name                   Decoded value
------------------------------------------------------------------------
- 0x0000 (0000) H     b602 structuresize                   : 694
- 0x0002 (0002) B       08 format_revision                 : 8
- 0x0003 (0003) B       01 content_revision                : 1
- 0x0004 (0004) B       00 TableRevision                   : 0
- 0x0005 (0005) H     5c00 TableSize                       : 92
- 0x0007 (0007) I e1060000 GoldenPPID                      : 1761
- 0x000b (0011) I ee2b0000 GoldenRevision                  : 11246
- 0x000f (0015) H     1b00 FormatID                        : 27
- 0x0011 (0017) I 48000000 PlatformCaps                    : 72
- 0x0015 (0021) I 80a90300 MaxODEngineClock                : 240000
- 0x0019 (0025) I f0490200 MaxODMemoryClock                : 150000
- 0x001d (0029) H     3200 PowerControlLimit               : 50
- 0x001f (0031) H     0800 UlvVoltageOffset                : 8
- 0x0021 (0033) H     0000 UlvSmnclkDid                    : 0
- 0x0023 (0035) H     0000 UlvMp1clkDid                    : 0
- 0x0025 (0037) H     0000 UlvGfxclkBypass                 : 0
- 0x0027 (0039) H     0000 GfxclkSlewRate                  : 0
- 0x0029 (0041) B       00 GfxVoltageMode                  : 0
- 0x002a (0042) B       00 SocVoltageMode                  : 0
- 0x002b (0043) B       00 UclkVoltageMode                 : 0
- 0x002c (0044) B       00 UvdVoltageMode                  : 0
- 0x002d (0045) B       00 VceVoltageMode                  : 0
- 0x002e (0046) B       02 Mp0VoltageMode                  : 2
- 0x002f (0047) B       01 DcefVoltageMode                 : 1
- 0x0030 (0048) H     5c00 StateArrayOffset                : 92
- 0x005c (0092) B       02 RevId                           : 2
- 0x005d (0093) B       02 NumEntries                      : 2
- 0x005e (0094) B       00 SocClockIndexHigh               : 0
- 0x005f (0095) B       00 SocClockIndexLow                : 0
- 0x0060 (0096) B       00 GfxClockIndexHigh               : 0
- 0x0061 (0097) B       00 GfxClockIndexLow                : 0
- 0x0062 (0098) B       00 MemClockIndexHigh               : 0
- 0x0063 (0099) B       00 MemClockIndexLow                : 0
- 0x0064 (0100) H     0800 Classification                  : 8
- 0x0066 (0102) I 00000000 CapsAndSettings                 : 0
- 0x006a (0106) H     0000 Classification2                 : 0
- 0x006c (0108) B       05 SocClockIndexHigh               : 5
- 0x006d (0109) B       00 SocClockIndexLow                : 0
- 0x006e (0110) B       07 GfxClockIndexHigh               : 7
- 0x006f (0111) B       00 GfxClockIndexLow                : 0
- 0x0070 (0112) B       03 MemClockIndexHigh               : 3
- 0x0071 (0113) B       00 MemClockIndexLow                : 0
- 0x0072 (0114) H     0500 Classification                  : 5
- 0x0074 (0116) I 00000000 CapsAndSettings                 : 0
- 0x0078 (0120) H     0000 Classification2                 : 0
- 0x0032 (0050) H     4f02 FanTableOffset                  : 591
- 0x024f (0591) B       0b RevId                           : 11
- 0x0250 (0592) H     e412 FanOutputSensitivity            : 4836
- 0x0252 (0594) H     6009 FanAcousticLimitRpm             : 2400
- 0x0254 (0596) H     6009 ThrottlingRPM                   : 2400
- 0x0256 (0598) H     4b00 TargetTemperature               : 75
- 0x0258 (0600) H     0a00 MinimumPWMLimit                 : 10
- 0x025a (0602) H     5403 TargetGfxClk                    : 852
- 0x025c (0604) H     9001 FanGainEdge                     : 400
- 0x025e (0606) H     9001 FanGainHotspot                  : 400
- 0x0260 (0608) H     9001 FanGainLiquid                   : 400
- 0x0262 (0610) H     9001 FanGainVrVddc                   : 400
- 0x0264 (0612) H     9001 FanGainVrMvdd                   : 400
- 0x0266 (0614) H     9001 FanGainPlx                      : 400
- 0x0268 (0616) H     9001 FanGainHbm                      : 400
- 0x026a (0618) B       00 EnableZeroRPM                   : 0
- 0x026b (0619) H     0000 FanStopTemperature              : 0
- 0x026d (0621) H     0000 FanStartTemperature             : 0
- 0x026f (0623) B       02 FanParameters                   : 2
- 0x0270 (0624) B       04 FanMinRPM                       : 4
- 0x0271 (0625) B       31 FanMaxRPM                       : 49
- 0x0034 (0052) H     4602 ThermalControllerOffset         : 582
- 0x0246 (0582) B       01 RevId                           : 1
- 0x0247 (0583) B       18 Type                            : 24
- 0x0248 (0584) B       00 I2cLine                         : 0
- 0x0249 (0585) B       00 I2cAddress                      : 0
- 0x024a (0586) B       00 FanParameters                   : 0
- 0x024b (0587) B       00 FanMinRPM                       : 0
- 0x024c (0588) B       00 FanMaxRPM                       : 0
- 0x024d (0589) B       00 Flags                           : 0
- 0x0036 (0054) H     9400 SocclkDependencyTableOffset     : 148
- 0x0094 (0148) B       00 RevId                           : 0
- 0x0095 (0149) B       08 NumEntries                      : 8
- 0x0096 (0150) I 60ea0000 Clk                             : 60000
- 0x009a (0154) B       00 VddInd                          : 0
- 0x009b (0155) I 40190100 Clk                             : 72000
- 0x009f (0159) B       01 VddInd                          : 1
- 0x00a0 (0160) I 80380100 Clk                             : 80000
- 0x00a4 (0164) B       02 VddInd                          : 2
- 0x00a5 (0165) I dc4a0100 Clk                             : 84700
- 0x00a9 (0169) B       03 VddInd                          : 3
- 0x00aa (0170) I 905f0100 Clk                             : 90000
- 0x00ae (0174) B       04 VddInd                          : 4
- 0x00af (0175) I 00770100 Clk                             : 96000
- 0x00b3 (0179) B       05 VddInd                          : 5
- 0x00b4 (0180) I 90910100 Clk                             : 102800
- 0x00b8 (0184) B       06 VddInd                          : 6
- 0x00b9 (0185) I 6cb00100 Clk                             : 110700
- 0x00bd (0189) B       07 VddInd                          : 7
- 0x0038 (0056) H     9e01 MclkDependencyTableOffset       : 414
- 0x019e (0414) B       01 RevId                           : 1
- 0x019f (0415) B       04 NumEntries                      : 4
- 0x01a0 (0416) I 3c410000 MemClk                          : 16700
- 0x01a4 (0420) B       00 VddInd                          : 0
- 0x01a5 (0421) B       00 VddMemInd                       : 0
- 0x01a6 (0422) B       00 VddciInd                        : 0
- 0x01a7 (0423) I 50c30000 MemClk                          : 50000
- 0x01ab (0427) B       00 VddInd                          : 0
- 0x01ac (0428) B       00 VddMemInd                       : 0
- 0x01ad (0429) B       00 VddciInd                        : 0
- 0x01ae (0430) I 80380100 MemClk                          : 80000
- 0x01b2 (0434) B       02 VddInd                          : 2
- 0x01b3 (0435) B       00 VddMemInd                       : 0
- 0x01b4 (0436) B       00 VddciInd                        : 0
- 0x01b5 (0437) I 24710100 MemClk                          : 94500
- 0x01b9 (0441) B       04 VddInd                          : 4
- 0x01ba (0442) B       00 VddMemInd                       : 0
- 0x01bb (0443) B       00 VddciInd                        : 0
- 0x003a (0058) H     be00 GfxclkDependencyTableOffset     : 190
- 0x00be (0190) B       01 RevId                           : 1
- 0x00bf (0191) B       08 NumEntries                      : 8
- 0x00c0 (0192) I d04c0100 Clk                             : 85200
- 0x00c4 (0196) B       00 VddInd                          : 0
- 0x00c5 (0197) H     0080 CKSVOffsetandDisable            : 32768
- 0x00c7 (0199) H     0000 AVFSOffset                      : 0
- 0x00c9 (0201) B       00 ACGEnable                       : 0
- 0x00ca (0202) B       00 Reserved                        : 0
- 0x00cb (0203) B       00 Reserved                        : 0
- 0x00cc (0204) B       00 Reserved                        : 0
- 0x00cd (0205) I 1c830100 Clk                             : 99100
- 0x00d1 (0209) B       01 VddInd                          : 1
- 0x00d2 (0210) H     0000 CKSVOffsetandDisable            : 0
- 0x00d4 (0212) H     0000 AVFSOffset                      : 0
- 0x00d6 (0214) B       00 ACGEnable                       : 0
- 0x00d7 (0215) B       00 Reserved                        : 0
- 0x00d8 (0216) B       00 Reserved                        : 0
- 0x00d9 (0217) B       00 Reserved                        : 0
- 0x00da (0218) I 70a70100 Clk                             : 108400
- 0x00de (0222) B       02 VddInd                          : 2
- 0x00df (0223) H     0000 CKSVOffsetandDisable            : 0
- 0x00e1 (0225) H     0000 AVFSOffset                      : 0
- 0x00e3 (0227) B       00 ACGEnable                       : 0
- 0x00e4 (0228) B       00 Reserved                        : 0
- 0x00e5 (0229) B       00 Reserved                        : 0
- 0x00e6 (0230) B       00 Reserved                        : 0
- 0x00e7 (0231) I 88bc0100 Clk                             : 113800
- 0x00eb (0235) B       03 VddInd                          : 3
- 0x00ec (0236) H     0000 CKSVOffsetandDisable            : 0
- 0x00ee (0238) H     0000 AVFSOffset                      : 0
- 0x00f0 (0240) B       00 ACGEnable                       : 0
- 0x00f1 (0241) B       00 Reserved                        : 0
- 0x00f2 (0242) B       00 Reserved                        : 0
- 0x00f3 (0243) B       00 Reserved                        : 0
- 0x00f4 (0244) I c0d40100 Clk                             : 120000
- 0x00f8 (0248) B       04 VddInd                          : 4
- 0x00f9 (0249) H     0000 CKSVOffsetandDisable            : 0
- 0x00fb (0251) H     0000 AVFSOffset                      : 0
- 0x00fd (0253) B       00 ACGEnable                       : 0
- 0x00fe (0254) B       00 Reserved                        : 0
- 0x00ff (0255) B       00 Reserved                        : 0
- 0x0100 (0256) B       00 Reserved                        : 0
- 0x0101 (0257) I 44230200 Clk                             : 140100
- 0x0105 (0261) B       05 VddInd                          : 5
- 0x0106 (0262) H     0000 CKSVOffsetandDisable            : 0
- 0x0108 (0264) H     0000 AVFSOffset                      : 0
- 0x010a (0266) B       01 ACGEnable                       : 1
- 0x010b (0267) B       00 Reserved                        : 0
- 0x010c (0268) B       00 Reserved                        : 0
- 0x010d (0269) B       00 Reserved                        : 0
- 0x010e (0270) I 00580200 Clk                             : 153600
- 0x0112 (0274) B       06 VddInd                          : 6
- 0x0113 (0275) H     0000 CKSVOffsetandDisable            : 0
- 0x0115 (0277) H     0000 AVFSOffset                      : 0
- 0x0117 (0279) B       01 ACGEnable                       : 1
- 0x0118 (0280) B       00 Reserved                        : 0
- 0x0119 (0281) B       00 Reserved                        : 0
- 0x011a (0282) B       00 Reserved                        : 0
- 0x011b (0283) I b87c0200 Clk                             : 163000
- 0x011f (0287) B       07 VddInd                          : 7
- 0x0120 (0288) H     0000 CKSVOffsetandDisable            : 0
- 0x0122 (0290) H     0000 AVFSOffset                      : 0
- 0x0124 (0292) B       01 ACGEnable                       : 1
- 0x0125 (0293) B       00 Reserved                        : 0
- 0x0126 (0294) B       00 Reserved                        : 0
- 0x0127 (0295) B       00 Reserved                        : 0
- 0x003c (0060) H     2801 DcefclkDependencyTableOffset    : 296
- 0x0128 (0296) B       00 RevId                           : 0
- 0x0129 (0297) B       05 NumEntries                      : 5
- 0x012a (0298) I 60ea0000 Clk                             : 60000
- 0x012e (0302) B       00 VddInd                          : 0
- 0x012f (0303) I 40190100 Clk                             : 72000
- 0x0133 (0307) B       00 VddInd                          : 0
- 0x0134 (0308) I 80380100 Clk                             : 80000
- 0x0138 (0312) B       00 VddInd                          : 0
- 0x0139 (0313) I dc4a0100 Clk                             : 84700
- 0x013d (0317) B       00 VddInd                          : 0
- 0x013e (0318) I 905f0100 Clk                             : 90000
- 0x0142 (0322) B       00 VddInd                          : 0
- 0x003e (0062) H     7a00 VddcLookupTableOffset           : 122
- 0x007a (0122) B       01 RevId                           : 1
- 0x007b (0123) B       08 NumEntries                      : 8
- 0x007c (0124) H     2003 Vdd                             : 800
- 0x007e (0126) H     8403 Vdd                             : 900
- 0x0080 (0128) H     b603 Vdd                             : 950
- 0x0082 (0130) H     e803 Vdd                             : 1000
- 0x0084 (0132) H     1a04 Vdd                             : 1050
- 0x0086 (0134) H     4c04 Vdd                             : 1100
- 0x0088 (0136) H     7e04 Vdd                             : 1150
- 0x008a (0138) H     b004 Vdd                             : 1200
- 0x0040 (0064) H     8c00 VddmemLookupTableOffset         : 140
- 0x008c (0140) B       01 RevId                           : 1
- 0x008d (0141) B       01 NumEntries                      : 1
- 0x008e (0142) H     4605 Vdd                             : 1350
- 0x0042 (0066) H     bc01 MMDependencyTableOffset         : 444
- 0x01bc (0444) B       01 RevId                           : 1
- 0x01bd (0445) B       08 NumEntries                      : 8
- 0x01be (0446) B       00 VddcInd                         : 0
- 0x01bf (0447) I 98850000 DClk                            : 34200
- 0x01c3 (0451) I 40b50000 VClk                            : 46400
- 0x01c7 (0455) I 60ea0000 EClk                            : 60000
- 0x01cb (0459) I 50c30000 PSPClk                          : 50000
- 0x01cf (0463) B       01 VddcInd                         : 1
- 0x01d0 (0464) I 80bb0000 DClk                            : 48000
- 0x01d4 (0468) I 60ea0000 VClk                            : 60000
- 0x01d8 (0472) I 940b0100 EClk                            : 68500
- 0x01dc (0476) I 50c30000 PSPClk                          : 50000
- 0x01e0 (0480) B       02 VddcInd                         : 2
- 0x01e1 (0481) I 00e10000 DClk                            : 57600
- 0x01e5 (0485) I 940b0100 VClk                            : 68500
- 0x01e9 (0489) I 40190100 EClk                            : 72000
- 0x01ed (0493) I 50c30000 PSPClk                          : 50000
- 0x01f1 (0497) B       03 VddcInd                         : 3
- 0x01f2 (0498) I 78ff0000 DClk                            : 65400
- 0x01f6 (0502) I 40190100 VClk                            : 72000
- 0x01fa (0506) I 88260100 EClk                            : 75400
- 0x01fe (0510) I 50c30000 PSPClk                          : 50000
- 0x0202 (0514) B       04 VddcInd                         : 4
- 0x0203 (0515) I 40190100 DClk                            : 72000
- 0x0207 (0519) I 80380100 VClk                            : 80000
- 0x020b (0523) I 80380100 EClk                            : 80000
- 0x020f (0527) I 50c30000 PSPClk                          : 50000
- 0x0213 (0531) B       05 VddcInd                         : 5
- 0x0214 (0532) I 80380100 DClk                            : 80000
- 0x0218 (0536) I dc4a0100 VClk                            : 84700
- 0x021c (0540) I dc4a0100 EClk                            : 84700
- 0x0220 (0544) I 50c30000 PSPClk                          : 50000
- 0x0224 (0548) B       06 VddcInd                         : 6
- 0x0225 (0549) I 00770100 DClk                            : 96000
- 0x0229 (0553) I 00770100 VClk                            : 96000
- 0x022d (0557) I 905f0100 EClk                            : 90000
- 0x0231 (0561) I 50c30000 PSPClk                          : 50000
- 0x0235 (0565) B       07 VddcInd                         : 7
- 0x0236 (0566) I 90910100 DClk                            : 102800
- 0x023a (0570) I 90910100 VClk                            : 102800
- 0x023e (0574) I 00770100 EClk                            : 96000
- 0x0242 (0578) I 50c30000 PSPClk                          : 50000
- 0x0044 (0068) H     0000 VCEStateTableOffset             : 0
- 0x0046 (0070) H     0000 Reserve                         : 0
- 0x0048 (0072) H     7202 PowerTuneTableOffset            : 626
- 0x0272 (0626) B       07 RevId                           : 7
- 0x0273 (0627) H     dc00 SocketPowerLimit                : 220
- 0x0275 (0629) H     dc00 BatteryPowerLimit               : 220
- 0x0277 (0631) H     dc00 SmallPowerLimit                 : 220
- 0x0279 (0633) H     2c01 TdcLimit                        : 300
- 0x027b (0635) H     0000 EdcLimit                        : 0
- 0x027d (0637) H     5900 SoftwareShutdownTemp            : 89
- 0x027f (0639) H     6900 TemperatureLimitHotSpot         : 105
- 0x0281 (0641) H     4a00 TemperatureLimitLiquid1         : 74
- 0x0283 (0643) H     4a00 TemperatureLimitLiquid2         : 74
- 0x0285 (0645) H     5f00 TemperatureLimitHBM             : 95
- 0x0287 (0647) H     7300 TemperatureLimitVrSoc           : 115
- 0x0289 (0649) H     7300 TemperatureLimitVrMem           : 115
- 0x028b (0651) H     6400 TemperatureLimitPlx             : 100
- 0x028d (0653) H     4000 LoadLineResistance              : 64
- 0x028f (0655) B       90 Liquid1_I2C_address             : 144
- 0x0290 (0656) B       92 Liquid2_I2C_address             : 146
- 0x0291 (0657) B       97 Liquid_I2C_Line                 : 151
- 0x0292 (0658) B       60 Vr_I2C_address                  : 96
- 0x0293 (0659) B       96 Vr_I2C_Line                     : 150
- 0x0294 (0660) B       00 Plx_I2C_address                 : 0
- 0x0295 (0661) B       90 Plx_I2C_Line                    : 144
- 0x0296 (0662) H     5500 TemperatureLimitTedge           : 85
- 0x0298 (0664) H     0000 BoostStartTemperature           : 0
- 0x029a (0666) H     0000 BoostStopTemperature            : 0
- 0x029c (0668) I 00000000 BoostClock                      : 0
- 0x02a0 (0672) I 00000000 Reserved                        : 0
- 0x02a4 (0676) I 00000000 Reserved                        : 0
- 0x004a (0074) H     0000 HardLimitTableOffset            : 0
- 0x004c (0076) H     9000 VddciLookupTableOffset          : 144
- 0x0090 (0144) B       01 RevId                           : 1
- 0x0091 (0145) B       01 NumEntries                      : 1
- 0x0092 (0146) H     8403 Vdd                             : 900
- 0x004e (0078) H     a802 PCIETableOffset                 : 680
- 0x02a8 (0680) B       02 RevId                           : 2
- 0x02a9 (0681) B       02 NumEntries                      : 2
- 0x02aa (0682) I d4300000 LCLK                            : 12500
- 0x02ae (0686) B       02 PCIEGenSpeed                    : 2
- 0x02af (0687) B       10 PCIELaneWidth                   : 16
- 0x02b0 (0688) I 60ea0000 LCLK                            : 60000
- 0x02b4 (0692) B       02 PCIEGenSpeed                    : 2
- 0x02b5 (0693) B       10 PCIELaneWidth                   : 16
- 0x0050 (0080) H     6d01 PixclkDependencyTableOffset     : 365
- 0x016d (0365) B       00 RevId                           : 0
- 0x016e (0366) B       08 NumEntries                      : 8
- 0x016f (0367) I 6c390000 Clk                             : 14700
- 0x0173 (0371) B       00 VddInd                          : 0
- 0x0174 (0372) I 245e0000 Clk                             : 24100
- 0x0178 (0376) B       01 VddInd                          : 1
- 0x0179 (0377) I fc850000 Clk                             : 34300
- 0x017d (0381) B       02 VddInd                          : 2
- 0x017e (0382) I acbc0000 Clk                             : 48300
- 0x0182 (0386) B       03 VddInd                          : 3
- 0x0183 (0387) I 34d00000 Clk                             : 53300
- 0x0187 (0391) B       04 VddInd                          : 4
- 0x0188 (0392) I 686e0100 Clk                             : 93800
- 0x018c (0396) B       05 VddInd                          : 5
- 0x018d (0397) I 08970100 Clk                             : 104200
- 0x0191 (0401) B       06 VddInd                          : 6
- 0x0192 (0402) I eca30100 Clk                             : 107500
- 0x0196 (0406) B       07 VddInd                          : 7
- 0x0052 (0082) H     4301 DispClkDependencyTableOffset    : 323
- 0x0143 (0323) B       00 RevId                           : 0
- 0x0144 (0324) B       08 NumEntries                      : 8
- 0x0145 (0325) I 286e0000 Clk                             : 28200
- 0x0149 (0329) B       00 VddInd                          : 0
- 0x014a (0330) I 2cc90000 Clk                             : 51500
- 0x014e (0334) B       01 VddInd                          : 1
- 0x014f (0335) I f80b0100 Clk                             : 68600
- 0x0153 (0339) B       02 VddInd                          : 2
- 0x0154 (0340) I 80380100 Clk                             : 80000
- 0x0158 (0344) B       03 VddInd                          : 3
- 0x0159 (0345) I 905f0100 Clk                             : 90000
- 0x015d (0349) B       04 VddInd                          : 4
- 0x015e (0350) I f4910100 Clk                             : 102900
- 0x0162 (0354) B       05 VddInd                          : 5
- 0x0163 (0355) I d0b00100 Clk                             : 110800
- 0x0167 (0359) B       06 VddInd                          : 6
- 0x0168 (0360) I c0d40100 Clk                             : 120000
- 0x016c (0364) B       07 VddInd                          : 7
- 0x0054 (0084) H     9701 PhyClkDependencyTableOffset     : 407
- 0x0197 (0407) B       00 RevId                           : 0
- 0x0198 (0408) B       01 NumEntries                      : 1
- 0x0199 (0409) I 683c0100 Clk                             : 81000
- 0x019d (0413) B       00 VddInd                          : 0
+ Offset (dec.) t Raw val. Variable name                         Decoded value
+------------------------------------------------------------------------------
+ 0x0000 (0000) H     b602 structuresize                             : 694
+ 0x0002 (0002) B       08 format_revision                           : 8
+ 0x0003 (0003) B       01 content_revision                          : 1
+ 0x0004 (0004) B       00 TableRevision                             : 0
+ 0x0005 (0005) H     5c00 TableSize                                 : 92
+ 0x0007 (0007) I e1060000 GoldenPPID                                : 1761
+ 0x000b (0011) I ee2b0000 GoldenRevision                            : 11246
+ 0x000f (0015) H     1b00 FormatID                                  : 27
+ 0x0011 (0017) I 48000000 PlatformCaps                              : 72
+ 0x0015 (0021) I 80a90300 MaxODEngineClock                          : 240000
+ 0x0019 (0025) I f0490200 MaxODMemoryClock                          : 150000
+ 0x001d (0029) H     3200 PowerControlLimit                         : 50
+ 0x001f (0031) H     0800 UlvVoltageOffset                          : 8
+ 0x0021 (0033) H     0000 UlvSmnclkDid                              : 0
+ 0x0023 (0035) H     0000 UlvMp1clkDid                              : 0
+ 0x0025 (0037) H     0000 UlvGfxclkBypass                           : 0
+ 0x0027 (0039) H     0000 GfxclkSlewRate                            : 0
+ 0x0029 (0041) B       00 GfxVoltageMode                            : 0
+ 0x002a (0042) B       00 SocVoltageMode                            : 0
+ 0x002b (0043) B       00 UclkVoltageMode                           : 0
+ 0x002c (0044) B       00 UvdVoltageMode                            : 0
+ 0x002d (0045) B       00 VceVoltageMode                            : 0
+ 0x002e (0046) B       02 Mp0VoltageMode                            : 2
+ 0x002f (0047) B       01 DcefVoltageMode                           : 1
+ 0x0030 (0048) H     5c00 StateArrayOffset                          : 92
+ 0x005c (0092) B       02 RevId                                     : 2
+ 0x005d (0093) B       02 NumEntries                                : 2
+ 0x005e (0094) B       00 SocClockIndexHigh                         : 0
+ 0x005f (0095) B       00 SocClockIndexLow                          : 0
+ 0x0060 (0096) B       00 GfxClockIndexHigh                         : 0
+ 0x0061 (0097) B       00 GfxClockIndexLow                          : 0
+ 0x0062 (0098) B       00 MemClockIndexHigh                         : 0
+ 0x0063 (0099) B       00 MemClockIndexLow                          : 0
+ 0x0064 (0100) H     0800 Classification                            : 8
+ 0x0066 (0102) I 00000000 CapsAndSettings                           : 0
+ 0x006a (0106) H     0000 Classification2                           : 0
+ 0x006c (0108) B       05 SocClockIndexHigh                         : 5
+ 0x006d (0109) B       00 SocClockIndexLow                          : 0
+ 0x006e (0110) B       07 GfxClockIndexHigh                         : 7
+ 0x006f (0111) B       00 GfxClockIndexLow                          : 0
+ 0x0070 (0112) B       03 MemClockIndexHigh                         : 3
+ 0x0071 (0113) B       00 MemClockIndexLow                          : 0
+ 0x0072 (0114) H     0500 Classification                            : 5
+ 0x0074 (0116) I 00000000 CapsAndSettings                           : 0
+ 0x0078 (0120) H     0000 Classification2                           : 0
+ 0x0032 (0050) H     4f02 FanTableOffset                            : 591
+ 0x024f (0591) B       0b RevId                                     : 11
+ 0x0250 (0592) H     e412 FanOutputSensitivity                      : 4836
+ 0x0252 (0594) H     6009 FanAcousticLimitRpm                       : 2400
+ 0x0254 (0596) H     6009 ThrottlingRPM                             : 2400
+ 0x0256 (0598) H     4b00 TargetTemperature                         : 75
+ 0x0258 (0600) H     0a00 MinimumPWMLimit                           : 10
+ 0x025a (0602) H     5403 TargetGfxClk                              : 852
+ 0x025c (0604) H     9001 FanGainEdge                               : 400
+ 0x025e (0606) H     9001 FanGainHotspot                            : 400
+ 0x0260 (0608) H     9001 FanGainLiquid                             : 400
+ 0x0262 (0610) H     9001 FanGainVrVddc                             : 400
+ 0x0264 (0612) H     9001 FanGainVrMvdd                             : 400
+ 0x0266 (0614) H     9001 FanGainPlx                                : 400
+ 0x0268 (0616) H     9001 FanGainHbm                                : 400
+ 0x026a (0618) B       00 EnableZeroRPM                             : 0
+ 0x026b (0619) H     0000 FanStopTemperature                        : 0
+ 0x026d (0621) H     0000 FanStartTemperature                       : 0
+ 0x026f (0623) B       02 FanParameters                             : 2
+ 0x0270 (0624) B       04 FanMinRPM                                 : 4
+ 0x0271 (0625) B       31 FanMaxRPM                                 : 49
+ 0x0034 (0052) H     4602 ThermalControllerOffset                   : 582
+ 0x0246 (0582) B       01 RevId                                     : 1
+ 0x0247 (0583) B       18 Type                                      : 24
+ 0x0248 (0584) B       00 I2cLine                                   : 0
+ 0x0249 (0585) B       00 I2cAddress                                : 0
+ 0x024a (0586) B       00 FanParameters                             : 0
+ 0x024b (0587) B       00 FanMinRPM                                 : 0
+ 0x024c (0588) B       00 FanMaxRPM                                 : 0
+ 0x024d (0589) B       00 Flags                                     : 0
+ 0x0036 (0054) H     9400 SocclkDependencyTableOffset               : 148
+ 0x0094 (0148) B       00 RevId                                     : 0
+ 0x0095 (0149) B       08 NumEntries                                : 8
+ 0x0096 (0150) I 60ea0000 Clk                                       : 60000
+ 0x009a (0154) B       00 VddInd                                    : 0
+ 0x009b (0155) I 40190100 Clk                                       : 72000
+ 0x009f (0159) B       01 VddInd                                    : 1
+ 0x00a0 (0160) I 80380100 Clk                                       : 80000
+ 0x00a4 (0164) B       02 VddInd                                    : 2
+ 0x00a5 (0165) I dc4a0100 Clk                                       : 84700
+ 0x00a9 (0169) B       03 VddInd                                    : 3
+ 0x00aa (0170) I 905f0100 Clk                                       : 90000
+ 0x00ae (0174) B       04 VddInd                                    : 4
+ 0x00af (0175) I 00770100 Clk                                       : 96000
+ 0x00b3 (0179) B       05 VddInd                                    : 5
+ 0x00b4 (0180) I 90910100 Clk                                       : 102800
+ 0x00b8 (0184) B       06 VddInd                                    : 6
+ 0x00b9 (0185) I 6cb00100 Clk                                       : 110700
+ 0x00bd (0189) B       07 VddInd                                    : 7
+ 0x0038 (0056) H     9e01 MclkDependencyTableOffset                 : 414
+ 0x019e (0414) B       01 RevId                                     : 1
+ 0x019f (0415) B       04 NumEntries                                : 4
+ 0x01a0 (0416) I 3c410000 MemClk                                    : 16700
+ 0x01a4 (0420) B       00 VddInd                                    : 0
+ 0x01a5 (0421) B       00 VddMemInd                                 : 0
+ 0x01a6 (0422) B       00 VddciInd                                  : 0
+ 0x01a7 (0423) I 50c30000 MemClk                                    : 50000
+ 0x01ab (0427) B       00 VddInd                                    : 0
+ 0x01ac (0428) B       00 VddMemInd                                 : 0
+ 0x01ad (0429) B       00 VddciInd                                  : 0
+ 0x01ae (0430) I 80380100 MemClk                                    : 80000
+ 0x01b2 (0434) B       02 VddInd                                    : 2
+ 0x01b3 (0435) B       00 VddMemInd                                 : 0
+ 0x01b4 (0436) B       00 VddciInd                                  : 0
+ 0x01b5 (0437) I 24710100 MemClk                                    : 94500
+ 0x01b9 (0441) B       04 VddInd                                    : 4
+ 0x01ba (0442) B       00 VddMemInd                                 : 0
+ 0x01bb (0443) B       00 VddciInd                                  : 0
+ 0x003a (0058) H     be00 GfxclkDependencyTableOffset               : 190
+ 0x00be (0190) B       01 RevId                                     : 1
+ 0x00bf (0191) B       08 NumEntries                                : 8
+ 0x00c0 (0192) I d04c0100 Clk                                       : 85200
+ 0x00c4 (0196) B       00 VddInd                                    : 0
+ 0x00c5 (0197) H     0080 CKSVOffsetandDisable                      : 32768
+ 0x00c7 (0199) H     0000 AVFSOffset                                : 0
+ 0x00c9 (0201) B       00 ACGEnable                                 : 0
+ 0x00ca (0202) B       00 Reserved                                  : 0
+ 0x00cb (0203) B       00 Reserved                                  : 0
+ 0x00cc (0204) B       00 Reserved                                  : 0
+ 0x00cd (0205) I 1c830100 Clk                                       : 99100
+ 0x00d1 (0209) B       01 VddInd                                    : 1
+ 0x00d2 (0210) H     0000 CKSVOffsetandDisable                      : 0
+ 0x00d4 (0212) H     0000 AVFSOffset                                : 0
+ 0x00d6 (0214) B       00 ACGEnable                                 : 0
+ 0x00d7 (0215) B       00 Reserved                                  : 0
+ 0x00d8 (0216) B       00 Reserved                                  : 0
+ 0x00d9 (0217) B       00 Reserved                                  : 0
+ 0x00da (0218) I 70a70100 Clk                                       : 108400
+ 0x00de (0222) B       02 VddInd                                    : 2
+ 0x00df (0223) H     0000 CKSVOffsetandDisable                      : 0
+ 0x00e1 (0225) H     0000 AVFSOffset                                : 0
+ 0x00e3 (0227) B       00 ACGEnable                                 : 0
+ 0x00e4 (0228) B       00 Reserved                                  : 0
+ 0x00e5 (0229) B       00 Reserved                                  : 0
+ 0x00e6 (0230) B       00 Reserved                                  : 0
+ 0x00e7 (0231) I 88bc0100 Clk                                       : 113800
+ 0x00eb (0235) B       03 VddInd                                    : 3
+ 0x00ec (0236) H     0000 CKSVOffsetandDisable                      : 0
+ 0x00ee (0238) H     0000 AVFSOffset                                : 0
+ 0x00f0 (0240) B       00 ACGEnable                                 : 0
+ 0x00f1 (0241) B       00 Reserved                                  : 0
+ 0x00f2 (0242) B       00 Reserved                                  : 0
+ 0x00f3 (0243) B       00 Reserved                                  : 0
+ 0x00f4 (0244) I c0d40100 Clk                                       : 120000
+ 0x00f8 (0248) B       04 VddInd                                    : 4
+ 0x00f9 (0249) H     0000 CKSVOffsetandDisable                      : 0
+ 0x00fb (0251) H     0000 AVFSOffset                                : 0
+ 0x00fd (0253) B       00 ACGEnable                                 : 0
+ 0x00fe (0254) B       00 Reserved                                  : 0
+ 0x00ff (0255) B       00 Reserved                                  : 0
+ 0x0100 (0256) B       00 Reserved                                  : 0
+ 0x0101 (0257) I 44230200 Clk                                       : 140100
+ 0x0105 (0261) B       05 VddInd                                    : 5
+ 0x0106 (0262) H     0000 CKSVOffsetandDisable                      : 0
+ 0x0108 (0264) H     0000 AVFSOffset                                : 0
+ 0x010a (0266) B       01 ACGEnable                                 : 1
+ 0x010b (0267) B       00 Reserved                                  : 0
+ 0x010c (0268) B       00 Reserved                                  : 0
+ 0x010d (0269) B       00 Reserved                                  : 0
+ 0x010e (0270) I 00580200 Clk                                       : 153600
+ 0x0112 (0274) B       06 VddInd                                    : 6
+ 0x0113 (0275) H     0000 CKSVOffsetandDisable                      : 0
+ 0x0115 (0277) H     0000 AVFSOffset                                : 0
+ 0x0117 (0279) B       01 ACGEnable                                 : 1
+ 0x0118 (0280) B       00 Reserved                                  : 0
+ 0x0119 (0281) B       00 Reserved                                  : 0
+ 0x011a (0282) B       00 Reserved                                  : 0
+ 0x011b (0283) I b87c0200 Clk                                       : 163000
+ 0x011f (0287) B       07 VddInd                                    : 7
+ 0x0120 (0288) H     0000 CKSVOffsetandDisable                      : 0
+ 0x0122 (0290) H     0000 AVFSOffset                                : 0
+ 0x0124 (0292) B       01 ACGEnable                                 : 1
+ 0x0125 (0293) B       00 Reserved                                  : 0
+ 0x0126 (0294) B       00 Reserved                                  : 0
+ 0x0127 (0295) B       00 Reserved                                  : 0
+ 0x003c (0060) H     2801 DcefclkDependencyTableOffset              : 296
+ 0x0128 (0296) B       00 RevId                                     : 0
+ 0x0129 (0297) B       05 NumEntries                                : 5
+ 0x012a (0298) I 60ea0000 Clk                                       : 60000
+ 0x012e (0302) B       00 VddInd                                    : 0
+ 0x012f (0303) I 40190100 Clk                                       : 72000
+ 0x0133 (0307) B       00 VddInd                                    : 0
+ 0x0134 (0308) I 80380100 Clk                                       : 80000
+ 0x0138 (0312) B       00 VddInd                                    : 0
+ 0x0139 (0313) I dc4a0100 Clk                                       : 84700
+ 0x013d (0317) B       00 VddInd                                    : 0
+ 0x013e (0318) I 905f0100 Clk                                       : 90000
+ 0x0142 (0322) B       00 VddInd                                    : 0
+ 0x003e (0062) H     7a00 VddcLookupTableOffset                     : 122
+ 0x007a (0122) B       01 RevId                                     : 1
+ 0x007b (0123) B       08 NumEntries                                : 8
+ 0x007c (0124) H     2003 Vdd                                       : 800
+ 0x007e (0126) H     8403 Vdd                                       : 900
+ 0x0080 (0128) H     b603 Vdd                                       : 950
+ 0x0082 (0130) H     e803 Vdd                                       : 1000
+ 0x0084 (0132) H     1a04 Vdd                                       : 1050
+ 0x0086 (0134) H     4c04 Vdd                                       : 1100
+ 0x0088 (0136) H     7e04 Vdd                                       : 1150
+ 0x008a (0138) H     b004 Vdd                                       : 1200
+ 0x0040 (0064) H     8c00 VddmemLookupTableOffset                   : 140
+ 0x008c (0140) B       01 RevId                                     : 1
+ 0x008d (0141) B       01 NumEntries                                : 1
+ 0x008e (0142) H     4605 Vdd                                       : 1350
+ 0x0042 (0066) H     bc01 MMDependencyTableOffset                   : 444
+ 0x01bc (0444) B       01 RevId                                     : 1
+ 0x01bd (0445) B       08 NumEntries                                : 8
+ 0x01be (0446) B       00 VddcInd                                   : 0
+ 0x01bf (0447) I 98850000 DClk                                      : 34200
+ 0x01c3 (0451) I 40b50000 VClk                                      : 46400
+ 0x01c7 (0455) I 60ea0000 EClk                                      : 60000
+ 0x01cb (0459) I 50c30000 PSPClk                                    : 50000
+ 0x01cf (0463) B       01 VddcInd                                   : 1
+ 0x01d0 (0464) I 80bb0000 DClk                                      : 48000
+ 0x01d4 (0468) I 60ea0000 VClk                                      : 60000
+ 0x01d8 (0472) I 940b0100 EClk                                      : 68500
+ 0x01dc (0476) I 50c30000 PSPClk                                    : 50000
+ 0x01e0 (0480) B       02 VddcInd                                   : 2
+ 0x01e1 (0481) I 00e10000 DClk                                      : 57600
+ 0x01e5 (0485) I 940b0100 VClk                                      : 68500
+ 0x01e9 (0489) I 40190100 EClk                                      : 72000
+ 0x01ed (0493) I 50c30000 PSPClk                                    : 50000
+ 0x01f1 (0497) B       03 VddcInd                                   : 3
+ 0x01f2 (0498) I 78ff0000 DClk                                      : 65400
+ 0x01f6 (0502) I 40190100 VClk                                      : 72000
+ 0x01fa (0506) I 88260100 EClk                                      : 75400
+ 0x01fe (0510) I 50c30000 PSPClk                                    : 50000
+ 0x0202 (0514) B       04 VddcInd                                   : 4
+ 0x0203 (0515) I 40190100 DClk                                      : 72000
+ 0x0207 (0519) I 80380100 VClk                                      : 80000
+ 0x020b (0523) I 80380100 EClk                                      : 80000
+ 0x020f (0527) I 50c30000 PSPClk                                    : 50000
+ 0x0213 (0531) B       05 VddcInd                                   : 5
+ 0x0214 (0532) I 80380100 DClk                                      : 80000
+ 0x0218 (0536) I dc4a0100 VClk                                      : 84700
+ 0x021c (0540) I dc4a0100 EClk                                      : 84700
+ 0x0220 (0544) I 50c30000 PSPClk                                    : 50000
+ 0x0224 (0548) B       06 VddcInd                                   : 6
+ 0x0225 (0549) I 00770100 DClk                                      : 96000
+ 0x0229 (0553) I 00770100 VClk                                      : 96000
+ 0x022d (0557) I 905f0100 EClk                                      : 90000
+ 0x0231 (0561) I 50c30000 PSPClk                                    : 50000
+ 0x0235 (0565) B       07 VddcInd                                   : 7
+ 0x0236 (0566) I 90910100 DClk                                      : 102800
+ 0x023a (0570) I 90910100 VClk                                      : 102800
+ 0x023e (0574) I 00770100 EClk                                      : 96000
+ 0x0242 (0578) I 50c30000 PSPClk                                    : 50000
+ 0x0044 (0068) H     0000 VCEStateTableOffset                       : 0
+ 0x0046 (0070) H     0000 Reserve                                   : 0
+ 0x0048 (0072) H     7202 PowerTuneTableOffset                      : 626
+ 0x0272 (0626) B       07 RevId                                     : 7
+ 0x0273 (0627) H     dc00 SocketPowerLimit                          : 220
+ 0x0275 (0629) H     dc00 BatteryPowerLimit                         : 220
+ 0x0277 (0631) H     dc00 SmallPowerLimit                           : 220
+ 0x0279 (0633) H     2c01 TdcLimit                                  : 300
+ 0x027b (0635) H     0000 EdcLimit                                  : 0
+ 0x027d (0637) H     5900 SoftwareShutdownTemp                      : 89
+ 0x027f (0639) H     6900 TemperatureLimitHotSpot                   : 105
+ 0x0281 (0641) H     4a00 TemperatureLimitLiquid1                   : 74
+ 0x0283 (0643) H     4a00 TemperatureLimitLiquid2                   : 74
+ 0x0285 (0645) H     5f00 TemperatureLimitHBM                       : 95
+ 0x0287 (0647) H     7300 TemperatureLimitVrSoc                     : 115
+ 0x0289 (0649) H     7300 TemperatureLimitVrMem                     : 115
+ 0x028b (0651) H     6400 TemperatureLimitPlx                       : 100
+ 0x028d (0653) H     4000 LoadLineResistance                        : 64
+ 0x028f (0655) B       90 Liquid1_I2C_address                       : 144
+ 0x0290 (0656) B       92 Liquid2_I2C_address                       : 146
+ 0x0291 (0657) B       97 Liquid_I2C_Line                           : 151
+ 0x0292 (0658) B       60 Vr_I2C_address                            : 96
+ 0x0293 (0659) B       96 Vr_I2C_Line                               : 150
+ 0x0294 (0660) B       00 Plx_I2C_address                           : 0
+ 0x0295 (0661) B       90 Plx_I2C_Line                              : 144
+ 0x0296 (0662) H     5500 TemperatureLimitTedge                     : 85
+ 0x0298 (0664) H     0000 BoostStartTemperature                     : 0
+ 0x029a (0666) H     0000 BoostStopTemperature                      : 0
+ 0x029c (0668) I 00000000 BoostClock                                : 0
+ 0x02a0 (0672) I 00000000 Reserved                                  : 0
+ 0x02a4 (0676) I 00000000 Reserved                                  : 0
+ 0x004a (0074) H     0000 HardLimitTableOffset                      : 0
+ 0x004c (0076) H     9000 VddciLookupTableOffset                    : 144
+ 0x0090 (0144) B       01 RevId                                     : 1
+ 0x0091 (0145) B       01 NumEntries                                : 1
+ 0x0092 (0146) H     8403 Vdd                                       : 900
+ 0x004e (0078) H     a802 PCIETableOffset                           : 680
+ 0x02a8 (0680) B       02 RevId                                     : 2
+ 0x02a9 (0681) B       02 NumEntries                                : 2
+ 0x02aa (0682) I d4300000 LCLK                                      : 12500
+ 0x02ae (0686) B       02 PCIEGenSpeed                              : 2
+ 0x02af (0687) B       10 PCIELaneWidth                             : 16
+ 0x02b0 (0688) I 60ea0000 LCLK                                      : 60000
+ 0x02b4 (0692) B       02 PCIEGenSpeed                              : 2
+ 0x02b5 (0693) B       10 PCIELaneWidth                             : 16
+ 0x0050 (0080) H     6d01 PixclkDependencyTableOffset               : 365
+ 0x016d (0365) B       00 RevId                                     : 0
+ 0x016e (0366) B       08 NumEntries                                : 8
+ 0x016f (0367) I 6c390000 Clk                                       : 14700
+ 0x0173 (0371) B       00 VddInd                                    : 0
+ 0x0174 (0372) I 245e0000 Clk                                       : 24100
+ 0x0178 (0376) B       01 VddInd                                    : 1
+ 0x0179 (0377) I fc850000 Clk                                       : 34300
+ 0x017d (0381) B       02 VddInd                                    : 2
+ 0x017e (0382) I acbc0000 Clk                                       : 48300
+ 0x0182 (0386) B       03 VddInd                                    : 3
+ 0x0183 (0387) I 34d00000 Clk                                       : 53300
+ 0x0187 (0391) B       04 VddInd                                    : 4
+ 0x0188 (0392) I 686e0100 Clk                                       : 93800
+ 0x018c (0396) B       05 VddInd                                    : 5
+ 0x018d (0397) I 08970100 Clk                                       : 104200
+ 0x0191 (0401) B       06 VddInd                                    : 6
+ 0x0192 (0402) I eca30100 Clk                                       : 107500
+ 0x0196 (0406) B       07 VddInd                                    : 7
+ 0x0052 (0082) H     4301 DispClkDependencyTableOffset              : 323
+ 0x0143 (0323) B       00 RevId                                     : 0
+ 0x0144 (0324) B       08 NumEntries                                : 8
+ 0x0145 (0325) I 286e0000 Clk                                       : 28200
+ 0x0149 (0329) B       00 VddInd                                    : 0
+ 0x014a (0330) I 2cc90000 Clk                                       : 51500
+ 0x014e (0334) B       01 VddInd                                    : 1
+ 0x014f (0335) I f80b0100 Clk                                       : 68600
+ 0x0153 (0339) B       02 VddInd                                    : 2
+ 0x0154 (0340) I 80380100 Clk                                       : 80000
+ 0x0158 (0344) B       03 VddInd                                    : 3
+ 0x0159 (0345) I 905f0100 Clk                                       : 90000
+ 0x015d (0349) B       04 VddInd                                    : 4
+ 0x015e (0350) I f4910100 Clk                                       : 102900
+ 0x0162 (0354) B       05 VddInd                                    : 5
+ 0x0163 (0355) I d0b00100 Clk                                       : 110800
+ 0x0167 (0359) B       06 VddInd                                    : 6
+ 0x0168 (0360) I c0d40100 Clk                                       : 120000
+ 0x016c (0364) B       07 VddInd                                    : 7
+ 0x0054 (0084) H     9701 PhyClkDependencyTableOffset               : 407
+ 0x0197 (0407) B       00 RevId                                     : 0
+ 0x0198 (0408) B       01 NumEntries                                : 1
+ 0x0199 (0409) I 683c0100 Clk                                       : 81000
+ 0x019d (0413) B       00 VddInd                                    : 0
```

### Comparing `upp-0.2.0/test/AMD.RXVegaFrontier.16384.170628.rom.dump` & `upp-0.2.1/test/AMD.RXVegaFrontier.16384.170628.rom.dump`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/test/AMD.RXVegaFrontier.16384.170628.rom.rawdump` & `upp-0.2.1/test/AMD.RXVegaFrontier.16384.170628.rom.rawdump`

 * *Files 6% similar despite different names*

```diff
@@ -1,302 +1,302 @@
 PowerPlay table rev 8.1 size 642 bytes
- Offset (dec.) t Raw val. Variable name                   Decoded value
------------------------------------------------------------------------
- 0x0000 (0000) H     8202 structuresize                   : 642
- 0x0002 (0002) B       08 format_revision                 : 8
- 0x0003 (0003) B       01 content_revision                : 1
- 0x0004 (0004) B       00 TableRevision                   : 0
- 0x0005 (0005) H     5c00 TableSize                       : 92
- 0x0007 (0007) I 12070000 GoldenPPID                      : 1810
- 0x000b (0011) I 3d2b0000 GoldenRevision                  : 11069
- 0x000f (0015) H     1b00 FormatID                        : 27
- 0x0011 (0017) I 48000000 PlatformCaps                    : 72
- 0x0015 (0021) I 80a90300 MaxODEngineClock                : 240000
- 0x0019 (0025) I f0490200 MaxODMemoryClock                : 150000
- 0x001d (0029) H     3200 PowerControlLimit               : 50
- 0x001f (0031) H     0800 UlvVoltageOffset                : 8
- 0x0021 (0033) H     0000 UlvSmnclkDid                    : 0
- 0x0023 (0035) H     0000 UlvMp1clkDid                    : 0
- 0x0025 (0037) H     0000 UlvGfxclkBypass                 : 0
- 0x0027 (0039) H     0000 GfxclkSlewRate                  : 0
- 0x0029 (0041) B       00 GfxVoltageMode                  : 0
- 0x002a (0042) B       00 SocVoltageMode                  : 0
- 0x002b (0043) B       00 UclkVoltageMode                 : 0
- 0x002c (0044) B       00 UvdVoltageMode                  : 0
- 0x002d (0045) B       00 VceVoltageMode                  : 0
- 0x002e (0046) B       02 Mp0VoltageMode                  : 2
- 0x002f (0047) B       01 DcefVoltageMode                 : 1
- 0x0030 (0048) H     5c00 StateArrayOffset                : 92
- 0x005c (0092) B       02 RevId                           : 2
- 0x005d (0093) B       02 NumEntries                      : 2
- 0x005e (0094) B       00 SocClockIndexHigh               : 0
- 0x005f (0095) B       00 SocClockIndexLow                : 0
- 0x0060 (0096) B       00 GfxClockIndexHigh               : 0
- 0x0061 (0097) B       00 GfxClockIndexLow                : 0
- 0x0062 (0098) B       00 MemClockIndexHigh               : 0
- 0x0063 (0099) B       00 MemClockIndexLow                : 0
- 0x0064 (0100) H     0800 Classification                  : 8
- 0x0066 (0102) I 00000000 CapsAndSettings                 : 0
- 0x006a (0106) H     0000 Classification2                 : 0
- 0x006c (0108) B       05 SocClockIndexHigh               : 5
- 0x006d (0109) B       00 SocClockIndexLow                : 0
- 0x006e (0110) B       07 GfxClockIndexHigh               : 7
- 0x006f (0111) B       00 GfxClockIndexLow                : 0
- 0x0070 (0112) B       03 MemClockIndexHigh               : 3
- 0x0071 (0113) B       00 MemClockIndexLow                : 0
- 0x0072 (0114) H     0500 Classification                  : 5
- 0x0074 (0116) I 00000000 CapsAndSettings                 : 0
- 0x0078 (0120) H     0000 Classification2                 : 0
- 0x0032 (0050) H     1b02 FanTableOffset                  : 539
- 0x021b (0539) B       0b RevId                           : 11
- 0x021c (0540) H     e412 FanOutputSensitivity            : 4836
- 0x021e (0542) H     dc05 FanAcousticLimitRpm             : 1500
- 0x0220 (0544) H     fc08 ThrottlingRPM                   : 2300
- 0x0222 (0546) H     4100 TargetTemperature               : 65
- 0x0224 (0548) H     0f00 MinimumPWMLimit                 : 15
- 0x0226 (0550) H     5403 TargetGfxClk                    : 852
- 0x0228 (0552) H     9001 FanGainEdge                     : 400
- 0x022a (0554) H     9001 FanGainHotspot                  : 400
- 0x022c (0556) H     9001 FanGainLiquid                   : 400
- 0x022e (0558) H     9001 FanGainVrVddc                   : 400
- 0x0230 (0560) H     9001 FanGainVrMvdd                   : 400
- 0x0232 (0562) H     9001 FanGainPlx                      : 400
- 0x0234 (0564) H     9001 FanGainHbm                      : 400
- 0x0236 (0566) B       00 EnableZeroRPM                   : 0
- 0x0237 (0567) H     0000 FanStopTemperature              : 0
- 0x0239 (0569) H     0000 FanStartTemperature             : 0
- 0x023b (0571) B       02 FanParameters                   : 2
- 0x023c (0572) B       04 FanMinRPM                       : 4
- 0x023d (0573) B       21 FanMaxRPM                       : 33
- 0x0034 (0052) H     1202 ThermalControllerOffset         : 530
- 0x0212 (0530) B       01 RevId                           : 1
- 0x0213 (0531) B       18 Type                            : 24
- 0x0214 (0532) B       00 I2cLine                         : 0
- 0x0215 (0533) B       00 I2cAddress                      : 0
- 0x0216 (0534) B       00 FanParameters                   : 0
- 0x0217 (0535) B       00 FanMinRPM                       : 0
- 0x0218 (0536) B       00 FanMaxRPM                       : 0
- 0x0219 (0537) B       00 Flags                           : 0
- 0x0036 (0054) H     9400 SocclkDependencyTableOffset     : 148
- 0x0094 (0148) B       00 RevId                           : 0
- 0x0095 (0149) B       06 NumEntries                      : 6
- 0x0096 (0150) I 60ea0000 Clk                             : 60000
- 0x009a (0154) B       00 VddInd                          : 0
- 0x009b (0155) I 40190100 Clk                             : 72000
- 0x009f (0159) B       01 VddInd                          : 1
- 0x00a0 (0160) I dc4a0100 Clk                             : 84700
- 0x00a4 (0164) B       02 VddInd                          : 2
- 0x00a5 (0165) I 00770100 Clk                             : 96000
- 0x00a9 (0169) B       03 VddInd                          : 3
- 0x00aa (0170) I 90910100 Clk                             : 102800
- 0x00ae (0174) B       04 VddInd                          : 4
- 0x00af (0175) I 6cb00100 Clk                             : 110700
- 0x00b3 (0179) B       05 VddInd                          : 5
- 0x0038 (0056) H     6a01 MclkDependencyTableOffset       : 362
- 0x016a (0362) B       01 RevId                           : 1
- 0x016b (0363) B       04 NumEntries                      : 4
- 0x016c (0364) I 3c410000 MemClk                          : 16700
- 0x0170 (0368) B       00 VddInd                          : 0
- 0x0171 (0369) B       00 VddMemInd                       : 0
- 0x0172 (0370) B       00 VddciInd                        : 0
- 0x0173 (0371) I 50c30000 MemClk                          : 50000
- 0x0177 (0375) B       01 VddInd                          : 1
- 0x0178 (0376) B       00 VddMemInd                       : 0
- 0x0179 (0377) B       00 VddciInd                        : 0
- 0x017a (0378) I 80380100 MemClk                          : 80000
- 0x017e (0382) B       02 VddInd                          : 2
- 0x017f (0383) B       00 VddMemInd                       : 0
- 0x0180 (0384) B       00 VddciInd                        : 0
- 0x0181 (0385) I 24710100 MemClk                          : 94500
- 0x0185 (0389) B       03 VddInd                          : 3
- 0x0186 (0390) B       00 VddMemInd                       : 0
- 0x0187 (0391) B       00 VddciInd                        : 0
- 0x003a (0058) H     b400 GfxclkDependencyTableOffset     : 180
- 0x00b4 (0180) B       00 RevId                           : 0
- 0x00b5 (0181) B       08 NumEntries                      : 8
- 0x00b6 (0182) I d04c0100 Clk                             : 85200
- 0x00ba (0186) B       00 VddInd                          : 0
- 0x00bb (0187) H     0080 CKSVOffsetandDisable            : 32768
- 0x00bd (0189) H     0000 AVFSOffset                      : 0
- 0x00bf (0191) I 1c830100 Clk                             : 99100
- 0x00c3 (0195) B       01 VddInd                          : 1
- 0x00c4 (0196) H     0000 CKSVOffsetandDisable            : 0
- 0x00c6 (0198) H     0000 AVFSOffset                      : 0
- 0x00c8 (0200) I 88bc0100 Clk                             : 113800
- 0x00cc (0204) B       02 VddInd                          : 2
- 0x00cd (0205) H     0000 CKSVOffsetandDisable            : 0
- 0x00cf (0207) H     0000 AVFSOffset                      : 0
- 0x00d1 (0209) I b4ef0100 Clk                             : 126900
- 0x00d5 (0213) B       03 VddInd                          : 3
- 0x00d6 (0214) H     0000 CKSVOffsetandDisable            : 0
- 0x00d8 (0216) H     0000 AVFSOffset                      : 0
- 0x00da (0218) I 900e0200 Clk                             : 134800
- 0x00de (0222) B       04 VddInd                          : 4
- 0x00df (0223) H     0000 CKSVOffsetandDisable            : 0
- 0x00e1 (0225) H     0000 AVFSOffset                      : 0
- 0x00e3 (0227) I 80320200 Clk                             : 144000
- 0x00e7 (0231) B       05 VddInd                          : 5
- 0x00e8 (0232) H     0000 CKSVOffsetandDisable            : 0
- 0x00ea (0234) H     0000 AVFSOffset                      : 0
- 0x00ec (0236) I e0540200 Clk                             : 152800
- 0x00f0 (0240) B       06 VddInd                          : 6
- 0x00f1 (0241) H     0000 CKSVOffsetandDisable            : 0
- 0x00f3 (0243) H     0000 AVFSOffset                      : 0
- 0x00f5 (0245) I 00710200 Clk                             : 160000
- 0x00f9 (0249) B       07 VddInd                          : 7
- 0x00fa (0250) H     0000 CKSVOffsetandDisable            : 0
- 0x00fc (0252) H     0000 AVFSOffset                      : 0
- 0x003c (0060) H     fe00 DcefclkDependencyTableOffset    : 254
- 0x00fe (0254) B       00 RevId                           : 0
- 0x00ff (0255) B       03 NumEntries                      : 3
- 0x0100 (0256) I 60ea0000 Clk                             : 60000
- 0x0104 (0260) B       00 VddInd                          : 0
- 0x0105 (0261) I 40190100 Clk                             : 72000
- 0x0109 (0265) B       00 VddInd                          : 0
- 0x010a (0266) I 80380100 Clk                             : 80000
- 0x010e (0270) B       00 VddInd                          : 0
- 0x003e (0062) H     7a00 VddcLookupTableOffset           : 122
- 0x007a (0122) B       01 RevId                           : 1
- 0x007b (0123) B       08 NumEntries                      : 8
- 0x007c (0124) H     2003 Vdd                             : 800
- 0x007e (0126) H     8403 Vdd                             : 900
- 0x0080 (0128) H     b603 Vdd                             : 950
- 0x0082 (0130) H     e803 Vdd                             : 1000
- 0x0084 (0132) H     1a04 Vdd                             : 1050
- 0x0086 (0134) H     4c04 Vdd                             : 1100
- 0x0088 (0136) H     7e04 Vdd                             : 1150
- 0x008a (0138) H     b004 Vdd                             : 1200
- 0x0040 (0064) H     8c00 VddmemLookupTableOffset         : 140
- 0x008c (0140) B       01 RevId                           : 1
- 0x008d (0141) B       01 NumEntries                      : 1
- 0x008e (0142) H     4605 Vdd                             : 1350
- 0x0042 (0066) H     8801 MMDependencyTableOffset         : 392
- 0x0188 (0392) B       01 RevId                           : 1
- 0x0189 (0393) B       08 NumEntries                      : 8
- 0x018a (0394) B       00 VddcInd                         : 0
- 0x018b (0395) I 98850000 DClk                            : 34200
- 0x018f (0399) I 78b40000 VClk                            : 46200
- 0x0193 (0403) I 60ea0000 EClk                            : 60000
- 0x0197 (0407) I 50c30000 PSPClk                          : 50000
- 0x019b (0411) B       01 VddcInd                         : 1
- 0x019c (0412) I 80bb0000 DClk                            : 48000
- 0x01a0 (0416) I 60ea0000 VClk                            : 60000
- 0x01a4 (0420) I 940b0100 EClk                            : 68500
- 0x01a8 (0424) I 50c30000 PSPClk                          : 50000
- 0x01ac (0428) B       02 VddcInd                         : 2
- 0x01ad (0429) I 78ff0000 DClk                            : 65400
- 0x01b1 (0433) I 40190100 VClk                            : 72000
- 0x01b5 (0437) I b4270100 EClk                            : 75700
- 0x01b9 (0441) I 50c30000 PSPClk                          : 50000
- 0x01bd (0445) B       03 VddcInd                         : 3
- 0x01be (0446) I b4270100 DClk                            : 75700
- 0x01c2 (0450) I dc4a0100 VClk                            : 84700
- 0x01c6 (0454) I dc4a0100 EClk                            : 84700
- 0x01ca (0458) I 50c30000 PSPClk                          : 50000
- 0x01ce (0462) B       04 VddcInd                         : 4
- 0x01cf (0463) I dc4a0100 DClk                            : 84700
- 0x01d3 (0467) I 905f0100 VClk                            : 90000
- 0x01d7 (0471) I 905f0100 EClk                            : 90000
- 0x01db (0475) I 50c30000 PSPClk                          : 50000
- 0x01df (0479) B       05 VddcInd                         : 5
- 0x01e0 (0480) I 00770100 DClk                            : 96000
- 0x01e4 (0484) I 90910100 VClk                            : 102800
- 0x01e8 (0488) I 00770100 EClk                            : 96000
- 0x01ec (0492) I 50c30000 PSPClk                          : 50000
- 0x01f0 (0496) B       06 VddcInd                         : 6
- 0x01f1 (0497) I 90910100 DClk                            : 102800
- 0x01f5 (0501) I 6cb00100 VClk                            : 110700
- 0x01f9 (0505) I 00770100 EClk                            : 96000
- 0x01fd (0509) I 50c30000 PSPClk                          : 50000
- 0x0201 (0513) B       07 VddcInd                         : 7
- 0x0202 (0514) I 6cb00100 DClk                            : 110700
- 0x0206 (0518) I 6cb00100 VClk                            : 110700
- 0x020a (0522) I 90910100 EClk                            : 102800
- 0x020e (0526) I 50c30000 PSPClk                          : 50000
- 0x0044 (0068) H     0000 VCEStateTableOffset             : 0
- 0x0046 (0070) H     0000 Reserve                         : 0
- 0x0048 (0072) H     3e02 PowerTuneTableOffset            : 574
- 0x023e (0574) B       07 RevId                           : 7
- 0x023f (0575) H     dc00 SocketPowerLimit                : 220
- 0x0241 (0577) H     dc00 BatteryPowerLimit               : 220
- 0x0243 (0579) H     dc00 SmallPowerLimit                 : 220
- 0x0245 (0581) H     2c01 TdcLimit                        : 300
- 0x0247 (0583) H     0000 EdcLimit                        : 0
- 0x0249 (0585) H     4a00 SoftwareShutdownTemp            : 74
- 0x024b (0587) H     6900 TemperatureLimitHotSpot         : 105
- 0x024d (0589) H     4a00 TemperatureLimitLiquid1         : 74
- 0x024f (0591) H     4a00 TemperatureLimitLiquid2         : 74
- 0x0251 (0593) H     5f00 TemperatureLimitHBM             : 95
- 0x0253 (0595) H     7300 TemperatureLimitVrSoc           : 115
- 0x0255 (0597) H     7300 TemperatureLimitVrMem           : 115
- 0x0257 (0599) H     6400 TemperatureLimitPlx             : 100
- 0x0259 (0601) H     4000 LoadLineResistance              : 64
- 0x025b (0603) B       90 Liquid1_I2C_address             : 144
- 0x025c (0604) B       92 Liquid2_I2C_address             : 146
- 0x025d (0605) B       97 Liquid_I2C_Line                 : 151
- 0x025e (0606) B       60 Vr_I2C_address                  : 96
- 0x025f (0607) B       96 Vr_I2C_Line                     : 150
- 0x0260 (0608) B       00 Plx_I2C_address                 : 0
- 0x0261 (0609) B       90 Plx_I2C_Line                    : 144
- 0x0262 (0610) H     4600 TemperatureLimitTedge           : 70
- 0x0264 (0612) H     0000 BoostStartTemperature           : 0
- 0x0266 (0614) H     0000 BoostStopTemperature            : 0
- 0x0268 (0616) I 00000000 BoostClock                      : 0
- 0x026c (0620) I 00000000 Reserved                        : 0
- 0x0270 (0624) I 00000000 Reserved                        : 0
- 0x004a (0074) H     0000 HardLimitTableOffset            : 0
- 0x004c (0076) H     9000 VddciLookupTableOffset          : 144
- 0x0090 (0144) B       01 RevId                           : 1
- 0x0091 (0145) B       01 NumEntries                      : 1
- 0x0092 (0146) H     8403 Vdd                             : 900
- 0x004e (0078) H     7402 PCIETableOffset                 : 628
- 0x0274 (0628) B       02 RevId                           : 2
- 0x0275 (0629) B       02 NumEntries                      : 2
- 0x0276 (0630) I d4300000 LCLK                            : 12500
- 0x027a (0634) B       02 PCIEGenSpeed                    : 2
- 0x027b (0635) B       10 PCIELaneWidth                   : 16
- 0x027c (0636) I 60ea0000 LCLK                            : 60000
- 0x0280 (0640) B       02 PCIEGenSpeed                    : 2
- 0x0281 (0641) B       10 PCIELaneWidth                   : 16
- 0x0050 (0080) H     3901 PixclkDependencyTableOffset     : 313
- 0x0139 (0313) B       00 RevId                           : 0
- 0x013a (0314) B       08 NumEntries                      : 8
- 0x013b (0315) I 6c390000 Clk                             : 14700
- 0x013f (0319) B       00 VddInd                          : 0
- 0x0140 (0320) I 245e0000 Clk                             : 24100
- 0x0144 (0324) B       01 VddInd                          : 1
- 0x0145 (0325) I fc850000 Clk                             : 34300
- 0x0149 (0329) B       02 VddInd                          : 2
- 0x014a (0330) I acbc0000 Clk                             : 48300
- 0x014e (0334) B       03 VddInd                          : 3
- 0x014f (0335) I 34d00000 Clk                             : 53300
- 0x0153 (0339) B       04 VddInd                          : 4
- 0x0154 (0340) I 686e0100 Clk                             : 93800
- 0x0158 (0344) B       05 VddInd                          : 5
- 0x0159 (0345) I 08970100 Clk                             : 104200
- 0x015d (0349) B       06 VddInd                          : 6
- 0x015e (0350) I eca30100 Clk                             : 107500
- 0x0162 (0354) B       07 VddInd                          : 7
- 0x0052 (0082) H     0f01 DispClkDependencyTableOffset    : 271
- 0x010f (0271) B       00 RevId                           : 0
- 0x0110 (0272) B       08 NumEntries                      : 8
- 0x0111 (0273) I 286e0000 Clk                             : 28200
- 0x0115 (0277) B       00 VddInd                          : 0
- 0x0116 (0278) I 2cc90000 Clk                             : 51500
- 0x011a (0282) B       01 VddInd                          : 1
- 0x011b (0283) I f80b0100 Clk                             : 68600
- 0x011f (0287) B       02 VddInd                          : 2
- 0x0120 (0288) I 80380100 Clk                             : 80000
- 0x0124 (0292) B       03 VddInd                          : 3
- 0x0125 (0293) I 905f0100 Clk                             : 90000
- 0x0129 (0297) B       04 VddInd                          : 4
- 0x012a (0298) I f4910100 Clk                             : 102900
- 0x012e (0302) B       05 VddInd                          : 5
- 0x012f (0303) I d0b00100 Clk                             : 110800
- 0x0133 (0307) B       06 VddInd                          : 6
- 0x0134 (0308) I c0d40100 Clk                             : 120000
- 0x0138 (0312) B       07 VddInd                          : 7
- 0x0054 (0084) H     6301 PhyClkDependencyTableOffset     : 355
- 0x0163 (0355) B       00 RevId                           : 0
- 0x0164 (0356) B       01 NumEntries                      : 1
- 0x0165 (0357) I 683c0100 Clk                             : 81000
- 0x0169 (0361) B       00 VddInd                          : 0
+ Offset (dec.) t Raw val. Variable name                         Decoded value
+------------------------------------------------------------------------------
+ 0x0000 (0000) H     8202 structuresize                             : 642
+ 0x0002 (0002) B       08 format_revision                           : 8
+ 0x0003 (0003) B       01 content_revision                          : 1
+ 0x0004 (0004) B       00 TableRevision                             : 0
+ 0x0005 (0005) H     5c00 TableSize                                 : 92
+ 0x0007 (0007) I 12070000 GoldenPPID                                : 1810
+ 0x000b (0011) I 3d2b0000 GoldenRevision                            : 11069
+ 0x000f (0015) H     1b00 FormatID                                  : 27
+ 0x0011 (0017) I 48000000 PlatformCaps                              : 72
+ 0x0015 (0021) I 80a90300 MaxODEngineClock                          : 240000
+ 0x0019 (0025) I f0490200 MaxODMemoryClock                          : 150000
+ 0x001d (0029) H     3200 PowerControlLimit                         : 50
+ 0x001f (0031) H     0800 UlvVoltageOffset                          : 8
+ 0x0021 (0033) H     0000 UlvSmnclkDid                              : 0
+ 0x0023 (0035) H     0000 UlvMp1clkDid                              : 0
+ 0x0025 (0037) H     0000 UlvGfxclkBypass                           : 0
+ 0x0027 (0039) H     0000 GfxclkSlewRate                            : 0
+ 0x0029 (0041) B       00 GfxVoltageMode                            : 0
+ 0x002a (0042) B       00 SocVoltageMode                            : 0
+ 0x002b (0043) B       00 UclkVoltageMode                           : 0
+ 0x002c (0044) B       00 UvdVoltageMode                            : 0
+ 0x002d (0045) B       00 VceVoltageMode                            : 0
+ 0x002e (0046) B       02 Mp0VoltageMode                            : 2
+ 0x002f (0047) B       01 DcefVoltageMode                           : 1
+ 0x0030 (0048) H     5c00 StateArrayOffset                          : 92
+ 0x005c (0092) B       02 RevId                                     : 2
+ 0x005d (0093) B       02 NumEntries                                : 2
+ 0x005e (0094) B       00 SocClockIndexHigh                         : 0
+ 0x005f (0095) B       00 SocClockIndexLow                          : 0
+ 0x0060 (0096) B       00 GfxClockIndexHigh                         : 0
+ 0x0061 (0097) B       00 GfxClockIndexLow                          : 0
+ 0x0062 (0098) B       00 MemClockIndexHigh                         : 0
+ 0x0063 (0099) B       00 MemClockIndexLow                          : 0
+ 0x0064 (0100) H     0800 Classification                            : 8
+ 0x0066 (0102) I 00000000 CapsAndSettings                           : 0
+ 0x006a (0106) H     0000 Classification2                           : 0
+ 0x006c (0108) B       05 SocClockIndexHigh                         : 5
+ 0x006d (0109) B       00 SocClockIndexLow                          : 0
+ 0x006e (0110) B       07 GfxClockIndexHigh                         : 7
+ 0x006f (0111) B       00 GfxClockIndexLow                          : 0
+ 0x0070 (0112) B       03 MemClockIndexHigh                         : 3
+ 0x0071 (0113) B       00 MemClockIndexLow                          : 0
+ 0x0072 (0114) H     0500 Classification                            : 5
+ 0x0074 (0116) I 00000000 CapsAndSettings                           : 0
+ 0x0078 (0120) H     0000 Classification2                           : 0
+ 0x0032 (0050) H     1b02 FanTableOffset                            : 539
+ 0x021b (0539) B       0b RevId                                     : 11
+ 0x021c (0540) H     e412 FanOutputSensitivity                      : 4836
+ 0x021e (0542) H     dc05 FanAcousticLimitRpm                       : 1500
+ 0x0220 (0544) H     fc08 ThrottlingRPM                             : 2300
+ 0x0222 (0546) H     4100 TargetTemperature                         : 65
+ 0x0224 (0548) H     0f00 MinimumPWMLimit                           : 15
+ 0x0226 (0550) H     5403 TargetGfxClk                              : 852
+ 0x0228 (0552) H     9001 FanGainEdge                               : 400
+ 0x022a (0554) H     9001 FanGainHotspot                            : 400
+ 0x022c (0556) H     9001 FanGainLiquid                             : 400
+ 0x022e (0558) H     9001 FanGainVrVddc                             : 400
+ 0x0230 (0560) H     9001 FanGainVrMvdd                             : 400
+ 0x0232 (0562) H     9001 FanGainPlx                                : 400
+ 0x0234 (0564) H     9001 FanGainHbm                                : 400
+ 0x0236 (0566) B       00 EnableZeroRPM                             : 0
+ 0x0237 (0567) H     0000 FanStopTemperature                        : 0
+ 0x0239 (0569) H     0000 FanStartTemperature                       : 0
+ 0x023b (0571) B       02 FanParameters                             : 2
+ 0x023c (0572) B       04 FanMinRPM                                 : 4
+ 0x023d (0573) B       21 FanMaxRPM                                 : 33
+ 0x0034 (0052) H     1202 ThermalControllerOffset                   : 530
+ 0x0212 (0530) B       01 RevId                                     : 1
+ 0x0213 (0531) B       18 Type                                      : 24
+ 0x0214 (0532) B       00 I2cLine                                   : 0
+ 0x0215 (0533) B       00 I2cAddress                                : 0
+ 0x0216 (0534) B       00 FanParameters                             : 0
+ 0x0217 (0535) B       00 FanMinRPM                                 : 0
+ 0x0218 (0536) B       00 FanMaxRPM                                 : 0
+ 0x0219 (0537) B       00 Flags                                     : 0
+ 0x0036 (0054) H     9400 SocclkDependencyTableOffset               : 148
+ 0x0094 (0148) B       00 RevId                                     : 0
+ 0x0095 (0149) B       06 NumEntries                                : 6
+ 0x0096 (0150) I 60ea0000 Clk                                       : 60000
+ 0x009a (0154) B       00 VddInd                                    : 0
+ 0x009b (0155) I 40190100 Clk                                       : 72000
+ 0x009f (0159) B       01 VddInd                                    : 1
+ 0x00a0 (0160) I dc4a0100 Clk                                       : 84700
+ 0x00a4 (0164) B       02 VddInd                                    : 2
+ 0x00a5 (0165) I 00770100 Clk                                       : 96000
+ 0x00a9 (0169) B       03 VddInd                                    : 3
+ 0x00aa (0170) I 90910100 Clk                                       : 102800
+ 0x00ae (0174) B       04 VddInd                                    : 4
+ 0x00af (0175) I 6cb00100 Clk                                       : 110700
+ 0x00b3 (0179) B       05 VddInd                                    : 5
+ 0x0038 (0056) H     6a01 MclkDependencyTableOffset                 : 362
+ 0x016a (0362) B       01 RevId                                     : 1
+ 0x016b (0363) B       04 NumEntries                                : 4
+ 0x016c (0364) I 3c410000 MemClk                                    : 16700
+ 0x0170 (0368) B       00 VddInd                                    : 0
+ 0x0171 (0369) B       00 VddMemInd                                 : 0
+ 0x0172 (0370) B       00 VddciInd                                  : 0
+ 0x0173 (0371) I 50c30000 MemClk                                    : 50000
+ 0x0177 (0375) B       01 VddInd                                    : 1
+ 0x0178 (0376) B       00 VddMemInd                                 : 0
+ 0x0179 (0377) B       00 VddciInd                                  : 0
+ 0x017a (0378) I 80380100 MemClk                                    : 80000
+ 0x017e (0382) B       02 VddInd                                    : 2
+ 0x017f (0383) B       00 VddMemInd                                 : 0
+ 0x0180 (0384) B       00 VddciInd                                  : 0
+ 0x0181 (0385) I 24710100 MemClk                                    : 94500
+ 0x0185 (0389) B       03 VddInd                                    : 3
+ 0x0186 (0390) B       00 VddMemInd                                 : 0
+ 0x0187 (0391) B       00 VddciInd                                  : 0
+ 0x003a (0058) H     b400 GfxclkDependencyTableOffset               : 180
+ 0x00b4 (0180) B       00 RevId                                     : 0
+ 0x00b5 (0181) B       08 NumEntries                                : 8
+ 0x00b6 (0182) I d04c0100 Clk                                       : 85200
+ 0x00ba (0186) B       00 VddInd                                    : 0
+ 0x00bb (0187) H     0080 CKSVOffsetandDisable                      : 32768
+ 0x00bd (0189) H     0000 AVFSOffset                                : 0
+ 0x00bf (0191) I 1c830100 Clk                                       : 99100
+ 0x00c3 (0195) B       01 VddInd                                    : 1
+ 0x00c4 (0196) H     0000 CKSVOffsetandDisable                      : 0
+ 0x00c6 (0198) H     0000 AVFSOffset                                : 0
+ 0x00c8 (0200) I 88bc0100 Clk                                       : 113800
+ 0x00cc (0204) B       02 VddInd                                    : 2
+ 0x00cd (0205) H     0000 CKSVOffsetandDisable                      : 0
+ 0x00cf (0207) H     0000 AVFSOffset                                : 0
+ 0x00d1 (0209) I b4ef0100 Clk                                       : 126900
+ 0x00d5 (0213) B       03 VddInd                                    : 3
+ 0x00d6 (0214) H     0000 CKSVOffsetandDisable                      : 0
+ 0x00d8 (0216) H     0000 AVFSOffset                                : 0
+ 0x00da (0218) I 900e0200 Clk                                       : 134800
+ 0x00de (0222) B       04 VddInd                                    : 4
+ 0x00df (0223) H     0000 CKSVOffsetandDisable                      : 0
+ 0x00e1 (0225) H     0000 AVFSOffset                                : 0
+ 0x00e3 (0227) I 80320200 Clk                                       : 144000
+ 0x00e7 (0231) B       05 VddInd                                    : 5
+ 0x00e8 (0232) H     0000 CKSVOffsetandDisable                      : 0
+ 0x00ea (0234) H     0000 AVFSOffset                                : 0
+ 0x00ec (0236) I e0540200 Clk                                       : 152800
+ 0x00f0 (0240) B       06 VddInd                                    : 6
+ 0x00f1 (0241) H     0000 CKSVOffsetandDisable                      : 0
+ 0x00f3 (0243) H     0000 AVFSOffset                                : 0
+ 0x00f5 (0245) I 00710200 Clk                                       : 160000
+ 0x00f9 (0249) B       07 VddInd                                    : 7
+ 0x00fa (0250) H     0000 CKSVOffsetandDisable                      : 0
+ 0x00fc (0252) H     0000 AVFSOffset                                : 0
+ 0x003c (0060) H     fe00 DcefclkDependencyTableOffset              : 254
+ 0x00fe (0254) B       00 RevId                                     : 0
+ 0x00ff (0255) B       03 NumEntries                                : 3
+ 0x0100 (0256) I 60ea0000 Clk                                       : 60000
+ 0x0104 (0260) B       00 VddInd                                    : 0
+ 0x0105 (0261) I 40190100 Clk                                       : 72000
+ 0x0109 (0265) B       00 VddInd                                    : 0
+ 0x010a (0266) I 80380100 Clk                                       : 80000
+ 0x010e (0270) B       00 VddInd                                    : 0
+ 0x003e (0062) H     7a00 VddcLookupTableOffset                     : 122
+ 0x007a (0122) B       01 RevId                                     : 1
+ 0x007b (0123) B       08 NumEntries                                : 8
+ 0x007c (0124) H     2003 Vdd                                       : 800
+ 0x007e (0126) H     8403 Vdd                                       : 900
+ 0x0080 (0128) H     b603 Vdd                                       : 950
+ 0x0082 (0130) H     e803 Vdd                                       : 1000
+ 0x0084 (0132) H     1a04 Vdd                                       : 1050
+ 0x0086 (0134) H     4c04 Vdd                                       : 1100
+ 0x0088 (0136) H     7e04 Vdd                                       : 1150
+ 0x008a (0138) H     b004 Vdd                                       : 1200
+ 0x0040 (0064) H     8c00 VddmemLookupTableOffset                   : 140
+ 0x008c (0140) B       01 RevId                                     : 1
+ 0x008d (0141) B       01 NumEntries                                : 1
+ 0x008e (0142) H     4605 Vdd                                       : 1350
+ 0x0042 (0066) H     8801 MMDependencyTableOffset                   : 392
+ 0x0188 (0392) B       01 RevId                                     : 1
+ 0x0189 (0393) B       08 NumEntries                                : 8
+ 0x018a (0394) B       00 VddcInd                                   : 0
+ 0x018b (0395) I 98850000 DClk                                      : 34200
+ 0x018f (0399) I 78b40000 VClk                                      : 46200
+ 0x0193 (0403) I 60ea0000 EClk                                      : 60000
+ 0x0197 (0407) I 50c30000 PSPClk                                    : 50000
+ 0x019b (0411) B       01 VddcInd                                   : 1
+ 0x019c (0412) I 80bb0000 DClk                                      : 48000
+ 0x01a0 (0416) I 60ea0000 VClk                                      : 60000
+ 0x01a4 (0420) I 940b0100 EClk                                      : 68500
+ 0x01a8 (0424) I 50c30000 PSPClk                                    : 50000
+ 0x01ac (0428) B       02 VddcInd                                   : 2
+ 0x01ad (0429) I 78ff0000 DClk                                      : 65400
+ 0x01b1 (0433) I 40190100 VClk                                      : 72000
+ 0x01b5 (0437) I b4270100 EClk                                      : 75700
+ 0x01b9 (0441) I 50c30000 PSPClk                                    : 50000
+ 0x01bd (0445) B       03 VddcInd                                   : 3
+ 0x01be (0446) I b4270100 DClk                                      : 75700
+ 0x01c2 (0450) I dc4a0100 VClk                                      : 84700
+ 0x01c6 (0454) I dc4a0100 EClk                                      : 84700
+ 0x01ca (0458) I 50c30000 PSPClk                                    : 50000
+ 0x01ce (0462) B       04 VddcInd                                   : 4
+ 0x01cf (0463) I dc4a0100 DClk                                      : 84700
+ 0x01d3 (0467) I 905f0100 VClk                                      : 90000
+ 0x01d7 (0471) I 905f0100 EClk                                      : 90000
+ 0x01db (0475) I 50c30000 PSPClk                                    : 50000
+ 0x01df (0479) B       05 VddcInd                                   : 5
+ 0x01e0 (0480) I 00770100 DClk                                      : 96000
+ 0x01e4 (0484) I 90910100 VClk                                      : 102800
+ 0x01e8 (0488) I 00770100 EClk                                      : 96000
+ 0x01ec (0492) I 50c30000 PSPClk                                    : 50000
+ 0x01f0 (0496) B       06 VddcInd                                   : 6
+ 0x01f1 (0497) I 90910100 DClk                                      : 102800
+ 0x01f5 (0501) I 6cb00100 VClk                                      : 110700
+ 0x01f9 (0505) I 00770100 EClk                                      : 96000
+ 0x01fd (0509) I 50c30000 PSPClk                                    : 50000
+ 0x0201 (0513) B       07 VddcInd                                   : 7
+ 0x0202 (0514) I 6cb00100 DClk                                      : 110700
+ 0x0206 (0518) I 6cb00100 VClk                                      : 110700
+ 0x020a (0522) I 90910100 EClk                                      : 102800
+ 0x020e (0526) I 50c30000 PSPClk                                    : 50000
+ 0x0044 (0068) H     0000 VCEStateTableOffset                       : 0
+ 0x0046 (0070) H     0000 Reserve                                   : 0
+ 0x0048 (0072) H     3e02 PowerTuneTableOffset                      : 574
+ 0x023e (0574) B       07 RevId                                     : 7
+ 0x023f (0575) H     dc00 SocketPowerLimit                          : 220
+ 0x0241 (0577) H     dc00 BatteryPowerLimit                         : 220
+ 0x0243 (0579) H     dc00 SmallPowerLimit                           : 220
+ 0x0245 (0581) H     2c01 TdcLimit                                  : 300
+ 0x0247 (0583) H     0000 EdcLimit                                  : 0
+ 0x0249 (0585) H     4a00 SoftwareShutdownTemp                      : 74
+ 0x024b (0587) H     6900 TemperatureLimitHotSpot                   : 105
+ 0x024d (0589) H     4a00 TemperatureLimitLiquid1                   : 74
+ 0x024f (0591) H     4a00 TemperatureLimitLiquid2                   : 74
+ 0x0251 (0593) H     5f00 TemperatureLimitHBM                       : 95
+ 0x0253 (0595) H     7300 TemperatureLimitVrSoc                     : 115
+ 0x0255 (0597) H     7300 TemperatureLimitVrMem                     : 115
+ 0x0257 (0599) H     6400 TemperatureLimitPlx                       : 100
+ 0x0259 (0601) H     4000 LoadLineResistance                        : 64
+ 0x025b (0603) B       90 Liquid1_I2C_address                       : 144
+ 0x025c (0604) B       92 Liquid2_I2C_address                       : 146
+ 0x025d (0605) B       97 Liquid_I2C_Line                           : 151
+ 0x025e (0606) B       60 Vr_I2C_address                            : 96
+ 0x025f (0607) B       96 Vr_I2C_Line                               : 150
+ 0x0260 (0608) B       00 Plx_I2C_address                           : 0
+ 0x0261 (0609) B       90 Plx_I2C_Line                              : 144
+ 0x0262 (0610) H     4600 TemperatureLimitTedge                     : 70
+ 0x0264 (0612) H     0000 BoostStartTemperature                     : 0
+ 0x0266 (0614) H     0000 BoostStopTemperature                      : 0
+ 0x0268 (0616) I 00000000 BoostClock                                : 0
+ 0x026c (0620) I 00000000 Reserved                                  : 0
+ 0x0270 (0624) I 00000000 Reserved                                  : 0
+ 0x004a (0074) H     0000 HardLimitTableOffset                      : 0
+ 0x004c (0076) H     9000 VddciLookupTableOffset                    : 144
+ 0x0090 (0144) B       01 RevId                                     : 1
+ 0x0091 (0145) B       01 NumEntries                                : 1
+ 0x0092 (0146) H     8403 Vdd                                       : 900
+ 0x004e (0078) H     7402 PCIETableOffset                           : 628
+ 0x0274 (0628) B       02 RevId                                     : 2
+ 0x0275 (0629) B       02 NumEntries                                : 2
+ 0x0276 (0630) I d4300000 LCLK                                      : 12500
+ 0x027a (0634) B       02 PCIEGenSpeed                              : 2
+ 0x027b (0635) B       10 PCIELaneWidth                             : 16
+ 0x027c (0636) I 60ea0000 LCLK                                      : 60000
+ 0x0280 (0640) B       02 PCIEGenSpeed                              : 2
+ 0x0281 (0641) B       10 PCIELaneWidth                             : 16
+ 0x0050 (0080) H     3901 PixclkDependencyTableOffset               : 313
+ 0x0139 (0313) B       00 RevId                                     : 0
+ 0x013a (0314) B       08 NumEntries                                : 8
+ 0x013b (0315) I 6c390000 Clk                                       : 14700
+ 0x013f (0319) B       00 VddInd                                    : 0
+ 0x0140 (0320) I 245e0000 Clk                                       : 24100
+ 0x0144 (0324) B       01 VddInd                                    : 1
+ 0x0145 (0325) I fc850000 Clk                                       : 34300
+ 0x0149 (0329) B       02 VddInd                                    : 2
+ 0x014a (0330) I acbc0000 Clk                                       : 48300
+ 0x014e (0334) B       03 VddInd                                    : 3
+ 0x014f (0335) I 34d00000 Clk                                       : 53300
+ 0x0153 (0339) B       04 VddInd                                    : 4
+ 0x0154 (0340) I 686e0100 Clk                                       : 93800
+ 0x0158 (0344) B       05 VddInd                                    : 5
+ 0x0159 (0345) I 08970100 Clk                                       : 104200
+ 0x015d (0349) B       06 VddInd                                    : 6
+ 0x015e (0350) I eca30100 Clk                                       : 107500
+ 0x0162 (0354) B       07 VddInd                                    : 7
+ 0x0052 (0082) H     0f01 DispClkDependencyTableOffset              : 271
+ 0x010f (0271) B       00 RevId                                     : 0
+ 0x0110 (0272) B       08 NumEntries                                : 8
+ 0x0111 (0273) I 286e0000 Clk                                       : 28200
+ 0x0115 (0277) B       00 VddInd                                    : 0
+ 0x0116 (0278) I 2cc90000 Clk                                       : 51500
+ 0x011a (0282) B       01 VddInd                                    : 1
+ 0x011b (0283) I f80b0100 Clk                                       : 68600
+ 0x011f (0287) B       02 VddInd                                    : 2
+ 0x0120 (0288) I 80380100 Clk                                       : 80000
+ 0x0124 (0292) B       03 VddInd                                    : 3
+ 0x0125 (0293) I 905f0100 Clk                                       : 90000
+ 0x0129 (0297) B       04 VddInd                                    : 4
+ 0x012a (0298) I f4910100 Clk                                       : 102900
+ 0x012e (0302) B       05 VddInd                                    : 5
+ 0x012f (0303) I d0b00100 Clk                                       : 110800
+ 0x0133 (0307) B       06 VddInd                                    : 6
+ 0x0134 (0308) I c0d40100 Clk                                       : 120000
+ 0x0138 (0312) B       07 VddInd                                    : 7
+ 0x0054 (0084) H     6301 PhyClkDependencyTableOffset               : 355
+ 0x0163 (0355) B       00 RevId                                     : 0
+ 0x0164 (0356) B       01 NumEntries                                : 1
+ 0x0165 (0357) I 683c0100 Clk                                       : 81000
+ 0x0169 (0361) B       00 VddInd                                    : 0
```

### Comparing `upp-0.2.0/test/AMD.RadeonVII.16384.190116.rom.dump` & `upp-0.2.1/test/AMD.RadeonVII.16384.190116.rom.dump`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/test/AMD.RadeonVII.16384.190116.rom.rawdump` & `upp-0.2.1/test/AMD.RX5700XT.8192.190616.rom.rawdump`

 * *Files 20% similar despite different names*

```diff
@@ -1,658 +1,706 @@
-PowerPlay table rev 11.0 size 1730 bytes
- Offset (dec.) t Raw val. Variable name                   Decoded value
------------------------------------------------------------------------
- 0x0000 (0000) H     c206 structuresize                   : 1730
- 0x0002 (0002) B       0b format_revision                 : 11
- 0x0003 (0003) B       00 content_revision                : 0
- 0x0004 (0004) B       02 TableRevision                   : 2
- 0x0005 (0005) H     c206 TableSize                       : 1730
- 0x0007 (0007) I 34080000 GoldenPPID                      : 2100
- 0x000b (0011) I a4350000 GoldenRevision                  : 13732
- 0x000f (0015) H     7c00 FormatID                        : 124
- 0x0011 (0017) I 09000000 PlatformCaps                    : 9
- 0x0015 (0021) B       1a ThermalControllerType           : 26
- 0x0016 (0022) H     fa00 SmallPowerLimit1                : 250
- 0x0018 (0024) H     fa00 SmallPowerLimit2                : 250
- 0x001a (0026) H     fa00 BoostPowerLimit                 : 250
- 0x001c (0028) H     0000 ODTurboPowerLimit               : 0
- 0x001e (0030) H     0000 ODPowerSavePowerLimit           : 0
- 0x0020 (0032) H     7600 SoftwareShutdownTemp            : 118
- 0x0022 (0034) B       01 TableRevision                   : 1
- 0x0023 (0035) I 0b000000 PowerSavingClockCount           : 11
- 0x0027 (0039) I 09070000 PowerSavingClockMax             : 1801
- 0x002b (0043) I 6e040000 PowerSavingClockMax             : 1134
- 0x002f (0047) I cc030000 PowerSavingClockMax             : 972
- 0x0033 (0051) I cc030000 PowerSavingClockMax             : 972
- 0x0037 (0055) I cc030000 PowerSavingClockMax             : 972
- 0x003b (0059) I e8030000 PowerSavingClockMax             : 1000
- 0x003f (0063) I c9040000 PowerSavingClockMax             : 1225
- 0x0043 (0067) I 6e040000 PowerSavingClockMax             : 1134
- 0x0047 (0071) I 6e040000 PowerSavingClockMax             : 1134
- 0x004b (0075) I 34040000 PowerSavingClockMax             : 1076
- 0x004f (0079) I 2a030000 PowerSavingClockMax             : 810
- 0x0053 (0083) I 00000000 PowerSavingClockMax             : 0
- 0x0057 (0087) I 00000000 PowerSavingClockMax             : 0
- 0x005b (0091) I 00000000 PowerSavingClockMax             : 0
- 0x005f (0095) I 00000000 PowerSavingClockMax             : 0
- 0x0063 (0099) I 00000000 PowerSavingClockMax             : 0
- 0x0067 (0103) I bc020000 PowerSavingClockMin             : 700
- 0x006b (0107) I 66010000 PowerSavingClockMin             : 358
- 0x006f (0111) I 36010000 PowerSavingClockMin             : 310
- 0x0073 (0115) I 36010000 PowerSavingClockMin             : 310
- 0x0077 (0119) I 36010000 PowerSavingClockMin             : 310
- 0x007b (0123) I 5e010000 PowerSavingClockMin             : 350
- 0x007f (0127) I 26020000 PowerSavingClockMin             : 550
- 0x0083 (0131) I 66010000 PowerSavingClockMin             : 358
- 0x0087 (0135) I 66010000 PowerSavingClockMin             : 358
- 0x008b (0139) I 93000000 PowerSavingClockMin             : 147
- 0x008f (0143) I 0e010000 PowerSavingClockMin             : 270
- 0x0093 (0147) I 00000000 PowerSavingClockMin             : 0
- 0x0097 (0151) I 00000000 PowerSavingClockMin             : 0
- 0x009b (0155) I 00000000 PowerSavingClockMin             : 0
- 0x009f (0159) I 00000000 PowerSavingClockMin             : 0
- 0x00a3 (0163) I 00000000 PowerSavingClockMin             : 0
- 0x00a7 (0167) B       01 ODTableRevision                 : 1
- 0x00a8 (0168) I 0e000000 ODFeatureCount                  : 14
- 0x00ac (0172) B       01 ODFeatureCapabilities           : 1
- 0x00ad (0173) B       01 ODFeatureCapabilities           : 1
- 0x00ae (0174) B       01 ODFeatureCapabilities           : 1
- 0x00af (0175) B       01 ODFeatureCapabilities           : 1
- 0x00b0 (0176) B       01 ODFeatureCapabilities           : 1
- 0x00b1 (0177) B       01 ODFeatureCapabilities           : 1
- 0x00b2 (0178) B       01 ODFeatureCapabilities           : 1
- 0x00b3 (0179) B       01 ODFeatureCapabilities           : 1
- 0x00b4 (0180) B       01 ODFeatureCapabilities           : 1
- 0x00b5 (0181) B       00 ODFeatureCapabilities           : 0
- 0x00b6 (0182) B       01 ODFeatureCapabilities           : 1
- 0x00b7 (0183) B       01 ODFeatureCapabilities           : 1
- 0x00b8 (0184) B       01 ODFeatureCapabilities           : 1
- 0x00b9 (0185) B       01 ODFeatureCapabilities           : 1
- 0x00ba (0186) B       00 ODFeatureCapabilities           : 0
- 0x00bb (0187) B       00 ODFeatureCapabilities           : 0
- 0x00bc (0188) B       00 ODFeatureCapabilities           : 0
- 0x00bd (0189) B       00 ODFeatureCapabilities           : 0
- 0x00be (0190) B       00 ODFeatureCapabilities           : 0
- 0x00bf (0191) B       00 ODFeatureCapabilities           : 0
- 0x00c0 (0192) B       00 ODFeatureCapabilities           : 0
- 0x00c1 (0193) B       00 ODFeatureCapabilities           : 0
- 0x00c2 (0194) B       00 ODFeatureCapabilities           : 0
- 0x00c3 (0195) B       00 ODFeatureCapabilities           : 0
- 0x00c4 (0196) B       00 ODFeatureCapabilities           : 0
- 0x00c5 (0197) B       00 ODFeatureCapabilities           : 0
- 0x00c6 (0198) B       00 ODFeatureCapabilities           : 0
- 0x00c7 (0199) B       00 ODFeatureCapabilities           : 0
- 0x00c8 (0200) B       00 ODFeatureCapabilities           : 0
- 0x00c9 (0201) B       00 ODFeatureCapabilities           : 0
- 0x00ca (0202) B       00 ODFeatureCapabilities           : 0
- 0x00cb (0203) B       00 ODFeatureCapabilities           : 0
- 0x00cc (0204) I 1d000000 ODSettingCount                  : 29
- 0x00d0 (0208) I 98080000 ODSettingsMax                   : 2200
- 0x00d4 (0212) I 98080000 ODSettingsMax                   : 2200
- 0x00d8 (0216) I 98080000 ODSettingsMax                   : 2200
- 0x00dc (0220) I c2040000 ODSettingsMax                   : 1218
- 0x00e0 (0224) I 98080000 ODSettingsMax                   : 2200
- 0x00e4 (0228) I c2040000 ODSettingsMax                   : 1218
- 0x00e8 (0232) I 98080000 ODSettingsMax                   : 2200
- 0x00ec (0236) I c2040000 ODSettingsMax                   : 1218
- 0x00f0 (0240) I b0040000 ODSettingsMax                   : 1200
- 0x00f4 (0244) I 14000000 ODSettingsMax                   : 20
- 0x00f8 (0248) I 0a0f0000 ODSettingsMax                   : 3850
- 0x00fc (0252) I 0a0f0000 ODSettingsMax                   : 3850
- 0x0100 (0256) I 5f000000 ODSettingsMax                   : 95
- 0x0104 (0260) I 6e000000 ODSettingsMax                   : 110
- 0x0108 (0264) I 02000000 ODSettingsMax                   : 2
- 0x010c (0268) I 00000000 ODSettingsMax                   : 0
- 0x0110 (0272) I 01000000 ODSettingsMax                   : 1
- 0x0114 (0276) I 01000000 ODSettingsMax                   : 1
- 0x0118 (0280) I 01000000 ODSettingsMax                   : 1
- 0x011c (0284) I 5f000000 ODSettingsMax                   : 95
- 0x0120 (0288) I 64000000 ODSettingsMax                   : 100
- 0x0124 (0292) I 5f000000 ODSettingsMax                   : 95
- 0x0128 (0296) I 64000000 ODSettingsMax                   : 100
- 0x012c (0300) I 5f000000 ODSettingsMax                   : 95
- 0x0130 (0304) I 64000000 ODSettingsMax                   : 100
- 0x0134 (0308) I 5f000000 ODSettingsMax                   : 95
- 0x0138 (0312) I 64000000 ODSettingsMax                   : 100
- 0x013c (0316) I 5f000000 ODSettingsMax                   : 95
- 0x0140 (0320) I 64000000 ODSettingsMax                   : 100
- 0x0144 (0324) I 00000000 ODSettingsMax                   : 0
- 0x0148 (0328) I 00000000 ODSettingsMax                   : 0
- 0x014c (0332) I 00000000 ODSettingsMax                   : 0
- 0x0150 (0336) I 28030000 ODSettingsMin                   : 808
- 0x0154 (0340) I 28030000 ODSettingsMin                   : 808
- 0x0158 (0344) I 28030000 ODSettingsMin                   : 808
- 0x015c (0348) I e2020000 ODSettingsMin                   : 738
- 0x0160 (0352) I 28030000 ODSettingsMin                   : 808
- 0x0164 (0356) I e2020000 ODSettingsMin                   : 738
- 0x0168 (0360) I 28030000 ODSettingsMin                   : 808
- 0x016c (0364) I e2020000 ODSettingsMin                   : 738
- 0x0170 (0368) I 5e010000 ODSettingsMin                   : 350
- 0x0174 (0372) I 14000000 ODSettingsMin                   : 20
- 0x0178 (0376) I c2010000 ODSettingsMin                   : 450
- 0x017c (0380) I c2010000 ODSettingsMin                   : 450
- 0x0180 (0384) I 19000000 ODSettingsMin                   : 25
- 0x0184 (0388) I 32000000 ODSettingsMin                   : 50
- 0x0188 (0392) I 00000000 ODSettingsMin                   : 0
- 0x018c (0396) I 00000000 ODSettingsMin                   : 0
- 0x0190 (0400) I 00000000 ODSettingsMin                   : 0
- 0x0194 (0404) I 00000000 ODSettingsMin                   : 0
- 0x0198 (0408) I 00000000 ODSettingsMin                   : 0
- 0x019c (0412) I 19000000 ODSettingsMin                   : 25
- 0x01a0 (0416) I 14000000 ODSettingsMin                   : 20
- 0x01a4 (0420) I 19000000 ODSettingsMin                   : 25
- 0x01a8 (0424) I 14000000 ODSettingsMin                   : 20
- 0x01ac (0428) I 19000000 ODSettingsMin                   : 25
- 0x01b0 (0432) I 14000000 ODSettingsMin                   : 20
- 0x01b4 (0436) I 19000000 ODSettingsMin                   : 25
- 0x01b8 (0440) I 14000000 ODSettingsMin                   : 20
- 0x01bc (0444) I 19000000 ODSettingsMin                   : 25
- 0x01c0 (0448) I 14000000 ODSettingsMin                   : 20
- 0x01c4 (0452) I 00000000 ODSettingsMin                   : 0
- 0x01c8 (0456) I 00000000 ODSettingsMin                   : 0
- 0x01cc (0460) I 00000000 ODSettingsMin                   : 0
- 0x01d0 (0464) H     0000 Reserve                         : 0
- 0x01d2 (0466) H     0000 Reserve                         : 0
- 0x01d4 (0468) H     0000 Reserve                         : 0
- 0x01d6 (0470) H     0000 Reserve                         : 0
- 0x01d8 (0472) H     0000 Reserve                         : 0
- 0x01da (0474) I 03000000 Version                         : 3
- 0x01de (0478) I ffeff439 FeaturesToRun                   : 972353535
- 0x01e2 (0482) I 00000000 FeaturesToRun                   : 0
- 0x01e6 (0486) H     fa00 SocketPowerLimitAc0             : 250
- 0x01e8 (0488) H     0000 SocketPowerLimitAc0Tau          : 0
- 0x01ea (0490) H     0000 SocketPowerLimitAc1             : 0
- 0x01ec (0492) H     0000 SocketPowerLimitAc1Tau          : 0
- 0x01ee (0494) H     0000 SocketPowerLimitAc2             : 0
- 0x01f0 (0496) H     0000 SocketPowerLimitAc2Tau          : 0
- 0x01f2 (0498) H     0000 SocketPowerLimitAc3             : 0
- 0x01f4 (0500) H     0000 SocketPowerLimitAc3Tau          : 0
- 0x01f6 (0502) H     fa00 SocketPowerLimitDc              : 250
- 0x01f8 (0504) H     0000 SocketPowerLimitDcTau           : 0
- 0x01fa (0506) H     3200 TdcLimitSoc                     : 50
- 0x01fc (0508) H     0000 TdcLimitSocTau                  : 0
- 0x01fe (0510) H     4a01 TdcLimitGfx                     : 330
- 0x0200 (0512) H     0000 TdcLimitGfxTau                  : 0
- 0x0202 (0514) H     6400 TedgeLimit                      : 100
- 0x0204 (0516) H     6e00 ThotspotLimit                   : 110
- 0x0206 (0518) H     5e00 ThbmLimit                       : 94
- 0x0208 (0520) H     7300 Tvr_gfxLimit                    : 115
- 0x020a (0522) H     7300 Tvr_memLimit                    : 115
- 0x020c (0524) H     ffff Tliquid1Limit                   : 65535
- 0x020e (0526) H     ffff Tliquid2Limit                   : 65535
- 0x0210 (0528) H     ffff TplxLimit                       : 65535
- 0x0212 (0530) I 00000000 FitLimit                        : 0
- 0x0216 (0534) H     0000 PpmPowerLimit                   : 0
- 0x0218 (0536) H     0000 PpmTemperatureThreshold         : 0
- 0x021a (0538) B       01 MemoryOnPackage                 : 1
- 0x021b (0539) B       00 padding8_limits                 : 0
- 0x021c (0540) H     7300 Tvr_SocLimit                    : 115
- 0x021e (0542) H     0000 UlvVoltageOffsetSoc             : 0
- 0x0220 (0544) H     0000 UlvVoltageOffsetGfx             : 0
- 0x0222 (0546) B       00 UlvSmnclkDid                    : 0
- 0x0223 (0547) B       00 UlvMp1clkDid                    : 0
- 0x0224 (0548) B       00 UlvGfxclkBypass                 : 0
- 0x0225 (0549) B       00 Padding234                      : 0
- 0x0226 (0550) H     860b MinVoltageGfx                   : 2950
- 0x0228 (0552) H     220b MinVoltageSoc                   : 2850
- 0x022a (0554) H     0b13 MaxVoltageGfx                   : 4875
- 0x022c (0556) H     4312 MaxVoltageSoc                   : 4675
- 0x022e (0558) H     2600 LoadLineResistanceGfx           : 38
- 0x0230 (0560) H     0000 LoadLineResistanceSoc           : 0
- 0x0232 (0562) B       01 VoltageMode                     : 1
- 0x0233 (0563) B       01 SnapToDiscrete                  : 1
- 0x0234 (0564) B       09 NumDiscreteLevels               : 9
- 0x0235 (0565) B       00 padding                         : 0
- 0x0236 (0566) f 00000000 m                               : 0
- 0x023a (0570) f 00000000 b                               : 0
- 0x023e (0574) f 5bb1bf3e a                               : 0.3744
- 0x0242 (0578) f ec51f8be b                               :-0.485
- 0x0246 (0582) f 6519523f c                               : 0.8207
- 0x024a (0586) B       00 VoltageMode                     : 0
- 0x024b (0587) B       01 SnapToDiscrete                  : 1
- 0x024c (0588) B       08 NumDiscreteLevels               : 8
- 0x024d (0589) B       00 padding                         : 0
- 0x024e (0590) f 643b9f3f m                               : 1.244
- 0x0252 (0594) f 16dea5bd b                               :-0.08099
- 0x0256 (0598) f 00000000 a                               : 0
- 0x025a (0602) f 00000000 b                               : 0
- 0x025e (0606) f 00000000 c                               : 0
- 0x0262 (0610) B       00 VoltageMode                     : 0
- 0x0263 (0611) B       01 SnapToDiscrete                  : 1
- 0x0264 (0612) B       08 NumDiscreteLevels               : 8
- 0x0265 (0613) B       00 padding                         : 0
- 0x0266 (0614) f 355e9a3f m                               : 1.206
- 0x026a (0618) f 8f362e3e b                               : 0.17013
- 0x026e (0622) f 00000000 a                               : 0
- 0x0272 (0626) f 00000000 b                               : 0
- 0x0276 (0630) f 00000000 c                               : 0
- 0x027a (0634) B       00 VoltageMode                     : 0
- 0x027b (0635) B       01 SnapToDiscrete                  : 1
- 0x027c (0636) B       08 NumDiscreteLevels               : 8
- 0x027d (0637) B       00 padding                         : 0
- 0x027e (0638) f 696fb03f m                               : 1.3784
- 0x0282 (0642) f 4833163d b                               : 0.03667
- 0x0286 (0646) f 00000000 a                               : 0
- 0x028a (0650) f 00000000 b                               : 0
- 0x028e (0654) f 00000000 c                               : 0
- 0x0292 (0658) B       00 VoltageMode                     : 0
- 0x0293 (0659) B       01 SnapToDiscrete                  : 1
- 0x0294 (0660) B       08 NumDiscreteLevels               : 8
- 0x0295 (0661) B       00 padding                         : 0
- 0x0296 (0662) f e561a13f m                               : 1.2608
- 0x029a (0666) f 12f758bd b                               :-0.05297
- 0x029e (0670) f 00000000 a                               : 0
- 0x02a2 (0674) f 00000000 b                               : 0
- 0x02a6 (0678) f 00000000 c                               : 0
- 0x02aa (0682) B       00 VoltageMode                     : 0
- 0x02ab (0683) B       01 SnapToDiscrete                  : 1
- 0x02ac (0684) B       03 NumDiscreteLevels               : 3
- 0x02ad (0685) B       00 padding                         : 0
- 0x02ae (0686) f b515833f m                               : 1.0241
- 0x02b2 (0690) f c2dd193e b                               : 0.15026
- 0x02b6 (0694) f 00000000 a                               : 0
- 0x02ba (0698) f 00000000 b                               : 0
- 0x02be (0702) f 00000000 c                               : 0
- 0x02c2 (0706) B       00 VoltageMode                     : 0
- 0x02c3 (0707) B       01 SnapToDiscrete                  : 1
- 0x02c4 (0708) B       08 NumDiscreteLevels               : 8
- 0x02c5 (0709) B       00 padding                         : 0
- 0x02c6 (0710) f 8638863f m                               : 1.0486
- 0x02ca (0714) f 0ebe303e b                               : 0.1726
- 0x02ce (0718) f 00000000 a                               : 0
- 0x02d2 (0722) f 00000000 b                               : 0
- 0x02d6 (0726) f 00000000 c                               : 0
- 0x02da (0730) B       00 VoltageMode                     : 0
- 0x02db (0731) B       01 SnapToDiscrete                  : 1
- 0x02dc (0732) B       08 NumDiscreteLevels               : 8
- 0x02dd (0733) B       00 padding                         : 0
- 0x02de (0734) f 83c05a3f m                               : 0.8545
- 0x02e2 (0738) f 4da1f33d b                               : 0.11896
- 0x02e6 (0742) f 00000000 a                               : 0
- 0x02ea (0746) f 00000000 b                               : 0
- 0x02ee (0750) f 00000000 c                               : 0
- 0x02f2 (0754) B       02 VoltageMode                     : 2
- 0x02f3 (0755) B       01 SnapToDiscrete                  : 1
- 0x02f4 (0756) B       08 NumDiscreteLevels               : 8
- 0x02f5 (0757) B       00 padding                         : 0
- 0x02f6 (0758) f 00000000 m                               : 0
- 0x02fa (0762) f 00000000 b                               : 0
- 0x02fe (0766) f a4708d3f a                               : 1.105
- 0x0302 (0770) f e41485bf b                               :-1.0397
- 0x0306 (0774) f d5e7323f c                               : 0.69885
- 0x030a (0778) B       02 VoltageMode                     : 2
- 0x030b (0779) B       01 SnapToDiscrete                  : 1
- 0x030c (0780) B       03 NumDiscreteLevels               : 3
- 0x030d (0781) B       00 padding                         : 0
- 0x030e (0782) f 00000000 m                               : 0
- 0x0312 (0786) f 00000000 b                               : 0
- 0x0316 (0790) f 00000000 a                               : 0
- 0x031a (0794) f 00000000 b                               : 0
- 0x031e (0798) f d5e7323f c                               : 0.69885
- 0x0322 (0802) B       01 VoltageMode                     : 1
- 0x0323 (0803) B       01 SnapToDiscrete                  : 1
- 0x0324 (0804) B       08 NumDiscreteLevels               : 8
- 0x0325 (0805) B       00 padding                         : 0
- 0x0326 (0806) f 0000803f m                               : 1
- 0x032a (0810) f 00000000 b                               : 0
- 0x032e (0814) f d191fc3e a                               : 0.4933
- 0x0332 (0818) f 1f852bbf b                               :-0.67
- 0x0336 (0822) f 3277753f c                               : 0.95885
- 0x033a (0826) H     bc02 FreqTableGfx                    : 700
- 0x033c (0828) H     2803 FreqTableGfx                    : 808
- 0x033e (0830) H     6e04 FreqTableGfx                    : 1134
- 0x0340 (0832) H     5c05 FreqTableGfx                    : 1372
- 0x0342 (0834) H     0a06 FreqTableGfx                    : 1546
- 0x0344 (0836) H     9306 FreqTableGfx                    : 1683
- 0x0346 (0838) H     d506 FreqTableGfx                    : 1749
- 0x0348 (0840) H     ed06 FreqTableGfx                    : 1773
- 0x034a (0842) H     0907 FreqTableGfx                    : 1801
- 0x034c (0844) H     0000 FreqTableGfx                    : 0
- 0x034e (0846) H     0000 FreqTableGfx                    : 0
- 0x0350 (0848) H     0000 FreqTableGfx                    : 0
- 0x0352 (0850) H     0000 FreqTableGfx                    : 0
- 0x0354 (0852) H     0000 FreqTableGfx                    : 0
- 0x0356 (0854) H     0000 FreqTableGfx                    : 0
- 0x0358 (0856) H     0000 FreqTableGfx                    : 0
- 0x035a (0858) H     6601 FreqTableVclk                   : 358
- 0x035c (0860) H     e601 FreqTableVclk                   : 486
- 0x035e (0862) H     6b02 FreqTableVclk                   : 619
- 0x0360 (0864) H     f402 FreqTableVclk                   : 756
- 0x0362 (0866) H     5203 FreqTableVclk                   : 850
- 0x0364 (0868) H     cc03 FreqTableVclk                   : 972
- 0x0366 (0870) H     6e04 FreqTableVclk                   : 1134
- 0x0368 (0872) H     6e04 FreqTableVclk                   : 1134
- 0x036a (0874) H     3601 FreqTableDclk                   : 310
- 0x036c (0876) H     9001 FreqTableDclk                   : 400
- 0x036e (0878) H     0c02 FreqTableDclk                   : 524
- 0x0370 (0880) H     6b02 FreqTableDclk                   : 619
- 0x0372 (0882) H     a802 FreqTableDclk                   : 680
- 0x0374 (0884) H     f402 FreqTableDclk                   : 756
- 0x0376 (0886) H     5203 FreqTableDclk                   : 850
- 0x0378 (0888) H     cc03 FreqTableDclk                   : 972
- 0x037a (0890) H     3601 FreqTableEclk                   : 310
- 0x037c (0892) H     9001 FreqTableEclk                   : 400
- 0x037e (0894) H     0c02 FreqTableEclk                   : 524
- 0x0380 (0896) H     6b02 FreqTableEclk                   : 619
- 0x0382 (0898) H     a802 FreqTableEclk                   : 680
- 0x0384 (0900) H     f402 FreqTableEclk                   : 756
- 0x0386 (0902) H     5203 FreqTableEclk                   : 850
- 0x0388 (0904) H     cc03 FreqTableEclk                   : 972
- 0x038a (0906) H     3601 FreqTableSocclk                 : 310
- 0x038c (0908) H     0c02 FreqTableSocclk                 : 524
- 0x038e (0910) H     3702 FreqTableSocclk                 : 567
- 0x0390 (0912) H     6b02 FreqTableSocclk                 : 619
- 0x0392 (0914) H     a802 FreqTableSocclk                 : 680
- 0x0394 (0916) H     f402 FreqTableSocclk                 : 756
- 0x0396 (0918) H     5203 FreqTableSocclk                 : 850
- 0x0398 (0920) H     cc03 FreqTableSocclk                 : 972
- 0x039a (0922) H     5e01 FreqTableUclk                   : 350
- 0x039c (0924) H     2003 FreqTableUclk                   : 800
- 0x039e (0926) H     e803 FreqTableUclk                   : 1000
- 0x03a0 (0928) H     e803 FreqTableUclk                   : 1000
- 0x03a2 (0930) H     2602 FreqTableFclk                   : 550
- 0x03a4 (0932) H     6202 FreqTableFclk                   : 610
- 0x03a6 (0934) H     b202 FreqTableFclk                   : 690
- 0x03a8 (0936) H     f802 FreqTableFclk                   : 760
- 0x03aa (0938) H     6603 FreqTableFclk                   : 870
- 0x03ac (0940) H     c003 FreqTableFclk                   : 960
- 0x03ae (0942) H     3804 FreqTableFclk                   : 1080
- 0x03b0 (0944) H     c904 FreqTableFclk                   : 1225
- 0x03b2 (0946) H     6601 FreqTableDcefclk                : 358
- 0x03b4 (0948) H     c601 FreqTableDcefclk                : 454
- 0x03b6 (0950) H     3702 FreqTableDcefclk                : 567
- 0x03b8 (0952) H     a802 FreqTableDcefclk                : 680
- 0x03ba (0954) H     f402 FreqTableDcefclk                : 756
- 0x03bc (0956) H     5203 FreqTableDcefclk                : 850
- 0x03be (0958) H     cc03 FreqTableDcefclk                : 972
- 0x03c0 (0960) H     6e04 FreqTableDcefclk                : 1134
- 0x03c2 (0962) H     6601 FreqTableDispclk                : 358
- 0x03c4 (0964) H     c601 FreqTableDispclk                : 454
- 0x03c6 (0966) H     3702 FreqTableDispclk                : 567
- 0x03c8 (0968) H     a802 FreqTableDispclk                : 680
- 0x03ca (0970) H     f402 FreqTableDispclk                : 756
- 0x03cc (0972) H     5203 FreqTableDispclk                : 850
- 0x03ce (0974) H     cc03 FreqTableDispclk                : 972
- 0x03d0 (0976) H     6e04 FreqTableDispclk                : 1134
- 0x03d2 (0978) H     9300 FreqTablePixclk                 : 147
- 0x03d4 (0980) H     f200 FreqTablePixclk                 : 242
- 0x03d6 (0982) H     5801 FreqTablePixclk                 : 344
- 0x03d8 (0984) H     e401 FreqTablePixclk                 : 484
- 0x03da (0986) H     1502 FreqTablePixclk                 : 533
- 0x03dc (0988) H     aa03 FreqTablePixclk                 : 938
- 0x03de (0990) H     1304 FreqTablePixclk                 : 1043
- 0x03e0 (0992) H     3404 FreqTablePixclk                 : 1076
- 0x03e2 (0994) H     0e01 FreqTablePhyclk                 : 270
- 0x03e4 (0996) H     1c02 FreqTablePhyclk                 : 540
- 0x03e6 (0998) H     2a03 FreqTablePhyclk                 : 810
- 0x03e8 (1000) H     0000 FreqTablePhyclk                 : 0
- 0x03ea (1002) H     0000 FreqTablePhyclk                 : 0
- 0x03ec (1004) H     0000 FreqTablePhyclk                 : 0
- 0x03ee (1006) H     0000 FreqTablePhyclk                 : 0
- 0x03f0 (1008) H     0000 FreqTablePhyclk                 : 0
- 0x03f2 (1010) H     0907 DcModeMaxFreq                   : 1801
- 0x03f4 (1012) H     6e04 DcModeMaxFreq                   : 1134
- 0x03f6 (1014) H     cc03 DcModeMaxFreq                   : 972
- 0x03f8 (1016) H     cc03 DcModeMaxFreq                   : 972
- 0x03fa (1018) H     cc03 DcModeMaxFreq                   : 972
- 0x03fc (1020) H     e803 DcModeMaxFreq                   : 1000
- 0x03fe (1022) H     6e04 DcModeMaxFreq                   : 1134
- 0x0400 (1024) H     6e04 DcModeMaxFreq                   : 1134
- 0x0402 (1026) H     3404 DcModeMaxFreq                   : 1076
- 0x0404 (1028) H     2a03 DcModeMaxFreq                   : 810
- 0x0406 (1030) H     c904 DcModeMaxFreq                   : 1225
- 0x0408 (1032) H     0000 Padding8_Clks                   : 0
- 0x040a (1034) H     c800 Mp0clkFreq                      : 200
- 0x040c (1036) H     2c01 Mp0clkFreq                      : 300
- 0x040e (1038) H     6009 Mp0DpmVoltage                   : 2400
- 0x0410 (1040) H     f00a Mp0DpmVoltage                   : 2800
- 0x0412 (1042) H     2803 GfxclkFidle                     : 808
- 0x0414 (1044) H     0000 GfxclkSlewRate                  : 0
- 0x0416 (1046) H     0000 CksEnableFreq                   : 0
- 0x0418 (1048) H     0000 Padding789                      : 0
- 0x041a (1050) f 00000000 a                               : 0
- 0x041e (1054) f 00000000 b                               : 0
- 0x0422 (1058) f 00000000 c                               : 0
- 0x0426 (1062) B       00 Padding567                      : 0
- 0x0427 (1063) B       00 Padding567                      : 0
- 0x0428 (1064) B       00 Padding567                      : 0
- 0x0429 (1065) B       00 Padding567                      : 0
- 0x042a (1066) H     0907 GfxclkDsMaxFreq                 : 1801
- 0x042c (1068) B       01 GfxclkSource                    : 1
- 0x042d (1069) B       00 Padding456                      : 0
- 0x042e (1070) B       00 LowestUclkReservedForUlv        : 0
- 0x042f (1071) B       00 Padding8_Uclk                   : 0
- 0x0430 (1072) B       00 Padding8_Uclk                   : 0
- 0x0431 (1073) B       00 Padding8_Uclk                   : 0
- 0x0432 (1074) B       00 PcieGenSpeed                    : 0
- 0x0433 (1075) B       02 PcieGenSpeed                    : 2
- 0x0434 (1076) B       06 PcieLaneCount                   : 6
- 0x0435 (1077) B       06 PcieLaneCount                   : 6
- 0x0436 (1078) H     5000 LclkFreq                        : 80
- 0x0438 (1080) H     3401 LclkFreq                        : 308
- 0x043a (1082) H     0000 EnableTdpm                      : 0
- 0x043c (1084) H     0000 TdpmHighHystTemperature         : 0
- 0x043e (1086) H     0000 TdpmLowHystTemperature          : 0
- 0x0440 (1088) H     0000 GfxclkFreqHighTempLimit         : 0
- 0x0442 (1090) H     0000 FanStopTemp                     : 0
- 0x0444 (1092) H     0000 FanStartTemp                    : 0
- 0x0446 (1094) H     9001 FanGainEdge                     : 400
- 0x0448 (1096) H     9001 FanGainHotspot                  : 400
- 0x044a (1098) H     9001 FanGainLiquid                   : 400
- 0x044c (1100) H     9001 FanGainVrGfx                    : 400
- 0x044e (1102) H     9001 FanGainVrSoc                    : 400
- 0x0450 (1104) H     9001 FanGainPlx                      : 400
- 0x0452 (1106) H     9001 FanGainHbm                      : 400
- 0x0454 (1108) H     1400 FanPwmMin                       : 20
- 0x0456 (1110) H     540b FanAcousticLimitRpm             : 2900
- 0x0458 (1112) H     540b FanThrottlingRpm                : 2900
- 0x045a (1114) H     0a0f FanMaximumRpm                   : 3850
- 0x045c (1116) H     5f00 FanTargetTemperature            : 95
- 0x045e (1118) H     0000 FanTargetGfxclk                 : 0
- 0x0460 (1120) B       00 FanZeroRpmEnable                : 0
- 0x0461 (1121) B       02 FanTachEdgePerRev               : 2
- 0x0462 (1122) h     0000 FuzzyFan_ErrorSetDelta          : 0
- 0x0464 (1124) h     0000 FuzzyFan_ErrorRateSetDelta      : 0
- 0x0466 (1126) h     0000 FuzzyFan_PwmSetDelta            : 0
- 0x0468 (1128) H     0000 FuzzyFan_Reserved               : 0
- 0x046a (1130) B       00 OverrideAvfsGb                  : 0
- 0x046b (1131) B       01 OverrideAvfsGb                  : 1
- 0x046c (1132) B       00 Padding8_Avfs                   : 0
- 0x046d (1133) B       00 Padding8_Avfs                   : 0
- 0x046e (1134) f 00000000 a                               : 0
- 0x0472 (1138) f 508d973c b                               : 0.0185
- 0x0476 (1142) f 0ad7a33b c                               : 0.005
- 0x047a (1146) f 00000000 a                               : 0
- 0x047e (1150) f eab2983c b                               : 0.01864
- 0x0482 (1154) f 87a2403d c                               : 0.04703
- 0x0486 (1158) f 00000000 a                               : 0
- 0x048a (1162) f 00000000 b                               : 0
- 0x048e (1166) f 00000000 c                               : 0
- 0x0492 (1170) f 00000000 a                               : 0
- 0x0496 (1174) f 00000000 b                               : 0
- 0x049a (1178) f 00000000 c                               : 0
- 0x049e (1182) f 00000000 a                               : 0
- 0x04a2 (1186) f 00000000 b                               : 0
- 0x04a6 (1190) f 00000000 c                               : 0
- 0x04aa (1194) f 00000000 a                               : 0
- 0x04ae (1198) f 00000000 b                               : 0
- 0x04b2 (1202) f 00000000 c                               : 0
- 0x04b6 (1206) f 00000000 m                               : 0
- 0x04ba (1210) f 00000000 b                               : 0
- 0x04be (1214) f 00000000 m                               : 0
- 0x04c2 (1218) f 00000000 b                               : 0
- 0x04c6 (1222) f 00000000 a                               : 0
- 0x04ca (1226) f 00000000 b                               : 0
- 0x04ce (1230) f 00000000 c                               : 0
- 0x04d2 (1234) f 00000000 a                               : 0
- 0x04d6 (1238) f 00000000 b                               : 0
- 0x04da (1242) f 00000000 c                               : 0
- 0x04de (1246) H     0000 DcTol                           : 0
- 0x04e0 (1248) H     a000 DcTol                           : 160
- 0x04e2 (1250) B       01 DcBtcEnabled                    : 1
- 0x04e3 (1251) B       00 DcBtcEnabled                    : 0
- 0x04e4 (1252) B       00 Padding8_GfxBtc                 : 0
- 0x04e5 (1253) B       00 Padding8_GfxBtc                 : 0
- 0x04e6 (1254) h     0000 DcBtcMin                        : 0
- 0x04e8 (1256) h     0000 DcBtcMin                        : 0
- 0x04ea (1258) H     a000 DcBtcMax                        : 160
- 0x04ec (1260) H     0000 DcBtcMax                        : 0
- 0x04ee (1262) B       08 XgmiLinkSpeed                   : 8
- 0x04ef (1263) B       10 XgmiLinkSpeed                   : 16
- 0x04f0 (1264) B       02 XgmiLinkWidth                   : 2
- 0x04f1 (1265) B       10 XgmiLinkWidth                   : 16
- 0x04f2 (1266) H     1a04 XgmiFclkFreq                    : 1050
- 0x04f4 (1268) H     4c04 XgmiFclkFreq                    : 1100
- 0x04f6 (1270) H     e803 XgmiUclkFreq                    : 1000
- 0x04f8 (1272) H     e803 XgmiUclkFreq                    : 1000
- 0x04fa (1274) H     e803 XgmiSocclkFreq                  : 1000
- 0x04fc (1276) H     e803 XgmiSocclkFreq                  : 1000
- 0x04fe (1278) H     0000 XgmiSocVoltage                  : 0
- 0x0500 (1280) H     0000 XgmiSocVoltage                  : 0
- 0x0502 (1282) I 00000000 DebugOverrides                  : 0
- 0x0506 (1286) f 00000000 a                               : 0
- 0x050a (1290) f 00000000 b                               : 0
- 0x050e (1294) f 00000000 c                               : 0
- 0x0512 (1298) f 00000000 a                               : 0
- 0x0516 (1302) f 00000000 b                               : 0
- 0x051a (1306) f 00000000 c                               : 0
- 0x051e (1310) f 00000000 a                               : 0
- 0x0522 (1314) f 00000000 b                               : 0
- 0x0526 (1318) f 00000000 c                               : 0
- 0x052a (1322) f 00000000 a                               : 0
- 0x052e (1326) f 00000000 b                               : 0
- 0x0532 (1330) f 00000000 c                               : 0
- 0x0536 (1334) H     860b MinVoltageUlvGfx                : 2950
- 0x0538 (1336) H     220b MinVoltageUlvSoc                : 2850
- 0x053a (1338) H     540b MGpuFanBoostLimitRpm            : 2900
- 0x053c (1340) H     0000 Fan                             : 0
- 0x053e (1342) H     9001 FanGainVrMem0                   : 400
- 0x0540 (1344) H     9001 FanGainVrMem1                   : 400
- 0x0542 (1346) H     3800 DcBtcGb                         : 56
- 0x0544 (1348) H     0000 DcBtcGb                         : 0
- 0x0546 (1350) I 00000000 Reserved                        : 0
- 0x054a (1354) I 00000000 Reserved                        : 0
- 0x054e (1358) I 00000000 Reserved                        : 0
- 0x0552 (1362) I 00000000 Reserved                        : 0
- 0x0556 (1366) I 00000000 Reserved                        : 0
- 0x055a (1370) I 00000000 Reserved                        : 0
- 0x055e (1374) I 00000000 Reserved                        : 0
- 0x0562 (1378) I 00000000 Reserved                        : 0
- 0x0566 (1382) I 00000000 Reserved                        : 0
- 0x056a (1386) I 00000000 Reserved                        : 0
- 0x056e (1390) I 00000000 Reserved                        : 0
- 0x0572 (1394) I 00000000 Padding32                       : 0
- 0x0576 (1398) I 00000000 Padding32                       : 0
- 0x057a (1402) I 00000000 Padding32                       : 0
- 0x057e (1406) H     0000 MaxVoltageStepGfx               : 0
- 0x0580 (1408) H     0000 MaxVoltageStepSoc               : 0
- 0x0582 (1410) B       00 VddGfxVrMapping                 : 0
- 0x0583 (1411) B       00 VddSocVrMapping                 : 0
- 0x0584 (1412) B       00 VddMem0VrMapping                : 0
- 0x0585 (1413) B       00 VddMem1VrMapping                : 0
- 0x0586 (1414) B       00 GfxUlvPhaseSheddingMask         : 0
- 0x0587 (1415) B       00 SocUlvPhaseSheddingMask         : 0
- 0x0588 (1416) B       00 ExternalSensorPresent           : 0
- 0x0589 (1417) B       00 Padding8_V                      : 0
- 0x058a (1418) H     0000 GfxMaxCurrent                   : 0
- 0x058c (1420) b       00 GfxOffset                       : 0
- 0x058d (1421) B       00 Padding_TelemetryGfx            : 0
- 0x058e (1422) H     0000 SocMaxCurrent                   : 0
- 0x0590 (1424) b       00 SocOffset                       : 0
- 0x0591 (1425) B       00 Padding_TelemetrySoc            : 0
- 0x0592 (1426) H     0000 Mem0MaxCurrent                  : 0
- 0x0594 (1428) b       00 Mem0Offset                      : 0
- 0x0595 (1429) B       00 Padding_TelemetryMem0           : 0
- 0x0596 (1430) H     0000 Mem1MaxCurrent                  : 0
- 0x0598 (1432) b       00 Mem1Offset                      : 0
- 0x0599 (1433) B       00 Padding_TelemetryMem1           : 0
- 0x059a (1434) B       00 AcDcGpio                        : 0
- 0x059b (1435) B       00 AcDcPolarity                    : 0
- 0x059c (1436) B       00 VR0HotGpio                      : 0
- 0x059d (1437) B       00 VR0HotPolarity                  : 0
- 0x059e (1438) B       00 VR1HotGpio                      : 0
- 0x059f (1439) B       00 VR1HotPolarity                  : 0
- 0x05a0 (1440) B       00 Padding1                        : 0
- 0x05a1 (1441) B       00 Padding2                        : 0
- 0x05a2 (1442) B       00 LedPin0                         : 0
- 0x05a3 (1443) B       00 LedPin1                         : 0
- 0x05a4 (1444) B       00 LedPin2                         : 0
- 0x05a5 (1445) B       00 padding8_4                      : 0
- 0x05a6 (1446) B       00 PllGfxclkSpreadEnabled          : 0
- 0x05a7 (1447) B       00 PllGfxclkSpreadPercent          : 0
- 0x05a8 (1448) H     0000 PllGfxclkSpreadFreq             : 0
- 0x05aa (1450) B       00 UclkSpreadEnabled               : 0
- 0x05ab (1451) B       00 UclkSpreadPercent               : 0
- 0x05ac (1452) H     0000 UclkSpreadFreq                  : 0
- 0x05ae (1454) B       00 FclkSpreadEnabled               : 0
- 0x05af (1455) B       00 FclkSpreadPercent               : 0
- 0x05b0 (1456) H     0000 FclkSpreadFreq                  : 0
- 0x05b2 (1458) B       00 FllGfxclkSpreadEnabled          : 0
- 0x05b3 (1459) B       00 FllGfxclkSpreadPercent          : 0
- 0x05b4 (1460) H     0000 FllGfxclkSpreadFreq             : 0
- 0x05b6 (1462) I 00000000 Enabled                         : 0
- 0x05ba (1466) I 00000000 SlaveAddress                    : 0
- 0x05be (1470) I 00000000 ControllerPort                  : 0
- 0x05c2 (1474) I 00000000 ControllerName                  : 0
- 0x05c6 (1478) I 00000000 ThermalThrottler                : 0
- 0x05ca (1482) I 00000000 I2cProtocol                     : 0
- 0x05ce (1486) I 00000000 I2cSpeed                        : 0
- 0x05d2 (1490) I 00000000 Enabled                         : 0
- 0x05d6 (1494) I 00000000 SlaveAddress                    : 0
- 0x05da (1498) I 00000000 ControllerPort                  : 0
- 0x05de (1502) I 00000000 ControllerName                  : 0
- 0x05e2 (1506) I 00000000 ThermalThrottler                : 0
- 0x05e6 (1510) I 00000000 I2cProtocol                     : 0
- 0x05ea (1514) I 00000000 I2cSpeed                        : 0
- 0x05ee (1518) I 00000000 Enabled                         : 0
- 0x05f2 (1522) I 00000000 SlaveAddress                    : 0
- 0x05f6 (1526) I 00000000 ControllerPort                  : 0
- 0x05fa (1530) I 00000000 ControllerName                  : 0
- 0x05fe (1534) I 00000000 ThermalThrottler                : 0
- 0x0602 (1538) I 00000000 I2cProtocol                     : 0
- 0x0606 (1542) I 00000000 I2cSpeed                        : 0
- 0x060a (1546) I 00000000 Enabled                         : 0
- 0x060e (1550) I 00000000 SlaveAddress                    : 0
- 0x0612 (1554) I 00000000 ControllerPort                  : 0
- 0x0616 (1558) I 00000000 ControllerName                  : 0
- 0x061a (1562) I 00000000 ThermalThrottler                : 0
- 0x061e (1566) I 00000000 I2cProtocol                     : 0
- 0x0622 (1570) I 00000000 I2cSpeed                        : 0
- 0x0626 (1574) I 00000000 Enabled                         : 0
- 0x062a (1578) I 00000000 SlaveAddress                    : 0
- 0x062e (1582) I 00000000 ControllerPort                  : 0
- 0x0632 (1586) I 00000000 ControllerName                  : 0
- 0x0636 (1590) I 00000000 ThermalThrottler                : 0
- 0x063a (1594) I 00000000 I2cProtocol                     : 0
- 0x063e (1598) I 00000000 I2cSpeed                        : 0
- 0x0642 (1602) I 00000000 Enabled                         : 0
- 0x0646 (1606) I 00000000 SlaveAddress                    : 0
- 0x064a (1610) I 00000000 ControllerPort                  : 0
- 0x064e (1614) I 00000000 ControllerName                  : 0
- 0x0652 (1618) I 00000000 ThermalThrottler                : 0
- 0x0656 (1622) I 00000000 I2cProtocol                     : 0
- 0x065a (1626) I 00000000 I2cSpeed                        : 0
- 0x065e (1630) I 00000000 Enabled                         : 0
- 0x0662 (1634) I 00000000 SlaveAddress                    : 0
- 0x0666 (1638) I 00000000 ControllerPort                  : 0
- 0x066a (1642) I 00000000 ControllerName                  : 0
- 0x066e (1646) I 00000000 ThermalThrottler                : 0
- 0x0672 (1650) I 00000000 I2cProtocol                     : 0
- 0x0676 (1654) I 00000000 I2cSpeed                        : 0
- 0x067a (1658) I 00000000 BoardReserved                   : 0
- 0x067e (1662) I 00000000 BoardReserved                   : 0
- 0x0682 (1666) I 00000000 BoardReserved                   : 0
- 0x0686 (1670) I 00000000 BoardReserved                   : 0
- 0x068a (1674) I 00000000 BoardReserved                   : 0
- 0x068e (1678) I 00000000 BoardReserved                   : 0
- 0x0692 (1682) I 00000000 BoardReserved                   : 0
- 0x0696 (1686) I 00000000 BoardReserved                   : 0
- 0x069a (1690) I 00000000 BoardReserved                   : 0
- 0x069e (1694) I 00000000 BoardReserved                   : 0
- 0x06a2 (1698) I 00000000 MmHubPadding                    : 0
- 0x06a6 (1702) I 00000000 MmHubPadding                    : 0
- 0x06aa (1706) I 00000000 MmHubPadding                    : 0
- 0x06ae (1710) I 00000000 MmHubPadding                    : 0
- 0x06b2 (1714) I 00000000 MmHubPadding                    : 0
- 0x06b6 (1718) I 00000000 MmHubPadding                    : 0
- 0x06ba (1722) I 00000000 MmHubPadding                    : 0
- 0x06be (1726) I 00000000 MmHubPadding                    : 0
+PowerPlay table rev 12.0 size 1674 bytes
+ Offset (dec.) t Raw val. Variable name                         Decoded value
+------------------------------------------------------------------------------
+ 0x0000 (0000) H     8a06 structuresize                             : 1674
+ 0x0002 (0002) B       0c format_revision                           : 12
+ 0x0003 (0003) B       00 content_revision                          : 0
+ 0x0004 (0004) B       01 table_revision                            : 1
+ 0x0005 (0005) H     e201 table_size                                : 482
+ 0x0007 (0007) I c7080000 golden_pp_id                              : 2247
+ 0x000b (0011) I 20380000 golden_revision                           : 14368
+ 0x000f (0015) H     7d00 format_id                                 : 125
+ 0x0011 (0017) I 08000000 platform_caps                             : 8
+ 0x0015 (0021) B       1b thermal_controller_type                   : 27
+ 0x0016 (0022) H     0000 small_power_limit1                        : 0
+ 0x0018 (0024) H     0000 small_power_limit2                        : 0
+ 0x001a (0026) H     0000 boost_power_limit                         : 0
+ 0x001c (0028) H     0000 od_turbo_power_limit                      : 0
+ 0x001e (0030) H     0000 od_power_save_power_limit                 : 0
+ 0x0020 (0032) H     7600 software_shutdown_temp                    : 118
+ 0x0022 (0034) H     0000 reserve                                   : 0
+ 0x0024 (0036) H     0000 reserve                                   : 0
+ 0x0026 (0038) H     0000 reserve                                   : 0
+ 0x0028 (0040) H     0000 reserve                                   : 0
+ 0x002a (0042) H     0000 reserve                                   : 0
+ 0x002c (0044) H     0000 reserve                                   : 0
+ 0x002e (0046) B       01 revision                                  : 1
+ 0x002f (0047) B       00 reserve                                   : 0
+ 0x0030 (0048) B       00 reserve                                   : 0
+ 0x0031 (0049) B       00 reserve                                   : 0
+ 0x0032 (0050) I 0a000000 count                                     : 10
+ 0x0036 (0054) I 34080000 max GFXCLK                                : 2100
+ 0x003a (0058) I f3040000 max VCLK                                  : 1267
+ 0x003e (0062) I 3e040000 max DCLK                                  : 1086
+ 0x0042 (0066) I f3040000 max ECLK                                  : 1267
+ 0x0046 (0070) I f3040000 max SOCCLK                                : 1267
+ 0x004a (0074) I 6b030000 max UCLK                                  : 875
+ 0x004e (0078) I f3040000 max DCEFCLK                               : 1267
+ 0x0052 (0082) I 04050000 max DISPCLK                               : 1284
+ 0x0056 (0086) I 04050000 max PIXCLK                                : 1284
+ 0x005a (0090) I 2a030000 max PHYCLK                                : 810
+ 0x005e (0094) I 00000000 max                                       : 0
+ 0x0062 (0098) I 00000000 max                                       : 0
+ 0x0066 (0102) I 00000000 max                                       : 0
+ 0x006a (0106) I 00000000 max                                       : 0
+ 0x006e (0110) I 00000000 max                                       : 0
+ 0x0072 (0114) I 00000000 max                                       : 0
+ 0x0076 (0118) I 2c010000 min GFXCLK                                : 300
+ 0x007a (0122) I 64000000 min VCLK                                  : 100
+ 0x007e (0126) I 64000000 min DCLK                                  : 100
+ 0x0082 (0130) I 64000000 min ECLK                                  : 100
+ 0x0086 (0134) I fb010000 min SOCCLK                                : 507
+ 0x008a (0138) I 64000000 min UCLK                                  : 100
+ 0x008e (0142) I fb010000 min DCEFCLK                               : 507
+ 0x0092 (0146) I 34010000 min DISPCLK                               : 308
+ 0x0096 (0150) I 2c010000 min PIXCLK                                : 300
+ 0x009a (0154) I 2c010000 min PHYCLK                                : 300
+ 0x009e (0158) I 00000000 min                                       : 0
+ 0x00a2 (0162) I 00000000 min                                       : 0
+ 0x00a6 (0166) I 00000000 min                                       : 0
+ 0x00aa (0170) I 00000000 min                                       : 0
+ 0x00ae (0174) I 00000000 min                                       : 0
+ 0x00b2 (0178) I 00000000 min                                       : 0
+ 0x00b6 (0182) B       80 revision                                  : 128
+ 0x00b7 (0183) B       00 reserve                                   : 0
+ 0x00b8 (0184) B       00 reserve                                   : 0
+ 0x00b9 (0185) B       00 reserve                                   : 0
+ 0x00ba (0186) I 0e000000 feature_count                             : 14
+ 0x00be (0190) I 1e000000 setting_count                             : 30
+ 0x00c2 (0194) B       01 cap GFXCLK_LIMITS                         : 1
+ 0x00c3 (0195) B       01 cap GFXCLK_CURVE                          : 1
+ 0x00c4 (0196) B       01 cap UCLK_MAX                              : 1
+ 0x00c5 (0197) B       01 cap POWER_LIMIT                           : 1
+ 0x00c6 (0198) B       01 cap FAN_ACOUSTIC_LIMIT                    : 1
+ 0x00c7 (0199) B       01 cap FAN_SPEED_MIN                         : 1
+ 0x00c8 (0200) B       01 cap TEMPERATURE_FAN                       : 1
+ 0x00c9 (0201) B       01 cap TEMPERATURE_SYSTEM                    : 1
+ 0x00ca (0202) B       01 cap MEMORY_TIMING_TUNE                    : 1
+ 0x00cb (0203) B       00 cap FAN_ZERO_RPM_CONTROL                  : 0
+ 0x00cc (0204) B       01 cap AUTO_UV_ENGINE                        : 1
+ 0x00cd (0205) B       01 cap AUTO_OC_ENGINE                        : 1
+ 0x00ce (0206) B       01 cap AUTO_OC_MEMORY                        : 1
+ 0x00cf (0207) B       01 cap FAN_CURVE                             : 1
+ 0x00d0 (0208) B       00 cap                                       : 0
+ 0x00d1 (0209) B       00 cap                                       : 0
+ 0x00d2 (0210) B       00 cap                                       : 0
+ 0x00d3 (0211) B       00 cap                                       : 0
+ 0x00d4 (0212) B       00 cap                                       : 0
+ 0x00d5 (0213) B       00 cap                                       : 0
+ 0x00d6 (0214) B       00 cap                                       : 0
+ 0x00d7 (0215) B       00 cap                                       : 0
+ 0x00d8 (0216) B       00 cap                                       : 0
+ 0x00d9 (0217) B       00 cap                                       : 0
+ 0x00da (0218) B       00 cap                                       : 0
+ 0x00db (0219) B       00 cap                                       : 0
+ 0x00dc (0220) B       00 cap                                       : 0
+ 0x00dd (0221) B       00 cap                                       : 0
+ 0x00de (0222) B       00 cap                                       : 0
+ 0x00df (0223) B       00 cap                                       : 0
+ 0x00e0 (0224) B       00 cap                                       : 0
+ 0x00e1 (0225) B       00 cap                                       : 0
+ 0x00e2 (0226) I 66080000 max GFXCLKFMAX                            : 2150
+ 0x00e6 (0230) I 66080000 max GFXCLKFMIN                            : 2150
+ 0x00ea (0234) I 66080000 max VDDGFXCURVEFREQ_P1                    : 2150
+ 0x00ee (0238) I b0040000 max VDDGFXCURVEVOLTAGE_P1                 : 1200
+ 0x00f2 (0242) I 66080000 max VDDGFXCURVEFREQ_P2                    : 2150
+ 0x00f6 (0246) I b0040000 max VDDGFXCURVEVOLTAGE_P2                 : 1200
+ 0x00fa (0250) I 66080000 max VDDGFXCURVEFREQ_P3                    : 2150
+ 0x00fe (0254) I b0040000 max VDDGFXCURVEVOLTAGE_P3                 : 1200
+ 0x0102 (0258) I b6030000 max UCLKFMAX                              : 950
+ 0x0106 (0262) I 32000000 max POWERPERCENTAGE                       : 50
+ 0x010a (0266) I 56130000 max FANRPMMIN                             : 4950
+ 0x010e (0270) I 56130000 max FANRPMACOUSTICLIMIT                   : 4950
+ 0x0112 (0274) I 64000000 max FANTARGETTEMPERATURE                  : 100
+ 0x0116 (0278) I 6e000000 max OPERATINGTEMPMAX                      : 110
+ 0x011a (0282) I 02000000 max ACTIMING                              : 2
+ 0x011e (0286) I 00000000 max FAN_ZERO_RPM_CONTROL                  : 0
+ 0x0122 (0290) I 01000000 max AUTOUVENGINE                          : 1
+ 0x0126 (0294) I 01000000 max AUTOOCENGINE                          : 1
+ 0x012a (0298) I 01000000 max AUTOOCMEMORY                          : 1
+ 0x012e (0302) I 64000000 max                                       : 100
+ 0x0132 (0306) I 64000000 max                                       : 100
+ 0x0136 (0310) I 64000000 max                                       : 100
+ 0x013a (0314) I 64000000 max                                       : 100
+ 0x013e (0318) I 64000000 max                                       : 100
+ 0x0142 (0322) I 64000000 max                                       : 100
+ 0x0146 (0326) I 64000000 max                                       : 100
+ 0x014a (0330) I 64000000 max                                       : 100
+ 0x014e (0334) I 64000000 max                                       : 100
+ 0x0152 (0338) I 64000000 max                                       : 100
+ 0x0156 (0342) I 00000000 max                                       : 0
+ 0x015a (0346) I 00000000 max                                       : 0
+ 0x015e (0350) I 00000000 max                                       : 0
+ 0x0162 (0354) I 20030000 min GFXCLKFMAX                            : 800
+ 0x0166 (0358) I 20030000 min GFXCLKFMIN                            : 800
+ 0x016a (0362) I 20030000 min VDDGFXCURVEFREQ_P1                    : 800
+ 0x016e (0366) I ee020000 min VDDGFXCURVEVOLTAGE_P1                 : 750
+ 0x0172 (0370) I 20030000 min VDDGFXCURVEFREQ_P2                    : 800
+ 0x0176 (0374) I ee020000 min VDDGFXCURVEVOLTAGE_P2                 : 750
+ 0x017a (0378) I 20030000 min VDDGFXCURVEFREQ_P3                    : 800
+ 0x017e (0382) I ee020000 min VDDGFXCURVEVOLTAGE_P3                 : 750
+ 0x0182 (0386) I 71020000 min UCLKFMAX                              : 625
+ 0x0186 (0390) I 32000000 min POWERPERCENTAGE                       : 50
+ 0x018a (0394) I 4c040000 min FANRPMMIN                             : 1100
+ 0x018e (0398) I 4c040000 min FANRPMACOUSTICLIMIT                   : 1100
+ 0x0192 (0402) I 19000000 min FANTARGETTEMPERATURE                  : 25
+ 0x0196 (0406) I 32000000 min OPERATINGTEMPMAX                      : 50
+ 0x019a (0410) I 00000000 min ACTIMING                              : 0
+ 0x019e (0414) I 00000000 min FAN_ZERO_RPM_CONTROL                  : 0
+ 0x01a2 (0418) I 00000000 min AUTOUVENGINE                          : 0
+ 0x01a6 (0422) I 00000000 min AUTOOCENGINE                          : 0
+ 0x01aa (0426) I 00000000 min AUTOOCMEMORY                          : 0
+ 0x01ae (0430) I 19000000 min                                       : 25
+ 0x01b2 (0434) I 0a000000 min                                       : 10
+ 0x01b6 (0438) I 19000000 min                                       : 25
+ 0x01ba (0442) I 0a000000 min                                       : 10
+ 0x01be (0446) I 19000000 min                                       : 25
+ 0x01c2 (0450) I 0a000000 min                                       : 10
+ 0x01c6 (0454) I 19000000 min                                       : 25
+ 0x01ca (0458) I 0a000000 min                                       : 10
+ 0x01ce (0462) I 19000000 min                                       : 25
+ 0x01d2 (0466) I 0a000000 min                                       : 10
+ 0x01d6 (0470) I 00000000 min                                       : 0
+ 0x01da (0474) I 00000000 min                                       : 0
+ 0x01de (0478) I 00000000 min                                       : 0
+ 0x01e2 (0482) I 08000000 Version                                   : 8
+ 0x01e6 (0486) I ffafdfb3 FeaturesToRun                             : 3017781247
+ 0x01ea (0490) I 23060000 FeaturesToRun                             : 1571
+ 0x01ee (0494) H     b400 SocketPowerLimitAc                        : 180
+ 0x01f0 (0496) H     0000 SocketPowerLimitAc                        : 0
+ 0x01f2 (0498) H     0000 SocketPowerLimitAc                        : 0
+ 0x01f4 (0500) H     0000 SocketPowerLimitAc                        : 0
+ 0x01f6 (0502) H     0000 SocketPowerLimitAcTau                     : 0
+ 0x01f8 (0504) H     0000 SocketPowerLimitAcTau                     : 0
+ 0x01fa (0506) H     0000 SocketPowerLimitAcTau                     : 0
+ 0x01fc (0508) H     0000 SocketPowerLimitAcTau                     : 0
+ 0x01fe (0510) H     b400 SocketPowerLimitDc                        : 180
+ 0x0200 (0512) H     0000 SocketPowerLimitDc                        : 0
+ 0x0202 (0514) H     0000 SocketPowerLimitDc                        : 0
+ 0x0204 (0516) H     0000 SocketPowerLimitDc                        : 0
+ 0x0206 (0518) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x0208 (0520) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x020a (0522) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x020c (0524) H     0000 SocketPowerLimitDcTau                     : 0
+ 0x020e (0526) H     0e00 TdcLimitSoc                               : 14
+ 0x0210 (0528) H     0000 TdcLimitSocTau                            : 0
+ 0x0212 (0530) H     aa00 TdcLimitGfx                               : 170
+ 0x0214 (0532) H     0000 TdcLimitGfxTau                            : 0
+ 0x0216 (0534) H     6400 TedgeLimit                                : 100
+ 0x0218 (0536) H     6e00 ThotspotLimit                             : 110
+ 0x021a (0538) H     6900 TmemLimit                                 : 105
+ 0x021c (0540) H     7300 Tvr_gfxLimit                              : 115
+ 0x021e (0542) H     7300 Tvr_mem0Limit                             : 115
+ 0x0220 (0544) H     7300 Tvr_mem1Limit                             : 115
+ 0x0222 (0546) H     7300 Tvr_socLimit                              : 115
+ 0x0224 (0548) H     0000 Tliquid0Limit                             : 0
+ 0x0226 (0550) H     0000 Tliquid1Limit                             : 0
+ 0x0228 (0552) H     0000 TplxLimit                                 : 0
+ 0x022a (0554) I 00000000 FitLimit                                  : 0
+ 0x022e (0558) H     0000 PpmPowerLimit                             : 0
+ 0x0230 (0560) H     0000 PpmTemperatureThreshold                   : 0
+ 0x0232 (0562) I fe700000 ThrottlerControlMask                      : 28926
+ 0x0236 (0566) I 01000000 FwDStateMask                              : 1
+ 0x023a (0570) H     6400 UlvVoltageOffsetSoc                       : 100
+ 0x023c (0572) H     6400 UlvVoltageOffsetGfx                       : 100
+ 0x023e (0574) B       00 GceaLinkMgrIdleThreshold                  : 0
+ 0x023f (0575) B       00 RlcUlvParams                              : 0
+ 0x0240 (0576) B       00 RlcUlvParams                              : 0
+ 0x0241 (0577) B       00 RlcUlvParams                              : 0
+ 0x0242 (0578) B       00 UlvSmnclkDid                              : 0
+ 0x0243 (0579) B       00 UlvMp1clkDid                              : 0
+ 0x0244 (0580) B       00 UlvGfxclkBypass                           : 0
+ 0x0245 (0581) B       00 Padding234                                : 0
+ 0x0246 (0582) H     540b MinVoltageUlvGfx                          : 2900
+ 0x0248 (0584) H     540b MinVoltageUlvSoc                          : 2900
+ 0x024a (0586) H     b80b MinVoltageGfx                             : 3000
+ 0x024c (0588) H     b80b MinVoltageSoc                             : 3000
+ 0x024e (0590) H     c012 MaxVoltageGfx                             : 4800
+ 0x0250 (0592) H     c012 MaxVoltageSoc                             : 4800
+ 0x0252 (0594) H     4c00 LoadLineResistanceGfx                     : 76
+ 0x0254 (0596) H     0000 LoadLineResistanceSoc                     : 0
+ 0x0256 (0598) B       01 VoltageMode                               : 1
+ 0x0257 (0599) B       00 SnapToDiscrete                            : 0
+ 0x0258 (0600) B       02 NumDiscreteLevels                         : 2
+ 0x0259 (0601) B       00 Padding                                   : 0
+ 0x025a (0602) f 00000000 m                                         : 0
+ 0x025e (0606) f 00000000 b                                         : 0
+ 0x0262 (0610) f 8126823e a                                         : 0.2542
+ 0x0266 (0614) f a4705dbe b                                         :-0.21625
+ 0x026a (0618) f b51a323f c                                         : 0.69572
+ 0x026e (0622) B       01 VoltageMode                               : 1
+ 0x026f (0623) B       00 SnapToDiscrete                            : 0
+ 0x0270 (0624) B       02 NumDiscreteLevels                         : 2
+ 0x0271 (0625) B       00 Padding                                   : 0
+ 0x0272 (0626) f 0000803f m                                         : 1
+ 0x0276 (0630) f 00000000 b                                         : 0
+ 0x027a (0634) f f1ba5e3e a                                         : 0.21751
+ 0x027e (0638) f abb26fbd b                                         :-0.05852
+ 0x0282 (0642) f 45f5363f c                                         : 0.71468
+ 0x0286 (0646) B       01 VoltageMode                               : 1
+ 0x0287 (0647) B       01 SnapToDiscrete                            : 1
+ 0x0288 (0648) B       04 NumDiscreteLevels                         : 4
+ 0x0289 (0649) B       00 Padding                                   : 0
+ 0x028a (0650) f 0000803f m                                         : 1
+ 0x028e (0654) f 00000000 b                                         : 0
+ 0x0292 (0658) f f1ba5e3e a                                         : 0.21751
+ 0x0296 (0662) f abb26fbd b                                         :-0.05852
+ 0x029a (0666) f 45f5363f c                                         : 0.71468
+ 0x029e (0670) B       01 VoltageMode                               : 1
+ 0x029f (0671) B       00 SnapToDiscrete                            : 0
+ 0x02a0 (0672) B       02 NumDiscreteLevels                         : 2
+ 0x02a1 (0673) B       00 Padding                                   : 0
+ 0x02a2 (0674) f d8f0243f m                                         : 0.6443
+ 0x02a6 (0678) f 35ef083f b                                         : 0.5349
+ 0x02aa (0682) f 00000000 a                                         : 0
+ 0x02ae (0686) f d42bc53e b                                         : 0.3851
+ 0x02b2 (0690) f 575b113f c                                         : 0.5678
+ 0x02b6 (0694) B       01 VoltageMode                               : 1
+ 0x02b7 (0695) B       00 SnapToDiscrete                            : 0
+ 0x02b8 (0696) B       02 NumDiscreteLevels                         : 2
+ 0x02b9 (0697) B       00 Padding                                   : 0
+ 0x02ba (0698) f 0a68023f m                                         : 0.5094
+ 0x02be (0702) f 14ae173f b                                         : 0.5925
+ 0x02c2 (0706) f 00000000 a                                         : 0
+ 0x02c6 (0710) f 8351a93e b                                         : 0.3307
+ 0x02ca (0714) f 3789113f c                                         : 0.5685
+ 0x02ce (0718) B       01 VoltageMode                               : 1
+ 0x02cf (0719) B       00 SnapToDiscrete                            : 0
+ 0x02d0 (0720) B       02 NumDiscreteLevels                         : 2
+ 0x02d1 (0721) B       00 Padding                                   : 0
+ 0x02d2 (0722) f 9cc4a03f m                                         : 1.256
+ 0x02d6 (0726) f 8e06b0be b                                         :-0.3438
+ 0x02da (0730) f 00000000 a                                         : 0
+ 0x02de (0734) f e3c7083f b                                         : 0.5343
+ 0x02e2 (0738) f ec2f7b3e c                                         : 0.2453
+ 0x02e6 (0742) B       01 VoltageMode                               : 1
+ 0x02e7 (0743) B       00 SnapToDiscrete                            : 0
+ 0x02e8 (0744) B       02 NumDiscreteLevels                         : 2
+ 0x02e9 (0745) B       00 Padding                                   : 0
+ 0x02ea (0746) f 6154523f m                                         : 0.8216
+ 0x02ee (0750) f d7346f3c b                                         : 0.0146
+ 0x02f2 (0754) f 00000000 a                                         : 0
+ 0x02f6 (0758) f fd87f43e b                                         : 0.4776
+ 0x02fa (0762) f ca54813e c                                         : 0.2526
+ 0x02fe (0766) B       02 VoltageMode                               : 2
+ 0x02ff (0767) B       00 SnapToDiscrete                            : 0
+ 0x0300 (0768) B       02 NumDiscreteLevels                         : 2
+ 0x0301 (0769) B       00 Padding                                   : 0
+ 0x0302 (0770) f 00000000 m                                         : 0
+ 0x0306 (0774) f 00000000 b                                         : 0
+ 0x030a (0778) f 00000000 a                                         : 0
+ 0x030e (0782) f 00000000 b                                         : 0
+ 0x0312 (0786) f 00000000 c                                         : 0
+ 0x0316 (0790) B       02 VoltageMode                               : 2
+ 0x0317 (0791) B       00 SnapToDiscrete                            : 0
+ 0x0318 (0792) B       02 NumDiscreteLevels                         : 2
+ 0x0319 (0793) B       00 Padding                                   : 0
+ 0x031a (0794) f 00000000 m                                         : 0
+ 0x031e (0798) f 00000000 b                                         : 0
+ 0x0322 (0802) f 00000000 a                                         : 0
+ 0x0326 (0806) f 00000000 b                                         : 0
+ 0x032a (0810) f 00000000 c                                         : 0
+ 0x032e (0814) H     2c01 FreqTableGfx                              : 300
+ 0x0330 (0816) H     3408 FreqTableGfx                              : 2100
+ 0x0332 (0818) H     7805 FreqTableGfx                              : 1400
+ 0x0334 (0820) H     7805 FreqTableGfx                              : 1400
+ 0x0336 (0822) H     7805 FreqTableGfx                              : 1400
+ 0x0338 (0824) H     7805 FreqTableGfx                              : 1400
+ 0x033a (0826) H     7805 FreqTableGfx                              : 1400
+ 0x033c (0828) H     7805 FreqTableGfx                              : 1400
+ 0x033e (0830) H     7805 FreqTableGfx                              : 1400
+ 0x0340 (0832) H     7805 FreqTableGfx                              : 1400
+ 0x0342 (0834) H     7805 FreqTableGfx                              : 1400
+ 0x0344 (0836) H     7805 FreqTableGfx                              : 1400
+ 0x0346 (0838) H     7805 FreqTableGfx                              : 1400
+ 0x0348 (0840) H     7805 FreqTableGfx                              : 1400
+ 0x034a (0842) H     7805 FreqTableGfx                              : 1400
+ 0x034c (0844) H     7805 FreqTableGfx                              : 1400
+ 0x034e (0846) H     6400 FreqTableVclk                             : 100
+ 0x0350 (0848) H     f304 FreqTableVclk                             : 1267
+ 0x0352 (0850) H     f304 FreqTableVclk                             : 1267
+ 0x0354 (0852) H     f304 FreqTableVclk                             : 1267
+ 0x0356 (0854) H     f304 FreqTableVclk                             : 1267
+ 0x0358 (0856) H     f304 FreqTableVclk                             : 1267
+ 0x035a (0858) H     f304 FreqTableVclk                             : 1267
+ 0x035c (0860) H     f304 FreqTableVclk                             : 1267
+ 0x035e (0862) H     6400 FreqTableDclk                             : 100
+ 0x0360 (0864) H     3e04 FreqTableDclk                             : 1086
+ 0x0362 (0866) H     3e04 FreqTableDclk                             : 1086
+ 0x0364 (0868) H     3e04 FreqTableDclk                             : 1086
+ 0x0366 (0870) H     3e04 FreqTableDclk                             : 1086
+ 0x0368 (0872) H     3e04 FreqTableDclk                             : 1086
+ 0x036a (0874) H     3e04 FreqTableDclk                             : 1086
+ 0x036c (0876) H     3e04 FreqTableDclk                             : 1086
+ 0x036e (0878) H     fb01 FreqTableSocclk                           : 507
+ 0x0370 (0880) H     f304 FreqTableSocclk                           : 1267
+ 0x0372 (0882) H     b603 FreqTableSocclk                           : 950
+ 0x0374 (0884) H     b603 FreqTableSocclk                           : 950
+ 0x0376 (0886) H     b603 FreqTableSocclk                           : 950
+ 0x0378 (0888) H     b603 FreqTableSocclk                           : 950
+ 0x037a (0890) H     b603 FreqTableSocclk                           : 950
+ 0x037c (0892) H     b603 FreqTableSocclk                           : 950
+ 0x037e (0894) H     6400 FreqTableUclk                             : 100
+ 0x0380 (0896) H     f401 FreqTableUclk                             : 500
+ 0x0382 (0898) H     7102 FreqTableUclk                             : 625
+ 0x0384 (0900) H     6b03 FreqTableUclk                             : 875
+ 0x0386 (0902) H     fb01 FreqTableDcefclk                          : 507
+ 0x0388 (0904) H     f304 FreqTableDcefclk                          : 1267
+ 0x038a (0906) H     f304 FreqTableDcefclk                          : 1267
+ 0x038c (0908) H     f304 FreqTableDcefclk                          : 1267
+ 0x038e (0910) H     f304 FreqTableDcefclk                          : 1267
+ 0x0390 (0912) H     f304 FreqTableDcefclk                          : 1267
+ 0x0392 (0914) H     f304 FreqTableDcefclk                          : 1267
+ 0x0394 (0916) H     f304 FreqTableDcefclk                          : 1267
+ 0x0396 (0918) H     3401 FreqTableDispclk                          : 308
+ 0x0398 (0920) H     0405 FreqTableDispclk                          : 1284
+ 0x039a (0922) H     0405 FreqTableDispclk                          : 1284
+ 0x039c (0924) H     0405 FreqTableDispclk                          : 1284
+ 0x039e (0926) H     0405 FreqTableDispclk                          : 1284
+ 0x03a0 (0928) H     0405 FreqTableDispclk                          : 1284
+ 0x03a2 (0930) H     0405 FreqTableDispclk                          : 1284
+ 0x03a4 (0932) H     0405 FreqTableDispclk                          : 1284
+ 0x03a6 (0934) H     2c01 FreqTablePixclk                           : 300
+ 0x03a8 (0936) H     0405 FreqTablePixclk                           : 1284
+ 0x03aa (0938) H     a404 FreqTablePixclk                           : 1188
+ 0x03ac (0940) H     a404 FreqTablePixclk                           : 1188
+ 0x03ae (0942) H     a404 FreqTablePixclk                           : 1188
+ 0x03b0 (0944) H     a404 FreqTablePixclk                           : 1188
+ 0x03b2 (0946) H     a404 FreqTablePixclk                           : 1188
+ 0x03b4 (0948) H     a404 FreqTablePixclk                           : 1188
+ 0x03b6 (0950) H     2c01 FreqTablePhyclk                           : 300
+ 0x03b8 (0952) H     2a03 FreqTablePhyclk                           : 810
+ 0x03ba (0954) H     2a03 FreqTablePhyclk                           : 810
+ 0x03bc (0956) H     2a03 FreqTablePhyclk                           : 810
+ 0x03be (0958) H     2a03 FreqTablePhyclk                           : 810
+ 0x03c0 (0960) H     2a03 FreqTablePhyclk                           : 810
+ 0x03c2 (0962) H     2a03 FreqTablePhyclk                           : 810
+ 0x03c4 (0964) H     2a03 FreqTablePhyclk                           : 810
+ 0x03c6 (0966) I d001d001 Paddingclks                               : 30409168
+ 0x03ca (0970) I d001d001 Paddingclks                               : 30409168
+ 0x03ce (0974) I d001d001 Paddingclks                               : 30409168
+ 0x03d2 (0978) I d001d001 Paddingclks                               : 30409168
+ 0x03d6 (0982) I d001d001 Paddingclks                               : 30409168
+ 0x03da (0986) I d001d001 Paddingclks                               : 30409168
+ 0x03de (0990) I d001d001 Paddingclks                               : 30409168
+ 0x03e2 (0994) I d001d001 Paddingclks                               : 30409168
+ 0x03e6 (0998) I d001d001 Paddingclks                               : 30409168
+ 0x03ea (1002) I d001d001 Paddingclks                               : 30409168
+ 0x03ee (1006) I d001d001 Paddingclks                               : 30409168
+ 0x03f2 (1010) I d001d001 Paddingclks                               : 30409168
+ 0x03f6 (1014) I d001d001 Paddingclks                               : 30409168
+ 0x03fa (1018) I d001d001 Paddingclks                               : 30409168
+ 0x03fe (1022) I d001d001 Paddingclks                               : 30409168
+ 0x0402 (1026) I d001d001 Paddingclks                               : 30409168
+ 0x0406 (1030) H     3408 DcModeMaxFreq                             : 2100
+ 0x0408 (1032) H     f304 DcModeMaxFreq                             : 1267
+ 0x040a (1034) H     6b03 DcModeMaxFreq                             : 875
+ 0x040c (1036) H     3e04 DcModeMaxFreq                             : 1086
+ 0x040e (1038) H     f304 DcModeMaxFreq                             : 1267
+ 0x0410 (1040) H     f304 DcModeMaxFreq                             : 1267
+ 0x0412 (1042) H     0405 DcModeMaxFreq                             : 1284
+ 0x0414 (1044) H     0405 DcModeMaxFreq                             : 1284
+ 0x0416 (1046) H     2a03 DcModeMaxFreq                             : 810
+ 0x0418 (1048) H     d001 Padding8_Clks                             : 464
+ 0x041a (1050) B       00 FreqTableUclkDiv                          : 0
+ 0x041b (1051) B       03 FreqTableUclkDiv                          : 3
+ 0x041c (1052) B       03 FreqTableUclkDiv                          : 3
+ 0x041d (1053) B       03 FreqTableUclkDiv                          : 3
+ 0x041e (1054) H     3001 Mp0clkFreq                                : 304
+ 0x0420 (1056) H     fb01 Mp0clkFreq                                : 507
+ 0x0422 (1058) H     b80b Mp0DpmVoltage                             : 3000
+ 0x0424 (1060) H     b80b Mp0DpmVoltage                             : 3000
+ 0x0426 (1062) H     8c0a MemVddciVoltage                           : 2700
+ 0x0428 (1064) H     480d MemVddciVoltage                           : 3400
+ 0x042a (1066) H     480d MemVddciVoltage                           : 3400
+ 0x042c (1068) H     480d MemVddciVoltage                           : 3400
+ 0x042e (1070) H     8813 MemMvddVoltage                            : 5000
+ 0x0430 (1072) H     1815 MemMvddVoltage                            : 5400
+ 0x0432 (1074) H     1815 MemMvddVoltage                            : 5400
+ 0x0434 (1076) H     1815 MemMvddVoltage                            : 5400
+ 0x0436 (1078) H     2003 GfxclkFgfxoffEntry                        : 800
+ 0x0438 (1080) H     2003 GfxclkFinit                               : 800
+ 0x043a (1082) H     2003 GfxclkFidle                               : 800
+ 0x043c (1084) H     0000 GfxclkSlewRate                            : 0
+ 0x043e (1086) H     0000 GfxclkFopt                                : 0
+ 0x0440 (1088) B       d0 Padding567                                : 208
+ 0x0441 (1089) B       01 Padding567                                : 1
+ 0x0442 (1090) H     0000 GfxclkDsMaxFreq                           : 0
+ 0x0444 (1092) B       01 GfxclkSource                              : 1
+ 0x0445 (1093) B       02 Padding456                                : 2
+ 0x0446 (1094) B       00 LowestUclkReservedForUlv                  : 0
+ 0x0447 (1095) B       00 Uclk                                      : 0
+ 0x0448 (1096) B       5b Uclk                                      : 91
+ 0x0449 (1097) B       00 Uclk                                      : 0
+ 0x044a (1098) B       00 MemoryType                                : 0
+ 0x044b (1099) B       10 MemoryChannels                            : 16
+ 0x044c (1100) B       00 PaddingMem                                : 0
+ 0x044d (1101) B       00 PaddingMem                                : 0
+ 0x044e (1102) B       00 PcieGenSpeed                              : 0
+ 0x044f (1103) B       03 PcieGenSpeed                              : 3
+ 0x0450 (1104) B       06 PcieLaneCount                             : 6
+ 0x0451 (1105) B       06 PcieLaneCount                             : 6
+ 0x0452 (1106) H     6b02 LclkFreq                                  : 619
+ 0x0454 (1108) H     6b02 LclkFreq                                  : 619
+ 0x0456 (1110) H     0000 EnableTdpm                                : 0
+ 0x0458 (1112) H     0000 TdpmHighHystTemperature                   : 0
+ 0x045a (1114) H     0000 TdpmLowHystTemperature                    : 0
+ 0x045c (1116) H     0000 GfxclkFreqHighTempLimit                   : 0
+ 0x045e (1118) H     0000 FanStopTemp                               : 0
+ 0x0460 (1120) H     0000 FanStartTemp                              : 0
+ 0x0462 (1122) H     9001 FanGainEdge                               : 400
+ 0x0464 (1124) H     9001 FanGainHotspot                            : 400
+ 0x0466 (1126) H     9001 FanGainLiquid0                            : 400
+ 0x0468 (1128) H     9001 FanGainLiquid1                            : 400
+ 0x046a (1130) H     9001 FanGainVrGfx                              : 400
+ 0x046c (1132) H     9001 FanGainVrSoc                              : 400
+ 0x046e (1134) H     9001 FanGainVrMem0                             : 400
+ 0x0470 (1136) H     9001 FanGainVrMem1                             : 400
+ 0x0472 (1138) H     9001 FanGainPlx                                : 400
+ 0x0474 (1140) H     9001 FanGainMem                                : 400
+ 0x0476 (1142) H     1400 FanPwmMin                                 : 20
+ 0x0478 (1144) H     3408 FanAcousticLimitRpm                       : 2100
+ 0x047a (1146) H     3408 FanThrottlingRpm                          : 2100
+ 0x047c (1148) H     5613 FanMaximumRpm                             : 4950
+ 0x047e (1150) H     5a00 FanTargetTemperature                      : 90
+ 0x0480 (1152) H     2003 FanTargetGfxclk                           : 800
+ 0x0482 (1154) B       01 FanTempInputSelect                        : 1
+ 0x0483 (1155) B       00 FanPadding                                : 0
+ 0x0484 (1156) B       00 FanZeroRpmEnable                          : 0
+ 0x0485 (1157) B       02 FanTachEdgePerRev                         : 2
+ 0x0486 (1158) h     0000 FuzzyFan_ErrorSetDelta                    : 0
+ 0x0488 (1160) h     0000 FuzzyFan_ErrorRateSetDelta                : 0
+ 0x048a (1162) h     0000 FuzzyFan_PwmSetDelta                      : 0
+ 0x048c (1164) H     0000 FuzzyFan_Reserved                         : 0
+ 0x048e (1166) B       00 OverrideAvfsGb                            : 0
+ 0x048f (1167) B       00 OverrideAvfsGb                            : 0
+ 0x0490 (1168) B       00 Padding8_Avfs                             : 0
+ 0x0491 (1169) B       00 Padding8_Avfs                             : 0
+ 0x0492 (1170) f 47e6913c a                                         : 0.01781
+ 0x0496 (1174) f aca841bd b                                         :-0.04728
+ 0x049a (1178) f 13445d3d c                                         : 0.05402
+ 0x049e (1182) f 00000000 a                                         : 0
+ 0x04a2 (1186) f 00000000 b                                         : 0
+ 0x04a6 (1190) f 8fc2f53c c                                         : 0.03
+ 0x04aa (1194) f 00000000 a                                         : 0
+ 0x04ae (1198) f 00000000 b                                         : 0
+ 0x04b2 (1202) f 00000000 c                                         : 0
+ 0x04b6 (1206) f 4bc8c73d a                                         : 0.09755
+ 0x04ba (1210) f 9834463d b                                         : 0.04839
+ 0x04be (1214) f 7042a1bd c                                         :-0.07874
+ 0x04c2 (1218) f af5a193b a                                         : 0.00234
+ 0x04c6 (1222) f 8ca11cbb b                                         :-0.00239
+ 0x04ca (1226) f f836bd3d c                                         : 0.09239
+ 0x04ce (1230) f 00000000 m                                         : 0
+ 0x04d2 (1234) f 00000000 b                                         : 0
+ 0x04d6 (1238) f 00000000 m                                         : 0
+ 0x04da (1242) f 00000000 b                                         : 0
+ 0x04de (1246) f 00000000 a                                         : 0
+ 0x04e2 (1250) f 00000000 b                                         : 0
+ 0x04e6 (1254) f 00000000 c                                         : 0
+ 0x04ea (1258) f 00000000 a                                         : 0
+ 0x04ee (1262) f 00000000 b                                         : 0
+ 0x04f2 (1266) f 00000000 c                                         : 0
+ 0x04f6 (1270) H     a000 DcTol                                     : 160
+ 0x04f8 (1272) H     a000 DcTol                                     : 160
+ 0x04fa (1274) B       01 DcBtcEnabled                              : 1
+ 0x04fb (1275) B       01 DcBtcEnabled                              : 1
+ 0x04fc (1276) B       00 Padding8_GfxBtc                           : 0
+ 0x04fd (1277) B       00 Padding8_GfxBtc                           : 0
+ 0x04fe (1278) H     0000 DcBtcMin                                  : 0
+ 0x0500 (1280) H     0000 DcBtcMin                                  : 0
+ 0x0502 (1282) H     a000 DcBtcMax                                  : 160
+ 0x0504 (1284) H     a000 DcBtcMax                                  : 160
+ 0x0506 (1286) I 00020000 DebugOverrides                            : 512
+ 0x050a (1290) f 00000000 a                                         : 0
+ 0x050e (1294) f 00000000 b                                         : 0
+ 0x0512 (1298) f 00000000 c                                         : 0
+ 0x0516 (1302) f 00000000 a                                         : 0
+ 0x051a (1306) f 00000000 b                                         : 0
+ 0x051e (1310) f 00000000 c                                         : 0
+ 0x0522 (1314) f 00000000 a                                         : 0
+ 0x0526 (1318) f 00000000 b                                         : 0
+ 0x052a (1322) f 00000000 c                                         : 0
+ 0x052e (1326) f 00000000 a                                         : 0
+ 0x0532 (1330) f 00000000 b                                         : 0
+ 0x0536 (1334) f 00000000 c                                         : 0
+ 0x053a (1338) B       01 TotalPowerConfig                          : 1
+ 0x053b (1339) B       00 TotalPowerSpare1                          : 0
+ 0x053c (1340) H     0000 TotalPowerSpare2                          : 0
+ 0x053e (1342) H     0000 PccThresholdLow                           : 0
+ 0x0540 (1344) H     0000 PccThresholdHigh                          : 0
+ 0x0542 (1346) I 00000000 MGpuFanBoostLimitRpm                      : 0
+ 0x0546 (1350) I 00000000 PaddingAPCC                               : 0
+ 0x054a (1354) I 00000000 PaddingAPCC                               : 0
+ 0x054e (1358) I 00000000 PaddingAPCC                               : 0
+ 0x0552 (1362) I 00000000 PaddingAPCC                               : 0
+ 0x0556 (1366) I 00000000 PaddingAPCC                               : 0
+ 0x055a (1370) H     0000 VDDGFX_TVmin                              : 0
+ 0x055c (1372) H     0000 VDDSOC_TVmin                              : 0
+ 0x055e (1374) H     0000 VDDGFX_Vmin_HiTemp                        : 0
+ 0x0560 (1376) H     0000 VDDGFX_Vmin_LoTemp                        : 0
+ 0x0562 (1378) H     0000 VDDSOC_Vmin_HiTemp                        : 0
+ 0x0564 (1380) H     0000 VDDSOC_Vmin_LoTemp                        : 0
+ 0x0566 (1382) H     0000 VDDGFX_TVminHystersis                     : 0
+ 0x0568 (1384) H     0000 VDDSOC_TVminHystersis                     : 0
+ 0x056a (1386) I 00000000 BtcConfig                                 : 0
+ 0x056e (1390) H     a901 SsFmin                                    : 425
+ 0x0570 (1392) H     8700 SsFmin                                    : 135
+ 0x0572 (1394) H     8700 SsFmin                                    : 135
+ 0x0574 (1396) H     0000 SsFmin                                    : 0
+ 0x0576 (1398) H     0000 SsFmin                                    : 0
+ 0x0578 (1400) H     0000 SsFmin                                    : 0
+ 0x057a (1402) H     0000 SsFmin                                    : 0
+ 0x057c (1404) H     0000 SsFmin                                    : 0
+ 0x057e (1406) H     0000 SsFmin                                    : 0
+ 0x0580 (1408) H     0000 SsFmin                                    : 0
+ 0x0582 (1410) H     1900 DcBtcGb                                   : 25
+ 0x0584 (1412) H     1900 DcBtcGb                                   : 25
+ 0x0586 (1414) I 00000000 Reserved                                  : 0
+ 0x058a (1418) I 00000000 Reserved                                  : 0
+ 0x058e (1422) I 00000000 Reserved                                  : 0
+ 0x0592 (1426) I 00000000 Reserved                                  : 0
+ 0x0596 (1430) I 00000000 Reserved                                  : 0
+ 0x059a (1434) I 00000000 Reserved                                  : 0
+ 0x059e (1438) I 00000000 Reserved                                  : 0
+ 0x05a2 (1442) I 00000000 Reserved                                  : 0
+ 0x05a6 (1446) B       00 Enabled                                   : 0
+ 0x05a7 (1447) B       00 Speed                                     : 0
+ 0x05a8 (1448) B       00 Padding                                   : 0
+ 0x05a9 (1449) B       00 Padding                                   : 0
+ 0x05aa (1450) I 00000000 SlaveAddress                              : 0
+ 0x05ae (1454) B       00 ControllerPort                            : 0
+ 0x05af (1455) B       00 ControllerName                            : 0
+ 0x05b0 (1456) B       00 ThermalThrotter                           : 0
+ 0x05b1 (1457) B       00 I2cProtocol                               : 0
+ 0x05b2 (1458) B       00 Enabled                                   : 0
+ 0x05b3 (1459) B       00 Speed                                     : 0
+ 0x05b4 (1460) B       00 Padding                                   : 0
+ 0x05b5 (1461) B       00 Padding                                   : 0
+ 0x05b6 (1462) I 00000000 SlaveAddress                              : 0
+ 0x05ba (1466) B       00 ControllerPort                            : 0
+ 0x05bb (1467) B       00 ControllerName                            : 0
+ 0x05bc (1468) B       00 ThermalThrotter                           : 0
+ 0x05bd (1469) B       00 I2cProtocol                               : 0
+ 0x05be (1470) B       00 Enabled                                   : 0
+ 0x05bf (1471) B       00 Speed                                     : 0
+ 0x05c0 (1472) B       00 Padding                                   : 0
+ 0x05c1 (1473) B       00 Padding                                   : 0
+ 0x05c2 (1474) I 00000000 SlaveAddress                              : 0
+ 0x05c6 (1478) B       00 ControllerPort                            : 0
+ 0x05c7 (1479) B       00 ControllerName                            : 0
+ 0x05c8 (1480) B       00 ThermalThrotter                           : 0
+ 0x05c9 (1481) B       00 I2cProtocol                               : 0
+ 0x05ca (1482) B       00 Enabled                                   : 0
+ 0x05cb (1483) B       00 Speed                                     : 0
+ 0x05cc (1484) B       00 Padding                                   : 0
+ 0x05cd (1485) B       00 Padding                                   : 0
+ 0x05ce (1486) I 00000000 SlaveAddress                              : 0
+ 0x05d2 (1490) B       00 ControllerPort                            : 0
+ 0x05d3 (1491) B       00 ControllerName                            : 0
+ 0x05d4 (1492) B       00 ThermalThrotter                           : 0
+ 0x05d5 (1493) B       00 I2cProtocol                               : 0
+ 0x05d6 (1494) B       00 Enabled                                   : 0
+ 0x05d7 (1495) B       00 Speed                                     : 0
+ 0x05d8 (1496) B       00 Padding                                   : 0
+ 0x05d9 (1497) B       00 Padding                                   : 0
+ 0x05da (1498) I 00000000 SlaveAddress                              : 0
+ 0x05de (1502) B       00 ControllerPort                            : 0
+ 0x05df (1503) B       00 ControllerName                            : 0
+ 0x05e0 (1504) B       00 ThermalThrotter                           : 0
+ 0x05e1 (1505) B       00 I2cProtocol                               : 0
+ 0x05e2 (1506) B       00 Enabled                                   : 0
+ 0x05e3 (1507) B       00 Speed                                     : 0
+ 0x05e4 (1508) B       00 Padding                                   : 0
+ 0x05e5 (1509) B       00 Padding                                   : 0
+ 0x05e6 (1510) I 00000000 SlaveAddress                              : 0
+ 0x05ea (1514) B       00 ControllerPort                            : 0
+ 0x05eb (1515) B       00 ControllerName                            : 0
+ 0x05ec (1516) B       00 ThermalThrotter                           : 0
+ 0x05ed (1517) B       00 I2cProtocol                               : 0
+ 0x05ee (1518) B       00 Enabled                                   : 0
+ 0x05ef (1519) B       00 Speed                                     : 0
+ 0x05f0 (1520) B       00 Padding                                   : 0
+ 0x05f1 (1521) B       00 Padding                                   : 0
+ 0x05f2 (1522) I 00000000 SlaveAddress                              : 0
+ 0x05f6 (1526) B       00 ControllerPort                            : 0
+ 0x05f7 (1527) B       00 ControllerName                            : 0
+ 0x05f8 (1528) B       00 ThermalThrotter                           : 0
+ 0x05f9 (1529) B       00 I2cProtocol                               : 0
+ 0x05fa (1530) B       00 Enabled                                   : 0
+ 0x05fb (1531) B       00 Speed                                     : 0
+ 0x05fc (1532) B       00 Padding                                   : 0
+ 0x05fd (1533) B       00 Padding                                   : 0
+ 0x05fe (1534) I 00000000 SlaveAddress                              : 0
+ 0x0602 (1538) B       00 ControllerPort                            : 0
+ 0x0603 (1539) B       00 ControllerName                            : 0
+ 0x0604 (1540) B       00 ThermalThrotter                           : 0
+ 0x0605 (1541) B       00 I2cProtocol                               : 0
+ 0x0606 (1542) H     0000 MaxVoltageStepGfx                         : 0
+ 0x0608 (1544) H     0000 MaxVoltageStepSoc                         : 0
+ 0x060a (1546) B       00 VddGfxVrMapping                           : 0
+ 0x060b (1547) B       00 VddSocVrMapping                           : 0
+ 0x060c (1548) B       00 VddMem0VrMapping                          : 0
+ 0x060d (1549) B       00 VddMem1VrMapping                          : 0
+ 0x060e (1550) B       00 GfxUlvPhaseSheddingMask                   : 0
+ 0x060f (1551) B       00 SocUlvPhaseSheddingMask                   : 0
+ 0x0610 (1552) B       00 ExternalSensorPresent                     : 0
+ 0x0611 (1553) B       00 Padding8_V                                : 0
+ 0x0612 (1554) H     0000 GfxMaxCurrent                             : 0
+ 0x0614 (1556) b       00 GfxOffset                                 : 0
+ 0x0615 (1557) B       00 Padding_TelemetryGfx                      : 0
+ 0x0616 (1558) H     0000 SocMaxCurrent                             : 0
+ 0x0618 (1560) b       00 SocOffset                                 : 0
+ 0x0619 (1561) B       00 Padding_TelemetrySoc                      : 0
+ 0x061a (1562) H     0000 Mem0MaxCurrent                            : 0
+ 0x061c (1564) b       00 Mem0Offset                                : 0
+ 0x061d (1565) B       00 Padding_TelemetryMem0                     : 0
+ 0x061e (1566) H     0000 Mem1MaxCurrent                            : 0
+ 0x0620 (1568) b       00 Mem1Offset                                : 0
+ 0x0621 (1569) B       00 Padding_TelemetryMem1                     : 0
+ 0x0622 (1570) B       00 AcDcGpio                                  : 0
+ 0x0623 (1571) B       00 AcDcPolarity                              : 0
+ 0x0624 (1572) B       00 VR0HotGpio                                : 0
+ 0x0625 (1573) B       00 VR0HotPolarity                            : 0
+ 0x0626 (1574) B       00 VR1HotGpio                                : 0
+ 0x0627 (1575) B       00 VR1HotPolarity                            : 0
+ 0x0628 (1576) B       00 GthrGpio                                  : 0
+ 0x0629 (1577) B       00 GthrPolarity                              : 0
+ 0x062a (1578) B       00 LedPin0                                   : 0
+ 0x062b (1579) B       00 LedPin1                                   : 0
+ 0x062c (1580) B       00 LedPin2                                   : 0
+ 0x062d (1581) B       00 padding8_4                                : 0
+ 0x062e (1582) B       00 PllGfxclkSpreadEnabled                    : 0
+ 0x062f (1583) B       00 PllGfxclkSpreadPercent                    : 0
+ 0x0630 (1584) H     0000 PllGfxclkSpreadFreq                       : 0
+ 0x0632 (1586) B       00 DfllGfxclkSpreadEnabled                   : 0
+ 0x0633 (1587) B       00 DfllGfxclkSpreadPercent                   : 0
+ 0x0634 (1588) H     0000 DfllGfxclkSpreadFreq                      : 0
+ 0x0636 (1590) B       00 UclkSpreadEnabled                         : 0
+ 0x0637 (1591) B       00 UclkSpreadPercent                         : 0
+ 0x0638 (1592) H     0000 UclkSpreadFreq                            : 0
+ 0x063a (1594) B       00 SoclkSpreadEnabled                        : 0
+ 0x063b (1595) B       00 SocclkSpreadPercent                       : 0
+ 0x063c (1596) H     0000 SocclkSpreadFreq                          : 0
+ 0x063e (1598) H     0000 TotalBoardPower                           : 0
+ 0x0640 (1600) H     0000 BoardPadding                              : 0
+ 0x0642 (1602) I 00000000 MvddRatio                                 : 0
+ 0x0646 (1606) B       00 RenesesLoadLineEnabled                    : 0
+ 0x0647 (1607) B       00 GfxLoadlineResistance                     : 0
+ 0x0648 (1608) B       00 SocLoadlineResistance                     : 0
+ 0x0649 (1609) B       00 Padding8_Loadline                         : 0
+ 0x064a (1610) I 00000000 BoardReserved                             : 0
+ 0x064e (1614) I 00000000 BoardReserved                             : 0
+ 0x0652 (1618) I 00000000 BoardReserved                             : 0
+ 0x0656 (1622) I 00000000 BoardReserved                             : 0
+ 0x065a (1626) I 00000000 BoardReserved                             : 0
+ 0x065e (1630) I 00000000 BoardReserved                             : 0
+ 0x0662 (1634) I 00000000 BoardReserved                             : 0
+ 0x0666 (1638) I 00000000 BoardReserved                             : 0
+ 0x066a (1642) I 00000000 MmHubPadding                              : 0
+ 0x066e (1646) I 00000000 MmHubPadding                              : 0
+ 0x0672 (1650) I 00000000 MmHubPadding                              : 0
+ 0x0676 (1654) I 00000000 MmHubPadding                              : 0
+ 0x067a (1658) I 00000000 MmHubPadding                              : 0
+ 0x067e (1662) I 00000000 MmHubPadding                              : 0
+ 0x0682 (1666) I 00000000 MmHubPadding                              : 0
+ 0x0686 (1670) I 00000000 MmHubPadding                              : 0
```

### Comparing `upp-0.2.0/test/navi23.mpt` & `upp-0.2.1/test/navi23.mpt`

 * *Files identical despite different names*

### Comparing `upp-0.2.0/test/test.sh` & `upp-0.2.1/test/test.sh`

 * *Files identical despite different names*

