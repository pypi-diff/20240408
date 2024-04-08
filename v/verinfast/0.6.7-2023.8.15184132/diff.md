# Comparing `tmp/verinfast-0.6.7.tar.gz` & `tmp/verinfast-2023.8.15184132.tar.gz`

## Comparing `verinfast-0.6.7.tar` & `verinfast-2023.8.15184132.tar`

### file list

```diff
@@ -1,71 +1,38 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 verinfast-0.6.7/.editorconfig
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 verinfast-0.6.7/.flake8
--rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 verinfast-0.6.7/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 verinfast-0.6.7/Dockerfile
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 verinfast-0.6.7/VERSION.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 verinfast-0.6.7/make_version.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 verinfast-0.6.7/pytest.ini
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 verinfast-0.6.7/requirements.txt
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 verinfast-0.6.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 verinfast-0.6.7/.github/dependabot.yml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 verinfast-0.6.7/.github/workflows/bundle.yml
--rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 verinfast-0.6.7/.github/workflows/release.yml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 verinfast-0.6.7/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/__init__.py
--rwxr-xr-x   0        0        0    37622 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/agent.py
--rw-r--r--   0        0        0    16550 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/config.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/config.yaml
--rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/reset.sh
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/upload.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/user.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/cloud/cloud_dataclass.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/cloud/aws/blocks.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/cloud/aws/costs.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/cloud/aws/get_profile.py
--rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/cloud/aws/instances.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/cloud/aws/regions.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/cloud/azure/blocks.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/cloud/azure/costs.py
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/cloud/azure/instances.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/cloud/gcp/blocks.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/cloud/gcp/instances.py
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/cloud/gcp/zones.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/dependencies/walk.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/dependencies/walkers/README.md
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/dependencies/walkers/classes.py
--rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/dependencies/walkers/gemwalker.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/dependencies/walkers/maven.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/dependencies/walkers/npm.py
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/dependencies/walkers/nuget.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/dependencies/walkers/python.py
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/templates/results.j2
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 verinfast-0.6.7/src/verinfast/utils/utils.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/aws_conf.yaml
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/aws_dash.yaml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/config.yaml
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/delete_temp.yaml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/gcp_conf.yaml
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/gemfile
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/package.json
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/requirements.txt
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/str_conf.yaml
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/test.csproj
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/test_args.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/test_aws.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/test_dependency.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/test_dry.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/test_gcp.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/test_local.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/test_print_cloud_provider.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/test_template.py
--rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/test_truncate.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/test_tsx.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/test_yaml.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/gemnest/gemfile
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/tsx_test/Blank.tsx
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 verinfast-0.6.7/tests/va_test/Gemfile
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 verinfast-0.6.7/.gitignore
--rw-r--r--   0        0        0    13318 2020-02-02 00:00:00.000000 verinfast-0.6.7/LICENSE
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 verinfast-0.6.7/README.md
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 verinfast-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 verinfast-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/.editorconfig
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/.flake8
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/VERSION.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/make_version.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/pytest.ini
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/requirements.txt
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/.github/dependabot.yml
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/.github/workflows/release.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/__init__.py
+-rwxr-xr-x   0        0        0    21958 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/agent.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/config.yaml
+-rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/reset.sh
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/cloud/aws/blocks.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/cloud/aws/costs.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/cloud/aws/instances.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/cloud/aws/regions.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/cloud/azure/blocks.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/cloud/azure/costs.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/cloud/azure/instances.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/cloud/gcp/blocks.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/cloud/gcp/instances.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/cloud/gcp/zones.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/dependencies/walk.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/dependencies/walkers/README.md
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/dependencies/walkers/classes.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/dependencies/walkers/maven.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/dependencies/walkers/npm.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/dependencies/walkers/nuget.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/dependencies/walkers/python.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/src/verinfast/utils/utils.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/tests/package.json
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/tests/test_dependency.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/.gitignore
+-rw-r--r--   0        0        0    13318 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/LICENSE
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/README.md
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/pyproject.toml
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 verinfast-2023.8.15184132/PKG-INFO
```

### Comparing `verinfast-0.6.7/src/verinfast/cloud/aws/blocks.py` & `verinfast-2023.8.15184132/src/verinfast/cloud/aws/blocks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,133 +1,126 @@
 from datetime import datetime, timedelta
 
 import json
 import os
 
 import boto3
-import botocore.exceptions
 
 import verinfast.cloud.aws.regions as r
 
-regions = r.regions
+from verinfast.utils.utils import DebugLog
+debugLog = DebugLog(os.getcwd())
 
+regions = r.regions
 
-def getBlocks(sub_id: str, log, path_to_output: str = "./", dry=False):
 
