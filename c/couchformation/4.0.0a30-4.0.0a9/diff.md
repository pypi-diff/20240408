# Comparing `tmp/couchformation-4.0.0a30.tar.gz` & `tmp/couchformation-4.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchformation-4.0.0a30.tar", last modified: Mon Apr  8 03:58:21 2024, max compression
+gzip compressed data, was "couchformation-4.0.0a9.tar", last modified: Thu Sep 21 21:03:08 2023, max compression
```

## Comparing `couchformation-4.0.0a30.tar` & `couchformation-4.0.0a9.tar`

### file list

```diff
@@ -1,161 +1,23 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:21.025425 couchformation-4.0.0a30/
--rw-r--r--   0 michael    (501) staff       (20)      491 2024-03-29 03:30:35.000000 couchformation-4.0.0a30/.bumpversion.cfg
--rw-r--r--   0 michael    (501) staff       (20)     3163 2024-02-12 23:24:52.000000 couchformation-4.0.0a30/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)    10141 2024-01-11 14:36:20.000000 couchformation-4.0.0a30/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     2375 2024-03-29 00:27:40.000000 couchformation-4.0.0a30/Makefile
--rw-r--r--   0 michael    (501) staff       (20)     9983 2024-04-08 03:58:21.025130 couchformation-4.0.0a30/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     9165 2024-03-29 03:30:35.000000 couchformation-4.0.0a30/README.md
--rw-r--r--   0 michael    (501) staff       (20)        8 2024-03-29 03:30:35.000000 couchformation-4.0.0a30/VERSION
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:20.984657 couchformation-4.0.0a30/couchformation/
--rw-r--r--   0 michael    (501) staff       (20)      225 2024-03-29 03:30:35.000000 couchformation-4.0.0a30/couchformation/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:20.987109 couchformation-4.0.0a30/couchformation/aws/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-08-28 18:45:45.000000 couchformation-4.0.0a30/couchformation/aws/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:20.991354 couchformation-4.0.0a30/couchformation/aws/driver/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-08-28 19:47:21.000000 couchformation-4.0.0a30/couchformation/aws/driver/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    10058 2024-03-26 15:13:30.000000 couchformation-4.0.0a30/couchformation/aws/driver/base.py
--rw-r--r--   0 michael    (501) staff       (20)     7861 2024-01-23 15:33:47.000000 couchformation-4.0.0a30/couchformation/aws/driver/constants.py
--rw-r--r--   0 michael    (501) staff       (20)     1273 2024-03-29 20:44:13.000000 couchformation-4.0.0a30/couchformation/aws/driver/cost.py
--rw-r--r--   0 michael    (501) staff       (20)     5124 2024-03-20 23:16:52.000000 couchformation-4.0.0a30/couchformation/aws/driver/dns.py
--rw-r--r--   0 michael    (501) staff       (20)     3330 2024-01-26 00:52:29.000000 couchformation-4.0.0a30/couchformation/aws/driver/gateway.py
--rw-r--r--   0 michael    (501) staff       (20)     7172 2024-01-23 01:13:01.000000 couchformation-4.0.0a30/couchformation/aws/driver/image.py
--rw-r--r--   0 michael    (501) staff       (20)     9221 2024-02-23 15:28:26.000000 couchformation-4.0.0a30/couchformation/aws/driver/instance.py
--rw-r--r--   0 michael    (501) staff       (20)     4695 2024-01-11 22:50:25.000000 couchformation-4.0.0a30/couchformation/aws/driver/machine.py
--rw-r--r--   0 michael    (501) staff       (20)     7301 2024-03-26 01:22:35.000000 couchformation-4.0.0a30/couchformation/aws/driver/network.py
--rw-r--r--   0 michael    (501) staff       (20)     4776 2024-01-26 01:15:08.000000 couchformation-4.0.0a30/couchformation/aws/driver/nsg.py
--rw-r--r--   0 michael    (501) staff       (20)     3932 2024-01-26 01:53:31.000000 couchformation-4.0.0a30/couchformation/aws/driver/route.py
--rw-r--r--   0 michael    (501) staff       (20)     4160 2024-01-26 01:15:08.000000 couchformation-4.0.0a30/couchformation/aws/driver/sshkey.py
--rw-r--r--   0 michael    (501) staff       (20)    15479 2024-03-26 01:27:00.000000 couchformation-4.0.0a30/couchformation/aws/network.py
--rw-r--r--   0 michael    (501) staff       (20)    10825 2024-03-27 17:10:47.000000 couchformation-4.0.0a30/couchformation/aws/node.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:20.992380 couchformation-4.0.0a30/couchformation/azure/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-09-12 19:20:27.000000 couchformation-4.0.0a30/couchformation/azure/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:20.996076 couchformation-4.0.0a30/couchformation/azure/driver/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-09-12 21:22:11.000000 couchformation-4.0.0a30/couchformation/azure/driver/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    10245 2024-03-25 15:27:42.000000 couchformation-4.0.0a30/couchformation/azure/driver/base.py
--rw-r--r--   0 michael    (501) staff       (20)     4854 2024-01-23 17:40:35.000000 couchformation-4.0.0a30/couchformation/azure/driver/constants.py
--rw-r--r--   0 michael    (501) staff       (20)     2281 2024-01-25 20:31:12.000000 couchformation-4.0.0a30/couchformation/azure/driver/disk.py
--rw-r--r--   0 michael    (501) staff       (20)     6199 2024-03-25 17:58:42.000000 couchformation-4.0.0a30/couchformation/azure/driver/dns.py
--rw-r--r--   0 michael    (501) staff       (20)     6206 2023-09-13 03:19:44.000000 couchformation-4.0.0a30/couchformation/azure/driver/image.py
--rw-r--r--   0 michael    (501) staff       (20)     6429 2024-02-16 19:11:45.000000 couchformation-4.0.0a30/couchformation/azure/driver/instance.py
--rw-r--r--   0 michael    (501) staff       (20)     4479 2024-01-23 18:00:01.000000 couchformation-4.0.0a30/couchformation/azure/driver/machine.py
--rw-r--r--   0 michael    (501) staff       (20)    13434 2024-01-25 22:04:22.000000 couchformation-4.0.0a30/couchformation/azure/driver/network.py
--rw-r--r--   0 michael    (501) staff       (20)     7464 2024-03-25 19:42:32.000000 couchformation-4.0.0a30/couchformation/azure/driver/private_dns.py
--rw-r--r--   0 michael    (501) staff       (20)    16243 2024-03-25 21:59:41.000000 couchformation-4.0.0a30/couchformation/azure/network.py
--rw-r--r--   0 michael    (501) staff       (20)    13421 2024-03-27 17:10:47.000000 couchformation-4.0.0a30/couchformation/azure/node.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:20.996542 couchformation-4.0.0a30/couchformation/capella/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:20.997991 couchformation-4.0.0a30/couchformation/capella/driver/
--rw-r--r--   0 michael    (501) staff       (20)     1183 2024-03-27 22:44:27.000000 couchformation-4.0.0a30/couchformation/capella/driver/base.py
--rw-r--r--   0 michael    (501) staff       (20)     3377 2024-03-27 21:54:02.000000 couchformation-4.0.0a30/couchformation/capella/driver/cb_bucket.py
--rw-r--r--   0 michael    (501) staff       (20)    27196 2024-03-27 22:06:19.000000 couchformation-4.0.0a30/couchformation/capella/driver/cb_capella.py
--rw-r--r--   0 michael    (501) staff       (20)     4456 2024-03-27 21:55:34.000000 couchformation-4.0.0a30/couchformation/capella/driver/cb_capella_config.py
--rw-r--r--   0 michael    (501) staff       (20)    11883 2024-03-27 22:44:27.000000 couchformation-4.0.0a30/couchformation/capella/node.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:20.998968 couchformation-4.0.0a30/couchformation/cli/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-11-02 01:40:10.000000 couchformation-4.0.0a30/couchformation/cli/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     5652 2024-03-27 14:55:23.000000 couchformation-4.0.0a30/couchformation/cli/cli.py
--rw-r--r--   0 michael    (501) staff       (20)     4284 2024-04-05 14:08:14.000000 couchformation-4.0.0a30/couchformation/cli/cloudmgr.py
--rw-r--r--   0 michael    (501) staff       (20)      981 2024-01-02 15:31:29.000000 couchformation-4.0.0a30/couchformation/cli/dbdump.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:20.975338 couchformation-4.0.0a30/couchformation/common/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:20.999244 couchformation-4.0.0a30/couchformation/common/config/
--rw-r--r--   0 michael    (501) staff       (20)    13795 2023-09-11 22:16:04.000000 couchformation-4.0.0a30/couchformation/common/config/resources.py
--rw-r--r--   0 michael    (501) staff       (20)    10343 2024-01-23 22:55:05.000000 couchformation-4.0.0a30/couchformation/config.py
--rw-r--r--   0 michael    (501) staff       (20)     5893 2024-03-26 16:18:37.000000 couchformation-4.0.0a30/couchformation/constants.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:21.001857 couchformation-4.0.0a30/couchformation/data/
--rw-r--r--   0 michael    (501) staff       (20)      579 2024-03-27 15:39:49.000000 couchformation-4.0.0a30/couchformation/data/build_profiles.yaml
--rw-r--r--   0 michael    (501) staff       (20)      146 2024-02-09 18:58:57.000000 couchformation-4.0.0a30/couchformation/data/cloud_profiles.yaml
--rw-r--r--   0 michael    (501) staff       (20)      377 2023-11-17 19:22:36.000000 couchformation-4.0.0a30/couchformation/data/container_profiles.yaml
--rw-r--r--   0 michael    (501) staff       (20)     1368 2024-03-15 19:33:16.000000 couchformation-4.0.0a30/couchformation/data/node_profiles.yaml
--rw-r--r--   0 michael    (501) staff       (20)     1305 2024-03-27 17:20:55.000000 couchformation-4.0.0a30/couchformation/data/provisioner_profiles.yaml
--rw-r--r--   0 michael    (501) staff       (20)      128 2024-01-05 17:37:26.000000 couchformation-4.0.0a30/couchformation/data/strategy_profiles.yaml
--rw-r--r--   0 michael    (501) staff       (20)     3576 2024-03-28 15:45:57.000000 couchformation-4.0.0a30/couchformation/data/target_profiles.yaml
--rw-r--r--   0 michael    (501) staff       (20)    17597 2024-04-07 23:43:21.000000 couchformation-4.0.0a30/couchformation/deployment.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:21.003045 couchformation-4.0.0a30/couchformation/docker/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-11-17 14:45:37.000000 couchformation-4.0.0a30/couchformation/docker/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:21.004768 couchformation-4.0.0a30/couchformation/docker/driver/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-11-17 14:45:24.000000 couchformation-4.0.0a30/couchformation/docker/driver/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     1341 2023-11-17 18:12:08.000000 couchformation-4.0.0a30/couchformation/docker/driver/base.py
--rw-r--r--   0 michael    (501) staff       (20)      231 2023-11-20 17:51:38.000000 couchformation-4.0.0a30/couchformation/docker/driver/constants.py
--rw-r--r--   0 michael    (501) staff       (20)     8613 2024-03-28 14:14:47.000000 couchformation-4.0.0a30/couchformation/docker/driver/container.py
--rw-r--r--   0 michael    (501) staff       (20)     2658 2023-11-20 17:57:39.000000 couchformation-4.0.0a30/couchformation/docker/driver/network.py
--rw-r--r--   0 michael    (501) staff       (20)     3548 2024-03-28 14:02:55.000000 couchformation-4.0.0a30/couchformation/docker/network.py
--rw-r--r--   0 michael    (501) staff       (20)     3407 2024-03-28 14:20:43.000000 couchformation-4.0.0a30/couchformation/docker/node.py
--rw-r--r--   0 michael    (501) staff       (20)     2111 2023-11-17 15:24:25.000000 couchformation-4.0.0a30/couchformation/docker/util.py
--rw-r--r--   0 michael    (501) staff       (20)     2790 2024-03-26 18:46:14.000000 couchformation-4.0.0a30/couchformation/exception.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:21.005215 couchformation-4.0.0a30/couchformation/exec/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-08-29 15:42:02.000000 couchformation-4.0.0a30/couchformation/exec/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      876 2024-01-10 21:47:39.000000 couchformation-4.0.0a30/couchformation/exec/process.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:21.006734 couchformation-4.0.0a30/couchformation/executor/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-11-02 01:40:35.000000 couchformation-4.0.0a30/couchformation/executor/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     1103 2024-01-12 20:49:32.000000 couchformation-4.0.0a30/couchformation/executor/dispatch.py
--rw-r--r--   0 michael    (501) staff       (20)    10821 2024-03-14 23:07:37.000000 couchformation-4.0.0a30/couchformation/executor/targets.py
--rw-r--r--   0 michael    (501) staff       (20)      521 2023-10-17 14:42:59.000000 couchformation-4.0.0a30/couchformation/executor/taskqueue.py
--rw-r--r--   0 michael    (501) staff       (20)      598 2024-01-02 17:20:41.000000 couchformation-4.0.0a30/couchformation/executor/worker.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:21.007588 couchformation-4.0.0a30/couchformation/gcp/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-09-08 13:45:36.000000 couchformation-4.0.0a30/couchformation/gcp/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:21.011055 couchformation-4.0.0a30/couchformation/gcp/driver/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-09-08 17:48:51.000000 couchformation-4.0.0a30/couchformation/gcp/driver/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     6655 2024-03-21 21:04:45.000000 couchformation-4.0.0a30/couchformation/gcp/driver/base.py
--rw-r--r--   0 michael    (501) staff       (20)     3333 2024-01-23 22:39:02.000000 couchformation-4.0.0a30/couchformation/gcp/driver/constants.py
--rw-r--r--   0 michael    (501) staff       (20)     3413 2024-01-25 19:10:07.000000 couchformation-4.0.0a30/couchformation/gcp/driver/disk.py
--rw-r--r--   0 michael    (501) staff       (20)     5601 2024-03-25 22:34:34.000000 couchformation-4.0.0a30/couchformation/gcp/driver/dns.py
--rw-r--r--   0 michael    (501) staff       (20)     3646 2024-01-25 19:25:09.000000 couchformation-4.0.0a30/couchformation/gcp/driver/firewall.py
--rw-r--r--   0 michael    (501) staff       (20)     5103 2023-09-18 22:46:09.000000 couchformation-4.0.0a30/couchformation/gcp/driver/image.py
--rw-r--r--   0 michael    (501) staff       (20)     7694 2024-01-25 16:25:38.000000 couchformation-4.0.0a30/couchformation/gcp/driver/instance.py
--rw-r--r--   0 michael    (501) staff       (20)     3332 2023-09-12 13:04:14.000000 couchformation-4.0.0a30/couchformation/gcp/driver/machine.py
--rw-r--r--   0 michael    (501) staff       (20)     8628 2024-03-25 22:26:58.000000 couchformation-4.0.0a30/couchformation/gcp/driver/network.py
--rw-r--r--   0 michael    (501) staff       (20)    14706 2024-03-25 23:46:01.000000 couchformation-4.0.0a30/couchformation/gcp/network.py
--rw-r--r--   0 michael    (501) staff       (20)    10527 2024-03-27 17:10:47.000000 couchformation-4.0.0a30/couchformation/gcp/node.py
--rw-r--r--   0 michael    (501) staff       (20)     8410 2024-01-26 20:29:03.000000 couchformation-4.0.0a30/couchformation/kvdb.py
--rw-r--r--   0 michael    (501) staff       (20)     1988 2023-11-20 20:32:05.000000 couchformation-4.0.0a30/couchformation/network.py
--rw-r--r--   0 michael    (501) staff       (20)      331 2023-11-03 17:19:30.000000 couchformation-4.0.0a30/couchformation/null.py
--rw-r--r--   0 michael    (501) staff       (20)    16828 2024-04-05 15:47:40.000000 couchformation-4.0.0a30/couchformation/project.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:21.014107 couchformation-4.0.0a30/couchformation/provisioner/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-08-30 23:18:42.000000 couchformation-4.0.0a30/couchformation/provisioner/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     4105 2024-03-08 23:32:28.000000 couchformation-4.0.0a30/couchformation/provisioner/docker.py
--rw-r--r--   0 michael    (501) staff       (20)      318 2023-10-12 04:30:47.000000 couchformation-4.0.0a30/couchformation/provisioner/provisioners.py
--rw-r--r--   0 michael    (501) staff       (20)     8318 2024-03-27 17:20:55.000000 couchformation-4.0.0a30/couchformation/provisioner/remote.py
--rw-r--r--   0 michael    (501) staff       (20)     3348 2024-03-08 22:22:58.000000 couchformation-4.0.0a30/couchformation/provisioner/sftp.py
--rw-r--r--   0 michael    (501) staff       (20)     1837 2024-03-27 22:14:27.000000 couchformation-4.0.0a30/couchformation/provisioner/shell.py
--rw-r--r--   0 michael    (501) staff       (20)     5671 2023-10-31 20:40:58.000000 couchformation-4.0.0a30/couchformation/provisioner/ssh.py
--rw-r--r--   0 michael    (501) staff       (20)     5879 2024-03-27 17:20:55.000000 couchformation-4.0.0a30/couchformation/provisioner/winrm.py
--rw-r--r--   0 michael    (501) staff       (20)    11611 2024-03-27 22:06:19.000000 couchformation-4.0.0a30/couchformation/restmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2833 2023-11-01 22:24:12.000000 couchformation-4.0.0a30/couchformation/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7976 2024-01-13 00:02:33.000000 couchformation-4.0.0a30/couchformation/ssh.py
--rw-r--r--   0 michael    (501) staff       (20)    11449 2023-09-21 20:33:18.000000 couchformation-4.0.0a30/couchformation/state.py
--rw-r--r--   0 michael    (501) staff       (20)     3622 2024-04-05 15:43:22.000000 couchformation-4.0.0a30/couchformation/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:20.986311 couchformation-4.0.0a30/couchformation.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     9983 2024-04-08 03:58:20.000000 couchformation-4.0.0a30/couchformation.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     4156 2024-04-08 03:58:20.000000 couchformation-4.0.0a30/couchformation.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2024-04-08 03:58:20.000000 couchformation-4.0.0a30/couchformation.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      102 2024-04-08 03:58:20.000000 couchformation-4.0.0a30/couchformation.egg-info/entry_points.txt
--rw-r--r--   0 michael    (501) staff       (20)     1031 2024-04-08 03:58:20.000000 couchformation-4.0.0a30/couchformation.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       15 2024-04-08 03:58:20.000000 couchformation-4.0.0a30/couchformation.egg-info/top_level.txt
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:21.016235 couchformation-4.0.0a30/doc/
--rw-r--r--   0 michael    (501) staff       (20)    81887 2023-09-12 17:56:25.000000 couchformation-4.0.0a30/doc/couch-formation-1.png
--rw-r--r--   0 michael    (501) staff       (20)     1031 2024-03-28 13:43:10.000000 couchformation-4.0.0a30/requirements.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2024-04-08 03:58:21.025480 couchformation-4.0.0a30/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     2986 2024-03-29 00:49:30.000000 couchformation-4.0.0a30/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-08 03:58:21.024657 couchformation-4.0.0a30/tests/
--rw-r--r--   0 michael    (501) staff       (20)        0 2024-01-23 23:49:17.000000 couchformation-4.0.0a30/tests/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     8776 2024-03-28 23:59:52.000000 couchformation-4.0.0a30/tests/common.py
--rw-r--r--   0 michael    (501) staff       (20)     3127 2024-02-13 15:41:33.000000 couchformation-4.0.0a30/tests/conftest.py
--rw-r--r--   0 michael    (501) staff       (20)     2302 2024-03-21 19:20:38.000000 couchformation-4.0.0a30/tests/interactive.py
--rw-r--r--   0 michael    (501) staff       (20)       98 2024-02-12 21:05:50.000000 couchformation-4.0.0a30/tests/pytest.ini
--rwxr-xr-x   0 michael    (501) staff       (20)     5666 2024-01-26 20:52:37.000000 couchformation-4.0.0a30/tests/test_1.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3910 2024-03-29 00:27:40.000000 couchformation-4.0.0a30/tests/test_10.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3870 2024-03-29 00:27:40.000000 couchformation-4.0.0a30/tests/test_11.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3876 2024-03-29 00:27:40.000000 couchformation-4.0.0a30/tests/test_12.py
--rwxr-xr-x   0 michael    (501) staff       (20)     7170 2024-01-26 21:12:49.000000 couchformation-4.0.0a30/tests/test_2.py
--rwxr-xr-x   0 michael    (501) staff       (20)     7913 2024-01-26 21:34:43.000000 couchformation-4.0.0a30/tests/test_3.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3574 2024-03-26 18:55:59.000000 couchformation-4.0.0a30/tests/test_4.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3534 2024-03-26 18:55:59.000000 couchformation-4.0.0a30/tests/test_5.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3540 2024-03-26 18:55:59.000000 couchformation-4.0.0a30/tests/test_6.py
--rwxr-xr-x   0 michael    (501) staff       (20)     4016 2024-03-26 21:24:59.000000 couchformation-4.0.0a30/tests/test_7.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3377 2024-01-25 00:38:30.000000 couchformation-4.0.0a30/tests/test_8.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3072 2024-01-25 00:38:30.000000 couchformation-4.0.0a30/tests/test_9.py
--rwxr-xr-x   0 michael    (501) staff       (20)     6397 2023-09-21 13:21:37.000000 couchformation-4.0.0a30/tests/test_aws_m.py
--rwxr-xr-x   0 michael    (501) staff       (20)     8602 2023-09-21 13:21:37.000000 couchformation-4.0.0a30/tests/test_azure_m.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3248 2024-03-27 22:36:32.000000 couchformation-4.0.0a30/tests/test_c.py
--rwxr-xr-x   0 michael    (501) staff       (20)      358 2023-09-12 13:04:14.000000 couchformation-4.0.0a30/tests/test_cli.py
--rwxr-xr-x   0 michael    (501) staff       (20)      356 2023-10-31 20:40:58.000000 couchformation-4.0.0a30/tests/test_db.py
--rwxr-xr-x   0 michael    (501) staff       (20)     8112 2023-09-21 13:21:37.000000 couchformation-4.0.0a30/tests/test_gcp_m.py
--rwxr-xr-x   0 michael    (501) staff       (20)      345 2024-03-21 19:17:15.000000 couchformation-4.0.0a30/tests/test_interactive.py
--rw-r--r--   0 michael    (501) staff       (20)     5311 2023-10-18 21:57:15.000000 couchformation-4.0.0a30/tests/test_kvdb.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-09-21 21:03:08.071573 couchformation-4.0.0a9/
+-rw-r--r--   0 michael    (501) staff       (20)     1833 2023-09-21 21:03:08.071310 couchformation-4.0.0a9/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1042 2023-09-21 21:02:26.000000 couchformation-4.0.0a9/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-09-21 21:03:07.967487 couchformation-4.0.0a9/couchformation/
+-rw-r--r--   0 michael    (501) staff       (20)      163 2023-09-21 21:02:26.000000 couchformation-4.0.0a9/couchformation/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    10098 2023-09-21 19:18:19.000000 couchformation-4.0.0a9/couchformation/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4922 2023-09-21 20:36:45.000000 couchformation-4.0.0a9/couchformation/constants.py
+-rw-r--r--   0 michael    (501) staff       (20)     4156 2023-09-21 18:42:19.000000 couchformation-4.0.0a9/couchformation/deployment.py
+-rw-r--r--   0 michael    (501) staff       (20)     1126 2023-09-15 15:04:28.000000 couchformation-4.0.0a9/couchformation/exception.py
+-rw-r--r--   0 michael    (501) staff       (20)     1596 2023-09-15 17:26:25.000000 couchformation-4.0.0a9/couchformation/network.py
+-rw-r--r--   0 michael    (501) staff       (20)     3027 2023-09-21 19:28:39.000000 couchformation-4.0.0a9/couchformation/project.py
+-rw-r--r--   0 michael    (501) staff       (20)     6591 2023-09-12 13:04:14.000000 couchformation-4.0.0a9/couchformation/ssh.py
+-rw-r--r--   0 michael    (501) staff       (20)    11449 2023-09-21 20:33:18.000000 couchformation-4.0.0a9/couchformation/state.py
+-rw-r--r--   0 michael    (501) staff       (20)     1720 2023-09-12 13:04:14.000000 couchformation-4.0.0a9/couchformation/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-09-21 21:03:08.069792 couchformation-4.0.0a9/couchformation.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1833 2023-09-21 21:03:07.000000 couchformation-4.0.0a9/couchformation.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      506 2023-09-21 21:03:07.000000 couchformation-4.0.0a9/couchformation.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-09-21 21:03:07.000000 couchformation-4.0.0a9/couchformation.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       62 2023-09-21 21:03:07.000000 couchformation-4.0.0a9/couchformation.egg-info/entry_points.txt
+-rw-r--r--   0 michael    (501) staff       (20)      824 2023-09-21 21:03:07.000000 couchformation-4.0.0a9/couchformation.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       15 2023-09-21 21:03:07.000000 couchformation-4.0.0a9/couchformation.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-09-21 21:03:08.071668 couchformation-4.0.0a9/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     2539 2023-09-12 13:14:30.000000 couchformation-4.0.0a9/setup.py
```

### Comparing `couchformation-4.0.0a30/couchformation/capella/node.py` & `couchformation-4.0.0a9/couchformation/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,261 +1,333 @@
 ##
 ##
 
