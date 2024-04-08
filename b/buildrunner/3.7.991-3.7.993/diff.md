# Comparing `tmp/buildrunner-3.7.991.tar.gz` & `tmp/buildrunner-3.7.993.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildrunner-3.7.991.tar", last modified: Wed Apr  3 16:06:49 2024, max compression
+gzip compressed data, was "buildrunner-3.7.993.tar", last modified: Mon Apr  8 20:41:27 2024, max compression
```

## Comparing `buildrunner-3.7.991.tar` & `buildrunner-3.7.993.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.813845 buildrunner-3.7.991/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-03 16:06:45.000000 buildrunner-3.7.991/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 16:06:45.000000 buildrunner-3.7.991/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    47194 2024-04-03 16:06:49.813845 buildrunner-3.7.991/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    45194 2024-04-03 16:06:45.000000 buildrunner-3.7.991/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.801845 buildrunner-3.7.991/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-04-03 16:06:45.000000 buildrunner-3.7.991/bin/buildrunner
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-03 16:06:45.000000 buildrunner-3.7.991/bin/buildrunner-cleanup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.801845 buildrunner-3.7.991/buildrunner/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/SourceDockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    20088 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12787 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.805845 buildrunner-3.7.991/buildrunner/config/
--rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.805845 buildrunner-3.7.991/buildrunner/config/fetch/
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/fetch/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/fetch/github.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/fetch/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/jinja_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/models_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.809846 buildrunner-3.7.991/buildrunner/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23618 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/multiplatform_image_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    23033 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.809846 buildrunner-3.7.991/buildrunner/provisioners/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/provisioners/salt.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/provisioners/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.809846 buildrunner-3.7.991/buildrunner/sshagent/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.809846 buildrunner-3.7.991/buildrunner/sshagent/SSHAgentProxyImage/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      212 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/sshagent/SSHAgentProxyImage/login.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/sshagent/SSHAgentProxyImage/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/sshagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.809846 buildrunner-3.7.991/buildrunner/steprunner/
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.809846 buildrunner-3.7.991/buildrunner/steprunner/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/tasks/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    18064 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/tasks/push.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/tasks/pypipush.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/tasks/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    43019 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/tasks/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 16:06:49.000000 buildrunner-3.7.991/buildrunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.813845 buildrunner-3.7.991/buildrunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    47194 2024-04-03 16:06:49.000000 buildrunner-3.7.991/buildrunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-03 16:06:49.000000 buildrunner-3.7.991/buildrunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:06:49.000000 buildrunner-3.7.991/buildrunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-03 16:06:49.000000 buildrunner-3.7.991/buildrunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 16:06:49.000000 buildrunner-3.7.991/buildrunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-03 16:06:45.000000 buildrunner-3.7.991/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:06:49.813845 buildrunner-3.7.991/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-03 16:06:45.000000 buildrunner-3.7.991/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-03 16:06:45.000000 buildrunner-3.7.991/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.813845 buildrunner-3.7.991/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_buildrunner_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    13838 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21059 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_multiplatform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_push_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)    15598 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_push_security_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_util_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_utils_flock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.471107 buildrunner-3.7.993/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-08 20:41:23.000000 buildrunner-3.7.993/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 20:41:23.000000 buildrunner-3.7.993/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    47194 2024-04-08 20:41:27.471107 buildrunner-3.7.993/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45194 2024-04-08 20:41:23.000000 buildrunner-3.7.993/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.459107 buildrunner-3.7.993/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-04-08 20:41:23.000000 buildrunner-3.7.993/bin/buildrunner
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-08 20:41:23.000000 buildrunner-3.7.993/bin/buildrunner-cleanup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.463107 buildrunner-3.7.993/buildrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/SourceDockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    20088 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.463107 buildrunner-3.7.993/buildrunner/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.463107 buildrunner-3.7.993/buildrunner/config/fetch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/config/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/config/fetch/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/config/fetch/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/config/fetch/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/config/jinja_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/config/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/config/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/config/models_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/config/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.463107 buildrunner-3.7.993/buildrunner/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/docker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/docker/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/docker/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/docker/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23618 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/docker/multiplatform_image_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23033 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/docker/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.467107 buildrunner-3.7.993/buildrunner/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/provisioners/salt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/provisioners/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.467107 buildrunner-3.7.993/buildrunner/sshagent/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.467107 buildrunner-3.7.993/buildrunner/sshagent/SSHAgentProxyImage/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      212 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/sshagent/SSHAgentProxyImage/login.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/sshagent/SSHAgentProxyImage/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/sshagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.467107 buildrunner-3.7.993/buildrunner/steprunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/steprunner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.467107 buildrunner-3.7.993/buildrunner/steprunner/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/steprunner/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/steprunner/tasks/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18064 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/steprunner/tasks/push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/steprunner/tasks/pypipush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/steprunner/tasks/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43019 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/steprunner/tasks/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-04-08 20:41:23.000000 buildrunner-3.7.993/buildrunner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 20:41:27.000000 buildrunner-3.7.993/buildrunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.471107 buildrunner-3.7.993/buildrunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    47194 2024-04-08 20:41:27.000000 buildrunner-3.7.993/buildrunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-08 20:41:27.000000 buildrunner-3.7.993/buildrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:41:27.000000 buildrunner-3.7.993/buildrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-08 20:41:27.000000 buildrunner-3.7.993/buildrunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 20:41:27.000000 buildrunner-3.7.993/buildrunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-08 20:41:23.000000 buildrunner-3.7.993/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:41:27.471107 buildrunner-3.7.993/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-08 20:41:23.000000 buildrunner-3.7.993/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-08 20:41:23.000000 buildrunner-3.7.993/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:41:27.471107 buildrunner-3.7.993/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_buildrunner_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13838 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21059 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_multiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_push_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15598 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_push_security_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_util_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_utils_flock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-08 20:41:23.000000 buildrunner-3.7.993/tests/test_version.py
```

### Comparing `buildrunner-3.7.991/LICENSE` & `buildrunner-3.7.993/LICENSE`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/PKG-INFO` & `buildrunner-3.7.993/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildrunner
-Version: 3.7.991
+Version: 3.7.993
 Summary: Docker-based build tool
 Home-page: https://github.com/adobe/buildrunner
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `buildrunner-3.7.991/README.rst` & `buildrunner-3.7.993/README.rst`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/__init__.py` & `buildrunner-3.7.993/buildrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/cli.py` & `buildrunner-3.7.993/buildrunner/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,15 @@
         run_config_file=args.config_file,
         build_time=epoch_time(),
         log_generated_files=(
             bool(args.log_generated_files or args.print_generated_files)
         ),
         # Do not attempt to load run configuration, just global configuration
         load_run_config=False,
+        global_config_overrides=_get_global_config_overrides(args),
     )
     BuildRunner.clean_cache()
 
 
 def _create_results_dir(cleanup_step_artifacts: bool, build_results_dir: str) -> None:
     try:
         # cleanup existing results dir (if needed)
```

