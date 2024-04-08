# Comparing `tmp/cryoemservices-0.2.0.tar.gz` & `tmp/cryoemservices-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryoemservices-0.2.0.tar", last modified: Tue Mar 26 16:36:37 2024, max compression
+gzip compressed data, was "cryoemservices-0.2.1.tar", last modified: Mon Apr  8 10:55:30 2024, max compression
```

## Comparing `cryoemservices-0.2.0.tar` & `cryoemservices-0.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:37.380981 cryoemservices-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-03-26 16:36:37.380981 cryoemservices-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-26 16:36:37.380981 cryoemservices-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:37.368981 cryoemservices-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:37.372981 cryoemservices-0.2.0/src/cryoemservices/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:37.372981 cryoemservices-0.2.0/src/cryoemservices/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/cli/resubmit_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:37.372981 cryoemservices-0.2.0/src/cryoemservices/pipeliner_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/pipeliner_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/pipeliner_plugins/combine_star_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/pipeliner_plugins/combine_star_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/pipeliner_plugins/reextract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:37.376981 cryoemservices-0.2.0/src/cryoemservices/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/bfactor_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/cluster_submission.py
--rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/cryolo.py
--rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/ctffind.py
--rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/denoise_iris.py
--rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    22585 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/extract_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    21270 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/icebreaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/images_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    46671 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/ispyb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/ispyb_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27255 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/motioncorr.py
--rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/motioncorr_slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/node_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/select_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/select_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)    22165 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/tomo_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/services/tomo_align_iris.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:37.380981 cryoemservices-0.2.0/src/cryoemservices/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/util/dispatcher_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/util/spa_output_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/util/spa_relion_service_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:37.380981 cryoemservices-0.2.0/src/cryoemservices/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/wrappers/class2d_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24235 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/wrappers/class3d_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-03-26 16:36:33.000000 cryoemservices-0.2.0/src/cryoemservices/wrappers/refine3d_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:36:37.380981 cryoemservices-0.2.0/src/cryoemservices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-03-26 16:36:37.000000 cryoemservices-0.2.0/src/cryoemservices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-26 16:36:37.000000 cryoemservices-0.2.0/src/cryoemservices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:36:37.000000 cryoemservices-0.2.0/src/cryoemservices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-03-26 16:36:37.000000 cryoemservices-0.2.0/src/cryoemservices.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:36:37.000000 cryoemservices-0.2.0/src/cryoemservices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-26 16:36:37.000000 cryoemservices-0.2.0/src/cryoemservices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-26 16:36:37.000000 cryoemservices-0.2.0/src/cryoemservices.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.273920 cryoemservices-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-08 10:55:30.273920 cryoemservices-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-08 10:55:30.277920 cryoemservices-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.265920 cryoemservices-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.265920 cryoemservices-0.2.1/src/cryoemservices/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.269920 cryoemservices-0.2.1/src/cryoemservices/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/cli/resubmit_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.269920 cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/combine_star_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/combine_star_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/reextract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.273920 cryoemservices-0.2.1/src/cryoemservices/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/bfactor_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/cluster_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/cryolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/ctffind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/denoise_iris.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22665 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/extract_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21270 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/icebreaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/images_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46671 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/ispyb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/ispyb_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27255 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/motioncorr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/motioncorr_slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/node_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/select_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/select_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22102 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/tomo_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/services/tomo_align_iris.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.273920 cryoemservices-0.2.1/src/cryoemservices/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/util/dispatcher_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/util/spa_output_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/util/spa_relion_service_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.273920 cryoemservices-0.2.1/src/cryoemservices/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/wrappers/class2d_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24235 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/wrappers/class3d_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-04-08 10:55:24.000000 cryoemservices-0.2.1/src/cryoemservices/wrappers/refine3d_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:55:30.273920 cryoemservices-0.2.1/src/cryoemservices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 10:55:30.000000 cryoemservices-0.2.1/src/cryoemservices.egg-info/top_level.txt
```

### Comparing `cryoemservices-0.2.0/LICENSE` & `cryoemservices-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/PKG-INFO` & `cryoemservices-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryoemservices
-Version: 0.2.0
+Version: 0.2.1
 Summary: Services for CryoEM processing
 Author: Diamond Light Source - Data Analysis et al.
 Author-email: dataanalysis@diamond.ac.uk
 License: BSD 3-Clause
 Project-URL: GitHub, https://github.com/DiamondLightSource/cryoem-services
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/cryoem-services/issues
 Keywords: cryoem-services