-import logging
-from couchformation.exception import FatalError
-from couchformation.capella.driver.base import CloudBase
-from couchformation.config import get_state_file, get_state_dir
-from couchformation.kvdb import KeyValueStore
-from couchformation.util import FileManager, Synchronize
-from couchformation.capella.driver.cb_capella import Capella, CapellaCluster, AllowedCIDR, Credentials, AppService
+import os
+from typing import Optional, Union, List
+from enum import Enum
+import attr
+import argparse
 import couchformation.constants as C
-from couchformation.util import PasswordUtility
 
 
-logger = logging.getLogger('couchformation.capella.node')
-logger.addHandler(logging.NullHandler())
-
-
-class CapellaNodeError(FatalError):
-    pass
-
-
-class CapellaDeployment(object):
-
-    def __init__(self, parameters: dict):
-        self.parameters = parameters
-        self.name = parameters.get('name')
-        self.deploy_type = parameters.get('type') if parameters.get('type') else "database"
-        self.cluster_id = parameters.get('instance_id')
-        self.project = parameters.get('project')
-        self.region = parameters.get('region') if parameters.get('region') else "us-east-1"
-        self.cloud = parameters.get('cloud')
-        self.provider = parameters.get('provider') if parameters.get('provider') else "aws"
-        self.username = parameters.get('username') if parameters.get('username') else "Administrator"
-        self.password = parameters.get('password')
-        self.account_email = parameters.get('account_email')
-        self.profile = parameters.get('profile') if parameters.get('profile') else 'default'
-        self.sw_version = self.parameters.get('sw_version') if self.parameters.get('sw_version') else "latest"
-        self.cidr = parameters.get('cidr') if parameters.get('cidr') else "10.0.0.0/23"
-        self.allow = parameters.get('allow') if parameters.get('allow') else "0.0.0.0/0"
-        self.db_name = f"{self.name}-database"
-
-        self.state_file = get_state_file(self.project, self.name)
-        self.state_dir = get_state_dir(self.project, self.name)
-
-        with Synchronize(C.GLOBAL_LOCK):
-            try:
-                FileManager().make_dir(self.state_dir)
-            except Exception as err:
-                raise CapellaNodeError(f"can not create state dir: {err}")
-
-        document = self.db_name
-        self.state = KeyValueStore(self.state_file, document)
-
-        CloudBase(self.parameters).test_session()
-
-    def compose(self):
-        if self.deploy_type == "mobile":
-            self.compose_app_svc()
+def get_base_dir():
+    if 'COUCH_FORMATION_CONFIG_DIR' in os.environ:
+        return os.environ['COUCH_FORMATION_CONFIG_DIR']
+    else:
+        return C.STATE_DIRECTORY
+
+
+def get_log_dir():
+    if 'COUCH_FORMATION_LOG_DIR' in os.environ:
+        return os.environ['COUCH_FORMATION_LOG_DIR']
+    else:
+        return C.LOG_DIRECTORY
+
+
+def get_resource_dir(name: str, tag: str):
+    return os.path.join(get_base_dir(), name, tag)
+
+
+def get_project_dir(name: str):
+    return os.path.join(get_base_dir(), name)
+
+
+def str_to_int(value: Union[str, int]) -> int:
+    return int(value)
+
+
+class AuthMode(Enum):
+    default = 0
+    sso = 1
+
+
+class PathMode(Enum):
+    resource = 0
+    common = 1
+
+
+class ProvisionMode(Enum):
+    public = 0
+    private = 1
+
+
+@attr.s
+class Parameters:
+    project: Optional[str] = attr.ib(default=None)
+    cloud: Optional[str] = attr.ib(default=None)
+    name: Optional[str] = attr.ib(default=None)
+    model: Optional[str] = attr.ib(default=None)
+    region: Optional[str] = attr.ib(default=None)
+    ssh_key: Optional[str] = attr.ib(default=None)
+    os_id: Optional[str] = attr.ib(default=None)
+    os_version: Optional[str] = attr.ib(default=None)
+    auth_mode: Optional[str] = attr.ib(default=None)
+    profile: Optional[str] = attr.ib(default=None)
+    base_dir: Optional[str] = attr.ib(default=None)
+    private_ip: Optional[bool] = attr.ib(default=None)
+    path_mode: Optional[PathMode] = attr.ib(default=None)
+    machine_type: Optional[str] = attr.ib(default=None)
+    quantity: Optional[int] = attr.ib(default=None)
+    services: Optional[str] = attr.ib(default=None)
+    volume_iops: Optional[str] = attr.ib(default=None)
+    volume_size: Optional[str] = attr.ib(default=None)
+    volume_type: Optional[str] = attr.ib(default=None)
+    volume_tier: Optional[str] = attr.ib(default=None)
+    root_size: Optional[str] = attr.ib(default=None)
+    connect_svc: Optional[str] = attr.ib(default=None)
+    connect_ip: Optional[str] = attr.ib(default=None)
+
+    @classmethod
+    def create(cls, args):
+        c = cls()
+        c.initialize_args(args)
+        return c
+
+    def initialize_args(self, args):
+        parser = argparse.ArgumentParser(add_help=False)
+        for attribute in self.__annotations__:
+            parser.add_argument(f"--{attribute}", action='store')
+        parameters, remainder = parser.parse_known_args(args)
+        self.from_namespace(parameters)
+
+    def from_namespace(self, namespace: argparse.Namespace):
+        args = vars(namespace)
+        for attribute in self.__annotations__:
+            if args.get(attribute):
+                setattr(self, attribute, args.get(attribute))
+
+    def from_dict(self, options: dict):
+        for attribute in self.__annotations__:
+            if options.get(attribute):
+                setattr(self, attribute, options.get(attribute))
+
+    @property
+    def project_dir(self):
+        return get_project_dir(self.project)
+
+    @property
+    def as_dict(self):
+        return {k: self.__dict__[k] for k in self.__dict__ if self.__dict__[k] is not None}
+
+
+@attr.s
+class BaseConfig:
+    project: Optional[str] = attr.ib(default="resources")
+    ssh_key: Optional[str] = attr.ib(default=os.path.join(os.environ['HOME'], '.ssh', 'couch-formation-key.pem'))
+    base_dir: Optional[str] = attr.ib(default=get_base_dir())
+    private_ip: Optional[bool] = attr.ib(default=False)
+
+    @classmethod
+    def create(cls, data: Union[list, dict]):
+        if type(data) == list:
+            c = cls()
+            c.initialize_args(data)
         else:
-            self.compose_database()
-
-    def compose_app_svc(self):
-        number = self.parameters.get('number') if self.parameters.get('number') else 1
-        document = f"{self.name}-node-group-{number:02d}"
-        group = KeyValueStore(self.state_file, document)
-
-        group['machine_type'] = self.parameters.get('machine_type')
-        group['quantity'] = self.parameters.get('quantity') if self.parameters.get('quantity') else 2
-
-    def compose_database(self):
-        number = self.parameters.get('number') if self.parameters.get('number') else 1
-        document = f"{self.name}-node-group-{number:02d}"
-        group = KeyValueStore(self.state_file, document)
-
-        group['cloud'] = self.parameters.get('provider')
-        group['machine_type'] = self.parameters.get('machine_type')
-        group['volume_size'] = self.parameters.get('volume_size') if self.parameters.get('volume_size') else "256"
-        group['quantity'] = self.parameters.get('quantity') if self.parameters.get('quantity') else 3
-        group['services'] = self.parameters.get('services') if self.parameters.get('services') else "data,index,query"
-
-    def deploy(self):
-        if self.deploy_type == "mobile":
-            self.deploy_app_svc()
+            c = cls()
+            c.initialize_dict(data)
+        return c
+
+    def initialize_args(self, args):
+        parser = argparse.ArgumentParser(add_help=False)
+        for attribute in self.__annotations__:
+            parser.add_argument(f"--{attribute}", action='store')
+        parameters, remainder = parser.parse_known_args(args)
+        self.from_namespace(parameters)
+
+    def initialize_dict(self, options):
+        self.from_dict(options)
+
+    @property
+    def project_dir(self):
+        return get_project_dir(self.project)
+
+    def from_namespace(self, namespace: argparse.Namespace):
+        args = vars(namespace)
+        for attribute in self.__annotations__:
+            if args.get(attribute):
+                setattr(self, attribute, args.get(attribute))
+
+    def from_dict(self, options: dict):
+        for attribute in self.__annotations__:
+            if options.get(attribute):
+                setattr(self, attribute, options.get(attribute))
+
+    @property
+    def as_dict(self):
+        return self.__dict__
+
+
+@attr.s
+class NodeConfig:
+    machine_type: Optional[str] = attr.ib(default=None)
+    quantity: Optional[int] = attr.ib(default=1, converter=str_to_int)
+    services: Optional[str] = attr.ib(default="default")
+    volume_iops: Optional[str] = attr.ib(default="3000")
+    volume_size: Optional[str] = attr.ib(default="256")
+    volume_type: Optional[str] = attr.ib(default=None)
+    root_size: Optional[str] = attr.ib(default="256")
+
+    @classmethod
+    def create(cls, data: Union[list, dict]):
+        if type(data) == list:
+            c = cls()
+            c.initialize_args(data)
         else:
