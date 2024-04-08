# Comparing `tmp/launch-cli-0.3.0.tar.gz` & `tmp/launch-cli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launch-cli-0.3.0.tar", last modified: Thu Mar  7 18:56:56 2024, max compression
+gzip compressed data, was "launch-cli-0.4.0.tar", last modified: Mon Apr  8 20:45:19 2024, max compression
```

## Comparing `launch-cli-0.3.0.tar` & `launch-cli-0.4.0.tar`

### file list

```diff
@@ -1,75 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.600565 launch-cli-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-07 18:56:42.000000 launch-cli-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-03-07 18:56:56.600565 launch-cli-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-03-07 18:56:42.000000 launch-cli-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.600565 launch-cli-0.3.0/launch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-03-07 18:56:56.000000 launch-cli-0.3.0/launch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-07 18:56:56.000000 launch-cli-0.3.0/launch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 18:56:56.000000 launch-cli-0.3.0/launch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-07 18:56:56.000000 launch-cli-0.3.0/launch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-07 18:56:56.000000 launch-cli-0.3.0/launch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-07 18:56:56.000000 launch-cli-0.3.0/launch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-07 18:56:42.000000 launch-cli-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 18:56:56.600565 launch-cli-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.588565 launch-cli-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.592565 launch-cli-0.3.0/src/launch/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.592565 launch-cli-0.3.0/src/launch/automation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/automation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.592565 launch-cli-0.3.0/src/launch/automation/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/automation/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/automation/common/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.592565 launch-cli-0.3.0/src/launch/automation/helm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/automation/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/automation/helm/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.592565 launch-cli-0.3.0/src/launch/automation/provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/automation/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.592565 launch-cli-0.3.0/src/launch/automation/provider/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/automation/provider/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/automation/provider/aws/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.592565 launch-cli-0.3.0/src/launch/automation/terragrunt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/automation/terragrunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/automation/terragrunt/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.592565 launch-cli-0.3.0/src/launch/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.592565 launch-cli-0.3.0/src/launch/cli/github/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.596565 launch-cli-0.3.0/src/launch/cli/github/access/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/github/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/github/access/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.596565 launch-cli-0.3.0/src/launch/cli/github/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/github/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/github/hooks/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.596565 launch-cli-0.3.0/src/launch/cli/github/repo/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/github/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/github/repo/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.596565 launch-cli-0.3.0/src/launch/cli/github/version/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/github/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/github/version/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.596565 launch-cli-0.3.0/src/launch/cli/helm/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/helm/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.596565 launch-cli-0.3.0/src/launch/cli/service/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/service/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.596565 launch-cli-0.3.0/src/launch/cli/terragrunt/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/terragrunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/cli/terragrunt/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.596565 launch-cli-0.3.0/src/launch/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/github/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/github/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/github/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/github/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/github/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.596565 launch-cli-0.3.0/src/launch/local_repo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/local_repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/local_repo/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/local_repo/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/local_repo/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:56.600565 launch-cli-0.3.0/src/launch/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/service/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-07 18:56:42.000000 launch-cli-0.3.0/src/launch/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.760166 launch-cli-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 20:45:06.000000 launch-cli-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19185 2024-04-08 20:45:19.760166 launch-cli-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-04-08 20:45:06.000000 launch-cli-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.760166 launch-cli-0.4.0/launch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19185 2024-04-08 20:45:19.000000 launch-cli-0.4.0/launch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-08 20:45:19.000000 launch-cli-0.4.0/launch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:45:19.000000 launch-cli-0.4.0/launch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 20:45:19.000000 launch-cli-0.4.0/launch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-08 20:45:19.000000 launch-cli-0.4.0/launch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 20:45:19.000000 launch-cli-0.4.0/launch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-08 20:45:06.000000 launch-cli-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:45:19.760166 launch-cli-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.748166 launch-cli-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/automation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/automation/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/common/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/automation/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/helm/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/automation/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/automation/provider/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/provider/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/provider/aws/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/automation/provider/az/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/provider/az/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/provider/az/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/automation/terragrunt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/terragrunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/terragrunt/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/github/access/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/access/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/github/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/hooks/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/github/repo/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/repo/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/github/version/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/version/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/helm/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/service/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/terragrunt/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/terragrunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/terragrunt/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/github/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/github/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/github/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/github/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/github/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.760166 launch-cli-0.4.0/src/launch/local_repo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/local_repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/local_repo/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/local_repo/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/local_repo/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/local_repo/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.760166 launch-cli-0.4.0/src/launch/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/service/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/update.py
```

### Comparing `launch-cli-0.3.0/LICENSE` & `launch-cli-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/launch_cli.egg-info/SOURCES.txt` & `launch-cli-0.4.0/launch_cli.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 src/launch/automation/common/__init__.py
 src/launch/automation/common/functions.py
 src/launch/automation/helm/__init__.py
 src/launch/automation/helm/functions.py
 src/launch/automation/provider/__init__.py
 src/launch/automation/provider/aws/__init__.py
 src/launch/automation/provider/aws/functions.py
