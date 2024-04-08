# Comparing `tmp/cdk-use-cases.custom-cloud9-ssm-1.3.1.tar.gz` & `tmp/cdk-use-cases.custom-cloud9-ssm-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-use-cases.custom-cloud9-ssm-1.3.1.tar", last modified: Fri Apr  5 13:40:15 2024, max compression
+gzip compressed data, was "cdk-use-cases.custom-cloud9-ssm-1.3.2.tar", last modified: Mon Apr  8 09:39:40 2024, max compression
```

## Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.1.tar` & `cdk-use-cases.custom-cloud9-ssm-1.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.974522 cdk-use-cases.custom-cloud9-ssm-1.3.1/
--rw-r--r--   0 bpguasch (1650823157) 1896053708    10279 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/LICENSE
--rw-r--r--   0 bpguasch (1650823157) 1896053708       23 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/MANIFEST.in
--rw-r--r--   0 bpguasch (1650823157) 1896053708     6376 2024-04-05 13:40:15.974038 cdk-use-cases.custom-cloud9-ssm-1.3.1/PKG-INFO
--rw-r--r--   0 bpguasch (1650823157) 1896053708     5472 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/README.md
--rw-r--r--   0 bpguasch (1650823157) 1896053708      234 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/pyproject.toml
--rw-r--r--   0 bpguasch (1650823157) 1896053708       38 2024-04-05 13:40:15.974702 cdk-use-cases.custom-cloud9-ssm-1.3.1/setup.cfg
--rw-r--r--   0 bpguasch (1650823157) 1896053708     1899 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/setup.py
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.953557 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.953912 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.967335 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/
--rw-r--r--   0 bpguasch (1650823157) 1896053708    15620 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/__init__.py
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.969694 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/_jsii/
--rw-r--r--   0 bpguasch (1650823157) 1896053708      505 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/_jsii/__init__.py
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.972756 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/
--rw-r--r--   0 bpguasch (1650823157) 1896053708      485 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm
--rw-r--r--   0 bpguasch (1650823157) 1896053708   294717 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.1.jsii.tgz
--rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/py.typed
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.964522 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/
--rw-r--r--   0 bpguasch (1650823157) 1896053708     6376 2024-04-05 13:40:15.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO
--rw-r--r--   0 bpguasch (1650823157) 1896053708      633 2024-04-05 13:40:15.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-05 13:40:15.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 bpguasch (1650823157) 1896053708      112 2024-04-05 13:40:15.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/requires.txt
--rw-r--r--   0 bpguasch (1650823157) 1896053708       14 2024-04-05 13:40:15.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/top_level.txt
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.937384 cdk-use-cases.custom-cloud9-ssm-1.3.2/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708    10279 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/LICENSE
+-rw-r--r--   0 bpguasch (1650823157) 1896053708       23 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/MANIFEST.in
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     6376 2024-04-08 09:39:40.936728 cdk-use-cases.custom-cloud9-ssm-1.3.2/PKG-INFO
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     5472 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/README.md
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      234 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/pyproject.toml
+-rw-r--r--   0 bpguasch (1650823157) 1896053708       38 2024-04-08 09:39:40.937636 cdk-use-cases.custom-cloud9-ssm-1.3.2/setup.cfg
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     1899 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/setup.py
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.899730 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.900004 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.930542 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708    15935 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/__init__.py
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.932679 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/_jsii/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      505 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/_jsii/__init__.py
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.935338 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      485 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm
+-rw-r--r--   0 bpguasch (1650823157) 1896053708   292444 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.2.jsii.tgz
+-rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-08 09:39:31.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/py.typed
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-08 09:39:40.907096 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     6376 2024-04-08 09:39:40.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      633 2024-04-08 09:39:40.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-08 09:39:40.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      112 2024-04-08 09:39:40.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/requires.txt
+-rw-r--r--   0 bpguasch (1650823157) 1896053708       14 2024-04-08 09:39:40.000000 cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/top_level.txt
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.1/LICENSE` & `cdk-use-cases.custom-cloud9-ssm-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.1/PKG-INFO` & `cdk-use-cases.custom-cloud9-ssm-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-use-cases.custom-cloud9-ssm
-Version: 1.3.1
+Version: 1.3.2
 Summary: Pattern for Cloud9 EC2 environment and SSM Document.
 Home-page: https://github.com/aws-samples/cdk-use-cases.git
 Author: Borja Pérez Guasch
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-use-cases.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.1/README.md` & `cdk-use-cases.custom-cloud9-ssm-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.1/setup.py` & `cdk-use-cases.custom-cloud9-ssm-1.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-use-cases.custom-cloud9-ssm",
-    "version": "1.3.1",
+    "version": "1.3.2",
     "description": "Pattern for Cloud9 EC2 environment and SSM Document.",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-samples/cdk-use-cases.git",
     "long_description_content_type": "text/markdown",
     "author": "Borja Pérez Guasch",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_use_cases.custom_cloud9_ssm",
         "cdk_use_cases.custom_cloud9_ssm._jsii"
     ],
     "package_data": {
         "cdk_use_cases.custom_cloud9_ssm._jsii": [
-            "custom-cloud9-ssm@1.3.1.jsii.tgz"
+            "custom-cloud9-ssm@1.3.2.jsii.tgz"
         ],
         "cdk_use_cases.custom_cloud9_ssm": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/__init__.py` & `cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases/custom_cloud9_ssm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,25 +257,31 @@
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7f65e24a0b3f838e5cc13a77ae47fdb74efac64f4f101d19732cdd9f146ed4c7)
             check_type(argname="argument steps", value=steps, expected_type=type_hints["steps"])
         return typing.cast(None, jsii.invoke(self, "addDocumentSteps", [steps]))
 
     @jsii.member(jsii_name="deployCDKProject")
-    def deploy_cdk_project(self, url: builtins.str) -> None:
+    def deploy_cdk_project(
+        self,
+        url: builtins.str,
+        stack_name: typing.Optional[builtins.str] = None,
+    ) -> None:
         '''(experimental) Adds a step to the SSM Document content that deploys a CDK project from its compressed version.
 
         :param url: from where to download the file using the wget command.
+        :param stack_name: name of the stack to deploy.
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3a3fb410590672b4abade9ba4a825a4c40ab6b12910dff2df7e9165adfcea34e)
             check_type(argname="argument url", value=url, expected_type=type_hints["url"])
-        return typing.cast(None, jsii.invoke(self, "deployCDKProject", [url]))
+            check_type(argname="argument stack_name", value=stack_name, expected_type=type_hints["stack_name"])
+        return typing.cast(None, jsii.invoke(self, "deployCDKProject", [url, stack_name]))
 
     @jsii.member(jsii_name="resizeEBSTo")
     def resize_ebs_to(self, size: jsii.Number) -> None:
         '''(experimental) Adds a step to the SSM Document content that resizes the EBS volume of the EC2 instance.
 
         Attaches the required policies to ec2Role.
 
@@ -398,14 +404,15 @@
     steps: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__3a3fb410590672b4abade9ba4a825a4c40ab6b12910dff2df7e9165adfcea34e(
     url: builtins.str,
+    stack_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__56ddfa2b8a6c41e3fd5100c991019ee37f14df788c7b63e1ef9a4ac192f29f29(
     size: jsii.Number,
 ) -> None:
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO` & `cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-use-cases.custom-cloud9-ssm
-Version: 1.3.1
+Version: 1.3.2
 Summary: Pattern for Cloud9 EC2 environment and SSM Document.
 Home-page: https://github.com/aws-samples/cdk-use-cases.git
 Author: Borja Pérez Guasch
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-use-cases.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt` & `cdk-use-cases.custom-cloud9-ssm-1.3.2/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt
 src/cdk_use_cases.custom_cloud9_ssm.egg-info/dependency_links.txt
 src/cdk_use_cases.custom_cloud9_ssm.egg-info/requires.txt
 src/cdk_use_cases.custom_cloud9_ssm.egg-info/top_level.txt
 src/cdk_use_cases/custom_cloud9_ssm/__init__.py
 src/cdk_use_cases/custom_cloud9_ssm/py.typed
 src/cdk_use_cases/custom_cloud9_ssm/_jsii/__init__.py
-src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.1.jsii.tgz
+src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.2.jsii.tgz
 src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm
```

