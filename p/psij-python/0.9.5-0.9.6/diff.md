# Comparing `tmp/psij-python-0.9.5.tar.gz` & `tmp/psij-python-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psij-python-0.9.5.tar", last modified: Mon Mar 25 16:31:53 2024, max compression
+gzip compressed data, was "psij-python-0.9.6.tar", last modified: Mon Apr  8 19:34:53 2024, max compression
```

## Comparing `psij-python-0.9.5.tar` & `psij-python-0.9.6.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.182849 psij-python-0.9.5/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1065 2024-03-25 16:31:01.000000 psij-python-0.9.5/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      399 2024-03-25 16:31:53.182849 psij-python-0.9.5/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      904 2024-03-25 16:31:01.000000 psij-python-0.9.5/README.md
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-03-25 16:31:53.182849 psij-python-0.9.5/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     1221 2024-03-25 16:31:01.000000 psij-python-0.9.5/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.174849 psij-python-0.9.5/src/
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.174849 psij-python-0.9.5/src/psij/
--rw-rw-r--   0 mike      (1000) mike      (1000)     3577 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      243 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/__main__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4766 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/_plugins.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4875 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3003 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/exceptions.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.178849 psij-python-0.9.5/src/psij/executors/
--rw-rw-r--   0 mike      (1000) mike      (1000)      341 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/__init__.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.178849 psij-python-0.9.5/src/psij/executors/batch/
--rw-rw-r--   0 mike      (1000) mike      (1000)       86 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    31379 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/batch_scheduler_executor.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.178849 psij-python-0.9.5/src/psij/executors/batch/cobalt/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1769 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/cobalt/cobalt.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)     5704 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/cobalt.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      807 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/escape_functions.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.178849 psij-python-0.9.5/src/psij/executors/batch/lsf/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1824 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/lsf/lsf.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)     6177 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/lsf.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.178849 psij-python-0.9.5/src/psij/executors/batch/pbs/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1596 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/pbs/pbs_classic.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)     1685 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/pbs/pbspro.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)      988 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/pbs.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     7118 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/pbs_base.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1138 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/pbs_classic.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3248 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/script_generator.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.178849 psij-python-0.9.5/src/psij/executors/batch/slurm/
--rw-rw-r--   0 mike      (1000) mike      (1000)     3235 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/slurm/slurm.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)     9839 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/slurm.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2343 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/batch/template_function_library.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     7359 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/flux.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    15054 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/local.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6220 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/executors/rp.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    10706 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/job.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6367 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/job_attributes.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    14194 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/job_executor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2721 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/job_executor_config.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4624 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/job_launcher.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    12790 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/job_spec.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4985 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/job_state.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1995 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/job_status.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4280 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launcher.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.178849 psij-python-0.9.5/src/psij/launchers/
--rw-rw-r--   0 mike      (1000) mike      (1000)      623 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      557 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/aprun.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      554 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/jsrun.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      692 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/mpirun.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1718 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/multiple.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     8023 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/script_based_launcher.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.178849 psij-python-0.9.5/src/psij/launchers/scripts/
--rw-rw-r--   0 mike      (1000) mike      (1000)       69 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/scripts/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      300 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/scripts/aprun_launch.sh
--rwxrwxr-x   0 mike      (1000) mike      (1000)      307 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/scripts/jsrun_launch.sh
--rwxrwxr-x   0 mike      (1000) mike      (1000)      812 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/scripts/launcher_lib.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      546 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/scripts/mpi_launch.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      594 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/scripts/multi_launch.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      236 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/scripts/single_launch.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      274 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/scripts/srun_launch.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      643 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/single.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      660 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/launchers/srun.py
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/py.typed
--rw-rw-r--   0 mike      (1000) mike      (1000)     9052 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/resource_spec.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    10549 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/serialize.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1881 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij/utils.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      168 2024-03-25 16:31:48.000000 psij-python-0.9.5/src/psij/version.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.178849 psij-python-0.9.5/src/psij-descriptors/
--rw-rw-r--   0 mike      (1000) mike      (1000)      217 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij-descriptors/aprun_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      262 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij-descriptors/cobalt_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      616 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij-descriptors/core_descriptors.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      248 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij-descriptors/flux_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      216 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij-descriptors/jsrun_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      250 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij-descriptors/lsf_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      564 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij-descriptors/pbs_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      285 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij-descriptors/rp_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      258 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij-descriptors/slurm_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      214 2024-03-25 16:31:01.000000 psij-python-0.9.5/src/psij-descriptors/srun_descriptor.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.178849 psij-python-0.9.5/src/psij_python.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      399 2024-03-25 16:31:53.000000 psij-python-0.9.5/src/psij_python.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     2821 2024-03-25 16:31:53.000000 psij-python-0.9.5/src/psij_python.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-03-25 16:31:53.000000 psij-python-0.9.5/src/psij_python.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       88 2024-03-25 16:31:53.000000 psij-python-0.9.5/src/psij_python.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       22 2024-03-25 16:31:53.000000 psij-python-0.9.5/src/psij_python.egg-info/top_level.txt
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-03-25 16:31:53.182849 psij-python-0.9.5/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)     2192 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_callbacks.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4938 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_doc_examples.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     7986 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_executor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      994 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_executor_loading.py
--rwxrwxr-x   0 mike      (1000) mike      (1000)      316 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_executor_versions.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      610 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_infrastructure.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_issue_387_1.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_issue_387_2.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_issue_387_3.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      589 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_issue_435.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1606 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_job_spec.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2159 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_mpi.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1209 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_nodefile.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3289 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_resources.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      836 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_serialization.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      911 2024-03-25 16:31:01.000000 psij-python-0.9.5/tests/test_wait.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.593047 psij-python-0.9.6/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1065 2024-04-08 19:34:25.000000 psij-python-0.9.6/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      399 2024-04-08 19:34:53.593047 psij-python-0.9.6/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      904 2024-04-08 19:34:25.000000 psij-python-0.9.6/README.md
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-08 19:34:53.593047 psij-python-0.9.6/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1221 2024-04-08 19:34:25.000000 psij-python-0.9.6/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.585047 psij-python-0.9.6/src/
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3577 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      243 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/__main__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4766 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/_plugins.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4875 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3003 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/exceptions.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/executors/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      341 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/__init__.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/executors/batch/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       86 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    31379 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/batch_scheduler_executor.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/executors/batch/cobalt/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1769 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/cobalt/cobalt.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5704 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/cobalt.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      807 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/escape_functions.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/executors/batch/lsf/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1824 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/lsf/lsf.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6177 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/lsf.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/executors/batch/pbs/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1596 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/pbs/pbs_classic.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1685 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/pbs/pbspro.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)      988 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/pbs.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7118 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/pbs_base.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1138 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/pbs_classic.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3248 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/script_generator.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/executors/batch/slurm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3235 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/slurm/slurm.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)     9839 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/slurm.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2343 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/template_function_library.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7359 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/flux.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    15054 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/local.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6220 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/rp.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    10706 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6367 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_attributes.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    14194 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_executor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2721 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_executor_config.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4624 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_launcher.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    12790 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_spec.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4985 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_state.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1995 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_status.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4280 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launcher.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.593047 psij-python-0.9.6/src/psij/launchers/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      623 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      557 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/aprun.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      554 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/jsrun.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      692 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/mpirun.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1718 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/multiple.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     8023 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/script_based_launcher.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.593047 psij-python-0.9.6/src/psij/launchers/scripts/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       69 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      300 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/aprun_launch.sh
+-rwxrwxr-x   0 mike      (1000) mike      (1000)      307 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/jsrun_launch.sh
+-rwxrwxr-x   0 mike      (1000) mike      (1000)      812 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/launcher_lib.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      546 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/mpi_launch.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      594 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/multi_launch.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      236 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/single_launch.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      274 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/srun_launch.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      643 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/single.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      660 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/srun.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/py.typed
+-rw-rw-r--   0 mike      (1000) mike      (1000)     9052 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/resource_spec.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    10549 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/serialize.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1881 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/utils.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      168 2024-04-08 19:34:50.000000 psij-python-0.9.6/src/psij/version.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij-descriptors/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      217 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/aprun_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      262 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/cobalt_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      616 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/core_descriptors.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      248 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/flux_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      216 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/jsrun_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      250 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/lsf_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      564 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/pbs_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      285 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/rp_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      258 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/slurm_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      214 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/srun_descriptor.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.593047 psij-python-0.9.6/src/psij_python.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      399 2024-04-08 19:34:53.000000 psij-python-0.9.6/src/psij_python.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2821 2024-04-08 19:34:53.000000 psij-python-0.9.6/src/psij_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-08 19:34:53.000000 psij-python-0.9.6/src/psij_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       88 2024-04-08 19:34:53.000000 psij-python-0.9.6/src/psij_python.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       22 2024-04-08 19:34:53.000000 psij-python-0.9.6/src/psij_python.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.593047 psij-python-0.9.6/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2192 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_callbacks.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4938 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_doc_examples.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7986 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_executor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      994 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_executor_loading.py
+-rwxrwxr-x   0 mike      (1000) mike      (1000)      316 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_executor_versions.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      610 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_infrastructure.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_issue_387_1.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_issue_387_2.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_issue_387_3.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      589 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_issue_435.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1606 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_job_spec.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2159 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_mpi.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1209 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_nodefile.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3289 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_resources.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      836 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_serialization.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      911 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_wait.py
```

### Comparing `psij-python-0.9.5/LICENSE` & `psij-python-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/README.md` & `psij-python-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/setup.py` & `psij-python-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/__init__.py` & `psij-python-0.9.6/src/psij/__init__.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/_plugins.py` & `psij-python-0.9.6/src/psij/_plugins.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/descriptor.py` & `psij-python-0.9.6/src/psij/descriptor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/exceptions.py` & `psij-python-0.9.6/src/psij/exceptions.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/batch_scheduler_executor.py` & `psij-python-0.9.6/src/psij/executors/batch/batch_scheduler_executor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/cobalt/cobalt.mustache` & `psij-python-0.9.6/src/psij/executors/batch/cobalt/cobalt.mustache`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/cobalt.py` & `psij-python-0.9.6/src/psij/executors/batch/cobalt.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/escape_functions.py` & `psij-python-0.9.6/src/psij/executors/batch/escape_functions.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/lsf/lsf.mustache` & `psij-python-0.9.6/src/psij/executors/batch/lsf/lsf.mustache`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/lsf.py` & `psij-python-0.9.6/src/psij/executors/batch/lsf.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/pbs/pbs_classic.mustache` & `psij-python-0.9.6/src/psij/executors/batch/pbs/pbs_classic.mustache`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/pbs/pbspro.mustache` & `psij-python-0.9.6/src/psij/executors/batch/pbs/pbspro.mustache`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/pbs.py` & `psij-python-0.9.6/src/psij/executors/batch/pbs.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/pbs_base.py` & `psij-python-0.9.6/src/psij/executors/batch/pbs_base.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/pbs_classic.py` & `psij-python-0.9.6/src/psij/executors/batch/pbs_classic.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/script_generator.py` & `psij-python-0.9.6/src/psij/executors/batch/script_generator.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/slurm/slurm.mustache` & `psij-python-0.9.6/src/psij/executors/batch/slurm/slurm.mustache`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/slurm.py` & `psij-python-0.9.6/src/psij/executors/batch/slurm.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/batch/template_function_library.py` & `psij-python-0.9.6/src/psij/executors/batch/template_function_library.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/flux.py` & `psij-python-0.9.6/src/psij/executors/flux.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/local.py` & `psij-python-0.9.6/src/psij/executors/local.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/executors/rp.py` & `psij-python-0.9.6/src/psij/executors/rp.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/job.py` & `psij-python-0.9.6/src/psij/job.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/job_attributes.py` & `psij-python-0.9.6/src/psij/job_attributes.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/job_executor.py` & `psij-python-0.9.6/src/psij/job_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from abc import ABC, abstractmethod
-from distutils.version import Version
+from packaging.version import Version
 from threading import RLock
 from typing import Optional, Dict, List, Type, cast, Union, Callable, Set
 
 import psij
 from psij import InvalidJobException
 from psij.descriptor import Descriptor, _VersionEntry
 from psij._plugins import _register_plugin, _get_plugin_class, _print_plugin_status
```