+src/launch/automation/provider/az/__init__.py
+src/launch/automation/provider/az/functions.py
 src/launch/automation/terragrunt/__init__.py
 src/launch/automation/terragrunt/functions.py
 src/launch/cli/__init__.py
 src/launch/cli/entrypoint.py
 src/launch/cli/github/__init__.py
 src/launch/cli/github/access/__init__.py
 src/launch/cli/github/access/commands.py
@@ -42,10 +44,11 @@
 src/launch/github/auth.py
 src/launch/github/hooks.py
 src/launch/github/repo.py
 src/launch/github/tags.py
 src/launch/local_repo/__init__.py
 src/launch/local_repo/branch.py
 src/launch/local_repo/predict.py
+src/launch/local_repo/repo.py
 src/launch/local_repo/tags.py
 src/launch/service/__init__.py
 src/launch/service/common.py
```

### Comparing `launch-cli-0.3.0/pyproject.toml` & `launch-cli-0.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "launch-cli"
-version = "0.3.0"
+version = "0.4.0"
 description = "CLI tooling for common Launch functions"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "Apache 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = ["click>=8.1.7", "pygithub>=2.1.1", "click-spinner>=0.1.10", "gitpython>=3.1", "semver>=3.0", "Jinja2>=3.1.3", "ruamel.yaml>=0.17.32"]
 
 [project.urls]
-Homepage = "https://github.com/nexient-llc/launch-cli"
-Issues = "https://github.com/nexient-llc/launch-cli/issues"
+Homepage = "https://github.com/launchbynttdata/launch-cli"
+Issues = "https://github.com/launchbynttdata/launch-cli/issues"
 
 [tool.setuptools]
 package-dir = {launch="src/launch"}
 
 [project.optional-dependencies]
 dev = ["pytest~=7.0", "pytest-mock~=3.0", "responses~=0.24.0", "black>=23.11.0", "isort>=5.12.0"]
```

### Comparing `launch-cli-0.3.0/src/launch/automation/common/functions.py` & `launch-cli-0.4.0/src/launch/automation/common/functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,76 +2,35 @@
 import json
 import logging
 import os
 import pathlib
 import shutil
 import string
 import subprocess
+from pathlib import Path
+from typing import Callable
 
-import git
-from git.repo import Repo
+from git import Repo
 from ruamel.yaml import YAML
 
 from launch import DISCOVERY_FORBIDDEN_DIRECTORIES
 
 logger = logging.getLogger(__name__)
 
 
-## GIT Specific Functions
-def git_clone(skip_git: str, target_dir: str, clone_url: str) -> Repo:
-    if not skip_git:
-        try:
-            logger.info(f"Cloning repository: {clone_url} into {target_dir}")
-            repository = Repo.clone_from(clone_url, target_dir)
-        except git.GitCommandError as e:
-            logger.error(
-                f"Error occurred while cloning the repository: {clone_url}, Error: {e}"
-            )
-            raise RuntimeError(
-                f"An error occurred while cloning the repository: {clone_url}"
-            ) from e
-        return repository
-    else:
-        try:
-            logger.info(f"Getting repository: {clone_url} into {target_dir}")
-            if clone_url.endswith(".git"):
-                clone_url = clone_url[:-4]
-            repo_name = clone_url.split("/")[-1:]
-            repository = Repo(f"./{repo_name[0]}")
-        except (git.GitCommandError, git.exc.NoSuchPathError) as e:
-            logger.error(
-                f"Error occurred while getting the repository: {clone_url}, Error: {e}"
-            )
-            raise RuntimeError(
-                f"An error occurred while getting the repository: {clone_url}"
-            ) from e
-        return repository
-
-
-def git_checkout(skip_git, repository: Repo, branch=None, new_branch=False) -> None:
-    if skip_git:
-        return None
-    if branch:
-        try:
-            if new_branch:
-                repository.git.checkout("-b", branch)
-                logger.info(f"Checked out new branch: {branch}")
-            else:
-                repository.git.checkout(branch)
-                logger.info(f"Checked out branch: {branch}")
-        except git.GitCommandError as e:
-            raise RuntimeError(
-                f"An error occurred while checking out {branch}:  {str(e)}"
-            ) from e
-
-
 ## Other Functions