@@ -28,16 +28,17 @@
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: mrcfile
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: plotly
 Requires-Dist: pydantic==1.10.7
 Requires-Dist: starfile
+Requires-Dist: stomp-py==8.1.0
 Requires-Dist: workflows
-Requires-Dist: zocalo
+Requires-Dist: zocalo==0.30.2
 
 # cryoem-services
 Services and configuration for cryo-EM pipelines.
 
 This package consists of a number of services to process cryo-EM micrographs,
 both for single particle analysis and tomography,
 using a range of commonly used cryo-EM processing software.
```

### Comparing `cryoemservices-0.2.0/README.md` & `cryoemservices-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/setup.cfg` & `cryoemservices-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cryoemservices
-version = 0.2.0
+version = 0.2.1
 description = Services for CryoEM processing
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Diamond Light Source - Data Analysis et al.
 author_email = dataanalysis@diamond.ac.uk
 license = BSD 3-Clause
 license_files = LICENSE
@@ -34,16 +34,17 @@
 	marshmallow-sqlalchemy
 	mrcfile
 	numpy
 	pillow
 	plotly
 	pydantic ==1.10.7
 	starfile
+	stomp-py ==8.1.0
 	workflows
-	zocalo
+	zocalo ==0.30.2
 packages = find:
 package_dir = 
 	=src
 python_requires = >=3.8
 zip_safe = False
 
 [options.entry_points]
```

### Comparing `cryoemservices-0.2.0/src/cryoemservices/cli/resubmit_wrapper.py` & `cryoemservices-0.2.1/src/cryoemservices/cli/resubmit_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/pipeliner_plugins/combine_star_files.py` & `cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/combine_star_files.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/pipeliner_plugins/combine_star_job.py` & `cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/combine_star_job.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/pipeliner_plugins/reextract.py` & `cryoemservices-0.2.1/src/cryoemservices/pipeliner_plugins/reextract.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/bfactor_setup.py` & `cryoemservices-0.2.1/src/cryoemservices/services/bfactor_setup.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/cluster_submission.py` & `cryoemservices-0.2.1/src/cryoemservices/services/cluster_submission.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from pydantic import BaseModel, Field
 from workflows.services.common_service import CommonService
 from zocalo.util import slurm
 
 
 class JobSubmissionParameters(BaseModel):
     scheduler: str = "slurm"
-    cluster: Optional[str]
     partition: Optional[str]
     prefer: Optional[str]
     job_name: Optional[str]
     environment: Optional[dict[str, str]] = None
     cpus_per_task: Optional[int] = None
     tasks: Optional[int] = None
     nodes: Optional[int]
@@ -31,15 +30,14 @@
     gpus_per_node: Optional[str] = None
     min_memory_per_cpu: Optional[int] = Field(
         None, description="Minimum real memory per cpu (MB)"
     )
     time_limit: Optional[datetime.timedelta] = None
     gpus: Optional[int] = None
     exclusive: bool = False
-    account: Optional[str]
     commands: str | list[str]
     qos: Optional[str]
 
 
 def submit_to_slurm(
     params: JobSubmissionParameters,
     working_directory: Path,
@@ -71,16 +69,14 @@
             memory_per_node=params.memory_per_node,
             environment=os.environ
             if params.environment is None
             else params.environment,
             memory_per_cpu=params.min_memory_per_cpu,
             time_limit=time_limit_minutes,
             gpus=params.gpus,
-            # exclusive=params.exclusive,
-            account=params.account,
             current_working_directory=os.fspath(working_directory),
             qos=params.qos,
         ),
     )
     try:
         response = api.submit_job(job_submission)
     except requests.HTTPError as e:
@@ -222,8 +218,8 @@
 
         # Send results onwards
         rw.set_default_channel("job_submitted")
         rw.send({"jobid": jobnumber}, transaction=txn)
 
         # Commit transaction
         self._transport.transaction_commit(txn)