### Comparing `psij-python-0.9.5/src/psij/job_executor_config.py` & `psij-python-0.9.6/src/psij/job_executor_config.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/job_launcher.py` & `psij-python-0.9.6/src/psij/job_launcher.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/job_spec.py` & `psij-python-0.9.6/src/psij/job_spec.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/job_state.py` & `psij-python-0.9.6/src/psij/job_state.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/job_status.py` & `psij-python-0.9.6/src/psij/job_status.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/launcher.py` & `psij-python-0.9.6/src/psij/launcher.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/launchers/__init__.py` & `psij-python-0.9.6/src/psij/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/launchers/aprun.py` & `psij-python-0.9.6/src/psij/launchers/aprun.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/launchers/jsrun.py` & `psij-python-0.9.6/src/psij/launchers/jsrun.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/launchers/mpirun.py` & `psij-python-0.9.6/src/psij/launchers/mpirun.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/launchers/multiple.py` & `psij-python-0.9.6/src/psij/launchers/multiple.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/launchers/script_based_launcher.py` & `psij-python-0.9.6/src/psij/launchers/script_based_launcher.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/launchers/scripts/launcher_lib.sh` & `psij-python-0.9.6/src/psij/launchers/scripts/launcher_lib.sh`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/launchers/scripts/mpi_launch.sh` & `psij-python-0.9.6/src/psij/launchers/scripts/mpi_launch.sh`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/launchers/scripts/multi_launch.sh` & `psij-python-0.9.6/src/psij/launchers/scripts/multi_launch.sh`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/launchers/single.py` & `psij-python-0.9.6/src/psij/launchers/single.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/launchers/srun.py` & `psij-python-0.9.6/src/psij/launchers/srun.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/resource_spec.py` & `psij-python-0.9.6/src/psij/resource_spec.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/serialize.py` & `psij-python-0.9.6/src/psij/serialize.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij/utils.py` & `psij-python-0.9.6/src/psij/utils.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij-descriptors/core_descriptors.py` & `psij-python-0.9.6/src/psij-descriptors/core_descriptors.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij-descriptors/pbs_descriptor.py` & `psij-python-0.9.6/src/psij-descriptors/pbs_descriptor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/src/psij_python.egg-info/SOURCES.txt` & `psij-python-0.9.6/src/psij_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/tests/test_callbacks.py` & `psij-python-0.9.6/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/tests/test_doc_examples.py` & `psij-python-0.9.6/tests/test_doc_examples.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/tests/test_executor.py` & `psij-python-0.9.6/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/tests/test_executor_loading.py` & `psij-python-0.9.6/tests/test_executor_loading.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/tests/test_infrastructure.py` & `psij-python-0.9.6/tests/test_infrastructure.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/tests/test_issue_435.py` & `psij-python-0.9.6/tests/test_issue_435.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/tests/test_job_spec.py` & `psij-python-0.9.6/tests/test_job_spec.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/tests/test_mpi.py` & `psij-python-0.9.6/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/tests/test_nodefile.py` & `psij-python-0.9.6/tests/test_nodefile.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/tests/test_resources.py` & `psij-python-0.9.6/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/tests/test_serialization.py` & `psij-python-0.9.6/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.5/tests/test_wait.py` & `psij-python-0.9.6/tests/test_wait.py`

 * *Files identical despite different names*

