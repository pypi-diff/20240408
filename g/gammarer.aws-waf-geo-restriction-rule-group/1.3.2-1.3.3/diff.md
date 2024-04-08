# Comparing `tmp/gammarer.aws-waf-geo-restriction-rule-group-1.3.2.tar.gz` & `tmp/gammarer.aws-waf-geo-restriction-rule-group-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-waf-geo-restriction-rule-group-1.3.2.tar", last modified: Mon Apr  1 19:24:10 2024, max compression
+gzip compressed data, was "gammarer.aws-waf-geo-restriction-rule-group-1.3.3.tar", last modified: Mon Apr  8 19:20:52 2024, max compression
```

## Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.2.tar` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:24:10.186466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-01 19:24:10.186466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:24:10.186466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:24:10.182466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:24:10.182466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:24:10.186466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:24:10.186466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27037 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/aws-waf-geo-restriction-rule-group@1.3.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:24:10.186466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-01 19:24:10.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-01 19:24:10.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:24:10.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 19:24:10.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 19:24:10.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:20:52.043142 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 19:20:39.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 19:20:39.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-08 19:20:52.043142 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-08 19:20:39.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 19:20:39.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:20:52.043142 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-08 19:20:39.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:20:52.039142 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:20:52.039142 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:20:52.043142 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer/aws_waf_geo_restriction_rule_group/
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-04-08 19:20:39.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer/aws_waf_geo_restriction_rule_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:20:52.043142 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-08 19:20:39.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27035 2024-04-08 19:20:39.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/aws-waf-geo-restriction-rule-group@1.3.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:20:39.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer/aws_waf_geo_restriction_rule_group/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:20:52.043142 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-08 19:20:52.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 19:20:52.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:20:52.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 19:20:52.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 19:20:52.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/top_level.txt
```

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/LICENSE` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/PKG-INFO` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-waf-geo-restriction-rule-group
-Version: 1.3.2
+Version: 1.3.3
 Summary: This is an AWS CDK Construct for Geo Restriction Rule Group on WAF V2
 Home-page: https://github.com/gammarer/aws-waf-geo-restriction-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-waf-geo-restriction-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/README.md` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/setup.py` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-waf-geo-restriction-rule-group",
-    "version": "1.3.2",
+    "version": "1.3.3",
     "description": "This is an AWS CDK Construct for Geo Restriction Rule Group on WAF V2",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-waf-geo-restriction-rule-group.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_waf_geo_restriction_rule_group",
         "gammarer.aws_waf_geo_restriction_rule_group._jsii"
     ],
     "package_data": {
         "gammarer.aws_waf_geo_restriction_rule_group._jsii": [
-            "aws-waf-geo-restriction-rule-group@1.3.2.jsii.tgz"
+            "aws-waf-geo-restriction-rule-group@1.3.3.jsii.tgz"
         ],
         "gammarer.aws_waf_geo_restriction_rule_group": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/__init__.py` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer/aws_waf_geo_restriction_rule_group/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/__init__.py` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-waf-geo-restriction-rule-group",
-    "1.3.2",
+    "1.3.3",
     __name__[0:-6],
-    "aws-waf-geo-restriction-rule-group@1.3.2.jsii.tgz",
+    "aws-waf-geo-restriction-rule-group@1.3.3.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/PKG-INFO` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-waf-geo-restriction-rule-group
-Version: 1.3.2
+Version: 1.3.3
 Summary: This is an AWS CDK Construct for Geo Restriction Rule Group on WAF V2
 Home-page: https://github.com/gammarer/aws-waf-geo-restriction-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-waf-geo-restriction-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.3/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt
 src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/dependency_links.txt
 src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/requires.txt
 src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/top_level.txt
 src/gammarer/aws_waf_geo_restriction_rule_group/__init__.py
 src/gammarer/aws_waf_geo_restriction_rule_group/py.typed
 src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/__init__.py
-src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/aws-waf-geo-restriction-rule-group@1.3.2.jsii.tgz
+src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/aws-waf-geo-restriction-rule-group@1.3.3.jsii.tgz
```