-def check_git_changes(repository, commit_id, main_branch, directory) -> bool:
+def check_git_changes(
+    repository: Repo,
+    commit_id: str,
+    main_branch: str,
+    directory: str,
+) -> bool:
     logger.info(f"Checking if git changes are exclusive to: {directory}")
-    origin = repository.remote(name="origin")
+
+    origin = repository.remotes.origin
     origin.fetch()
 
     commit_main = repository.commit(f"origin/{main_branch}")
 
     # Check if the PR commit hash is the same as the commit sha of the main branch
     if commit_id == repository.rev_parse(f"origin/{main_branch}"):
         logger.info(f"Commit hash is the same as origin/{main_branch}")
@@ -155,43 +114,58 @@
     logger.info(f"Running make configure")
     try:
         subprocess.run(["make", "configure"], check=True)
     except subprocess.CalledProcessError as e:
         raise RuntimeError(f"An error occurred: {str(e)}") from e
 
 
-def deploy_remote_state(provider_config: dict) -> None:
-    run_list = ["make"]
-
-    if provider_config["az"].get("name_prefix"):
-        run_list.append(f"NAME_PREFIX={provider_config['az'].get('name_prefix')}")
-    if provider_config["az"].get("region"):
-        run_list.append(f"REGION={provider_config['az'].get('region')}")
-    if provider_config["az"].get("environment"):
-        run_list.append(f"ENVIRONMENT={provider_config['az'].get('environment')}")
-    if provider_config["az"].get("env_instance"):
-        run_list.append(f"ENV_INSTANCE={provider_config['az'].get('env_instance')}")
-    if provider_config["az"].get("container_name"):
-        run_list.append(f"CONTAINER_NAME={provider_config['az'].get('container_name')}")
-    if provider_config["az"].get("storage_account_name"):
-        run_list.append(
-            f"STORAGE_ACCOUNT_NAME={provider_config['az'].get('storage_account_name')}"
-        )
-    if provider_config["az"].get("resource_group_name"):
-        run_list.append(
-            f"RESOURCE_GROUP_NAME={provider_config['az'].get('resource_group_name')}"
-        )
+def traverse_with_callback(
+    dictionary: dict,
+    callback: Callable,
+    current_path: Path = Path("platform"),
+    **kwargs,
+) -> dict:
+    """
+    Recursively traverses a dictionary and applies a callback function. The callback function is expected to return a dictionary, which will replace the current dictionary. If the callback function returns None, the current dictionary will be used. The callback function is expected to accept the following keyword arguments:
+    - key: The current key in the dictionary
+    - value: The current value in the dictionary
+    - dictionary: The current dictionary being traversed
+    - current_path: The current path in the dictionary
+    - **kwargs: Additional keyword arguments to pass to the callback function
 
-    run_list.append("terragrunt/remote_state/azure")
+    Args:
+        dictionary (dict): The dictionary to traverse.
+        callback (Callable): The callback function to apply to each key-value pair.
+        current_path (Path, optional): The current path in the dictionary. Defaults to Path("platform").
+        **kwargs: Additional keyword arguments to pass to the callback function.
 
-    logger.info(f"Running {run_list}")
-    try:
-        subprocess.run(run_list, check=True)
-    except subprocess.CalledProcessError as e:
-        raise RuntimeError(f"An error occurred: {str(e)}") from e
+    Returns:
+        dict: The modified dictionary after applying the callback function.
+    """
+    data = None
+    if isinstance(dictionary, dict):
+        for key, value in list(dictionary.items()):
+            kwargs["nested_dict"] = dictionary
+            data = callback(
+                key=key,
+                value=value,
+                dictionary=dictionary,
+                current_path=current_path,
+                **kwargs,
+            )
+            if not data:
+                traverse_with_callback(
+                    dictionary=value,
+                    callback=callback,
+                    current_path=current_path / Path(key),
+                    **kwargs,
+                )
+    elif isinstance(dict, list):
+        pass
+    return data or dictionary
 
 
 def discover_files(
     root_path: pathlib.Path,
     filename_partial: str = "",
     forbidden_directories: list[str] = None,
 ) -> list[pathlib.Path]:
