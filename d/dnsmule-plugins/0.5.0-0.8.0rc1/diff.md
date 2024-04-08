# Comparing `tmp/dnsmule-plugins-0.5.0.tar.gz` & `tmp/dnsmule-plugins-0.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnsmule-plugins-0.5.0.tar", last modified: Sat May 13 17:41:07 2023, max compression
+gzip compressed data, was "dnsmule-plugins-0.8.0rc1.tar", last modified: Mon Apr  8 13:36:22 2024, max compression
```

## Comparing `dnsmule-plugins-0.5.0.tar` & `dnsmule-plugins-0.8.0rc1.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:41:07.233670 dnsmule-plugins-0.5.0/
--rw-r--r--   0 jonium     (501) staff       (20)     4693 2023-05-13 17:41:07.233469 dnsmule-plugins-0.5.0/PKG-INFO
--rw-r--r--   0 jonium     (501) staff       (20)     3934 2023-05-09 13:07:06.000000 dnsmule-plugins-0.5.0/README.md
--rw-r--r--   0 jonium     (501) staff       (20)       38 2023-05-13 17:41:07.233719 dnsmule-plugins-0.5.0/setup.cfg
--rw-r--r--   0 jonium     (501) staff       (20)     1597 2023-05-13 11:43:22.000000 dnsmule-plugins-0.5.0/setup.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:41:07.223397 dnsmule-plugins-0.5.0/src/
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:41:07.224430 dnsmule-plugins-0.5.0/src/dnsmule_plugins/
--rw-r--r--   0 jonium     (501) staff       (20)      134 2023-05-09 13:07:06.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/__init__.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:41:07.227088 dnsmule-plugins-0.5.0/src/dnsmule_plugins/certcheck/
--rw-r--r--   0 jonium     (501) staff       (20)      569 2023-05-13 12:34:45.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/certcheck/__init__.py
--rw-r--r--   0 jonium     (501) staff       (20)      591 2023-05-10 11:29:17.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/certcheck/adapter.py
--rw-r--r--   0 jonium     (501) staff       (20)     5514 2023-05-10 10:10:12.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/certcheck/certificates.py
--rw-r--r--   0 jonium     (501) staff       (20)      842 2023-05-12 15:44:26.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/certcheck/domains.py
--rw-r--r--   0 jonium     (501) staff       (20)     1608 2023-05-13 12:34:45.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/certcheck/rule.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:41:07.227957 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/
--rw-r--r--   0 jonium     (501) staff       (20)      271 2023-05-10 10:10:12.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/__init__.py
--rw-r--r--   0 jonium     (501) staff       (20)      791 2023-05-13 11:18:33.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/iprange.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:41:07.230319 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/
--rw-r--r--   0 jonium     (501) staff       (20)      302 2023-05-12 23:14:04.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/__init__.py
--rw-r--r--   0 jonium     (501) staff       (20)     1373 2023-05-13 12:10:26.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/_core.py
--rw-r--r--   0 jonium     (501) staff       (20)      557 2023-05-12 22:46:44.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/amazon.py
--rw-r--r--   0 jonium     (501) staff       (20)      612 2023-05-13 11:16:35.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/cloudflare.py
--rw-r--r--   0 jonium     (501) staff       (20)      517 2023-05-12 23:00:03.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/digitalocean.py
--rw-r--r--   0 jonium     (501) staff       (20)      979 2023-05-12 22:46:44.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/google.py
--rw-r--r--   0 jonium     (501) staff       (20)     1671 2023-05-12 23:07:19.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/microsoft.py
--rw-r--r--   0 jonium     (501) staff       (20)     2462 2023-05-13 12:36:23.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/rule.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:41:07.230876 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ptrscan/
--rw-r--r--   0 jonium     (501) staff       (20)      277 2023-05-10 10:10:12.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ptrscan/__init__.py
--rw-r--r--   0 jonium     (501) staff       (20)     1605 2023-05-10 10:10:12.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins/ptrscan/rule.py
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:41:07.225288 dnsmule-plugins-0.5.0/src/dnsmule_plugins.egg-info/
--rw-r--r--   0 jonium     (501) staff       (20)     4693 2023-05-13 17:41:07.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins.egg-info/PKG-INFO
--rw-r--r--   0 jonium     (501) staff       (20)     1231 2023-05-13 17:41:07.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 jonium     (501) staff       (20)        1 2023-05-13 17:41:07.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 jonium     (501) staff       (20)       67 2023-05-13 17:41:07.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins.egg-info/requires.txt
--rw-r--r--   0 jonium     (501) staff       (20)       16 2023-05-13 17:41:07.000000 dnsmule-plugins-0.5.0/src/dnsmule_plugins.egg-info/top_level.txt
-drwxr-xr-x   0 jonium     (501) staff       (20)        0 2023-05-13 17:41:07.233101 dnsmule-plugins-0.5.0/test/
--rw-r--r--   0 jonium     (501) staff       (20)     2952 2023-05-13 12:36:53.000000 dnsmule-plugins-0.5.0/test/test_certcheck.py
--rw-r--r--   0 jonium     (501) staff       (20)     1248 2023-05-10 11:26:14.000000 dnsmule-plugins-0.5.0/test/test_certcheck_adapter.py
--rw-r--r--   0 jonium     (501) staff       (20)      785 2023-05-12 15:46:10.000000 dnsmule-plugins-0.5.0/test/test_certcheck_domains.py
--rw-r--r--   0 jonium     (501) staff       (20)     9345 2023-05-09 13:07:06.000000 dnsmule-plugins-0.5.0/test/test_certificates.py
--rw-r--r--   0 jonium     (501) staff       (20)     2478 2023-05-12 22:46:44.000000 dnsmule-plugins-0.5.0/test/test_ipranges.py
--rw-r--r--   0 jonium     (501) staff       (20)      692 2023-05-09 13:07:06.000000 dnsmule-plugins-0.5.0/test/test_plugins_registration.py
--rw-r--r--   0 jonium     (501) staff       (20)     3280 2023-05-09 13:07:06.000000 dnsmule-plugins-0.5.0/test/test_ptrscan.py
--rw-r--r--   0 jonium     (501) staff       (20)     2028 2023-05-13 12:13:57.000000 dnsmule-plugins-0.5.0/test/test_ranges.py
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:22.115558 dnsmule-plugins-0.8.0rc1/
+-rw-r--r--   0 jonium     (501) staff       (20)     4888 2024-04-08 13:36:22.115357 dnsmule-plugins-0.8.0rc1/PKG-INFO
+-rw-r--r--   0 jonium     (501) staff       (20)     3934 2023-05-09 13:07:06.000000 dnsmule-plugins-0.8.0rc1/README.md
+-rw-r--r--   0 jonium     (501) staff       (20)       38 2024-04-08 13:36:22.115593 dnsmule-plugins-0.8.0rc1/setup.cfg
+-rw-r--r--   0 jonium     (501) staff       (20)     1597 2023-05-13 11:43:22.000000 dnsmule-plugins-0.8.0rc1/setup.py
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:22.108479 dnsmule-plugins-0.8.0rc1/src/
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:22.109090 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/
+-rw-r--r--   0 jonium     (501) staff       (20)      127 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/__init__.py
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:22.111165 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/certcheck/
+-rw-r--r--   0 jonium     (501) staff       (20)      110 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/certcheck/__init__.py
+-rw-r--r--   0 jonium     (501) staff       (20)      591 2023-05-10 11:29:17.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/certcheck/adapter.py
+-rw-r--r--   0 jonium     (501) staff       (20)     5549 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/certcheck/certificates.py
+-rw-r--r--   0 jonium     (501) staff       (20)      842 2023-05-12 15:44:26.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/certcheck/domains.py
+-rw-r--r--   0 jonium     (501) staff       (20)     1013 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/certcheck/rule.py
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:22.111777 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/
+-rw-r--r--   0 jonium     (501) staff       (20)       70 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/__init__.py
+-rw-r--r--   0 jonium     (501) staff       (20)      791 2023-05-13 11:18:33.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/iprange.py
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:22.113457 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/
+-rw-r--r--   0 jonium     (501) staff       (20)      302 2023-05-12 23:14:04.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/__init__.py
+-rw-r--r--   0 jonium     (501) staff       (20)     1373 2023-05-13 12:10:26.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/_core.py
+-rw-r--r--   0 jonium     (501) staff       (20)      557 2023-05-12 22:46:44.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/amazon.py
+-rw-r--r--   0 jonium     (501) staff       (20)      612 2023-05-13 11:16:35.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/cloudflare.py
+-rw-r--r--   0 jonium     (501) staff       (20)      517 2023-05-12 23:00:03.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/digitalocean.py
+-rw-r--r--   0 jonium     (501) staff       (20)      979 2023-05-12 22:46:44.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/google.py
+-rw-r--r--   0 jonium     (501) staff       (20)     1671 2023-05-12 23:07:19.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/microsoft.py
+-rw-r--r--   0 jonium     (501) staff       (20)     4058 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/rule.py
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:22.113789 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ptrscan/
+-rw-r--r--   0 jonium     (501) staff       (20)       55 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ptrscan/__init__.py
+-rw-r--r--   0 jonium     (501) staff       (20)     1453 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ptrscan/rule.py
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:22.114950 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins.egg-info/
+-rw-r--r--   0 jonium     (501) staff       (20)     4888 2024-04-08 13:36:22.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 jonium     (501) staff       (20)     1197 2024-04-08 13:36:22.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 jonium     (501) staff       (20)        1 2024-04-08 13:36:22.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 jonium     (501) staff       (20)       67 2024-04-08 13:36:22.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins.egg-info/requires.txt
+-rw-r--r--   0 jonium     (501) staff       (20)       16 2024-04-08 13:36:22.000000 dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 jonium     (501) staff       (20)        0 2024-04-08 13:36:22.114775 dnsmule-plugins-0.8.0rc1/test/
+-rw-r--r--   0 jonium     (501) staff       (20)     2132 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/test/test_certcheck.py
+-rw-r--r--   0 jonium     (501) staff       (20)     1256 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/test/test_certcheck_adapter.py
+-rw-r--r--   0 jonium     (501) staff       (20)      785 2023-05-12 15:46:10.000000 dnsmule-plugins-0.8.0rc1/test/test_certcheck_domains.py
+-rw-r--r--   0 jonium     (501) staff       (20)     9394 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/test/test_certificates.py
+-rw-r--r--   0 jonium     (501) staff       (20)     2663 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/test/test_ipranges.py
+-rw-r--r--   0 jonium     (501) staff       (20)     3270 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/test/test_ptrscan.py
+-rw-r--r--   0 jonium     (501) staff       (20)     2218 2024-04-08 13:27:27.000000 dnsmule-plugins-0.8.0rc1/test/test_ranges.py
```

### Comparing `dnsmule-plugins-0.5.0/PKG-INFO` & `dnsmule-plugins-0.8.0rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnsmule-plugins
-Version: 0.5.0
+Version: 0.8.0rc1
 Summary: Plugins for DNSMule
 Home-page: https://github.com/joniumGit/dnsmule
 Author: joniumGit
 Author-email: 52005121+joniumGit@users.noreply.github.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/joniumGit/dnsmule/issues
 Project-URL: Source, https://github.com/joniumGit/dnsmule
