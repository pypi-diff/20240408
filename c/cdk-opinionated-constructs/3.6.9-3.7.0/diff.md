# Comparing `tmp/cdk-opinionated-constructs-3.6.9.tar.gz` & `tmp/cdk-opinionated-constructs-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-opinionated-constructs-3.6.9.tar", last modified: Tue Feb 27 13:27:39 2024, max compression
+gzip compressed data, was "cdk-opinionated-constructs-3.7.0.tar", last modified: Mon Apr  8 20:47:38 2024, max compression
```

## Comparing `cdk-opinionated-constructs-3.6.9.tar` & `cdk-opinionated-constructs-3.7.0.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-02-27 13:27:39.780925 cdk-opinionated-constructs-3.6.9/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-3.6.9/LICENSE
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      555 2024-02-27 13:27:39.780607 cdk-opinionated-constructs-3.6.9/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    27598 2024-02-26 09:49:43.000000 cdk-opinionated-constructs-3.6.9/README.md
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-02-27 13:27:39.652780 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     5852 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/alb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2817 2024-01-24 11:50:26.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/ecr.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    10448 2024-01-24 12:01:51.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/lmb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     6821 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/nlb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4710 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/rds_instance.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2933 2024-02-26 09:49:43.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/s3.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-02-27 13:27:39.654190 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/schemas/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/schemas/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3766 2024-02-05 17:16:33.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/schemas/configuration_vars.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1272 2024-02-26 09:49:43.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/sns.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-02-27 13:27:39.699413 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     8444 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2261 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/code_quality_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     6602 2024-02-06 00:49:23.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/governance_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2175 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1926 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/integration_tests_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     6534 2024-02-26 09:49:43.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/notifications_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1872 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3644 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-02-27 13:27:39.727918 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stages/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stages/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1104 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stages/code_quality_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      958 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stages/infrastructure_tests_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      934 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stages/integration_tests_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1045 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stages/notifications_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1494 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stages/plugins_stage.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-02-27 13:27:39.728509 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/utils/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2880 2024-02-05 22:11:31.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/utils/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    15910 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/wafv2.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-02-27 13:27:39.779015 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs.egg-info/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      555 2024-02-27 13:27:39.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs.egg-info/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2260 2024-02-27 13:27:39.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2024-02-27 13:27:39.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      125 2024-02-27 13:27:39.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs.egg-info/requires.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2024-02-27 13:27:39.000000 cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs.egg-info/top_level.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2024-02-27 13:27:39.781757 cdk-opinionated-constructs-3.6.9/setup.cfg
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      806 2024-02-27 13:27:25.000000 cdk-opinionated-constructs-3.6.9/setup.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-02-27 13:27:39.729454 cdk-opinionated-constructs-3.6.9/test/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-3.6.9/test/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1758 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/app.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-02-27 13:27:39.748829 cdk-opinionated-constructs-3.6.9/test/infrastucture/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/infrastucture/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2036 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/infrastucture/test_alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1173 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/infrastucture/test_ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1851 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/infrastucture/test_lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1516 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/infrastucture/test_s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1148 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/infrastucture/test_sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3739 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/infrastucture/test_wafv2_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-02-27 13:27:39.761157 cdk-opinionated-constructs-3.6.9/test/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-3.6.9/test/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3435 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/stacks/alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1384 2024-01-24 11:27:38.000000 cdk-opinionated-constructs-3.6.9/test/stacks/ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4412 2024-01-24 11:50:26.000000 cdk-opinionated-constructs-3.6.9/test/stacks/lmb_docker_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3591 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/stacks/lmb_monitoring_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2719 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/stacks/lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2152 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/stacks/nlb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3293 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/stacks/rds_mysql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3308 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/stacks/rds_postgresql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1619 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/stacks/s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1067 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/stacks/sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2567 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.6.9/test/stacks/wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.447295 cdk-opinionated-constructs-3.7.0/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-3.7.0/LICENSE
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      555 2024-04-08 20:47:38.447029 cdk-opinionated-constructs-3.7.0/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    27598 2024-02-26 09:49:43.000000 cdk-opinionated-constructs-3.7.0/README.md
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.382575 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     5852 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/alb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2817 2024-01-24 11:50:26.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/ecr.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    10448 2024-01-24 12:01:51.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/lmb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     6821 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/nlb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4710 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/rds_instance.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2933 2024-02-26 09:49:43.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/s3.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.384522 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/schemas/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/schemas/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3702 2024-03-06 09:09:15.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/schemas/configuration_vars.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1272 2024-02-26 09:49:43.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/sns.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.414843 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     8283 2024-03-21 08:42:47.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2261 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/code_quality_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     6602 2024-02-06 00:49:23.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/governance_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2101 2024-03-21 08:42:47.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1852 2024-03-21 08:42:47.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/integration_tests_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     7239 2024-04-08 20:45:23.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/notifications_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1872 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3644 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2077 2024-03-21 08:42:47.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/services_tests_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.417587 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1103 2024-03-04 14:20:14.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/code_quality_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      958 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/infrastructure_tests_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      934 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/integration_tests_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1045 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/notifications_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1494 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/plugins_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      915 2024-03-04 14:20:14.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/services_tests_stage.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.418087 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/utils/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2880 2024-02-05 22:11:31.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/utils/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    15910 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/wafv2.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.446365 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      555 2024-04-08 20:47:38.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2380 2024-04-08 20:47:38.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2024-04-08 20:47:38.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      125 2024-04-08 20:47:38.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/requires.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2024-04-08 20:47:38.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/top_level.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2024-04-08 20:47:38.448045 cdk-opinionated-constructs-3.7.0/setup.cfg
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      806 2024-04-08 20:47:06.000000 cdk-opinionated-constructs-3.7.0/setup.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.419117 cdk-opinionated-constructs-3.7.0/test/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-3.7.0/test/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1758 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/app.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.421429 cdk-opinionated-constructs-3.7.0/test/infrastucture/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2036 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/test_alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1173 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/test_ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1851 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/test_lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1516 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/test_s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1148 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/test_sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3739 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/test_wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.444028 cdk-opinionated-constructs-3.7.0/test/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-3.7.0/test/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3435 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1384 2024-01-24 11:27:38.000000 cdk-opinionated-constructs-3.7.0/test/stacks/ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4412 2024-01-24 11:50:26.000000 cdk-opinionated-constructs-3.7.0/test/stacks/lmb_docker_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3591 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/lmb_monitoring_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2719 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2152 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/nlb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3293 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/rds_mysql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3308 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/rds_postgresql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1619 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1067 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2567 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/wafv2_stack.py
```

### Comparing `cdk-opinionated-constructs-3.6.9/LICENSE` & `cdk-opinionated-constructs-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/PKG-INFO` & `cdk-opinionated-constructs-3.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-opinionated-constructs
-Version: 3.6.9
+Version: 3.7.0
 Summary: AWS CDK constructs come without added security configurations.
 License: MIT
 Requires-Python: >=3.11
 License-File: LICENSE
 Requires-Dist: aws-cdk-lib>=2.98.0
 Requires-Dist: constructs>=10.2.69
 Requires-Dist: cdk-monitoring-constructs>=6.0.0
