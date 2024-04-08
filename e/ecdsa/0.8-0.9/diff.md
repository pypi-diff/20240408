# Comparing `tmp/ecdsa-0.8.tar.gz` & `tmp/ecdsa-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecdsa-0.8.tar", last modified: Fri Jul 13 19:13:12 2012, max compression, from Unix
+gzip compressed data, was "dist/ecdsa-0.9.tar", last modified: Wed Oct  2 00:11:42 2013, max compression
```

## Comparing `ecdsa-0.8.tar` & `ecdsa-0.9.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 warner     (501) staff       (20)        0 2012-07-13 19:13:12.000000 ecdsa-0.8/
-drwxr-xr-x   0 warner     (501) staff       (20)        0 2012-07-13 19:13:12.000000 ecdsa-0.8/ecdsa/
--rw-r--r--   0 warner     (501) staff       (20)      270 2012-07-13 19:13:12.000000 ecdsa-0.8/PKG-INFO
--rw-r--r--   0 warner     (501) staff       (20)    12005 2010-12-01 01:06:33.000000 ecdsa-0.8/README
--rwxr-xr-x   0 warner     (501) staff       (20)     2985 2010-12-01 01:06:33.000000 ecdsa-0.8/setup.py
--rw-r--r--   0 warner     (501) staff       (20)      501 2010-06-09 18:47:42.000000 ecdsa-0.8/ecdsa/__init__.py
--rw-r--r--   0 warner     (501) staff       (20)      177 2012-07-13 19:13:12.000000 ecdsa-0.8/ecdsa/_version.py
--rw-r--r--   0 warner     (501) staff       (20)     1452 2010-12-01 01:06:33.000000 ecdsa-0.8/ecdsa/curves.py
--rw-r--r--   0 warner     (501) staff       (20)     6200 2010-04-19 17:53:40.000000 ecdsa-0.8/ecdsa/der.py
--rw-r--r--   0 warner     (501) staff       (20)    23745 2010-12-01 01:06:33.000000 ecdsa-0.8/ecdsa/ecdsa.py
--rw-r--r--   0 warner     (501) staff       (20)     8499 2010-12-01 01:06:33.000000 ecdsa-0.8/ecdsa/ellipticcurve.py
--rw-r--r--   0 warner     (501) staff       (20)    11162 2011-10-04 22:30:48.000000 ecdsa-0.8/ecdsa/keys.py
--rw-r--r--   0 warner     (501) staff       (20)    16073 2010-12-01 01:06:33.000000 ecdsa-0.8/ecdsa/numbertheory.py
--rw-r--r--   0 warner     (501) staff       (20)    21452 2011-10-04 22:43:50.000000 ecdsa-0.8/ecdsa/test_pyecdsa.py
--rw-r--r--   0 warner     (501) staff       (20)     8885 2010-12-01 01:06:33.000000 ecdsa-0.8/ecdsa/util.py
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2013-10-02 00:11:42.000000 ecdsa-0.9/
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2013-10-02 00:11:42.000000 ecdsa-0.9/ecdsa/
+-rw-r--r--   0 warner     (502) staff       (20)      622 2013-10-01 23:13:25.000000 ecdsa-0.9/ecdsa/__init__.py
+-rw-r--r--   0 warner     (502) staff       (20)      177 2013-10-02 00:11:41.000000 ecdsa-0.9/ecdsa/_version.py
+-rw-r--r--   0 warner     (502) staff       (20)     1640 2013-10-01 23:13:25.000000 ecdsa-0.9/ecdsa/curves.py
+-rw-r--r--   0 warner     (502) staff       (20)     7023 2013-10-01 23:13:25.000000 ecdsa-0.9/ecdsa/der.py
+-rw-r--r--   0 warner     (502) staff       (20)    24328 2013-10-01 23:39:22.000000 ecdsa-0.9/ecdsa/ecdsa.py
+-rw-r--r--   0 warner     (502) staff       (20)     8609 2013-10-01 23:41:31.000000 ecdsa-0.9/ecdsa/ellipticcurve.py
+-rw-r--r--   0 warner     (502) staff       (20)    12323 2013-10-01 23:13:25.000000 ecdsa-0.9/ecdsa/keys.py
+-rw-r--r--   0 warner     (502) staff       (20)    16105 2013-10-01 23:41:06.000000 ecdsa-0.9/ecdsa/numbertheory.py
+-rw-r--r--   0 warner     (502) staff       (20)     2794 2013-10-01 23:40:27.000000 ecdsa-0.9/ecdsa/rfc6979.py
+-rw-r--r--   0 warner     (502) staff       (20)    11985 2013-10-01 23:13:25.000000 ecdsa-0.9/ecdsa/six.py
+-rw-r--r--   0 warner     (502) staff       (20)    28868 2013-10-01 23:31:28.000000 ecdsa-0.9/ecdsa/test_pyecdsa.py
+-rw-r--r--   0 warner     (502) staff       (20)     9263 2013-10-01 23:31:48.000000 ecdsa-0.9/ecdsa/util.py
+-rw-r--r--   0 warner     (502) staff       (20)     1147 2010-04-27 19:08:46.000000 ecdsa-0.9/LICENSE
+-rw-r--r--   0 warner     (502) staff       (20)       60 2013-10-01 23:50:50.000000 ecdsa-0.9/MANIFEST.in
+-rw-r--r--   0 warner     (502) staff       (20)     1273 2013-10-01 23:56:15.000000 ecdsa-0.9/NEWS
+-rw-r--r--   0 warner     (502) staff       (20)      270 2013-10-02 00:11:42.000000 ecdsa-0.9/PKG-INFO
+-rw-r--r--   0 warner     (502) staff       (20)    13016 2013-10-02 00:02:52.000000 ecdsa-0.9/README.md
+-rwxr-xr-x   0 warner     (502) staff       (20)     3023 2013-10-01 23:13:25.000000 ecdsa-0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ecdsa-0.8/README` & `ecdsa-0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,293 +1,305 @@
+# Pure-Python ECDSA
+
+[![build status](https://travis-ci.org/warner/python-ecdsa.png)](http://travis-ci.org/warner/python-ecdsa)
 
-= Pure-Python ECDSA =
 
 This is an easy-to-use implementation of ECDSA cryptography (Elliptic Curve
 Digital Signature Algorithm), implemented purely in Python, released under
 the MIT license. With this library, you can quickly create keypairs (signing
 key and verifying key), sign messages, and verify the signatures. The keys
 and signatures are very short, making them easy to handle and incorporate
 into other protocols.
 
-== Features ==
+## Features
 
 This library provides key generation, signing, and verifying, for five
 popular NIST "Suite B" GF(p) curves, with key lengths of 192, 224, 256, 384,
 and 521 bits. The "short names" for these curves, as known by the OpenSSL
 tool, are: prime192v1, secp224r1, prime256v1, secp384r1, and secp521r1. No
 other curves are included, but it would not be too hard to add more.
 
-== Dependencies ==
+## Dependencies
 
 This library uses only Python. It requires python2.5 or later versions of the
-python2.x series. It is not compatible with python3.x .
+python2.x series. It is also compatible with python3.2 and 3.3.
 
 To run the OpenSSL compatibility tests, the 'openssl' tool must be on your
 $PATH. This release has been tested successfully against both OpenSSL 0.9.8o
 and 1.0.0a .
 
-== Speed ==
+## Speed
 
 The following table shows how long this library takes to generate keypairs
 (keygen=), to sign data (sign=), and to verify those signatures (verify=), on
 my 2008 Mac laptop. All times are in seconds. It also shows the length of a
 signature (in bytes): the verifying ("public") key is typically the same
 length as the signature, and the signing ("private") key is half that length.
 
-  NIST192p: siglen= 48, keygen=0.160s, sign=0.058s, verify=0.116s
-  NIST224p: siglen= 56, keygen=0.230s, sign=0.086s, verify=0.165s
-  NIST256p: siglen= 64, keygen=0.305s, sign=0.112s, verify=0.220s
-  NIST384p: siglen= 96, keygen=0.801s, sign=0.289s, verify=0.558s
-  NIST521p: siglen=132, keygen=1.582s, sign=0.584s, verify=1.152s
+* NIST192p: siglen= 48, keygen=0.160s, sign=0.058s, verify=0.116s
+* NIST224p: siglen= 56, keygen=0.230s, sign=0.086s, verify=0.165s
+* NIST256p: siglen= 64, keygen=0.305s, sign=0.112s, verify=0.220s
+* NIST384p: siglen= 96, keygen=0.801s, sign=0.289s, verify=0.558s
+* NIST521p: siglen=132, keygen=1.582s, sign=0.584s, verify=1.152s
 
 For comparison, a quality C++ implementation of ECDSA (Crypto++) typically
 computes a NIST256p signature in 2.88ms and a verification in 8.53ms, about
 30-40x faster.
 
 Keys and signature can be serialized in different ways (see Usage, below).
 For a NIST192p key, the three basic representations require strings of the
 following lengths (in bytes):
 
-  to_string:  signkey= 24, verifykey= 48, signature=48
-  DER:        signkey=106, verifykey= 80, signature=55
-  PEM:        signkey=278, verifykey=162, (no support for PEM signatures)
+    to_string:  signkey= 24, verifykey= 48, signature=48
+    DER:        signkey=106, verifykey= 80, signature=55
+    PEM:        signkey=278, verifykey=162, (no support for PEM signatures)
 
-== History ==
+## History
 
 In 2006, Peter Pearson announced his pure-python implementation of ECDSA in a
-message to sci.crypt[1], available from his download site[2]. In 2010, Brian
-Warner wrote a wrapper around this code, to make it a bit easier and safer to
-use. You are looking at the README for this wrapper.
+[message to sci.crypt][1], available from his [download site][2]. In 2010,
+Brian Warner wrote a wrapper around this code, to make it a bit easier and
+safer to use. You are looking at the README for this wrapper.
+
+[1]: http://www.derkeiler.com/Newsgroups/sci.crypt/2006-01/msg00651.html
+[2]: http://webpages.charter.net/curryfans/peter/downloads.html
 
-== Testing ==
+## Testing
 
 There are four test suites, three for the original Pearson module, and one
 more for the wrapper. To run them all, do this:
 
- python ecdsa/numbertheory.py   # look for "****" and "failed" for problems
- python ecdsa/ellipticcurve.py   # look for "Bad" for problems
- python ecdsa/ecdsa.py   # look for "****" and "failed" for problems
- python ecdsa/test_pyecdsa.py  # look for "FAILED" for problems
+    python ecdsa/numbertheory.py   # look for "****" and "failed" for problems
+    python ecdsa/ellipticcurve.py   # look for "Bad" for problems
+    python ecdsa/ecdsa.py   # look for "****" and "failed" for problems
+    python ecdsa/test_pyecdsa.py  # look for "FAILED" for problems
 
 On my 2009 Mac laptop, the combined tests take about 34 seconds to run. On a
 2.4GHz P4 Linux box, they take 81 seconds.
 
-One component of test_pyecdsa.py checks compatibility with OpenSSL, by
+One component of `test_pyecdsa.py` checks compatibility with OpenSSL, by
 running the "openssl" CLI tool. If this tool is not on your $PATH, you may
 want to comment out this test (the easiest way is to add a line that says
 "del OpenSSL" to the end of test_pyecdsa.py).
 
-== Security ==
+## Security
 
 This library does not protect against timing attacks. Do not allow attackers
 to measure how long it takes you to generate a keypair or sign a message.
 This library depends upon a strong source of random numbers. Do not use it on
 a system where os.urandom() is weak.
 
-== Usage ==
+## Usage
 
 You start by creating a SigningKey. You can use this to sign data, by passing
 in a data string and getting back the signature (also a string). You can also
 ask a SigningKey to give you the corresponding VerifyingKey. The VerifyingKey
 can be used to verify a signature, by passing it both the data string and the
 signature string: it either returns True or raises BadSignatureError.
 
- from ecdsa import SigningKey
- sk = SigningKey.generate() # uses NIST192p
- vk = sk.get_verifying_key()
- signature = sk.sign("message")
- assert sk.verify(signature, "message")
+    from ecdsa import SigningKey
+    sk = SigningKey.generate() # uses NIST192p
+    vk = sk.get_verifying_key()
+    signature = sk.sign("message")
+    assert vk.verify(signature, "message")
 
 Each SigningKey/VerifyingKey is associated with a specific curve, like
 NIST192p (the default one). Longer curves are more secure, but take longer to
 use, and result in longer keys and signatures.
 
- from ecdsa import SigningKey, NIST384p
- sk = SigningKey.generate(curve=NIST384p)
- vk = sk.get_verifying_key()
- signature = sk.sign("message")
- assert sk.verify(signature, "message")
+    from ecdsa import SigningKey, NIST384p
+    sk = SigningKey.generate(curve=NIST384p)
+    vk = sk.get_verifying_key()
+    signature = sk.sign("message")
+    assert vk.verify(signature, "message")
 
 The SigningKey can be serialized into several different formats: the shortest
-is to call s=sk.to_string(), and then re-create it with
-SigningKey.from_string(s, curve) . This short form does not record the curve,
-so you must be sure to tell from_string() the same curve you used for the
-original key. The short form of a NIST192p-based signing key is just 24 bytes
-long.
-
- from ecdsa import SigningKey, NIST384p
- sk = SigningKey.generate(curve=NIST384p)
- sk_string = sk.to_string()
- sk2 = SigningKey.from_string(sk_string, curve=NIST384p)
- # sk and sk2 are the same key
+is to call `s=sk.to_string()`, and then re-create it with
+`SigningKey.from_string(s, curve)` . This short form does not record the
+curve, so you must be sure to tell from_string() the same curve you used for
+the original key. The short form of a NIST192p-based signing key is just 24
+bytes long.
+
+    from ecdsa import SigningKey, NIST384p
+    sk = SigningKey.generate(curve=NIST384p)
+    sk_string = sk.to_string()
+    sk2 = SigningKey.from_string(sk_string, curve=NIST384p)
+    # sk and sk2 are the same key
 
-sk.to_pem() and sk.to_der() will serialize the signing key into the same
+`sk.to_pem()` and `sk.to_der()` will serialize the signing key into the same
 formats that OpenSSL uses. The PEM file looks like the familiar ASCII-armored
-"-----BEGIN EC PRIVATE KEY-----" base64-encoded format, and the DER format is
-a shorter binary form of the same data. SigningKey.from_pem()/.from_der()
-will undo this serialization. These formats include the curve name, so you do
-not need to pass in a curve identifier to the deserializer.
-
- from ecdsa import SigningKey, NIST384p
- sk = SigningKey.generate(curve=NIST384p)
- sk_pem = sk.to_pem()
- sk2 = SigningKey.from_pem(sk_pem)
- # sk and sk2 are the same key
+`"-----BEGIN EC PRIVATE KEY-----"` base64-encoded format, and the DER format
+is a shorter binary form of the same data.
+`SigningKey.from_pem()/.from_der()` will undo this serialization. These
+formats include the curve name, so you do not need to pass in a curve
+identifier to the deserializer.
+
+    from ecdsa import SigningKey, NIST384p
+    sk = SigningKey.generate(curve=NIST384p)
+    sk_pem = sk.to_pem()
+    sk2 = SigningKey.from_pem(sk_pem)
+    # sk and sk2 are the same key
 
 Likewise, the VerifyingKey can be serialized in the same way:
-vk.to_string()/VerifyingKey.from_string(), to_pem()/from_pem(), and
-to_der()/from_der(). The same curve= argument is needed for
-VerifyingKey.from_string().
-
- from ecdsa import SigningKey, VerifyingKey, NIST384p
- sk = SigningKey.generate(curve=NIST384p)
- vk = sk.get_verifying_key()
- vk_string = vk.to_string()
- vk2 = VerifyingKey.from_string(vk_string, curve=NIST384p)
- # vk and vk2 are the same key
-
- from ecdsa import SigningKey, VerifyingKey, NIST384p
- sk = SigningKey.generate(curve=NIST384p)
- vk = sk.get_verifying_key()
- vk_pem = vk.to_pem()
- vk2 = VerifyingKey.from_pem(vk_pem)
- # vk and vk2 are the same key
+`vk.to_string()/VerifyingKey.from_string()`, `to_pem()/from_pem()`, and
+`to_der()/from_der()`. The same curve= argument is needed for
+`VerifyingKey.from_string()`.
+
+    from ecdsa import SigningKey, VerifyingKey, NIST384p
+    sk = SigningKey.generate(curve=NIST384p)
+    vk = sk.get_verifying_key()
+    vk_string = vk.to_string()
+    vk2 = VerifyingKey.from_string(vk_string, curve=NIST384p)
+    # vk and vk2 are the same key
+
+    from ecdsa import SigningKey, VerifyingKey, NIST384p
+    sk = SigningKey.generate(curve=NIST384p)
+    vk = sk.get_verifying_key()
+    vk_pem = vk.to_pem()
+    vk2 = VerifyingKey.from_pem(vk_pem)
+    # vk and vk2 are the same key
 
 There are a couple of different ways to compute a signature. Fundamentally,
 ECDSA takes a number that represents the data being signed, and returns a
 pair of numbers that represent the signature. The hashfunc= argument to
-sk.sign() and vk.verify() is used to turn an arbitrary string into
+`sk.sign()` and `vk.verify()` is used to turn an arbitrary string into
 fixed-length digest, which is then turned into a number that ECDSA can sign,
 and both sign and verify must use the same approach. The default value is
 hashlib.sha1, but if you use NIST256p or a longer curve, you can use
 hashlib.sha256 instead.
 
-There are also multiple ways to represent a signature. The default sk.sign()
-and vk.verify() methods present it as a short string, for simplicity and
-minimal overhead. To use a different scheme, use the sk.sign(sigencode=) and
-vk.verify(sigdecode=) arguments. There are helper funcions in the
-"ecdsa.util" module that can be useful here.
+There are also multiple ways to represent a signature. The default
+`sk.sign()` and `vk.verify()` methods present it as a short string, for
+simplicity and minimal overhead. To use a different scheme, use the
+`sk.sign(sigencode=)` and `vk.verify(sigdecode=)` arguments. There are helper
+funcions in the "ecdsa.util" module that can be useful here.
 
 It is also possible to create a SigningKey from a "seed", which is
 deterministic. This can be used in protocols where you want to derive
 consistent signing keys from some other secret, for example when you want
 three separate keys and only want to store a single master secret. You should
 start with a uniformly-distributed unguessable seed with about curve.baselen
 bytes of entropy, and then use one of the helper functions in ecdsa.util to
 convert it into an integer in the correct range, and then finally pass it
-into SigningKey.from_secret_exponent(), like this:
+into `SigningKey.from_secret_exponent()`, like this:
 
- from pyecdsa import NIST384p, SigningKey
- from pyecdsa.util import randrange_from_seed__trytryagain
+    from pyecdsa import NIST384p, SigningKey
+    from pyecdsa.util import randrange_from_seed__trytryagain
 
- def make_key(seed):
-   secexp = randrange_from_seed__trytryagain(seed, NIST384p.order)
-   return SigningKey.from_secret_exponent(secexp, curve=NIST384p)
-
- seed = os.urandom(NIST384p.baselen) # or other starting point
- sk1a = make_key(seed)
- sk1b = make_key(seed)
- # note: sk1a and sk1b are the same key
- sk2 = make_key("2-"+seed)  # different key
+    def make_key(seed):
+      secexp = randrange_from_seed__trytryagain(seed, NIST384p.order)
+      return SigningKey.from_secret_exponent(secexp, curve=NIST384p)
+
+    seed = os.urandom(NIST384p.baselen) # or other starting point
+    sk1a = make_key(seed)
+    sk1b = make_key(seed)
+    # note: sk1a and sk1b are the same key
+    sk2 = make_key("2-"+seed)  # different key
 
-== OpenSSL Compatibility ==
+## OpenSSL Compatibility
 
 To produce signatures that can be verified by OpenSSL tools, or to verify
 signatures that were produced by those tools, use:
 
- # openssl ecparam -name secp224r1 -genkey -out sk.pem
- # openssl ec -in sk.pem -pubout -out pk.pem
- # openssl dgst -ecdsa-with-SHA1 -sign sk.pem -out data.sig data
- # openssl dgst -ecdsa-with-SHA1 -prverify vk.pem -signature data.sig data
+    # openssl ecparam -name secp224r1 -genkey -out sk.pem
+    # openssl ec -in sk.pem -pubout -out vk.pem
+    # openssl dgst -ecdsa-with-SHA1 -sign sk.pem -out data.sig data
+    # openssl dgst -ecdsa-with-SHA1 -verify vk.pem -signature data.sig data
+    # openssl dgst -ecdsa-with-SHA1 -prverify sk.pem -signature data.sig data
 
- sk.sign(msg, hashfunc=hashlib.sha1, sigencode=ecdsa.util.sigencode_der)
- vk.verify(sig, msg, hashfunc=hashlib.sha1, sigdecode=ecdsa.util.sigdecode_der)
+    sk.sign(msg, hashfunc=hashlib.sha1, sigencode=ecdsa.util.sigencode_der)
+    vk.verify(sig, msg, hashfunc=hashlib.sha1, sigdecode=ecdsa.util.sigdecode_der)
 
 The keys that openssl handles can be read and written as follows:
 
- sk = SigningKey.from_pem(open("sk.pem").read())
- open("sk.pem","w").write(sk.to_pem())
+    sk = SigningKey.from_pem(open("sk.pem").read())
+    open("sk.pem","w").write(sk.to_pem())
 
- vk = VerifyingKey.from_pem(open("vk.pem").read())
- open("vk.pem","w").write(vk.to_pem())
+    vk = VerifyingKey.from_pem(open("vk.pem").read())
+    open("vk.pem","w").write(vk.to_pem())
 
-== Entropy ==
+## Entropy
 
-Creating a signing key with SigningKey.generate() requires some form of
-entropy (as opposed to from_secret_exponent/from_string/from_der/from_pem,
+Creating a signing key with `SigningKey.generate()` requires some form of
+entropy (as opposed to `from_secret_exponent/from_string/from_der/from_pem`,
 which are deterministic and do not require an entropy source). The default
-source is os.urandom(), but you can pass any other function that behaves like
-os.urandom as the entropy= argument to do something different. This may be
-useful in unit tests, where you want to achieve repeatable results. The
+source is `os.urandom()`, but you can pass any other function that behaves
+like os.urandom as the entropy= argument to do something different. This may
+be useful in unit tests, where you want to achieve repeatable results. The
 ecdsa.util.PRNG utility is handy here: it takes a seed and produces a strong
 pseudo-random stream from it:
 
- from ecdsa.util import PRNG
- from ecdsa import SigningKey
- rng1 = PRNG("seed")
- sk1 = SigningKey.generate(entropy=rng1)
- rng2 = PRNG("seed")
- sk2 = SigningKey.generate(entropy=rng2)
- # sk1 and sk2 are the same key
+    from ecdsa.util import PRNG
+    from ecdsa import SigningKey
+    rng1 = PRNG("seed")
+    sk1 = SigningKey.generate(entropy=rng1)
+    rng2 = PRNG("seed")
+    sk2 = SigningKey.generate(entropy=rng2)
+    # sk1 and sk2 are the same key
 
 Likewise, ECDSA signature generation requires a random number, and each
 signature must use a different one (using the same number twice will
-immediately reveal the private signing key). The sk.sign() method takes an
-entropy= argument which behaves the same as SigningKey.generate(entropy=).
+immediately reveal the private signing key). The `sk.sign()` method takes an
+entropy= argument which behaves the same as `SigningKey.generate(entropy=)`.
+
+## Deterministic Signatures
+
+If you call `SigningKey.sign_deterministic(data)` instead of `.sign(data)`,
+the code will generate a deterministic signature instead of a random one.
+This uses the algorithm from RFC6979 to safely generate a unique `k` value,
+derived from the private key and the message being signed. Each time you sign
+the same message with the same key, you will get the same signature (using
+the same `k`).
+
+This may become the default in a future version, as it is not vulnerable to
+failures of the entropy source.
 
-== Examples ==
+## Examples
 
 Create a NIST192p keypair and immediately save both to disk:
 
- from ecdsa import SigningKey
- sk = SigningKey.generate()
- vk = sk.get_verifying_key()
- open("private.pem","w").write(sk.to_pem())
- open("public.pem","w").write(vk.to_pem())
+    from ecdsa import SigningKey
+    sk = SigningKey.generate()
+    vk = sk.get_verifying_key()
+    open("private.pem","w").write(sk.to_pem())
+    open("public.pem","w").write(vk.to_pem())
 
 Load a signing key from disk, use it to sign a message, and write the
 signature to disk:
 
- from ecdsa import SigningKey
- sk = SigningKey.from_pem(open("private.pem").read())
- message = open("message","rb").read()
- sig = sk.sign(message)
- open("signature","wb").write(sig)
+    from ecdsa import SigningKey
+    sk = SigningKey.from_pem(open("private.pem").read())
+    message = open("message","rb").read()
+    sig = sk.sign(message)
+    open("signature","wb").write(sig)
 
 Load the verifying key, message, and signature from disk, and verify the
 signature:
 
- from ecdsa import VerifyingKey, BadSignatureError
- vk = VerifyingKey.from_pem(open("public.pem").read())
- message = open("message","rb").read()
- sig = open("signature","rb").read()
- try:
-   vk.verify(sig, message)
-   print "good signature"
- except BadSignatureError:
-   print "BAD SIGNATURE"
+    from ecdsa import VerifyingKey, BadSignatureError
+    vk = VerifyingKey.from_pem(open("public.pem").read())
+    message = open("message","rb").read()
+    sig = open("signature","rb").read()
+    try:
+      vk.verify(sig, message)
+      print "good signature"
+    except BadSignatureError:
+      print "BAD SIGNATURE"
 
 Create a NIST521p keypair
 
- from ecdsa import SigningKey, NIST521p
- sk = SigningKey.generate(curve=NIST521p)
- vk = sk.get_verifying_key()
+    from ecdsa import SigningKey, NIST521p
+    sk = SigningKey.generate(curve=NIST521p)
+    vk = sk.get_verifying_key()
 
 Create three independent signing keys from a master seed:
 
- from pyecdsa import NIST192p, SigningKey
- from pyecdsa.util import randrange_from_seed__trytryagain
-
- def make_key_from_seed(seed, curve=NIST192p):
-   secexp = randrange_from_seed__trytryagain(seed, curve.order)
-   return SigningKey.from_secret_exponent(secexp, curve)
-
- sk1 = make_key_from_seed("1:%s" % seed)
- sk2 = make_key_from_seed("2:%s" % seed)
- sk3 = make_key_from_seed("3:%s" % seed)
-
-
---footnotes--
-
-[1]: http://www.derkeiler.com/Newsgroups/sci.crypt/2006-01/msg00651.html
-[2]: http://webpages.charter.net/curryfans/peter/downloads.html
+    from pyecdsa import NIST192p, SigningKey
+    from pyecdsa.util import randrange_from_seed__trytryagain
 
+    def make_key_from_seed(seed, curve=NIST192p):
+      secexp = randrange_from_seed__trytryagain(seed, curve.order)
+      return SigningKey.from_secret_exponent(secexp, curve)
+
+    sk1 = make_key_from_seed("1:%s" % seed)
+    sk2 = make_key_from_seed("2:%s" % seed)
+    sk3 = make_key_from_seed("3:%s" % seed)
```

### Comparing `ecdsa-0.8/setup.py` & `ecdsa-0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
-
 import os, subprocess, re
 from distutils.core import setup, Command
 from distutils.command.sdist import sdist as _sdist
+from ecdsa.six import print_
 
 class Test(Command):
     description = "run unit tests"
     user_options = []
     boolean_options = []
     def initialize_options(self):
         pass
@@ -28,34 +28,34 @@
 # version'. Distribution tarballs contain a pre-generated copy of this file.
 
 __version__ = '%s'
 """
 
 def update_version_py():
     if not os.path.isdir(".git"):
-        print "This does not appear to be a Git repository."
+        print_("This does not appear to be a Git repository.")
         return
     try:
         p = subprocess.Popen(["git", "describe",
                               "--tags", "--dirty", "--always"],
                              stdout=subprocess.PIPE)
     except EnvironmentError:
-        print "unable to run git, leaving ecdsa/_version.py alone"
+        print_("unable to run git, leaving ecdsa/_version.py alone")
         return
     stdout = p.communicate()[0]
     if p.returncode != 0:
-        print "unable to run git, leaving ecdsa/_version.py alone"
+        print_("unable to run git, leaving ecdsa/_version.py alone")
         return
     # we use tags like "python-ecdsa-0.5", so strip the prefix
     assert stdout.startswith("python-ecdsa-")
     ver = stdout[len("python-ecdsa-"):].strip()
     f = open("ecdsa/_version.py", "w")
     f.write(VERSION_PY % ver)
     f.close()
-    print "set ecdsa/_version.py to '%s'" % ver
+    print_("set ecdsa/_version.py to '%s'" % ver)
 
 def get_version():
     try:
         f = open("ecdsa/_version.py")
     except EnvironmentError:
         return None
     for line in f.readlines():
@@ -71,15 +71,15 @@
     boolean_options = []
     def initialize_options(self):
         pass
     def finalize_options(self):
         pass
     def run(self):
         update_version_py()
-        print "Version is now", get_version()
+        print_("Version is now", get_version())
 
 class sdist(_sdist):
     def run(self):
         update_version_py()
         # unless we update this, the sdist command will keep using the old
         # version
         self.distribution.metadata.version = get_version()
```

### Comparing `ecdsa-0.8/ecdsa/curves.py` & `ecdsa-0.9/ecdsa/curves.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import der, ecdsa
+from __future__ import division
+
+from . import der, ecdsa
 
 class UnknownCurveError(Exception):
     pass
 
 def orderlen(order):
     return (1+len("%x"%order))//2 # bytes
 
@@ -25,16 +27,19 @@
                  (1, 3, 132, 0, 33))
 NIST256p = Curve("NIST256p", ecdsa.curve_256, ecdsa.generator_256,
                  (1, 2, 840, 10045, 3, 1, 7))
 NIST384p = Curve("NIST384p", ecdsa.curve_384, ecdsa.generator_384,
                  (1, 3, 132, 0, 34))
 NIST521p = Curve("NIST521p", ecdsa.curve_521, ecdsa.generator_521,
                  (1, 3, 132, 0, 35))
+SECP256k1 = Curve("SECP256k1",
+                  ecdsa.curve_secp256k1, ecdsa.generator_secp256k1,
+                  (1, 3, 132, 0, 10))
 
-curves = [NIST192p, NIST224p, NIST256p, NIST384p, NIST521p]
+curves = [NIST192p, NIST224p, NIST256p, NIST384p, NIST521p, SECP256k1]
 
 def find_curve(oid_curve):
     for c in curves:
         if c.oid == oid_curve:
             return c
     raise UnknownCurveError("I don't know about the curve with oid %s."
                             "I only know about these: %s" %
```

### Comparing `ecdsa-0.8/ecdsa/der.py` & `ecdsa-0.9/ecdsa/der.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,89 @@
+from __future__ import division
+
 import binascii
 import base64
+from .six import int2byte, b, PY3, integer_types, text_type
 
 class UnexpectedDER(Exception):
     pass
 
 def encode_constructed(tag, value):
-    return chr(0xa0+tag) + encode_length(len(value)) + value
+    return int2byte(0xa0+tag) + encode_length(len(value)) + value
 def encode_integer(r):
     assert r >= 0 # can't support negative numbers yet
-    h = "%x" % r
-    if len(h)%2:
-        h = "0" + h
+    h = ("%x" % r).encode()
+    if len(h) % 2:
+        h = b("0") + h
     s = binascii.unhexlify(h)
-    if ord(s[0]) <= 0x7f:
-        return "\x02" + chr(len(s)) + s
+    num = s[0] if isinstance(s[0], integer_types) else ord(s[0])
+    if num <= 0x7f:
+        return b("\x02") + int2byte(len(s)) + s
     else:
         # DER integers are two's complement, so if the first byte is
         # 0x80-0xff then we need an extra 0x00 byte to prevent it from
         # looking negative.
-        return "\x02" + chr(len(s)+1) + "\x00" + s
+        return b("\x02") + int2byte(len(s)+1) + b("\x00") + s
 
 def encode_bitstring(s):
-    return "\x03" + encode_length(len(s)) + s
+    return b("\x03") + encode_length(len(s)) + s
 def encode_octet_string(s):
-    return "\x04" + encode_length(len(s)) + s
+    return b("\x04") + encode_length(len(s)) + s
 def encode_oid(first, second, *pieces):
     assert first <= 2
     assert second <= 39
-    encoded_pieces = [chr(40*first+second)] + [encode_number(p)
-                                               for p in pieces]
-    body = "".join(encoded_pieces)
-    return "\x06" + encode_length(len(body)) + body
+    encoded_pieces = [int2byte(40*first+second)] + [encode_number(p)
+                                                    for p in pieces]
+    body = b('').join(encoded_pieces)
+    return b('\x06') + encode_length(len(body)) + body
 def encode_sequence(*encoded_pieces):
     total_len = sum([len(p) for p in encoded_pieces])
-    return "\x30" + encode_length(total_len) + "".join(encoded_pieces)
+    return b('\x30') + encode_length(total_len) + b('').join(encoded_pieces)
 def encode_number(n):
     b128_digits = []
     while n:
         b128_digits.insert(0, (n & 0x7f) | 0x80)
         n = n >> 7
     if not b128_digits:
         b128_digits.append(0)
     b128_digits[-1] &= 0x7f
-    return "".join([chr(d) for d in b128_digits])
+    return b('').join([int2byte(d) for d in b128_digits])
 
 def remove_constructed(string):
-    s0 = ord(string[0])
+    s0 = string[0] if isinstance(string[0], integer_types) else ord(string[0])
     if (s0 & 0xe0) != 0xa0:
         raise UnexpectedDER("wanted constructed tag (0xa0-0xbf), got 0x%02x"
                             % s0)
     tag = s0 & 0x1f
     length, llen = read_length(string[1:])
     body = string[1+llen:1+llen+length]
     rest = string[1+llen+length:]
     return tag, body, rest
 
 def remove_sequence(string):
-    if not string.startswith("\x30"):
-        raise UnexpectedDER("wanted sequence (0x30), got 0x%02x" %
-                            ord(string[0]))
+    if not string.startswith(b("\x30")):
+        n = string[0] if isinstance(string[0], integer_types) else ord(string[0])
+        raise UnexpectedDER("wanted sequence (0x30), got 0x%02x" % n)
     length, lengthlength = read_length(string[1:])
     endseq = 1+lengthlength+length
     return string[1+lengthlength:endseq], string[endseq:]
 
 def remove_octet_string(string):
-    if not string.startswith("\x04"):
-        raise UnexpectedDER("wanted octetstring (0x04), got 0x%02x" %
-                            ord(string[0]))
+    if not string.startswith(b("\x04")):
+        n = string[0] if isinstance(string[0], integer_types) else ord(string[0])
+        raise UnexpectedDER("wanted octetstring (0x04), got 0x%02x" % n)
     length, llen = read_length(string[1:])
     body = string[1+llen:1+llen+length]
     rest = string[1+llen+length:]
     return body, rest
 
 def remove_object(string):
-    if not string.startswith("\x06"):
-        raise UnexpectedDER("wanted object (0x06), got 0x%02x" %
-                            ord(string[0]))
+    if not string.startswith(b("\x06")):
+        n = string[0] if isinstance(string[0], integer_types) else ord(string[0])
+        raise UnexpectedDER("wanted object (0x06), got 0x%02x" % n)
     length, lengthlength = read_length(string[1:])
     body = string[1+lengthlength:1+lengthlength+length]
     rest = string[1+lengthlength+length:]
     numbers = []
     while body:
         n, ll = read_number(body)
         numbers.append(n)
@@ -88,64 +92,66 @@
     first = n0//40
     second = n0-(40*first)
     numbers.insert(0, first)
     numbers.insert(1, second)
     return tuple(numbers), rest
 
 def remove_integer(string):
-    if not string.startswith("\x02"):
-        raise UnexpectedDER("wanted integer (0x02), got 0x%02x" %
-                            ord(string[0]))
+    if not string.startswith(b("\x02")):
+        n = string[0] if isinstance(string[0], integer_types) else ord(string[0])
+        raise UnexpectedDER("wanted integer (0x02), got 0x%02x" % n)
     length, llen = read_length(string[1:])
     numberbytes = string[1+llen:1+llen+length]
     rest = string[1+llen+length:]
-    assert ord(numberbytes[0]) < 0x80 # can't support negative numbers yet
+    nbytes = numberbytes[0] if isinstance(numberbytes[0], integer_types) else ord(numberbytes[0])
+    assert nbytes < 0x80 # can't support negative numbers yet
     return int(binascii.hexlify(numberbytes), 16), rest
 
 def read_number(string):
     number = 0
     llen = 0
     # base-128 big endian, with b7 set in all but the last byte
     while True:
         if llen > len(string):
             raise UnexpectedDER("ran out of length bytes")
         number = number << 7
-        d = ord(string[llen])
+        d = string[llen] if isinstance(string[llen], integer_types) else ord(string[llen])
         number += (d & 0x7f)
         llen += 1
         if not d & 0x80:
             break
     return number, llen
 
 def encode_length(l):
     assert l >= 0
     if l < 0x80:
-        return chr(l)
-    s = "%x" % l
+        return int2byte(l)
+    s = ("%x" % l).encode()
     if len(s)%2:
-        s = "0"+s
+        s = b("0")+s
     s = binascii.unhexlify(s)
     llen = len(s)
-    return chr(0x80|llen) + s
+    return int2byte(0x80|llen) + s
 
 def read_length(string):
-    if not (ord(string[0]) & 0x80):
+    num = string[0] if isinstance(string[0], integer_types) else ord(string[0])
+    if not (num & 0x80):
         # short form
-        return (ord(string[0]) & 0x7f), 1
+        return (num & 0x7f), 1
     # else long-form: b0&0x7f is number of additional base256 length bytes,
     # big-endian
-    llen = ord(string[0]) & 0x7f
+    llen = num & 0x7f
     if llen > len(string)-1:
         raise UnexpectedDER("ran out of length bytes")
     return int(binascii.hexlify(string[1:1+llen]), 16), 1+llen
 
 def remove_bitstring(string):
-    if not string.startswith("\x03"):
-        raise UnexpectedDER("wanted bitstring (0x03), got 0x%02x" %
-                            ord(string[0]))
+    num = string[0] if isinstance(string[0], integer_types) else ord(string[0])
+    if not string.startswith(b("\x03")):
+        raise UnexpectedDER("wanted bitstring (0x03), got 0x%02x" % num)
     length, llen = read_length(string[1:])
     body = string[1+llen:1+llen+length]
     rest = string[1+llen+length:]
     return body, rest
 
 # SEQUENCE([1, STRING(secexp), cont[0], OBJECT(curvename), cont[1], BINTSTRING)
 
@@ -173,18 +179,21 @@
 #  secp224r1 OBJECT IDENTIFIER ::= {
 #  iso(1) identified-organization(3) certicom(132) curve(0) 33 }
 # and the secp384r1 is (t=06,l=05,v=2b81040022)
 #  secp384r1 OBJECT IDENTIFIER ::= {
 #  iso(1) identified-organization(3) certicom(132) curve(0) 34 }
 
 def unpem(pem):
-    d = "".join([l.strip() for l in pem.split("\n")
-                 if l and not l.startswith("-----")])
+    if isinstance(pem, text_type):
+        pem = pem.encode()
+
+    d = b("").join([l.strip() for l in pem.split(b("\n"))
+                    if l and not l.startswith(b("-----"))])
     return base64.b64decode(d)
 def topem(der, name):
     b64 = base64.b64encode(der)
-    lines = ["-----BEGIN %s-----\n" % name]
-    lines.extend([b64[start:start+64]+"\n"
+    lines = [("-----BEGIN %s-----\n" % name).encode()]
+    lines.extend([b64[start:start+64]+b("\n")
                   for start in range(0, len(b64), 64)])
-    lines.append("-----END %s-----\n" % name)
-    return "".join(lines)
+    lines.append(("-----END %s-----\n" % name).encode())
+    return b("").join(lines)
```

### Comparing `ecdsa-0.8/ecdsa/ecdsa.py` & `ecdsa-0.9/ecdsa/ecdsa.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #! /usr/bin/env python
+
 """
 Implementation of Elliptic-Curve Digital Signatures.
 
 Classes and methods for elliptic-curve signatures:
 private keys, public keys, signatures,
 NIST prime-modulus curves with modulus lengths of
 192, 224, 256, 384, and 521 bits.
@@ -19,46 +20,46 @@
   g = generator_192
   n = g.order()
   secret = randrange( 1, n )
   pubkey = Public_key( g, g * secret )
   privkey = Private_key( pubkey, secret )
 
   # Signing a hash value:
- 
+
   hash = randrange( 1, n )
   signature = privkey.sign( hash, randrange( 1, n ) )
 
   # Verifying a signature for a hash value:
 
   if pubkey.verifies( hash, signature ):
-    print "Demo verification succeeded."
+    print_("Demo verification succeeded.")
   else:
-    print "*** Demo verification failed."
+    print_("*** Demo verification failed.")
 
   # Verification fails if the hash value is modified:
 
   if pubkey.verifies( hash-1, signature ):
-    print "**** Demo verification failed to reject tampered hash."
+    print_("**** Demo verification failed to reject tampered hash.")
   else:
-    print "Demo verification correctly rejected tampered hash."
+    print_("Demo verification correctly rejected tampered hash.")
 
 Version of 2009.05.16.
 
 Revision history:
       2005.12.31 - Initial version.
       2008.11.25 - Substantial revisions introducing new classes.
       2009.05.16 - Warn against using random.randrange in real applications.
       2009.05.17 - Use random.SystemRandom by default.
 
 Written in 2005 by Peter Pearson and placed in the public domain.
 """
 
-
-import ellipticcurve
-import numbertheory
+from .six import int2byte, b, print_
+from . import ellipticcurve
+from . import numbertheory
 import random
 
 
 
 class Signature( object ):
   """ECDSA signature.
   """
@@ -72,25 +73,25 @@
   """Public key for ECDSA.
   """
 
   def __init__( self, generator, point ):
     """generator is the Point that generates the group,
     point is the Point that defines the public key.
     """
-    
+
     self.curve = generator.curve()
     self.generator = generator
     self.point = point
     n = generator.order()
     if not n:
-      raise RuntimeError, "Generator point must have order."
+      raise RuntimeError("Generator point must have order.")
     if not n * point == ellipticcurve.INFINITY:
-      raise RuntimeError, "Generator point order is bad."
+      raise RuntimeError("Generator point order is bad.")
     if point.x() < 0 or n <= point.x() or point.y() < 0 or n <= point.y():
-      raise RuntimeError, "Generator point has x or y out of range."
+      raise RuntimeError("Generator point has x or y out of range.")
 
 
   def verifies( self, hash, signature ):
     """Verify that signature is a valid signature of hash.
     Return True if the signature is valid.
     """
 
@@ -104,26 +105,26 @@
     if s < 1 or s > n-1: return False
     c = numbertheory.inverse_mod( s, n )
     u1 = ( hash * c ) % n
     u2 = ( r * c ) % n
     xy = u1 * G + u2 * self.point
     v = xy.x() % n
     return v == r
-    
+
 
 
 class Private_key( object ):
   """Private key for ECDSA.
   """
 
   def __init__( self, public_key, secret_multiplier ):
     """public_key is of class Public_key;
     secret_multiplier is a large integer.
     """
-    
+
     self.public_key = public_key
     self.secret_multiplier = secret_multiplier
 
   def sign( self, hash, random_k ):
     """Return a signature for the provided hash, using the provided
     random nonce.  It is absolutely vital that random_k be an unpredictable
     number in the range [1, self.public_key.point.order()-1].  If
@@ -139,38 +140,42 @@
     """
 
     G = self.public_key.generator
     n = G.order()
     k = random_k % n
     p1 = k * G
     r = p1.x()
-    if r == 0: raise RuntimeError, "amazingly unlucky random number r"
+    if r == 0: raise RuntimeError("amazingly unlucky random number r")
     s = ( numbertheory.inverse_mod( k, n ) * \
           ( hash + ( self.secret_multiplier * r ) % n ) ) % n
-    if s == 0: raise RuntimeError, "amazingly unlucky random number s"
+    if s == 0: raise RuntimeError("amazingly unlucky random number s")
     return Signature( r, s )
 
 
 
 def int_to_string( x ):
   """Convert integer x into a string of bytes, as per X9.62."""
   assert x >= 0
-  if x == 0: return chr(0)
-  result = ""
-  while x > 0:
-    q, r = divmod( x, 256 )
-    result = chr( r ) + result
-    x = q
-  return result
+  if x == 0: return b('\0')
+  result = []
+  while x:
+    ordinal = x & 0xFF
+    result.append(int2byte(ordinal))
+    x >>= 8
+
+  result.reverse()
+  return b('').join(result)
 
 
 def string_to_int( s ):
   """Convert a string of bytes into an integer, as per X9.62."""
-  result = 0L
-  for c in s: result = 256 * result + ord( c )
+  result = 0
+  for c in s:
+    if not isinstance(c, int): c = ord( c )
+    result = 256 * result + c
   return result
 
 
 def digest_integer( m ):
   """Convert an integer into a string of bytes, compute
      its SHA-1 hash, and convert the result to an integer."""
   #
@@ -197,364 +202,375 @@
      ellipticcurve.INFINITY:
     return False
   return True
 
 
 
 # NIST Curve P-192:
-_p = 6277101735386680763835789423207666416083908700390324961279L
-_r = 6277101735386680763835789423176059013767194773182842284081L
+_p = 6277101735386680763835789423207666416083908700390324961279
+_r = 6277101735386680763835789423176059013767194773182842284081
 # s = 0x3045ae6fc8422f64ed579528d38120eae12196d5L
 # c = 0x3099d2bbbfcb2538542dcd5fb078b6ef5f3d6fe2c745de65L
-_b = 0x64210519e59c80e70fa7e9ab72243049feb8deecc146b9b1L
-_Gx = 0x188da80eb03090f67cbf20eb43a18800f4ff0afd82ff1012L
-_Gy = 0x07192b95ffc8da78631011ed6b24cdd573f977a11e794811L
+_b = 0x64210519e59c80e70fa7e9ab72243049feb8deecc146b9b1
+_Gx = 0x188da80eb03090f67cbf20eb43a18800f4ff0afd82ff1012
+_Gy = 0x07192b95ffc8da78631011ed6b24cdd573f977a11e794811
 
 curve_192 = ellipticcurve.CurveFp( _p, -3, _b )
 generator_192 = ellipticcurve.Point( curve_192, _Gx, _Gy, _r )
 
 
 # NIST Curve P-224:
-_p = 26959946667150639794667015087019630673557916260026308143510066298881L
-_r = 26959946667150639794667015087019625940457807714424391721682722368061L
+_p = 26959946667150639794667015087019630673557916260026308143510066298881
+_r = 26959946667150639794667015087019625940457807714424391721682722368061
 # s = 0xbd71344799d5c7fcdc45b59fa3b9ab8f6a948bc5L
 # c = 0x5b056c7e11dd68f40469ee7f3c7a7d74f7d121116506d031218291fbL
-_b = 0xb4050a850c04b3abf54132565044b0b7d7bfd8ba270b39432355ffb4L
-_Gx =0xb70e0cbd6bb4bf7f321390b94a03c1d356c21122343280d6115c1d21L
-_Gy = 0xbd376388b5f723fb4c22dfe6cd4375a05a07476444d5819985007e34L
+_b = 0xb4050a850c04b3abf54132565044b0b7d7bfd8ba270b39432355ffb4
+_Gx =0xb70e0cbd6bb4bf7f321390b94a03c1d356c21122343280d6115c1d21
+_Gy = 0xbd376388b5f723fb4c22dfe6cd4375a05a07476444d5819985007e34
 
 curve_224 = ellipticcurve.CurveFp( _p, -3, _b )
 generator_224 = ellipticcurve.Point( curve_224, _Gx, _Gy, _r )
 
 # NIST Curve P-256:
-_p = 115792089210356248762697446949407573530086143415290314195533631308867097853951L
-_r = 115792089210356248762697446949407573529996955224135760342422259061068512044369L
+_p = 115792089210356248762697446949407573530086143415290314195533631308867097853951
+_r = 115792089210356248762697446949407573529996955224135760342422259061068512044369
 # s = 0xc49d360886e704936a6678e1139d26b7819f7e90L
 # c = 0x7efba1662985be9403cb055c75d4f7e0ce8d84a9c5114abcaf3177680104fa0dL
-_b = 0x5ac635d8aa3a93e7b3ebbd55769886bc651d06b0cc53b0f63bce3c3e27d2604bL
-_Gx = 0x6b17d1f2e12c4247f8bce6e563a440f277037d812deb33a0f4a13945d898c296L
-_Gy = 0x4fe342e2fe1a7f9b8ee7eb4a7c0f9e162bce33576b315ececbb6406837bf51f5L
+_b = 0x5ac635d8aa3a93e7b3ebbd55769886bc651d06b0cc53b0f63bce3c3e27d2604b
+_Gx = 0x6b17d1f2e12c4247f8bce6e563a440f277037d812deb33a0f4a13945d898c296
+_Gy = 0x4fe342e2fe1a7f9b8ee7eb4a7c0f9e162bce33576b315ececbb6406837bf51f5
 
 curve_256 = ellipticcurve.CurveFp( _p, -3, _b )
 generator_256 = ellipticcurve.Point( curve_256, _Gx, _Gy, _r )
 
 # NIST Curve P-384:
-_p = 39402006196394479212279040100143613805079739270465446667948293404245721771496870329047266088258938001861606973112319L
-_r = 39402006196394479212279040100143613805079739270465446667946905279627659399113263569398956308152294913554433653942643L
+_p = 39402006196394479212279040100143613805079739270465446667948293404245721771496870329047266088258938001861606973112319
+_r = 39402006196394479212279040100143613805079739270465446667946905279627659399113263569398956308152294913554433653942643
 # s = 0xa335926aa319a27a1d00896a6773a4827acdac73L
 # c = 0x79d1e655f868f02fff48dcdee14151ddb80643c1406d0ca10dfe6fc52009540a495e8042ea5f744f6e184667cc722483L
-_b = 0xb3312fa7e23ee7e4988e056be3f82d19181d9c6efe8141120314088f5013875ac656398d8a2ed19d2a85c8edd3ec2aefL
-_Gx = 0xaa87ca22be8b05378eb1c71ef320ad746e1d3b628ba79b9859f741e082542a385502f25dbf55296c3a545e3872760ab7L
-_Gy = 0x3617de4a96262c6f5d9e98bf9292dc29f8f41dbd289a147ce9da3113b5f0b8c00a60b1ce1d7e819d7a431d7c90ea0e5fL
+_b = 0xb3312fa7e23ee7e4988e056be3f82d19181d9c6efe8141120314088f5013875ac656398d8a2ed19d2a85c8edd3ec2aef
+_Gx = 0xaa87ca22be8b05378eb1c71ef320ad746e1d3b628ba79b9859f741e082542a385502f25dbf55296c3a545e3872760ab7
+_Gy = 0x3617de4a96262c6f5d9e98bf9292dc29f8f41dbd289a147ce9da3113b5f0b8c00a60b1ce1d7e819d7a431d7c90ea0e5f
 
 curve_384 = ellipticcurve.CurveFp( _p, -3, _b )
 generator_384 = ellipticcurve.Point( curve_384, _Gx, _Gy, _r )
 
 # NIST Curve P-521:
-_p = 6864797660130609714981900799081393217269435300143305409394463459185543183397656052122559640661454554977296311391480858037121987999716643812574028291115057151L
-_r = 6864797660130609714981900799081393217269435300143305409394463459185543183397655394245057746333217197532963996371363321113864768612440380340372808892707005449L
+_p = 6864797660130609714981900799081393217269435300143305409394463459185543183397656052122559640661454554977296311391480858037121987999716643812574028291115057151
+_r = 6864797660130609714981900799081393217269435300143305409394463459185543183397655394245057746333217197532963996371363321113864768612440380340372808892707005449
 # s = 0xd09e8800291cb85396cc6717393284aaa0da64baL
 # c = 0x0b48bfa5f420a34949539d2bdfc264eeeeb077688e44fbf0ad8f6d0edb37bd6b533281000518e19f1b9ffbe0fe9ed8a3c2200b8f875e523868c70c1e5bf55bad637L
-_b = 0x051953eb9618e1c9a1f929a21a0b68540eea2da725b99b315f3b8b489918ef109e156193951ec7e937b1652c0bd3bb1bf073573df883d2c34f1ef451fd46b503f00L
-_Gx = 0xc6858e06b70404e9cd9e3ecb662395b4429c648139053fb521f828af606b4d3dbaa14b5e77efe75928fe1dc127a2ffa8de3348b3c1856a429bf97e7e31c2e5bd66L
-_Gy = 0x11839296a789a3bc0045c8a5fb42c7d1bd998f54449579b446817afbd17273e662c97ee72995ef42640c550b9013fad0761353c7086a272c24088be94769fd16650L
+_b = 0x051953eb9618e1c9a1f929a21a0b68540eea2da725b99b315f3b8b489918ef109e156193951ec7e937b1652c0bd3bb1bf073573df883d2c34f1ef451fd46b503f00
+_Gx = 0xc6858e06b70404e9cd9e3ecb662395b4429c648139053fb521f828af606b4d3dbaa14b5e77efe75928fe1dc127a2ffa8de3348b3c1856a429bf97e7e31c2e5bd66
+_Gy = 0x11839296a789a3bc0045c8a5fb42c7d1bd998f54449579b446817afbd17273e662c97ee72995ef42640c550b9013fad0761353c7086a272c24088be94769fd16650
 
 curve_521 = ellipticcurve.CurveFp( _p, -3, _b )
 generator_521 = ellipticcurve.Point( curve_521, _Gx, _Gy, _r )
 
-  
+# Certicom secp256-k1
+_a  = 0x0000000000000000000000000000000000000000000000000000000000000000
+_b  = 0x0000000000000000000000000000000000000000000000000000000000000007
+_p  = 0xfffffffffffffffffffffffffffffffffffffffffffffffffffffffefffffc2f
+_Gx = 0x79be667ef9dcbbac55a06295ce870b07029bfcdb2dce28d959f2815b16f81798
+_Gy = 0x483ada7726a3c4655da4fbfc0e1108a8fd17b448a68554199c47d08ffb10d4b8
+_r  = 0xfffffffffffffffffffffffffffffffebaaedce6af48a03bbfd25e8cd0364141
+
+curve_secp256k1 = ellipticcurve.CurveFp( _p, _a, _b)
+generator_secp256k1 = ellipticcurve.Point( curve_secp256k1, _Gx, _Gy, _r)
+
+
 
 def __main__():
   class TestFailure(Exception): pass
 
   def test_point_validity( generator, x, y, expected ):
     """generator defines the curve; is (x,y) a point on
        this curve? "expected" is True if the right answer is Yes."""
     if point_is_valid( generator, x, y ) == expected:
-      print "Point validity tested as expected."
+      print_("Point validity tested as expected.")
     else:
       raise TestFailure("*** Point validity test gave wrong result.")
 
   def test_signature_validity( Msg, Qx, Qy, R, S, expected ):
     """Msg = message, Qx and Qy represent the base point on
        elliptic curve c192, R and S are the signature, and
        "expected" is True iff the signature is expected to be valid."""
     pubk = Public_key( generator_192,
                        ellipticcurve.Point( curve_192, Qx, Qy ) )
     got = pubk.verifies( digest_integer( Msg ), Signature( R, S ) )
     if got == expected:
-      print "Signature tested as expected: got %s, expected %s." % \
-            ( got, expected )
+      print_("Signature tested as expected: got %s, expected %s." % \
+            ( got, expected ))
     else:
       raise TestFailure("*** Signature test failed: got %s, expected %s." % \
                         ( got, expected ))
 
-  print "NIST Curve P-192:"
+  print_("NIST Curve P-192:")
 
   p192 = generator_192
 
   # From X9.62:
 
-  d = 651056770906015076056810763456358567190100156695615665659L
+  d = 651056770906015076056810763456358567190100156695615665659
   Q = d * p192
-  if Q.x() != 0x62B12D60690CDCF330BABAB6E69763B471F994DD702D16A5L:
+  if Q.x() != 0x62B12D60690CDCF330BABAB6E69763B471F994DD702D16A5:
     raise TestFailure("*** p192 * d came out wrong.")
   else:
-    print "p192 * d came out right."
+    print_("p192 * d came out right.")
 
-  k = 6140507067065001063065065565667405560006161556565665656654L
+  k = 6140507067065001063065065565667405560006161556565665656654
   R = k * p192
-  if R.x() != 0x885052380FF147B734C330C43D39B2C4A89F29B0F749FEADL \
-     or R.y() != 0x9CF9FA1CBEFEFB917747A3BB29C072B9289C2547884FD835L:
+  if R.x() != 0x885052380FF147B734C330C43D39B2C4A89F29B0F749FEAD \
+     or R.y() != 0x9CF9FA1CBEFEFB917747A3BB29C072B9289C2547884FD835:
     raise TestFailure("*** k * p192 came out wrong.")
   else:
-    print "k * p192 came out right."
+    print_("k * p192 came out right.")
 
-  u1 = 2563697409189434185194736134579731015366492496392189760599L
-  u2 = 6266643813348617967186477710235785849136406323338782220568L
+  u1 = 2563697409189434185194736134579731015366492496392189760599
+  u2 = 6266643813348617967186477710235785849136406323338782220568
   temp = u1 * p192 + u2 * Q
-  if temp.x() != 0x885052380FF147B734C330C43D39B2C4A89F29B0F749FEADL \
-     or temp.y() != 0x9CF9FA1CBEFEFB917747A3BB29C072B9289C2547884FD835L:
+  if temp.x() != 0x885052380FF147B734C330C43D39B2C4A89F29B0F749FEAD \
+     or temp.y() != 0x9CF9FA1CBEFEFB917747A3BB29C072B9289C2547884FD835:
     raise TestFailure("*** u1 * p192 + u2 * Q came out wrong.")
   else:
-    print "u1 * p192 + u2 * Q came out right."
+    print_("u1 * p192 + u2 * Q came out right.")
 
-  e = 968236873715988614170569073515315707566766479517L
+  e = 968236873715988614170569073515315707566766479517
   pubk = Public_key( generator_192, generator_192 * d )
   privk = Private_key( pubk, d )
   sig = privk.sign( e, k )
   r, s = sig.r, sig.s
-  if r != 3342403536405981729393488334694600415596881826869351677613L \
-     or s != 5735822328888155254683894997897571951568553642892029982342L:
+  if r != 3342403536405981729393488334694600415596881826869351677613 \
+     or s != 5735822328888155254683894997897571951568553642892029982342:
     raise TestFailure("*** r or s came out wrong.")
   else:
-    print "r and s came out right."
+    print_("r and s came out right.")
 
   valid = pubk.verifies( e, sig )
-  if valid: print "Signature verified OK."
+  if valid: print_("Signature verified OK.")
   else: raise TestFailure("*** Signature failed verification.")
 
   valid = pubk.verifies( e-1, sig )
-  if not valid: print "Forgery was correctly rejected."
+  if not valid: print_("Forgery was correctly rejected.")
   else: raise TestFailure("*** Forgery was erroneously accepted.")
 
-  print "Testing point validity, as per ECDSAVS.pdf B.2.2:"
+  print_("Testing point validity, as per ECDSAVS.pdf B.2.2:")
 
   test_point_validity( \
     p192, \
-    0xcd6d0f029a023e9aaca429615b8f577abee685d8257cc83aL, \
-    0x00019c410987680e9fb6c0b6ecc01d9a2647c8bae27721bacdfcL, \
+    0xcd6d0f029a023e9aaca429615b8f577abee685d8257cc83a, \
+    0x00019c410987680e9fb6c0b6ecc01d9a2647c8bae27721bacdfc, \
     False )
 
   test_point_validity(
     p192, \
-    0x00017f2fce203639e9eaf9fb50b81fc32776b30e3b02af16c73bL, \
-    0x95da95c5e72dd48e229d4748d4eee658a9a54111b23b2adbL, \
+    0x00017f2fce203639e9eaf9fb50b81fc32776b30e3b02af16c73b, \
+    0x95da95c5e72dd48e229d4748d4eee658a9a54111b23b2adb, \
     False )
 
   test_point_validity(
     p192, \
-    0x4f77f8bc7fccbadd5760f4938746d5f253ee2168c1cf2792L, \
-    0x000147156ff824d131629739817edb197717c41aab5c2a70f0f6L, \
+    0x4f77f8bc7fccbadd5760f4938746d5f253ee2168c1cf2792, \
+    0x000147156ff824d131629739817edb197717c41aab5c2a70f0f6, \
     False )
 
   test_point_validity(
     p192, \
-    0xc58d61f88d905293bcd4cd0080bcb1b7f811f2ffa41979f6L, \
-    0x8804dc7a7c4c7f8b5d437f5156f3312ca7d6de8a0e11867fL, \
+    0xc58d61f88d905293bcd4cd0080bcb1b7f811f2ffa41979f6, \
+    0x8804dc7a7c4c7f8b5d437f5156f3312ca7d6de8a0e11867f, \
     True )
 
   test_point_validity(
     p192, \
-    0xcdf56c1aa3d8afc53c521adf3ffb96734a6a630a4a5b5a70L, \
-    0x97c1c44a5fb229007b5ec5d25f7413d170068ffd023caa4eL, \
+    0xcdf56c1aa3d8afc53c521adf3ffb96734a6a630a4a5b5a70, \
+    0x97c1c44a5fb229007b5ec5d25f7413d170068ffd023caa4e, \
     True )
 
   test_point_validity(
     p192, \
-    0x89009c0dc361c81e99280c8e91df578df88cdf4b0cdedcedL, \
-    0x27be44a529b7513e727251f128b34262a0fd4d8ec82377b9L, \
+    0x89009c0dc361c81e99280c8e91df578df88cdf4b0cdedced, \
+    0x27be44a529b7513e727251f128b34262a0fd4d8ec82377b9, \
     True )
 
   test_point_validity(
     p192, \
-    0x6a223d00bd22c52833409a163e057e5b5da1def2a197dd15L, \
-    0x7b482604199367f1f303f9ef627f922f97023e90eae08abfL, \
+    0x6a223d00bd22c52833409a163e057e5b5da1def2a197dd15, \
+    0x7b482604199367f1f303f9ef627f922f97023e90eae08abf, \
     True )
-  
+
   test_point_validity(
     p192, \
-    0x6dccbde75c0948c98dab32ea0bc59fe125cf0fb1a3798edaL, \
-    0x0001171a3e0fa60cf3096f4e116b556198de430e1fbd330c8835L, \
+    0x6dccbde75c0948c98dab32ea0bc59fe125cf0fb1a3798eda, \
+    0x0001171a3e0fa60cf3096f4e116b556198de430e1fbd330c8835, \
     False )
-  
+
   test_point_validity(
     p192, \
-    0xd266b39e1f491fc4acbbbc7d098430931cfa66d55015af12L, \
-    0x193782eb909e391a3148b7764e6b234aa94e48d30a16dbb2L, \
+    0xd266b39e1f491fc4acbbbc7d098430931cfa66d55015af12, \
+    0x193782eb909e391a3148b7764e6b234aa94e48d30a16dbb2, \
     False )
-  
+
   test_point_validity(
     p192, \
-    0x9d6ddbcd439baa0c6b80a654091680e462a7d1d3f1ffeb43L, \
-    0x6ad8efc4d133ccf167c44eb4691c80abffb9f82b932b8caaL, \
+    0x9d6ddbcd439baa0c6b80a654091680e462a7d1d3f1ffeb43, \
+    0x6ad8efc4d133ccf167c44eb4691c80abffb9f82b932b8caa, \
     False )
-  
+
   test_point_validity(
     p192, \
-    0x146479d944e6bda87e5b35818aa666a4c998a71f4e95edbcL, \
-    0xa86d6fe62bc8fbd88139693f842635f687f132255858e7f6L, \
+    0x146479d944e6bda87e5b35818aa666a4c998a71f4e95edbc, \
+    0xa86d6fe62bc8fbd88139693f842635f687f132255858e7f6, \
     False )
-  
+
   test_point_validity(
     p192, \
-    0xe594d4a598046f3598243f50fd2c7bd7d380edb055802253L, \
-    0x509014c0c4d6b536e3ca750ec09066af39b4c8616a53a923L, \
+    0xe594d4a598046f3598243f50fd2c7bd7d380edb055802253, \
+    0x509014c0c4d6b536e3ca750ec09066af39b4c8616a53a923, \
     False )
 
-  print "Trying signature-verification tests from ECDSAVS.pdf B.2.4:"
-  print "P-192:"
-  Msg = 0x84ce72aa8699df436059f052ac51b6398d2511e49631bcb7e71f89c499b9ee425dfbc13a5f6d408471b054f2655617cbbaf7937b7c80cd8865cf02c8487d30d2b0fbd8b2c4e102e16d828374bbc47b93852f212d5043c3ea720f086178ff798cc4f63f787b9c2e419efa033e7644ea7936f54462dc21a6c4580725f7f0e7d158L
-  Qx = 0xd9dbfb332aa8e5ff091e8ce535857c37c73f6250ffb2e7acL
-  Qy = 0x282102e364feded3ad15ddf968f88d8321aa268dd483ebc4L
-  R = 0x64dca58a20787c488d11d6dd96313f1b766f2d8efe122916L
-  S = 0x1ecba28141e84ab4ecad92f56720e2cc83eb3d22dec72479L
+  print_("Trying signature-verification tests from ECDSAVS.pdf B.2.4:")
+  print_("P-192:")
+  Msg = 0x84ce72aa8699df436059f052ac51b6398d2511e49631bcb7e71f89c499b9ee425dfbc13a5f6d408471b054f2655617cbbaf7937b7c80cd8865cf02c8487d30d2b0fbd8b2c4e102e16d828374bbc47b93852f212d5043c3ea720f086178ff798cc4f63f787b9c2e419efa033e7644ea7936f54462dc21a6c4580725f7f0e7d158
+  Qx = 0xd9dbfb332aa8e5ff091e8ce535857c37c73f6250ffb2e7ac
+  Qy = 0x282102e364feded3ad15ddf968f88d8321aa268dd483ebc4
+  R = 0x64dca58a20787c488d11d6dd96313f1b766f2d8efe122916
+  S = 0x1ecba28141e84ab4ecad92f56720e2cc83eb3d22dec72479
   test_signature_validity( Msg, Qx, Qy, R, S, True )
 
-  Msg = 0x94bb5bacd5f8ea765810024db87f4224ad71362a3c28284b2b9f39fab86db12e8beb94aae899768229be8fdb6c4f12f28912bb604703a79ccff769c1607f5a91450f30ba0460d359d9126cbd6296be6d9c4bb96c0ee74cbb44197c207f6db326ab6f5a659113a9034e54be7b041ced9dcf6458d7fb9cbfb2744d999f7dfd63f4L
-  Qx = 0x3e53ef8d3112af3285c0e74842090712cd324832d4277ae7L
-  Qy = 0xcc75f8952d30aec2cbb719fc6aa9934590b5d0ff5a83adb7L
-  R = 0x8285261607283ba18f335026130bab31840dcfd9c3e555afL
-  S = 0x356d89e1b04541afc9704a45e9c535ce4a50929e33d7e06cL
+  Msg = 0x94bb5bacd5f8ea765810024db87f4224ad71362a3c28284b2b9f39fab86db12e8beb94aae899768229be8fdb6c4f12f28912bb604703a79ccff769c1607f5a91450f30ba0460d359d9126cbd6296be6d9c4bb96c0ee74cbb44197c207f6db326ab6f5a659113a9034e54be7b041ced9dcf6458d7fb9cbfb2744d999f7dfd63f4
+  Qx = 0x3e53ef8d3112af3285c0e74842090712cd324832d4277ae7
+  Qy = 0xcc75f8952d30aec2cbb719fc6aa9934590b5d0ff5a83adb7
+  R = 0x8285261607283ba18f335026130bab31840dcfd9c3e555af
+  S = 0x356d89e1b04541afc9704a45e9c535ce4a50929e33d7e06c
   test_signature_validity( Msg, Qx, Qy, R, S, True )
 
-  Msg = 0xf6227a8eeb34afed1621dcc89a91d72ea212cb2f476839d9b4243c66877911b37b4ad6f4448792a7bbba76c63bdd63414b6facab7dc71c3396a73bd7ee14cdd41a659c61c99b779cecf07bc51ab391aa3252386242b9853ea7da67fd768d303f1b9b513d401565b6f1eb722dfdb96b519fe4f9bd5de67ae131e64b40e78c42ddL
-  Qx = 0x16335dbe95f8e8254a4e04575d736befb258b8657f773cb7L
-  Qy = 0x421b13379c59bc9dce38a1099ca79bbd06d647c7f6242336L
-  R = 0x4141bd5d64ea36c5b0bd21ef28c02da216ed9d04522b1e91L
-  S = 0x159a6aa852bcc579e821b7bb0994c0861fb08280c38daa09L
+  Msg = 0xf6227a8eeb34afed1621dcc89a91d72ea212cb2f476839d9b4243c66877911b37b4ad6f4448792a7bbba76c63bdd63414b6facab7dc71c3396a73bd7ee14cdd41a659c61c99b779cecf07bc51ab391aa3252386242b9853ea7da67fd768d303f1b9b513d401565b6f1eb722dfdb96b519fe4f9bd5de67ae131e64b40e78c42dd
+  Qx = 0x16335dbe95f8e8254a4e04575d736befb258b8657f773cb7
+  Qy = 0x421b13379c59bc9dce38a1099ca79bbd06d647c7f6242336
+  R = 0x4141bd5d64ea36c5b0bd21ef28c02da216ed9d04522b1e91
+  S = 0x159a6aa852bcc579e821b7bb0994c0861fb08280c38daa09
   test_signature_validity( Msg, Qx, Qy, R, S, False )
 
-  Msg = 0x16b5f93afd0d02246f662761ed8e0dd9504681ed02a253006eb36736b563097ba39f81c8e1bce7a16c1339e345efabbc6baa3efb0612948ae51103382a8ee8bc448e3ef71e9f6f7a9676694831d7f5dd0db5446f179bcb737d4a526367a447bfe2c857521c7f40b6d7d7e01a180d92431fb0bbd29c04a0c420a57b3ed26ccd8aL
-  Qx = 0xfd14cdf1607f5efb7b1793037b15bdf4baa6f7c16341ab0bL
-  Qy = 0x83fa0795cc6c4795b9016dac928fd6bac32f3229a96312c4L
-  R = 0x8dfdb832951e0167c5d762a473c0416c5c15bc1195667dc1L
-  S = 0x1720288a2dc13fa1ec78f763f8fe2ff7354a7e6fdde44520L
+  Msg = 0x16b5f93afd0d02246f662761ed8e0dd9504681ed02a253006eb36736b563097ba39f81c8e1bce7a16c1339e345efabbc6baa3efb0612948ae51103382a8ee8bc448e3ef71e9f6f7a9676694831d7f5dd0db5446f179bcb737d4a526367a447bfe2c857521c7f40b6d7d7e01a180d92431fb0bbd29c04a0c420a57b3ed26ccd8a
+  Qx = 0xfd14cdf1607f5efb7b1793037b15bdf4baa6f7c16341ab0b
+  Qy = 0x83fa0795cc6c4795b9016dac928fd6bac32f3229a96312c4
+  R = 0x8dfdb832951e0167c5d762a473c0416c5c15bc1195667dc1
+  S = 0x1720288a2dc13fa1ec78f763f8fe2ff7354a7e6fdde44520
   test_signature_validity( Msg, Qx, Qy, R, S, False )
 
-  Msg = 0x08a2024b61b79d260e3bb43ef15659aec89e5b560199bc82cf7c65c77d39192e03b9a895d766655105edd9188242b91fbde4167f7862d4ddd61e5d4ab55196683d4f13ceb90d87aea6e07eb50a874e33086c4a7cb0273a8e1c4408f4b846bceae1ebaac1b2b2ea851a9b09de322efe34cebe601653efd6ddc876ce8c2f2072fbL
-  Qx = 0x674f941dc1a1f8b763c9334d726172d527b90ca324db8828L
-  Qy = 0x65adfa32e8b236cb33a3e84cf59bfb9417ae7e8ede57a7ffL
-  R = 0x9508b9fdd7daf0d8126f9e2bc5a35e4c6d800b5b804d7796L
-  S = 0x36f2bf6b21b987c77b53bb801b3435a577e3d493744bfab0L
+  Msg = 0x08a2024b61b79d260e3bb43ef15659aec89e5b560199bc82cf7c65c77d39192e03b9a895d766655105edd9188242b91fbde4167f7862d4ddd61e5d4ab55196683d4f13ceb90d87aea6e07eb50a874e33086c4a7cb0273a8e1c4408f4b846bceae1ebaac1b2b2ea851a9b09de322efe34cebe601653efd6ddc876ce8c2f2072fb
+  Qx = 0x674f941dc1a1f8b763c9334d726172d527b90ca324db8828
+  Qy = 0x65adfa32e8b236cb33a3e84cf59bfb9417ae7e8ede57a7ff
+  R = 0x9508b9fdd7daf0d8126f9e2bc5a35e4c6d800b5b804d7796
+  S = 0x36f2bf6b21b987c77b53bb801b3435a577e3d493744bfab0
   test_signature_validity( Msg, Qx, Qy, R, S, False )
 
-  Msg = 0x1843aba74b0789d4ac6b0b8923848023a644a7b70afa23b1191829bbe4397ce15b629bf21a8838298653ed0c19222b95fa4f7390d1b4c844d96e645537e0aae98afb5c0ac3bd0e4c37f8daaff25556c64e98c319c52687c904c4de7240a1cc55cd9756b7edaef184e6e23b385726e9ffcba8001b8f574987c1a3fedaaa83ca6dL
-  Qx = 0x10ecca1aad7220b56a62008b35170bfd5e35885c4014a19fL
-  Qy = 0x04eb61984c6c12ade3bc47f3c629ece7aa0a033b9948d686L
-  R = 0x82bfa4e82c0dfe9274169b86694e76ce993fd83b5c60f325L
-  S = 0xa97685676c59a65dbde002fe9d613431fb183e8006d05633L
+  Msg = 0x1843aba74b0789d4ac6b0b8923848023a644a7b70afa23b1191829bbe4397ce15b629bf21a8838298653ed0c19222b95fa4f7390d1b4c844d96e645537e0aae98afb5c0ac3bd0e4c37f8daaff25556c64e98c319c52687c904c4de7240a1cc55cd9756b7edaef184e6e23b385726e9ffcba8001b8f574987c1a3fedaaa83ca6d
+  Qx = 0x10ecca1aad7220b56a62008b35170bfd5e35885c4014a19f
+  Qy = 0x04eb61984c6c12ade3bc47f3c629ece7aa0a033b9948d686
+  R = 0x82bfa4e82c0dfe9274169b86694e76ce993fd83b5c60f325
+  S = 0xa97685676c59a65dbde002fe9d613431fb183e8006d05633
   test_signature_validity( Msg, Qx, Qy, R, S, False )
 
-  Msg = 0x5a478f4084ddd1a7fea038aa9732a822106385797d02311aeef4d0264f824f698df7a48cfb6b578cf3da416bc0799425bb491be5b5ecc37995b85b03420a98f2c4dc5c31a69a379e9e322fbe706bbcaf0f77175e05cbb4fa162e0da82010a278461e3e974d137bc746d1880d6eb02aa95216014b37480d84b87f717bb13f76e1L
-  Qx = 0x6636653cb5b894ca65c448277b29da3ad101c4c2300f7c04L
-  Qy = 0xfdf1cbb3fc3fd6a4f890b59e554544175fa77dbdbeb656c1L
-  R = 0xeac2ddecddfb79931a9c3d49c08de0645c783a24cb365e1cL
-  S = 0x3549fee3cfa7e5f93bc47d92d8ba100e881a2a93c22f8d50L
+  Msg = 0x5a478f4084ddd1a7fea038aa9732a822106385797d02311aeef4d0264f824f698df7a48cfb6b578cf3da416bc0799425bb491be5b5ecc37995b85b03420a98f2c4dc5c31a69a379e9e322fbe706bbcaf0f77175e05cbb4fa162e0da82010a278461e3e974d137bc746d1880d6eb02aa95216014b37480d84b87f717bb13f76e1
+  Qx = 0x6636653cb5b894ca65c448277b29da3ad101c4c2300f7c04
+  Qy = 0xfdf1cbb3fc3fd6a4f890b59e554544175fa77dbdbeb656c1
+  R = 0xeac2ddecddfb79931a9c3d49c08de0645c783a24cb365e1c
+  S = 0x3549fee3cfa7e5f93bc47d92d8ba100e881a2a93c22f8d50
   test_signature_validity( Msg, Qx, Qy, R, S, False )
 
-  Msg = 0xc598774259a058fa65212ac57eaa4f52240e629ef4c310722088292d1d4af6c39b49ce06ba77e4247b20637174d0bd67c9723feb57b5ead232b47ea452d5d7a089f17c00b8b6767e434a5e16c231ba0efa718a340bf41d67ea2d295812ff1b9277daacb8bc27b50ea5e6443bcf95ef4e9f5468fe78485236313d53d1c68f6ba2L
-  Qx = 0xa82bd718d01d354001148cd5f69b9ebf38ff6f21898f8aaaL
-  Qy = 0xe67ceede07fc2ebfafd62462a51e4b6c6b3d5b537b7caf3eL
-  R = 0x4d292486c620c3de20856e57d3bb72fcde4a73ad26376955L
-  S = 0xa85289591a6081d5728825520e62ff1c64f94235c04c7f95L
+  Msg = 0xc598774259a058fa65212ac57eaa4f52240e629ef4c310722088292d1d4af6c39b49ce06ba77e4247b20637174d0bd67c9723feb57b5ead232b47ea452d5d7a089f17c00b8b6767e434a5e16c231ba0efa718a340bf41d67ea2d295812ff1b9277daacb8bc27b50ea5e6443bcf95ef4e9f5468fe78485236313d53d1c68f6ba2
+  Qx = 0xa82bd718d01d354001148cd5f69b9ebf38ff6f21898f8aaa
+  Qy = 0xe67ceede07fc2ebfafd62462a51e4b6c6b3d5b537b7caf3e
+  R = 0x4d292486c620c3de20856e57d3bb72fcde4a73ad26376955
+  S = 0xa85289591a6081d5728825520e62ff1c64f94235c04c7f95
   test_signature_validity( Msg, Qx, Qy, R, S, False )
 
-  Msg = 0xca98ed9db081a07b7557f24ced6c7b9891269a95d2026747add9e9eb80638a961cf9c71a1b9f2c29744180bd4c3d3db60f2243c5c0b7cc8a8d40a3f9a7fc910250f2187136ee6413ffc67f1a25e1c4c204fa9635312252ac0e0481d89b6d53808f0c496ba87631803f6c572c1f61fa049737fdacce4adff757afed4f05beb658L
-  Qx = 0x7d3b016b57758b160c4fca73d48df07ae3b6b30225126c2fL
-  Qy = 0x4af3790d9775742bde46f8da876711be1b65244b2b39e7ecL
-  R = 0x95f778f5f656511a5ab49a5d69ddd0929563c29cbc3a9e62L
-  S = 0x75c87fc358c251b4c83d2dd979faad496b539f9f2ee7a289L
+  Msg = 0xca98ed9db081a07b7557f24ced6c7b9891269a95d2026747add9e9eb80638a961cf9c71a1b9f2c29744180bd4c3d3db60f2243c5c0b7cc8a8d40a3f9a7fc910250f2187136ee6413ffc67f1a25e1c4c204fa9635312252ac0e0481d89b6d53808f0c496ba87631803f6c572c1f61fa049737fdacce4adff757afed4f05beb658
+  Qx = 0x7d3b016b57758b160c4fca73d48df07ae3b6b30225126c2f
+  Qy = 0x4af3790d9775742bde46f8da876711be1b65244b2b39e7ec
+  R = 0x95f778f5f656511a5ab49a5d69ddd0929563c29cbc3a9e62
+  S = 0x75c87fc358c251b4c83d2dd979faad496b539f9f2ee7a289
   test_signature_validity( Msg, Qx, Qy, R, S, False )
 
-  Msg = 0x31dd9a54c8338bea06b87eca813d555ad1850fac9742ef0bbe40dad400e10288acc9c11ea7dac79eb16378ebea9490e09536099f1b993e2653cd50240014c90a9c987f64545abc6a536b9bd2435eb5e911fdfde2f13be96ea36ad38df4ae9ea387b29cced599af777338af2794820c9cce43b51d2112380a35802ab7e396c97aL
-  Qx = 0x9362f28c4ef96453d8a2f849f21e881cd7566887da8beb4aL
-  Qy = 0xe64d26d8d74c48a024ae85d982ee74cd16046f4ee5333905L
-  R = 0xf3923476a296c88287e8de914b0b324ad5a963319a4fe73bL
-  S = 0xf0baeed7624ed00d15244d8ba2aede085517dbdec8ac65f5L
+  Msg = 0x31dd9a54c8338bea06b87eca813d555ad1850fac9742ef0bbe40dad400e10288acc9c11ea7dac79eb16378ebea9490e09536099f1b993e2653cd50240014c90a9c987f64545abc6a536b9bd2435eb5e911fdfde2f13be96ea36ad38df4ae9ea387b29cced599af777338af2794820c9cce43b51d2112380a35802ab7e396c97a
+  Qx = 0x9362f28c4ef96453d8a2f849f21e881cd7566887da8beb4a
+  Qy = 0xe64d26d8d74c48a024ae85d982ee74cd16046f4ee5333905
+  R = 0xf3923476a296c88287e8de914b0b324ad5a963319a4fe73b
+  S = 0xf0baeed7624ed00d15244d8ba2aede085517dbdec8ac65f5
   test_signature_validity( Msg, Qx, Qy, R, S, True )
 
-  Msg = 0xb2b94e4432267c92f9fdb9dc6040c95ffa477652761290d3c7de312283f6450d89cc4aabe748554dfb6056b2d8e99c7aeaad9cdddebdee9dbc099839562d9064e68e7bb5f3a6bba0749ca9a538181fc785553a4000785d73cc207922f63e8ce1112768cb1de7b673aed83a1e4a74592f1268d8e2a4e9e63d414b5d442bd0456dL
-  Qx = 0xcc6fc032a846aaac25533eb033522824f94e670fa997ecefL
-  Qy = 0xe25463ef77a029eccda8b294fd63dd694e38d223d30862f1L
-  R = 0x066b1d07f3a40e679b620eda7f550842a35c18b80c5ebe06L
-  S = 0xa0b0fb201e8f2df65e2c4508ef303bdc90d934016f16b2dcL
+  Msg = 0xb2b94e4432267c92f9fdb9dc6040c95ffa477652761290d3c7de312283f6450d89cc4aabe748554dfb6056b2d8e99c7aeaad9cdddebdee9dbc099839562d9064e68e7bb5f3a6bba0749ca9a538181fc785553a4000785d73cc207922f63e8ce1112768cb1de7b673aed83a1e4a74592f1268d8e2a4e9e63d414b5d442bd0456d
+  Qx = 0xcc6fc032a846aaac25533eb033522824f94e670fa997ecef
+  Qy = 0xe25463ef77a029eccda8b294fd63dd694e38d223d30862f1
+  R = 0x066b1d07f3a40e679b620eda7f550842a35c18b80c5ebe06
+  S = 0xa0b0fb201e8f2df65e2c4508ef303bdc90d934016f16b2dc
   test_signature_validity( Msg, Qx, Qy, R, S, False )
 
-  Msg = 0x4366fcadf10d30d086911de30143da6f579527036937007b337f7282460eae5678b15cccda853193ea5fc4bc0a6b9d7a31128f27e1214988592827520b214eed5052f7775b750b0c6b15f145453ba3fee24a085d65287e10509eb5d5f602c440341376b95c24e5c4727d4b859bfe1483d20538acdd92c7997fa9c614f0f839d7L
-  Qx = 0x955c908fe900a996f7e2089bee2f6376830f76a19135e753L
-  Qy = 0xba0c42a91d3847de4a592a46dc3fdaf45a7cc709b90de520L
-  R = 0x1f58ad77fc04c782815a1405b0925e72095d906cbf52a668L
-  S = 0xf2e93758b3af75edf784f05a6761c9b9a6043c66b845b599L
+  Msg = 0x4366fcadf10d30d086911de30143da6f579527036937007b337f7282460eae5678b15cccda853193ea5fc4bc0a6b9d7a31128f27e1214988592827520b214eed5052f7775b750b0c6b15f145453ba3fee24a085d65287e10509eb5d5f602c440341376b95c24e5c4727d4b859bfe1483d20538acdd92c7997fa9c614f0f839d7
+  Qx = 0x955c908fe900a996f7e2089bee2f6376830f76a19135e753
+  Qy = 0xba0c42a91d3847de4a592a46dc3fdaf45a7cc709b90de520
+  R = 0x1f58ad77fc04c782815a1405b0925e72095d906cbf52a668
+  S = 0xf2e93758b3af75edf784f05a6761c9b9a6043c66b845b599
   test_signature_validity( Msg, Qx, Qy, R, S, False )
 
-  Msg = 0x543f8af57d750e33aa8565e0cae92bfa7a1ff78833093421c2942cadf9986670a5ff3244c02a8225e790fbf30ea84c74720abf99cfd10d02d34377c3d3b41269bea763384f372bb786b5846f58932defa68023136cd571863b304886e95e52e7877f445b9364b3f06f3c28da12707673fecb4b8071de06b6e0a3c87da160cef3L
-  Qx = 0x31f7fa05576d78a949b24812d4383107a9a45bb5fccdd835L
-  Qy = 0x8dc0eb65994a90f02b5e19bd18b32d61150746c09107e76bL
-  R = 0xbe26d59e4e883dde7c286614a767b31e49ad88789d3a78ffL
-  S = 0x8762ca831c1ce42df77893c9b03119428e7a9b819b619068L
+  Msg = 0x543f8af57d750e33aa8565e0cae92bfa7a1ff78833093421c2942cadf9986670a5ff3244c02a8225e790fbf30ea84c74720abf99cfd10d02d34377c3d3b41269bea763384f372bb786b5846f58932defa68023136cd571863b304886e95e52e7877f445b9364b3f06f3c28da12707673fecb4b8071de06b6e0a3c87da160cef3
+  Qx = 0x31f7fa05576d78a949b24812d4383107a9a45bb5fccdd835
+  Qy = 0x8dc0eb65994a90f02b5e19bd18b32d61150746c09107e76b
+  R = 0xbe26d59e4e883dde7c286614a767b31e49ad88789d3a78ff
+  S = 0x8762ca831c1ce42df77893c9b03119428e7a9b819b619068
   test_signature_validity( Msg, Qx, Qy, R, S, False )
 
-  Msg = 0xd2e8454143ce281e609a9d748014dcebb9d0bc53adb02443a6aac2ffe6cb009f387c346ecb051791404f79e902ee333ad65e5c8cb38dc0d1d39a8dc90add5023572720e5b94b190d43dd0d7873397504c0c7aef2727e628eb6a74411f2e400c65670716cb4a815dc91cbbfeb7cfe8c929e93184c938af2c078584da045e8f8d1L
-  Qx = 0x66aa8edbbdb5cf8e28ceb51b5bda891cae2df84819fe25c0L
-  Qy = 0x0c6bc2f69030a7ce58d4a00e3b3349844784a13b8936f8daL
-  R = 0xa4661e69b1734f4a71b788410a464b71e7ffe42334484f23L
-  S = 0x738421cf5e049159d69c57a915143e226cac8355e149afe9L
+  Msg = 0xd2e8454143ce281e609a9d748014dcebb9d0bc53adb02443a6aac2ffe6cb009f387c346ecb051791404f79e902ee333ad65e5c8cb38dc0d1d39a8dc90add5023572720e5b94b190d43dd0d7873397504c0c7aef2727e628eb6a74411f2e400c65670716cb4a815dc91cbbfeb7cfe8c929e93184c938af2c078584da045e8f8d1
+  Qx = 0x66aa8edbbdb5cf8e28ceb51b5bda891cae2df84819fe25c0
+  Qy = 0x0c6bc2f69030a7ce58d4a00e3b3349844784a13b8936f8da
+  R = 0xa4661e69b1734f4a71b788410a464b71e7ffe42334484f23
+  S = 0x738421cf5e049159d69c57a915143e226cac8355e149afe9
   test_signature_validity( Msg, Qx, Qy, R, S, False )
 
-  Msg = 0x6660717144040f3e2f95a4e25b08a7079c702a8b29babad5a19a87654bc5c5afa261512a11b998a4fb36b5d8fe8bd942792ff0324b108120de86d63f65855e5461184fc96a0a8ffd2ce6d5dfb0230cbbdd98f8543e361b3205f5da3d500fdc8bac6db377d75ebef3cb8f4d1ff738071ad0938917889250b41dd1d98896ca06fbL
-  Qx = 0xbcfacf45139b6f5f690a4c35a5fffa498794136a2353fc77L
-  Qy = 0x6f4a6c906316a6afc6d98fe1f0399d056f128fe0270b0f22L
-  R = 0x9db679a3dafe48f7ccad122933acfe9da0970b71c94c21c1L
-  S = 0x984c2db99827576c0a41a5da41e07d8cc768bc82f18c9da9L
+  Msg = 0x6660717144040f3e2f95a4e25b08a7079c702a8b29babad5a19a87654bc5c5afa261512a11b998a4fb36b5d8fe8bd942792ff0324b108120de86d63f65855e5461184fc96a0a8ffd2ce6d5dfb0230cbbdd98f8543e361b3205f5da3d500fdc8bac6db377d75ebef3cb8f4d1ff738071ad0938917889250b41dd1d98896ca06fb
+  Qx = 0xbcfacf45139b6f5f690a4c35a5fffa498794136a2353fc77
+  Qy = 0x6f4a6c906316a6afc6d98fe1f0399d056f128fe0270b0f22
+  R = 0x9db679a3dafe48f7ccad122933acfe9da0970b71c94c21c1
+  S = 0x984c2db99827576c0a41a5da41e07d8cc768bc82f18c9da9
   test_signature_validity( Msg, Qx, Qy, R, S, False )
 
 
 
-  print "Testing the example code:"
+  print_("Testing the example code:")
 
   # Building a public/private key pair from the NIST Curve P-192:
 
   g = generator_192
   n = g.order()
 
   # (random.SystemRandom is supposed to provide
   # crypto-quality random numbers, but as Debian recently
   # illustrated, a systems programmer can accidentally
   # demolish this security, so in serious applications
   # further precautions are appropriate.)
 
   randrange = random.SystemRandom().randrange
-  
+
   secret = randrange( 1, n )
   pubkey = Public_key( g, g * secret )
   privkey = Private_key( pubkey, secret )
 
   # Signing a hash value:
-  
+
   hash = randrange( 1, n )
   signature = privkey.sign( hash, randrange( 1, n ) )
 
   # Verifying a signature for a hash value:
-  
+
   if pubkey.verifies( hash, signature ):
-    print "Demo verification succeeded."
+    print_("Demo verification succeeded.")
   else:
     raise TestFailure("*** Demo verification failed.")
 
   if pubkey.verifies( hash-1, signature ):
     raise TestFailure( "**** Demo verification failed to reject tampered hash.")
   else:
-    print "Demo verification correctly rejected tampered hash."
+    print_("Demo verification correctly rejected tampered hash.")
 
 if __name__ == "__main__":
   __main__()
```

### Comparing `ecdsa-0.8/ecdsa/ellipticcurve.py` & `ecdsa-0.9/ecdsa/ellipticcurve.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,18 @@
 #
 # Revision history:
 #    2005.12.31 - Initial version.
 #    2008.11.25 - Change CurveFp.is_on to contains_point.
 #
 # Written in 2005 by Peter Pearson and placed in the public domain.
 
-import numbertheory
+from __future__ import division
+
+from .six import print_
+from . import numbertheory
 
 class CurveFp( object ):
   """Elliptic Curve over the field of integers modulo a prime."""
   def __init__( self, p, a, b ):
     """The curve of points satisfying y^2 = x^3 + a*x + b (mod p)."""
     self.__p = p
     self.__a = a
@@ -65,27 +68,27 @@
     self.__curve = curve
     self.__x = x
     self.__y = y
     self.__order = order
     # self.curve is allowed to be None only for INFINITY:
     if self.__curve: assert self.__curve.contains_point( x, y )
     if order: assert self * order == INFINITY
- 
-  def __cmp__( self, other ):
-    """Return 0 if the points are identical, 1 otherwise."""
+
+  def __eq__( self, other ):
+    """Return True if the points are identical, False otherwise."""
     if self.__curve == other.__curve \
        and self.__x == other.__x \
        and self.__y == other.__y:
-      return 0
+      return True
     else:
-      return 1
+      return False
 
   def __add__( self, other ):
     """Add one point to another point."""
-    
+
     # X9.62 B.3:
 
     if other == INFINITY: return self
     if self == INFINITY: return other
     assert self.__curve == other.__curve
     if self.__x == other.__x:
       if ( self.__y + other.__y ) % self.__curve.p() == 0:
@@ -96,23 +99,23 @@
     p = self.__curve.p()
 
     l = ( ( other.__y - self.__y ) * \
           numbertheory.inverse_mod( other.__x - self.__x, p ) ) % p
 
     x3 = ( l * l - self.__x - other.__x ) % p
     y3 = ( l * ( self.__x - x3 ) - self.__y ) % p
-    
+
     return Point( self.__curve, x3, y3 )
 
   def __mul__( self, other ):
     """Multiply a point by an integer."""
 
     def leftmost_bit( x ):
       assert x > 0
-      result = 1L
+      result = 1
       while result <= x: result = 2 * result
       return result // 2
 
     e = other
     if self.__order: e = e % self.__order
     if e == 0: return INFINITY
     if self == INFINITY: return INFINITY
@@ -120,27 +123,27 @@
 
     # From X9.62 D.3.2:
 
     e3 = 3 * e
     negative_self = Point( self.__curve, self.__x, -self.__y, self.__order )
     i = leftmost_bit( e3 ) // 2
     result = self
-    # print "Multiplying %s by %d (e3 = %d):" % ( self, other, e3 )
+    # print_("Multiplying %s by %d (e3 = %d):" % ( self, other, e3 ))
     while i > 1:
       result = result.double()
       if ( e3 & i ) != 0 and ( e & i ) == 0: result = result + self
       if ( e3 & i ) == 0 and ( e & i ) != 0: result = result + negative_self
-      # print ". . . i = %d, result = %s" % ( i, result )
+      # print_(". . . i = %d, result = %s" % ( i, result ))
       i = i // 2
 
     return result
 
   def __rmul__( self, other ):
     """Multiply a point by an integer."""
-    
+
     return self * other
 
   def __str__( self ):
     if self == INFINITY: return "infinity"
     return "(%d,%d)" % ( self.__x, self.__y )
 
   def double( self ):
@@ -155,76 +158,76 @@
     a = self.__curve.a()
 
     l = ( ( 3 * self.__x * self.__x + a ) * \
           numbertheory.inverse_mod( 2 * self.__y, p ) ) % p
 
     x3 = ( l * l - 2 * self.__x ) % p
     y3 = ( l * ( self.__x - x3 ) - self.__y ) % p
-    
+
     return Point( self.__curve, x3, y3 )
 
   def x( self ):
     return self.__x
 
   def y( self ):
     return self.__y
 
   def curve( self ):
     return self.__curve
-  
+
   def order( self ):
     return self.__order
 
 
 # This one point is the Point At Infinity for all purposes:
-INFINITY = Point( None, None, None )  
+INFINITY = Point( None, None, None )
 
 def __main__():
 
   class FailedTest(Exception): pass
   def test_add( c, x1, y1, x2,  y2, x3, y3 ):
     """We expect that on curve c, (x1,y1) + (x2, y2 ) = (x3, y3)."""
     p1 = Point( c, x1, y1 )
     p2 = Point( c, x2, y2 )
     p3 = p1 + p2
-    print "%s + %s = %s" % ( p1, p2, p3 ),
+    print_("%s + %s = %s" % ( p1, p2, p3 ), end=' ')
     if p3.x() != x3 or p3.y() != y3:
       raise FailedTest("Failure: should give (%d,%d)." % ( x3, y3 ))
     else:
-      print " Good."
+      print_(" Good.")
 
   def test_double( c, x1, y1, x3, y3 ):
     """We expect that on curve c, 2*(x1,y1) = (x3, y3)."""
     p1 = Point( c, x1, y1 )
     p3 = p1.double()
-    print "%s doubled = %s" % ( p1, p3 ),
+    print_("%s doubled = %s" % ( p1, p3 ), end=' ')
     if p3.x() != x3 or p3.y() != y3:
       raise FailedTest("Failure: should give (%d,%d)." % ( x3, y3 ))
     else:
-      print " Good."
+      print_(" Good.")
 
   def test_double_infinity( c ):
     """We expect that on curve c, 2*INFINITY = INFINITY."""
     p1 = INFINITY
     p3 = p1.double()
-    print "%s doubled = %s" % ( p1, p3 ),
+    print_("%s doubled = %s" % ( p1, p3 ), end=' ')
     if p3.x() != INFINITY.x() or p3.y() != INFINITY.y():
       raise FailedTest("Failure: should give (%d,%d)." % ( INFINITY.x(), INFINITY.y() ))
     else:
-      print " Good."
+      print_(" Good.")
 
   def test_multiply( c, x1, y1, m, x3, y3 ):
     """We expect that on curve c, m*(x1,y1) = (x3,y3)."""
     p1 = Point( c, x1, y1 )
     p3 = p1 * m
-    print "%s * %d = %s" % ( p1, m, p3 ),
+    print_("%s * %d = %s" % ( p1, m, p3 ), end=' ')
     if p3.x() != x3 or p3.y() != y3:
       raise FailedTest("Failure: should give (%d,%d)." % ( x3, y3 ))
     else:
-      print " Good."
+      print_(" Good.")
 
 
   # A few tests from X9.62 B.3:
 
   c = CurveFp( 23, 1, 1 )
   test_add( c, 3, 10, 9, 7, 17, 20 )
   test_double( c, 3, 10, 7, 12 )
@@ -236,55 +239,55 @@
   # From X9.62 I.1 (p. 96):
 
   g = Point( c, 13, 7, 7 )
 
   check = INFINITY
   for i in range( 7 + 1 ):
     p = ( i % 7 ) * g
-    print "%s * %d = %s, expected %s . . ." % ( g, i, p, check ),
+    print_("%s * %d = %s, expected %s . . ." % ( g, i, p, check ), end=' ')
     if p == check:
-      print " Good."
+      print_(" Good.")
     else:
       raise FailedTest("Bad.")
     check = check + g
 
   # NIST Curve P-192:
-  p = 6277101735386680763835789423207666416083908700390324961279L
-  r = 6277101735386680763835789423176059013767194773182842284081L
+  p = 6277101735386680763835789423207666416083908700390324961279
+  r = 6277101735386680763835789423176059013767194773182842284081
   #s = 0x3045ae6fc8422f64ed579528d38120eae12196d5L
-  c = 0x3099d2bbbfcb2538542dcd5fb078b6ef5f3d6fe2c745de65L
-  b = 0x64210519e59c80e70fa7e9ab72243049feb8deecc146b9b1L
-  Gx = 0x188da80eb03090f67cbf20eb43a18800f4ff0afd82ff1012L
-  Gy = 0x07192b95ffc8da78631011ed6b24cdd573f977a11e794811L
+  c = 0x3099d2bbbfcb2538542dcd5fb078b6ef5f3d6fe2c745de65
+  b = 0x64210519e59c80e70fa7e9ab72243049feb8deecc146b9b1
+  Gx = 0x188da80eb03090f67cbf20eb43a18800f4ff0afd82ff1012
+  Gy = 0x07192b95ffc8da78631011ed6b24cdd573f977a11e794811
 
   c192 = CurveFp( p, -3, b )
   p192 = Point( c192, Gx, Gy, r )
 
   # Checking against some sample computations presented
   # in X9.62:
 
-  d = 651056770906015076056810763456358567190100156695615665659L
+  d = 651056770906015076056810763456358567190100156695615665659
   Q = d * p192
-  if Q.x() != 0x62B12D60690CDCF330BABAB6E69763B471F994DD702D16A5L:
+  if Q.x() != 0x62B12D60690CDCF330BABAB6E69763B471F994DD702D16A5:
     raise FailedTest("p192 * d came out wrong.")
   else:
-    print "p192 * d came out right."
+    print_("p192 * d came out right.")
 
-  k = 6140507067065001063065065565667405560006161556565665656654L
+  k = 6140507067065001063065065565667405560006161556565665656654
   R = k * p192
-  if R.x() != 0x885052380FF147B734C330C43D39B2C4A89F29B0F749FEADL \
-     or R.y() != 0x9CF9FA1CBEFEFB917747A3BB29C072B9289C2547884FD835L:
+  if R.x() != 0x885052380FF147B734C330C43D39B2C4A89F29B0F749FEAD \
+     or R.y() != 0x9CF9FA1CBEFEFB917747A3BB29C072B9289C2547884FD835:
     raise FailedTest("k * p192 came out wrong.")
   else:
-    print "k * p192 came out right."
+    print_("k * p192 came out right.")
 
-  u1 = 2563697409189434185194736134579731015366492496392189760599L
-  u2 = 6266643813348617967186477710235785849136406323338782220568L
+  u1 = 2563697409189434185194736134579731015366492496392189760599
+  u2 = 6266643813348617967186477710235785849136406323338782220568
   temp = u1 * p192 + u2 * Q
-  if temp.x() != 0x885052380FF147B734C330C43D39B2C4A89F29B0F749FEADL \
-     or temp.y() != 0x9CF9FA1CBEFEFB917747A3BB29C072B9289C2547884FD835L:
+  if temp.x() != 0x885052380FF147B734C330C43D39B2C4A89F29B0F749FEAD \
+     or temp.y() != 0x9CF9FA1CBEFEFB917747A3BB29C072B9289C2547884FD835:
     raise FailedTest("u1 * p192 + u2 * Q came out wrong.")
   else:
-    print "u1 * p192 + u2 * Q came out right."
+    print_("u1 * p192 + u2 * Q came out right.")
 
 if __name__ == "__main__":
   __main__()
```

### Comparing `ecdsa-0.8/ecdsa/keys.py` & `ecdsa-0.9/ecdsa/keys.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import binascii
 
-import ecdsa
-import der
-from curves import NIST192p, find_curve
-from util import string_to_number, number_to_string, randrange
-from util import sigencode_string, sigdecode_string
-from util import oid_ecPublicKey, encoded_oid_ecPublicKey
+from . import ecdsa
+from . import der
+from . import rfc6979
+from .curves import NIST192p, find_curve
+from .util import string_to_number, number_to_string, randrange
+from .util import sigencode_string, sigdecode_string
+from .util import oid_ecPublicKey, encoded_oid_ecPublicKey
+from .six import PY3, b
 from hashlib import sha1
 
 class BadSignatureError(Exception):
     pass
 class BadDigestError(Exception):
     pass
 
@@ -35,43 +37,43 @@
         xs = string[:curve.baselen]
         ys = string[curve.baselen:]
         assert len(xs) == curve.baselen, (len(xs), curve.baselen)
         assert len(ys) == curve.baselen, (len(ys), curve.baselen)
         x = string_to_number(xs)
         y = string_to_number(ys)
         assert ecdsa.point_is_valid(curve.generator, x, y)
-        import ellipticcurve
+        from . import ellipticcurve
         point = ellipticcurve.Point(curve.curve, x, y, order)
         return klass.from_public_point(point, curve, hashfunc)
 
     @classmethod
     def from_pem(klass, string):
         return klass.from_der(der.unpem(string))
 
     @classmethod
     def from_der(klass, string):
         # [[oid_ecPublicKey,oid_curve], point_str_bitstring]
         s1,empty = der.remove_sequence(string)
-        if empty != "":
+        if empty != b(""):
             raise der.UnexpectedDER("trailing junk after DER pubkey: %s" %
                                     binascii.hexlify(empty))
         s2,point_str_bitstring = der.remove_sequence(s1)
         # s2 = oid_ecPublicKey,oid_curve
         oid_pk, rest = der.remove_object(s2)
         oid_curve, empty = der.remove_object(rest)
-        if empty != "":
+        if empty != b(""):
             raise der.UnexpectedDER("trailing junk after DER pubkey objects: %s" %
                                     binascii.hexlify(empty))
         assert oid_pk == oid_ecPublicKey, (oid_pk, oid_ecPublicKey)
         curve = find_curve(oid_curve)
         point_str, empty = der.remove_bitstring(point_str_bitstring)
-        if empty != "":
+        if empty != b(""):
             raise der.UnexpectedDER("trailing junk after pubkey pointstring: %s" %
                                     binascii.hexlify(empty))
-        assert point_str.startswith("\x00\x04")
+        assert point_str.startswith(b("\x00\x04"))
         return klass.from_string(point_str[2:], curve)
 
     def to_string(self):
         # VerifyingKey.from_string(vk.to_string()) == vk as long as the
         # curves are the same: the curve itself is not included in the
         # serialized form
         order = self.pubkey.order
@@ -82,15 +84,15 @@
     def to_pem(self):
         return der.topem(self.to_der(), "PUBLIC KEY")
 
     def to_der(self):
         order = self.pubkey.order
         x_str = number_to_string(self.pubkey.point.x(), order)
         y_str = number_to_string(self.pubkey.point.y(), order)
-        point_str = "\x00\x04" + x_str + y_str
+        point_str = b("\x00\x04") + x_str + y_str
         return der.encode_sequence(der.encode_sequence(encoded_oid_ecPublicKey,
                                                        self.curve.encoded_oid),
                                    der.encode_bitstring(point_str))
 
     def verify(self, signature, data, hashfunc=None, sigdecode=sigdecode_string):
         hashfunc = hashfunc or self.default_hashfunc
         digest = hashfunc(data).digest()
@@ -146,35 +148,37 @@
         secexp = string_to_number(string)
         return klass.from_secret_exponent(secexp, curve, hashfunc)
 
     @classmethod
     def from_pem(klass, string, hashfunc=sha1):
         # the privkey pem file has two sections: "EC PARAMETERS" and "EC
         # PRIVATE KEY". The first is redundant.
-        privkey_pem = string[string.index("-----BEGIN EC PRIVATE KEY-----"):]
+        if PY3 and isinstance(string, str):
+            string = string.encode()
+        privkey_pem = string[string.index(b("-----BEGIN EC PRIVATE KEY-----")):]
         return klass.from_der(der.unpem(privkey_pem), hashfunc)
     @classmethod
     def from_der(klass, string, hashfunc=sha1):
         # SEQ([int(1), octetstring(privkey),cont[0], oid(secp224r1),
         #      cont[1],bitstring])
         s, empty = der.remove_sequence(string)
-        if empty != "":
+        if empty != b(""):
             raise der.UnexpectedDER("trailing junk after DER privkey: %s" %
                                     binascii.hexlify(empty))
         one, s = der.remove_integer(s)
         if one != 1:
             raise der.UnexpectedDER("expected '1' at start of DER privkey,"
                                     " got %d" % one)
         privkey_str, s = der.remove_octet_string(s)
         tag, curve_oid_str, s = der.remove_constructed(s)
         if tag != 0:
             raise der.UnexpectedDER("expected tag 0 in DER privkey,"
                                     " got %d" % tag)
         curve_oid, empty = der.remove_object(curve_oid_str)
-        if empty != "":
+        if empty != b(""):
             raise der.UnexpectedDER("trailing junk after DER privkey "
                                     "curve_oid: %s" % binascii.hexlify(empty))
         curve = find_curve(curve_oid)
 
         # we don't actually care about the following fields
         #
         #tag, pubkey_bitstring, s = der.remove_constructed(s)
@@ -184,69 +188,93 @@
         #pubkey_str = der.remove_bitstring(pubkey_bitstring)
         #if empty != "":
         #    raise der.UnexpectedDER("trailing junk after DER privkey "
         #                            "pubkeystr: %s" % binascii.hexlify(empty))
 
         # our from_string method likes fixed-length privkey strings
         if len(privkey_str) < curve.baselen:
-            privkey_str = "\x00"*(curve.baselen-len(privkey_str)) + privkey_str
+            privkey_str = b("\x00")*(curve.baselen-len(privkey_str)) + privkey_str
         return klass.from_string(privkey_str, curve, hashfunc)
 
     def to_string(self):
         secexp = self.privkey.secret_multiplier
         s = number_to_string(secexp, self.privkey.order)
         return s
 
     def to_pem(self):
         # TODO: "BEGIN ECPARAMETERS"
         return der.topem(self.to_der(), "EC PRIVATE KEY")
 
     def to_der(self):
         # SEQ([int(1), octetstring(privkey),cont[0], oid(secp224r1),
         #      cont[1],bitstring])
-        encoded_vk = "\x00\x04" + self.get_verifying_key().to_string()
+        encoded_vk = b("\x00\x04") + self.get_verifying_key().to_string()
         return der.encode_sequence(der.encode_integer(1),
                                    der.encode_octet_string(self.to_string()),
                                    der.encode_constructed(0, self.curve.encoded_oid),
                                    der.encode_constructed(1, der.encode_bitstring(encoded_vk)),
                                    )
 
     def get_verifying_key(self):
         return self.verifying_key
 
-    def sign(self, data, entropy=None, hashfunc=None, sigencode=sigencode_string):
+    def sign_deterministic(self, data, hashfunc=None, sigencode=sigencode_string):
+        hashfunc = hashfunc or self.default_hashfunc
+        digest = hashfunc(data).digest()
+
+        return self.sign_digest_deterministic(digest, hashfunc=hashfunc, sigencode=sigencode)
+
+    def sign_digest_deterministic(self, digest, hashfunc=None, sigencode=sigencode_string):
+        """
+        Calculates 'k' from data itself, removing the need for strong
+        random generator and producing deterministic (reproducible) signatures.
+        See RFC 6979 for more details.
+        """
+        secexp = self.privkey.secret_multiplier
+        k = rfc6979.generate_k(self.curve.generator, secexp, hashfunc, digest)
+
+        return self.sign_digest(digest, sigencode=sigencode, k=k)
+
+    def sign(self, data, entropy=None, hashfunc=None, sigencode=sigencode_string, k=None):
         """
         hashfunc= should behave like hashlib.sha1 . The output length of the
         hash (in bytes) must not be longer than the length of the curve order
         (rounded up to the nearest byte), so using SHA256 with nist256p is
         ok, but SHA256 with nist192p is not. (In the 2**-96ish unlikely event
         of a hash output larger than the curve order, the hash will
         effectively be wrapped mod n).
 
         Use hashfunc=hashlib.sha1 to match openssl's -ecdsa-with-SHA1 mode,
         or hashfunc=hashlib.sha256 for openssl-1.0.0's -ecdsa-with-SHA256.
         """
 
         hashfunc = hashfunc or self.default_hashfunc
         h = hashfunc(data).digest()
-        return self.sign_digest(h, entropy, sigencode)
+        return self.sign_digest(h, entropy, sigencode, k)
 
-    def sign_digest(self, digest, entropy=None, sigencode=sigencode_string):
+    def sign_digest(self, digest, entropy=None, sigencode=sigencode_string, k=None):
         if len(digest) > self.curve.baselen:
             raise BadDigestError("this curve (%s) is too short "
                                  "for your digest (%d)" % (self.curve.name,
                                                            8*len(digest)))
         number = string_to_number(digest)
-        r, s = self.sign_number(number, entropy)
+        r, s = self.sign_number(number, entropy, k)
         return sigencode(r, s, self.privkey.order)
 
-    def sign_number(self, number, entropy=None):
+    def sign_number(self, number, entropy=None, k=None):
         # returns a pair of numbers
         order = self.privkey.order
         # privkey.sign() may raise RuntimeError in the amazingly unlikely
         # (2**-192) event that r=0 or s=0, because that would leak the key.
         # We could re-try with a different 'k', but we couldn't test that
         # code, so I choose to allow the signature to fail instead.
-        k = randrange(order, entropy)
-        assert 1 <= k < order
-        sig = self.privkey.sign(number, k)
+
+        # If k is set, it is used directly. In other cases
+        # it is generated using entropy function
+        if k is not None:
+            _k = k
+        else:
+            _k = randrange(order, entropy)
+
+        assert 1 <= _k < order
+        sig = self.privkey.sign(number, _k)
         return sig.r, sig.s
```

### Comparing `ecdsa-0.8/ecdsa/numbertheory.py` & `ecdsa-0.9/ecdsa/numbertheory.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 # Version of 2008.11.14.
 #
 # Written in 2005 and 2006 by Peter Pearson and placed in the public domain.
 # Revision history:
 #   2008.11.14: Use pow( base, exponent, modulus ) for modular_exp.
 #               Make gcd and lcm accept arbitrarly many arguments.
 
+from __future__ import division
 
+from .six import print_, integer_types
+from .six.moves import reduce
 
 import math
 import types
 
 
 class Error( Exception ):
   """Base class for exceptions in this module."""
@@ -85,17 +88,15 @@
 
   for i in range( len( m1 ) ):
     for j in range( len( m2 ) ):
       prod[i+j] = ( prod[i+j] + m1[i] * m2[j] ) % p
 
   return polynomial_reduce_mod( prod, polymod, p )
 
-  
 
-  
 def polynomial_exp_mod( base, exponent, polymod, p ):
   """Polynomial exponentiation modulo a polynomial over ints mod p.
 
   Polynomials are represented as lists of coefficients
   of increasing powers of x."""
 
   # Based on the Handbook of Applied Cryptography, algorithm 2.227.
@@ -139,15 +140,14 @@
   while a1%2 == 0:
     a1, e = a1//2, e+1
   if e%2 == 0 or n%8 == 1 or n%8 == 7: s = 1
   else: s = -1
   if a1 == 1: return s
   if n%4 == 3 and a1%4 == 3: s = -s
   return s * jacobi( n % a1, a1 )
-  
 
 
 
 def square_root_mod_prime( a, p ):
   """Modular square root of a, mod p, p prime."""
 
   # Based on the Handbook of Applied Cryptography, algorithms 3.34 to 3.39.
@@ -156,34 +156,34 @@
   # every prime p from 3 to 1229.
 
   assert 0 <= a < p
   assert 1 < p
 
   if a == 0: return 0
   if p == 2: return a
-  
+
   jac = jacobi( a, p )
   if jac == -1: raise SquareRootError( "%d has no square root modulo %d" \
                                        % ( a, p ) )
 
   if p % 4 == 3: return modular_exp( a, (p+1)//4, p )
 
   if p % 8 == 5:
     d = modular_exp( a, (p-1)//4, p )
     if d == 1: return modular_exp( a, (p+3)//8, p )
     if d == p-1: return ( 2 * a * modular_exp( 4*a, (p-5)//8, p ) ) % p
-    raise RuntimeError, "Shouldn't get here."
+    raise RuntimeError("Shouldn't get here.")
 
   for b in range( 2, p ):
     if jacobi( b*b-4*a, p ) == -1:
       f = ( a, -b, 1 )
       ff = polynomial_exp_mod( ( 0, 1 ), (p+1)//2, f, p )
       assert ff[1] == 0
       return ff[0]
-  raise RuntimeError, "No b found."
+  raise RuntimeError("No b found.")
 
 
 
 def inverse_mod( a, m ):
   """Inverse of a mod m."""
 
   if a < 0 or m <= a: a = a % m
@@ -241,15 +241,15 @@
   return a[0]
 
 
 
 def factorization( n ):
   """Decompose n into a list of (prime,exponent) pairs."""
 
-  assert isinstance( n, types.IntType ) or isinstance( n, types.LongType )
+  assert isinstance( n, integer_types )
 
   if n < 2: return []
 
   result = []
   d = 2
 
   # Test the small primes:
@@ -284,23 +284,23 @@
           while d <= n:                 # As long as d might still divide n,
             q, r = divmod( n, d )       # see if it does.
             if r != 0: break
             n = q                       # It does. Reduce n, increase count.
             count = count + 1
           result.append( ( d, count ) )
       if n > 1: result.append( ( n, 1 ) )
-        
+
   return result
 
 
 
 def phi( n ):
   """Return the Euler totient function of n."""
 
-  assert isinstance( n, types.IntType ) or isinstance( n, types.LongType )
+  assert isinstance( n, integer_types )
 
   if n < 3: return 1
 
   result = 1
   ff = factorization( n )
   for f in ff:
     e = f[1]
@@ -398,20 +398,20 @@
   about 66 composites got past the first test,
   5 got past the second test, and none got past the third.
   Since factors of 2, 3, 5, 7, and 11 were detected during
   preliminary screening, the number of numbers tested by
   Miller-Rabin was (19999999 - 10000001)*(2/3)*(4/5)*(6/7)
   = 4.57 million.
   """
-  
+
   # (This is used to study the risk of false positives:)
   global miller_rabin_test_count
 
   miller_rabin_test_count = 0
-  
+
   if n <= smallprimes[-1]:
     if n in smallprimes: return True
     else: return False
 
   if gcd( n, 2*3*5*7*11 ) != 1: return False
 
   # Choose a number of iterations sufficient to reduce the
@@ -439,15 +439,15 @@
   # Run the test t times:
 
   s = 0
   r = n - 1
   while ( r % 2 ) == 0:
     s = s + 1
     r = r // 2
-  for i in xrange( t ):
+  for i in range( t ):
     a = smallprimes[ i ]
     y = modular_exp( a, r, n )
     if y != 1 and y != n-1:
       j = 1
       while j <= s - 1 and y != n - 1:
         y = modular_exp( y, 2, n )
         if y == 1:
@@ -489,31 +489,31 @@
                1039, 1049, 1051, 1061, 1063, 1069, 1087, 1091, 1093,
                1097, 1103, 1109, 1117, 1123, 1129, 1151, 1153, 1163,
                1171, 1181, 1187, 1193, 1201, 1213, 1217, 1223, 1229]
 
 miller_rabin_test_count = 0
 
 def __main__():
-  
+
   # Making sure locally defined exceptions work:
   # p = modular_exp( 2, -2, 3 )
   # p = square_root_mod_prime( 2, 3 )
 
 
-  print "Testing gcd..."
+  print_("Testing gcd...")
   assert gcd( 3*5*7, 3*5*11, 3*5*13 )     == 3*5
   assert gcd( [ 3*5*7, 3*5*11, 3*5*13 ] ) == 3*5
   assert gcd( 3 ) == 3
 
-  print "Testing lcm..."
+  print_("Testing lcm...")
   assert lcm( 3, 5*3, 7*3 )     == 3*5*7
   assert lcm( [ 3, 5*3, 7*3 ] ) == 3*5*7
   assert lcm( 3 ) == 3
 
-  print "Testing next_prime..."
+  print_("Testing next_prime...")
   bigprimes = ( 999671,
                 999683,
                 999721,
                 999727,
                 999749,
                 999763,
                 999769,
@@ -527,88 +527,88 @@
                 999931,
                 999953,
                 999959,
                 999961,
                 999979,
                 999983 )
 
-  for i in xrange( len( bigprimes ) - 1 ):
+  for i in range( len( bigprimes ) - 1 ):
     assert next_prime( bigprimes[i] ) == bigprimes[ i+1 ]
 
   error_tally = 0
 
   # Test the square_root_mod_prime function:
 
   for p in smallprimes:
-    print "Testing square_root_mod_prime for modulus p = %d." % p
+    print_("Testing square_root_mod_prime for modulus p = %d." % p)
     squares = []
 
     for root in range( 0, 1+p//2 ):
       sq = ( root * root ) % p
       squares.append( sq )
       calculated = square_root_mod_prime( sq, p )
       if ( calculated * calculated ) % p != sq:
         error_tally = error_tally + 1
-        print "Failed to find %d as sqrt( %d ) mod %d. Said %d." % \
-              ( root, sq, p, calculated )
+        print_("Failed to find %d as sqrt( %d ) mod %d. Said %d." % \
+              ( root, sq, p, calculated ))
 
     for nonsquare in range( 0, p ):
       if nonsquare not in squares:
         try:
           calculated = square_root_mod_prime( nonsquare, p )
         except SquareRootError:
           pass
         else:
           error_tally = error_tally + 1
-          print "Failed to report no root for sqrt( %d ) mod %d." % \
-                ( nonsquare, p )
+          print_("Failed to report no root for sqrt( %d ) mod %d." % \
+                ( nonsquare, p ))
 
   # Test the jacobi function:
   for m in range( 3, 400, 2 ):
-    print "Testing jacobi for modulus m = %d." % m
+    print_("Testing jacobi for modulus m = %d." % m)
     if is_prime( m ):
       squares = []
       for root in range( 1, m ):
         if jacobi( root * root, m ) != 1:
           error_tally = error_tally + 1
-          print "jacobi( %d * %d, %d ) != 1" % ( root, root, m )
+          print_("jacobi( %d * %d, %d ) != 1" % ( root, root, m ))
         squares.append( root * root % m )
       for i in range( 1, m ):
         if not i in squares:
           if jacobi( i, m ) != -1:
             error_tally = error_tally + 1
-            print "jacobi( %d, %d ) != -1" % ( i, m )
+            print_("jacobi( %d, %d ) != -1" % ( i, m ))
     else:       # m is not prime.
       f = factorization( m )
       for a in range( 1, m ):
         c = 1
         for i in f:
           c = c * jacobi( a, i[0] ) ** i[1]
         if c != jacobi( a, m ):
           error_tally = error_tally + 1
-          print "%d != jacobi( %d, %d )" % ( c, a, m )
+          print_("%d != jacobi( %d, %d )" % ( c, a, m ))
 
 
 # Test the inverse_mod function:
-  print "Testing inverse_mod . . ."
+  print_("Testing inverse_mod . . .")
   import random
   n_tests = 0
   for i in range( 100 ):
     m = random.randint( 20, 10000 )
     for j in range( 100 ):
       a = random.randint( 1, m-1 )
       if gcd( a, m ) == 1:
         n_tests = n_tests + 1
         inv = inverse_mod( a, m )
         if inv <= 0 or inv >= m or ( a * inv ) % m != 1:
           error_tally = error_tally + 1
-          print "%d = inverse_mod( %d, %d ) is wrong." % ( inv, a, m )
+          print_("%d = inverse_mod( %d, %d ) is wrong." % ( inv, a, m ))
   assert n_tests > 1000
-  print n_tests, " tests of inverse_mod completed."
+  print_(n_tests, " tests of inverse_mod completed.")
 
   class FailedTest(Exception): pass
-  print error_tally, "errors detected."
+  print_(error_tally, "errors detected.")
   if error_tally != 0:
     raise FailedTest("%d errors detected" % error_tally)
 
 if __name__ == '__main__':
   __main__()
```

### Comparing `ecdsa-0.8/ecdsa/util.py` & `ecdsa-0.9/ecdsa/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from __future__ import division
 
 import os
 import math
 import binascii
 from hashlib import sha256
-import der
-from curves import orderlen
+from . import der
+from .curves import orderlen
+from .six import PY3, int2byte, b, next
 
 # RFC5480:
 #   The "unrestricted" algorithm identifier is:
 #     id-ecPublicKey OBJECT IDENTIFIER ::= {
 #       iso(1) member-body(2) us(840) ansi-X9-62(10045) keyType(2) 1 }
 
 oid_ecPublicKey = (1, 2, 840, 10045, 2, 1)
@@ -60,20 +62,26 @@
     # primarily for the needs of randrange_from_seed__trytryagain(), which
     # only needs to run it a few times per seed. It does not provide
     # protection against state compromise (forward security).
     def __init__(self, seed):
         self.generator = self.block_generator(seed)
 
     def __call__(self, numbytes):
-        return "".join([self.generator.next() for i in range(numbytes)])
+        a = [next(self.generator) for i in range(numbytes)]
+
+        if PY3:
+            return bytes(a)
+        else:
+            return "".join(a)
+
 
     def block_generator(self, seed):
         counter = 0
         while True:
-            for byte in sha256("prng-%d-%s" % (counter, seed)).digest():
+            for byte in sha256(("prng-%d-%s" % (counter, seed)).encode()).digest():
                 yield byte
             counter += 1
 
 def randrange_from_seed__overshoot_modulo(seed, order):
     # hash the data, then turn the digest into a number in [1,order).
     #
     # We use David-Sarah Hopwood's suggestion: turn it into a number that's
@@ -122,15 +130,15 @@
     # half a bit
     bits = int(math.log(order-1, 2)+1)
     maxbytes = (bits+7) // 8
     base = hashmod(seed).digest()[:maxbytes]
     base = "\x00"*(maxbytes-len(base)) + base
     topbits = 8*maxbytes - bits
     if topbits:
-        base = chr(ord(base[0]) & lsb_of_ones(topbits)) + base[1:]
+        base = int2byte(ord(base[0]) & lsb_of_ones(topbits)) + base[1:]
     number = 1+int(binascii.hexlify(base), 16)
     assert 1 <= number < order
     return number
 
 def randrange_from_seed__trytryagain(seed, order):
     # figure out exactly how many bits we need (rounded up to the nearest
     # bit), so we can reduce the chance of looping to less than 0.5 . This is
@@ -138,29 +146,35 @@
     # high-order bits of the first byte as necessary to get the right number
     # of bits. The average number of loops will range from 1.0 (when
     # order=2**k-1) to 2.0 (when order=2**k+1).
     assert order > 1
     bits, bytes, extrabits = bits_and_bytes(order)
     generate = PRNG(seed)
     while True:
-        extrabyte = ""
+        extrabyte = b("")
         if extrabits:
-            extrabyte = chr(ord(generate(1)) & lsb_of_ones(extrabits))
+            extrabyte = int2byte(ord(generate(1)) & lsb_of_ones(extrabits))
         guess = string_to_number(extrabyte + generate(bytes)) + 1
         if 1 <= guess < order:
             return guess
 
 
 def number_to_string(num, order):
     l = orderlen(order)
     fmt_str = "%0" + str(2*l) + "x"
-    string = binascii.unhexlify(fmt_str % num)
+    string = binascii.unhexlify((fmt_str % num).encode())
     assert len(string) == l, (len(string), l)
     return string
 
+def number_to_string_crop(num, order):
+    l = orderlen(order)
+    fmt_str = "%0" + str(2*l) + "x"
+    string = binascii.unhexlify((fmt_str % num).encode())
+    return string[:l]
+
 def string_to_number(string):
     return int(binascii.hexlify(string), 16)
 
 def string_to_number_fixedlen(string, order):
     l = orderlen(order)
     assert len(string) == l, (len(string), l)
     return int(binascii.hexlify(string), 16)
@@ -199,17 +213,17 @@
     r = string_to_number_fixedlen(r_str, order)
     s = string_to_number_fixedlen(s_str, order)
     return r, s
 
 def sigdecode_der(sig_der, order):
     #return der.encode_sequence(der.encode_integer(r), der.encode_integer(s))
     rs_strings, empty = der.remove_sequence(sig_der)
-    if empty != "":
+    if empty != b(""):
         raise der.UnexpectedDER("trailing junk after DER sig: %s" %
                                 binascii.hexlify(empty))
     r, rest = der.remove_integer(rs_strings)
     s, empty = der.remove_integer(rest)
-    if empty != "":
+    if empty != b(""):
         raise der.UnexpectedDER("trailing junk after DER numbers: %s" %
                                 binascii.hexlify(empty))
     return r, s
```

