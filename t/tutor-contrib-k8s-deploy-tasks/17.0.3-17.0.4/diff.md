# Comparing `tmp/tutor-contrib-k8s-deploy-tasks-17.0.3.tar.gz` & `tmp/tutor-contrib-k8s-deploy-tasks-17.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-k8s-deploy-tasks-17.0.3.tar", last modified: Wed Jan 10 18:12:38 2024, max compression
+gzip compressed data, was "tutor-contrib-k8s-deploy-tasks-17.0.4.tar", last modified: Mon Apr  8 14:10:44 2024, max compression
```

## Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3.tar` & `tutor-contrib-k8s-deploy-tasks-17.0.4.tar`

### file list

```diff
@@ -1,107 +1,121 @@
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.044715 tutor-contrib-k8s-deploy-tasks-17.0.3/
--rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-12-18 17:50:08.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/LICENSE
--rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/MANIFEST.in
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4014 2024-01-10 18:12:38.044654 tutor-contrib-k8s-deploy-tasks-17.0.3/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2694 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/README.rst
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.021312 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.021366 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.021419 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.021472 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.024267 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/
--rwxr-xr-x   0 mcdaniel   (501) staff       (20)     1250 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/gyp_main.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.021741 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.033107 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/
--rw-r--r--   0 mcdaniel   (501) staff       (20)    13029 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     6739 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    45344 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py
--rwxr-xr-x   0 mcdaniel   (501) staff       (20)    74297 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     1789 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5333 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUserFile.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    10231 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUtil.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    19742 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSVersion.py
--rwxr-xr-x   0 mcdaniel   (501) staff       (20)    24134 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    22667 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common.py
--rwxr-xr-x   0 mcdaniel   (501) staff       (20)     2162 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common_test.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5425 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml.py
--rwxr-xr-x   0 mcdaniel   (501) staff       (20)     3950 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml_test.py
--rwxr-xr-x   0 mcdaniel   (501) staff       (20)     1886 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/flock_tool.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.038111 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    31562 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/analyzer.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    49956 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/android.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    49196 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/cmake.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4704 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/compile_commands_json.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     3101 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/dump_dependency_json.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    17501 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/eclipse.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     3505 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypd.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     1713 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypsh.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)   110262 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)   150989 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py
--rwxr-xr-x   0 mcdaniel   (501) staff       (20)     1266 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)   118347 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     1910 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    66020 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)      672 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)   126319 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input.py
--rwxr-xr-x   0 mcdaniel   (501) staff       (20)     3425 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input_test.py
--rwxr-xr-x   0 mcdaniel   (501) staff       (20)    30260 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/mac_tool.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    54133 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/msvs_emulation.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5640 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/ninja_syntax.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     1293 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/simple_copy.py
--rwxr-xr-x   0 mcdaniel   (501) staff       (20)    15131 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/win_tool.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    81728 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_emulation.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    12124 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_ninja.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)   135641 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2245 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xml_fix.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.041006 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/
--rw-r--r--   0 mcdaniel   (501) staff       (20)      501 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     3266 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_elffile.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     9526 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_manylinux.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2676 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_musllinux.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    10382 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_parser.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     1431 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_structures.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5292 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_tokenizer.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     8208 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/markers.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    33036 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/metadata.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/py.typed
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2952 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/requirements.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    39969 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/specifiers.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    18355 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/tags.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5268 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/utils.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    16236 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/version.py
--rwxr-xr-x   0 mcdaniel   (501) staff       (20)     7691 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/test_gyp.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)      278 2024-01-02 23:23:21.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/pyproject.toml
--rw-r--r--   0 mcdaniel   (501) staff       (20)       67 2024-01-10 18:12:38.044914 tutor-contrib-k8s-deploy-tasks-17.0.3/setup.cfg
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2118 2024-01-04 01:26:04.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/setup.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.044422 tutor-contrib-k8s-deploy-tasks-17.0.3/tutor_contrib_k8s_deploy_tasks.egg-info/
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4014 2024-01-10 18:12:37.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutor_contrib_k8s_deploy_tasks.egg-info/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5318 2024-01-10 18:12:38.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutor_contrib_k8s_deploy_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2024-01-10 18:12:37.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutor_contrib_k8s_deploy_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       66 2024-01-10 18:12:37.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutor_contrib_k8s_deploy_tasks.egg-info/entry_points.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       22 2024-01-10 18:12:37.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutor_contrib_k8s_deploy_tasks.egg-info/requires.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       40 2024-01-10 18:12:37.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutor_contrib_k8s_deploy_tasks.egg-info/top_level.txt
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.042212 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/
--rw-r--r--   0 mcdaniel   (501) staff       (20)       23 2024-01-10 18:08:51.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/__about__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/__init__.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.042886 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/patches/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/patches/.gitignore
--rw-r--r--   0 mcdaniel   (501) staff       (20)      687 2024-01-04 01:29:27.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/patches/openedx-cms-production-settings
--rw-r--r--   0 mcdaniel   (501) staff       (20)     1505 2024-01-04 00:54:39.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/patches/openedx-lms-common-settings
--rw-r--r--   0 mcdaniel   (501) staff       (20)     3289 2024-01-10 18:02:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/patches/openedx-lms-production-settings
--rw-r--r--   0 mcdaniel   (501) staff       (20)     7845 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/plugin.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.022068 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.022262 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.043091 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/.gitignore
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.043187 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/.gitignore
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.022316 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.043288 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/.gitignore
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.043385 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/cms/
--rw-r--r--   0 mcdaniel   (501) staff       (20)       71 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/cms/nutmeg_deploy_tasks
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.043845 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2895 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/fix_oauth_redirect_uris
--rw-r--r--   0 mcdaniel   (501) staff       (20)       74 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/nutmeg_deploy_tasks
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-01-10 18:12:38.044098 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/mysql/
--rw-r--r--   0 mcdaniel   (501) staff       (20)      472 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/mysql/add_user_profiles
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.255501 tutor-contrib-k8s-deploy-tasks-17.0.4/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2024-04-08 13:40:15.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/LICENSE
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/MANIFEST.in
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4014 2024-04-08 14:10:44.255425 tutor-contrib-k8s-deploy-tasks-17.0.4/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2694 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/README.rst
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.226173 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.226230 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.226300 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.226362 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.229600 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)     1250 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/gyp_main.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.226689 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.240764 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    13029 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     6739 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    45344 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)    74297 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     1789 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5333 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUserFile.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    10231 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUtil.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    19742 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSVersion.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)    24134 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    22667 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)     2162 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common_test.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5425 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)     3950 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml_test.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)     1886 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/flock_tool.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.245692 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    31562 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/analyzer.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    49956 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/android.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    49196 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/cmake.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4704 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/compile_commands_json.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     3101 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/dump_dependency_json.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    17501 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/eclipse.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     3505 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypd.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     1713 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypsh.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)   110262 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)   150989 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)     1266 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)   118347 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     1910 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    66020 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      672 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)   126319 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)     3425 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input_test.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)    30260 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/mac_tool.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    54133 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/msvs_emulation.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5640 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/ninja_syntax.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     1293 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/simple_copy.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)    15131 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/win_tool.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    81728 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_emulation.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    12124 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_ninja.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)   135641 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2245 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xml_fix.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.248994 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      501 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     3266 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_elffile.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     9526 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_manylinux.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2676 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_musllinux.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    10382 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_parser.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     1431 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_structures.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5292 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_tokenizer.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     8208 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/markers.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    33036 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/metadata.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/py.typed
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2952 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/requirements.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    39969 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/specifiers.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    18355 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/tags.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5268 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/utils.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    16236 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/version.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)     7691 2024-01-03 01:47:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/test_gyp.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      277 2024-04-08 14:07:23.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/pyproject.toml
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       67 2024-04-08 14:10:44.255705 tutor-contrib-k8s-deploy-tasks-17.0.4/setup.cfg
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2118 2024-04-08 13:42:06.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/setup.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.255020 tutor-contrib-k8s-deploy-tasks-17.0.4/tutor_contrib_k8s_deploy_tasks.egg-info/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4014 2024-04-08 14:10:44.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutor_contrib_k8s_deploy_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5587 2024-04-08 14:10:44.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutor_contrib_k8s_deploy_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2024-04-08 14:10:44.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutor_contrib_k8s_deploy_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       66 2024-04-08 14:10:44.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutor_contrib_k8s_deploy_tasks.egg-info/entry_points.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       22 2024-04-08 14:10:44.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutor_contrib_k8s_deploy_tasks.egg-info/requires.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       45 2024-04-08 14:10:44.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutor_contrib_k8s_deploy_tasks.egg-info/top_level.txt
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.250330 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       23 2024-04-08 13:41:13.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/__about__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/__init__.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.251140 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/patches/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/patches/.gitignore
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      687 2024-04-08 13:40:15.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/patches/openedx-cms-production-settings
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     1505 2024-04-08 13:40:15.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/patches/openedx-lms-common-settings
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4869 2024-04-08 13:40:25.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/patches/openedx-lms-production-settings
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     7845 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/plugin.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.227040 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.227216 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.251644 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/.gitignore
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.251737 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/.gitignore
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.227265 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.251827 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/.gitignore
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.251930 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/cms/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       71 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/cms/nutmeg_deploy_tasks
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.252460 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2895 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/fix_oauth_redirect_uris
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       74 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/nutmeg_deploy_tasks
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.252680 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/mysql/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      472 2024-01-02 23:20:42.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/mysql/add_user_profiles
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.227646 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2024-04-08 14:10:44.254812 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)      663 2024-04-08 13:55:48.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/rst2html.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)      785 2024-04-08 13:55:48.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/rst2html4.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)     1120 2024-04-08 13:55:48.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/rst2html5.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)      862 2024-04-08 13:55:48.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/rst2latex.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)      685 2024-04-08 13:55:48.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/rst2man.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)      851 2024-04-08 13:55:48.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/rst2odt.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)      657 2024-04-08 13:55:48.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)      670 2024-04-08 13:55:48.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)      706 2024-04-08 13:55:48.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/rst2s5.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)      942 2024-04-08 13:55:48.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)      671 2024-04-08 13:55:48.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/rst2xml.py
+-rwxr-xr-x   0 mcdaniel   (501) staff       (20)      739 2024-04-08 13:55:48.000000 tutor-contrib-k8s-deploy-tasks-17.0.4/venv/bin/rstpep2html.py
```

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/LICENSE` & `tutor-contrib-k8s-deploy-tasks-17.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/PKG-INFO` & `tutor-contrib-k8s-deploy-tasks-17.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-k8s-deploy-tasks
-Version: 17.0.3
+Version: 17.0.4
 Summary: A Tutor plugin to manage deployment tasks that are exclusively (or mostly) specific to Kubernetes deployments
 Home-page: https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
 Author: Lawrence McDaniel
 Maintainer: Lawrence McDaniel
 Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
 Project-URL: Code, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