@@ -13,16 +13,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: dnsmule
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: cryptography; extra == "dev"
 Provides-Extra: full
+Requires-Dist: cryptography; extra == "full"
 
 # Plugins for DNSMule
 
 It is recommended to look through each module to see what arguments they take.
 
 #### Certcheck
```

### Comparing `dnsmule-plugins-0.5.0/README.md` & `dnsmule-plugins-0.8.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dnsmule-plugins-0.5.0/setup.py` & `dnsmule-plugins-0.8.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins/certcheck/adapter.py` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/certcheck/adapter.py`

 * *Files identical despite different names*

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins/certcheck/certificates.py` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/certcheck/certificates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import socket
 import ssl
 from dataclasses import dataclass
+from logging import getLogger
 from typing import List, Optional, Tuple
 
-from dnsmule.logger import get_logger
+LOGGER = 'dnsmule.plugins.certcheck'
 
 
 @dataclass(frozen=True, eq=True)
 class Certificate:
     version: str
     common: str
     alts: List[str]
@@ -65,15 +66,15 @@
             'valid_from': cert.not_valid_before,
             'version': cert.version.name,
         }
         return cert
     except ImportError:
         pass
     except Exception as e:
-        get_logger().warning(
+        getLogger(LOGGER).debug(
             'CERTS-CRYPTOGRAPHY: Failed to get cert for %s:%s (%s)',
             *address.tuple[0:2],
             repr(e),
         )
 
 
 def issuer_str(issuer):
@@ -121,15 +122,15 @@
         ctx.check_hostname = False
         with socket.socket(address.family, socket.SOCK_STREAM) as raw_socket:
             raw_socket.settimeout(timeout)
             with ctx.wrap_socket(raw_socket, do_handshake_on_connect=True) as s:
                 s.connect(address.tuple)
                 return massage_certificate_stdlib(s.getpeercert(binary_form=False))
     except Exception as e:
-        get_logger().warning(
+        getLogger(LOGGER).debug(
             'CERTS-STDLIB: Failed to get cert for %s:%s (%s)',
             *address.tuple[0:2],
             repr(e),
         )
 
 
 def collect_certificate(
```

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins/certcheck/domains.py` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/certcheck/domains.py`

 * *Files identical despite different names*

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins/certcheck/rule.py` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ptrscan/rule.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,53 @@
-from typing import Callable, Collection, List, Optional
+import ipaddress
 
-from dnsmule import Rule, Result, Record
+from dnsmule import Record, RRType, Domain, Result
 from dnsmule.utils import extend_set
-from . import certificates
-from .domains import process_domains
-from .adapter import load_result, save_result
 
 
-class CertChecker(Rule):
-    id = 'ip.certs'
+class PTRScan:
+    type = 'ip.ptr'
 
-    ports: List[int] = [443, 8443]
-    timeout: float = 1
-    stdlib: bool = False
-    callback: bool = False
-
-    _callback: Callable[[str, ...], None]
+    context: dict
 
     @staticmethod
-    def creator(callback: Optional[Callable[[Collection[str]], None]]):
-        def registerer(**kwargs):
-            rule = CertChecker(**kwargs)
-            rule._callback = callback
-            return rule
-
-        return registerer
-
-    def __call__(self, record: Record) -> Result:
-        certs = {
-            cert
-            for port in self.ports
-            for cert in certificates.collect_certificates(
-                record.text,
-                port=port,
-                timeout=self.timeout,
-                prefer_stdlib=self.stdlib,
+    def reverse_query(ip: str) -> Domain:
+        return Domain(ipaddress.ip_address(ip).reverse_pointer)
+
+    @property
+    def mule(self):
+        return self.context['mule']
+
+    def __call__(self, record: Record, result: Result):
+        address = record.text
+        ptr_patterns = [
+            '-'.join(reversed(address.split('.'))),
+            '.'.join(reversed(address.split('.'))),
+            address,
+            '-'.join(address.split('.')),
+        ]
+        ptrs = [
+            ptr.text
+            for ptr in self.mule.backend.scan(
+                self.reverse_query(record.text),
+                RRType.PTR,
             )
-        }
-        if certs:
-            load_result(record.result)
-            extend_set(record.result.data, 'resolvedCertificates', certs)
-            save_result(record.result)
-            if self.callback:
-                domains = [*process_domains(
-                    domain
-                    for cert in certs
-                    for domain in certificates.resolve_domain_from_certificate(cert)
-                    if domain != record.domain
-                )]
-                self._callback(*domains)
-        return record.result
+        ]
+        if ptrs:
+            for ptr in ptrs:
+                for pattern in ptr_patterns:
+                    if pattern in ptr:
+                        if ptr.startswith(pattern):
+                            _id = ptr.removeprefix(pattern)
+                        else:
+                            _id = ptr.partition(pattern)[2]
+                        result.tags.add(
+                            f'IP::PTR'
+                            f'::{_id.strip(".").upper()}'
+                        )
+                        break
+            extend_set(result.data, 'resolvedPointers', *ptrs)
 
 
 __all__ = [
-    'CertChecker',
+    'PTRScan',
 ]
```

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/iprange.py` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/iprange.py`

 * *Files identical despite different names*

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/_core.py` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/_core.py`

 * *Files identical despite different names*

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/amazon.py` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/amazon.py`

 * *Files identical despite different names*

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/cloudflare.py` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/digitalocean.py` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/digitalocean.py`

 * *Files identical despite different names*

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/google.py` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/google.py`

 * *Files identical despite different names*

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/providers/microsoft.py` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/providers/microsoft.py`

 * *Files identical despite different names*

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins/ipranges/rule.py` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins/ipranges/rule.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,117 @@
-import asyncio
+import dataclasses
 import datetime