-            self.deploy_database()
-
-    def deploy_app_svc(self):
-        state_db = KeyValueStore(self.state_file)
-        node_groups = state_db.doc_id_startswith(f"{self.name}-node-group")
-
-        if len(node_groups) == 0:
-            raise CapellaNodeError("no node groups present")
-
-        if self.state.get('project_id'):
-            project_id = self.state.get('project_id')
+            c = cls()
+            c.initialize_dict(data)
+        return c
+
+    def initialize_args(self, args):
+        parser = argparse.ArgumentParser(add_help=False)
+        for attribute in self.__annotations__:
+            parser.add_argument(f"--{attribute}", action='store')
+        parameters, undefined = parser.parse_known_args(args)
+        self.from_namespace(parameters)
+
+    def initialize_dict(self, options):
+        self.from_dict(options)
+
+    def from_namespace(self, namespace: argparse.Namespace):
+        args = vars(namespace)
+        for attribute in self.__annotations__:
+            if args.get(attribute):
+                setattr(self, attribute, args.get(attribute))
+
+    def from_dict(self, options: dict):
+        for attribute in self.__annotations__:
+            if options.get(attribute):
+                setattr(self, attribute, options.get(attribute))
+
+    @property
+    def as_dict(self):
+        return self.__dict__
+
+
+@attr.s
+class DeploymentConfig:
+    core: Optional[BaseConfig] = attr.ib(default=BaseConfig())
+    config: Optional[List[NodeConfig]] = attr.ib(default=[])
+
+    def add_config(self, index: Union[str, int], config: NodeConfig):
+        index = int(index)
+        config.group = str(index)
+        if index > len(self.config) + 1:
+            raise ValueError(f"config index {index} out of range")
+        elif index == len(self.config) + 1:
+            self.config.append(config)
         else:
