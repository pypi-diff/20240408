# Comparing `tmp/cdk-rds-dump-2.0.5.tar.gz` & `tmp/cdk-rds-dump-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-rds-dump-2.0.5.tar", last modified: Tue Mar 26 09:16:08 2024, max compression
+gzip compressed data, was "cdk-rds-dump-2.1.0.tar", last modified: Mon Apr  8 04:52:33 2024, max compression
```

## Comparing `cdk-rds-dump-2.0.5.tar` & `cdk-rds-dump-2.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 09:16:08.882998 cdk-rds-dump-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-26 09:15:55.000000 cdk-rds-dump-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 09:15:55.000000 cdk-rds-dump-2.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-03-26 09:16:08.882998 cdk-rds-dump-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-03-26 09:15:55.000000 cdk-rds-dump-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-26 09:15:55.000000 cdk-rds-dump-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 09:16:08.882998 cdk-rds-dump-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-26 09:15:55.000000 cdk-rds-dump-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 09:16:08.874998 cdk-rds-dump-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 09:16:08.874998 cdk-rds-dump-2.0.5/src/cdk_rds_dump/
--rw-r--r--   0 runner    (1001) docker     (127)    24136 2024-03-26 09:15:55.000000 cdk-rds-dump-2.0.5/src/cdk_rds_dump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 09:16:08.878998 cdk-rds-dump-2.0.5/src/cdk_rds_dump/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-26 09:15:55.000000 cdk-rds-dump-2.0.5/src/cdk_rds_dump/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2647713 2024-03-26 09:15:55.000000 cdk-rds-dump-2.0.5/src/cdk_rds_dump/_jsii/cdk-rds-dump@2.0.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 09:15:55.000000 cdk-rds-dump-2.0.5/src/cdk_rds_dump/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 09:16:08.878998 cdk-rds-dump-2.0.5/src/cdk_rds_dump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-03-26 09:16:08.000000 cdk-rds-dump-2.0.5/src/cdk_rds_dump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-26 09:16:08.000000 cdk-rds-dump-2.0.5/src/cdk_rds_dump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 09:16:08.000000 cdk-rds-dump-2.0.5/src/cdk_rds_dump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-26 09:16:08.000000 cdk-rds-dump-2.0.5/src/cdk_rds_dump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-26 09:16:08.000000 cdk-rds-dump-2.0.5/src/cdk_rds_dump.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:52:33.891008 cdk-rds-dump-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-08 04:52:33.891008 cdk-rds-dump-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 04:52:33.891008 cdk-rds-dump-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:52:33.883008 cdk-rds-dump-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:52:33.887008 cdk-rds-dump-2.1.0/src/cdk_rds_dump/
+-rw-r--r--   0 runner    (1001) docker     (127)    25150 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:52:33.887008 cdk-rds-dump-2.1.0/src/cdk_rds_dump/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2648201 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump/_jsii/cdk-rds-dump@2.1.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:52:22.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:52:33.887008 cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-08 04:52:33.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 04:52:33.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:52:33.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 04:52:33.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 04:52:33.000000 cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/top_level.txt
```

### Comparing `cdk-rds-dump-2.0.5/LICENSE` & `cdk-rds-dump-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-2.0.5/PKG-INFO` & `cdk-rds-dump-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 2.0.5
+Version: 2.1.0
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-rds-dump-2.0.5/README.md` & `cdk-rds-dump-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-2.0.5/setup.py` & `cdk-rds-dump-2.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-rds-dump",
-    "version": "2.0.5",
+    "version": "2.1.0",
     "description": "CDK Construct Library by Typescript for RDS Dump",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-rds-dump.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_rds_dump",
         "cdk_rds_dump._jsii"
     ],
     "package_data": {
         "cdk_rds_dump._jsii": [
-            "cdk-rds-dump@2.0.5.jsii.tgz"
+            "cdk-rds-dump@2.1.0.jsii.tgz"
         ],
         "cdk_rds_dump": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-rds-dump-2.0.5/src/cdk_rds_dump/__init__.py` & `cdk-rds-dump-2.1.0/src/cdk_rds_dump/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,15 @@
         rds_cluster: _aws_cdk_aws_rds_ceddda9d.DatabaseCluster,
         schedule: _aws_cdk_aws_events_ceddda9d.Schedule,
         create_s3_gateway_endpoint: typing.Optional[builtins.bool] = None,
         create_secrets_manager_vpc_endpoint: typing.Optional[builtins.bool] = None,
         id_suffix: typing.Optional[builtins.str] = None,
         lambda_env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         lambda_nsg: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        memory_size: typing.Optional[jsii.Number] = None,
         secret_id: typing.Optional[builtins.str] = None,
         secrets_manager_vpc_endpoint_nsg_id: typing.Optional[builtins.str] = None,
         unsecure_password: typing.Optional[builtins.str] = None,
         unsecure_user_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
@@ -123,14 +124,15 @@
         :param rds_cluster: RDS Cluster to dump.
         :param schedule: Schedule to dump. See aws-cdk-lib/aws-events.Schedule. ex. import * as events from 'aws-cdk-lib/aws-events' // It is executed daily at 00:00 UTC. events.Schedule.cron({ minute: "0", hour: "0" })
         :param create_s3_gateway_endpoint: Whether to create an S3 Gateway Endpoint for the VPC where the RDS is located. Default: false
         :param create_secrets_manager_vpc_endpoint: Whether to create an Interface Endpoint for the Secrets Manager. It is recommended to use a secret stored in the Secrets Manager, but in that case, the lambda doing the dump needs a route to access the Secrets Manager. If createSecretsManagerVPCEndpoint is true, an Interface Endpoint is created to allow access to the Secrets Manager. Default: false
         :param id_suffix: Suffix to add to the resource ID. Default: - no suffix
         :param lambda_env: Environment variables to set in the lambda function. ex. { "ENV_VAR": "value" } Default: - no environment variables
         :param lambda_nsg: Security group to allow access to the lambda function. Default: - use auto generated security group
+        :param memory_size: The amount of memory in MB allocated to the Lambda function. Default: 1024
         :param secret_id: Secret id for database connection information stored in the Secrets Manager. We recommend using the secret stored in the Secrets Manager as the connection information to the DB, but it is also possible to specify the user name and password directly. If secretId is set, the corresponding secret on SecretsManager is retrieved to access the DB. Default: - use database cluster's secret
         :param secrets_manager_vpc_endpoint_nsg_id: List of IDs of security groups to attach to the Interface Endpoint for Secrets Manager. Only used if createSecretsManagerVPCEndpoint is true. Default: - use auto generated security group
         :param unsecure_password: Database Password. We recommend using the secret stored in the Secrets Manager as the connection information to the DB, but it is also possible to specify the user name and password directly. unsecurePassword is a parameter to pass the password when the ``unsecureUsername`` is used. Default: - do not use unsecurePassword
         :param unsecure_user_name: Database username. We recommend using the secret stored in the Secrets Manager as the connection information to the DB, but it is also possible to specify the user name and password directly. unsecureUserName is a parameter to pass the user name when the ``unsecurePassword`` is used. Default: - do not use unsecureUserName
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a38fc7ecfd277f87fd8e580c47c6b6b6ef0f7559271578ac203a7ce2e09649b7)
@@ -142,14 +144,15 @@
             rds_cluster=rds_cluster,
             schedule=schedule,
             create_s3_gateway_endpoint=create_s3_gateway_endpoint,
             create_secrets_manager_vpc_endpoint=create_secrets_manager_vpc_endpoint,
             id_suffix=id_suffix,
             lambda_env=lambda_env,
             lambda_nsg=lambda_nsg,
