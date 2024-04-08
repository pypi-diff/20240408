# Comparing `tmp/libbs-1.2.2.tar.gz` & `tmp/libbs-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbs-1.2.2.tar", last modified: Fri Apr  5 00:50:29 2024, max compression
+gzip compressed data, was "libbs-1.2.3.tar", last modified: Mon Apr  8 17:26:37 2024, max compression
```

## Comparing `libbs-1.2.2.tar` & `libbs-1.2.3.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.882559 libbs-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-05 00:50:25.000000 libbs-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-05 00:50:29.882559 libbs-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-05 00:50:25.000000 libbs-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.870559 libbs-1.2.2/libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.874559 libbs-1.2.2/libbs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/api/artifact_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/api/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/api/decompiler_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/api/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.874559 libbs-1.2.2/libbs/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/decompilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/stack_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.874559 libbs-1.2.2/libbs/decompiler_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.874559 libbs-1.2.2/libbs/decompiler_stubs/angr_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/angr_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.874559 libbs-1.2.2/libbs/decompiler_stubs/binja_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/binja_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ida_libbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompilers/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/angr/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/angr/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/binja/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/binja/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/artifact_lifter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.882559 libbs-1.2.2/libbs/decompilers/ghidra/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/compat/ghidra_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/compat/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    32537 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.882559 libbs-1.2.2/libbs/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ida/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ida/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ida/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/plugin_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.882559 libbs-1.2.2/libbs/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.882559 libbs-1.2.2/libbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-05 00:50:29.000000 libbs-1.2.2/libbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-05 00:50:29.000000 libbs-1.2.2/libbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:50:29.000000 libbs-1.2.2/libbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 00:50:29.000000 libbs-1.2.2/libbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 00:50:29.000000 libbs-1.2.2/libbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 00:50:29.000000 libbs-1.2.2/libbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-05 00:50:29.882559 libbs-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 00:50:25.000000 libbs-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.882559 libbs-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-05 00:50:25.000000 libbs-1.2.2/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-05 00:50:25.000000 libbs-1.2.2/tests/test_decompilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.242225 libbs-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-08 17:26:30.000000 libbs-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-08 17:26:37.242225 libbs-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-08 17:26:30.000000 libbs-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.230224 libbs-1.2.3/libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.234225 libbs-1.2.3/libbs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/api/artifact_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/api/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/api/decompiler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/api/type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.234225 libbs-1.2.3/libbs/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/artifacts/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/artifacts/decompilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/artifacts/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/artifacts/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/artifacts/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/artifacts/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/artifacts/stack_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/artifacts/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.234225 libbs-1.2.3/libbs/decompiler_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.234225 libbs-1.2.3/libbs/decompiler_stubs/angr_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/angr_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.234225 libbs-1.2.3/libbs/decompiler_stubs/binja_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/binja_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.238225 libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.238225 libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.238225 libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompiler_stubs/ida_libbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.238225 libbs-1.2.3/libbs/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.238225 libbs-1.2.3/libbs/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/angr/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/angr/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.238225 libbs-1.2.3/libbs/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/binja/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/binja/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.238225 libbs-1.2.3/libbs/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/ghidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/ghidra/artifact_lifter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.242225 libbs-1.2.3/libbs/decompilers/ghidra/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/ghidra/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/ghidra/compat/ghidra_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/ghidra/compat/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/ghidra/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32537 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/ghidra/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.242225 libbs-1.2.3/libbs/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/ida/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/ida/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/decompilers/ida/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/plugin_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.242225 libbs-1.2.3/libbs/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-08 17:26:30.000000 libbs-1.2.3/libbs/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.242225 libbs-1.2.3/libbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-08 17:26:37.000000 libbs-1.2.3/libbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-08 17:26:37.000000 libbs-1.2.3/libbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:26:37.000000 libbs-1.2.3/libbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 17:26:37.000000 libbs-1.2.3/libbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 17:26:37.000000 libbs-1.2.3/libbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 17:26:37.000000 libbs-1.2.3/libbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-08 17:26:37.246224 libbs-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 17:26:30.000000 libbs-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:26:37.242225 libbs-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-08 17:26:30.000000 libbs-1.2.3/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-08 17:26:30.000000 libbs-1.2.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-08 17:26:30.000000 libbs-1.2.3/tests/test_decompilers.py
```

### Comparing `libbs-1.2.2/LICENSE` & `libbs-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/PKG-INFO` & `libbs-1.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.2.2
+Version: 1.2.3
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toml
 Requires-Dist: pycparser
 Requires-Dist: setuptools
 Requires-Dist: prompt_toolkit
 Requires-Dist: tqdm