+import json
 from concurrent.futures import ThreadPoolExecutor, wait, ALL_COMPLETED
+from logging import getLogger
 from typing import List, Optional, Dict, cast
 
-from dnsmule.definitions import Record, Result
-from dnsmule.logger import get_logger
-from dnsmule.rules import Rule
+from dnsmule import Record, Result
 from .iprange import IPvXRange
 from .providers import Providers
 
+LOGGER = 'dnsmule.plugins.ipranges'
 
-class IpRangeChecker(Rule):
-    id = 'ip.ranges'
 
-    providers: List[str]
-    interval_hours: int = 10
+class IpRangeChecker:
+    type = 'ip.ranges'
 
-    _last_fetch: Optional[datetime.datetime] = None
     _provider_ranges: Dict[str, List[IPvXRange]]
-    _task: asyncio.Task
+    _last_fetch: Optional[datetime.datetime] = None
 
-    def __init__(self, **kwargs):
-        kwargs['code'] = 'pass'
-        super().__init__(**kwargs)
-        self.globals = {}
-        self.providers = [*{*self.providers}] if hasattr(self, 'providers') else Providers.all()
-        self._provider_ranges = cast(Dict[str, List[IPvXRange]], {})
-        for provider in self.providers:
+    def __init__(
+            self,
+            *,
+            providers: Optional[List[str]] = None,
+            interval_hours: int = 10,
+            cache: bool = False,
+    ):
+        if providers is not None:
+            providers = [*{*providers}]
+        else:
+            providers = Providers.all()
+        for provider in providers:
             if not Providers.available(provider):
                 raise KeyError(f'Provider {provider} does not exist')