@@ -323,7 +297,51 @@
     else:
         logger.debug(
             f"Unpacking archive {archive_path} to {destination} with overridden format {format_override}"
         )
         shutil.unpack_archive(
             filename=archive_path, extract_dir=destination, format=format_override
         )
+
+
+def recursive_dictionary_merge(a: dict, b: dict, path=[]) -> dict:
+    """Merges dictionary 'b' into dictionary 'a', will halt upon encountering a difference in the two dictionaries' values.
+
+    Args:
+        a (dict): Dictionary of arbitrary depth
+        b (dict): Dictionary of arbitrary depth
+        path (list, optional): Mechanism to report on where conflicts arise, no need to set this for external callers. Defaults to [].
+
+    Raises:
+        ValueError: Raised when both dictionaries contain a common key with a differing value.
+
+    Returns:
+        dict: Modified 'a' dictionary with keys and values merged from 'b'
+    """
+    for key in b:
+        if key in a:
+            if isinstance(a[key], dict) and isinstance(b[key], dict):
+                recursive_dictionary_merge(a[key], b[key], path + [str(key)])
+            elif a[key] != b[key]:
+                raise ValueError(f"Conflict at {'.'.join(path + [str(key)])}")
+        else:
+            a[key] = b[key]
+    return a
+
+
+def extract_uuid_key(source_data: dict) -> dict:
+    """Given a 'source_data' dictionary of arbitrary depth, find and return any 'uuid' keys while retaining the structure
+    of the dictionary. If there is not 'uuid' key, an dictionary matching the structure will be returned with no keys other
+    than the ones required to give it that structure.
+
+    Args:
+        source_data (dict): Nested dictionary
+
+    Returns:
+        dict: Nested dictionary with all keys excepting 'uuid' removed. The nesting structure of the input will be otherwise maintained.
+    """
+    for key in source_data:
+        if isinstance(source_data[key], dict):
+            return {key: extract_uuid_key(source_data=source_data[key])}
+        elif key == "uuid":
+            return {key: source_data[key]}
+    return {}
```

### Comparing `launch-cli-0.3.0/src/launch/automation/helm/functions.py` & `launch-cli-0.4.0/src/launch/automation/helm/functions.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/automation/provider/aws/functions.py` & `launch-cli-0.4.0/src/launch/automation/provider/aws/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 
 
 def assume_role(
     provider_config: dict, repository_name: str, target_environment: str
 ) -> None:
     logger.info("Assuming the IAM deployment role")
 
-    profile = provider_config["aws"]["role_arn"]
+    provider = provider_config["provider"]
+    profile = provider_config[provider]["role_arn"]
 
     try:
         sts_credentials = json.loads(
             subprocess.check_output(
                 [
                     "aws",
                     "sts",
                     "assume-role",
                     "--role-arn",
-                    provider_config["aws"]["role_arn"],
+                    provider_config[provider]["role_arn"],
                     "--role-session-name",
                     "caf-build-agent",
                 ]
             )
         )
     except Exception as e:
         raise RuntimeError(f"Failed aws sts assume-role: {str(e)}") from e
@@ -65,12 +66,12 @@
         )
         subprocess.run(
             [
                 "aws",
                 "configure",
                 "set",
                 f"profile.{profile}.region",
-                provider_config["aws"]["region"],
+                provider_config[provider]["region"],
             ]
         )
     except subprocess.CalledProcessError as e:
         raise RuntimeError(f"Failed set aws configure: {str(e)}")
```

### Comparing `launch-cli-0.3.0/src/launch/cli/entrypoint.py` & `launch-cli-0.4.0/src/launch/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/cli/github/access/commands.py` & `launch-cli-0.4.0/src/launch/cli/github/access/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/cli/github/hooks/commands.py` & `launch-cli-0.4.0/src/launch/cli/github/hooks/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/cli/github/repo/commands.py` & `launch-cli-0.4.0/src/launch/cli/github/repo/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     return repository
 
 
 @click.command()
 @click.option(
     "--organization",
     default=GITHUB_ORG_NAME,
-    help="GitHub organization containing your repository. Defaults to the nexient-llc organization.",
+    help=f"GitHub organization containing your repository. Defaults to the {GITHUB_ORG_NAME} organization.",
 )
 @click.option("--name", required=True, help="The name of the repository.")
 @click.option(
     "--description",
     default="Service created with launch-cli.",
     help="A short description of the repository.",
 )