```

### Comparing `libbs-1.2.2/README.md` & `libbs-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/__main__.py` & `libbs-1.2.3/libbs/__main__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/api/artifact_dict.py` & `libbs-1.2.3/libbs/api/artifact_dict.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/api/artifact_lifter.py` & `libbs-1.2.3/libbs/api/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/api/decompiler_interface.py` & `libbs-1.2.3/libbs/api/decompiler_interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/api/type_parser.py` & `libbs-1.2.3/libbs/api/type_parser.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/api/utils.py` & `libbs-1.2.3/libbs/api/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/artifacts/artifact.py` & `libbs-1.2.3/libbs/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/artifacts/comment.py` & `libbs-1.2.3/libbs/artifacts/comment.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/artifacts/decompilation.py` & `libbs-1.2.3/libbs/artifacts/decompilation.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/artifacts/enum.py` & `libbs-1.2.3/libbs/artifacts/enum.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/artifacts/func.py` & `libbs-1.2.3/libbs/artifacts/func.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/artifacts/global_variable.py` & `libbs-1.2.3/libbs/artifacts/global_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/artifacts/patch.py` & `libbs-1.2.3/libbs/artifacts/patch.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/artifacts/stack_variable.py` & `libbs-1.2.3/libbs/artifacts/stack_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/artifacts/struct.py` & `libbs-1.2.3/libbs/artifacts/struct.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py` & `libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py` & `libbs-1.2.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/angr/artifact_lifter.py` & `libbs-1.2.3/libbs/decompilers/angr/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/angr/compat.py` & `libbs-1.2.3/libbs/decompilers/angr/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/angr/interface.py` & `libbs-1.2.3/libbs/decompilers/angr/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/binja/artifact_lifter.py` & `libbs-1.2.3/libbs/decompilers/binja/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/binja/hooks.py` & `libbs-1.2.3/libbs/decompilers/binja/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/binja/interface.py` & `libbs-1.2.3/libbs/decompilers/binja/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/ghidra/artifact_lifter.py` & `libbs-1.2.3/libbs/decompilers/ghidra/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/ghidra/compat/ghidra_api.py` & `libbs-1.2.3/libbs/decompilers/ghidra/compat/ghidra_api.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/ghidra/hooks.py` & `libbs-1.2.3/libbs/decompilers/ghidra/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/ghidra/interface.py` & `libbs-1.2.3/libbs/decompilers/ghidra/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/ida/artifact_lifter.py` & `libbs-1.2.3/libbs/decompilers/ida/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/ida/compat.py` & `libbs-1.2.3/libbs/decompilers/ida/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/ida/hooks.py` & `libbs-1.2.3/libbs/decompilers/ida/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/decompilers/ida/interface.py` & `libbs-1.2.3/libbs/decompilers/ida/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/logger.py` & `libbs-1.2.3/libbs/logger.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/plugin_installer.py` & `libbs-1.2.3/libbs/plugin_installer.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/ui/__init__.py` & `libbs-1.2.3/libbs/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/ui/qt_objects.py` & `libbs-1.2.3/libbs/ui/qt_objects.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs/ui/utils.py` & `libbs-1.2.3/libbs/ui/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/libbs.egg-info/PKG-INFO` & `libbs-1.2.3/libbs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.2.2
+Version: 1.2.3
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toml
 Requires-Dist: pycparser
 Requires-Dist: setuptools
 Requires-Dist: prompt_toolkit
 Requires-Dist: tqdm
```

### Comparing `libbs-1.2.2/libbs.egg-info/SOURCES.txt` & `libbs-1.2.3/libbs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,8 +63,9 @@
 libbs/decompilers/ida/hooks.py
 libbs/decompilers/ida/interface.py
 libbs/ui/__init__.py
 libbs/ui/qt_objects.py
 libbs/ui/utils.py
 libbs/ui/version.py
 tests/test_artifacts.py
+tests/test_cli.py
 tests/test_decompilers.py
```

### Comparing `libbs-1.2.2/setup.cfg` & `libbs-1.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = libbs
 version = attr: libbs.__version__
 url = https://github.com/binsync/libbs
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.7
 license = BSD 2 Clause
 license_files = LICENSE
 description = Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
@@ -18,15 +18,15 @@
 	pycparser
 	setuptools
 	prompt_toolkit
 	tqdm
 	jfx_bridge
 	ghidra_bridge
 	psutil
-python_requires = >= 3.8
+python_requires = >= 3.7
 include_package_data = True
 packages = find:
 
 [options.entry_points]
 console_scripts = 
 	libbs = libbs.__main__:main
```

### Comparing `libbs-1.2.2/tests/test_artifacts.py` & `libbs-1.2.3/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.2/tests/test_decompilers.py` & `libbs-1.2.3/tests/test_decompilers.py`

 * *Files identical despite different names*

