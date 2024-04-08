# Comparing `tmp/gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3.tar.gz` & `tmp/gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3.tar", last modified: Mon Apr  1 19:22:11 2024, max compression
+gzip compressed data, was "gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4.tar", last modified: Mon Apr  8 19:20:39 2024, max compression
```

## Comparing `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3.tar` & `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:22:11.413927 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 19:22:00.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 19:22:00.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-01 19:22:11.413927 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-01 19:22:00.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-01 19:22:00.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:22:11.413927 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-01 19:22:00.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:22:11.409927 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:22:11.409927 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:22:11.409927 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer/aws_waf_ip_rate_limit_rule_group/
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-01 19:22:00.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer/aws_waf_ip_rate_limit_rule_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:22:11.409927 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer/aws_waf_ip_rate_limit_rule_group/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-01 19:22:00.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer/aws_waf_ip_rate_limit_rule_group/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24093 2024-04-01 19:22:00.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer/aws_waf_ip_rate_limit_rule_group/_jsii/aws-waf-ip-rate-limit-rule-group@1.2.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:22:00.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer/aws_waf_ip_rate_limit_rule_group/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:22:11.409927 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-01 19:22:11.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-01 19:22:11.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:22:11.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 19:22:11.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 19:22:11.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:20:39.739865 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 19:20:26.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 19:20:26.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-08 19:20:39.739865 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-08 19:20:26.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 19:20:26.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:20:39.739865 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-08 19:20:26.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:20:39.735865 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:20:39.735865 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:20:39.739865 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer/aws_waf_ip_rate_limit_rule_group/
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-08 19:20:26.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer/aws_waf_ip_rate_limit_rule_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:20:39.739865 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer/aws_waf_ip_rate_limit_rule_group/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-08 19:20:26.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer/aws_waf_ip_rate_limit_rule_group/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24088 2024-04-08 19:20:26.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer/aws_waf_ip_rate_limit_rule_group/_jsii/aws-waf-ip-rate-limit-rule-group@1.2.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:20:26.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer/aws_waf_ip_rate_limit_rule_group/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:20:39.739865 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-08 19:20:39.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-08 19:20:39.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:20:39.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 19:20:39.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 19:20:39.000000 gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/top_level.txt
```

### Comparing `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/LICENSE` & `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/PKG-INFO` & `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-waf-ip-rate-limit-rule-group
-Version: 1.2.3
+Version: 1.2.4
 Summary: This is an AWS CDK Construct for Rate Limit Rule on WAF V2.
 Home-page: https://github.com/gammarer/aws-waf-ip-rate-limit-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-waf-ip-rate-limit-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/README.md` & `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/setup.py` & `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-waf-ip-rate-limit-rule-group",
-    "version": "1.2.3",
+    "version": "1.2.4",
     "description": "This is an AWS CDK Construct for Rate Limit Rule on WAF V2.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-waf-ip-rate-limit-rule-group.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_waf_ip_rate_limit_rule_group",
         "gammarer.aws_waf_ip_rate_limit_rule_group._jsii"
     ],
     "package_data": {
         "gammarer.aws_waf_ip_rate_limit_rule_group._jsii": [
-            "aws-waf-ip-rate-limit-rule-group@1.2.3.jsii.tgz"
+            "aws-waf-ip-rate-limit-rule-group@1.2.4.jsii.tgz"
         ],
         "gammarer.aws_waf_ip_rate_limit_rule_group": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer/aws_waf_ip_rate_limit_rule_group/__init__.py` & `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer/aws_waf_ip_rate_limit_rule_group/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer/aws_waf_ip_rate_limit_rule_group/_jsii/__init__.py` & `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer/aws_waf_ip_rate_limit_rule_group/_jsii/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-waf-ip-rate-limit-rule-group",
-    "1.2.3",
+    "1.2.4",
     __name__[0:-6],
-    "aws-waf-ip-rate-limit-rule-group@1.2.3.jsii.tgz",
+    "aws-waf-ip-rate-limit-rule-group@1.2.4.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/PKG-INFO` & `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-waf-ip-rate-limit-rule-group
-Version: 1.2.3
+Version: 1.2.4
 Summary: This is an AWS CDK Construct for Rate Limit Rule on WAF V2.
 Home-page: https://github.com/gammarer/aws-waf-ip-rate-limit-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-waf-ip-rate-limit-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.3/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/SOURCES.txt` & `gammarer.aws-waf-ip-rate-limit-rule-group-1.2.4/src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/SOURCES.txt
 src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/dependency_links.txt
 src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/requires.txt
 src/gammarer.aws_waf_ip_rate_limit_rule_group.egg-info/top_level.txt
 src/gammarer/aws_waf_ip_rate_limit_rule_group/__init__.py
 src/gammarer/aws_waf_ip_rate_limit_rule_group/py.typed
 src/gammarer/aws_waf_ip_rate_limit_rule_group/_jsii/__init__.py
-src/gammarer/aws_waf_ip_rate_limit_rule_group/_jsii/aws-waf-ip-rate-limit-rule-group@1.2.3.jsii.tgz
+src/gammarer/aws_waf_ip_rate_limit_rule_group/_jsii/aws-waf-ip-rate-limit-rule-group@1.2.4.jsii.tgz
```