+        self.providers = providers
+        self.interval_hours = interval_hours
+        self.cache = cache
+        self._provider_ranges = cast(Dict[str, List[IPvXRange]], {})
+
+    def __enter__(self):
+        self._executor = ThreadPoolExecutor()
+        self._executor.__enter__()
+        if self.cache:
+            try:
+                with open('ipranges-cache.json', 'r') as f:
+                    data = json.load(f)
+                    self._last_fetch = datetime.datetime.fromisoformat(data['last_fetch'])
+                    self._provider_ranges = {
+                        provider: [IPvXRange.create(**item) for item in items]
+                        for provider, items in data['items'].items()
+                    }
+            except (FileNotFoundError, json.JSONDecodeError):
+                """Ignored
+                """
+        self.check_fetch()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self._executor.__exit__(exc_type, exc_val, exc_tb)
 
     def fetch_provider(self, provider: str):
         self._provider_ranges[provider] = Providers.fetch(provider)
 
     def fetch_ranges(self):
-        with ThreadPoolExecutor() as tp:
-            tasks = []
-            for k in self.providers:
-                tasks.append(tp.submit(self.fetch_provider, k))
-            if tasks:
-                wait(tasks, return_when=ALL_COMPLETED)
-                for t in tasks:
-                    if t.done() and t.exception() is not None:
-                        get_logger().error('Failed to fetch ranges', exc_info=t.exception())
+        tasks = []
+        for k in self.providers:
+            tasks.append(self._executor.submit(self.fetch_provider, k))
+        if tasks:
+            wait(tasks, return_when=ALL_COMPLETED)
+            for t in tasks:
+                if t.done() and t.exception() is not None:
+                    getLogger(LOGGER).error(
+                        'Failed to fetch ranges',
+                        exc_info=t.exception(),
+                    )
 
     def check_fetch(self):
         if (
                 not self._last_fetch
                 or abs(datetime.datetime.now() - self._last_fetch) > datetime.timedelta(hours=self.interval_hours)
         ):
             self.fetch_ranges()
             self._last_fetch = datetime.datetime.now()
