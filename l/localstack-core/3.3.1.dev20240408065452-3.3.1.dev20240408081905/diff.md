# Comparing `tmp/localstack-core-3.3.1.dev20240408065452.tar.gz` & `tmp/localstack-core-3.3.1.dev20240408081905.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-3.3.1.dev20240408065452.tar", last modified: Mon Apr  8 06:55:14 2024, max compression
+gzip compressed data, was "localstack-core-3.3.1.dev20240408081905.tar", last modified: Mon Apr  8 08:19:28 2024, max compression
```

## Comparing `localstack-core-3.3.1.dev20240408065452.tar` & `localstack-core-3.3.1.dev20240408081905.tar`

### file list

```diff
@@ -1,1334 +1,1335 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.312748 localstack-core-3.3.1.dev20240408065452/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19752 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5407 2024-04-08 06:55:14.308748 localstack-core-3.3.1.dev20240408065452/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13116 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/README.md
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       24 2024-04-08 06:54:52.000000 localstack-core-3.3.1.dev20240408065452/VERSION
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.680757 localstack-core-3.3.1.dev20240408065452/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     6157 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.684757 localstack-core-3.3.1.dev20240408065452/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.696756 localstack-core-3.3.1.dev20240408065452/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3043 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.696756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.696756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17659 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.696756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75049 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.696756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10739 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.700756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   105561 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.700756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43470 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.700756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   135405 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.704756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    87711 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.704756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6954 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.704756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   811395 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.712756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    63522 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.712756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    56604 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.712756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48880 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.716756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   106527 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.716756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27200 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.716756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    51040 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.716756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    74323 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.720756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59701 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.720756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    78880 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.724756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   148716 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.724756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14828 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.724756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8623 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.724756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69704 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.728756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    58025 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.728756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   142744 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.732756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    89829 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.732756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/scheduler/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15493 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/scheduler/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.732756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23419 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.732756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55788 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.732756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28332 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.736756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19153 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.736756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   220012 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.736756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    44031 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.740756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10092 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.740756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16813 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.740756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60518 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.740756 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    47602 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4822 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1218 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8024 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26256 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/connect.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.668757 localstack-core-3.3.1.dev20240408065452/localstack/aws/data/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.668757 localstack-core-3.3.1.dev20240408065452/localstack/aws/data/sqs-json/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.744756 localstack-core-3.3.1.dev20240408065452/localstack/aws/data/sqs-json/2012-11-05/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      793 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/data/sqs-json/2012-11-05/README.md
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36725 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/data/sqs-json/2012-11-05/service-2.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12084 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      687 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.756755 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1876 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2455 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1946 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10598 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1464 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1790 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1628 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6079 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6241 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12518 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      988 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11678 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2917 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13778 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.760755 localstack-core-3.3.1.dev20240408065452/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50501 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    80521 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17939 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5317 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19961 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.764755 localstack-core-3.3.1.dev20240408065452/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       76 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3918 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5852 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/serving/twisted.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2093 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       76 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8216 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37490 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11599 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12838 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.768755 localstack-core-3.3.1.dev20240408065452/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/cli/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30929 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4222 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      877 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3499 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    57967 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7725 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12965 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.768755 localstack-core-3.3.1.dev20240408065452/localstack/dev/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/dev/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.772755 localstack-core-3.3.1.dev20240408065452/localstack/dev/run/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/dev/run/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12603 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/dev/run/__main__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13833 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/dev/run/configurators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/dev/run/paths.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.772755 localstack-core-3.3.1.dev20240408065452/localstack/dns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/dns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5785 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/dns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1428 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/dns/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33217 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/dns/server.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.772755 localstack-core-3.3.1.dev20240408065452/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       96 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.776755 localstack-core-3.3.1.dev20240408065452/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      139 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      739 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2867 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.784755 localstack-core-3.3.1.dev20240408065452/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      471 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      152 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      755 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/http/duplex_socket.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5356 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      115 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      418 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      747 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      591 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/http/router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      300 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/http/websocket.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.784755 localstack-core-3.3.1.dev20240408065452/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5078 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.792755 localstack-core-3.3.1.dev20240408065452/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16302 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11588 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1310 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      898 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.796755 localstack-core-3.3.1.dev20240408065452/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4126 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3112 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7332 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      818 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2276 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.800755 localstack-core-3.3.1.dev20240408065452/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.800755 localstack-core-3.3.1.dev20240408065452/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.812755 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6310 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13445 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/exporter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69091 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    47983 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15097 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3248 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9586 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   113627 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.836754 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2896 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_account.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1081 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_account.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      587 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_account_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3726 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4214 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_apikey_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3524 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1855 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      627 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5644 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11600 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      602 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_deployment_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4719 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2565 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      602 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_domainname_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3494 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1946 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      627 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8627 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_method.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10052 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_method.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_method_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3757 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_model.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2020 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_model.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_model_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3856 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1917 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      632 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3856 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1788 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_resource.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      592 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_resource_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7513 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3921 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      587 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_restapi_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5067 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_stage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9587 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_stage.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_stage_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6642 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5762 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      597 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3091 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1776 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      612 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6078 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15000 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.836754 localstack-core-3.3.1.dev20240408065452/localstack/services/cdk/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cdk/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.836754 localstack-core-3.3.1.dev20240408065452/localstack/services/cdk/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cdk/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2129 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cdk/resource_providers/cdk_metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cdk/resource_providers/cdk_metadata.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      521 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cdk/resource_providers/cdk_metadata_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.840754 localstack-core-3.3.1.dev20240408065452/localstack/services/certificatemanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/certificatemanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.840754 localstack-core-3.3.1.dev20240408065452/localstack/services/certificatemanager/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/certificatemanager/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4341 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1978 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      655 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.840754 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.848754 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4052 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2468 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10054 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.856754 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13849 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8600 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3542 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/quirks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/schema.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    57929 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1802 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16933 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/template_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10828 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2164 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.856754 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48462 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4788 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/provider_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21708 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.860754 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2812 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      680 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6447 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1192 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2306 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      546 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2495 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      351 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      671 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.864754 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/scaffolding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30872 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/scaffolding/__main__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7821 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/scaffolding/propgen.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5186 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4479 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.864754 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15637 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16749 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/cloudwatch_database_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3194 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18650 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35869 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/provider_v2.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.868754 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3829 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5149 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4118 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      622 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.872754 localstack-core-3.3.1.dev20240408065452/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.876754 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4008 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    89047 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.880754 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14456 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14592 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14688 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12160 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/aws_dynamodb_table_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6437 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11609 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.884754 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8003 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6411 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.884754 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20681 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.904753 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4694 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2752 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10103 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_instance.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11562 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_instance.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      525 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_instance_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3456 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1650 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      585 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_internetgateway_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3674 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_keypair.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3451 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_keypair.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      520 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_keypair_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5790 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_natgateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2703 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_natgateway.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_natgateway_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3124 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_networkacl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1864 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_networkacl.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_networkacl_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_route.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1178 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_route.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_route_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3340 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_routetable.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1959 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_routetable.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_routetable_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4018 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2951 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_securitygroup_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5578 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_subnet.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3233 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_subnet.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      515 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_subnet_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4381 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1376 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4268 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2404 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      580 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_transitgateway_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3816 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3101 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      630 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6920 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_vpc.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4974 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_vpc.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      500 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_vpc_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3189 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      610 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.904753 localstack-core-3.3.1.dev20240408065452/localstack/services/ecr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ecr/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.904753 localstack-core-3.3.1.dev20240408065452/localstack/services/ecr/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ecr/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5022 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ecr/resource_providers/aws_ecr_repository.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7832 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ecr/resource_providers/aws_ecr_repository.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ecr/resource_providers/aws_ecr_repository_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6701 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.908753 localstack-core-3.3.1.dev20240408065452/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17509 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.908753 localstack-core-3.3.1.dev20240408065452/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28882 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2109 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/provider_v2.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.912753 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4444 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_connection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_connection.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      578 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_connection_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2782 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_eventbus.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1121 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_eventbus.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_eventbus_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4388 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_eventbuspolicy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1079 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_eventbuspolicy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      598 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_eventbuspolicy_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8269 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10787 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_rule.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      523 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_rule_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2814 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.916753 localstack-core-3.3.1.dev20240408065452/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6844 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37255 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/firehose/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.916753 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20613 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.928753 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3905 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_accesskey.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      662 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_accesskey.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      555 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_accesskey_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4333 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_group.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1134 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_group.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_group_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4157 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_instanceprofile.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1915 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_instanceprofile.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      585 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_instanceprofile_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3815 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_managedpolicy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1058 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_managedpolicy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_managedpolicy_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4979 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_policy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_policy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      515 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_policy_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7879 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_role.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5495 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_role.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      505 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_role_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3756 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_servercertificate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3458 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_servercertificate.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_servercertificate_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2549 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      622 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4773 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_user.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_user.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      505 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_user_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11028 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12533 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.932753 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6751 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7630 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.936753 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5302 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/aws_kinesis_stream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5738 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/aws_kinesis_stream.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      564 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/aws_kinesis_stream_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3963 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      858 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.936753 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesisfirehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesisfirehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.936753 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesisfirehose/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesisfirehose/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16350 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29805 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.940753 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30899 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60540 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.944753 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2630 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/resource_providers/aws_kms_alias.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1795 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/resource_providers/aws_kms_alias.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/resource_providers/aws_kms_alias_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4258 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/resource_providers/aws_kms_key.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5752 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/resource_providers/aws_kms_key.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      500 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/resource_providers/aws_kms_key_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.952753 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23983 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.956753 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9817 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2451 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      204 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6591 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      584 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/lambda_legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12587 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20150 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7484 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      763 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.968752 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6619 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/assignment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11752 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/counting_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21414 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24779 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/event_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16703 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/execution_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7600 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7292 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/internal_sqs_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18483 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26993 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2580 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1134 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/metrics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      402 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4197 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11407 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1878 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.968752 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      938 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/networking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3570 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      812 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   168930 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.980752 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3397 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3318 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      614 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3218 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      614 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5321 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13019 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      619 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17919 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16077 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_function.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      569 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_function_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3301 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      589 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_layerversion_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3949 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      639 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4367 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_permission.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1096 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_permission.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      579 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_permission_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3662 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4941 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_url.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_url_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4011 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_version.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1073 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_version.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      564 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_version_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4563 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/lambda_alias.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1909 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/lambda_alias.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      525 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/lambda_alias_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7437 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/runtimes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8020 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      397 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.980752 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      569 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18481 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.984752 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4161 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_loggroup.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4890 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_loggroup.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      556 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_loggroup_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_logstream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_logstream.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      561 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_logstream_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3451 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3051 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7769 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/moto.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.992752 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25638 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15220 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27982 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.996752 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6974 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6977 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      597 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10221 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11638 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      617 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10344 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24425 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13385 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.996752 localstack-core-3.3.1.dev20240408065452/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2053 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:13.996752 localstack-core-3.3.1.dev20240408065452/localstack/services/redshift/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/redshift/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9140 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/redshift/resource_providers/aws_redshift_cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15749 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/redshift/resource_providers/aws_redshift_cluster.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/redshift/resource_providers/aws_redshift_cluster_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.000752 localstack-core-3.3.1.dev20240408065452/localstack/services/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/resource_groups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/resource_groups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.000752 localstack-core-3.3.1.dev20240408065452/localstack/services/resource_groups/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/resource_groups/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4752 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      602 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.000752 localstack-core-3.3.1.dev20240408065452/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.000752 localstack-core-3.3.1.dev20240408065452/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3673 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.004752 localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3627 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/aws_route53_healthcheck.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/aws_route53_healthcheck.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      589 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/aws_route53_healthcheck_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6335 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/aws_route53_recordset.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2475 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/aws_route53_recordset.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      579 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/aws_route53_recordset_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.008752 localstack-core-3.3.1.dev20240408065452/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8325 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34472 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.016752 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4781 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3641 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13339 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1554 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3515 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34546 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33980 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    85266 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.020752 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22741 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/aws_s3_bucket.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52629 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/aws_s3_bucket.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      509 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/aws_s3_bucket_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2778 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      527 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      564 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/aws_s3_bucketpolicy_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36205 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2274 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/utils_moto.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.020752 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/v3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/v3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26562 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/v3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   156398 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/v3/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.024752 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/v3/storage/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/v3/storage/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7328 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/v3/storage/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20244 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/v3/storage/ephemeral.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16129 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/validation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5661 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16627 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.028752 localstack-core-3.3.1.dev20240408065452/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.028752 localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      238 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.032752 localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6213 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21941 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      586 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/aws_scheduler_schedule_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3526 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3196 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      611 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.032752 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35107 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.036752 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3084 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      619 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3386 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2045 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      656 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6637 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2360 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2738 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      573 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.040752 localstack-core-3.3.1.dev20240408065452/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22213 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.040752 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1882 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/certificate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1210 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5630 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52777 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    62864 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.044752 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4170 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_subscription.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1059 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_subscription.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_subscription_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5281 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_topic.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6001 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_topic.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_topic_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3325 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_topicpolicy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1677 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_topicpolicy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_topicpolicy_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.052751 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2228 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48438 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71592 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8532 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/query_api.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.052751 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8116 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/aws_sqs_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6980 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/aws_sqs_queue.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/aws_sqs_queue_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3294 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      547 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6483 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.052751 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17767 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.060751 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3432 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1384 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3304 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1264 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5919 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5344 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      615 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5552 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      555 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_parameter_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3788 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.064751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.064751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.064751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1306 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.072751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13817 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicLexer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24010 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4096 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserListener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2546 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserVisitor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    81171 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLLexer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   296690 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLParser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32053 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserListener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18991 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserVisitor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.072751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.072751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.076751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.080751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       83 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3996 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      161 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/comment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.084751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2674 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2820 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.088751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      295 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.092751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      736 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      786 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.092751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.092751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      151 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.092751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.096751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      633 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2180 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.096751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.100751 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      539 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.108750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1598 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      930 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/jitter_strategy_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1590 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      930 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/max_delay_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4300 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.112750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/timeouts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1576 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2062 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      492 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/version.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      171 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2771 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.112750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.120750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      682 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_context_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      747 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.120750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.124750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.128750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1050 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1714 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1781 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1596 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2299 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1895 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.128750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2032 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2014 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.132750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3624 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.132750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2858 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.132750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3162 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1323 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.136750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2507 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2323 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      597 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.136750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2213 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.136750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.140750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1072 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1072 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      394 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.140750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6628 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.140750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7715 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.144750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      987 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.148750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3314 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1226 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2227 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      962 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.152750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.152750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5580 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6009 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6399 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/variable.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2489 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      357 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.152750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11236 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.156750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      167 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/execution_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.156750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2934 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/item_reader_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.160750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      502 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/csv_header_location.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/csv_headers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/input_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/max_items_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2663 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      712 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.160750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      826 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2512 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_s3.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.164750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      164 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_csv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1202 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2110 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.168750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8633 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/distributed_iteration_component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4251 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/inline_iteration_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.176750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2334 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6034 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2183 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1708 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      198 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1648 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6630 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/map_run_record.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      820 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      789 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1004 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_declaration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8427 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.180750 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2213 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5120 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1522 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1703 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1519 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3247 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9848 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.184749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1967 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branch_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4404 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3727 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.188749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2571 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.196749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5272 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12414 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10571 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_api_gateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4659 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7597 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5417 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5014 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_ecs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4713 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2499 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3797 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9188 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3946 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4144 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3576 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8877 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_activitiy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6854 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.200749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      404 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_fail/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1774 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_fail/cause_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      404 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_fail/error_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1774 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_fail/error_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2302 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.200749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3343 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1979 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.200749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.200749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.204749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2506 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1593 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2950 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1392 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.204749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      286 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/aws_execution_details.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.208749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/callback/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/callback/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7586 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/callback/callback.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.208749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7620 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.208749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2726 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1582 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/program_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.212749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2304 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.212749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6145 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40211 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.216749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      704 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/utils/boto_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      689 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.220749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/activity.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11429 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3589 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      378 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7245 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      947 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/store.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.220749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/legacy/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/legacy/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2829 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/legacy/provider_legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4955 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/legacy/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7013 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37121 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/quotas.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.224749 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3263 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1864 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      610 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7105 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5388 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      630 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      801 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11685 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.224749 localstack-core-3.3.1.dev20240408065452/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      319 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sts/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2456 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.228749 localstack-core-3.3.1.dev20240408065452/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.228749 localstack-core-3.3.1.dev20240408065452/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.228749 localstack-core-3.3.1.dev20240408065452/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      704 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/transcribe/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      198 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/transcribe/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13806 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.232749 localstack-core-3.3.1.dev20240408065452/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4003 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4383 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      749 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.232749 localstack-core-3.3.1.dev20240408065452/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.236749 localstack-core-3.3.1.dev20240408065452/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5816 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1733 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/aws/eventbus_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12185 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8030 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.244749 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       73 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.244749 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      214 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/app.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.244749 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2198 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/cloudtrail_tracking_stack.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.244749 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/handler/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2450 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/handler/index.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.248749 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/tests/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/tests/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2353 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/tests/test_cloudtrail_tracking_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2846 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9181 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/container.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1336 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1497 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    74004 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2788 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/in_memory_localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5549 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/marker_report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7547 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/marking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3417 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/path_filter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5000 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/validation_tracking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.248749 localstack-core-3.3.1.dev20240408065452/localstack/testing/scenario/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/scenario/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6145 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/scenario/cdk_lambda_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18243 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/scenario/provisioning.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.248749 localstack-core-3.3.1.dev20240408065452/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31986 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.252749 localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/git.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      893 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/github.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6919 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/matching.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2025 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/opt_in.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.252749 localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/scripts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/scripts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1043 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/scripts/filter_by_test_selection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2400 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/scripts/generate_test_selection_from_commits.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2631 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/scripts/generate_test_selection_from_pr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1187 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/testselection.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.280748 localstack-core-3.3.1.dev20240408065452/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.288748 localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3425 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6500 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8629 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.296748 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13402 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10609 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3524 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14987 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5517 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12235 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8601 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7504 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4666 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48628 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.296748 localstack-core-3.3.1.dev20240408065452/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8474 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17435 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6402 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1218 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5473 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.300748 localstack-core-3.3.1.dev20240408065452/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50771 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33875 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34387 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7297 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4187 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9604 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2967 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11352 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2084 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/iputils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6290 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.300748 localstack-core-3.3.1.dev20240408065452/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3827 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14773 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19689 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7234 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1750 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17967 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.304748 localstack-core-3.3.1.dev20240408065452/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12434 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2535 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5935 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3664 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22548 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5056 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2017 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      717 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3194 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1465 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/localstack/utils/xml.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2024-04-08 06:55:13.000000 localstack-core-3.3.1.dev20240408065452/localstack/version.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 06:55:14.304748 localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5407 2024-04-08 06:55:13.000000 localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71481 2024-04-08 06:55:13.000000 localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 06:55:13.000000 localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18753 2024-04-08 06:55:13.000000 localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18947 2024-04-08 06:55:05.000000 localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2284 2024-04-08 06:55:13.000000 localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2024-04-08 06:55:13.000000 localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8117 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       38 2024-04-08 06:55:14.312748 localstack-core-3.3.1.dev20240408065452/setup.cfg
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      552 2024-04-08 06:09:54.000000 localstack-core-3.3.1.dev20240408065452/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.419432 localstack-core-3.3.1.dev20240408081905/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19752 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5407 2024-04-08 08:19:28.419432 localstack-core-3.3.1.dev20240408081905/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13116 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/README.md
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       24 2024-04-08 08:19:05.000000 localstack-core-3.3.1.dev20240408081905/VERSION
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.635444 localstack-core-3.3.1.dev20240408081905/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     6157 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.643444 localstack-core-3.3.1.dev20240408081905/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.651444 localstack-core-3.3.1.dev20240408081905/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3043 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.651444 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.651444 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17659 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.651444 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75049 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.655444 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10739 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.655444 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   105561 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.655444 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43470 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.655444 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   135405 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.659443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    87711 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.659443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6954 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.659443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   811395 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.667443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    63522 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.667443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    56604 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.667443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48880 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.691443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   106527 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.695443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27200 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.695443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    51040 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.695443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    74323 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.699443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59701 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.699443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    78880 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.703443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   148716 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.703443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14828 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.703443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8623 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.707443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69704 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.711443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    58025 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.715443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   142744 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.715443 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    89829 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.719442 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/scheduler/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15493 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/scheduler/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.719442 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23419 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.723442 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55788 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.723442 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28332 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.723442 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19153 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.727442 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   220012 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.727442 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    44031 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.731442 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10092 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.731442 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16813 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.731442 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60518 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.735442 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47602 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4822 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1218 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8024 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26256 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/connect.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.619444 localstack-core-3.3.1.dev20240408081905/localstack/aws/data/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.619444 localstack-core-3.3.1.dev20240408081905/localstack/aws/data/sqs-json/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.739442 localstack-core-3.3.1.dev20240408081905/localstack/aws/data/sqs-json/2012-11-05/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      793 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/data/sqs-json/2012-11-05/README.md
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36725 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/data/sqs-json/2012-11-05/service-2.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12084 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      687 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.751442 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1876 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2455 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1946 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10598 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1464 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1790 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1628 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6079 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6241 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12518 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      988 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11678 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2917 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13778 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.755442 localstack-core-3.3.1.dev20240408081905/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50501 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    80521 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17939 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5317 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19961 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.759442 localstack-core-3.3.1.dev20240408081905/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       76 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3918 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5852 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/serving/twisted.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2093 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       76 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8216 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37490 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11599 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12838 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.767442 localstack-core-3.3.1.dev20240408081905/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/cli/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30929 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4222 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      877 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3499 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    57967 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7725 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12965 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.767442 localstack-core-3.3.1.dev20240408081905/localstack/dev/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/dev/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.767442 localstack-core-3.3.1.dev20240408081905/localstack/dev/run/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/dev/run/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12603 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/dev/run/__main__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13833 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/dev/run/configurators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/dev/run/paths.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.771442 localstack-core-3.3.1.dev20240408081905/localstack/dns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/dns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5785 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/dns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1428 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/dns/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33217 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/dns/server.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.771442 localstack-core-3.3.1.dev20240408081905/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       96 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.775442 localstack-core-3.3.1.dev20240408081905/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      139 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      739 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2867 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.787442 localstack-core-3.3.1.dev20240408081905/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      471 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      152 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      755 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/http/duplex_socket.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5356 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      115 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      418 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      747 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      591 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/http/router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      300 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/http/websocket.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.787442 localstack-core-3.3.1.dev20240408081905/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5078 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.791442 localstack-core-3.3.1.dev20240408081905/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16302 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11588 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1310 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      898 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.795441 localstack-core-3.3.1.dev20240408081905/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4126 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3112 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7332 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      818 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2276 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.803441 localstack-core-3.3.1.dev20240408081905/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.807441 localstack-core-3.3.1.dev20240408081905/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.815441 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6310 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13445 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/exporter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69091 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47983 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15097 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3248 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9586 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   113627 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.831441 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2896 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_account.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1081 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_account.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      587 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_account_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3726 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4214 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_apikey_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3524 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1855 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      627 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5644 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11600 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      602 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_deployment_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4719 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2565 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      602 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_domainname_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3494 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1946 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      627 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8627 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_method.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10052 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_method.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_method_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3757 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_model.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2020 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_model.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_model_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3856 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1917 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      632 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3856 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1788 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_resource.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      592 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_resource_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7513 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3921 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      587 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_restapi_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5067 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_stage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9587 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_stage.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_stage_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6642 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5762 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      597 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3091 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1776 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      612 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6078 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15000 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.831441 localstack-core-3.3.1.dev20240408081905/localstack/services/cdk/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cdk/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.831441 localstack-core-3.3.1.dev20240408081905/localstack/services/cdk/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cdk/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2129 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cdk/resource_providers/cdk_metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cdk/resource_providers/cdk_metadata.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      521 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cdk/resource_providers/cdk_metadata_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.835441 localstack-core-3.3.1.dev20240408081905/localstack/services/certificatemanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/certificatemanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.835441 localstack-core-3.3.1.dev20240408081905/localstack/services/certificatemanager/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/certificatemanager/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4341 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1978 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      655 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.835441 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.843441 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4052 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2468 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10054 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.855440 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13849 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8600 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3542 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/quirks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/schema.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    57929 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1802 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16933 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/template_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10828 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2164 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.855440 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48462 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4788 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/provider_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21708 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.859440 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2812 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      680 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6447 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1192 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2306 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      546 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2495 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      351 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      671 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.859440 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/scaffolding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30872 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/scaffolding/__main__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7821 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/scaffolding/propgen.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5186 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4479 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.863440 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15637 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16749 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/cloudwatch_database_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3194 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18650 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35869 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/provider_v2.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.867440 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3829 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5149 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4118 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      622 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.867440 localstack-core-3.3.1.dev20240408081905/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.871440 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4008 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    89047 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.875440 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14456 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14592 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14688 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12160 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/aws_dynamodb_table_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6437 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11609 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.875440 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8003 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6411 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.879440 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20681 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.915440 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4694 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2752 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10103 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_instance.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11562 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_instance.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      525 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_instance_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3456 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1650 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      585 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_internetgateway_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3674 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_keypair.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3451 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_keypair.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      520 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_keypair_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5790 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_natgateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2703 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_natgateway.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_natgateway_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3124 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_networkacl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1864 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_networkacl.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_networkacl_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_route.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1178 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_route.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_route_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3340 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_routetable.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1959 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_routetable.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_routetable_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4018 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2951 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_securitygroup_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5578 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_subnet.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3233 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_subnet.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      515 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_subnet_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4381 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1376 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4268 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2404 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      580 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_transitgateway_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3816 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3101 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      630 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6920 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_vpc.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4974 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_vpc.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      500 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_vpc_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3189 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      610 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.915440 localstack-core-3.3.1.dev20240408081905/localstack/services/ecr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ecr/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.915440 localstack-core-3.3.1.dev20240408081905/localstack/services/ecr/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ecr/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5022 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ecr/resource_providers/aws_ecr_repository.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7832 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ecr/resource_providers/aws_ecr_repository.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ecr/resource_providers/aws_ecr_repository_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6701 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.915440 localstack-core-3.3.1.dev20240408081905/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17509 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.919440 localstack-core-3.3.1.dev20240408081905/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20752 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2109 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/provider_v2.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.927440 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4444 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_connection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_connection.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      578 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_connection_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2782 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_eventbus.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1121 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_eventbus.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_eventbus_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4388 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_eventbuspolicy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1079 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_eventbuspolicy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      598 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_eventbuspolicy_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8269 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10787 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_rule.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      523 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_rule_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2814 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12452 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/events/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.931439 localstack-core-3.3.1.dev20240408081905/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6844 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37255 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/firehose/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.931439 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20613 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.943439 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3905 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_accesskey.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      662 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_accesskey.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      555 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_accesskey_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4333 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_group.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1134 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_group.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_group_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4157 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_instanceprofile.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1915 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_instanceprofile.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      585 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_instanceprofile_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3815 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_managedpolicy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1058 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_managedpolicy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_managedpolicy_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4979 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_policy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_policy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      515 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_policy_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7879 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_role.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5495 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_role.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      505 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_role_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3756 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_servercertificate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3458 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_servercertificate.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_servercertificate_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2549 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      622 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4773 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_user.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_user.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      505 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_user_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11028 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12533 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.947439 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6751 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7630 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.951439 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5302 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/aws_kinesis_stream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5738 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/aws_kinesis_stream.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      564 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/aws_kinesis_stream_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3963 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      858 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.951439 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesisfirehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesisfirehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.951439 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesisfirehose/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesisfirehose/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16350 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29805 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.955439 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30899 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60540 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.959439 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2630 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/resource_providers/aws_kms_alias.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1795 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/resource_providers/aws_kms_alias.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/resource_providers/aws_kms_alias_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4258 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/resource_providers/aws_kms_key.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5752 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/resource_providers/aws_kms_key.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      500 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/resource_providers/aws_kms_key_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.967439 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23983 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.971439 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9817 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2451 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      204 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6591 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      584 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/lambda_legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12587 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20150 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9312 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      763 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.979439 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6619 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/assignment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11752 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/counting_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21414 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24779 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/event_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16703 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/execution_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7600 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7292 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/internal_sqs_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18483 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26993 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2580 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1134 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/metrics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      402 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4197 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11407 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1878 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.983439 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      938 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/networking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3570 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      812 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   168930 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.999438 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3397 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3318 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      614 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3218 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      614 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5321 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13019 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      619 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17919 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16077 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_function.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      569 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_function_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3301 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      589 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_layerversion_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3949 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      639 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4367 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_permission.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1096 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_permission.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      579 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_permission_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3662 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4941 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_url.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_url_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4011 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_version.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1073 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_version.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      564 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_version_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4563 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/lambda_alias.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1909 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/lambda_alias.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      525 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/lambda_alias_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7437 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/runtimes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8020 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      397 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:27.999438 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      569 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18481 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.003438 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4161 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_loggroup.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4890 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_loggroup.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      556 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_loggroup_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_logstream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_logstream.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      561 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_logstream_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3451 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3051 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7769 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/moto.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.011438 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25638 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15220 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27982 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.015438 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6974 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6977 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      597 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10221 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11638 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      617 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10344 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24425 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13385 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.019438 localstack-core-3.3.1.dev20240408081905/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2053 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.019438 localstack-core-3.3.1.dev20240408081905/localstack/services/redshift/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/redshift/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9140 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/redshift/resource_providers/aws_redshift_cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15749 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/redshift/resource_providers/aws_redshift_cluster.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/redshift/resource_providers/aws_redshift_cluster_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.019438 localstack-core-3.3.1.dev20240408081905/localstack/services/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/resource_groups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/resource_groups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.019438 localstack-core-3.3.1.dev20240408081905/localstack/services/resource_groups/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/resource_groups/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4752 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      602 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.019438 localstack-core-3.3.1.dev20240408081905/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.023438 localstack-core-3.3.1.dev20240408081905/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3673 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.027438 localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3627 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/aws_route53_healthcheck.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/aws_route53_healthcheck.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      589 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/aws_route53_healthcheck_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6335 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/aws_route53_recordset.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2475 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/aws_route53_recordset.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      579 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/aws_route53_recordset_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.027438 localstack-core-3.3.1.dev20240408081905/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8325 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34472 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.071437 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4781 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3641 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13339 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1554 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3515 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34546 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33980 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    85266 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.075437 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22741 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/aws_s3_bucket.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52629 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/aws_s3_bucket.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      509 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/aws_s3_bucket_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2778 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      527 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      564 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/aws_s3_bucketpolicy_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36205 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2274 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/utils_moto.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.079437 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/v3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/v3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26562 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/v3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   156398 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/v3/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.083437 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/v3/storage/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/v3/storage/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7328 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/v3/storage/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20244 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/v3/storage/ephemeral.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16129 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/validation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5661 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16627 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.087437 localstack-core-3.3.1.dev20240408081905/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.087437 localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      238 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.091437 localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6213 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21941 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      586 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/aws_scheduler_schedule_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3526 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3196 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      611 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.091437 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35107 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.099437 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3084 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      619 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3386 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2045 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      656 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6637 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2360 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2738 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      573 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.099437 localstack-core-3.3.1.dev20240408081905/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22213 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.103437 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1882 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/certificate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1210 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5630 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52777 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    62864 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.107437 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4170 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_subscription.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1059 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_subscription.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_subscription_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5281 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_topic.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6001 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_topic.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_topic_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3325 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_topicpolicy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1677 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_topicpolicy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_topicpolicy_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.111437 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2228 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48438 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    71592 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8532 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/query_api.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.119437 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8116 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/aws_sqs_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6980 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/aws_sqs_queue.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/aws_sqs_queue_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3294 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      547 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6483 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.119437 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17767 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.127436 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3432 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1384 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3304 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1264 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5919 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5344 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      615 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5552 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      555 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_parameter_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3788 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.131436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.131436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.131436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1306 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.139436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13817 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicLexer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24010 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4096 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserListener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2546 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserVisitor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81171 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLLexer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   296690 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLParser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32053 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserListener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18991 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserVisitor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.139436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.143436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.159436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.163436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       83 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3996 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      161 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/comment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.167436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2674 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2820 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.171436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      295 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.175436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      736 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      786 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.175436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.175436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      151 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.175436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.183436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      633 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2180 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.183436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.187436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      539 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.195436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1598 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      930 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/jitter_strategy_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1590 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      930 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/max_delay_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4300 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.195436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/timeouts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1576 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2062 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      492 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/version.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      171 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2771 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.199436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.203436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      682 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_context_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      747 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.203436 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.211435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.211435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1050 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1714 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1781 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1596 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2299 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1895 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.215435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2032 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2014 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.215435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3624 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.215435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2858 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.219435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3162 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1323 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.219435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2507 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2323 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      597 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.219435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2213 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.219435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.223435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1072 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1072 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      394 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.223435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6628 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.227435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7715 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.231435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      987 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.231435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3314 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1226 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2227 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      962 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.235435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.235435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5580 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6009 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6399 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/variable.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2489 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      357 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.235435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11236 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.243435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      167 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/execution_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.243435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2934 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/item_reader_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.247435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      502 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/csv_header_location.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/csv_headers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/input_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/max_items_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2663 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      712 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.247435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      826 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2512 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_s3.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.251435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      164 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_csv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1202 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2110 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.255435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8633 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/distributed_iteration_component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4251 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/inline_iteration_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.259435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2334 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6034 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2183 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1708 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      198 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1648 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6630 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/map_run_record.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      820 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      789 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1004 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_declaration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8427 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.263435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2213 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5120 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1522 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1703 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1519 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3247 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9848 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.263435 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1967 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branch_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4404 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3727 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.267434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2571 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.275434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5272 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12414 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10571 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_api_gateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4659 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7597 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5417 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5014 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_ecs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4713 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2499 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3797 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9188 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3946 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4144 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3576 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8877 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_activitiy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6854 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.279434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      404 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_fail/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1774 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_fail/cause_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      404 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_fail/error_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1774 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_fail/error_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2302 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.279434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3343 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1979 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.279434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.283434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.283434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2506 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1593 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2950 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1392 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.291434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      286 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/aws_execution_details.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.291434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/callback/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/callback/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7586 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/callback/callback.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.291434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7620 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.295434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2726 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1582 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/program_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.295434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2304 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.299434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6145 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40211 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.299434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      704 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/utils/boto_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      689 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.303434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/activity.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11429 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3589 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      378 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7245 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      947 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/store.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.303434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/legacy/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/legacy/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2829 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/legacy/provider_legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4955 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/legacy/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7013 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37121 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/quotas.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.307434 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3263 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1864 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      610 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7105 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5388 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      630 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      801 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11685 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.307434 localstack-core-3.3.1.dev20240408081905/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      319 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sts/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2456 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.311434 localstack-core-3.3.1.dev20240408081905/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.311434 localstack-core-3.3.1.dev20240408081905/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.311434 localstack-core-3.3.1.dev20240408081905/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      704 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/transcribe/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      198 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/transcribe/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13806 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.315434 localstack-core-3.3.1.dev20240408081905/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4003 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4383 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      749 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.315434 localstack-core-3.3.1.dev20240408081905/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.319434 localstack-core-3.3.1.dev20240408081905/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5816 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1733 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/aws/eventbus_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12185 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8030 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.331434 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       73 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.331434 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      214 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/app.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.331434 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2198 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/cloudtrail_tracking_stack.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.335434 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/handler/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2450 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/handler/index.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.335434 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/tests/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/tests/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2353 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/tests/test_cloudtrail_tracking_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2846 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9181 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/container.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1336 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1497 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    74004 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2788 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/in_memory_localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5549 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/marker_report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7547 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/marking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3417 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/path_filter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5000 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/validation_tracking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.335434 localstack-core-3.3.1.dev20240408081905/localstack/testing/scenario/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/scenario/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6145 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/scenario/cdk_lambda_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18243 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/scenario/provisioning.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.339434 localstack-core-3.3.1.dev20240408081905/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31986 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.343433 localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/git.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      893 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/github.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6919 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/matching.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2025 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/opt_in.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.343433 localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/scripts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/scripts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1043 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/scripts/filter_by_test_selection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2400 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/scripts/generate_test_selection_from_commits.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2631 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/scripts/generate_test_selection_from_pr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1187 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/testselection.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.375433 localstack-core-3.3.1.dev20240408081905/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.395433 localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3425 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6500 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8629 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.403432 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13402 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10609 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3524 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14987 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5517 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12235 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8601 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7504 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4666 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48628 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.403432 localstack-core-3.3.1.dev20240408081905/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8474 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17435 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6402 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1218 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5473 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.407432 localstack-core-3.3.1.dev20240408081905/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50771 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33875 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34387 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7297 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4187 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9604 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2967 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11352 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2084 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/iputils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6290 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.411432 localstack-core-3.3.1.dev20240408081905/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3827 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14773 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19689 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7234 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1750 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17967 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.415432 localstack-core-3.3.1.dev20240408081905/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12434 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2535 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5935 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3664 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22548 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5056 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2017 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      717 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3194 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1465 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/localstack/utils/xml.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2024-04-08 08:19:27.000000 localstack-core-3.3.1.dev20240408081905/localstack/version.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 08:19:28.415432 localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5407 2024-04-08 08:19:27.000000 localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    71517 2024-04-08 08:19:27.000000 localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 08:19:27.000000 localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18753 2024-04-08 08:19:27.000000 localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18947 2024-04-08 08:19:19.000000 localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2284 2024-04-08 08:19:27.000000 localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2024-04-08 08:19:27.000000 localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8117 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       38 2024-04-08 08:19:28.419432 localstack-core-3.3.1.dev20240408081905/setup.cfg
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      552 2024-04-08 07:37:36.000000 localstack-core-3.3.1.dev20240408081905/setup.py
```

### Comparing `localstack-core-3.3.1.dev20240408065452/LICENSE.txt` & `localstack-core-3.3.1.dev20240408081905/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/Makefile` & `localstack-core-3.3.1.dev20240408081905/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/PKG-INFO` & `localstack-core-3.3.1.dev20240408081905/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 3.3.1.dev20240408065452
+Version: 3.3.1.dev20240408081905
 Summary: The core library and runtime of LocalStack
 Author-email: LocalStack Contributors <info@localstack.cloud>
 Project-URL: Homepage, https://localstack.cloud
 Project-URL: Documentation, https://docs.localstack.cloud
 Project-URL: Repository, https://github.com/localstack/localstack.git
 Project-URL: Issues, https://github.com/localstack/localstack/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `localstack-core-3.3.1.dev20240408065452/README.md` & `localstack-core-3.3.1.dev20240408081905/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/bin/localstack` & `localstack-core-3.3.1.dev20240408081905/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/bin/localstack-supervisor` & `localstack-core-3.3.1.dev20240408081905/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/accounts.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/acm/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/apigateway/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/config/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/core.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/ec2/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/es/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/events/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/firehose/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/iam/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/kinesis/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/kms/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/lambda_/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/logs/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/opensearch/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/redshift/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/route53/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/s3/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/s3control/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/scheduler/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/ses/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/sns/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/sqs/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/ssm/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/sts/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/support/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/swf/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/api/transcribe/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/app.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/chain.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/client.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/connect.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/data/sqs-json/2012-11-05/README.md` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/data/sqs-json/2012-11-05/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/data/sqs-json/2012-11-05/service-2.json` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/data/sqs-json/2012-11-05/service-2.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/forwarder.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/gateway.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/analytics.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/auth.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/codec.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/cors.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/fallback.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/internal.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/internal_requests.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/legacy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/logging.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/metric_handler.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/presigned_url.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/proxy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/region.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/service.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/handlers/service_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/mocking.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/protocol/op_router.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/protocol/parser.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/protocol/serializer.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/protocol/service_router.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/protocol/validate.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/scaffold.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/serving/edge.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/serving/hypercorn.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/serving/twisted.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/serving/twisted.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/serving/werkzeug.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/skeleton.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/spec-patches.json` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/spec.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/aws/trace.py` & `localstack-core-3.3.1.dev20240408081905/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/cli/exceptions.py` & `localstack-core-3.3.1.dev20240408081905/localstack/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/cli/localstack.py` & `localstack-core-3.3.1.dev20240408081905/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/cli/lpm.py` & `localstack-core-3.3.1.dev20240408081905/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/cli/plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/cli/plugins.py` & `localstack-core-3.3.1.dev20240408081905/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/cli/profiles.py` & `localstack-core-3.3.1.dev20240408081905/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/config.py` & `localstack-core-3.3.1.dev20240408081905/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/constants.py` & `localstack-core-3.3.1.dev20240408081905/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/deprecations.py` & `localstack-core-3.3.1.dev20240408081905/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/dev/run/__main__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/dev/run/__main__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/dev/run/configurators.py` & `localstack-core-3.3.1.dev20240408081905/localstack/dev/run/configurators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/dev/run/paths.py` & `localstack-core-3.3.1.dev20240408081905/localstack/dev/run/paths.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/dns/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/dns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/dns/plugins.py` & `localstack-core-3.3.1.dev20240408081905/localstack/dns/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/dns/server.py` & `localstack-core-3.3.1.dev20240408081905/localstack/dns/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/extensions/api/aws.py` & `localstack-core-3.3.1.dev20240408081905/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/extensions/api/extension.py` & `localstack-core-3.3.1.dev20240408081905/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/http/dispatcher.py` & `localstack-core-3.3.1.dev20240408081905/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/http/duplex_socket.py` & `localstack-core-3.3.1.dev20240408081905/localstack/http/duplex_socket.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/http/hypercorn.py` & `localstack-core-3.3.1.dev20240408081905/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/http/response.py` & `localstack-core-3.3.1.dev20240408081905/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/http/router.py` & `localstack-core-3.3.1.dev20240408081905/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/logging/format.py` & `localstack-core-3.3.1.dev20240408081905/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/logging/setup.py` & `localstack-core-3.3.1.dev20240408081905/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/packages/__init__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/packages/api.py` & `localstack-core-3.3.1.dev20240408081905/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/packages/core.py` & `localstack-core-3.3.1.dev20240408081905/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/packages/debugpy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/packages/ffmpeg.py` & `localstack-core-3.3.1.dev20240408081905/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/packages/terraform.py` & `localstack-core-3.3.1.dev20240408081905/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/plugins.py` & `localstack-core-3.3.1.dev20240408081905/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/runtime/analytics.py` & `localstack-core-3.3.1.dev20240408081905/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/runtime/hooks.py` & `localstack-core-3.3.1.dev20240408081905/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/runtime/init.py` & `localstack-core-3.3.1.dev20240408081905/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/runtime/main.py` & `localstack-core-3.3.1.dev20240408081905/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/runtime/shutdown.py` & `localstack-core-3.3.1.dev20240408081905/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/acm/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/context.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/exporter.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/exporter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/helpers.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/integration.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/invocations.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/patches.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_account.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_account.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_account.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_account.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_account_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_account_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_apikey_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_apikey_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_deployment_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_deployment_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_domainname_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_domainname_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_method.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_method.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_method.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_method.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_method_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_method_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_model.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_model.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_model.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_model.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_model_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_model_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_resource.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_resource.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_resource.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_resource_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_resource_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_restapi_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_restapi_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_stage.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_stage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_stage.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_stage.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_stage_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_stage_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/router_asf.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/apigateway/templates.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cdk/resource_providers/cdk_metadata.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cdk/resource_providers/cdk_metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cdk/resource_providers/cdk_metadata_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cdk/resource_providers/cdk_metadata_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/api_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/deploy.html` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/entities.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/quirks.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/quirks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/template_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/template_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/types.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/provider_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/provider_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/scaffolding/__main__.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/scaffolding/__main__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/scaffolding/propgen.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/scaffolding/propgen.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/service_models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudformation/stores.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/cloudwatch_database_helper.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/cloudwatch_database_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/provider_v2.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/packages.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/resource_providers/aws_dynamodb_table_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/resource_providers/aws_dynamodb_table_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/server.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodb/utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/dynamodbstreams/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/exceptions.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_instance.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_instance.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_instance.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_instance.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_instance_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_instance_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_internetgateway_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_internetgateway_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_keypair.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_keypair.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_keypair.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_keypair.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_keypair_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_keypair_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_natgateway.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_natgateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_natgateway.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_natgateway.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_natgateway_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_natgateway_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_networkacl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_networkacl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_networkacl.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_networkacl.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_networkacl_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_networkacl_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_route.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_route.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_route.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_route.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_routetable.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_routetable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_routetable.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_routetable.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_routetable_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_routetable_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_securitygroup_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_securitygroup_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_subnet.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_subnet.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_subnet.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_subnet.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_subnet_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_subnet_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_transitgateway_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_transitgateway_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_vpc.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_vpc.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_vpc.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_vpc.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ecr/resource_providers/aws_ecr_repository.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ecr/resource_providers/aws_ecr_repository.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ecr/resource_providers/aws_ecr_repository.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ecr/resource_providers/aws_ecr_repository.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ecr/resource_providers/aws_ecr_repository_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ecr/resource_providers/aws_ecr_repository_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/edge.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/es/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/provider.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import datetime
