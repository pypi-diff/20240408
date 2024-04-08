# Comparing `tmp/cSecp256k1-1.1.1.tar.gz` & `tmp/cSecp256k1-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cSecp256k1-1.1.1.tar", last modified: Mon Jan 24 09:09:16 2022, max compression
+gzip compressed data, was "cSecp256k1-1.1.2.tar", last modified: Mon Apr  8 20:18:15 2024, max compression
```

## Comparing `cSecp256k1-1.1.1.tar` & `cSecp256k1-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-01-24 09:09:16.655388 cSecp256k1-1.1.1/
--rw-rw-rw-   0        0        0       80 2021-03-21 23:20:08.000000 cSecp256k1-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3851 2022-01-24 09:09:16.654389 cSecp256k1-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2022-01-24 09:09:12.000000 cSecp256k1-1.1.1/README.md
--rw-rw-rw-   0        0        0        5 2022-01-24 09:06:15.000000 cSecp256k1-1.1.1/VERSION
-drwxrwxrwx   0        0        0        0 2022-01-24 09:09:16.612503 cSecp256k1-1.1.1/cSecp256k1/
--rw-rw-rw-   0        0        0    12531 2021-07-21 18:06:00.000000 cSecp256k1-1.1.1/cSecp256k1/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-24 09:09:16.626471 cSecp256k1-1.1.1/cSecp256k1.egg-info/
--rw-rw-rw-   0        0        0     3851 2022-01-24 09:09:15.000000 cSecp256k1-1.1.1/cSecp256k1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2022-01-24 09:09:16.000000 cSecp256k1-1.1.1/cSecp256k1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-24 09:09:15.000000 cSecp256k1-1.1.1/cSecp256k1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-01-24 09:09:15.000000 cSecp256k1-1.1.1/cSecp256k1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-24 09:09:16.655388 cSecp256k1-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     4541 2021-11-07 15:54:10.000000 cSecp256k1-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-24 09:09:16.645414 cSecp256k1-1.1.1/src/
--rw-rw-rw-   0        0        0     2713 2021-06-20 05:35:27.000000 cSecp256k1-1.1.1/src/ecdsa.c
--rw-rw-rw-   0        0        0      304 2021-06-20 05:23:44.000000 cSecp256k1-1.1.1/src/ecdsa.h
--rw-rw-rw-   0        0        0     7143 2022-01-24 07:23:38.000000 cSecp256k1-1.1.1/src/schnorr.c
--rw-rw-rw-   0        0        0     1648 2021-06-19 13:47:28.000000 cSecp256k1-1.1.1/src/schnorr.h
--rw-rw-rw-   0        0        0     8324 2021-06-20 20:42:09.000000 cSecp256k1-1.1.1/src/secp256k1.h
--rw-rw-rw-   0        0        0     5263 2015-04-27 03:50:49.000000 cSecp256k1-1.1.1/src/sha256.c
--rw-rw-rw-   0        0        0     1215 2015-04-27 03:50:49.000000 cSecp256k1-1.1.1/src/sha256.h
-drwxrwxrwx   0        0        0        0 2022-01-24 09:09:16.652396 cSecp256k1-1.1.1/test/
--rw-rw-rw-   0        0        0     2024 2021-06-20 12:05:18.000000 cSecp256k1-1.1.1/test/test_code.py
--rw-rw-rw-   0        0        0     2862 2021-06-19 12:38:31.000000 cSecp256k1-1.1.1/test/test_signatures.py
--rw-rw-rw-   0        0        0     2414 2021-06-05 15:18:54.000000 cSecp256k1-1.1.1/test/test_vectors.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:18:15.370248 cSecp256k1-1.1.2/
+-rw-rw-rw-   0        0        0       80 2021-03-21 23:20:08.000000 cSecp256k1-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3802 2024-04-08 20:18:15.369250 cSecp256k1-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2196 2024-04-08 20:14:20.000000 cSecp256k1-1.1.2/README.md
+-rw-rw-rw-   0        0        0        5 2022-12-27 16:04:13.000000 cSecp256k1-1.1.2/VERSION
+drwxrwxrwx   0        0        0        0 2024-04-08 20:18:14.835862 cSecp256k1-1.1.2/cSecp256k1/
+-rw-rw-rw-   0        0        0    13842 2024-04-01 20:35:11.000000 cSecp256k1-1.1.2/cSecp256k1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:18:14.876332 cSecp256k1-1.1.2/cSecp256k1.egg-info/
+-rw-rw-rw-   0        0        0     3802 2024-04-08 20:18:12.000000 cSecp256k1-1.1.2/cSecp256k1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-04-08 20:18:14.000000 cSecp256k1-1.1.2/cSecp256k1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 20:18:12.000000 cSecp256k1-1.1.2/cSecp256k1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-08 20:18:12.000000 cSecp256k1-1.1.2/cSecp256k1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 20:18:15.371245 cSecp256k1-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     4541 2021-11-07 15:54:10.000000 cSecp256k1-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 20:18:15.294394 cSecp256k1-1.1.2/src/
+-rw-rw-rw-   0        0        0     2713 2021-06-20 05:35:27.000000 cSecp256k1-1.1.2/src/ecdsa.c
+-rw-rw-rw-   0        0        0      304 2021-06-20 05:23:44.000000 cSecp256k1-1.1.2/src/ecdsa.h
+-rw-rw-rw-   0        0        0     7143 2022-01-24 07:23:38.000000 cSecp256k1-1.1.2/src/schnorr.c
+-rw-rw-rw-   0        0        0     1648 2021-06-19 13:47:28.000000 cSecp256k1-1.1.2/src/schnorr.h
+-rw-rw-rw-   0        0        0     8324 2021-06-20 20:42:09.000000 cSecp256k1-1.1.2/src/secp256k1.h
+-rw-rw-rw-   0        0        0     5263 2015-04-27 03:50:49.000000 cSecp256k1-1.1.2/src/sha256.c
+-rw-rw-rw-   0        0        0     1215 2015-04-27 03:50:49.000000 cSecp256k1-1.1.2/src/sha256.h
+drwxrwxrwx   0        0        0        0 2024-04-08 20:18:15.347571 cSecp256k1-1.1.2/test/
+-rw-rw-rw-   0        0        0     2024 2021-06-20 12:05:18.000000 cSecp256k1-1.1.2/test/test_code.py
+-rw-rw-rw-   0        0        0     2871 2024-04-01 21:50:18.000000 cSecp256k1-1.1.2/test/test_signatures.py
+-rw-rw-rw-   0        0        0     2432 2024-04-01 21:49:23.000000 cSecp256k1-1.1.2/test/test_vectors.py
```

### Comparing `cSecp256k1-1.1.1/PKG-INFO` & `cSecp256k1-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 Metadata-Version: 2.1
 Name: cSecp256k1
