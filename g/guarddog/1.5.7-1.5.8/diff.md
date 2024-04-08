# Comparing `tmp/guarddog-1.5.7.tar.gz` & `tmp/guarddog-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guarddog-1.5.7.tar", max compression
+gzip compressed data, was "guarddog-1.5.8.tar", max compression
```

## Comparing `guarddog-1.5.7.tar` & `guarddog-1.5.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0    11377 2024-04-03 15:42:21.654554 guarddog-1.5.7/LICENSE
--rw-r--r--   0        0        0      314 2024-04-03 15:42:21.654554 guarddog-1.5.7/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0      140 2024-04-03 15:42:21.654554 guarddog-1.5.7/NOTICE
--rw-r--r--   0        0        0      154 2024-04-03 15:42:21.654554 guarddog-1.5.7/guarddog/__init__.py
--rw-r--r--   0        0        0      246 2024-04-03 15:42:21.654554 guarddog-1.5.7/guarddog/__main__.py
--rw-r--r--   0        0        0        0 2024-04-03 15:42:21.654554 guarddog-1.5.7/guarddog/analyzer/__init__.py
--rw-r--r--   0        0        0     9680 2024-04-03 15:42:21.654554 guarddog-1.5.7/guarddog/analyzer/analyzer.py
--rw-r--r--   0        0        0      457 2024-04-03 15:42:21.654554 guarddog-1.5.7/guarddog/analyzer/metadata/__init__.py
--rw-r--r--   0        0        0      609 2024-04-03 15:42:21.654554 guarddog-1.5.7/guarddog/analyzer/metadata/detector.py
--rw-r--r--   0        0        0     1166 2024-04-03 15:42:21.654554 guarddog-1.5.7/guarddog/analyzer/metadata/empty_information.py
--rw-r--r--   0        0        0      951 2024-04-03 15:42:21.654554 guarddog-1.5.7/guarddog/analyzer/metadata/npm/__init__.py
--rw-r--r--   0        0        0     2449 2024-04-03 15:42:21.654554 guarddog-1.5.7/guarddog/analyzer/metadata/npm/direct_url_dependency.py
--rw-r--r--   0        0        0      793 2024-04-03 15:42:21.654554 guarddog-1.5.7/guarddog/analyzer/metadata/npm/empty_information.py
--rw-r--r--   0        0        0     4215 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py
--rw-r--r--   0        0        0     1260 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      578 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/npm/release_zero.py
--rw-r--r--   0        0        0     1732 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/npm/typosquatting.py
--rw-r--r--   0        0        0     4153 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      976 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/pypi/__init__.py
--rw-r--r--   0        0        0      723 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/pypi/empty_information.py
--rw-r--r--   0        0        0     1873 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      716 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/pypi/release_zero.py
--rw-r--r--   0        0        0    11635 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
--rw-r--r--   0        0        0     1369 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/pypi/single_python_file.py
--rw-r--r--   0        0        0     3490 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/pypi/typosquatting.py
--rw-r--r--   0        0        0      438 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/release_zero.py
--rw-r--r--   0        0        0      743 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/repository_integrity_mismatch.py
--rw-r--r--   0        0        0   373303 2024-04-03 15:42:21.658554 guarddog-1.5.7/guarddog/analyzer/metadata/resources/top_npm_packages.json
--rw-r--r--   0        0        0   387251 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/metadata/resources/top_pypi_packages.json
--rw-r--r--   0        0        0     5619 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/metadata/typosquatting.py
--rw-r--r--   0        0        0      889 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/__init__.py
--rw-r--r--   0        0        0      524 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/clipboard-access.yml
--rw-r--r--   0        0        0      682 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/cmd-overwrite.yml
--rw-r--r--   0        0        0     4599 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/code-execution.yml
--rw-r--r--   0        0        0     1806 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/download-executable.yml
--rw-r--r--   0        0        0     2371 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/exec-base64.yml
--rw-r--r--   0        0        0     1815 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
--rw-r--r--   0        0        0      576 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/npm-exec-base64.yml
--rw-r--r--   0        0        0     1067 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/npm-install-script.yml
--rw-r--r--   0        0        0      835 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
--rw-r--r--   0        0        0     3513 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
--rw-r--r--   0        0        0      582 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/obfuscation.yml
--rw-r--r--   0        0        0     1415 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/shady-links.yml
--rw-r--r--   0        0        0      418 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/silent-process-execution.yml
--rw-r--r--   0        0        0      606 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/analyzer/sourcecode/steganography.yml
--rw-r--r--   0        0        0    13182 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/cli.py
--rw-r--r--   0        0        0      315 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/ecosystems.py
--rw-r--r--   0        0        0        0 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/reporters/__init__.py
--rw-r--r--   0        0        0     6189 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/reporters/sarif.py
--rw-r--r--   0        0        0      752 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/scanners/__init__.py
--rw-r--r--   0        0        0     1968 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/scanners/npm_package_scanner.py
--rw-r--r--   0        0        0     2243 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/scanners/npm_project_scanner.py
--rw-r--r--   0        0        0     2512 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/scanners/pypi_package_scanner.py
--rw-r--r--   0        0        0     5491 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/scanners/pypi_project_scanner.py
--rw-r--r--   0        0        0    11170 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/scanners/scanner.py
--rw-r--r--   0        0        0        0 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/utils/__init__.py
--rw-r--r--   0        0        0     1323 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/utils/archives.py
--rw-r--r--   0        0        0       54 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/utils/exceptions.py
--rw-r--r--   0        0        0      953 2024-04-03 15:42:21.662554 guarddog-1.5.7/guarddog/utils/package_info.py
--rw-r--r--   0        0        0       52 2024-04-03 15:42:21.662554 guarddog-1.5.7/pypi.rst
--rw-r--r--   0        0        0     1338 2024-04-03 15:42:31.070628 guarddog-1.5.7/pyproject.toml
--rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 guarddog-1.5.7/PKG-INFO
+-rw-r--r--   0        0        0    11377 2024-04-08 10:37:22.648802 guarddog-1.5.8/LICENSE
+-rw-r--r--   0        0        0      314 2024-04-08 10:37:22.648802 guarddog-1.5.8/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0      140 2024-04-08 10:37:22.648802 guarddog-1.5.8/NOTICE
+-rw-r--r--   0        0        0      154 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/__init__.py
+-rw-r--r--   0        0        0     9680 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/analyzer.py
+-rw-r--r--   0        0        0      457 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/__init__.py
+-rw-r--r--   0        0        0      609 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/detector.py
+-rw-r--r--   0        0        0     1166 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/empty_information.py
+-rw-r--r--   0        0        0      951 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/__init__.py
+-rw-r--r--   0        0        0     2449 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/direct_url_dependency.py
+-rw-r--r--   0        0        0      793 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/empty_information.py
+-rw-r--r--   0        0        0     4215 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py
+-rw-r--r--   0        0        0     1260 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      578 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/release_zero.py
+-rw-r--r--   0        0        0     1732 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/typosquatting.py
+-rw-r--r--   0        0        0     4153 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      976 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/empty_information.py
+-rw-r--r--   0        0        0     1873 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      716 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/release_zero.py
+-rw-r--r--   0        0        0    11635 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0     1369 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/single_python_file.py
+-rw-r--r--   0        0        0     3490 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/typosquatting.py
+-rw-r--r--   0        0        0      438 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/release_zero.py
+-rw-r--r--   0        0        0      743 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0   373303 2024-04-08 10:37:22.652802 guarddog-1.5.8/guarddog/analyzer/metadata/resources/top_npm_packages.json
+-rw-r--r--   0        0        0   387251 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/metadata/resources/top_pypi_packages.json
+-rw-r--r--   0        0        0     5619 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/metadata/typosquatting.py
+-rw-r--r--   0        0        0      889 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/__init__.py
+-rw-r--r--   0        0        0      524 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/clipboard-access.yml
+-rw-r--r--   0        0        0      682 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/cmd-overwrite.yml
+-rw-r--r--   0        0        0     4655 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/code-execution.yml
+-rw-r--r--   0        0        0     1806 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/download-executable.yml
+-rw-r--r--   0        0        0     2371 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/exec-base64.yml
+-rw-r--r--   0        0        0     1815 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
+-rw-r--r--   0        0        0      576 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-exec-base64.yml
+-rw-r--r--   0        0        0     1067 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-install-script.yml
+-rw-r--r--   0        0        0      835 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
+-rw-r--r--   0        0        0     3513 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
+-rw-r--r--   0        0        0      582 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/obfuscation.yml
+-rw-r--r--   0        0        0     1415 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/shady-links.yml
+-rw-r--r--   0        0        0      418 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/silent-process-execution.yml
+-rw-r--r--   0        0        0      606 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/steganography.yml
+-rw-r--r--   0        0        0    13182 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/cli.py
+-rw-r--r--   0        0        0      315 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/ecosystems.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/reporters/__init__.py
+-rw-r--r--   0        0        0     6189 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/reporters/sarif.py
+-rw-r--r--   0        0        0      752 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/scanners/__init__.py
+-rw-r--r--   0        0        0     1968 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/scanners/npm_package_scanner.py
+-rw-r--r--   0        0        0     2243 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/scanners/npm_project_scanner.py
+-rw-r--r--   0        0        0     2512 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/scanners/pypi_package_scanner.py
+-rw-r--r--   0        0        0     5491 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/scanners/pypi_project_scanner.py
+-rw-r--r--   0        0        0    11170 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/utils/__init__.py
+-rw-r--r--   0        0        0     1323 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/utils/archives.py
+-rw-r--r--   0        0        0       54 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/utils/exceptions.py
+-rw-r--r--   0        0        0      953 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/utils/package_info.py
+-rw-r--r--   0        0        0       52 2024-04-08 10:37:22.656802 guarddog-1.5.8/pypi.rst
+-rw-r--r--   0        0        0     1213 2024-04-08 10:37:32.188830 guarddog-1.5.8/pyproject.toml
+-rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 guarddog-1.5.8/PKG-INFO
```

### Comparing `guarddog-1.5.7/LICENSE` & `guarddog-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/analyzer.py` & `guarddog-1.5.8/guarddog/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/detector.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/detector.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/empty_information.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/npm/__init__.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/npm/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/npm/direct_url_dependency.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/npm/direct_url_dependency.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/npm/empty_information.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/npm/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/npm/release_zero.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/npm/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/npm/typosquatting.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/npm/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/potentially_compromised_email_domain.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/pypi/__init__.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/pypi/empty_information.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/pypi/release_zero.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/pypi/single_python_file.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/single_python_file.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/pypi/typosquatting.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/repository_integrity_mismatch.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/resources/top_npm_packages.json` & `guarddog-1.5.8/guarddog/analyzer/metadata/resources/top_npm_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/resources/top_pypi_packages.json` & `guarddog-1.5.8/guarddog/analyzer/metadata/resources/top_pypi_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/metadata/typosquatting.py` & `guarddog-1.5.8/guarddog/analyzer/metadata/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/__init__.py` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/clipboard-access.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/clipboard-access.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/cmd-overwrite.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/cmd-overwrite.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/code-execution.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/code-execution.yml`

 * *Files 8% similar despite different names*