-import ipaddress
 import json
 import logging
 import os
 import re
 import time
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, Optional
 
 from moto.events import events_backends
 from moto.events.responses import EventsHandler as MotoEventsHandler
 from werkzeug import Request
 from werkzeug.exceptions import NotFound
 
 from localstack import config
@@ -38,14 +37,15 @@
     TestEventPatternResponse,
 )
 from localstack.constants import APPLICATION_AMZ_JSON_1_1
 from localstack.http import route
 from localstack.services.edge import ROUTER
 from localstack.services.events.models import EventsStore, events_stores
 from localstack.services.events.scheduler import JobScheduler
+from localstack.services.events.utils import matches_event
 from localstack.services.moto import call_moto
 from localstack.services.plugins import ServiceLifecycleHook
 from localstack.utils.aws.arns import event_bus_arn, parse_arn
 from localstack.utils.aws.client_types import ServicePrincipal
 from localstack.utils.aws.message_forwarding import send_event_to_target
 from localstack.utils.collections import pick_attributes
 from localstack.utils.common import TMP_FILES, mkdir, save_file, truncate
@@ -55,15 +55,14 @@
 
 LOG = logging.getLogger(__name__)
 
 # list of events used to run assertions during integration testing (not exposed to the user)
 TEST_EVENTS_CACHE = []
 EVENTS_TMP_DIR = "cw_events"
 DEFAULT_EVENT_BUS_NAME = "default"