+            memory_size=memory_size,
             secret_id=secret_id,
             secrets_manager_vpc_endpoint_nsg_id=secrets_manager_vpc_endpoint_nsg_id,
             unsecure_password=unsecure_password,
             unsecure_user_name=unsecure_user_name,
         )
 
         jsii.create(self.__class__, self, [scope, id, __2])
@@ -164,14 +167,15 @@
         "rds_cluster": "rdsCluster",
         "schedule": "schedule",
         "create_s3_gateway_endpoint": "createS3GatewayEndpoint",
         "create_secrets_manager_vpc_endpoint": "createSecretsManagerVPCEndpoint",
         "id_suffix": "idSuffix",
         "lambda_env": "lambdaEnv",
         "lambda_nsg": "lambdaNsg",
+        "memory_size": "memorySize",
         "secret_id": "secretId",
         "secrets_manager_vpc_endpoint_nsg_id": "secretsManagerVPCEndpointNsgId",
         "unsecure_password": "unsecurePassword",
         "unsecure_user_name": "unsecureUserName",
     },
 )
 class RdsDumpProps:
@@ -183,14 +187,15 @@
         rds_cluster: _aws_cdk_aws_rds_ceddda9d.DatabaseCluster,
         schedule: _aws_cdk_aws_events_ceddda9d.Schedule,
         create_s3_gateway_endpoint: typing.Optional[builtins.bool] = None,
         create_secrets_manager_vpc_endpoint: typing.Optional[builtins.bool] = None,
         id_suffix: typing.Optional[builtins.str] = None,
         lambda_env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         lambda_nsg: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        memory_size: typing.Optional[jsii.Number] = None,
         secret_id: typing.Optional[builtins.str] = None,
         secrets_manager_vpc_endpoint_nsg_id: typing.Optional[builtins.str] = None,
         unsecure_password: typing.Optional[builtins.str] = None,
         unsecure_user_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param database_name: Database name to dump.