```

### Comparing `cdk-opinionated-constructs-3.6.9/README.md` & `cdk-opinionated-constructs-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/alb.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/alb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/ecr.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/ecr.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/lmb.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/lmb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/nlb.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/nlb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/rds_instance.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/rds_instance.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/s3.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/s3.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/schemas/configuration_vars.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/schemas/configuration_vars.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,21 +65,21 @@
 
       - alarm_emails (list[EmailStr]): List of emails to receive alarm notifications.
 
       - plugins (PipelinePluginsVars): Pipeline plugins configuration.
 
       - project (str): The name of the project.
 
-      - stage (Literal["dev", "ppe", "prod", "dr"]): The deployment stage.
+      - stage (str): The deployment stage.
     """
 
     alarm_emails: list[EmailStr]
     plugins: PipelinePluginsVars
     project: str
-    stage: Literal["dev", "ppe", "prod", "dr"]
+    stage: str
 
 
 class ApplicationTags(BaseModel):
     """Defines the ApplicationTags model.
 
     This model represents the tags associated with an AWS application, specifically the AWS Resource Group ARN.
```

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/sns.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/sns.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/__init__.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,15 @@
 
     Parameters:
         - values: The environment configuration properties.
 
     Returns:
       - The number of characters.
     """
-
-    total_value_characters = sum(len(str(v)) for v in values.values())
-    total_key_characters = sum(len(str(v)) for v in values)
-    return total_key_characters + total_value_characters
+    return len(str(values))
 
 
 def reduce_items_number(
     values: dict[list, dict], standard_character_number: int = 4096
 ) -> dict[list, dict] | dict[str, str]:
     """Counts the number of characters in the values.
```

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/code_quality_stack.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/code_quality_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/governance_stack.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/governance_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import aws_cdk as cdk
 import aws_cdk.aws_ssm as ssm
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks
 from cdk_opinionated_constructs.schemas.configuration_vars import ConfigurationVars