### Comparing `buildrunner-3.7.991/buildrunner/config/__init__.py` & `buildrunner-3.7.993/buildrunner/config/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/config/fetch/__init__.py` & `buildrunner-3.7.993/buildrunner/config/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/config/fetch/file.py` & `buildrunner-3.7.993/buildrunner/config/fetch/file.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/config/fetch/github.py` & `buildrunner-3.7.993/buildrunner/config/fetch/github.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/config/jinja_context.py` & `buildrunner-3.7.993/buildrunner/config/jinja_context.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/config/loader.py` & `buildrunner-3.7.993/buildrunner/config/loader.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/config/models.py` & `buildrunner-3.7.993/buildrunner/config/models.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/config/models_step.py` & `buildrunner-3.7.993/buildrunner/config/models_step.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/config/validation.py` & `buildrunner-3.7.993/buildrunner/config/validation.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/docker/__init__.py` & `buildrunner-3.7.993/buildrunner/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/docker/builder.py` & `buildrunner-3.7.993/buildrunner/docker/builder.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/docker/daemon.py` & `buildrunner-3.7.993/buildrunner/docker/daemon.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/docker/image_info.py` & `buildrunner-3.7.993/buildrunner/docker/image_info.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/docker/importer.py` & `buildrunner-3.7.993/buildrunner/docker/importer.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/docker/multiplatform_image_builder.py` & `buildrunner-3.7.993/buildrunner/docker/multiplatform_image_builder.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/docker/runner.py` & `buildrunner-3.7.993/buildrunner/docker/runner.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/errors.py` & `buildrunner-3.7.993/buildrunner/errors.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/loggers.py` & `buildrunner-3.7.993/buildrunner/loggers.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/provisioners/__init__.py` & `buildrunner-3.7.993/buildrunner/provisioners/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/provisioners/salt.py` & `buildrunner-3.7.993/buildrunner/provisioners/salt.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/provisioners/shell.py` & `buildrunner-3.7.993/buildrunner/provisioners/shell.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile` & `buildrunner-3.7.993/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/sshagent/__init__.py` & `buildrunner-3.7.993/buildrunner/sshagent/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/steprunner/__init__.py` & `buildrunner-3.7.993/buildrunner/steprunner/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/steprunner/tasks/__init__.py` & `buildrunner-3.7.993/buildrunner/steprunner/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/steprunner/tasks/build.py` & `buildrunner-3.7.993/buildrunner/steprunner/tasks/build.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/steprunner/tasks/push.py` & `buildrunner-3.7.993/buildrunner/steprunner/tasks/push.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/steprunner/tasks/pypipush.py` & `buildrunner-3.7.993/buildrunner/steprunner/tasks/pypipush.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/steprunner/tasks/remote.py` & `buildrunner-3.7.993/buildrunner/steprunner/tasks/remote.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/steprunner/tasks/run.py` & `buildrunner-3.7.993/buildrunner/steprunner/tasks/run.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner/utils.py` & `buildrunner-3.7.993/buildrunner/utils.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner.egg-info/PKG-INFO` & `buildrunner-3.7.993/buildrunner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildrunner
-Version: 3.7.991
+Version: 3.7.993
 Summary: Docker-based build tool
 Home-page: https://github.com/adobe/buildrunner
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `buildrunner-3.7.991/buildrunner.egg-info/SOURCES.txt` & `buildrunner-3.7.993/buildrunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/buildrunner.egg-info/requires.txt` & `buildrunner-3.7.993/buildrunner.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/requirements.txt` & `buildrunner-3.7.993/requirements.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/setup.py` & `buildrunner-3.7.993/setup.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/test_requirements.txt` & `buildrunner-3.7.993/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_buildrunner_files.py` & `buildrunner-3.7.993/tests/test_buildrunner_files.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_caching.py` & `buildrunner-3.7.993/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_cli.py` & `buildrunner-3.7.993/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_dependencies.py` & `buildrunner-3.7.993/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_image_info.py` & `buildrunner-3.7.993/tests/test_image_info.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_loggers.py` & `buildrunner-3.7.993/tests/test_loggers.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_multiplatform.py` & `buildrunner-3.7.993/tests/test_multiplatform.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_push_artifact.py` & `buildrunner-3.7.993/tests/test_push_artifact.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_push_security_scan.py` & `buildrunner-3.7.993/tests/test_push_security_scan.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_runner.py` & `buildrunner-3.7.993/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_util_checksum.py` & `buildrunner-3.7.993/tests/test_util_checksum.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_utils_flock.py` & `buildrunner-3.7.993/tests/test_utils_flock.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.7.991/tests/test_version.py` & `buildrunner-3.7.993/tests/test_version.py`

 * *Files identical despite different names*