-            project_data = Capella(profile=self.profile).get_project(self.project)
-            if not project_data:
-                raise CapellaNodeError(f"Project {self.project} does not exist, please create a database for app service {self.name}")
-            else:
-                project_id = project_data.get('id')
-
-        self.state['project'] = self.project
-        self.state['type'] = self.deploy_type
-
-        if not self.cluster_id:
-            raise CapellaNodeError(f"Please connect the app service {self.name} to a Capella database")
-
-        self.state['instance_id'] = self.cluster_id
-
-        for group in node_groups:
-            group_db = KeyValueStore(self.state_file, group)
-
-            if self.state.get('app_svc_id'):
-                logger.info(f"App service {self.name} already exists")
-                app_svc_id = self.state['app_svc_id']
-            else:
-                quantity = int(group_db.get('quantity'))
-                machine = group_db.get('machine_type')
-                logger.info(f"Creating app service {self.name} with {quantity} {machine} nodes")
-                app_svc = AppService.create(self.name, "CouchFormation managed app service", quantity, machine, "3.0")
-
-                app_svc_id = Capella(project_id=project_id, profile=self.profile).create_app_svc(self.cluster_id, app_svc)
-                self.state['name'] = self.name
-                self.state['app_svc_id'] = app_svc_id
-                logger.info("Waiting for app service creation to complete")
-                if not Capella(project_id=project_id, profile=self.profile).wait_for_app_svc(self.cluster_id):
-                    raise CapellaNodeError("Timeout waiting for app service to deploy")
-
-            logger.info(f"App service ID: {app_svc_id}")
-
-        logger.info("Capella app service successfully created")
-
-        return self.state.as_dict
-
-    def deploy_database(self):
-        state_db = KeyValueStore(self.state_file)
-        node_groups = state_db.doc_id_startswith(f"{self.name}-node-group")
-
-        if len(node_groups) == 0:
-            raise CapellaNodeError("no node groups present")
-
-        cluster = CapellaCluster().create(self.name, "CouchFormation managed cluster", self.provider, self.region, self.cidr, version=self.sw_version)
-
-        for group in node_groups:
-            group_db = KeyValueStore(self.state_file, group)
-            cluster.add_service_group(group_db.get('cloud'),
-                                      group_db.get('machine_type'),
-                                      int(group_db.get('volume_size')),
-                                      int(group_db.get('quantity')),
-                                      group_db.get('services').split(','))
+            self.config[index - 1] = config
 