```diff
@@ -19,30 +19,30 @@
           - patterns:
               - pattern: exec("..." + ...)
               - pattern: exec($ARG1 + ..., ...)
 
           # subprocess module
           - pattern: subprocess.getoutput($ARG1, ...)
           - pattern: getoutput($ARG1, ...)
-          - pattern: subprocess.getoutput([..., "$ARG1", ...], ...)
-          - pattern: getoutput([..., "$ARG1", ...], ...)
+          - pattern: subprocess.getoutput([..., "... $ARG1 ...", ...], ...)
+          - pattern: getoutput([..., "... $ARG1 ...", ...], ...)
 
           - pattern: subprocess.call($ARG1, ...)
           - pattern: call($ARG1, ...)
-          - pattern: subprocess.call([..., "$ARG1", ...], ...)
-          - pattern: call([..., "$ARG1", ...], ...)
+          - pattern: subprocess.call([..., "... $ARG1 ...", ...], ...)
+          - pattern: call([..., "... $ARG1 ...", ...], ...)
 
           - pattern: subprocess.check_output($ARG1, ...)
           - pattern: check_output($ARG1, ...)
-          - pattern: subprocess.check_output([..., "$ARG1", ...], ...)
-          - pattern: check_output([..., "$ARG1", ...], ...)
+          - pattern: subprocess.check_output([..., "... $ARG1 ...", ...], ...)
+          - pattern: check_output([..., "... $ARG1 ...", ...], ...)
 
           - pattern: subprocess.run($ARG1, ...)
           - pattern: run($ARG1, ...)
-          - pattern: subprocess.run([..., "$ARG1", ...], ...)
+          - pattern: subprocess.run([..., "... $ARG1 ...", ...], ...)
           - pattern: run([..., "$ARG1", ...], ...)
 
           # eval, allow checking for version
           - patterns:
               - pattern-either:
                   - pattern: eval($ARG1. ..., ...)
                   - pattern: eval($ARG1, ...)
```

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/download-executable.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/download-executable.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/exec-base64.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/npm-exec-base64.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/npm-install-script.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-install-script.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/npm-serialize-environment.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-serialize-environment.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/obfuscation.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/obfuscation.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/shady-links.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/shady-links.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/analyzer/sourcecode/steganography.yml` & `guarddog-1.5.8/guarddog/analyzer/sourcecode/steganography.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/cli.py` & `guarddog-1.5.8/guarddog/cli.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/reporters/sarif.py` & `guarddog-1.5.8/guarddog/reporters/sarif.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/scanners/__init__.py` & `guarddog-1.5.8/guarddog/scanners/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/scanners/npm_package_scanner.py` & `guarddog-1.5.8/guarddog/scanners/npm_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/scanners/npm_project_scanner.py` & `guarddog-1.5.8/guarddog/scanners/npm_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/scanners/pypi_package_scanner.py` & `guarddog-1.5.8/guarddog/scanners/pypi_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/scanners/pypi_project_scanner.py` & `guarddog-1.5.8/guarddog/scanners/pypi_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/scanners/scanner.py` & `guarddog-1.5.8/guarddog/scanners/scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/utils/archives.py` & `guarddog-1.5.8/guarddog/utils/archives.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/guarddog/utils/package_info.py` & `guarddog-1.5.8/guarddog/utils/package_info.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.7/PKG-INFO` & `guarddog-1.5.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guarddog
-Version: 1.5.7
+Version: 1.5.8
 Summary: GuardDog is a CLI tool to Identify malicious PyPI packages
 Home-page: https://github.com/DataDog/guarddog
 License: Apache-2.0
 Author: Ellen Wang
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -18,18 +18,18 @@
 Requires-Dist: prettytable (>=3.6.0,<4.0.0)
 Requires-Dist: pygit2 (>=1.11,<1.13)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-whois (>=0.8.0,<0.9.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
-Requires-Dist: semgrep (==0.112.1)
+Requires-Dist: semgrep (==1.67.0)
 Requires-Dist: tarsafe (>=0.0.5,<0.0.6)
 Requires-Dist: termcolor (>=2.1.0,<3.0.0)
-Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
+Requires-Dist: urllib3 (==2.2.1)
 Project-URL: Repository, https://github.com/DataDog/guarddog
 Description-Content-Type: text/x-rst
 
 # GuardDog
 
 See https://github.com/datadog/guarddog
```