+            if self.cache:
+                with open('ipranges-cache.json', 'w') as f:
+                    json.dump(
+                        {
+                            'last_fetch': self._last_fetch.isoformat(),
+                            'items': {
+                                provider: [
+                                    dataclasses.asdict(item)
+                                    for item in items
+                                ]
+                                for provider, items in self._provider_ranges.items()
+                            }
+                        },
+                        f,
+                        default=str,
+                        indent=4,
+                        ensure_ascii=False,
+                    )
 
-    def __call__(self, record: Record) -> Result:
+    def __call__(self, record: Record, result: Result):
         self.check_fetch()
         address: str = record.text
         for provider, p_ranges in self._provider_ranges.items():
             for p_range in p_ranges:
                 if address in p_range:
-                    record.result.tags.add(
+                    result.tags.add(
                         f'IP::RANGES'
-                        f'::{self.name.upper()}'
                         f'::{p_range.service.upper()}'
                         f'::{p_range.region.upper()}'
                     )
-        return record.result
 
 
 __all__ = [
     'IpRangeChecker',
 ]
```

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins.egg-info/PKG-INFO` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnsmule-plugins
-Version: 0.5.0
+Version: 0.8.0rc1
 Summary: Plugins for DNSMule
 Home-page: https://github.com/joniumGit/dnsmule
 Author: joniumGit
 Author-email: 52005121+joniumGit@users.noreply.github.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/joniumGit/dnsmule/issues
 Project-URL: Source, https://github.com/joniumGit/dnsmule
@@ -13,16 +13,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: dnsmule
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: cryptography; extra == "dev"
 Provides-Extra: full
+Requires-Dist: cryptography; extra == "full"
 
 # Plugins for DNSMule
 
 It is recommended to look through each module to see what arguments they take.
 
 #### Certcheck
```

### Comparing `dnsmule-plugins-0.5.0/src/dnsmule_plugins.egg-info/SOURCES.txt` & `dnsmule-plugins-0.8.0rc1/src/dnsmule_plugins.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,10 +24,9 @@
 src/dnsmule_plugins/ptrscan/__init__.py
 src/dnsmule_plugins/ptrscan/rule.py
 test/test_certcheck.py
 test/test_certcheck_adapter.py
 test/test_certcheck_domains.py
 test/test_certificates.py
 test/test_ipranges.py
-test/test_plugins_registration.py
 test/test_ptrscan.py
 test/test_ranges.py
```

### Comparing `dnsmule-plugins-0.5.0/test/test_certcheck_adapter.py` & `dnsmule-plugins-0.8.0rc1/test/test_certcheck_adapter.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,30 +11,30 @@
     valid_from=datetime.datetime.now(),
     valid_until=datetime.datetime.now(),
     alts=[],
 )
 
 
 def test_saving():
-    result = Result(Domain('example.com'), RRType.TXT)
+    result = Result(Domain('example.com'), [RRType.TXT])
     result.data['resolvedCertificates'] = {test_cert}
     result = save_result(result)
     assert result.data['resolvedCertificates'] == [test_cert.to_json()]
 
 
 def test_loading():
-    result = Result(Domain('example.com'), RRType.TXT)
+    result = Result(Domain('example.com'), [RRType.TXT])
     result.data['resolvedCertificates'] = [test_cert.to_json()]
     result = load_result(result)
     assert result.data['resolvedCertificates'] == {test_cert}
 
 
 def test_saving_no_key():