```

### Comparing `launch-cli-0.3.0/src/launch/cli/github/version/commands.py` & `launch-cli-0.4.0/src/launch/cli/github/version/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/cli/helm/commands.py` & `launch-cli-0.4.0/src/launch/cli/helm/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/env.py` & `launch-cli-0.4.0/src/launch/env.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/github/access.py` & `launch-cli-0.4.0/src/launch/github/access.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/github/auth.py` & `launch-cli-0.4.0/src/launch/github/auth.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/github/hooks.py` & `launch-cli-0.4.0/src/launch/github/hooks.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/github/repo.py` & `launch-cli-0.4.0/src/launch/local_repo/repo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,45 @@
 import logging
+import subprocess
 
-import git
-from git.repo import Repo
-from github import Github
-from github.AuthenticatedUser import AuthenticatedUser
-from github.Repository import Repository
+from git import GitCommandError, Repo
+
+from launch import INIT_BRANCH
 
 logger = logging.getLogger(__name__)
 
 
-def get_github_repos(
-    g: Github, user: AuthenticatedUser | None = None
-) -> list[Repository]:
-    if user:
-        return user.get_repos()
-    repos = [repo for repo in g.get_user().get_repos()]
-    logger.debug(f"Fetched {len(repos)}")
-    return repos
+def checkout_branch(
+    repository: Repo, target_branch: str, new_branch: bool = False
+) -> None:
+    command_args = []
+    if new_branch:
+        command_args.append("-b")
+    command_args.append(target_branch)
+
+    try:
+        logger.debug(f"{repository}: git checkout {' '.join(command_args)}")
+        repository.git.checkout(command_args)
+        logger.info(f"Checked out branch {target_branch}")
+    except GitCommandError as e:
+        message = f"An error occurred while checking out {target_branch}"
+        logger.exception(message)
+        raise RuntimeError(message) from e
 
 
-def clone_repository(repository_url: str, target: str, branch: str):
+def clone_repository(repository_url: str, target: str, branch: str) -> Repo:
     try:
         logger.info(f"Attempting to clone repository: {repository_url} into {target}")
         repository = Repo.clone_from(repository_url, target, branch=branch)
         logger.info(f"Repository {repository_url} cloned successfully to {target}")
-    except git.GitCommandError as e:
-        logger.error(
-            f"Error occurred while cloning the repository: {repository_url}, Error: {e}"
-        )
-        raise RuntimeError(
-            f"An error occurred while cloning the repository: {repository_url}"
-        ) from e
+    except GitCommandError as e:
+        message = f"Error occurred while cloning the repository from {repository_url}"
+        logger.exception(message)
+        raise RuntimeError(message) from e
     return repository
 
 
-def create_repository(
-    g: Github,
-    organization: str,
-    name: str,
-    description: str,
-    public: bool,
-    visibility: str,
-) -> Repo:
-    try:
-        return g.get_organization(organization).create_repo(
-            name=name,
-            description=description,
-            private=not public,
-            visibility=visibility,
-        )
-    except Exception as e:
-        raise RuntimeError(
-            f"Failed to create repository {name} in {organization}"
-        ) from e
+def push_branch(repository: Repo, branch: str, commit_msg="Initial commit") -> None:
+    logger.info(f"{repository=}, {branch=}, {commit_msg=}")
+    repository.git.add(["."])
+    repository.git.commit(["-m", commit_msg])
+    repository.git.push(["--set-upstream", "origin", branch])
```

### Comparing `launch-cli-0.3.0/src/launch/github/tags.py` & `launch-cli-0.4.0/src/launch/github/tags.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/local_repo/predict.py` & `launch-cli-0.4.0/src/launch/local_repo/predict.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/local_repo/tags.py` & `launch-cli-0.4.0/src/launch/local_repo/tags.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.3.0/src/launch/update.py` & `launch-cli-0.4.0/src/launch/update.py`

 * *Files identical despite different names*