```

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/README.rst` & `tutor-contrib-k8s-deploy-tasks-17.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/gyp_main.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/gyp_main.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUserFile.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUserFile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUtil.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUtil.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSVersion.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSVersion.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/__init__.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/__init__.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common_test.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common_test.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml_test.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml_test.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/flock_tool.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/flock_tool.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/analyzer.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/analyzer.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/android.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/android.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/cmake.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/cmake.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/compile_commands_json.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/compile_commands_json.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/dump_dependency_json.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/dump_dependency_json.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/eclipse.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/eclipse.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypd.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypd.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypsh.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypsh.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input_test.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input_test.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/mac_tool.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/mac_tool.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/msvs_emulation.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/msvs_emulation.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/ninja_syntax.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/ninja_syntax.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/simple_copy.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/simple_copy.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/win_tool.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/win_tool.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_emulation.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_emulation.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_ninja.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_ninja.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xml_fix.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xml_fix.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_elffile.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_manylinux.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_musllinux.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_parser.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_structures.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_tokenizer.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/markers.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/metadata.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/requirements.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/specifiers.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/tags.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/utils.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/version.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/version.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/node_modules/npm/node_modules/node-gyp/gyp/test_gyp.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/node_modules/npm/node_modules/node-gyp/gyp/test_gyp.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/setup.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/tutor_contrib_k8s_deploy_tasks.egg-info/PKG-INFO` & `tutor-contrib-k8s-deploy-tasks-17.0.4/tutor_contrib_k8s_deploy_tasks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-k8s-deploy-tasks
-Version: 17.0.3
+Version: 17.0.4
 Summary: A Tutor plugin to manage deployment tasks that are exclusively (or mostly) specific to Kubernetes deployments
 Home-page: https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
 Author: Lawrence McDaniel
 Maintainer: Lawrence McDaniel
 Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
 Project-URL: Code, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
```

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/tutor_contrib_k8s_deploy_tasks.egg-info/SOURCES.txt` & `tutor-contrib-k8s-deploy-tasks-17.0.4/tutor_contrib_k8s_deploy_tasks.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -77,8 +77,20 @@
 tutork8s_deploy_tasks/patches/openedx-lms-production-settings
 tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/.gitignore
 tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/.gitignore
 tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/.gitignore
 tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/cms/nutmeg_deploy_tasks
 tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/fix_oauth_redirect_uris
 tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/nutmeg_deploy_tasks
-tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/mysql/add_user_profiles
+tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/mysql/add_user_profiles
+venv/bin/rst2html.py
+venv/bin/rst2html4.py
+venv/bin/rst2html5.py
+venv/bin/rst2latex.py
+venv/bin/rst2man.py
+venv/bin/rst2odt.py
+venv/bin/rst2odt_prepstyles.py
+venv/bin/rst2pseudoxml.py
+venv/bin/rst2s5.py
+venv/bin/rst2xetex.py
+venv/bin/rst2xml.py
+venv/bin/rstpep2html.py
```

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/patches/openedx-cms-production-settings` & `tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/patches/openedx-cms-production-settings`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/patches/openedx-lms-common-settings` & `tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/patches/openedx-lms-common-settings`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/plugin.py` & `tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-17.0.3/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/fix_oauth_redirect_uris` & `tutor-contrib-k8s-deploy-tasks-17.0.4/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/fix_oauth_redirect_uris`

 * *Files identical despite different names*