-        if self.state.get('project_id'):
-            project_id = self.state.get('project_id')
+    @classmethod
+    def new(cls, core: BaseConfig):
+        return cls(
+            core,
+            []
+        )
+
+    def reset(self, args):
+        self.config.clear()
+        self.core = BaseConfig().create(args)
+
+    @property
+    def length(self):
+        return len(self.config)
+
+    @property
+    def as_dict(self):
+        return self.__dict__
+
+
+@attr.s
+class NodeEntry:
+    name: Optional[str] = attr.ib(default=None)
+    username: Optional[str] = attr.ib(default=None)
+    private_ip: Optional[str] = attr.ib(default=None)
+    public_ip: Optional[str] = attr.ib(default=None)
+    use_private_ip: Optional[bool] = attr.ib(default=False)
+    availability_zone: Optional[str] = attr.ib(default=None)
+    services: Optional[str] = attr.ib(default=None)
+    connect_svc: Optional[str] = attr.ib(default=None)
+    connect_ip: Optional[str] = attr.ib(default=None)
+
+    @classmethod
+    def create(cls,
+               name: str,
+               username: str,
+               private_ip: str,
+               public_ip: str = None,
+               use_private_ip: bool = False,
+               zone: str = None,
+               services: str = "default",
+               connect_svc: str = None,
+               connect_ip: str = None
+               ):
+        return cls(
+            name,
+            username,
+            private_ip,
+            public_ip,
+            use_private_ip,
+            zone,
+            services,
+            connect_svc,
+            connect_ip
+        )
+
+
+@attr.s
+class NodeList:
+    username: Optional[str] = attr.ib(default=None)
+    ssh_key: Optional[str] = attr.ib(default=None)
+    nodes: Optional[List[NodeEntry]] = attr.ib(default=[])
+    working_dir: Optional[str] = attr.ib(default=None)
+    provision_ip: Optional[ProvisionMode] = attr.ib(default=ProvisionMode.public)
+
+    @classmethod
+    def create(cls, username: str, ssh_key: str, working_dir: str = None, use_private_ip: bool = False):
+        return cls(
+            username,
+            ssh_key,
+            [],
+            working_dir,
+            ProvisionMode(use_private_ip)
+        )
+
+    def add(self, name: str, private_ip: str, public_ip: str = None, zone: str = None, services: str = "default", connect_svc: str = None, connect_ip: str = None):
+        self.nodes.append(
+            NodeEntry.create(
+                name,
+                self.username,
+                private_ip,
+                public_ip,
+                bool(self.provision_ip.value),
+                zone,
+                services,
+                connect_svc,
+                connect_ip
+            )
+        )
+
+    @property
+    def node_list(self) -> List[NodeEntry]:
+        return self.nodes
+
+    def list_public_ip(self):
+        address_list = []
+        for entry in self.nodes:
+            address_list.append(entry.public_ip)
+        return address_list
+
+    def list_private_ip(self):
+        address_list = []
+        for entry in self.nodes:
+            address_list.append(entry.private_ip)
+        return address_list
+
+    def provision_list(self):
+        if self.provision_ip == ProvisionMode.public:
+            return self.list_public_ip()
         else:
-            project_data = Capella(profile=self.profile).get_project(self.project)
-            if not project_data:
-                logger.info(f"Creating project {self.project}")
-                project_id = Capella(profile=self.profile).create_project(self.project, self.account_email)
-                self.state['project_id'] = project_id
-            else:
-                project_id = project_data.get('id')
-
-        self.state['project'] = self.project
-        self.state['type'] = self.deploy_type
-
-        if self.state.get('instance_id'):
-            logger.info(f"Database {self.db_name} already exists")
-            cluster_id = self.state['instance_id']
-        else:
-            logger.info(f"Creating cluster {self.name}")
-            cluster_id = Capella(project_id=project_id, profile=self.profile).create_cluster(cluster)
-            self.state['instance_id'] = cluster_id
-            self.state['provider'] = self.provider
-            self.state['region'] = self.region
-            self.state['cidr'] = self.cidr
-            self.state['name'] = self.name
-            self.state['cloud'] = self.cloud
-            logger.info("Waiting for cluster creation to complete")
-            if not Capella(project_id=project_id, profile=self.profile).wait_for_cluster(self.name):
-                raise CapellaNodeError("Timeout waiting for cluster to deploy")
-
-        logger.info(f"Cluster ID: {cluster_id}")
-
-        cluster_info = Capella(project_id=project_id, profile=self.profile).get_cluster_by_id(cluster_id)
-        connect_string = cluster_info.get('connectionString')
-        self.state['connect_string'] = connect_string
-        logger.info(f"Connect string: {connect_string}")
-
-        if self.state.get('allow'):
-            logger.info(f"Allow list already set to {self.state.get('allow')}")
-        else:
-            allow_cidr = AllowedCIDR().create(self.allow)
-            logger.info(f"Configuring allowed CIDR {self.allow}")
-            Capella(project_id=project_id, profile=self.profile).allow_cidr(cluster_id, allow_cidr)
-            self.state['allow'] = self.allow
-
-        if self.state.get('username'):
-            logger.info(f"Database user {self.state.get('username')} already exists")
-        else:
-            if self.password:
-                password = self.password
-            else:
-                password = PasswordUtility().generate(16)
-                self.state['password'] = password
-                logger.info(f"Password: {password}")
-            credentials = Credentials().create(self.username, password)
-            logger.info(f"Creating database user {self.username}")
-            Capella(project_id=project_id, profile=self.profile).add_db_user(cluster_id, credentials)
-            self.state['username'] = self.username
-
-        logger.info("Capella database successfully created")
-
-        return self.state.as_dict
-
-    def destroy(self):
-        project = self.state.get('project')
-        if not project:
-            return
-        project_data = Capella(profile=self.profile).get_project(project)
-        project_id = project_data.get('id')
-        logger.info(f"Project {project} ID {project_id}")
-
-        if self.state.get('type') == "mobile":
-            self.destroy_app_svc(project_id)
-        else:
-            self.destroy_database(project, project_id)
-
-    def destroy_app_svc(self, project_id):
-        app_svc_name = self.state['name']
-        cluster_id = self.state['instance_id']
-
-        logger.info(f"Destroying app service {app_svc_name}")
-        Capella(project_id=project_id, profile=self.profile).delete_app_svc(cluster_id)
-        logger.info("Waiting for app service deletion to complete")
-        if not Capella(project_id=project_id, profile=self.profile).wait_for_app_svc_delete(cluster_id):
-            raise CapellaNodeError("Timeout waiting for app service deletion to complete")
-
-        self.state.clear()
-
-    def destroy_database(self, project, project_id):
-        cluster_name = self.state['name'] = self.name
-        logger.info(f"Destroying cluster {cluster_name}")
-        Capella(project_id=project_id, profile=self.profile).delete_cluster(cluster_name)
-        logger.info("Waiting for cluster deletion to complete")
-        if not Capella(project_id=project_id, profile=self.profile).wait_for_cluster_delete(cluster_name):
-            raise CapellaNodeError("Timeout waiting for cluster deletion to complete")
-
-        if self.state.get('project_id'):
-            cluster_list = Capella(project_id=project_id, profile=self.profile).list_clusters()
-            if len(cluster_list) == 0:
-                logger.info(f"Removing project {project}")
-                Capella(profile=self.profile).delete_project(project)
-            else:
-                logger.warning(f"Project {project} has active clusters, it will not be removed")
-
-        self.state.clear()
+            return self.list_private_ip()
 