@@ -198,14 +203,15 @@
         :param rds_cluster: RDS Cluster to dump.
         :param schedule: Schedule to dump. See aws-cdk-lib/aws-events.Schedule. ex. import * as events from 'aws-cdk-lib/aws-events' // It is executed daily at 00:00 UTC. events.Schedule.cron({ minute: "0", hour: "0" })
         :param create_s3_gateway_endpoint: Whether to create an S3 Gateway Endpoint for the VPC where the RDS is located. Default: false
         :param create_secrets_manager_vpc_endpoint: Whether to create an Interface Endpoint for the Secrets Manager. It is recommended to use a secret stored in the Secrets Manager, but in that case, the lambda doing the dump needs a route to access the Secrets Manager. If createSecretsManagerVPCEndpoint is true, an Interface Endpoint is created to allow access to the Secrets Manager. Default: false
         :param id_suffix: Suffix to add to the resource ID. Default: - no suffix
         :param lambda_env: Environment variables to set in the lambda function. ex. { "ENV_VAR": "value" } Default: - no environment variables
         :param lambda_nsg: Security group to allow access to the lambda function. Default: - use auto generated security group
+        :param memory_size: The amount of memory in MB allocated to the Lambda function. Default: 1024
         :param secret_id: Secret id for database connection information stored in the Secrets Manager. We recommend using the secret stored in the Secrets Manager as the connection information to the DB, but it is also possible to specify the user name and password directly. If secretId is set, the corresponding secret on SecretsManager is retrieved to access the DB. Default: - use database cluster's secret
         :param secrets_manager_vpc_endpoint_nsg_id: List of IDs of security groups to attach to the Interface Endpoint for Secrets Manager. Only used if createSecretsManagerVPCEndpoint is true. Default: - use auto generated security group
         :param unsecure_password: Database Password. We recommend using the secret stored in the Secrets Manager as the connection information to the DB, but it is also possible to specify the user name and password directly. unsecurePassword is a parameter to pass the password when the ``unsecureUsername`` is used. Default: - do not use unsecurePassword
         :param unsecure_user_name: Database username. We recommend using the secret stored in the Secrets Manager as the connection information to the DB, but it is also possible to specify the user name and password directly. unsecureUserName is a parameter to pass the user name when the ``unsecurePassword`` is used. Default: - do not use unsecureUserName
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b2e5f91888e54819ce8e66b2c7e425c251eafd75500758ab8d657b3e1e91f875)
@@ -214,14 +220,15 @@
             check_type(argname="argument rds_cluster", value=rds_cluster, expected_type=type_hints["rds_cluster"])
             check_type(argname="argument schedule", value=schedule, expected_type=type_hints["schedule"])
             check_type(argname="argument create_s3_gateway_endpoint", value=create_s3_gateway_endpoint, expected_type=type_hints["create_s3_gateway_endpoint"])
             check_type(argname="argument create_secrets_manager_vpc_endpoint", value=create_secrets_manager_vpc_endpoint, expected_type=type_hints["create_secrets_manager_vpc_endpoint"])
             check_type(argname="argument id_suffix", value=id_suffix, expected_type=type_hints["id_suffix"])
             check_type(argname="argument lambda_env", value=lambda_env, expected_type=type_hints["lambda_env"])
             check_type(argname="argument lambda_nsg", value=lambda_nsg, expected_type=type_hints["lambda_nsg"])