-CONTENT_BASE_FILTER_KEYWORDS = ["prefix", "anything-but", "numeric", "cidr", "exists"]
 CONNECTION_NAME_PATTERN = re.compile("^[\\.\\-_A-Za-z0-9]+$")
 
 
 class ValidationException(ServiceException):
     code: str = "ValidationException"
     sender_fault: bool = True
     status_code: int = 400
@@ -104,24 +103,40 @@
     @staticmethod
     def get_store(context: RequestContext) -> EventsStore:
         return events_stores[context.account_id][context.region]
 
     def test_event_pattern(
         self, context: RequestContext, event_pattern: EventPattern, event: String, **kwargs
     ) -> TestEventPatternResponse:
-        # https://docs.aws.amazon.com/eventbridge/latest/APIReference/API_TestEventPattern.html
-        # Test event pattern uses event pattern to match against event.
-        # So event pattern keys must be in the event keys and values must match.
-        # If event pattern has a key that event does not have, it is not a match.
-        evt_pattern = json.loads(str(event_pattern))
-        evt = json.loads(str(event))
-
-        if any(key not in evt or evt[key] not in values for key, values in evt_pattern.items()):
-            return TestEventPatternResponse(Result=False)
-        return TestEventPatternResponse(Result=True)
+        """Test event pattern uses EventBridge event pattern matching:
+        https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-event-patterns.html
+        """
+        event_pattern_dict = json.loads(event_pattern)
+        event_dict = json.loads(event)
+
+        # TODO: unify all these different implementation below ;)
+
+        # EventBridge implementation:
+        result = matches_event(event_pattern_dict, event_dict)
+
+        # EventSourceMapping implementation:
+        # result = does_match_event(event_pattern_dict, event_dict)
+
+        # moto implementation:
+        # from moto.events.models import EventPattern as EventPatternMoto
+        #
+        # event_pattern = EventPatternMoto.load(event_pattern)
+        # result = event_pattern.matches_event(event_dict)
+
+        # SNS:
+        # from localstack.services.sns.publisher import SubscriptionFilter
+        # subscription_filter = SubscriptionFilter()
+        # result = subscription_filter._evaluate_nested_filter_policy_on_dict(event_pattern_dict, event_dict)
+
+        return TestEventPatternResponse(Result=result)
 
     @staticmethod
     def get_scheduled_rule_func(
         store: EventsStore,
         rule_name: RuleName,
         event_bus_name_or_arn: Optional[EventBusNameOrArn] = None,
     ):