-    if not dry:
-        session = boto3.Session()
-        profiles = session.available_profiles
-        right_session = None
-        for profile in profiles:
-            s2 = boto3.Session(profile_name=profile)
-            sts = s2.client('sts')
-            try:
-                id = sts.get_caller_identity()
-            except botocore.exceptions.ClientError:
-                continue
-            if int(id['Account']) == int(sub_id):
-                right_session = s2
-                break
-        if right_session is None:
-            return None
-        # for region in regions:
-        #     try:
-        s3 = right_session.client('s3', region_name=regions[0])
-        response = s3.list_buckets()
-        known_buckets = {}
-        for bucket in response['Buckets']:
-            bucket_name = bucket["Name"]
-            resp = s3.get_bucket_location(Bucket=bucket_name)
-
-            permissions = []
-            public = False
-            try:
-                policy_status_resp = s3.get_bucket_policy_status(Bucket=bucket_name)
-                public = policy_status_resp["PolicyStatus"]["IsPublic"]
-
-                if "Policy" in policy_status_resp:
-                    p_string = policy_status_resp["Policy"]
-                    p_dict = json.loads(p_string)
-                    statements = p_dict["Statement"]
-                    # print(statements)
-                    permissions = [json.dumps(s) for s in statements]
-                    # print(s2)
-            except s3.exceptions.from_code('NoSuchBucketPolicy'):
-                log(msg=bucket_name, tag="No Bucket Policy for bucket")
-
-            versioning = None
-            try:
-                versioning_response = s3.get_bucket_versioning(Bucket=bucket_name)
-                if "Status" in versioning_response:
-                    versioning = versioning_response["Status"]
-
-            except s3.exceptions.from_code('NoSuchBucketStatus'):
-                log(msg=bucket_name, tag="No Bucket Status for bucket")
-
-            region = resp['LocationConstraint']
-            # print(region)
-            if region:
-                # print('Have region')
-                cloudwatch = right_session.client('cloudwatch', region_name=region)
-            else:
-                cloudwatch = right_session.client(
-                    'cloudwatch',
-                    region_name='us-east-1'
-                )
-
-            response = cloudwatch.get_metric_statistics(
-                Namespace="AWS/S3",
-                MetricName="BucketSizeBytes",
-                Dimensions=[
-                    {
-                        u"Name": u"BucketName",
-                        u"Value": bucket_name
-                    },
-                    {
-                        u'Name': 'StorageType',
-                        u'Value': 'StandardStorage'
-                    }
-                ],
-                StartTime=datetime.now() - timedelta(days=2),
-                EndTime=datetime.now(),
-                Period=3600,
-                Statistics=['Average'],
-                Unit="Bytes"
+def getBlocks(sub_id: str, path_to_output: str = "./"):
+    session = boto3.Session()
+    profiles = session.available_profiles
+    right_session = None
+    for profile in profiles:
+        s2 = boto3.Session(profile_name=profile)
+        sts = s2.client('sts')
+        id = sts.get_caller_identity()
+        print(id["Account"])
+        if int(id['Account']) == int(sub_id):
+            right_session = s2
+            break
+    if right_session is None:
+        return None
+    # for region in regions:
+    #     try:
+    s3 = right_session.client('s3', region_name=regions[0])
+    response = s3.list_buckets()
+    known_buckets = {}
+    for bucket in response['Buckets']:
+        bucket_name = bucket["Name"]
+        resp = s3.get_bucket_location(Bucket=bucket_name)
+
+        permissions = []
+        try:
+            policy_status_resp = s3.get_bucket_policy_status(Bucket=bucket_name)
+            public = policy_status_resp["PolicyStatus"]["IsPublic"]
+
+            if "Policy" in policy_status_resp:
+                p_string = policy_status_resp["Policy"]
+                p_dict = json.loads(p_string)
+                statements = p_dict["Statement"]
+                # print(statements)
+                permissions = [json.dumps(s) for s in statements]
+                # print(s2)
+        except s3.exceptions.from_code('NoSuchBucketPolicy'):
+            debugLog.log(msg=bucket_name, tag="No Bucket Policy for bucket")
+
+        versioning = None
+        try:
+            versioning_response = s3.get_bucket_versioning(Bucket=bucket_name)
+            if "Status" in versioning_response:
+                versioning = versioning_response["Status"]
+
+        except s3.exceptions.from_code('NoSuchBucketStatus'):
+            debugLog.log(msg=bucket_name, tag="No Bucket Status for bucket")
+
+        region = resp['LocationConstraint']
+        # print(region)
+        if region:
+            # print('Have region')
+            cloudwatch = right_session.client('cloudwatch', region_name=region)
+        else:
+            cloudwatch = right_session.client(
+                'cloudwatch',
+                region_name='us-east-1'
             )
-            if response['Datapoints']:
-                bucket_size_bytes = response['Datapoints'][-1]['Average']
-                known_buckets[bucket_name] = {
-                    "name": bucket_name,
-                    "size": int(bucket_size_bytes),
-                    "retention": versioning,
-                    "public": public,
-                    "permissions": permissions
-                }
-            else:
-                pass
-                # print(response)
-            # except:
-            #     pass
-
-        my_buckets = list(known_buckets.values())
-        upload = {
-                    "metadata": {
-                        "provider": "aws",
-                        "account": str(sub_id)
-                    },
-                    "data": my_buckets
-                }
-    # End dry block
 
+        response = cloudwatch.get_metric_statistics(
+            Namespace="AWS/S3",
+            MetricName="BucketSizeBytes",
+            Dimensions=[
+                {
+                    u"Name": u"BucketName",
+                    u"Value": bucket_name
+                },
+                {
+                    u'Name': 'StorageType',
+                    u'Value': 'StandardStorage'
+                }
+            ],
+            StartTime=datetime.now() - timedelta(days=2),
+            EndTime=datetime.now(),
+            Period=3600,
+            Statistics=['Average'],
+            Unit="Bytes"
+        )
+        if response['Datapoints']:
+            bucket_size_bytes = response['Datapoints'][-1]['Average']
+            known_buckets[bucket_name] = {
+                "name": bucket_name,
+                "size": int(bucket_size_bytes),
+                "retention": versioning,
+                "public": public,
+                "permissions": permissions
+            }
+        else:
+            pass
+            # print(response)
+        # except:
+        #     pass
+
+    my_buckets = list(known_buckets.values())
+    upload = {
+                "metadata": {
+                    "provider": "aws",
+                    "account": str(sub_id)
+                },
+                "data": my_buckets
+            }
     aws_output_file = os.path.join(
         path_to_output,
         f'aws-storage-{sub_id}.json'
     )
 
-    if not dry:
-        with open(aws_output_file, 'w') as outfile:
-            outfile.write(json.dumps(upload, indent=4))
-
+    with open(aws_output_file, 'w') as outfile:
+        outfile.write(json.dumps(upload, indent=4))
     return aws_output_file
 
 # Test Code
 # getBlocks(sub_id='436708548746')
```

### Comparing `verinfast-0.6.7/src/verinfast/cloud/aws/costs.py` & `verinfast-2023.8.15184132/src/verinfast/cloud/aws/costs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,77 @@
 import json
 import os
 import subprocess
 
 from verinfast.utils.utils import DebugLog
-from verinfast.cloud.aws.get_profile import find_profile
 debugLog = DebugLog(os.getcwd())
 
 
-def runAws(targeted_account, start, end, path_to_output,
-           profile=None, log=debugLog.log, dry=False):
-
-    def _get_costs_and_usage(profile: str, aws_output_file: str):
-        cmd = f'''
-            aws ce get-cost-and-usage \
-            --time-period Start={start},End={end} \
-            --granularity=DAILY \
-            --metrics "BlendedCost" \
-            --group-by Type=DIMENSION,Key=SERVICE \
-            --profile="{profile}" \
-            --output=json | cat
-        '''
-
-        try:
-            results = subprocess.run(
-                cmd,
-                shell=True,
-                stdout=subprocess.PIPE,
-                check=True
-            )
-
-        except subprocess.CalledProcessError:
-            log(msg="Error getting data from AWS CLI get-cost-and-usage",
-                tag="AWS CLI")
-            raise Exception("Error getting aws cli data.")
+def runAws(targeted_account, start, end, path_to_output):
+    results = subprocess.run(
+        'aws configure list-profiles',
+        shell=True,
+        stdout=subprocess.PIPE
+    )
 
+    text = results.stdout.decode()
+    profiles = []
+    available_accounts = []
+    for line in text.splitlines():
+        profiles.append(line)
+        cmd = f'aws sts get-caller-identity --profile={line}'
+        results = subprocess.run(cmd, shell=True, stdout=subprocess.PIPE)
         text = results.stdout.decode()
-        if text is None or isinstance(text, str) is False:
-            log(msg="No data returned from AWS CLI get-cost-and-usage",
-                tag="AWS CLI")
-            return None
-
-        obj = json.loads(text)
-        results_by_time = obj["ResultsByTime"]
-        charges = []
-        for charge in results_by_time:
-            if charge["Groups"]:
-                for group in charge["Groups"]:
-                    newCharge = {
-                        "Date": charge["TimePeriod"]["Start"],
-                        "Group": group["Keys"][0],
-                        "Cost": group["Metrics"]["BlendedCost"]["Amount"],
-                        "Currency": group["Metrics"]["BlendedCost"]["Unit"]
-                    }
-                    charges.append(newCharge)
-        upload = {
-            "metadata": {
-                "provider": "aws",
-                "account": str(targeted_account)
-            },
-            "data": charges
-        }
-
-        with open(aws_output_file, 'w') as outfile:
-            outfile.write(json.dumps(upload, indent=4))
-        return aws_output_file
-
-    if profile is None:
-        profile = find_profile(targeted_account=targeted_account, log=log)
-
-    if profile is None:
-        log(msg="No matching profiles found",
-            tag=targeted_account)
-        return None
-
-    output_file = os.path.join(
-        path_to_output,
-        f'aws-cost-{targeted_account}.json'
-    )
-    if not dry:
-        _get_costs_and_usage(profile, output_file)
+        identity = json.loads(text)
+        account = identity["Account"]
+        available_accounts.append(account)
+        if str(account) == str(targeted_account):
+            cmd = f'''
+                aws ce get-cost-and-usage \
+                --time-period Start={start},End={end} \
+                --granularity=DAILY \
+                --metrics "BlendedCost" \
+                --group-by Type=DIMENSION,Key=SERVICE \
+                --profile={line} | cat
+            '''
+
+            try:
+                results = subprocess.run(
+                    cmd,
+                    shell=True,
+                    stdout=subprocess.PIPE
+                )
+
+            except subprocess.CalledProcessError:
+                raise Exception("Error getting aws cli data.")
+
+            text = results.stdout.decode()
+            obj = json.loads(text)
+            results_by_time = obj["ResultsByTime"]
+            charges = []
+            for charge in results_by_time:
+                if charge["Groups"]:
+                    for group in charge["Groups"]:
+                        newCharge = {
+                            "Date": charge["TimePeriod"]["Start"],
+                            "Group": group["Keys"][0],
+                            "Cost": group["Metrics"]["BlendedCost"]["Amount"],
+                            "Currency": group["Metrics"]["BlendedCost"]["Unit"]
+                        }
+                        charges.append(newCharge)
+            upload = {
+                "metadata": {
+                    "provider": "aws",
+                    "account": str(targeted_account)
+                },
+                "data": charges
+            }
+            aws_output_file = os.path.join(
+                path_to_output,
+                f'aws-cost-{targeted_account}.json'
+            )
 
-    return output_file
+            with open(aws_output_file, 'w') as outfile:
+                outfile.write(json.dumps(upload, indent=4))
+            return aws_output_file
+    debugLog.log(msg=profiles, tag="AWS Profiles")
+    debugLog.log(msg=available_accounts, tag="AWS Available Accounts")
```

### Comparing `verinfast-0.6.7/src/verinfast/cloud/aws/regions.py` & `verinfast-2023.8.15184132/src/verinfast/cloud/aws/regions.py`

 * *Files identical despite different names*

### Comparing `verinfast-0.6.7/src/verinfast/cloud/azure/blocks.py` & `verinfast-2023.8.15184132/src/verinfast/cloud/azure/blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,90 +4,88 @@
 
 from azure.identity import DefaultAzureCredential
 from azure.monitor.query import MetricsQueryClient
 from azure.mgmt.storage import StorageManagementClient
 from azure.mgmt.resource import ResourceManagementClient
 
 
-def getBlocks(sub_id: str, path_to_output: str = "./", dry=False):
-    if not dry:
-        credential = DefaultAzureCredential()
-        client = MetricsQueryClient(credential)
-        resource_client = ResourceManagementClient(
-            credential,
-            subscription_id=sub_id
-        )
-
-        group_list = resource_client.resource_groups.list()
-        storage_client = StorageManagementClient(
-            credential,
-            subscription_id=sub_id
-        )
-
-        known_buckets = {}
-        for group in group_list:
-            accounts = storage_client.storage_accounts.list_by_resource_group(
-                    resource_group_name=group.name
-                )
-
-            for account in accounts:
-                containers = storage_client.blob_containers.list(
-                    resource_group_name=group.name,
-                    account_name=account.name
-                )
-
-                file_shares = storage_client.file_shares.list(
-                    resource_group_name=group.name,
-                    account_name=account.name
-                )
-
-                # print(containers)
-                d = datetime.timedelta(
-                    days=1,
-                    seconds=0,
-                    microseconds=0,
-                    milliseconds=0,
-                    minutes=0,
-                    hours=0,
-                    weeks=0
-                )
-
-                o = client.query_resource(
-                    resource_uri=account.id,
-                    metric_names=['UsedCapacity'],
-                    timespan=d
-                )
-
-                bytes = o.metrics[0].timeseries[0].data[0].average
-                print(bytes)
-                known_buckets[account.name] = {
-                        "name": account.name,
-                        "size": bytes,
-                        "retention": None,
-                        "public": False,
-                        "permissions": []
-                    }
-                for c in containers:
-                    if c.public_access:
-                        known_buckets[account.name]["public"] = True
-                for f in file_shares:
-                    print(f)
-        my_buckets = list(known_buckets.values())
-        upload = {
-                    "metadata": {
-                        "provider": "azure",
-                        "account": str(sub_id)
-                    },
-                    "data": my_buckets
+def getBlocks(sub_id: str, path_to_output: str = "./"):
+    credential = DefaultAzureCredential()
+    client = MetricsQueryClient(credential)
+    resource_client = ResourceManagementClient(
+        credential,
+        subscription_id=sub_id
+    )
+
+    group_list = resource_client.resource_groups.list()
+    storage_client = StorageManagementClient(
+        credential,
+        subscription_id=sub_id
+    )
+
+    known_buckets = {}
+    for group in group_list:
+        accounts = storage_client.storage_accounts.list_by_resource_group(
+                resource_group_name=group.name
+            )
+
+        for account in accounts:
+            containers = storage_client.blob_containers.list(
+                resource_group_name=group.name,
+                account_name=account.name
+            )
+
+            file_shares = storage_client.file_shares.list(
+                resource_group_name=group.name,
+                account_name=account.name
+            )
+
+            # print(containers)
+            d = datetime.timedelta(
+                days=1,
+                seconds=0,
+                microseconds=0,
+                milliseconds=0,
+                minutes=0,
+                hours=0,
+                weeks=0
+            )
+
+            o = client.query_resource(
+                resource_uri=account.id,
+                metric_names=['UsedCapacity'],
+                timespan=d
+            )
+
+            bytes = o.metrics[0].timeseries[0].data[0].average
+            print(bytes)
+            known_buckets[account.name] = {
+                    "name": account.name,
+                    "size": bytes,
+                    "retention": None,
+                    "public": False,
+                    "permissions": []
                 }
-    # End dry block
+            for c in containers:
+                if c.public_access:
+                    known_buckets[account.name]["public"] = True
+            for f in file_shares:
+                print(f)
+    my_buckets = list(known_buckets.values())
+    upload = {
+                "metadata": {
+                    "provider": "azure",
+                    "account": str(sub_id)
+                },
+                "data": my_buckets
+            }
     azure_output_file = os.path.join(
         path_to_output,
         f'azure-storage-{sub_id}.json'
     )
-    if not dry:
-        with open(azure_output_file, 'w') as outfile:
-            outfile.write(json.dumps(upload, indent=4))
+
+    with open(azure_output_file, 'w') as outfile:
+        outfile.write(json.dumps(upload, indent=4))
     return azure_output_file
 
 # Test Code
 # getBlocks(sub_id="80dc7a6b-df94-44be-a235-7e7ade335a3c")
```

### Comparing `verinfast-0.6.7/src/verinfast/cloud/azure/costs.py` & `verinfast-2023.8.15184132/src/verinfast/cloud/azure/costs.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,108 +5,105 @@
 import ssl
 import subprocess
 
 from verinfast.utils.utils import DebugLog
 debugLog = DebugLog(os.getcwd())
 
 
-def runAzure(subscription_id, start, end, path_to_output, dry=False):
-    if not dry:
-        ssl.SSLContext.verify_mode = property(
-            lambda self: ssl.CERT_OPTIONAL,
-            lambda self,
-            newval: None
-        )
-
-        conn = http.client.HTTPSConnection("management.azure.com")
-        subprocess.run(
-            f'az account set --subscription {subscription_id}',
-            shell=True
-        )
-        # results = subprocess.run(f'az account show --query id" -o tsv', shell=True, stdout=subprocess.PIPE)  # noqa: E501
-        # subscription_id = results.stdout.decode()[:-1]
-        # 80dc7a6b-df94-44be-a235-7e7ade335a3c
-        req_path = f'/subscriptions/{subscription_id}/providers/Microsoft.CostManagement/query'  # noqa: E501
-        req_params = "api-version=2023-03-01"
-        body = {
-            "dataset": {
-                "granularity": "Daily",
-                "aggregation": {
-                    "totalCost": {
-                        "name": "PreTaxCost",
-                        "function": "Sum"
-                    }
-                },
-                "grouping": [
-                    {
-                        "type": "Dimension",
-                        "name": "ServiceName"
-                    }
-                ]
-            },
-            "timeframe": "custom",
-            "timePeriod": {
-                    "from": str(start),
-                    "to": str(end)
-            },
-            "type": "ActualCost"
-        }
-        results = subprocess.run(
-            "az account get-access-token --resource=https://management.azure.com/ --query accessToken -o tsv",  # noqa: E501
-            shell=True,
-            stdout=subprocess.PIPE
-        )
-
-        bearer_token = "Bearer "+results.stdout.decode().strip()
-        # print(bearer_token)
-        print("Fetching data for subscription: " + subscription_id)
-        conn.request(
-            "POST",
-            req_path + "?" + req_params,
-            headers={
-                "Authorization": bearer_token,
-                "Content-Type": "application/json"
-            },
-            body=json.dumps(body)
-        )
-        response = conn.getresponse()
-        print("Parsing response")
-        data = json.loads(response.read().decode())
-        if 'error' in data:
-            debugLog.log(msg=json.dumps(data["error"]), tag="Azure error")
-            return
-
-        with open(f"{path_to_output}/azure_output_raw.json", "w") as outfile:
-            outfile.write(json.dumps(data, indent=4))
-
-        vals = data["properties"]["rows"]
-        new_vals = []
-        for val in vals:
-            nv = {
-                "Date": str(val[1]),
-                "Cost": str(val[0]),
-                "Group": val[2],
-                "Currency": val[3]
-            }
-            s = nv["Date"]
-            if re.match('^[0-9]*$', s) and len(s) == 8:
-                nv["Date"] = s[0:4] + "-" + s[4:6] + "-" + s[6:8]
-            new_vals.append(nv)
-        upload = {
-            "metadata": {
-                "provider": "azure",
-                "account": subscription_id
+def runAzure(subscription_id, start, end, path_to_output):
+    ssl.SSLContext.verify_mode = property(
+        lambda self: ssl.CERT_OPTIONAL,
+        lambda self,
+        newval: None
+    )
+
+    conn = http.client.HTTPSConnection("management.azure.com")
+    subprocess.run(
+        f'az account set --subscription {subscription_id}',
+        shell=True
+    )
+    # results = subprocess.run(f'az account show --query id" -o tsv', shell=True, stdout=subprocess.PIPE)  # noqa: E501
+    # subscription_id = results.stdout.decode()[:-1]
+    # 80dc7a6b-df94-44be-a235-7e7ade335a3c
+    req_path = f'/subscriptions/{subscription_id}/providers/Microsoft.CostManagement/query'  # noqa: E501
+    req_params = "api-version=2023-03-01"
+    body = {
+        "dataset": {
+            "granularity": "Daily",
+            "aggregation": {
+                "totalCost": {
+                    "name": "PreTaxCost",
+                    "function": "Sum"
+                }
             },
-            "data": new_vals
+            "grouping": [
+                {
+                    "type": "Dimension",
+                    "name": "ServiceName"
+                }
+            ]
+        },
+        "timeframe": "custom",
+        "timePeriod": {
+                "from": str(start),
+                "to": str(end)
+        },
+        "type": "ActualCost"
+    }
+    results = subprocess.run(
+        "az account get-access-token --resource=https://management.azure.com/ --query accessToken -o tsv",  # noqa: E501
+        shell=True,
+        stdout=subprocess.PIPE
+    )
+
+    bearer_token = "Bearer "+results.stdout.decode()[:-1]
+    # print(bearer_token)
+    print("Fetching data for subscription: " + subscription_id)
+    conn.request(
+        "POST",
+        req_path + "?" + req_params,
+        headers={
+            "Authorization": bearer_token,
+            "Content-Type": "application/json"
+        },
+        body=json.dumps(body)
+    )
+    response = conn.getresponse()
+    print("Parsing response")
+    data = json.loads(response.read().decode())
+    if 'error' in data:
+        debugLog.log(msg=json.dumps(data["error"]), tag="Azure error")
+        return
+
+    with open(f"{path_to_output}/azure_output_raw.json", "w") as outfile:
+        outfile.write(json.dumps(data, indent=4))
+
+    vals = data["properties"]["rows"]
+    new_vals = []
+    for val in vals:
+        nv = {
+            "Date": str(val[1]),
+            "Cost": str(val[0]),
+            "Group": val[2],
+            "Currency": val[3]
         }
-    # End dry block
+        s = nv["Date"]
+        if re.match('^[0-9]*$', s) and len(s) == 8:
+            nv["Date"] = s[0:4] + "-" + s[4:6] + "-" + s[6:8]
+        new_vals.append(nv)
+    upload = {
+        "metadata": {
+            "provider": "azure",
+            "account": subscription_id
+        },
+        "data": new_vals
+    }
 
     az_output_file = os.path.join(
         path_to_output,
         f'az-cost-{subscription_id}.json'
     )
 
-    if not dry:
-        with open(az_output_file, "w") as outfile:
-            outfile.write(json.dumps(upload, indent=4))
+    with open(az_output_file, "w") as outfile:
+        outfile.write(json.dumps(upload, indent=4))
 
     return az_output_file
```

### Comparing `verinfast-0.6.7/src/verinfast/cloud/gcp/blocks.py` & `verinfast-2023.8.15184132/src/verinfast/cloud/gcp/blocks.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,82 +2,79 @@
 import os
 import time
 
 from google.cloud.monitoring_v3 import MetricServiceClient, TimeInterval, ListTimeSeriesRequest  # noqa: E501
 from google.cloud import storage
 
 
-def getBlocks(sub_id: str, path_to_output: str = "./", dry=False):
-    if not dry:
-        # Instantiates a client
-        storage_client = storage.Client(project=sub_id)
-
-        # List all the buckets available
-        client = MetricServiceClient()
-        # for bucket in storage_client.list_buckets():
-        #     print(bucket)
-        #     print(bucket.name)
-
-        now = time.time()
-        seconds = int(now)
-        nanos = int((now - seconds) * 10**9)
-        interval = TimeInterval(
-            {
-                "end_time": {"seconds": seconds, "nanos": nanos},
-                "start_time": {"seconds": (seconds - 300), "nanos": nanos},
-            }
-        )
+def getBlocks(sub_id: str, path_to_output: str = "./"):
+    # Instantiates a client
+    storage_client = storage.Client(project=sub_id)
+
+    # List all the buckets available
+    client = MetricServiceClient()
+    # for bucket in storage_client.list_buckets():
+    #     print(bucket)
+    #     print(bucket.name)
+
+    now = time.time()
+    seconds = int(now)
+    nanos = int((now - seconds) * 10**9)
+    interval = TimeInterval(
+        {
+            "end_time": {"seconds": seconds, "nanos": nanos},
+            "start_time": {"seconds": (seconds - 300), "nanos": nanos},
+        }
+    )
 
-        results = client.list_time_series(
-            request={
-                "name": f"projects/{sub_id}",
-                "filter": 'metric.type = "storage.googleapis.com/storage/total_bytes"',  # noqa: E501
-                "interval": interval,
-                "view": ListTimeSeriesRequest.TimeSeriesView.FULL,
-            }
-        )
-        my_buckets = []
-        known_buckets = {}
-        all_buckets = storage_client.list_buckets()
-        for bucket in all_buckets:
-            rp = bucket.retention_period
-            known_buckets[bucket.name] = {
-                "name": bucket.name,
-                "size": 0,
-                "retention": rp,
-                "public": False
+    results = client.list_time_series(
+        request={
+            "name": f"projects/{sub_id}",
+            "filter": 'metric.type = "storage.googleapis.com/storage/total_bytes"',  # noqa: E501
+            "interval": interval,
+            "view": ListTimeSeriesRequest.TimeSeriesView.FULL,
+        }
+    )
+    my_buckets = []
+    known_buckets = {}
+    all_buckets = storage_client.list_buckets()
+    for bucket in all_buckets:
+        rp = bucket.retention_period
+        known_buckets[bucket.name] = {
+            "name": bucket.name,
+            "size": 0,
+            "retention": rp,
+            "public": False
+        }
+        iam = bucket.get_iam_policy()
+        permissions = []
+        for b in iam.bindings:
+            p = {"permission": b["role"], "roles": list(b["members"])}
+            permissions.append(json.dumps(p))
+            if "allUsers" in b["members"]:
+                known_buckets[bucket.name]["public"] = True
+        known_buckets[bucket.name]["permissions"] = permissions
+
+    for result in results:
+        if result.resource and result.resource.labels:
+            bn = result.resource.labels["bucket_name"]
+            size = result.points[-1].value.double_value
+            if bn in known_buckets:
+                known_buckets[bn]["size"] = size
+    my_buckets = list(known_buckets.values())
+    upload = {
+                "metadata": {
+                    "provider": "gcp",
+                    "account": str(sub_id)
+                },
+                "data": my_buckets
             }
-            iam = bucket.get_iam_policy()
-            permissions = []
-            for b in iam.bindings:
-                p = {"permission": b["role"], "roles": list(b["members"])}
-                permissions.append(json.dumps(p))
-                if "allUsers" in b["members"]:
-                    known_buckets[bucket.name]["public"] = True
-            known_buckets[bucket.name]["permissions"] = permissions
-
-        for result in results:
-            if result.resource and result.resource.labels:
-                bn = result.resource.labels["bucket_name"]
-                size = result.points[-1].value.double_value
-                if bn in known_buckets:
-                    known_buckets[bn]["size"] = size
-        my_buckets = list(known_buckets.values())
-        upload = {
-                    "metadata": {
-                        "provider": "gcp",
-                        "account": str(sub_id)
-                    },
-                    "data": my_buckets
-                }
-    # End dry block
     gcp_output_file = os.path.join(
         path_to_output,
         f'gcp-storage-{sub_id}.json'
     )
-    if not dry:
-        with open(gcp_output_file, 'w') as outfile:
-            outfile.write(json.dumps(upload, indent=4))
+    with open(gcp_output_file, 'w') as outfile:
+        outfile.write(json.dumps(upload, indent=4))
     return gcp_output_file
 
 # Test Code
 # getBlocks(sub_id="startupos-328814")
```

### Comparing `verinfast-0.6.7/src/verinfast/cloud/gcp/zones.py` & `verinfast-2023.8.15184132/src/verinfast/cloud/gcp/zones.py`

 * *Files identical despite different names*

### Comparing `verinfast-0.6.7/src/verinfast/dependencies/walkers/README.md` & `verinfast-2023.8.15184132/src/verinfast/dependencies/walkers/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ## What's a Walker?
 Walkers are functions that descend a file tree and find and parse manifests in a certain folder or subfolders.
 
 ## Neat. How many are there?
 Ideally one for every manifest type.
 
 ## What's a manifest type? Is that a language?
-No. Manifest types are files associated with build or software management packages. Think of the Gradle's build.gradle or Maven's pom.xml, as opposed to Java.
+No. Manifest types are like Gradle or Maven, as opposed to Java.
 
 ## Does a manifest need to have a central repository like Maven or PyPi?
 No, although a `walker` may use a central repository to fetch supplementary data about a dependency listed in a manifest. For example, the npm walker installs all dependencies from the central repository, then reads the license string. This allows for capturing the whole dependency tree at once.
 
 ## What is the minimum a Walker must do?
 A walker must update its internal list of `Entry` elements with at least a name and a source (e.g. `pandas` and `pip` respectively). Ideally an entry contains more, like a version, called a specifier, since it can be logical (e.g. `>=1.2.3`), a license, and a description.
```

### Comparing `verinfast-0.6.7/src/verinfast/dependencies/walkers/classes.py` & `verinfast-2023.8.15184132/src/verinfast/dependencies/walkers/classes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import glob
 import json
 import subprocess
 from pathlib import Path
 from typing import List
 
 import httpx
 
@@ -44,71 +43,39 @@
         d["source"] = self.source
         if self.specifier:
             d["specifier"] = self.specifier
         if self.license:
             d["license"] = self.license
         if self.summary:
             d["summary"] = self.summary
-        if self.required_by:
-            d["required_by"] = self.required_by
         return d
 
 
 class Walker():
     def __init__(
         self,
         manifest_type: str,  # "json",
-        manifest_files: List[str],  # ["package.json"]
-        logger,
-        root_dir: str = "./"
+        manifest_files: List[str]  # ["package.json"]
     ) -> None:
         self.files = []
         self.manifest_files = manifest_files
-        for f in self.manifest_files:
-            if "*" in f:
-                expanded = glob.glob(f, root_dir=root_dir)
-                self.manifest_files.remove(f)
-                self.manifest_files += expanded
         self.manifest_type = manifest_type
         self.entries = []
         self.requestx = httpx.Client(http2=True, timeout=None)
-        self.loggerFunc = logger
 
     def initialize(self, command: str):
         if command:
             subprocess.call(args=command)
 
-    def log(self, msg, tag=None, display=False, timestamp=True):
-        self.loggerFunc(
-            msg,
-            tag=tag,
-            display=display,
-            timestamp=timestamp
-        )
-
     def getUrl(self, url: str, headers: dict = {}):
-        return  (  # noqa: E271
-                    self
-                        .requestx  # NOQA: E131
-                        .get(url=url, headers=headers)
-                        .content
-                        .decode('utf-8-sig')
-                )
-
-    def walk(self,
-             path: str = "./",
-             parse: bool = True,
-             expand: bool = False,
-             debug: int = 0):
-        for p in Path(path).rglob('**/*'):
-            if debug > 1:
-                self.log(F"EVALUATING: {p}", display=(debug > 2))
+        return self.requestx.get(url=url, headers=headers)
+
+    def walk(self, path: str = "./", parse: bool = True, expand: bool = False):
+        for p in Path(path).rglob('**/*.*'):
             if p.name in self.manifest_files:
-                if debug > 0:
-                    self.log(f"FOUND: {p.name}", display=True)
                 self.files.append(p)
                 if parse:
                     self.parse(file=str(p.absolute()), expand=expand)
 
     def parse(self, file: str, expand=False):
         raise Exception("No parser for this Walker")
```

### Comparing `verinfast-0.6.7/src/verinfast/dependencies/walkers/npm.py` & `verinfast-2023.8.15184132/src/verinfast/dependencies/walkers/npm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import os
-import subprocess
 from pathlib import Path
 from typing import List
 
 from curses.ascii import isdigit
 
 from verinfast.dependencies.walkers.classes import Walker, Entry
 
@@ -15,66 +14,58 @@
         self.install_points: List[Path] = []
         for p in Path(root_path).rglob('**/*.*'):
             if p.name in self.manifest_files:
                 self.install_points.append(p)
         for p in self.install_points:
             target_dir = Path(p).parent
             os.chdir(target_dir)
-            try:
-                subprocess.run(
-                    "npm install --production --silent --yes",
-                    capture_output=True,
-                    shell=True
-                )
-            except Exception as error:
-                self.log(f'Error with npm install: {error}')
-            else:
-                self.walk('node_modules')
+            os.system("npm install --production")
+            self.walk('node_modules')
             os.chdir(root_path)
 
     def parse(self, file: str, expand=False):
         entry = {}
         license = {}
         try:
             with open(file) as f:
                 d = json.load(f)
-                if "name" in d and "version" in d:
-                    key = d["name"] + "@" + d["version"]
-                    entry["source"] = "npm"
-                    entry["name"] = d["name"]
-                    entry["specifier"] = "==" + d["version"]
-                    if "license" in d and isinstance(d["license"], dict):
-                        license[key] = d["license"]["type"]
-                    elif "license" in d and isinstance(d["license"], list):
-                        license[key] = ' '.join(d["license"])
-                    elif "license" in d:
-                        license[key] = d["license"]
-                    else:
-                        license[key] = ""
-                    entry["license"] = license[key]
-                    entry["requires"] = []
-                    if "dependencies" in d:
-                        for key in d["dependencies"].keys():
-                            k = key
-                            value = d["dependencies"][k]
-                            if isdigit(value[0]):
-                                value = "==" + value
-                            entry["requires"].append(k+value)
-
-                    entry["required_by"] = []
-                    if "description" in d:
-                        entry["summary"] = d["description"]
-                    else:
-                        entry["summary"] = ""
-
-                    e = Entry(
-                        name=entry["name"],
-                        specifier=entry["specifier"],
-                        source=entry["source"],
-                        license=entry["license"],
-                        summary=entry["summary"]
-                    )
-                    self.entries.append(e)
+                key = d["name"] + "@" + d["version"]
+                entry["source"] = "npm"
+                entry["name"] = d["name"]
+                entry["specifier"] = "==" + d["version"]
+                if "license" in d and isinstance(d["license"], dict):
+                    license[key] = d["license"]["type"]
+                elif "license" in d:
+                    license[key] = d["license"]
+                else:
+                    license[key] = ""
+                entry["license"] = license[key]
+                entry["requires"] = []
+                if "dependencies" in d:
+                    for key in d["dependencies"].keys():
+                        k = key
+                        value = d["dependencies"][k]
+                        if isdigit(value[0]):
+                            value = "==" + value
+                        entry["requires"].append(k+value)
+
+                entry["required_by"] = []
+                if "description" in d:
+                    entry["summary"] = d["description"]
+                else:
+                    entry["summary"] = ""
+
+                e = Entry(
+                    name=entry["name"],
+                    specifier=entry["specifier"],
+                    source=entry["source"],
+                    license=entry["license"],
+                    summary=entry["summary"]
+                )
+                self.entries.append(e)
         except Exception as error:
             # handle the exception
-            self.log(f"error parsing {file}")
-            self.log(error)
+            print("An exception occurred in npm.py:", error)
+            pass
+
+
+nodeWalker = NodeWalker(manifest_type='json', manifest_files=["package.json"])
```

### Comparing `verinfast-0.6.7/src/verinfast/dependencies/walkers/nuget.py` & `verinfast-2023.8.15184132/src/verinfast/dependencies/walkers/nuget.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,69 +4,58 @@
 from verinfast.dependencies.walkers.classes import Walker, Entry
 
 
 class NuGetWalker(Walker):
     def initialize(self, command: str = None):
         discoveryUrl = 'https://api.nuget.org/v3/index.json'
         uselessList = json.loads(
-            self.getUrl(discoveryUrl)
+            self.getUrl(discoveryUrl).content.decode('utf-8')
         )
         for r in uselessList["resources"]:
             if "Catalog" in r["@type"]:
                 self.catalogUrl = r["@id"]
             elif r["@type"] == "RegistrationsBaseUrl":
                 self.registrationUrl = r["@id"]
         if command:
             return super().initialize(command)
 
     def get_license(self, name: str, version: str) -> str:
-        resp = None
-        name2 = name.lower()
-        try:
-            license_resp = self.getUrl(f"{self.registrationUrl}{name}/{version}.json")  # NOQA:E501
-            resp = json.loads(license_resp)
-        except Exception as e:
-            self.log(e, display=False)
-            try:
-                license_resp = (
-                    self
-                    .getUrl(f"{self.registrationUrl}{name2}/{version}.json")
-                )
-                resp = json.loads(license_resp)
-            except Exception as e2:
-                self.log(
-                    f"License not found for: {name}@{version}",
-                    display=True
-                )
-                self.log(e2, display=False)
-        if resp is not None:
-            catalog_entry_url = resp["catalogEntry"]
-            catalog_entry = json.loads(self.getUrl(catalog_entry_url))
-            if "licenseExpression" in catalog_entry:
-                return catalog_entry["licenseExpression"]
-            elif "licenseUrl" in catalog_entry:
-                return catalog_entry["licenseUrl"]
-            else:
-                return ""
+        resp = json.loads(
+            self.getUrl(f"{self.registrationUrl}{name}/{version}.json")
+                .content
+                .decode('utf-8')
+            )
+        catalog_entry_url = resp["catalogEntry"]
+        catalog_entry = json.loads(
+            self.getUrl(catalog_entry_url)
+                .content
+                .decode("utf-8")
+        )
+        if "licenseExpression" in catalog_entry:
+            return catalog_entry["licenseExpression"]
+        elif "licenseUrl" in catalog_entry:
+            return catalog_entry["licenseUrl"]
         else:
             return ""
 
     def parse(self, file: str, expand=False):
         # Reference: <PackageReference Include="Swashbuckle.AspNetCore" Version="6.5.0" /> # noqa: E501
         tree = ET.parse(file)
         x_path = "ItemGroup/PackageReference"
         dependencies = tree.findall(x_path)
         for d in dependencies:
-            v = d.attrib["Version"]
-            n = d.attrib["Include"]
+            v = d["Version"]
+            n = d["Include"]
             lic = self.get_license(name=n, version=v)
             e = Entry(
                 source="nuget",
                 name=n,
                 specifier="=="+v,
                 license=lic,
             )
             self.entries.append(e)
 
 
 # Example: https://github.com/umbraco/Umbraco-CMS/pull/13787/files
 c_sharp_matches = ["*.csproj"]
+
+nugetWalker = NuGetWalker(manifest_type='xml', manifest_files=c_sharp_matches)
```

### Comparing `verinfast-0.6.7/.gitignore` & `verinfast-2023.8.15184132/.gitignore`

 * *Files identical despite different names*

### Comparing `verinfast-0.6.7/LICENSE` & `verinfast-2023.8.15184132/LICENSE`

 * *Files identical despite different names*

### Comparing `verinfast-0.6.7/pyproject.toml` & `verinfast-2023.8.15184132/pyproject.toml`

 * *Files identical despite different names*

### Comparing `verinfast-0.6.7/PKG-INFO` & `verinfast-2023.8.15184132/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,47 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: verinfast
-Version: 0.6.7
+Version: 2023.8.15184132
 Summary: This tool safely and securely analyzes applications for benchmarking.
 Project-URL: Homepage, https://github.com/StartupOS/verinfast
 Project-URL: Bug Tracker, https://github.com/StartupOS/verinfast/issues
 Project-URL: Source, https://github.com/StartupOS/verinfast
 Author-email: Jason Nichols <github@startupos.dev>, Sean Conrad <github@startupos.dev>
 License-File: LICENSE
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: azure-identity~=1.15.0
-Requires-Dist: azure-mgmt-compute~=30.6.0
-Requires-Dist: azure-mgmt-monitor~=6.0.2
-Requires-Dist: azure-mgmt-network~=25.3.0
-Requires-Dist: azure-mgmt-resource~=23.0.1
-Requires-Dist: azure-mgmt-storage~=21.1.0
-Requires-Dist: azure-monitor-query~=1.3.0
-Requires-Dist: boto3~=1.34.79
-Requires-Dist: coverage~=7.4.4
-Requires-Dist: defusedxml~=0.7.1
-Requires-Dist: flake8-pytest-style~=2.0.0
-Requires-Dist: flake8~=7.0.0
-Requires-Dist: gemfileparser~=0.8.0
+Requires-Dist: azure-identity
+Requires-Dist: azure-mgmt-compute
+Requires-Dist: azure-mgmt-monitor
+Requires-Dist: azure-mgmt-network
+Requires-Dist: azure-mgmt-resource
+Requires-Dist: azure-mgmt-storage
+Requires-Dist: azure-monitor-query
+Requires-Dist: boto3
+Requires-Dist: coverage>=7.2.7
+Requires-Dist: defusedxml
+Requires-Dist: flake8
+Requires-Dist: flake8-pytest-style
 Requires-Dist: google-cloud-compute>=1.14.0
-Requires-Dist: google-cloud-monitoring>=2.15.0
+Requires-Dist: google-cloud-monitoring>=2.15.1
 Requires-Dist: google-cloud-storage>=2.10.0
-Requires-Dist: httpx[http2]~=0.27.0
-Requires-Dist: jinja2==3.1.3
-Requires-Dist: johnnydep~=1.20.4
-Requires-Dist: modernmetric>=1.4.8
-Requires-Dist: protobuf~=4.25.3
-Requires-Dist: pygments-tsx>=1.0.1
-Requires-Dist: pytest-cov~=5.0.0
-Requires-Dist: pytest-xdist~=3.5.0
-Requires-Dist: pytest~=8.1.1
-Requires-Dist: pyyaml~=6.0.1
-Requires-Dist: semgrep~=1.67.0
-Requires-Dist: windows-curses~=2.3.2; sys_platform == 'win32'
+Requires-Dist: httpx[http2]
+Requires-Dist: johnnydep
+Requires-Dist: modernmetric>=1.0.2
+Requires-Dist: pandas
+Requires-Dist: protobuf
+Requires-Dist: pygount==1.6.1
+Requires-Dist: pytest
+Requires-Dist: pytest-cov
+Requires-Dist: pyyaml
+Requires-Dist: semgrep
 Description-Content-Type: text/markdown
 
-[![Python Release](https://github.com/StartupOS/verinfast/actions/workflows/release.yml/badge.svg?event=release)](https://github.com/StartupOS/verinfast/actions/workflows/release.yml)
-[![codecov](https://codecov.io/gh/StartupOS/verinfast/graph/badge.svg?token=IECR8RD60P)](https://codecov.io/gh/StartupOS/verinfast)
-[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
 # VerinFast™
 
  Welcome to the Scanning Agent.
 
  This tool safely and securely analyzes applications for benchmarking.
 
 ## Requirements:
```