-    result = Result(Domain('example.com'), RRType.TXT)
+    result = Result(Domain('example.com'), [RRType.TXT])
     result = save_result(result)
     assert 'resolvedCertificates' not in result.data, 'Added key when not present'
 
 
 def test_loading_no_key():
-    result = Result(Domain('example.com'), RRType.TXT)
+    result = Result(Domain('example.com'), [RRType.TXT])
     result = load_result(result)
     assert 'resolvedCertificates' not in result.data, 'Added key when not present'
```

### Comparing `dnsmule-plugins-0.5.0/test/test_certcheck_domains.py` & `dnsmule-plugins-0.8.0rc1/test/test_certcheck_domains.py`

 * *Files identical despite different names*

### Comparing `dnsmule-plugins-0.5.0/test/test_certificates.py` & `dnsmule-plugins-0.8.0rc1/test/test_certificates.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,21 +161,24 @@
 
 def test_import_error_2(monkeypatch):
     def thrower(*_, **__):
         raise ImportError()
 
     class FailLogger:
 
+        def __init__(self, *_):
+            pass
+
         @staticmethod
         def warning(*o):
             pytest.fail(repr(o))
 
     with monkeypatch.context() as m:
         m.setattr(ssl, 'get_server_certificate', thrower)
-        m.setattr(certificates, 'get_logger', FailLogger)
+        m.setattr(certificates, 'getLogger', FailLogger)
         cert = certificates.collect_certificate_cryptography(EXAMPLE_ADDRESS, 1.)
     assert cert is None, 'Failed to pass on exception'
 
 
 def test_collect_certificates(monkeypatch, mock_cert_stdlib):
     with monkeypatch.context() as m:
         m.setattr(socket, 'getaddrinfo', lambda *_, **__: [
```

### Comparing `dnsmule-plugins-0.5.0/test/test_ipranges.py` & `dnsmule-plugins-0.8.0rc1/test/test_ipranges.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,94 @@
 import datetime
 from ipaddress import IPv4Network
 from time import sleep
 
 import pytest
 
-from dnsmule import Record, RRType
 from dnsmule_plugins.ipranges.iprange import IPvXRange
 from dnsmule_plugins.ipranges.rule import IpRangeChecker
 
 
-def test_task():
+def test_fetching_add_last_fetch():
     checker = IpRangeChecker(providers=[])
 
     assert checker._last_fetch is None, 'Spawned with fetch time'
 
     def fetch_ranges():
         sleep(.1)
 
     checker.fetch_ranges = fetch_ranges
 
     checker.check_fetch()
 
-    assert not hasattr(checker, '_task'), 'Task did not get deleted'
     assert checker._last_fetch is not None, 'Missing fetch time'
 
 
-def test_task_if_task_exists():
+def test_context_should_fetch_on_enter():
     checker = IpRangeChecker(providers=[])
     called = []
 
     def fetch_ranges():
         called.append('fetch')
 
     checker.fetch_ranges = fetch_ranges
 
-    checker.check_fetch()
+    with checker:
+        pass
+
     assert called == ['fetch'], 'Not fetched'
 
 
+def test_context_should_not_fetch_on_enter_if_recently_fetched():
+    checker = IpRangeChecker(providers=[])
+    called = []
+
+    def fetch_ranges():
+        called.append('fetch')
+
+    checker.fetch_ranges = fetch_ranges
+    checker._last_fetch = datetime.datetime.now()
+
+    with checker:
+        pass
+
+    assert called == [], 'Fetched twice'
+
+
 def test_unknown_provider():
     with pytest.raises(Exception):
         IpRangeChecker(providers=['adwadawdawdawdwad'])
 
 
-def test_provider_tags():
-    rule = IpRangeChecker(providers=[], name='test_rule')
+def test_provider_tags(record, result):
+    rule = IpRangeChecker(providers=[])
     rule._provider_ranges['test_provider'] = [IPvXRange(
         address=IPv4Network('127.0.0.0/31'),
         region='test_region',
         service='test_service',
     )]
-    r = Record('', RRType.A, '127.0.0.1')
     rule._last_fetch = datetime.datetime.now()
-    rule(r)
-    assert 'IP::RANGES::TEST_RULE::TEST_SERVICE::TEST_REGION' in r.result
+    rule(record, result)
+    assert 'IP::RANGES::TEST_SERVICE::TEST_REGION' in result.tags
 
 
-def test_provider_no_tags_if_no_match():
-    rule = IpRangeChecker(providers=[], name='test_rule')
+def test_provider_no_tags_if_no_match(record, result):
+    rule = IpRangeChecker(providers=[])
     rule._provider_ranges['test_provider'] = [IPvXRange(
         address=IPv4Network('128.0.0.0/24'),
         region='test_region',
         service='test_service',
     )]
-    r = Record('', RRType.A, '127.0.0.1')
     rule._last_fetch = datetime.datetime.now()
-    rule(r)
-    assert len(r.result.tags) == 0, 'Had a tag'
+    rule(record, result)
+    assert len(result.tags) == 0, 'Had a tag'
 
 
 def test_provider_empty_provider_fetch_ok():
-    rule = IpRangeChecker(providers=[], name='test_rule')
+    rule = IpRangeChecker(providers=[])
     rule.check_fetch()
     assert rule._last_fetch is not None, 'Failed fetch'
 
 
 def test_fetcher_for_provider(monkeypatch):
     sentinel = object()
     with monkeypatch.context() as m:
```

### Comparing `dnsmule-plugins-0.5.0/test/test_ptrscan.py` & `dnsmule-plugins-0.8.0rc1/test/test_ptrscan.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,111 +1,116 @@
-from typing import Any
-
 import pytest
 
-from dnsmule import DNSMule, Record, RRType, Domain
+from dnsmule import DNSMule, Record, RRType, Domain, Rules
+from dnsmule import DictStorage, DataBackend
 from dnsmule_plugins.ptrscan.rule import PTRScan
 
 
 def test_init_no_backend():
     r = PTRScan()
     assert not hasattr(r, '_mule'), 'Had mule on create'
 
 
-def test_creator_appends_backend():
-    marker: Any = object()
-    creator = PTRScan.creator(marker)
-    r = creator()
-    assert r._mule is marker, 'Failed to set mule to marker'
-
-
 def test_reverses_ipv4():
     assert PTRScan.reverse_query('127.0.0.1') == '1.0.0.127.in-addr.arpa'
 
 
 def test_reverses_ipv6():
     res = 'b.a.9.8.7.6.5.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.8.b.d.0.1.0.0.2.ip6.arpa'
     assert PTRScan.reverse_query('2001:db8::567:89ab') == res
 
 
-def test_with_mock_empty_result():
-    mule = DNSMule.make()
-    r = PTRScan.creator(mule)(name='test')
-
+def test_with_mock_empty_result(record, result):
     def run_single(domain, rtype):
         assert domain == '1.0.0.127.in-addr.arpa'
         assert rtype == RRType.PTR
         for _ in []:
             yield
 
-    mule.backend.single = run_single
+    mule = DNSMule(
+        storage=DictStorage(),
+        backend=DataBackend(),
+        rules=Rules()
+    )
+    mule.backend.scan = run_single
 
-    # This also checks dupes
-    r(Record(Domain('example.com'), RRType.A, '127.0.0.1'))
-    result = r(Record(Domain('example.com'), RRType.A, '127.0.0.1'))
+    rule = PTRScan()
+    mule.rules.register(RRType.A, rule)
 
+    mule._run_rule(rule, record, result)
     assert len(result.tags) == 0, 'Identified empty'
     assert 'resolvedPointers' not in result.data, 'Added pointers'
 
 
-def test_with_mock():
-    mule = DNSMule.make()
-    r = PTRScan.creator(mule)(name='test')
-
+def test_with_mock(record, result):
     def run_single(domain, rtype):
         assert domain == '1.0.0.127.in-addr.arpa'
         assert rtype == RRType.PTR
-        yield Record(Domain('1.0.0.127.in-addr.arpa'), RRType.PTR, '127.0.0.1.provider.com')
+        yield Record(
+            Domain('1.0.0.127.in-addr.arpa'),
+            RRType.PTR,
+            '127.0.0.1.provider.com',
+        )
+
+    mule = DNSMule(
+        storage=DictStorage(),
+        backend=DataBackend(),
+        rules=Rules()
+    )
+    mule.backend.scan = run_single
 
-    mule.backend.single = run_single
-
-    # This also checks dupes
-    r(Record(Domain('example.com'), RRType.A, '127.0.0.1'))
-    result = r(Record(Domain('example.com'), RRType.A, '127.0.0.1'))
+    rule = PTRScan()
+    mule.rules.register(RRType.A, rule)
 
+    mule._run_rule(rule, record, result)
     assert len(result.tags) != 0, 'Failed to identify'
-    assert result.tags.pop() == 'IP::PTR::TEST::PROVIDER.COM'
+    assert result.tags.pop() == 'IP::PTR::PROVIDER.COM'
     assert result.data['resolvedPointers'] == ['127.0.0.1.provider.com']
 
 
 @pytest.mark.parametrize('ptr', [
     '127-0-0-1-provider.com',
     '127.0.0.1.provider.com',
     '1.0.0.127.provider.com',
     '127-0-0-1.provider.com',
     '1-0-0-127.provider.com',
     'cdn-127-0-0-1.provider.com',
     'cdn.127.0.0.1.provider.com',
 ])
-def test_with_mock_no_dupes_and_ptr_appended(ptr):
-    mule = DNSMule.make()
-    r = PTRScan.creator(mule)(name='test')
-
+def test_with_mock_no_dupes_and_ptr_appended(ptr, record, result):
     def run_single(*_):
         yield Record(Domain('1.0.0.127.in-addr.arpa'), RRType.PTR, ptr)
 
-    mule.backend.single = run_single
+    mule = DNSMule(
+        storage=DictStorage(),
+        backend=DataBackend(),
+        rules=Rules()
+    )
+    mule.backend.scan = run_single
 
-    # Adds ptr
-    record = Record(Domain('example.com'), RRType.A, '127.0.0.1')
-    record.result.data['resolvedPointers'] = ['sample-127.0.0.1.provider.com', 'sample-127.0.0.1.provider.com']
+    rule = PTRScan()
+    mule.rules.register(RRType.A, rule)
 
-    r(record)
-    result = r(record)
+    # Adds ptr
+    result.data['resolvedPointers'] = ['sample-127.0.0.1.provider.com', 'sample-127.0.0.1.provider.com']
 
+    mule._run_rule(rule, record, result)
     assert len(result.data['resolvedPointers']) == 2, 'Failed to prevent or remove duplicate'
 
 
-def test_with_mock_ptr_no_match():
-    mule = DNSMule.make()
-    r = PTRScan.creator(mule)(name='test')
-
+def test_with_mock_ptr_no_match(record, result):
     def run_single(*_):
         yield Record(Domain('1.0.0.127.in-addr.arpa'), RRType.PTR, 'aaaa')
 
-    mule.backend.single = run_single
+    mule = DNSMule(
+        storage=DictStorage(),
+        backend=DataBackend(),
+        rules=Rules()
+    )
+    mule.backend.scan = run_single
 
-    record = Record(Domain('example.com'), RRType.A, '127.0.0.1')
+    rule = PTRScan()
+    mule.rules.register(RRType.A, rule)
 
-    result = r(record)
+    mule._run_rule(rule, record, result)
     assert len(result.tags) == 0, 'Identified'
     assert result.data['resolvedPointers'] == ['aaaa'], 'Failed to add ptr'
```

### Comparing `dnsmule-plugins-0.5.0/test/test_ranges.py` & `dnsmule-plugins-0.8.0rc1/test/test_ranges.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,54 +5,79 @@
 
 from dnsmule_plugins.ipranges import rule
 from dnsmule_plugins.ipranges.iprange import IPvXRange
 from dnsmule_plugins.ipranges.providers import Providers
 
 
 def test_ipvx_has_address_str():
-    r = IPvXRange(address=IPv4Network('127.0.0.0/24'), service='test', region='test-region')
+    r = IPvXRange(
+        address=IPv4Network('127.0.0.0/24'),
+        service='test',
+        region='test-region',
+    )
     assert '127.0.0.20' in r
 
 
 def test_ipvx_has_ipv6_address_str():
-    r = IPvXRange(address=IPv6Network('2001:db8:a::/64'), service='test', region='test-region')
+    r = IPvXRange(
+        address=IPv6Network('2001:db8:a::/64'),
+        service='test',
+        region='test-region',
+    )
     assert '2001:db8:a::123' in r
 
 
 def test_ipvx_has_address():
-    r = IPvXRange(address=IPv4Network('127.0.0.0/24'), service='test', region='test-region')
+    r = IPvXRange(
+        address=IPv4Network('127.0.0.0/24'),
+        service='test',
+        region='test-region',
+    )
     assert IPv4Address('127.0.0.20') in r
 
 
 def test_ipvx_has_no_network():
-    r = IPvXRange(address=IPv4Network('127.0.0.0/24'), service='test', region='test-region')
+    r = IPvXRange(
+        address=IPv4Network('127.0.0.0/24'),
+        service='test',
+        region='test-region',
+    )
     assert IPv4Network('127.0.0.0/31') not in r
 
 
 def test_ipvx_has_no_proto_mismatch():
-    r = IPvXRange(address=IPv4Network('127.0.0.0/24'), service='test', region='test-region')
+    r = IPvXRange(
+        address=IPv4Network('127.0.0.0/24'),
+        service='test',
+        region='test-region',
+    )
     assert '2001:db8:a::123' not in r
 
 
 def test_ipvx_network_raises():
-    r = IPvXRange(address=IPv4Network('127.0.0.0/24'), service='test', region='test-region')
+    r = IPvXRange(
+        address=IPv4Network('127.0.0.0/24'),
+        service='test',
+        region='test-region',
+    )
     assert '127.0.0.0/16' not in r
 
 
 def test_rule_fetching_failure_cancels_tasks():
     r = rule.IpRangeChecker(providers=[])
     r.providers = ['a', 'b']  # Prevents throw on init
 
     def fetch_provider(key):
         if key == 'b':
             raise ValueError()
 
     r.fetch_provider = fetch_provider
 
-    r.fetch_ranges()
+    with r:
+        pass
 
 
 @pytest.mark.skipif(os.getenv('FETCH_RANGES', 'false') != 'true', reason='Range fetch disabled')
 class TestRangesFetching:
 
     @pytest.fixture(params=Providers.all())
     def provider(self, request):
```