-    def info(self):
-        return self.state.as_dict
+    def ip_csv_list(self):
+        return ','.join(self.list_private_ip())
```

### Comparing `couchformation-4.0.0a30/couchformation/constants.py` & `couchformation-4.0.0a9/couchformation/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,15 @@
 ##
 ##
 
-import multiprocessing
 import os
-from couchformation import get_data_dir
-from pathlib import Path
 
-GLOBAL_LOCK = multiprocessing.Lock()
-
-ROOT_DIRECTORY = os.path.join(Path.home(), '.config', 'couch-formation')
+ROOT_DIRECTORY = os.path.join(os.environ.get('HOME'), '.config', 'couch-formation')
 STATE_DIRECTORY = os.path.join(ROOT_DIRECTORY, 'state')
 LOG_DIRECTORY = os.path.join(ROOT_DIRECTORY, 'log')
-DATA_DIRECTORY = get_data_dir()
-NODE_PROFILES = os.path.join(DATA_DIRECTORY, "node_profiles.yaml")
-TARGET_PROFILES = os.path.join(DATA_DIRECTORY, "target_profiles.yaml")
-PROVISIONER_PROFILES = os.path.join(DATA_DIRECTORY, "provisioner_profiles.yaml")
-STRATEGY_PROFILES = os.path.join(DATA_DIRECTORY, "strategy_profiles.yaml")
-CONTAINER_PROFILES = os.path.join(DATA_DIRECTORY, "container_profiles.yaml")
-CLOUD_PROFILES = os.path.join(DATA_DIRECTORY, "cloud_profiles.yaml")
-BUILD_PROFILES = os.path.join(DATA_DIRECTORY, "build_profiles.yaml")
-PLAYBOOK_DIR = os.path.join(DATA_DIRECTORY, "playbooks")
-
-METADATA = "metadata.db"
-NETWORK = "network.db"
-STATE = "state.db"
-CREDENTIALS = "credentials.db"
 
 GREY_COLOR = "\x1b[38;20m"
 YELLOW_COLOR = "\x1b[33;20m"
 RED_COLOR = "\x1b[31;20m"
 BOLD_RED_COLOR = "\x1b[31;1m"
 GREEN_COLOR = "\x1b[32;20m"
 SCREEN_RESET = "\x1b[0m"
@@ -46,16 +27,14 @@
     'ol': ['8', '9'],
     'rocky': ['8', '9'],
     'fedora': ['34'],
     'sles': ['12', '15'],
     'opensuse-leap': ['15'],
     'ubuntu': ['20.04', '22.04'],
     'debian': ['10', '11'],