-from cdk_opinionated_constructs.stacks import count_characters_number, reduce_items_number, set_ssm_parameter_tier_type
+from cdk_opinionated_constructs.stacks import reduce_items_number, set_ssm_parameter_tier_type
 from cdk_opinionated_constructs.utils import load_properties
 from constructs import Construct
 
 
 class InfrastructureTestsStack(cdk.Stack):
     """Infrastructure tests stack."""
 
@@ -38,19 +38,18 @@
         6. Validates the stack against the AWS Solutions checklist using Aspects.
         """
 
         super().__init__(scope, construct_id, env=env, **kwargs)
         config_vars = ConfigurationVars(**props)
 
         props_env = load_properties(stage=config_vars.stage)
-        character_number = count_characters_number(props_env)
         ssm_parameter_value = reduce_items_number(values=props_env)
 
         ssm.StringParameter(
             self,
             id="config_file",
             string_value=str(ssm_parameter_value),
             parameter_name=f"/{config_vars.project}/{config_vars.stage}/infrastructure/tests/config",
-            tier=set_ssm_parameter_tier_type(character_number=character_number),
+            tier=set_ssm_parameter_tier_type(character_number=len(str(ssm_parameter_value))),
         )
 
         Aspects.of(self).add(AwsSolutionsChecks(log_ignores=True))
```

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/integration_tests_stack.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 import aws_cdk as cdk
 import aws_cdk.aws_ssm as ssm
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks
 from cdk_opinionated_constructs.schemas.configuration_vars import ConfigurationVars
-from cdk_opinionated_constructs.stacks import count_characters_number, reduce_items_number, set_ssm_parameter_tier_type
 from cdk_opinionated_constructs.utils import load_properties
 from constructs import Construct
 
 
-class IntegrationTestsStack(cdk.Stack):
-    """IntegrationTestsStack defines a CDK stack for integration tests
-    configuration.
-
-    It loads configuration files from the cdk/config directory into a dict.
-    It creates a ConfigurationVars object from the combined props and config.
-
-    It stores the ConfigurationVars as a StringParameter in SSM, with a name built from
-    the config values.
-
-    It validates the stack against the AWS Solutions checklist.
-
-    Parameters:
-
-    - scope: The CDK scope constructing this stack.
-    - construct_id: ID for the stack construct.
-    - env: The CDK environment.
-    - props: Configuration properties passed to the stack.
-    - **kwargs: Additional stack options.
-    """
-
+class PipelinePluginsStack(cdk.Stack):
     def __init__(self, scope: Construct, construct_id: str, env, props, **kwargs) -> None:
+        """Initializes the PipelinePluginsStack construct.
+
+        Parameters:
+        - scope (Construct): The parent construct.
+        - construct_id (str): The construct ID.
+        - env: The CDK environment.
+        - props: Stack configuration properties.
+        - **kwargs: Additional keyword arguments passed to the Stack constructor.
+
+        The constructor does the following:
+
+        1. Call the parent Stack constructor.
+
+        2. Loads configuration from YAML files in the config directory for the stage.
+
+        3. Merge the loaded configuration with the passed props.
+
+        4. Create ConfigurationVars and PipelineVars objects from the configuration.
+
+        5. Create an SSM StringParameter to store the pipeline plugins configuration
+           from PipelineVars, for later retrieval.
+
+        6. Validates the stack against the AWS Solutions checklist using Aspects.
+        """
+
         super().__init__(scope, construct_id, env=env, **kwargs)
         config_vars = ConfigurationVars(**props)
-
         props_env = load_properties(stage=config_vars.stage)
-        character_number = count_characters_number(props_env)
-        ssm_parameter_value = reduce_items_number(values=props_env)
+
+        config_vars = ConfigurationVars(**props_env)
 
         ssm.StringParameter(
             self,
-            id="config_file",
-            string_value=str(ssm_parameter_value),
-            parameter_name=f"/{config_vars.project}/{config_vars.stage}/integration/tests/config",
-            tier=set_ssm_parameter_tier_type(character_number=character_number),
+            id="pipeline_plugins",
+            string_value=str(config_vars.plugins),
+            parameter_name=f"/{config_vars.project}/{config_vars.stage}/pipeline_plugins",
         )
 
         Aspects.of(self).add(AwsSolutionsChecks(log_ignores=True))
```

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/notifications_stack.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/notifications_stack.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,46 +16,39 @@
 class NotificationsStack(cdk.Stack):
     """Service stack.
 
     Create notifications cloudformation stack.
     """
 
     def __init__(self, scope: Construct, construct_id: str, env: cdk.Environment, props: dict, **kwargs) -> None:
-        """Initializes the NotificationsStack construct.
-
+        """
         Parameters:
-        - scope (Construct): The parent construct.
-        - construct_id (str): The construct ID.
-        - env (cdk.Environment): The CDK environment.
-        - props (dict): Stack configuration properties.
-        - **kwargs: Additional keyword arguments passed to the Stack constructor.
-
-        The constructor does the following:
-
-        1. Call the parent Stack constructor.
-
-        2. Loads configuration variables from YAML files.
-
-        3. Create a NotificationVars object from props.
-
-        4. Creates an SNS topic for alarms using the SNSTopic construct.
-
-        5. Grants CloudWatch permissions to publish to the SNS topic.
-
-        6. Creates an SSM parameter to store the SNS topic ARN.
-
-        7. Subscribe an email address to the SNS topic.
-
-        8. Conditionally create a Chatbot Slack channel subscription if Slack credentials are provided.
+        scope (Construct): The scope in which to define this construct.
+        construct_id (str): The scoped construct ID. Must be unique amongst siblings in the same scope.
+        env (cdk.Environment): The deployment environment (account/region) where the stack will be deployed.
+        props (dict): The properties for the notifications stack.
+        **kwargs: Additional keyword arguments.
+
+        Functionality:
+        Initializes a new instance of the NotificationsStack class,
+        which creates a notification CloudFormation stack.
+        This stack includes an SNS topic
+        configured with specific policies for CloudWatch and AWS Budgets to publish messages.
+        It also supports sending notifications to an email address and optionally to a Slack channel via AWS Chatbot.
+
+        Arguments:
+        scope: The scope in which this stack is defined.
+        construct_id: The unique ID for this stack.
+        env: The AWS environment (account and region) where the stack will be deployed.
+        props: A dictionary containing configuration properties for the stack,
+        such as project name, stage, and notification settings.
 
-        9. Adds CFN-NAG suppression.
-
-        10. Validates the stack against the AWS Solutions checklist using Aspects.
+        Returns:
+        None
         """