-        self.log.info(f"Submitted job {jobnumber} to {cluster_params.cluster}")
+        self.log.info(f"Submitted job {jobnumber} to slurm")
```

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/cryolo.py` & `cryoemservices-0.2.1/src/cryoemservices/services/cryolo.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/ctffind.py` & `cryoemservices-0.2.1/src/cryoemservices/services/ctffind.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/denoise_iris.py` & `cryoemservices-0.2.1/src/cryoemservices/services/denoise_iris.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/extract.py` & `cryoemservices-0.2.1/src/cryoemservices/services/extract.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/extract_class.py` & `cryoemservices-0.2.1/src/cryoemservices/services/extract_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class ExtractClassParameters(BaseModel):
     extraction_executable: str = "cryoemservices.reextract"
     class3d_dir: str = Field(..., min_length=1)
     refine_job_dir: str = Field(..., min_length=1)
     refine_class_nr: int
     original_pixel_size: float
     boxsize: int = 150
-    nr_iter_3d: int = 20
+    nr_iter_3d: int = 25
     bg_radius: int = -1
     downscale_factor: float = 2
     downscale: bool = True
     normalise: bool = True
     invert_contrast: bool = True
     relion_options: RelionServiceOptions
 
@@ -60,14 +60,16 @@
             "set": True,
             "infinite": False,
         },
     },
 }
 slurm_script_template = (
     "#!/bin/bash\necho \"$(date '+%Y-%m-%d %H:%M:%S.%3N'): running ReExtraction\"\n"
+    "source /etc/profile.d/modules.sh\n"
+    "module load EM/cryoem-services\n"
 )
 
 
 class ExtractClass(CommonService):
     """
     A service for extracting particles from a class for refinement
     """
```

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/icebreaker.py` & `cryoemservices-0.2.1/src/cryoemservices/services/icebreaker.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/images.py` & `cryoemservices-0.2.1/src/cryoemservices/services/images.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/images_plugins.py` & `cryoemservices-0.2.1/src/cryoemservices/services/images_plugins.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/ispyb.py` & `cryoemservices-0.2.1/src/cryoemservices/services/ispyb.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/ispyb_buffer.py` & `cryoemservices-0.2.1/src/cryoemservices/services/ispyb_buffer.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/motioncorr.py` & `cryoemservices-0.2.1/src/cryoemservices/services/motioncorr.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/motioncorr_slurm.py` & `cryoemservices-0.2.1/src/cryoemservices/services/motioncorr_slurm.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/node_creator.py` & `cryoemservices-0.2.1/src/cryoemservices/services/node_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,21 +101,21 @@
         "input_stars": {
             "fn_img": "particles_split1.star",
             "fn_ref": "initial_model.mrc",
         },
     },
     "relion.select.onvalue": {
         "folder": "Select",
-        "input_stars": {"fn_data": "run_it020_data.star"},
+        "input_stars": {"fn_data": "run_it025_data.star"},
     },
     "relion.refine3d": {
         "folder": "Refine3D",
         "input_stars": {
             "fn_img": "particles_split1.star",
-            "fn_ref": "run_it020_class.mrc",
+            "fn_ref": "run_it025_class.mrc",
         },
     },
     "relion.maskcreate": {
         "folder": "MaskCreate",
         "input_stars": {"fn_in": "run_class001.star"},
     },
     "relion.postprocess": {
```

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/postprocess.py` & `cryoemservices-0.2.1/src/cryoemservices/services/postprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import os
+import shutil
 import subprocess
 from pathlib import Path
 
 import numpy as np
 import workflows.recipe
 from gemmi import cif
 from pydantic import BaseModel, Field, ValidationError
@@ -178,14 +179,23 @@
                 "Refinement post-process failed with exitcode "
                 f"{postprocess_result.returncode}:\n"
                 + postprocess_result.stderr.decode("utf8", "replace")
             )
             rw.transport.nack(header)
             return
 
+        # Copy the angular distribution from Refinement
+        refine_angdist = (
+            Path(postprocess_params.half_map).parent / "run_class001_angdist.jpeg"
+        )
+        if refine_angdist.is_file():
+            shutil.copy(
+                refine_angdist, f"{postprocess_params.job_dir}/postprocess_angdist.jpeg"
+            )
+
         # Get the bfactor and resolution from the postprocessing output
         # Should this be interpolated??
         postprocess_lines = postprocess_result.stdout.decode("utf8", "replace").split(
             "\n"
         )
         final_bfactor = None
         final_resolution = None
@@ -323,15 +333,15 @@
 
         # Tell Murfey the refinement has finished
         if postprocess_params.is_first_refinement:
             murfey_postprocess_params = {
                 "register": "done_refinement",
                 "project_dir": str(project_dir),
                 "resolution": final_resolution,
-                "batch_size": postprocess_params.number_of_particles,
+                "number_of_particles": postprocess_params.number_of_particles,
                 "refined_grp_uuid": postprocess_params.refined_grp_uuid,
                 "refined_class_uuid": postprocess_params.refined_class_uuid,
                 "class_reference": postprocess_params.rescaled_class_reference,
                 "class_number": postprocess_params.class_number,
                 "mask_file": postprocess_params.mask,
                 "pixel_size": postprocess_params.pixel_size,
             }
```

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/select_classes.py` & `cryoemservices-0.2.1/src/cryoemservices/services/select_classes.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/select_particles.py` & `cryoemservices-0.2.1/src/cryoemservices/services/select_particles.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/tomo_align.py` & `cryoemservices-0.2.1/src/cryoemservices/services/tomo_align.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,14 @@
         try:
             if isinstance(message, dict):
                 tomo_params = TomoParameters(
                     **{**rw.recipe_step.get("parameters", {}), **message}
                 )
             else:
                 tomo_params = TomoParameters(**{**rw.recipe_step.get("parameters", {})})
-            tomo_params.pix_size = tomo_params.pix_size * 1e10
         except (ValidationError, TypeError) as e:
             self.log.warning(
                 f"TomoAlign parameter validation failed for message: {message} "
                 f"and recipe parameters: {rw.recipe_step.get('parameters', {})} "
                 f"with exception: {e}"
             )
             rw.transport.nack(header)
```

### Comparing `cryoemservices-0.2.0/src/cryoemservices/services/tomo_align_iris.py` & `cryoemservices-0.2.1/src/cryoemservices/services/tomo_align_iris.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/util/dispatcher_tools.py` & `cryoemservices-0.2.1/src/cryoemservices/util/dispatcher_tools.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/util/spa_output_files.py` & `cryoemservices-0.2.1/src/cryoemservices/util/spa_output_files.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/util/spa_relion_service_options.py` & `cryoemservices-0.2.1/src/cryoemservices/util/spa_relion_service_options.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/wrappers/class2d_wrapper.py` & `cryoemservices-0.2.1/src/cryoemservices/wrappers/class2d_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/wrappers/class3d_wrapper.py` & `cryoemservices-0.2.1/src/cryoemservices/wrappers/class3d_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices/wrappers/refine3d_wrapper.py` & `cryoemservices-0.2.1/src/cryoemservices/wrappers/refine3d_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     rescaled_class_reference: str = Field(..., min_length=1)
     rescaling_command: List[str] = []
     is_first_refinement: bool
     number_of_particles: int
     batch_size: int
     pixel_size: float
     class_number: int
-    mask_diameter: float
+    particle_diameter: float = 0
+    mask_diameter: float = 190
     mask: Optional[str] = None
     mask_lowpass: float = 15
     mask_threshold_fraction: float = 0.2
     mask_extend: int = 3
     mask_soft_edge: int = 3
     mpi_run_command: str = "srun -n 5"
     dont_correct_greyscale: bool = True
@@ -143,15 +144,15 @@
                 "--i",
                 str(refine_params.particles_file),
                 "--o",
                 f"{refine_params.refine_job_dir}/run",
                 "--ref",
                 str(refine_params.rescaled_class_reference),
                 "--particle_diameter",
-                f"{refine_params.mask_diameter}",
+                f"{refine_params.relion_options.mask_diameter}",
                 "--auto_refine",
                 "--split_random_halves",
             ]
         )
 
         # Add flags to the command based on the input parameters
         refine_flags = {
```

### Comparing `cryoemservices-0.2.0/src/cryoemservices.egg-info/PKG-INFO` & `cryoemservices-0.2.1/src/cryoemservices.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryoemservices
-Version: 0.2.0
+Version: 0.2.1
 Summary: Services for CryoEM processing
 Author: Diamond Light Source - Data Analysis et al.
 Author-email: dataanalysis@diamond.ac.uk
 License: BSD 3-Clause
 Project-URL: GitHub, https://github.com/DiamondLightSource/cryoem-services
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/cryoem-services/issues
 Keywords: cryoem-services
@@ -28,16 +28,17 @@
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: mrcfile
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: plotly
 Requires-Dist: pydantic==1.10.7
 Requires-Dist: starfile
+Requires-Dist: stomp-py==8.1.0
 Requires-Dist: workflows
-Requires-Dist: zocalo
+Requires-Dist: zocalo==0.30.2
 
 # cryoem-services
 Services and configuration for cryo-EM pipelines.
 
 This package consists of a number of services to process cryo-EM micrographs,
 both for single particle analysis and tomography,
 using a range of commonly used cryo-EM processing software.
```

### Comparing `cryoemservices-0.2.0/src/cryoemservices.egg-info/SOURCES.txt` & `cryoemservices-0.2.1/src/cryoemservices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.0/src/cryoemservices.egg-info/entry_points.txt` & `cryoemservices-0.2.1/src/cryoemservices.egg-info/entry_points.txt`

 * *Files identical despite different names*