+            check_type(argname="argument memory_size", value=memory_size, expected_type=type_hints["memory_size"])
             check_type(argname="argument secret_id", value=secret_id, expected_type=type_hints["secret_id"])
             check_type(argname="argument secrets_manager_vpc_endpoint_nsg_id", value=secrets_manager_vpc_endpoint_nsg_id, expected_type=type_hints["secrets_manager_vpc_endpoint_nsg_id"])
             check_type(argname="argument unsecure_password", value=unsecure_password, expected_type=type_hints["unsecure_password"])
             check_type(argname="argument unsecure_user_name", value=unsecure_user_name, expected_type=type_hints["unsecure_user_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "database_name": database_name,
             "db_engine": db_engine,
@@ -234,14 +241,16 @@
             self._values["create_secrets_manager_vpc_endpoint"] = create_secrets_manager_vpc_endpoint
         if id_suffix is not None:
             self._values["id_suffix"] = id_suffix
         if lambda_env is not None:
             self._values["lambda_env"] = lambda_env
         if lambda_nsg is not None:
             self._values["lambda_nsg"] = lambda_nsg
+        if memory_size is not None:
+            self._values["memory_size"] = memory_size
         if secret_id is not None:
             self._values["secret_id"] = secret_id
         if secrets_manager_vpc_endpoint_nsg_id is not None:
             self._values["secrets_manager_vpc_endpoint_nsg_id"] = secrets_manager_vpc_endpoint_nsg_id
         if unsecure_password is not None:
             self._values["unsecure_password"] = unsecure_password
         if unsecure_user_name is not None:
@@ -335,14 +344,23 @@
 
         :default: - use auto generated security group
         '''
         result = self._values.get("lambda_nsg")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
 
     @builtins.property
+    def memory_size(self) -> typing.Optional[jsii.Number]:
+        '''The amount of memory in MB allocated to the Lambda function.
+
+        :default: 1024
+        '''
+        result = self._values.get("memory_size")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
     def secret_id(self) -> typing.Optional[builtins.str]:
         '''Secret id for database connection information stored in the Secrets Manager.
 
         We recommend using the secret stored in the Secrets Manager as the connection information to the DB,
         but it is also possible to specify the user name and password directly.
         If secretId is set, the corresponding secret on SecretsManager is retrieved to access the DB.
 
@@ -417,14 +435,15 @@
     rds_cluster: _aws_cdk_aws_rds_ceddda9d.DatabaseCluster,
     schedule: _aws_cdk_aws_events_ceddda9d.Schedule,
     create_s3_gateway_endpoint: typing.Optional[builtins.bool] = None,
     create_secrets_manager_vpc_endpoint: typing.Optional[builtins.bool] = None,
     id_suffix: typing.Optional[builtins.str] = None,
     lambda_env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     lambda_nsg: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+    memory_size: typing.Optional[jsii.Number] = None,
     secret_id: typing.Optional[builtins.str] = None,
     secrets_manager_vpc_endpoint_nsg_id: typing.Optional[builtins.str] = None,
     unsecure_password: typing.Optional[builtins.str] = None,
     unsecure_user_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -436,14 +455,15 @@
     rds_cluster: _aws_cdk_aws_rds_ceddda9d.DatabaseCluster,
     schedule: _aws_cdk_aws_events_ceddda9d.Schedule,
     create_s3_gateway_endpoint: typing.Optional[builtins.bool] = None,
     create_secrets_manager_vpc_endpoint: typing.Optional[builtins.bool] = None,
     id_suffix: typing.Optional[builtins.str] = None,
     lambda_env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     lambda_nsg: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+    memory_size: typing.Optional[jsii.Number] = None,
     secret_id: typing.Optional[builtins.str] = None,
     secrets_manager_vpc_endpoint_nsg_id: typing.Optional[builtins.str] = None,
     unsecure_password: typing.Optional[builtins.str] = None,
     unsecure_user_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdk-rds-dump-2.0.5/src/cdk_rds_dump.egg-info/PKG-INFO` & `cdk-rds-dump-2.1.0/src/cdk_rds_dump.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 2.0.5
+Version: 2.1.0
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