-
         super().__init__(scope, construct_id, env=env, **kwargs)
         config_vars = ConfigurationVars(**props)
 
         props_env = load_properties(stage=config_vars.stage)
 
         notifications_vars = NotificationVars(**props_env)
 
@@ -89,17 +82,24 @@
         ssm.StringParameter(
             self,
             id="sns_topic_ssm_param",
             string_value=sns_topic.topic_arn,
             parameter_name=f"/{config_vars.project}/{config_vars.stage}/topic/alarm/arn",
         )
 
-        sns_topic.add_subscription(
-            topic_subscription=sns_subscriptions.EmailSubscription(email_address=props["ci_cd_notification_email"]),
-        )
+        if ci_cd_notification_email := props.get("ci_cd_notification_email"):
+            sns_topic.add_subscription(
+                topic_subscription=sns_subscriptions.EmailSubscription(email_address=ci_cd_notification_email),
+            )
+
+        if alarm_emails := props.get("alarm_emails"):
+            for email in alarm_emails:
+                sns_topic.add_subscription(
+                    topic_subscription=sns_subscriptions.EmailSubscription(email_address=email),
+                )
 
         if notifications_vars.slack_workspace_id and notifications_vars.slack_channel_id_alarms:
             chatbot_iam_role = iam.Role(
                 self,
                 id="iam_role_chatbot",
                 assumed_by=iam.ServicePrincipal(service="chatbot.amazonaws.com"),
                 managed_policies=[iam.ManagedPolicy.from_aws_managed_policy_name("ReadOnlyAccess")],
@@ -130,14 +130,20 @@
             )
             chatbot_iam_role.add_to_policy(
                 iam.PolicyStatement(
                     actions=["cloudwatch:Describe*", "cloudwatch:Get*", "cloudwatch:List*"],
                     resources=["*"],
                 ),
             )