-    'windows': ['2019', '2022'],
-    'macos': ['13', '14'],
     'arch': []
 }
 
 MACHINE_TYPES = [
         {
             "name": "2x4",
             "cpu": 2,
@@ -78,19 +57,14 @@
         },
         {
             "name": "8x16",
             "cpu": 8,
             "memory": 16384
         },
         {
-            "name": "8x24",
-            "cpu": 8,
-            "memory": 24576
-        },
-        {
             "name": "8x32",
             "cpu": 8,
             "memory": 32768
         },
         {
             "name": "16x32",
             "cpu": 16,
```

### Comparing `couchformation-4.0.0a30/couchformation/network.py` & `couchformation-4.0.0a9/couchformation/network.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 ##
 ##
 
-import socket
 import ipaddress
 from ipaddress import IPv4Network
 import logging
 from typing import Union
 
 
 class NetworkDriver(object):
@@ -44,22 +43,7 @@
 
         if len(candidates) == 0:
             return None
 
         self.active_network = candidates[0]
         self.ip_space.append(self.active_network)
         return self.active_network.exploded
-
-
-class NetworkUtil(object):
-
-    @staticmethod
-    def local_ip_address():
-        try:
-            socket.setdefaulttimeout(2)
-            s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-            s.connect(("8.8.8.8", 80))
-            local_ip = s.getsockname()[0]
-            s.close()
-            return local_ip
-        except TimeoutError:
-            return None
```

### Comparing `couchformation-4.0.0a30/couchformation/ssh.py` & `couchformation-4.0.0a9/couchformation/ssh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 ##
 ##
 
 import logging
 import os
-import rsa
 from enum import Enum
 from typing import Union, List
 from Crypto.PublicKey import RSA
-from Crypto.Util.number import long_to_bytes
-from Crypto.Cipher import PKCS1_OAEP
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 import hashlib
 from cryptography.exceptions import UnsupportedAlgorithm
 from couchformation.exception import FatalError, NonFatalError
 
 logger = logging.getLogger('couchformation.ssh')
@@ -51,25 +48,14 @@
         for location in SSH_PATHS:
             for file_found in os.listdir(location):
                 if file_found == name or next((f"{name}{e.value}" for e in SSHExtensions if f"{name}{e.value}" == file_found), None):
                     return location + '/' + file_found
         return None
 
     @staticmethod
-    def decrypt_with_key(encrypted_data: bytes, key_file: str) -> str:
-        try:
-            with open(key_file, 'r') as file_handle:
-                blob = file_handle.read()
-                private_key = rsa.PrivateKey.load_pkcs1(blob.encode('latin-1'))
-                decrypted = rsa.decrypt(encrypted_data, private_key)
-                return decrypted.decode('utf-8')
-        except OSError as err:
-            raise SSHError(f"can not read key file {key_file}: {err}.")
-
-    @staticmethod
     def list_private_key_files() -> Union[List[dict], None]:
         dir_list = []
         key_file_list = []
 
         for location in SSH_PATHS:
             for file_name in os.listdir(location):
                 full_path = location + '/' + file_name
@@ -143,37 +129,14 @@
         prime_q = rsa_key.q
         private_key = RSA.construct((modulus, pub_exp_e, pri_exp_d, prime_p, prime_q))
         public_key = private_key.public_key().exportKey('OpenSSH')
         ssh_public_key = public_key.decode('utf-8')
         return ssh_public_key
 
     @staticmethod
-    def get_mod_exp(key_file: str):
-        if not os.path.isabs(key_file):
-            key_file = SSHUtil.ssh_key_absolute_path(key_file)
-        fh = open(key_file, 'r')
-        key_pem = fh.read()
-        fh.close()
-        rsa_key = RSA.importKey(key_pem)
-        modulus = long_to_bytes(rsa_key.n)
-        exponent = long_to_bytes(rsa_key.e)
-        return modulus, exponent
-
-    @staticmethod
-    def decrypt_with_rsa(encrypted_data: bytes, key_file: str):
-        if not os.path.isabs(key_file):
-            key_file = SSHUtil.ssh_key_absolute_path(key_file)
-        fh = open(key_file, 'r')
-        key_pem = fh.read()
-        fh.close()
-        rsa_key = RSA.importKey(key_pem)
-        cipher = PKCS1_OAEP.new(rsa_key)
-        return cipher.decrypt(encrypted_data)
-
-    @staticmethod
     def write_file(file_name: str, data: str) -> bool:
         try:
             file_handle = open(file_name, 'w')
             file_handle.write(data)
             file_handle.write("\n")
             file_handle.close()
             return True
```

### Comparing `couchformation-4.0.0a30/couchformation/state.py` & `couchformation-4.0.0a9/couchformation/state.py`

 * *Files identical despite different names*

### Comparing `couchformation-4.0.0a30/couchformation.egg-info/requires.txt` & `couchformation-4.0.0a9/couchformation.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,38 @@
 attrs==23.1.0
-boto3>=1.34.17
-botocore>=1.34.17
-cryptography>=42.0.5
+boto3==1.28.11
+botocore==1.31.11
+cryptography>=36.0.1
 dnspython>=2.1.0
 google-api-core>=2.4.0
 google-api-python-client>=2.34.0
 google-auth>=2.3.3
 google-auth-httplib2>=0.1.0
 googleapis-common-protos>=1.54.0
 google-cloud>=0.34.0
 google-cloud-compute>=1.6.1
 google-cloud-storage>=2.10.0
-google-cloud-dns>=0.35.0
 google-cloud-network-management>=1.5.4
-Jinja2>=3.0.0
+Jinja2>=3.0.3
 passlib>=1.7.4
-pycryptodome>=3.20.0
+pycryptodome>=3.12.0
 pytz>=2021.3
 pyvmomi>=8.0.0.1.1
 requests>=2.31.0
-urllib3>=1.26.16
+urllib3>=1.26.7
 azure-common>=1.1.28
 azure-core>=1.26.1
 azure-mgmt-resource>=22.0.0
 azure-identity>=1.12.0
 azure.mgmt.network>=22.2.0
 azure.mgmt.compute>=29.0.0
 azure-mgmt-core>=1.3.2
 azure.mgmt.storage>=21.0.0
-azure-mgmt-dns>=8.1.0
-azure-mgmt-privatedns>=1.1.0
 azure.mgmt.subscription>=3.1.1
 ply>=3.11
 pytest==7.4.0
 pytest-asyncio==0.21.1
 pytest-rerunfailures==12.0
 sqlite-utils~=3.11
-docker>=5.0.3
-paramiko>=3.4.0
+paramiko>=3.3.1
 overrides>=7.4.0
 bumpversion>=0.6.0
-PyYAML>=5.1
-rsa>=4.9
-pywinrm>=0.4.3
-aiohttp>=3.9.3
-python-certifi-win32>=1.6.1
-certifi>=2023.5.7
-pyhostprep>=1.0.10
```

### Comparing `couchformation-4.0.0a30/setup.py` & `couchformation-4.0.0a9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,90 +1,76 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 import couchformation
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='couchformation',
     version=couchformation.__version__,
-    packages=find_packages(exclude=['tests']),
+    packages=['couchformation'],
     url='https://github.com/mminichino/couch-formation-core',
     license='Apache License 2.0',
     author='Michael Minichino',
     python_requires='>=3.8',
     entry_points={
         'console_scripts': [
             'cloudmgr = couchformation.cli.cloudmgr:main',
-            'dbdump = couchformation.cli.dbdump:main'
         ]
     },
-    package_data={'couchformation': ['data/*']},
     install_requires=[
         "attrs==23.1.0",
-        "boto3>=1.34.17",
-        "botocore>=1.34.17",
-        "cryptography>=42.0.5",
+        "boto3==1.28.11",
+        "botocore==1.31.11",
+        "cryptography>=36.0.1",
         "dnspython>=2.1.0",
         "google-api-core>=2.4.0",
         "google-api-python-client>=2.34.0",
         "google-auth>=2.3.3",
         "google-auth-httplib2>=0.1.0",
         "googleapis-common-protos>=1.54.0",
         "google-cloud>=0.34.0",
         "google-cloud-compute>=1.6.1",
         "google-cloud-storage>=2.10.0",
-        "google-cloud-dns>=0.35.0",
         "google-cloud-network-management>=1.5.4",
-        "Jinja2>=3.0.0",
+        "Jinja2>=3.0.3",
         "passlib>=1.7.4",
-        "pycryptodome>=3.20.0",
+        "pycryptodome>=3.12.0",
         "pytz>=2021.3",
         "pyvmomi>=8.0.0.1.1",
         "requests>=2.31.0",
-        "urllib3>=1.26.16",
+        "urllib3>=1.26.7",
         "azure-common>=1.1.28",
         "azure-core>=1.26.1",
         "azure-mgmt-resource>=22.0.0",
         "azure-identity>=1.12.0",
         "azure.mgmt.network>=22.2.0",
         "azure.mgmt.compute>=29.0.0",
         "azure-mgmt-core>=1.3.2",
         "azure.mgmt.storage>=21.0.0",
-        "azure-mgmt-dns>=8.1.0",
-        "azure-mgmt-privatedns>=1.1.0",
         "azure.mgmt.subscription>=3.1.1",
         "ply>=3.11",
         "pytest==7.4.0",
         "pytest-asyncio==0.21.1",
         "pytest-rerunfailures==12.0",
         "sqlite-utils~=3.11",
-        "docker>=5.0.3",
-        "paramiko>=3.4.0",
+        "paramiko>=3.3.1",
         "overrides>=7.4.0",
-        "bumpversion>=0.6.0",
-        "PyYAML>=5.1",
-        "rsa>=4.9",
-        "pywinrm>=0.4.3",
-        "aiohttp>=3.9.3",
-        "python-certifi-win32>=1.6.1",
-        "certifi>=2023.5.7",
-        "pyhostprep>=1.0.10"
+        "bumpversion>=0.6.0"
     ],
     author_email='info@unix.us.com',
     description='Couchbase Cloud Automation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=["couchbase", "devops", "automation"],
     classifiers=[
-        "Development Status :: 4 - Beta",
-        "License :: OSI Approved :: Apache Software License",
-        "Intended Audience :: Developers",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Topic :: Database",
-        "Topic :: Software Development :: Libraries",
-        "Topic :: Software Development :: Libraries :: Python Modules"
-    ],
+          "Development Status :: 4 - Beta",
+          "License :: OSI Approved :: Apache Software License",
+          "Intended Audience :: Developers",
+          "Operating System :: OS Independent",
+          "Programming Language :: Python",
+          "Programming Language :: Python :: 3",
+          "Topic :: Database",
+          "Topic :: Software Development :: Libraries",
+          "Topic :: Software Development :: Libraries :: Python Modules"],
 )
```