@@ -378,222 +393,27 @@
                 "%s_%s" % (current_time_millis, event["uuid"]),
             )
             save_file(target, json.dumps(event["event"]))
     except Exception as e:
         LOG.info("Unable to dump events to tmp dir %s: %s", _get_events_tmp_dir(), e)
 
 
-def handle_numeric_conditions(conditions: list[Any], value: float):
-    for i in range(0, len(conditions), 2):
-        if conditions[i] == "<" and not (value < conditions[i + 1]):
-            return False
-        if conditions[i] == ">" and not (value > conditions[i + 1]):
-            return False
-        if conditions[i] == "<=" and not (value <= conditions[i + 1]):
-            return False
-        if conditions[i] == ">=" and not (value >= conditions[i + 1]):
-            return False
-    return True
-
-
-def check_valid_numeric_content_base_rule(list_of_operators):
-    if len(list_of_operators) > 4:
-        return False
-
-    if "=" in list_of_operators:
-        return False
-
-    if len(list_of_operators) > 2:
-        upper_limit = None
-        lower_limit = None
-        for index in range(len(list_of_operators)):
-            if not isinstance(list_of_operators[index], int) and "<" in list_of_operators[index]:
-                upper_limit = list_of_operators[index + 1]
-            if not isinstance(list_of_operators[index], int) and ">" in list_of_operators[index]:
-                lower_limit = list_of_operators[index + 1]
-            if upper_limit and lower_limit and upper_limit < lower_limit:
-                return False
-            index = index + 1
-    return True
-
-
-def filter_event_with_content_base_parameter(pattern_value: list, event_value: str | int):
-    for element in pattern_value:
-        if (isinstance(element, (str, int))) and (event_value == element or element in event_value):
-            return True
-        elif isinstance(element, dict):
-            element_key = list(element.keys())[0]
-            element_value = element.get(element_key)
-            if element_key.lower() == "prefix":
-                if isinstance(event_value, str) and event_value.startswith(element_value):
-                    return True
-            elif element_key.lower() == "exists":
-                if element_value and event_value:
-                    return True
-                elif not element_value and isinstance(event_value, object):
-                    return True
-            elif element_key.lower() == "cidr":
-                ips = [str(ip) for ip in ipaddress.IPv4Network(element_value)]
-                if event_value in ips:
-                    return True
-            elif element_key.lower() == "numeric":
-                if check_valid_numeric_content_base_rule(element_value):
-                    for index in range(len(element_value)):
-                        if isinstance(element_value[index], int):
-                            continue
-                        if (
-                            element_value[index] == ">"
-                            and isinstance(element_value[index + 1], int)
-                            and event_value <= element_value[index + 1]
-                        ):
-                            break
-                        elif (
-                            element_value[index] == ">="
-                            and isinstance(element_value[index + 1], int)
-                            and event_value < element_value[index + 1]
-                        ):
-                            break
-                        elif (
-                            element_value[index] == "<"
-                            and isinstance(element_value[index + 1], int)
-                            and event_value >= element_value[index + 1]
-                        ):
-                            break
-                        elif (
-                            element_value[index] == "<="
-                            and isinstance(element_value[index + 1], int)
-                            and event_value > element_value[index + 1]
-                        ):
-                            break
-                    else:
-                        return True
-
-            elif element_key.lower() == "anything-but":
-                if isinstance(element_value, list) and event_value not in element_value:
-                    return True
-                elif (isinstance(element_value, (str, int))) and event_value != element_value:
-                    return True
-                elif isinstance(element_value, dict):
-                    nested_key = list(element_value)[0]
-                    if nested_key == "prefix" and not re.match(
-                        r"^{}".format(element_value.get(nested_key)), event_value
-                    ):
-                        return True
-    return False
-
-
-# TODO: unclear shared responsibility for filtering with filter_event_with_content_base_parameter
-def handle_prefix_filtering(event_pattern, value):
-    for element in event_pattern:
-        if isinstance(element, (int, str)):
-            if str(element) == str(value):
-                return True
-            if element in value:
-                return True
-        elif isinstance(element, dict) and "prefix" in element:
-            if value.startswith(element.get("prefix")):
-                return True
-        elif isinstance(element, dict) and "anything-but" in element:
-            if element.get("anything-but") != value:
-                return True
-        elif isinstance(element, dict) and "exists" in element:
-            if element.get("exists") and value:
-                return True
-        elif "numeric" in element:
-            return handle_numeric_conditions(element.get("numeric"), value)
-        elif isinstance(element, list):
-            if value in list:
-                return True
-    return False
-
-
-def identify_content_base_parameter_in_pattern(parameters) -> bool:
-    return any(
-        list(param.keys())[0] in CONTENT_BASE_FILTER_KEYWORDS
-        for param in parameters
-        if isinstance(param, dict)
-    )
-
-
-def get_two_lists_intersection(lst1: List, lst2: List) -> List:
-    lst3 = [value for value in lst1 if value in lst2]
-    return lst3
-
-
-def event_pattern_prefix_bool_filter(event_pattern_filter_value_list: list[dict[str, Any]]) -> bool:
-    for event_pattern_filter_value in event_pattern_filter_value_list:
-        if "exists" in event_pattern_filter_value:
-            return event_pattern_filter_value.get("exists")
-        else:
-            return True
-
-
-# TODO: refactor/simplify!
 def filter_event_based_on_event_format(
     self, rule_name: str, event_bus_name: str, event: dict[str, Any]
 ):