+            chatbot_iam_role.add_to_policy(
+                iam.PolicyStatement(
+                    actions=["codepipeline:RetryStageExecution"],
+                    resources=["*"],
+                ),
+            )
 
             chatbot.SlackChannelConfiguration(
                 self,
                 "chatbot",
                 slack_channel_configuration_name=f"{config_vars.project}-{config_vars.stage}",
                 notification_topics=[sns_topic],  # type: ignore
                 slack_workspace_id=notifications_vars.slack_workspace_id,
```

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/services_tests_stack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import aws_cdk as cdk
 import aws_cdk.aws_ssm as ssm
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks
 from cdk_opinionated_constructs.schemas.configuration_vars import ConfigurationVars
+from cdk_opinionated_constructs.stacks import reduce_items_number, set_ssm_parameter_tier_type
 from cdk_opinionated_constructs.utils import load_properties
 from constructs import Construct
 
 
-class PipelinePluginsStack(cdk.Stack):
+class ServicesTestsStack(cdk.Stack):
+    """Services tests stack."""
+
     def __init__(self, scope: Construct, construct_id: str, env, props, **kwargs) -> None:
-        """Initializes the PipelinePluginsStack construct.
+        """Initializes the ServicesTestsStack construct.
 
         Parameters:
         - scope (Construct): The parent construct.
         - construct_id (str): The construct ID.
         - env: The CDK environment.
         - props: Stack configuration properties.
         - **kwargs: Additional keyword arguments passed to the Stack constructor.
@@ -23,29 +26,30 @@
 
         1. Call the parent Stack constructor.
 
         2. Loads configuration from YAML files in the config directory for the stage.
 
         3. Merge the loaded configuration with the passed props.
 
-        4. Create ConfigurationVars and PipelineVars objects from the configuration.
+        4. Create a ConfigurationVars object from the merged configuration.
 
-        5. Create an SSM StringParameter to store the pipeline plugins configuration
-           from PipelineVars, for later retrieval.
+        5. Create an SSM StringParameter to store the ConfigurationVars as a string,
+           for later retrieval.
 
         6. Validates the stack against the AWS Solutions checklist using Aspects.
         """
 
         super().__init__(scope, construct_id, env=env, **kwargs)
         config_vars = ConfigurationVars(**props)
-        props_env = load_properties(stage=config_vars.stage)
 
-        config_vars = ConfigurationVars(**props_env)
+        props_env = load_properties(stage=config_vars.stage)
+        ssm_parameter_value = reduce_items_number(values=props_env)
 
         ssm.StringParameter(
             self,
-            id="pipeline_plugins",
-            string_value=str(config_vars.plugins),
-            parameter_name=f"/{config_vars.project}/{config_vars.stage}/pipeline_plugins",
+            id="config_file",
+            string_value=str(ssm_parameter_value),
+            parameter_name=f"/{config_vars.project}/{config_vars.stage}/services/tests/config",
+            tier=set_ssm_parameter_tier_type(character_number=len(str(ssm_parameter_value))),
         )
 
         Aspects.of(self).add(AwsSolutionsChecks(log_ignores=True))
```

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stages/code_quality_stage.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/code_quality_stage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""The CI/CD stage - implements jobs to validate code quality.
-"""
+"""The CI/CD stage - implements jobs to validate code quality."""
 
 import aws_cdk as cdk
 
 from cdk_opinionated_constructs.stacks.code_quality_stack import CodeQualityStack
 from constructs import Construct
```

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stages/infrastructure_tests_stage.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/infrastructure_tests_stage.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stages/integration_tests_stage.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/integration_tests_stage.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stages/notifications_stage.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/notifications_stage.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/stages/plugins_stage.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/plugins_stage.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/utils/__init__.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs/wafv2.py` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/wafv2.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs.egg-info/PKG-INFO` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-opinionated-constructs
-Version: 3.6.9
+Version: 3.7.0
 Summary: AWS CDK constructs come without added security configurations.
 License: MIT
 Requires-Python: >=3.11
 License-File: LICENSE
 Requires-Dist: aws-cdk-lib>=2.98.0
 Requires-Dist: constructs>=10.2.69
 Requires-Dist: cdk-monitoring-constructs>=6.0.0
```

### Comparing `cdk-opinionated-constructs-3.6.9/cdk_opinionated_constructs.egg-info/SOURCES.txt` & `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 ./cdk_opinionated_constructs/stacks/code_quality_stack.py
 ./cdk_opinionated_constructs/stacks/governance_stack.py
 ./cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py
 ./cdk_opinionated_constructs/stacks/integration_tests_stack.py
 ./cdk_opinionated_constructs/stacks/notifications_stack.py
 ./cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py
 ./cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py
+./cdk_opinionated_constructs/stacks/services_tests_stack.py
 ./cdk_opinionated_constructs/stages/__init__.py
 ./cdk_opinionated_constructs/stages/code_quality_stage.py
 ./cdk_opinionated_constructs/stages/infrastructure_tests_stage.py
 ./cdk_opinionated_constructs/stages/integration_tests_stage.py
 ./cdk_opinionated_constructs/stages/notifications_stage.py
 ./cdk_opinionated_constructs/stages/plugins_stage.py
+./cdk_opinionated_constructs/stages/services_tests_stage.py
 ./cdk_opinionated_constructs/utils/__init__.py
 ./test/__init__.py
 ./test/app.py
 ./test/infrastucture/__init__.py
 ./test/infrastucture/test_alb_stack.py
 ./test/infrastucture/test_ecr_stack.py
 ./test/infrastucture/test_lmb_stack.py
```

### Comparing `cdk-opinionated-constructs-3.6.9/setup.cfg` & `cdk-opinionated-constructs-3.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/setup.py` & `cdk-opinionated-constructs-3.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 https://packaging.python.org/en/latest/distributing.html
 """
 
 from setuptools import find_packages, setup
 
 setup(
     name="cdk-opinionated-constructs",
-    version="3.6.9",
+    version="3.7.0",
     description="AWS CDK constructs come without added security configurations.",
     long_description="The idea behind this project is to create secured constructs from the start. \n"
     "Supported constructs: ALB, ECR, LMB, NLB, S3, SNS, WAF, RDS",
     license="MIT",
     package_dir={"": "."},
     packages=find_packages(where="."),
     install_requires=[
```

### Comparing `cdk-opinionated-constructs-3.6.9/test/app.py` & `cdk-opinionated-constructs-3.7.0/test/app.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/infrastucture/test_alb_stack.py` & `cdk-opinionated-constructs-3.7.0/test/infrastucture/test_alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/infrastucture/test_ecr_stack.py` & `cdk-opinionated-constructs-3.7.0/test/infrastucture/test_ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/infrastucture/test_lmb_stack.py` & `cdk-opinionated-constructs-3.7.0/test/infrastucture/test_lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/infrastucture/test_s3_stack.py` & `cdk-opinionated-constructs-3.7.0/test/infrastucture/test_s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/infrastucture/test_sns_stack.py` & `cdk-opinionated-constructs-3.7.0/test/infrastucture/test_sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/infrastucture/test_wafv2_stack.py` & `cdk-opinionated-constructs-3.7.0/test/infrastucture/test_wafv2_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/stacks/alb_stack.py` & `cdk-opinionated-constructs-3.7.0/test/stacks/alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/stacks/ecr_stack.py` & `cdk-opinionated-constructs-3.7.0/test/stacks/ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/stacks/lmb_docker_stack.py` & `cdk-opinionated-constructs-3.7.0/test/stacks/lmb_docker_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/stacks/lmb_monitoring_stack.py` & `cdk-opinionated-constructs-3.7.0/test/stacks/lmb_monitoring_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/stacks/lmb_stack.py` & `cdk-opinionated-constructs-3.7.0/test/stacks/lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/stacks/nlb_stack.py` & `cdk-opinionated-constructs-3.7.0/test/stacks/nlb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/stacks/rds_mysql_stack.py` & `cdk-opinionated-constructs-3.7.0/test/stacks/rds_mysql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/stacks/rds_postgresql_stack.py` & `cdk-opinionated-constructs-3.7.0/test/stacks/rds_postgresql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/stacks/s3_stack.py` & `cdk-opinionated-constructs-3.7.0/test/stacks/s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/stacks/sns_stack.py` & `cdk-opinionated-constructs-3.7.0/test/stacks/sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.6.9/test/stacks/wafv2_stack.py` & `cdk-opinionated-constructs-3.7.0/test/stacks/wafv2_stack.py`

 * *Files identical despite different names*