-Version: 1.1.1
+Version: 1.1.2
 Summary: Fast python implementation for bitcoin curve
 Home-page: https://github.com/Moustikitos/fast-curve
 Author: Toons
 Author-email: moustikitos@gmail.com
 Maintainer: Toons
 Maintainer-email: moustikitos@gmail.com
 License: Copyright 2021, MIT licence
 Download-URL: https://github.com/Moustikitos/fast-curve/archive/master.zip
 Description: # fast-curve
         
         `ctypes` implementation for bitcoin curve `secp256k1`. It is 100 times faster than pure python implementation and may be even faster if used in lower level development languages.
         
-        ## Support this project
-         
-         [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate)
-         
-         [Buy &#1126;](https://bittrex.com/Account/Register?referralCode=NW5-DQO-QMT) and:
-         
-           * [X] Send &#1126; to `AUahWfkfr5J4tYakugRbfow7RWVTK35GPW`
-           * [X] Vote `arky` on [Ark blockchain](https://explorer.ark.io) and [earn &#1126; weekly](http://dpos.arky-delegate.info/arky)
-        
         
         # Dependencies
         
         ## Ubuntu
         
         ```shell
         sudo apt-get install python3-dev libgmp3-dev libgmp3
@@ -61,14 +52,17 @@
         
         For **Windows users**, a built package is available
         [here](https://github.com/Moustikitos/fast-curve/raw/master/download/cSecp256k1-1.1.1-win64.7z).
         Exctract content anywhere in python path defined by `sys.path`.
         
         # Versions
         
+        ## 1.1.2
+         - [x] typing update
+        
         ## 1.1.1
          - [x] exclusive use of `hash_sha256_s` in `schnorr.c`
         
         ## 1.0.6
          - [x] bugfix in `bcrypto410_*` schnorr signature
         
         ## 1.0.5
@@ -76,24 +70,25 @@
          - [x] minor `setup.py` module tweaks
         
         ## 1.0.4
          - [x] C code improvement
          - [x] code coverage improvement
          - [x] pydoc-markdown documentation added
         
-        ## 1.0.4
-         - [x] C code improvement
-         - [x] code coverage improvement
-         - [x] pydoc-markdown documentation added
-        
         ## 1.0.3
          - [x] ecdsa signature support
          - [x] bcrypto 4.10 schnorr signature support
          - [x] [BIP0340 sipa](https://github.com/sipa/bips/tree/3b1fb9600b938172dd98a63e4906a861af9c3ab0/bip-0340) shnorr signatures support
         
+        ## Support this project
+        
+        <!-- [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate) -->
+        [![Paypal me](https://img.shields.io/badge/PayPal-toons-00457C?logo=paypal&logoColor=white)](https://paypal.me/toons)
+        [![Bitcoin](https://img.shields.io/badge/Donate-bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x-ff9900?logo=bitcoin)](https://github.com/Moustikitos/python-mainsail/blob/master/docs/img/bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x.png)
+        
 Keywords: ctypes,curve,bitcoin
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cSecp256k1-1.1.1/README.md` & `cSecp256k1-1.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,11 @@
 # fast-curve
 
 `ctypes` implementation for bitcoin curve `secp256k1`. It is 100 times faster than pure python implementation and may be even faster if used in lower level development languages.
 
-## Support this project
- 
- [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate)
- 
- [Buy &#1126;](https://bittrex.com/Account/Register?referralCode=NW5-DQO-QMT) and:
- 
-   * [X] Send &#1126; to `AUahWfkfr5J4tYakugRbfow7RWVTK35GPW`
-   * [X] Vote `arky` on [Ark blockchain](https://explorer.ark.io) and [earn &#1126; weekly](http://dpos.arky-delegate.info/arky)
-
 
 # Dependencies
 
 ## Ubuntu
 
 ```shell
 sudo apt-get install python3-dev libgmp3-dev libgmp3
@@ -50,14 +41,17 @@
 
 For **Windows users**, a built package is available
 [here](https://github.com/Moustikitos/fast-curve/raw/master/download/cSecp256k1-1.1.1-win64.7z).
 Exctract content anywhere in python path defined by `sys.path`.
 
 # Versions
 
+## 1.1.2
+ - [x] typing update
+
 ## 1.1.1
  - [x] exclusive use of `hash_sha256_s` in `schnorr.c`
 
 ## 1.0.6
  - [x] bugfix in `bcrypto410_*` schnorr signature
 
 ## 1.0.5
@@ -65,16 +59,17 @@
  - [x] minor `setup.py` module tweaks
 
 ## 1.0.4
  - [x] C code improvement
  - [x] code coverage improvement
  - [x] pydoc-markdown documentation added
 
-## 1.0.4
- - [x] C code improvement
- - [x] code coverage improvement
- - [x] pydoc-markdown documentation added
-
 ## 1.0.3
  - [x] ecdsa signature support
  - [x] bcrypto 4.10 schnorr signature support
  - [x] [BIP0340 sipa](https://github.com/sipa/bips/tree/3b1fb9600b938172dd98a63e4906a861af9c3ab0/bip-0340) shnorr signatures support
+
+## Support this project
+
+<!-- [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate) -->
+[![Paypal me](https://img.shields.io/badge/PayPal-toons-00457C?logo=paypal&logoColor=white)](https://paypal.me/toons)
+[![Bitcoin](https://img.shields.io/badge/Donate-bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x-ff9900?logo=bitcoin)](https://github.com/Moustikitos/python-mainsail/blob/master/docs/img/bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x.png)
```

### Comparing `cSecp256k1-1.1.1/cSecp256k1.egg-info/PKG-INFO` & `cSecp256k1-1.1.2/cSecp256k1.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 Metadata-Version: 2.1
 Name: cSecp256k1
-Version: 1.1.1
+Version: 1.1.2
 Summary: Fast python implementation for bitcoin curve
 Home-page: https://github.com/Moustikitos/fast-curve
 Author: Toons
 Author-email: moustikitos@gmail.com
 Maintainer: Toons
 Maintainer-email: moustikitos@gmail.com
 License: Copyright 2021, MIT licence
 Download-URL: https://github.com/Moustikitos/fast-curve/archive/master.zip
 Description: # fast-curve
         
         `ctypes` implementation for bitcoin curve `secp256k1`. It is 100 times faster than pure python implementation and may be even faster if used in lower level development languages.
         
-        ## Support this project
-         
-         [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate)
-         
-         [Buy &#1126;](https://bittrex.com/Account/Register?referralCode=NW5-DQO-QMT) and:
-         
-           * [X] Send &#1126; to `AUahWfkfr5J4tYakugRbfow7RWVTK35GPW`
-           * [X] Vote `arky` on [Ark blockchain](https://explorer.ark.io) and [earn &#1126; weekly](http://dpos.arky-delegate.info/arky)
-        
         
         # Dependencies
         
         ## Ubuntu
         
         ```shell
         sudo apt-get install python3-dev libgmp3-dev libgmp3
@@ -61,14 +52,17 @@
         
         For **Windows users**, a built package is available
         [here](https://github.com/Moustikitos/fast-curve/raw/master/download/cSecp256k1-1.1.1-win64.7z).
         Exctract content anywhere in python path defined by `sys.path`.
         
         # Versions
         
+        ## 1.1.2
+         - [x] typing update
+        
         ## 1.1.1
          - [x] exclusive use of `hash_sha256_s` in `schnorr.c`
         
         ## 1.0.6
          - [x] bugfix in `bcrypto410_*` schnorr signature
         
         ## 1.0.5
@@ -76,24 +70,25 @@
          - [x] minor `setup.py` module tweaks
         
         ## 1.0.4
          - [x] C code improvement
          - [x] code coverage improvement
          - [x] pydoc-markdown documentation added
         
-        ## 1.0.4
-         - [x] C code improvement
-         - [x] code coverage improvement
-         - [x] pydoc-markdown documentation added
-        
         ## 1.0.3
          - [x] ecdsa signature support
          - [x] bcrypto 4.10 schnorr signature support
          - [x] [BIP0340 sipa](https://github.com/sipa/bips/tree/3b1fb9600b938172dd98a63e4906a861af9c3ab0/bip-0340) shnorr signatures support
         
+        ## Support this project
+        
+        <!-- [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate) -->
+        [![Paypal me](https://img.shields.io/badge/PayPal-toons-00457C?logo=paypal&logoColor=white)](https://paypal.me/toons)
+        [![Bitcoin](https://img.shields.io/badge/Donate-bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x-ff9900?logo=bitcoin)](https://github.com/Moustikitos/python-mainsail/blob/master/docs/img/bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x.png)
+        
 Keywords: ctypes,curve,bitcoin
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cSecp256k1-1.1.1/setup.py` & `cSecp256k1-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `cSecp256k1-1.1.1/src/ecdsa.c` & `cSecp256k1-1.1.2/src/ecdsa.c`

 * *Files identical despite different names*

### Comparing `cSecp256k1-1.1.1/src/schnorr.c` & `cSecp256k1-1.1.2/src/schnorr.c`

 * *Files identical despite different names*

### Comparing `cSecp256k1-1.1.1/src/schnorr.h` & `cSecp256k1-1.1.2/src/schnorr.h`

 * *Files identical despite different names*

### Comparing `cSecp256k1-1.1.1/src/secp256k1.h` & `cSecp256k1-1.1.2/src/secp256k1.h`

 * *Files identical despite different names*

### Comparing `cSecp256k1-1.1.1/src/sha256.c` & `cSecp256k1-1.1.2/src/sha256.c`

 * *Files identical despite different names*

### Comparing `cSecp256k1-1.1.1/src/sha256.h` & `cSecp256k1-1.1.2/src/sha256.h`

 * *Files identical despite different names*

### Comparing `cSecp256k1-1.1.1/test/test_code.py` & `cSecp256k1-1.1.2/test/test_code.py`

 * *Files identical despite different names*

### Comparing `cSecp256k1-1.1.1/test/test_signatures.py` & `cSecp256k1-1.1.2/test/test_signatures.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     from pySecp256k1 import schnorr
     import binascii
 
     class TestCompare:
         def test_schnorr(self):
             signer = _schnorr.bcrypto410_sign
             sig = signer(msg, pr_key).contents
-            assert sig.raw() == binascii.hexlify(
+            assert sig.raw().encode() == binascii.hexlify(
                 schnorr.bcrypto410_sign(
                     binascii.unhexlify(msg), binascii.unhexlify(pr_key)
                 )
             )
 
 except ImportError:
     pass
```

### Comparing `cSecp256k1-1.1.1/test/test_vectors.py` & `cSecp256k1-1.1.2/test/test_vectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,28 +37,28 @@
             print("pubkey =", pubkey)
             print("rnd =", rnd)
             print("msg =", msg)
 
             assert secp256k1.PublicKey.from_hex(secret0).x == pubkey
             assert (
                 secp256k1._schnorr.sign(msg, secret0, rnd).contents.raw() ==
-                sig
+                sig.decode()
             ) == result
 
     def testVector3(self):
         secret0, pubkey, rnd, msg, sig, result = read_vector(VECTORS[3])
         print("secret0 =", secret0)
         print("pubkey =", pubkey)
         print("rnd =", rnd)
         print("msg =", msg)
 
         assert secp256k1.PublicKey.from_hex(secret0).x == pubkey
         assert (
             secp256k1._schnorr.sign(msg, secret0, rnd).contents.raw() ==
-            sig
+            sig.decode()
         ) == result
 
         msg_mod_p = b"%064x" % (int(msg, 16) % secp256k1.p)
         msg_mod_n = b"%064x" % (int(msg, 16) % secp256k1.n)
         r, s = sig[:64], sig[64:]
         assert not secp256k1._schnorr.verify(msg_mod_p, pubkey, r, s)
         assert not secp256k1._schnorr.verify(msg_mod_n, pubkey, r, s)
```