-    def filter_event(event_pattern_filter: dict[str, Any], event: dict[str, Any]):
-        for key, value in event_pattern_filter.items():
-            fallback = object()
-            event_value = event.get(key.lower(), event.get(key, fallback))
-            if event_value is fallback and event_pattern_prefix_bool_filter(value):
-                return False
-
-            # 1. check if certain values in the event do not match the expected pattern
-            if event_value and isinstance(event_value, dict):
-                for key_a, value_a in event_value.items():
-                    if key_a == "ip":
-                        # TODO add IP-Address check here
-                        continue
-                    if isinstance(value.get(key_a), (int, str)):
-                        if value_a != value.get(key_a):
-                            return False
-                    if isinstance(value.get(key_a), list) and value_a not in value.get(key_a):
-                        if not handle_prefix_filtering(value.get(key_a), value_a):
-                            return False
-
-            # 2. check if the pattern is a list and event values are not contained in it
-            if isinstance(value, list):
-                if identify_content_base_parameter_in_pattern(value):
-                    if not filter_event_with_content_base_parameter(value, event_value):
-                        return False
-                else:
-                    if (
-                        isinstance(event_value, list)
-                        and get_two_lists_intersection(value, event_value) == []
-                    ):
-                        return False
-                    if (
-                        not isinstance(event_value, list)
-                        and isinstance(event_value, (str, int))
-                        and event_value not in value
-                    ):
-                        return False
-
-            # 3. recursively call filter_event(..) for dict types
-            elif isinstance(value, (str, dict)):
-                try:
-                    value = json.loads(value) if isinstance(value, str) else value
-                    if isinstance(value, dict) and not filter_event(value, event_value):
-                        return False
-                except json.decoder.JSONDecodeError:
-                    return False
-
-        return True
-
     rule_information = self.events_backend.describe_rule(
         rule_name, event_bus_arn(event_bus_name, self.current_account, self.region)
     )
 
     if not rule_information:
         LOG.info('Unable to find rule "%s" in backend: %s', rule_name, rule_information)
         return False
     if rule_information.event_pattern._pattern:
         event_pattern = rule_information.event_pattern._pattern
-        if not filter_event(event_pattern, event):
+        if not matches_event(event_pattern, event):
             return False
     return True
 
 
 def filter_event_with_target_input_path(target: Dict, event: Dict) -> Dict:
     input_path = target.get("InputPath")
     if input_path:
```

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/provider_v2.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_connection.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_connection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_connection.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_connection.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_connection_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_connection_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_eventbus.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_eventbus.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_eventbus.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_eventbus.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_eventbus_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_eventbus_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_eventbuspolicy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_eventbuspolicy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_eventbuspolicy.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_eventbuspolicy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_eventbuspolicy_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_eventbuspolicy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_rule.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_rule.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_rule.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/resource_providers/aws_events_rule_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/resource_providers/aws_events_rule_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/events/scheduler.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/firehose/mappers.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/firehose/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/firehose/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_accesskey.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_accesskey.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_accesskey.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_accesskey.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_accesskey_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_accesskey_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_group.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_group.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_group.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_group.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_instanceprofile.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_instanceprofile.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_instanceprofile.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_instanceprofile.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_instanceprofile_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_instanceprofile_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_managedpolicy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_managedpolicy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_managedpolicy.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_managedpolicy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_managedpolicy_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_managedpolicy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_policy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_policy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_policy.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_policy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_policy_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_policy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_role.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_role.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_role.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_role.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_servercertificate.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_servercertificate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_servercertificate.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_servercertificate.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_servercertificate_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_servercertificate_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_user.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_user.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/iam/resource_providers/aws_iam_user.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/iam/resource_providers/aws_iam_user.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/infra.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/internal.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/packages.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/aws_kinesis_stream.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/aws_kinesis_stream.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/aws_kinesis_stream.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/aws_kinesis_stream.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/aws_kinesis_stream_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/aws_kinesis_stream_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kms/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kms/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kms/resource_providers/aws_kms_alias.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kms/resource_providers/aws_kms_alias.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kms/resource_providers/aws_kms_alias.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kms/resource_providers/aws_kms_alias.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kms/resource_providers/aws_kms_key.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kms/resource_providers/aws_kms_key.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kms/resource_providers/aws_kms_key.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kms/resource_providers/aws_kms_key.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/kms/utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/api_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/adapters.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/event_source_listener.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/lambda_legacy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/lambda_legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/event_source_listeners/stream_event_source_listener.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/hooks.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/assignment.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/assignment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/counting_service.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/counting_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/docker_runtime_executor.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/event_manager.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/event_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/execution_environment.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/execution_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/executor_endpoint.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/internal_sqs_queue.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/internal_sqs_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/lambda_models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/lambda_service.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/logs.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/metrics.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/metrics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/runtime_executor.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/invocation/version_manager.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/lambda_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/layerfetcher/layer_fetcher.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/networking.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/packages.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/plugins.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_function.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_function.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_function.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_function_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_function_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_layerversion_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_layerversion_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_permission.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_permission.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_permission.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_permission.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_permission_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_permission_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_url.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_url.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_url.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_url_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_url_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_version.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_version.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_version.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_version.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/aws_lambda_version_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/aws_lambda_version_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/lambda_alias.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/lambda_alias.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/lambda_alias.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/lambda_alias.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/resource_providers/lambda_alias_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/resource_providers/lambda_alias_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/runtimes.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/runtimes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/lambda_/urlrouter.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/lambda_/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/logs/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/logs/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_loggroup.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_loggroup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_loggroup.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_loggroup.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_loggroup_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_loggroup_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_logstream.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_logstream.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_logstream.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_logstream.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_logstream_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_logstream_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/messages.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/moto.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/cluster.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/cluster_manager.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/packages.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/opensearch/versions.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/plugins.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/providers.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/redshift/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/redshift/resource_providers/aws_redshift_cluster.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/redshift/resource_providers/aws_redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/redshift/resource_providers/aws_redshift_cluster.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/redshift/resource_providers/aws_redshift_cluster.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/redshift/resource_providers/aws_redshift_cluster_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/redshift/resource_providers/aws_redshift_cluster_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/route53/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/aws_route53_healthcheck.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/aws_route53_healthcheck.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/aws_route53_healthcheck.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/aws_route53_healthcheck.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/aws_route53_healthcheck_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/aws_route53_healthcheck_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/aws_route53_recordset.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/aws_route53_recordset.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/aws_route53_recordset.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/aws_route53_recordset.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/route53/resource_providers/aws_route53_recordset_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/route53/resource_providers/aws_route53_recordset_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/route53resolver/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/route53resolver/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/route53resolver/utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/codec.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/constants.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/cors.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/exceptions.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/notifications.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/presigned_url.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/aws_s3_bucket.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/aws_s3_bucket.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/aws_s3_bucket.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/aws_s3_bucket.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/resource_providers/aws_s3_bucketpolicy_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/resource_providers/aws_s3_bucketpolicy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/utils_moto.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/utils_moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/v3/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/v3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/v3/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/v3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/v3/storage/core.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/v3/storage/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/v3/storage/ephemeral.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/v3/storage/ephemeral.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/validation.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/validation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/virtual_host.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/s3/website_hosting.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/aws_scheduler_schedule_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/aws_scheduler_schedule_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ses/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/certificate.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/certificate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/constants.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/publisher.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_subscription.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_subscription.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_subscription.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_subscription.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_subscription_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_subscription_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_topic.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_topic.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_topic.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_topic.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_topicpolicy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_topicpolicy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_topicpolicy.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_topicpolicy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sns/resource_providers/aws_sns_topicpolicy_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sns/resource_providers/aws_sns_topicpolicy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/constants.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/exceptions.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/models.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/query_api.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/aws_sqs_queue.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/aws_sqs_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/aws_sqs_queue.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/aws_sqs_queue.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sqs/utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_parameter.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_parameter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_parameter_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_parameter_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/Makefile` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicLexer.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicLexer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParser.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserListener.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserListener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserVisitor.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserVisitor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLLexer.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLLexer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLParser.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLParser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserListener.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserListener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserVisitor.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserVisitor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/jitter_strategy_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/jitter_strategy_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/max_delay_seconds_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/max_delay_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_context_path.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_context_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_variable.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/variable.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/item_reader_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/item_reader_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/input_type.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/input_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/max_items_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/max_items_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_props.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_factory.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_s3.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_csv.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_csv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_factory.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_json.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/distributed_iteration_component.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/distributed_iteration_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/inline_iteration_component.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/inline_iteration_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor_worker.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor_worker.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_factory.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/map_run_record.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/map_run_record.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_declaration.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_declaration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator_worker.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator_worker.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_factory.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branch_worker.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branch_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_api_gateway.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_api_gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_ecs.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_ecs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_events.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_factory.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sns.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_activitiy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_activitiy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_factory.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_fail/cause_path.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_fail/cause_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_fail/error_path.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_fail/error_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/callback/callback.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/callback/callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/eval/program_state.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/eval/program_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/utils/boto_client.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/utils/boto_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/asl/utils/json_path.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/asl/utils/json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/activity.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/activity.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/backend/store.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/legacy/provider_legacy.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/legacy/provider_legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/legacy/stepfunctions_starter.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/legacy/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/packages.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.schema.json` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine_plugin.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/stores.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/sts/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/transcribe/packages.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/transcribe/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/services/transcribe/provider.py` & `localstack-core-3.3.1.dev20240408081905/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/state/core.py` & `localstack-core-3.3.1.dev20240408081905/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/state/inspect.py` & `localstack-core-3.3.1.dev20240408081905/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/state/pickle.py` & `localstack-core-3.3.1.dev20240408081905/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/state/snapshot.py` & `localstack-core-3.3.1.dev20240408081905/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/aws/asf_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/aws/eventbus_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/aws/eventbus_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/aws/lambda_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/aws/util.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/cloudtrail_tracking_stack.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/cloudtrail_tracking_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/handler/index.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/handler/index.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking/tests/test_cloudtrail_tracking_handler.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking/tests/test_cloudtrail_tracking_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/container.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/container.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/filters.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/fixtures.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/in_memory_localstack.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/in_memory_localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/marker_report.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/marker_report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/marking.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/marking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/metric_collection.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/path_filter.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/path_filter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/util.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/pytest/validation_tracking.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/pytest/validation_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/scenario/cdk_lambda_helper.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/scenario/cdk_lambda_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/scenario/provisioning.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/scenario/provisioning.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/git.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/git.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/github.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/github.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/matching.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/matching.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/opt_in.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/opt_in.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/scripts/filter_by_test_selection.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/scripts/filter_by_test_selection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/scripts/generate_test_selection_from_commits.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/scripts/generate_test_selection_from_commits.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/scripts/generate_test_selection_from_pr.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/scripts/generate_test_selection_from_pr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/testing/testselection/testselection.py` & `localstack-core-3.3.1.dev20240408081905/localstack/testing/testselection/testselection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/cli.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/client.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/events.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/logger.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/metadata.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/publisher.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/analytics/usage.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/archives.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/asyncio.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/auth.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/arns.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/aws_responses.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/aws_stack.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/client.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/client_types.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/message_forwarding.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/queries.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/request_context.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/resources.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/aws/templating.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/bootstrap.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/collections.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/common.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/config_listener.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/container_networking.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/container_utils/container_client.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/coverage_docs.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/crypto.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/diagnose.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/docker_utils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/files.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/functions.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/http.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/iputils.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/iputils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/json.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/net.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/no_exit_argument_parser.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/numbers.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/objects.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/patch.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/platform.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/run.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/scheduler.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/server/http2_server.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/server/proxy_server.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/serving.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/ssl.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/strings.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/sync.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/tagging.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/testutil.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/threads.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/time.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/urls.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/venv.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack/utils/xml.py` & `localstack-core-3.3.1.dev20240408081905/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/PKG-INFO` & `localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 3.3.1.dev20240408065452
+Version: 3.3.1.dev20240408081905
 Summary: The core library and runtime of LocalStack
 Author-email: LocalStack Contributors <info@localstack.cloud>
 Project-URL: Homepage, https://localstack.cloud
 Project-URL: Documentation, https://docs.localstack.cloud
 Project-URL: Repository, https://github.com/localstack/localstack.git
 Project-URL: Issues, https://github.com/localstack/localstack/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/SOURCES.txt` & `localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -362,14 +362,15 @@
 localstack/services/es/plugins.py
 localstack/services/es/provider.py
 localstack/services/events/__init__.py
 localstack/services/events/models.py
 localstack/services/events/provider.py
 localstack/services/events/provider_v2.py
 localstack/services/events/scheduler.py
+localstack/services/events/utils.py
 localstack/services/events/resource_providers/__init__.py
 localstack/services/events/resource_providers/aws_events_connection.py
 localstack/services/events/resource_providers/aws_events_connection.schema.json
 localstack/services/events/resource_providers/aws_events_connection_plugin.py
 localstack/services/events/resource_providers/aws_events_eventbus.py
 localstack/services/events/resource_providers/aws_events_eventbus.schema.json
 localstack/services/events/resource_providers/aws_events_eventbus_plugin.py
```

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/entry_points.txt` & `localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/plux.json` & `localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/plux.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8187864465954353%*

 * *Differences: {"'localstack.cloudformation.resource_providers'": '{insert: [(0, '*

 * *                                                   "'AWS::ApiGateway::GatewayResponse=localstack.services.apigateway.resource_providers.aws_apigateway_gatewayresponse_plugin:ApiGatewayGatewayResponseProviderPlugin'), "*

 * *                                                   '(1, '*

 * *                                                   "'AWS::ApiGateway::ApiKey=localstack.services.apigateway.resource_providers.aws_apigateway_apikey_plugin:ApiGatewayA […]*

```diff
@@ -47,149 +47,149 @@
         "stepfunctions:v2=localstack.services.providers:stepfunctions_v2",
         "sts:default=localstack.services.providers:sts",
         "support:default=localstack.services.providers:support",
         "swf:default=localstack.services.providers:swf",
         "transcribe:default=localstack.services.providers:transcribe"
     ],
     "localstack.cloudformation.resource_providers": [
-        "AWS::Scheduler::Schedule=localstack.services.scheduler.resource_providers.aws_scheduler_schedule_plugin:SchedulerScheduleProviderPlugin",
-        "AWS::CloudFormation::Macro=localstack.services.cloudformation.resource_providers.aws_cloudformation_macro_plugin:CloudFormationMacroProviderPlugin",
-        "AWS::EC2::Instance=localstack.services.ec2.resource_providers.aws_ec2_instance_plugin:EC2InstanceProviderPlugin",
-        "AWS::Lambda::CodeSigningConfig=localstack.services.lambda_.resource_providers.aws_lambda_codesigningconfig_plugin:LambdaCodeSigningConfigProviderPlugin",
-        "AWS::ApiGateway::BasePathMapping=localstack.services.apigateway.resource_providers.aws_apigateway_basepathmapping_plugin:ApiGatewayBasePathMappingProviderPlugin",
+        "AWS::ApiGateway::GatewayResponse=localstack.services.apigateway.resource_providers.aws_apigateway_gatewayresponse_plugin:ApiGatewayGatewayResponseProviderPlugin",
+        "AWS::ApiGateway::ApiKey=localstack.services.apigateway.resource_providers.aws_apigateway_apikey_plugin:ApiGatewayApiKeyProviderPlugin",
+        "AWS::EC2::Subnet=localstack.services.ec2.resource_providers.aws_ec2_subnet_plugin:EC2SubnetProviderPlugin",
+        "AWS::ApiGateway::RequestValidator=localstack.services.apigateway.resource_providers.aws_apigateway_requestvalidator_plugin:ApiGatewayRequestValidatorProviderPlugin",
+        "AWS::SQS::QueuePolicy=localstack.services.sqs.resource_providers.aws_sqs_queuepolicy_plugin:SQSQueuePolicyProviderPlugin",
+        "AWS::DynamoDB::Table=localstack.services.dynamodb.resource_providers.aws_dynamodb_table_plugin:DynamoDBTableProviderPlugin",
+        "AWS::EC2::NatGateway=localstack.services.ec2.resource_providers.aws_ec2_natgateway_plugin:EC2NatGatewayProviderPlugin",
+        "AWS::EC2::KeyPair=localstack.services.ec2.resource_providers.aws_ec2_keypair_plugin:EC2KeyPairProviderPlugin",
+        "AWS::ECR::Repository=localstack.services.ecr.resource_providers.aws_ecr_repository_plugin:ECRRepositoryProviderPlugin",
+        "AWS::SecretsManager::SecretTargetAttachment=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_secrettargetattachment_plugin:SecretsManagerSecretTargetAttachmentProviderPlugin",
         "AWS::SNS::TopicPolicy=localstack.services.sns.resource_providers.aws_sns_topicpolicy_plugin:SNSTopicPolicyProviderPlugin",
+        "AWS::ApiGateway::BasePathMapping=localstack.services.apigateway.resource_providers.aws_apigateway_basepathmapping_plugin:ApiGatewayBasePathMappingProviderPlugin",
+        "AWS::Lambda::EventInvokeConfig=localstack.services.lambda_.resource_providers.aws_lambda_eventinvokeconfig_plugin:LambdaEventInvokeConfigProviderPlugin",
+        "AWS::SQS::Queue=localstack.services.sqs.resource_providers.aws_sqs_queue_plugin:SQSQueueProviderPlugin",
         "AWS::ApiGateway::Resource=localstack.services.apigateway.resource_providers.aws_apigateway_resource_plugin:ApiGatewayResourceProviderPlugin",
-        "AWS::IAM::Policy=localstack.services.iam.resource_providers.aws_iam_policy_plugin:IAMPolicyProviderPlugin",
-        "AWS::ApiGateway::Model=localstack.services.apigateway.resource_providers.aws_apigateway_model_plugin:ApiGatewayModelProviderPlugin",
+        "AWS::Scheduler::ScheduleGroup=localstack.services.scheduler.resource_providers.aws_scheduler_schedulegroup_plugin:SchedulerScheduleGroupProviderPlugin",
+        "AWS::EC2::Instance=localstack.services.ec2.resource_providers.aws_ec2_instance_plugin:EC2InstanceProviderPlugin",
         "AWS::Events::Rule=localstack.services.events.resource_providers.aws_events_rule_plugin:EventsRuleProviderPlugin",
-        "AWS::EC2::SubnetRouteTableAssociation=localstack.services.ec2.resource_providers.aws_ec2_subnetroutetableassociation_plugin:EC2SubnetRouteTableAssociationProviderPlugin",
-        "AWS::Lambda::EventSourceMapping=localstack.services.lambda_.resource_providers.aws_lambda_eventsourcemapping_plugin:LambdaEventSourceMappingProviderPlugin",
+        "AWS::EC2::InternetGateway=localstack.services.ec2.resource_providers.aws_ec2_internetgateway_plugin:EC2InternetGatewayProviderPlugin",
         "AWS::SSM::Parameter=localstack.services.ssm.resource_providers.aws_ssm_parameter_plugin:SSMParameterProviderPlugin",
-        "AWS::Lambda::EventInvokeConfig=localstack.services.lambda_.resource_providers.aws_lambda_eventinvokeconfig_plugin:LambdaEventInvokeConfigProviderPlugin",
-        "AWS::SQS::Queue=localstack.services.sqs.resource_providers.aws_sqs_queue_plugin:SQSQueueProviderPlugin",
-        "AWS::ApiGateway::Method=localstack.services.apigateway.resource_providers.aws_apigateway_method_plugin:ApiGatewayMethodProviderPlugin",
-        "AWS::IAM::Group=localstack.services.iam.resource_providers.aws_iam_group_plugin:IAMGroupProviderPlugin",
-        "AWS::CloudFormation::WaitCondition=localstack.services.cloudformation.resource_providers.aws_cloudformation_waitcondition_plugin:CloudFormationWaitConditionProviderPlugin",
-        "AWS::EC2::TransitGatewayAttachment=localstack.services.ec2.resource_providers.aws_ec2_transitgatewayattachment_plugin:EC2TransitGatewayAttachmentProviderPlugin",
-        "AWS::Redshift::Cluster=localstack.services.redshift.resource_providers.aws_redshift_cluster_plugin:RedshiftClusterProviderPlugin",
-        "AWS::ECR::Repository=localstack.services.ecr.resource_providers.aws_ecr_repository_plugin:ECRRepositoryProviderPlugin",
-        "AWS::StepFunctions::Activity=localstack.services.stepfunctions.resource_providers.aws_stepfunctions_activity_plugin:StepFunctionsActivityProviderPlugin",
-        "AWS::Lambda::Url=localstack.services.lambda_.resource_providers.aws_lambda_url_plugin:LambdaUrlProviderPlugin",
-        "AWS::Elasticsearch::Domain=localstack.services.opensearch.resource_providers.aws_elasticsearch_domain_plugin:ElasticsearchDomainProviderPlugin",
-        "AWS::CloudWatch::CompositeAlarm=localstack.services.cloudwatch.resource_providers.aws_cloudwatch_compositealarm_plugin:CloudWatchCompositeAlarmProviderPlugin",
-        "AWS::IAM::Role=localstack.services.iam.resource_providers.aws_iam_role_plugin:IAMRoleProviderPlugin",
-        "AWS::EC2::DHCPOptions=localstack.services.ec2.resource_providers.aws_ec2_dhcpoptions_plugin:EC2DHCPOptionsProviderPlugin",
-        "AWS::KMS::Key=localstack.services.kms.resource_providers.aws_kms_key_plugin:KMSKeyProviderPlugin",
-        "AWS::IAM::ServiceLinkedRole=localstack.services.iam.resource_providers.aws_iam_servicelinkedrole_plugin:IAMServiceLinkedRoleProviderPlugin",
+        "AWS::Route53::RecordSet=localstack.services.route53.resource_providers.aws_route53_recordset_plugin:Route53RecordSetProviderPlugin",
         "AWS::CertificateManager::Certificate=localstack.services.certificatemanager.resource_providers.aws_certificatemanager_certificate_plugin:CertificateManagerCertificateProviderPlugin",
-        "AWS::EC2::KeyPair=localstack.services.ec2.resource_providers.aws_ec2_keypair_plugin:EC2KeyPairProviderPlugin",
-        "AWS::EC2::Subnet=localstack.services.ec2.resource_providers.aws_ec2_subnet_plugin:EC2SubnetProviderPlugin",
-        "AWS::IAM::User=localstack.services.iam.resource_providers.aws_iam_user_plugin:IAMUserProviderPlugin",
-        "AWS::EC2::InternetGateway=localstack.services.ec2.resource_providers.aws_ec2_internetgateway_plugin:EC2InternetGatewayProviderPlugin",
-        "AWS::Lambda::Version=localstack.services.lambda_.resource_providers.aws_lambda_version_plugin:LambdaVersionProviderPlugin",
-        "AWS::Lambda::Permission=localstack.services.lambda_.resource_providers.aws_lambda_permission_plugin:LambdaPermissionProviderPlugin",
-        "AWS::ApiGateway::Stage=localstack.services.apigateway.resource_providers.aws_apigateway_stage_plugin:ApiGatewayStageProviderPlugin",
-        "AWS::KMS::Alias=localstack.services.kms.resource_providers.aws_kms_alias_plugin:KMSAliasProviderPlugin",
-        "AWS::EC2::VPCGatewayAttachment=localstack.services.ec2.resource_providers.aws_ec2_vpcgatewayattachment_plugin:EC2VPCGatewayAttachmentProviderPlugin",
-        "AWS::SQS::QueuePolicy=localstack.services.sqs.resource_providers.aws_sqs_queuepolicy_plugin:SQSQueuePolicyProviderPlugin",
-        "AWS::KinesisFirehose::DeliveryStream=localstack.services.kinesisfirehose.resource_providers.aws_kinesisfirehose_deliverystream_plugin:KinesisFirehoseDeliveryStreamProviderPlugin",
+        "AWS::S3::Bucket=localstack.services.s3.resource_providers.aws_s3_bucket_plugin:S3BucketProviderPlugin",
+        "AWS::IAM::Policy=localstack.services.iam.resource_providers.aws_iam_policy_plugin:IAMPolicyProviderPlugin",
+        "AWS::IAM::ServiceLinkedRole=localstack.services.iam.resource_providers.aws_iam_servicelinkedrole_plugin:IAMServiceLinkedRoleProviderPlugin",
+        "AWS::StepFunctions::StateMachine=localstack.services.stepfunctions.resource_providers.aws_stepfunctions_statemachine_plugin:StepFunctionsStateMachineProviderPlugin",
+        "AWS::CloudFormation::WaitConditionHandle=localstack.services.cloudformation.resource_providers.aws_cloudformation_waitconditionhandle_plugin:CloudFormationWaitConditionHandleProviderPlugin",
+        "AWS::ApiGateway::UsagePlan=localstack.services.apigateway.resource_providers.aws_apigateway_usageplan_plugin:ApiGatewayUsagePlanProviderPlugin",
         "AWS::Lambda::LayerVersion=localstack.services.lambda_.resource_providers.aws_lambda_layerversion_plugin:LambdaLayerVersionProviderPlugin",
+        "AWS::SecretsManager::Secret=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_secret_plugin:SecretsManagerSecretProviderPlugin",
+        "AWS::ApiGateway::Deployment=localstack.services.apigateway.resource_providers.aws_apigateway_deployment_plugin:ApiGatewayDeploymentProviderPlugin",
+        "AWS::OpenSearchService::Domain=localstack.services.opensearch.resource_providers.aws_opensearchservice_domain_plugin:OpenSearchServiceDomainProviderPlugin",
+        "AWS::SNS::Subscription=localstack.services.sns.resource_providers.aws_sns_subscription_plugin:SNSSubscriptionProviderPlugin",
+        "AWS::IAM::AccessKey=localstack.services.iam.resource_providers.aws_iam_accesskey_plugin:IAMAccessKeyProviderPlugin",
+        "AWS::SecretsManager::ResourcePolicy=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_resourcepolicy_plugin:SecretsManagerResourcePolicyProviderPlugin",
+        "AWS::CloudWatch::CompositeAlarm=localstack.services.cloudwatch.resource_providers.aws_cloudwatch_compositealarm_plugin:CloudWatchCompositeAlarmProviderPlugin",
+        "AWS::CloudFormation::Macro=localstack.services.cloudformation.resource_providers.aws_cloudformation_macro_plugin:CloudFormationMacroProviderPlugin",
+        "AWS::Lambda::Function=localstack.services.lambda_.resource_providers.aws_lambda_function_plugin:LambdaFunctionProviderPlugin",
+        "AWS::KMS::Key=localstack.services.kms.resource_providers.aws_kms_key_plugin:KMSKeyProviderPlugin",
+        "AWS::Lambda::LayerVersionPermission=localstack.services.lambda_.resource_providers.aws_lambda_layerversionpermission_plugin:LambdaLayerVersionPermissionProviderPlugin",
+        "AWS::Logs::LogStream=localstack.services.logs.resource_providers.aws_logs_logstream_plugin:LogsLogStreamProviderPlugin",
         "AWS::Events::EventBusPolicy=localstack.services.events.resource_providers.aws_events_eventbuspolicy_plugin:EventsEventBusPolicyProviderPlugin",
-        "AWS::ResourceGroups::Group=localstack.services.resource_groups.resource_providers.aws_resourcegroups_group_plugin:ResourceGroupsGroupProviderPlugin",
-        "AWS::EC2::NatGateway=localstack.services.ec2.resource_providers.aws_ec2_natgateway_plugin:EC2NatGatewayProviderPlugin",
-        "AWS::Lambda::Alias=localstack.services.lambda_.resource_providers.lambda_alias_plugin:LambdaAliasProviderPlugin",
-        "AWS::SSM::PatchBaseline=localstack.services.ssm.resource_providers.aws_ssm_patchbaseline_plugin:SSMPatchBaselineProviderPlugin",
+        "AWS::Kinesis::Stream=localstack.services.kinesis.resource_providers.aws_kinesis_stream_plugin:KinesisStreamProviderPlugin",
         "AWS::EC2::VPC=localstack.services.ec2.resource_providers.aws_ec2_vpc_plugin:EC2VPCProviderPlugin",
+        "AWS::EC2::DHCPOptions=localstack.services.ec2.resource_providers.aws_ec2_dhcpoptions_plugin:EC2DHCPOptionsProviderPlugin",
+        "AWS::ApiGateway::Account=localstack.services.apigateway.resource_providers.aws_apigateway_account_plugin:ApiGatewayAccountProviderPlugin",
+        "AWS::SSM::MaintenanceWindowTask=localstack.services.ssm.resource_providers.aws_ssm_maintenancewindowtask_plugin:SSMMaintenanceWindowTaskProviderPlugin",
+        "AWS::EC2::SecurityGroup=localstack.services.ec2.resource_providers.aws_ec2_securitygroup_plugin:EC2SecurityGroupProviderPlugin",
+        "AWS::Elasticsearch::Domain=localstack.services.opensearch.resource_providers.aws_elasticsearch_domain_plugin:ElasticsearchDomainProviderPlugin",
+        "AWS::EC2::TransitGateway=localstack.services.ec2.resource_providers.aws_ec2_transitgateway_plugin:EC2TransitGatewayProviderPlugin",
+        "AWS::Lambda::Version=localstack.services.lambda_.resource_providers.aws_lambda_version_plugin:LambdaVersionProviderPlugin",
+        "AWS::EC2::RouteTable=localstack.services.ec2.resource_providers.aws_ec2_routetable_plugin:EC2RouteTableProviderPlugin",
+        "AWS::SSM::PatchBaseline=localstack.services.ssm.resource_providers.aws_ssm_patchbaseline_plugin:SSMPatchBaselineProviderPlugin",
+        "AWS::Lambda::Url=localstack.services.lambda_.resource_providers.aws_lambda_url_plugin:LambdaUrlProviderPlugin",
+        "AWS::IAM::Group=localstack.services.iam.resource_providers.aws_iam_group_plugin:IAMGroupProviderPlugin",
         "AWS::Kinesis::StreamConsumer=localstack.services.kinesis.resource_providers.aws_kinesis_streamconsumer_plugin:KinesisStreamConsumerProviderPlugin",
+        "AWS::S3::BucketPolicy=localstack.services.s3.resource_providers.aws_s3_bucketpolicy_plugin:S3BucketPolicyProviderPlugin",
+        "AWS::Logs::SubscriptionFilter=localstack.services.logs.resource_providers.aws_logs_subscriptionfilter_plugin:LogsSubscriptionFilterProviderPlugin",
         "AWS::Events::Connection=localstack.services.events.resource_providers.aws_events_connection_plugin:EventsConnectionProviderPlugin",
+        "AWS::IAM::ServerCertificate=localstack.services.iam.resource_providers.aws_iam_servercertificate_plugin:IAMServerCertificateProviderPlugin",
+        "AWS::ApiGateway::DomainName=localstack.services.apigateway.resource_providers.aws_apigateway_domainname_plugin:ApiGatewayDomainNameProviderPlugin",
+        "AWS::SSM::MaintenanceWindowTarget=localstack.services.ssm.resource_providers.aws_ssm_maintenancewindowtarget_plugin:SSMMaintenanceWindowTargetProviderPlugin",
+        "AWS::ResourceGroups::Group=localstack.services.resource_groups.resource_providers.aws_resourcegroups_group_plugin:ResourceGroupsGroupProviderPlugin",
+        "AWS::EC2::NetworkAcl=localstack.services.ec2.resource_providers.aws_ec2_networkacl_plugin:EC2NetworkAclProviderPlugin",
+        "AWS::ApiGateway::Method=localstack.services.apigateway.resource_providers.aws_apigateway_method_plugin:ApiGatewayMethodProviderPlugin",
+        "AWS::EC2::SubnetRouteTableAssociation=localstack.services.ec2.resource_providers.aws_ec2_subnetroutetableassociation_plugin:EC2SubnetRouteTableAssociationProviderPlugin",
         "AWS::DynamoDB::GlobalTable=localstack.services.dynamodb.resource_providers.aws_dynamodb_globaltable_plugin:DynamoDBGlobalTableProviderPlugin",
-        "AWS::Route53::RecordSet=localstack.services.route53.resource_providers.aws_route53_recordset_plugin:Route53RecordSetProviderPlugin",
-        "AWS::SNS::Subscription=localstack.services.sns.resource_providers.aws_sns_subscription_plugin:SNSSubscriptionProviderPlugin",
-        "AWS::ApiGateway::Deployment=localstack.services.apigateway.resource_providers.aws_apigateway_deployment_plugin:ApiGatewayDeploymentProviderPlugin",
-        "AWS::ApiGateway::RequestValidator=localstack.services.apigateway.resource_providers.aws_apigateway_requestvalidator_plugin:ApiGatewayRequestValidatorProviderPlugin",
-        "AWS::Logs::LogGroup=localstack.services.logs.resource_providers.aws_logs_loggroup_plugin:LogsLogGroupProviderPlugin",
-        "AWS::CloudFormation::WaitConditionHandle=localstack.services.cloudformation.resource_providers.aws_cloudformation_waitconditionhandle_plugin:CloudFormationWaitConditionHandleProviderPlugin",
-        "AWS::Kinesis::Stream=localstack.services.kinesis.resource_providers.aws_kinesis_stream_plugin:KinesisStreamProviderPlugin",
-        "AWS::SecretsManager::SecretTargetAttachment=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_secrettargetattachment_plugin:SecretsManagerSecretTargetAttachmentProviderPlugin",
-        "AWS::Lambda::Function=localstack.services.lambda_.resource_providers.aws_lambda_function_plugin:LambdaFunctionProviderPlugin",
-        "AWS::SecretsManager::Secret=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_secret_plugin:SecretsManagerSecretProviderPlugin",
-        "AWS::IAM::InstanceProfile=localstack.services.iam.resource_providers.aws_iam_instanceprofile_plugin:IAMInstanceProfileProviderPlugin",
-        "AWS::ApiGateway::GatewayResponse=localstack.services.apigateway.resource_providers.aws_apigateway_gatewayresponse_plugin:ApiGatewayGatewayResponseProviderPlugin",
-        "AWS::CloudFormation::Stack=localstack.services.cloudformation.resource_providers.aws_cloudformation_stack_plugin:CloudFormationStackProviderPlugin",
-        "AWS::Scheduler::ScheduleGroup=localstack.services.scheduler.resource_providers.aws_scheduler_schedulegroup_plugin:SchedulerScheduleGroupProviderPlugin",
+        "AWS::ApiGateway::Stage=localstack.services.apigateway.resource_providers.aws_apigateway_stage_plugin:ApiGatewayStageProviderPlugin",
+        "AWS::Events::EventBus=localstack.services.events.resource_providers.aws_events_eventbus_plugin:EventsEventBusProviderPlugin",
+        "AWS::EC2::TransitGatewayAttachment=localstack.services.ec2.resource_providers.aws_ec2_transitgatewayattachment_plugin:EC2TransitGatewayAttachmentProviderPlugin",
+        "AWS::IAM::ManagedPolicy=localstack.services.iam.resource_providers.aws_iam_managedpolicy_plugin:IAMManagedPolicyProviderPlugin",
+        "AWS::IAM::Role=localstack.services.iam.resource_providers.aws_iam_role_plugin:IAMRoleProviderPlugin",
+        "AWS::StepFunctions::Activity=localstack.services.stepfunctions.resource_providers.aws_stepfunctions_activity_plugin:StepFunctionsActivityProviderPlugin",
+        "AWS::CDK::Metadata=localstack.services.cdk.resource_providers.cdk_metadata_plugin:LambdaAliasProviderPlugin",
         "AWS::ApiGateway::RestApi=localstack.services.apigateway.resource_providers.aws_apigateway_restapi_plugin:ApiGatewayRestApiProviderPlugin",
-        "AWS::SecretsManager::ResourcePolicy=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_resourcepolicy_plugin:SecretsManagerResourcePolicyProviderPlugin",
+        "AWS::Lambda::Permission=localstack.services.lambda_.resource_providers.aws_lambda_permission_plugin:LambdaPermissionProviderPlugin",
+        "AWS::ApiGateway::Model=localstack.services.apigateway.resource_providers.aws_apigateway_model_plugin:ApiGatewayModelProviderPlugin",
+        "AWS::IAM::User=localstack.services.iam.resource_providers.aws_iam_user_plugin:IAMUserProviderPlugin",
+        "AWS::Logs::LogGroup=localstack.services.logs.resource_providers.aws_logs_loggroup_plugin:LogsLogGroupProviderPlugin",
+        "AWS::CloudFormation::WaitCondition=localstack.services.cloudformation.resource_providers.aws_cloudformation_waitcondition_plugin:CloudFormationWaitConditionProviderPlugin",
         "AWS::SecretsManager::RotationSchedule=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_rotationschedule_plugin:SecretsManagerRotationScheduleProviderPlugin",
-        "AWS::Logs::SubscriptionFilter=localstack.services.logs.resource_providers.aws_logs_subscriptionfilter_plugin:LogsSubscriptionFilterProviderPlugin",
-        "AWS::DynamoDB::Table=localstack.services.dynamodb.resource_providers.aws_dynamodb_table_plugin:DynamoDBTableProviderPlugin",
+        "AWS::Redshift::Cluster=localstack.services.redshift.resource_providers.aws_redshift_cluster_plugin:RedshiftClusterProviderPlugin",
+        "AWS::Lambda::CodeSigningConfig=localstack.services.lambda_.resource_providers.aws_lambda_codesigningconfig_plugin:LambdaCodeSigningConfigProviderPlugin",
+        "AWS::KinesisFirehose::DeliveryStream=localstack.services.kinesisfirehose.resource_providers.aws_kinesisfirehose_deliverystream_plugin:KinesisFirehoseDeliveryStreamProviderPlugin",
+        "AWS::CloudFormation::Stack=localstack.services.cloudformation.resource_providers.aws_cloudformation_stack_plugin:CloudFormationStackProviderPlugin",
+        "AWS::ApiGateway::UsagePlanKey=localstack.services.apigateway.resource_providers.aws_apigateway_usageplankey_plugin:ApiGatewayUsagePlanKeyProviderPlugin",
+        "AWS::Scheduler::Schedule=localstack.services.scheduler.resource_providers.aws_scheduler_schedule_plugin:SchedulerScheduleProviderPlugin",
+        "AWS::IAM::InstanceProfile=localstack.services.iam.resource_providers.aws_iam_instanceprofile_plugin:IAMInstanceProfileProviderPlugin",
         "AWS::SSM::MaintenanceWindow=localstack.services.ssm.resource_providers.aws_ssm_maintenancewindow_plugin:SSMMaintenanceWindowProviderPlugin",
-        "AWS::EC2::Route=localstack.services.ec2.resource_providers.aws_ec2_route_plugin:EC2RouteProviderPlugin",
-        "AWS::IAM::ManagedPolicy=localstack.services.iam.resource_providers.aws_iam_managedpolicy_plugin:IAMManagedPolicyProviderPlugin",
-        "AWS::ApiGateway::ApiKey=localstack.services.apigateway.resource_providers.aws_apigateway_apikey_plugin:ApiGatewayApiKeyProviderPlugin",
-        "AWS::IAM::ServerCertificate=localstack.services.iam.resource_providers.aws_iam_servercertificate_plugin:IAMServerCertificateProviderPlugin",
-        "AWS::IAM::AccessKey=localstack.services.iam.resource_providers.aws_iam_accesskey_plugin:IAMAccessKeyProviderPlugin",
-        "AWS::EC2::RouteTable=localstack.services.ec2.resource_providers.aws_ec2_routetable_plugin:EC2RouteTableProviderPlugin",
-        "AWS::Lambda::LayerVersionPermission=localstack.services.lambda_.resource_providers.aws_lambda_layerversionpermission_plugin:LambdaLayerVersionPermissionProviderPlugin",
+        "AWS::Lambda::EventSourceMapping=localstack.services.lambda_.resource_providers.aws_lambda_eventsourcemapping_plugin:LambdaEventSourceMappingProviderPlugin",
         "AWS::Route53::HealthCheck=localstack.services.route53.resource_providers.aws_route53_healthcheck_plugin:Route53HealthCheckProviderPlugin",
-        "AWS::ApiGateway::DomainName=localstack.services.apigateway.resource_providers.aws_apigateway_domainname_plugin:ApiGatewayDomainNameProviderPlugin",
-        "AWS::SSM::MaintenanceWindowTask=localstack.services.ssm.resource_providers.aws_ssm_maintenancewindowtask_plugin:SSMMaintenanceWindowTaskProviderPlugin",
-        "AWS::ApiGateway::Account=localstack.services.apigateway.resource_providers.aws_apigateway_account_plugin:ApiGatewayAccountProviderPlugin",
-        "AWS::EC2::SecurityGroup=localstack.services.ec2.resource_providers.aws_ec2_securitygroup_plugin:EC2SecurityGroupProviderPlugin",
-        "AWS::Events::EventBus=localstack.services.events.resource_providers.aws_events_eventbus_plugin:EventsEventBusProviderPlugin",
-        "AWS::SNS::Topic=localstack.services.sns.resource_providers.aws_sns_topic_plugin:SNSTopicProviderPlugin",
         "AWS::CloudWatch::Alarm=localstack.services.cloudwatch.resource_providers.aws_cloudwatch_alarm_plugin:CloudWatchAlarmProviderPlugin",
-        "AWS::EC2::NetworkAcl=localstack.services.ec2.resource_providers.aws_ec2_networkacl_plugin:EC2NetworkAclProviderPlugin",
-        "AWS::OpenSearchService::Domain=localstack.services.opensearch.resource_providers.aws_opensearchservice_domain_plugin:OpenSearchServiceDomainProviderPlugin",
-        "AWS::S3::BucketPolicy=localstack.services.s3.resource_providers.aws_s3_bucketpolicy_plugin:S3BucketPolicyProviderPlugin",
-        "AWS::StepFunctions::StateMachine=localstack.services.stepfunctions.resource_providers.aws_stepfunctions_statemachine_plugin:StepFunctionsStateMachineProviderPlugin",
-        "AWS::ApiGateway::UsagePlanKey=localstack.services.apigateway.resource_providers.aws_apigateway_usageplankey_plugin:ApiGatewayUsagePlanKeyProviderPlugin",
-        "AWS::S3::Bucket=localstack.services.s3.resource_providers.aws_s3_bucket_plugin:S3BucketProviderPlugin",
-        "AWS::EC2::TransitGateway=localstack.services.ec2.resource_providers.aws_ec2_transitgateway_plugin:EC2TransitGatewayProviderPlugin",
-        "AWS::ApiGateway::UsagePlan=localstack.services.apigateway.resource_providers.aws_apigateway_usageplan_plugin:ApiGatewayUsagePlanProviderPlugin",
-        "AWS::SSM::MaintenanceWindowTarget=localstack.services.ssm.resource_providers.aws_ssm_maintenancewindowtarget_plugin:SSMMaintenanceWindowTargetProviderPlugin",
-        "AWS::CDK::Metadata=localstack.services.cdk.resource_providers.cdk_metadata_plugin:LambdaAliasProviderPlugin",
-        "AWS::Logs::LogStream=localstack.services.logs.resource_providers.aws_logs_logstream_plugin:LogsLogStreamProviderPlugin"
+        "AWS::SNS::Topic=localstack.services.sns.resource_providers.aws_sns_topic_plugin:SNSTopicProviderPlugin",
+        "AWS::EC2::VPCGatewayAttachment=localstack.services.ec2.resource_providers.aws_ec2_vpcgatewayattachment_plugin:EC2VPCGatewayAttachmentProviderPlugin",
+        "AWS::EC2::Route=localstack.services.ec2.resource_providers.aws_ec2_route_plugin:EC2RouteProviderPlugin",
+        "AWS::KMS::Alias=localstack.services.kms.resource_providers.aws_kms_alias_plugin:KMSAliasProviderPlugin",
+        "AWS::Lambda::Alias=localstack.services.lambda_.resource_providers.lambda_alias_plugin:LambdaAliasProviderPlugin"
     ],
     "localstack.hooks.configure_localstack_container": [
         "_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file"
     ],
     "localstack.hooks.on_infra_ready": [
-        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
-        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
+        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes",
+        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
     ],
     "localstack.hooks.on_infra_shutdown": [
-        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
-        "stop_server=localstack.dns.plugins:stop_server",
         "run_on_after_service_shutdown_handlers=localstack.runtime.shutdown:run_on_after_service_shutdown_handlers",
         "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
-        "shutdown_services=localstack.runtime.shutdown:shutdown_services"
+        "shutdown_services=localstack.runtime.shutdown:shutdown_services",
+        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
+        "stop_server=localstack.dns.plugins:stop_server"
     ],
     "localstack.hooks.on_infra_start": [
-        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
+        "validate_configuration=localstack.services.lambda_.plugins:validate_configuration",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
-        "validate_configuration=localstack.services.lambda_.plugins:validate_configuration",
         "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
         "setup_dns_configuration_on_host=localstack.dns.plugins:setup_dns_configuration_on_host",
-        "start_dns_server=localstack.dns.plugins:start_dns_server"
+        "start_dns_server=localstack.dns.plugins:start_dns_server",
+        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.lambda_.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "lambda-java-libs/community=localstack.services.lambda_.plugins:lambda_java_libs",
-        "lambda-runtime/community=localstack.services.lambda_.plugins:lambda_runtime_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
-        "vosk/community=localstack.services.transcribe.plugins:vosk_package",
         "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
         "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
         "terraform/community=localstack.packages.plugins:terraform_package",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
         "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package"
+        "lambda-java-libs/community=localstack.services.lambda_.plugins:lambda_java_libs",
+        "lambda-runtime/community=localstack.services.lambda_.plugins:lambda_runtime_package",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "vosk/community=localstack.services.transcribe.plugins:vosk_package"
     ]
 }
```

### Comparing `localstack-core-3.3.1.dev20240408065452/localstack_core.egg-info/requires.txt` & `localstack-core-3.3.1.dev20240408081905/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/pyproject.toml` & `localstack-core-3.3.1.dev20240408081905/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-3.3.1.dev20240408065452/setup.py` & `localstack-core-3.3.1.dev20240408081905/setup.py`

 * *Files identical despite different names*

