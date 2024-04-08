# Comparing `tmp/fake-bpy-module-latest-20240407.tar.gz` & `tmp/fake-bpy-module-latest-20240408.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fake-bpy-module-latest-20240407.tar", last modified: Sun Apr  7 06:12:19 2024, max compression
+gzip compressed data, was "fake-bpy-module-latest-20240408.tar", last modified: Mon Apr  8 06:13:21 2024, max compression
```

## Comparing `fake-bpy-module-latest-20240407.tar` & `fake-bpy-module-latest-20240408.tar`

### file list

```diff
@@ -1,905 +1,905 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.386709 fake-bpy-module-latest-20240407/
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-07 06:12:19.386709 fake-bpy-module-latest-20240407/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-07 06:12:16.000000 fake-bpy-module-latest-20240407/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.282709 fake-bpy-module-latest-20240407/addon_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-07 06:11:50.000000 fake-bpy-module-latest-20240407/addon_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/addon_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.282709 fake-bpy-module-latest-20240407/animsys_refactor/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-07 06:11:50.000000 fake-bpy-module-latest-20240407/animsys_refactor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/animsys_refactor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.282709 fake-bpy-module-latest-20240407/aud/
--rw-r--r--   0 runner    (1001) docker     (127)    30520 2024-04-07 06:11:36.000000 fake-bpy-module-latest-20240407/aud/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/aud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.282709 fake-bpy-module-latest-20240407/bgl/
--rw-r--r--   0 runner    (1001) docker     (127)   105957 2024-04-07 06:11:32.000000 fake-bpy-module-latest-20240407/bgl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bgl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.282709 fake-bpy-module-latest-20240407/bl_app_override/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-07 06:11:50.000000 fake-bpy-module-latest-20240407/bl_app_override/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.282709 fake-bpy-module-latest-20240407/bl_app_override/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-07 06:11:50.000000 fake-bpy-module-latest-20240407/bl_app_override/helpers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_app_override/helpers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_app_override/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.282709 fake-bpy-module-latest-20240407/bl_app_template_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-07 06:11:48.000000 fake-bpy-module-latest-20240407/bl_app_template_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_app_template_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.282709 fake-bpy-module-latest-20240407/bl_console_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-07 06:11:48.000000 fake-bpy-module-latest-20240407/bl_console_utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-07 06:11:48.000000 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/complete_calltip/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 06:11:48.000000 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/complete_calltip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/complete_calltip/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/complete_import/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-07 06:11:48.000000 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/complete_import/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/complete_import/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/complete_namespace/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-07 06:11:48.000000 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/complete_namespace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/complete_namespace/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/intellisense/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-07 06:11:48.000000 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/intellisense/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/intellisense/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_console_utils/autocomplete/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_console_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_i18n_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-07 06:11:49.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_i18n_utils/bl_extract_messages/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-07 06:11:50.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/bl_extract_messages/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/bl_extract_messages/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_i18n_utils/merge_po/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 06:11:50.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/merge_po/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/merge_po/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_i18n_utils/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-07 06:11:50.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/settings/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/settings/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_i18n_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-07 06:11:49.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_i18n_utils/utils_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-07 06:11:50.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/utils_cli/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/utils_cli/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_i18n_utils/utils_languages_menu/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-07 06:11:49.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/utils_languages_menu/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/utils_languages_menu/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.286708 fake-bpy-module-latest-20240407/bl_i18n_utils/utils_rtl/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-07 06:11:49.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/utils_rtl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_i18n_utils/utils_rtl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_keymap_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-07 06:11:49.000000 fake-bpy-module-latest-20240407/bl_keymap_utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_keymap_utils/io/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-07 06:11:49.000000 fake-bpy-module-latest-20240407/bl_keymap_utils/io/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_keymap_utils/io/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_keymap_utils/keymap_from_toolbar/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-07 06:11:49.000000 fake-bpy-module-latest-20240407/bl_keymap_utils/keymap_from_toolbar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_keymap_utils/keymap_from_toolbar/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_keymap_utils/keymap_hierarchy/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-07 06:11:49.000000 fake-bpy-module-latest-20240407/bl_keymap_utils/keymap_hierarchy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_keymap_utils/keymap_hierarchy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_keymap_utils/platform_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-07 06:11:49.000000 fake-bpy-module-latest-20240407/bl_keymap_utils/platform_helpers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_keymap_utils/platform_helpers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_keymap_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_keymap_utils/versioning/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-07 06:11:49.000000 fake-bpy-module-latest-20240407/bl_keymap_utils/versioning/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_keymap_utils/versioning/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_math/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-07 06:11:37.000000 fake-bpy-module-latest-20240407/bl_math/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_math/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_operators/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-07 06:11:45.000000 fake-bpy-module-latest-20240407/bl_operators/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_operators/add_mesh_torus/
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-07 06:11:46.000000 fake-bpy-module-latest-20240407/bl_operators/add_mesh_torus/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/add_mesh_torus/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_operators/anim/
--rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-04-07 06:11:47.000000 fake-bpy-module-latest-20240407/bl_operators/anim/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/anim/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_operators/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-07 06:11:46.000000 fake-bpy-module-latest-20240407/bl_operators/assets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/assets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_operators/bmesh/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 06:11:48.000000 fake-bpy-module-latest-20240407/bl_operators/bmesh/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.290708 fake-bpy-module-latest-20240407/bl_operators/bmesh/find_adjacent/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-07 06:11:48.000000 fake-bpy-module-latest-20240407/bl_operators/bmesh/find_adjacent/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/bmesh/find_adjacent/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/bmesh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.294708 fake-bpy-module-latest-20240407/bl_operators/clip/
--rw-r--r--   0 runner    (1001) docker     (127)    20846 2024-04-07 06:11:46.000000 fake-bpy-module-latest-20240407/bl_operators/clip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/clip/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.294708 fake-bpy-module-latest-20240407/bl_operators/console/
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-04-07 06:11:47.000000 fake-bpy-module-latest-20240407/bl_operators/console/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/console/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.294708 fake-bpy-module-latest-20240407/bl_operators/constraint/
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-07 06:11:47.000000 fake-bpy-module-latest-20240407/bl_operators/constraint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/constraint/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.294708 fake-bpy-module-latest-20240407/bl_operators/file/
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-04-07 06:11:46.000000 fake-bpy-module-latest-20240407/bl_operators/file/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/file/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.294708 fake-bpy-module-latest-20240407/bl_operators/freestyle/
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-04-07 06:11:45.000000 fake-bpy-module-latest-20240407/bl_operators/freestyle/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/freestyle/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.294708 fake-bpy-module-latest-20240407/bl_operators/geometry_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)    36068 2024-04-07 06:11:47.000000 fake-bpy-module-latest-20240407/bl_operators/geometry_nodes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/geometry_nodes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.294708 fake-bpy-module-latest-20240407/bl_operators/image/
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-07 06:11:47.000000 fake-bpy-module-latest-20240407/bl_operators/image/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/image/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.294708 fake-bpy-module-latest-20240407/bl_operators/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-07 06:11:46.000000 fake-bpy-module-latest-20240407/bl_operators/mesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/mesh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.294708 fake-bpy-module-latest-20240407/bl_operators/node/
--rw-r--r--   0 runner    (1001) docker     (127)    27034 2024-04-07 06:11:46.000000 fake-bpy-module-latest-20240407/bl_operators/node/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/node/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.294708 fake-bpy-module-latest-20240407/bl_operators/object/
--rw-r--r--   0 runner    (1001) docker     (127)    30487 2024-04-07 06:11:46.000000 fake-bpy-module-latest-20240407/bl_operators/object/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/object/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.294708 fake-bpy-module-latest-20240407/bl_operators/object_align/
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-07 06:11:45.000000 fake-bpy-module-latest-20240407/bl_operators/object_align/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/object_align/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.294708 fake-bpy-module-latest-20240407/bl_operators/object_quick_effects/
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-04-07 06:11:47.000000 fake-bpy-module-latest-20240407/bl_operators/object_quick_effects/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/object_quick_effects/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.298709 fake-bpy-module-latest-20240407/bl_operators/object_randomize_transform/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-07 06:11:47.000000 fake-bpy-module-latest-20240407/bl_operators/object_randomize_transform/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/object_randomize_transform/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.298709 fake-bpy-module-latest-20240407/bl_operators/presets/
--rw-r--r--   0 runner    (1001) docker     (127)    55588 2024-04-07 06:11:46.000000 fake-bpy-module-latest-20240407/bl_operators/presets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/presets/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.298709 fake-bpy-module-latest-20240407/bl_operators/rigidbody/
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-07 06:11:46.000000 fake-bpy-module-latest-20240407/bl_operators/rigidbody/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/rigidbody/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.298709 fake-bpy-module-latest-20240407/bl_operators/screen_play_rendered_anim/
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-07 06:11:47.000000 fake-bpy-module-latest-20240407/bl_operators/screen_play_rendered_anim/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/screen_play_rendered_anim/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.298709 fake-bpy-module-latest-20240407/bl_operators/sequencer/
--rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-04-07 06:11:45.000000 fake-bpy-module-latest-20240407/bl_operators/sequencer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/sequencer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.298709 fake-bpy-module-latest-20240407/bl_operators/spreadsheet/
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-07 06:11:47.000000 fake-bpy-module-latest-20240407/bl_operators/spreadsheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/spreadsheet/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.298709 fake-bpy-module-latest-20240407/bl_operators/userpref/
--rw-r--r--   0 runner    (1001) docker     (127)    51510 2024-04-07 06:11:45.000000 fake-bpy-module-latest-20240407/bl_operators/userpref/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/userpref/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.298709 fake-bpy-module-latest-20240407/bl_operators/uvcalc_follow_active/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-07 06:11:47.000000 fake-bpy-module-latest-20240407/bl_operators/uvcalc_follow_active/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/uvcalc_follow_active/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.298709 fake-bpy-module-latest-20240407/bl_operators/uvcalc_lightmap/
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-07 06:11:47.000000 fake-bpy-module-latest-20240407/bl_operators/uvcalc_lightmap/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/uvcalc_lightmap/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.298709 fake-bpy-module-latest-20240407/bl_operators/uvcalc_transform/
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-07 06:11:47.000000 fake-bpy-module-latest-20240407/bl_operators/uvcalc_transform/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/uvcalc_transform/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.298709 fake-bpy-module-latest-20240407/bl_operators/vertexpaint_dirt/
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-07 06:11:46.000000 fake-bpy-module-latest-20240407/bl_operators/vertexpaint_dirt/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/vertexpaint_dirt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.298709 fake-bpy-module-latest-20240407/bl_operators/view3d/
--rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-04-07 06:11:46.000000 fake-bpy-module-latest-20240407/bl_operators/view3d/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/view3d/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.302708 fake-bpy-module-latest-20240407/bl_operators/wm/
--rw-r--r--   0 runner    (1001) docker     (127)    94752 2024-04-07 06:11:45.000000 fake-bpy-module-latest-20240407/bl_operators/wm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_operators/wm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.302708 fake-bpy-module-latest-20240407/bl_previews_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-07 06:11:52.000000 fake-bpy-module-latest-20240407/bl_previews_utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.302708 fake-bpy-module-latest-20240407/bl_previews_utils/bl_previews_render/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-07 06:11:52.000000 fake-bpy-module-latest-20240407/bl_previews_utils/bl_previews_render/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_previews_utils/bl_previews_render/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_previews_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.302708 fake-bpy-module-latest-20240407/bl_rna_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-07 06:11:51.000000 fake-bpy-module-latest-20240407/bl_rna_utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.302708 fake-bpy-module-latest-20240407/bl_rna_utils/data_path/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-07 06:11:51.000000 fake-bpy-module-latest-20240407/bl_rna_utils/data_path/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_rna_utils/data_path/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_rna_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.302708 fake-bpy-module-latest-20240407/bl_text_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-07 06:11:51.000000 fake-bpy-module-latest-20240407/bl_text_utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.302708 fake-bpy-module-latest-20240407/bl_text_utils/external_editor/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-07 06:11:51.000000 fake-bpy-module-latest-20240407/bl_text_utils/external_editor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_text_utils/external_editor/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_text_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.302708 fake-bpy-module-latest-20240407/bl_ui/
--rw-r--r--   0 runner    (1001) docker     (127)    10870 2024-04-07 06:11:37.000000 fake-bpy-module-latest-20240407/bl_ui/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.302708 fake-bpy-module-latest-20240407/bl_ui/anim/
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-07 06:11:44.000000 fake-bpy-module-latest-20240407/bl_ui/anim/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/anim/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.302708 fake-bpy-module-latest-20240407/bl_ui/asset_shelf/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-07 06:11:45.000000 fake-bpy-module-latest-20240407/bl_ui/asset_shelf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/asset_shelf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.302708 fake-bpy-module-latest-20240407/bl_ui/generic_ui_list/
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-07 06:11:42.000000 fake-bpy-module-latest-20240407/bl_ui/generic_ui_list/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/generic_ui_list/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.302708 fake-bpy-module-latest-20240407/bl_ui/node_add_menu/
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-07 06:11:45.000000 fake-bpy-module-latest-20240407/bl_ui/node_add_menu/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/node_add_menu/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.306708 fake-bpy-module-latest-20240407/bl_ui/node_add_menu_compositor/
--rw-r--r--   0 runner    (1001) docker     (127)    50565 2024-04-07 06:11:43.000000 fake-bpy-module-latest-20240407/bl_ui/node_add_menu_compositor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/node_add_menu_compositor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.306708 fake-bpy-module-latest-20240407/bl_ui/node_add_menu_geometry/
--rw-r--r--   0 runner    (1001) docker     (127)   134623 2024-04-07 06:11:37.000000 fake-bpy-module-latest-20240407/bl_ui/node_add_menu_geometry/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/node_add_menu_geometry/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.306708 fake-bpy-module-latest-20240407/bl_ui/node_add_menu_shader/
--rw-r--r--   0 runner    (1001) docker     (127)    28547 2024-04-07 06:11:39.000000 fake-bpy-module-latest-20240407/bl_ui/node_add_menu_shader/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/node_add_menu_shader/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.306708 fake-bpy-module-latest-20240407/bl_ui/node_add_menu_texture/
--rw-r--r--   0 runner    (1001) docker     (127)    25256 2024-04-07 06:11:44.000000 fake-bpy-module-latest-20240407/bl_ui/node_add_menu_texture/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/node_add_menu_texture/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.306708 fake-bpy-module-latest-20240407/bl_ui/properties_animviz/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-07 06:11:44.000000 fake-bpy-module-latest-20240407/bl_ui/properties_animviz/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_animviz/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.306708 fake-bpy-module-latest-20240407/bl_ui/properties_collection/
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-04-07 06:11:40.000000 fake-bpy-module-latest-20240407/bl_ui/properties_collection/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_collection/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.306708 fake-bpy-module-latest-20240407/bl_ui/properties_constraint/
--rw-r--r--   0 runner    (1001) docker     (127)   426665 2024-04-07 06:11:41.000000 fake-bpy-module-latest-20240407/bl_ui/properties_constraint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_constraint/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.306708 fake-bpy-module-latest-20240407/bl_ui/properties_data_armature/
--rw-r--r--   0 runner    (1001) docker     (127)    29413 2024-04-07 06:11:40.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_armature/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_armature/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.306708 fake-bpy-module-latest-20240407/bl_ui/properties_data_bone/
--rw-r--r--   0 runner    (1001) docker     (127)    23826 2024-04-07 06:11:41.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_bone/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_bone/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.306708 fake-bpy-module-latest-20240407/bl_ui/properties_data_camera/
--rw-r--r--   0 runner    (1001) docker     (127)    35270 2024-04-07 06:11:40.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_camera/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_camera/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.310709 fake-bpy-module-latest-20240407/bl_ui/properties_data_curve/
--rw-r--r--   0 runner    (1001) docker     (127)    36121 2024-04-07 06:11:41.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_curve/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_curve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.310709 fake-bpy-module-latest-20240407/bl_ui/properties_data_curves/
--rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-04-07 06:11:38.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_curves/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_curves/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.310709 fake-bpy-module-latest-20240407/bl_ui/properties_data_empty/
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-07 06:11:37.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_empty/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_empty/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.310709 fake-bpy-module-latest-20240407/bl_ui/properties_data_gpencil/
--rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-04-07 06:11:39.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_gpencil/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_gpencil/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.310709 fake-bpy-module-latest-20240407/bl_ui/properties_data_grease_pencil/
--rw-r--r--   0 runner    (1001) docker     (127)    31889 2024-04-07 06:11:44.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_grease_pencil/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_grease_pencil/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.310709 fake-bpy-module-latest-20240407/bl_ui/properties_data_lattice/
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-07 06:11:45.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_lattice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_lattice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.310709 fake-bpy-module-latest-20240407/bl_ui/properties_data_light/
--rw-r--r--   0 runner    (1001) docker     (127)    24093 2024-04-07 06:11:43.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_light/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_light/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.310709 fake-bpy-module-latest-20240407/bl_ui/properties_data_lightprobe/
--rw-r--r--   0 runner    (1001) docker     (127)    14426 2024-04-07 06:11:41.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_lightprobe/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_lightprobe/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.310709 fake-bpy-module-latest-20240407/bl_ui/properties_data_mesh/
--rw-r--r--   0 runner    (1001) docker     (127)    49618 2024-04-07 06:11:40.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_mesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_mesh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.310709 fake-bpy-module-latest-20240407/bl_ui/properties_data_metaball/
--rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-07 06:11:44.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_metaball/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_metaball/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.310709 fake-bpy-module-latest-20240407/bl_ui/properties_data_modifier/
--rw-r--r--   0 runner    (1001) docker     (127)    25817 2024-04-07 06:11:40.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_modifier/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_modifier/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.314709 fake-bpy-module-latest-20240407/bl_ui/properties_data_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (127)    12873 2024-04-07 06:11:43.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_pointcloud/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_pointcloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.314709 fake-bpy-module-latest-20240407/bl_ui/properties_data_shaderfx/
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-07 06:11:44.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_shaderfx/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_shaderfx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.314709 fake-bpy-module-latest-20240407/bl_ui/properties_data_speaker/
--rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-04-07 06:11:44.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_speaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_speaker/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.314709 fake-bpy-module-latest-20240407/bl_ui/properties_data_volume/
--rw-r--r--   0 runner    (1001) docker     (127)    19050 2024-04-07 06:11:42.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_volume/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_data_volume/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.314709 fake-bpy-module-latest-20240407/bl_ui/properties_freestyle/
--rw-r--r--   0 runner    (1001) docker     (127)    62310 2024-04-07 06:11:41.000000 fake-bpy-module-latest-20240407/bl_ui/properties_freestyle/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_freestyle/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.314709 fake-bpy-module-latest-20240407/bl_ui/properties_grease_pencil_common/
--rw-r--r--   0 runner    (1001) docker     (127)    39922 2024-04-07 06:11:39.000000 fake-bpy-module-latest-20240407/bl_ui/properties_grease_pencil_common/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_grease_pencil_common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.314709 fake-bpy-module-latest-20240407/bl_ui/properties_mask_common/
--rw-r--r--   0 runner    (1001) docker     (127)    20923 2024-04-07 06:11:44.000000 fake-bpy-module-latest-20240407/bl_ui/properties_mask_common/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_mask_common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.314709 fake-bpy-module-latest-20240407/bl_ui/properties_material/
--rw-r--r--   0 runner    (1001) docker     (127)    36095 2024-04-07 06:11:38.000000 fake-bpy-module-latest-20240407/bl_ui/properties_material/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_material/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.314709 fake-bpy-module-latest-20240407/bl_ui/properties_material_gpencil/
--rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-07 06:11:41.000000 fake-bpy-module-latest-20240407/bl_ui/properties_material_gpencil/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_material_gpencil/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.314709 fake-bpy-module-latest-20240407/bl_ui/properties_object/
--rw-r--r--   0 runner    (1001) docker     (127)    33035 2024-04-07 06:11:40.000000 fake-bpy-module-latest-20240407/bl_ui/properties_object/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_object/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.314709 fake-bpy-module-latest-20240407/bl_ui/properties_output/
--rw-r--r--   0 runner    (1001) docker     (127)    44922 2024-04-07 06:11:40.000000 fake-bpy-module-latest-20240407/bl_ui/properties_output/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_output/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.314709 fake-bpy-module-latest-20240407/bl_ui/properties_paint_common/
--rw-r--r--   0 runner    (1001) docker     (127)    18891 2024-04-07 06:11:43.000000 fake-bpy-module-latest-20240407/bl_ui/properties_paint_common/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_paint_common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.318709 fake-bpy-module-latest-20240407/bl_ui/properties_particle/
--rw-r--r--   0 runner    (1001) docker     (127)   125718 2024-04-07 06:11:39.000000 fake-bpy-module-latest-20240407/bl_ui/properties_particle/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_particle/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.318709 fake-bpy-module-latest-20240407/bl_ui/properties_physics_cloth/
--rw-r--r--   0 runner    (1001) docker     (127)    34539 2024-04-07 06:11:42.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_cloth/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_cloth/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.318709 fake-bpy-module-latest-20240407/bl_ui/properties_physics_common/
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-07 06:11:43.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_common/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.318709 fake-bpy-module-latest-20240407/bl_ui/properties_physics_dynamicpaint/
--rw-r--r--   0 runner    (1001) docker     (127)    67182 2024-04-07 06:11:42.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_dynamicpaint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_dynamicpaint/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.318709 fake-bpy-module-latest-20240407/bl_ui/properties_physics_field/
--rw-r--r--   0 runner    (1001) docker     (127)    25951 2024-04-07 06:11:42.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_field/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_field/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.318709 fake-bpy-module-latest-20240407/bl_ui/properties_physics_fluid/
--rw-r--r--   0 runner    (1001) docker     (127)    92051 2024-04-07 06:11:42.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_fluid/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_fluid/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.318709 fake-bpy-module-latest-20240407/bl_ui/properties_physics_geometry_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-07 06:11:43.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_geometry_nodes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_geometry_nodes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.318709 fake-bpy-module-latest-20240407/bl_ui/properties_physics_rigidbody/
--rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-04-07 06:11:44.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_rigidbody/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_rigidbody/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.318709 fake-bpy-module-latest-20240407/bl_ui/properties_physics_rigidbody_constraint/
--rw-r--r--   0 runner    (1001) docker     (127)    31264 2024-04-07 06:11:43.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_rigidbody_constraint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_rigidbody_constraint/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.318709 fake-bpy-module-latest-20240407/bl_ui/properties_physics_softbody/
--rw-r--r--   0 runner    (1001) docker     (127)    36573 2024-04-07 06:11:39.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_softbody/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_physics_softbody/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.318709 fake-bpy-module-latest-20240407/bl_ui/properties_render/
--rw-r--r--   0 runner    (1001) docker     (127)   124916 2024-04-07 06:11:38.000000 fake-bpy-module-latest-20240407/bl_ui/properties_render/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_render/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.322709 fake-bpy-module-latest-20240407/bl_ui/properties_scene/
--rw-r--r--   0 runner    (1001) docker     (127)    33211 2024-04-07 06:11:43.000000 fake-bpy-module-latest-20240407/bl_ui/properties_scene/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_scene/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.322709 fake-bpy-module-latest-20240407/bl_ui/properties_texture/
--rw-r--r--   0 runner    (1001) docker     (127)    62820 2024-04-07 06:11:41.000000 fake-bpy-module-latest-20240407/bl_ui/properties_texture/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_texture/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.322709 fake-bpy-module-latest-20240407/bl_ui/properties_view_layer/
--rw-r--r--   0 runner    (1001) docker     (127)    42615 2024-04-07 06:11:44.000000 fake-bpy-module-latest-20240407/bl_ui/properties_view_layer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_view_layer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.322709 fake-bpy-module-latest-20240407/bl_ui/properties_workspace/
--rw-r--r--   0 runner    (1001) docker     (127)     9707 2024-04-07 06:11:39.000000 fake-bpy-module-latest-20240407/bl_ui/properties_workspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_workspace/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.322709 fake-bpy-module-latest-20240407/bl_ui/properties_world/
--rw-r--r--   0 runner    (1001) docker     (127)    16818 2024-04-07 06:11:40.000000 fake-bpy-module-latest-20240407/bl_ui/properties_world/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/properties_world/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.322709 fake-bpy-module-latest-20240407/bl_ui/space_clip/
--rw-r--r--   0 runner    (1001) docker     (127)   175596 2024-04-07 06:11:37.000000 fake-bpy-module-latest-20240407/bl_ui/space_clip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_clip/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.322709 fake-bpy-module-latest-20240407/bl_ui/space_console/
--rw-r--r--   0 runner    (1001) docker     (127)    15952 2024-04-07 06:11:41.000000 fake-bpy-module-latest-20240407/bl_ui/space_console/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_console/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.322709 fake-bpy-module-latest-20240407/bl_ui/space_dopesheet/
--rw-r--r--   0 runner    (1001) docker     (127)    67891 2024-04-07 06:11:42.000000 fake-bpy-module-latest-20240407/bl_ui/space_dopesheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_dopesheet/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.322709 fake-bpy-module-latest-20240407/bl_ui/space_filebrowser/
--rw-r--r--   0 runner    (1001) docker     (127)    74428 2024-04-07 06:11:42.000000 fake-bpy-module-latest-20240407/bl_ui/space_filebrowser/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_filebrowser/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.322709 fake-bpy-module-latest-20240407/bl_ui/space_graph/
--rw-r--r--   0 runner    (1001) docker     (127)    52963 2024-04-07 06:11:38.000000 fake-bpy-module-latest-20240407/bl_ui/space_graph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_graph/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.326709 fake-bpy-module-latest-20240407/bl_ui/space_image/
--rw-r--r--   0 runner    (1001) docker     (127)   191743 2024-04-07 06:11:40.000000 fake-bpy-module-latest-20240407/bl_ui/space_image/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_image/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.326709 fake-bpy-module-latest-20240407/bl_ui/space_info/
--rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-04-07 06:11:42.000000 fake-bpy-module-latest-20240407/bl_ui/space_info/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_info/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.326709 fake-bpy-module-latest-20240407/bl_ui/space_nla/
--rw-r--r--   0 runner    (1001) docker     (127)    45091 2024-04-07 06:11:37.000000 fake-bpy-module-latest-20240407/bl_ui/space_nla/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_nla/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.326709 fake-bpy-module-latest-20240407/bl_ui/space_node/
--rw-r--r--   0 runner    (1001) docker     (127)    88748 2024-04-07 06:11:43.000000 fake-bpy-module-latest-20240407/bl_ui/space_node/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_node/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.326709 fake-bpy-module-latest-20240407/bl_ui/space_outliner/
--rw-r--r--   0 runner    (1001) docker     (127)    37796 2024-04-07 06:11:43.000000 fake-bpy-module-latest-20240407/bl_ui/space_outliner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_outliner/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.326709 fake-bpy-module-latest-20240407/bl_ui/space_properties/
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-07 06:11:41.000000 fake-bpy-module-latest-20240407/bl_ui/space_properties/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_properties/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.326709 fake-bpy-module-latest-20240407/bl_ui/space_sequencer/
--rw-r--r--   0 runner    (1001) docker     (127)   190965 2024-04-07 06:11:38.000000 fake-bpy-module-latest-20240407/bl_ui/space_sequencer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_sequencer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.326709 fake-bpy-module-latest-20240407/bl_ui/space_spreadsheet/
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-07 06:11:44.000000 fake-bpy-module-latest-20240407/bl_ui/space_spreadsheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_spreadsheet/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.326709 fake-bpy-module-latest-20240407/bl_ui/space_statusbar/
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-07 06:11:45.000000 fake-bpy-module-latest-20240407/bl_ui/space_statusbar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_statusbar/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.326709 fake-bpy-module-latest-20240407/bl_ui/space_text/
--rw-r--r--   0 runner    (1001) docker     (127)    41578 2024-04-07 06:11:42.000000 fake-bpy-module-latest-20240407/bl_ui/space_text/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_text/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.326709 fake-bpy-module-latest-20240407/bl_ui/space_time/
--rw-r--r--   0 runner    (1001) docker     (127)    18567 2024-04-07 06:11:43.000000 fake-bpy-module-latest-20240407/bl_ui/space_time/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_time/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.330709 fake-bpy-module-latest-20240407/bl_ui/space_toolsystem_common/
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-07 06:11:39.000000 fake-bpy-module-latest-20240407/bl_ui/space_toolsystem_common/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_toolsystem_common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.330709 fake-bpy-module-latest-20240407/bl_ui/space_toolsystem_toolbar/
--rw-r--r--   0 runner    (1001) docker     (127)    24608 2024-04-07 06:11:40.000000 fake-bpy-module-latest-20240407/bl_ui/space_toolsystem_toolbar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_toolsystem_toolbar/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.330709 fake-bpy-module-latest-20240407/bl_ui/space_topbar/
--rw-r--r--   0 runner    (1001) docker     (127)    68597 2024-04-07 06:11:37.000000 fake-bpy-module-latest-20240407/bl_ui/space_topbar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_topbar/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.330709 fake-bpy-module-latest-20240407/bl_ui/space_userpref/
--rw-r--r--   0 runner    (1001) docker     (127)   208885 2024-04-07 06:11:38.000000 fake-bpy-module-latest-20240407/bl_ui/space_userpref/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_userpref/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.330709 fake-bpy-module-latest-20240407/bl_ui/space_view3d/
--rw-r--r--   0 runner    (1001) docker     (127)   685989 2024-04-07 06:11:39.000000 fake-bpy-module-latest-20240407/bl_ui/space_view3d/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_view3d/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.330709 fake-bpy-module-latest-20240407/bl_ui/space_view3d_toolbar/
--rw-r--r--   0 runner    (1001) docker     (127)   259201 2024-04-07 06:11:39.000000 fake-bpy-module-latest-20240407/bl_ui/space_view3d_toolbar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/space_view3d_toolbar/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.330709 fake-bpy-module-latest-20240407/bl_ui/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-07 06:11:45.000000 fake-bpy-module-latest-20240407/bl_ui/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.330709 fake-bpy-module-latest-20240407/bl_ui_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-07 06:11:51.000000 fake-bpy-module-latest-20240407/bl_ui_utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.330709 fake-bpy-module-latest-20240407/bl_ui_utils/bug_report_url/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-07 06:11:51.000000 fake-bpy-module-latest-20240407/bl_ui_utils/bug_report_url/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui_utils/bug_report_url/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.334709 fake-bpy-module-latest-20240407/bl_ui_utils/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-07 06:11:51.000000 fake-bpy-module-latest-20240407/bl_ui_utils/layout/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui_utils/layout/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bl_ui_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.334709 fake-bpy-module-latest-20240407/blend_render_info/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-07 06:11:51.000000 fake-bpy-module-latest-20240407/blend_render_info/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/blend_render_info/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.334709 fake-bpy-module-latest-20240407/blf/
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-07 06:11:33.000000 fake-bpy-module-latest-20240407/blf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/blf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.334709 fake-bpy-module-latest-20240407/bmesh/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-07 06:11:36.000000 fake-bpy-module-latest-20240407/bmesh/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.334709 fake-bpy-module-latest-20240407/bmesh/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-07 06:11:36.000000 fake-bpy-module-latest-20240407/bmesh/geometry/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bmesh/geometry/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.334709 fake-bpy-module-latest-20240407/bmesh/ops/
--rw-r--r--   0 runner    (1001) docker     (127)    70887 2024-04-07 06:11:36.000000 fake-bpy-module-latest-20240407/bmesh/ops/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bmesh/ops/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bmesh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.334709 fake-bpy-module-latest-20240407/bmesh/types/
--rw-r--r--   0 runner    (1001) docker     (127)    39319 2024-04-07 06:11:36.000000 fake-bpy-module-latest-20240407/bmesh/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bmesh/types/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.334709 fake-bpy-module-latest-20240407/bmesh/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-07 06:11:36.000000 fake-bpy-module-latest-20240407/bmesh/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bmesh/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.334709 fake-bpy-module-latest-20240407/bpy/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.334709 fake-bpy-module-latest-20240407/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-07 06:11:32.000000 fake-bpy-module-latest-20240407/bpy/app/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.334709 fake-bpy-module-latest-20240407/bpy/app/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-07 06:11:32.000000 fake-bpy-module-latest-20240407/bpy/app/handlers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/app/handlers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.334709 fake-bpy-module-latest-20240407/bpy/app/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-07 06:11:32.000000 fake-bpy-module-latest-20240407/bpy/app/icons/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/app/icons/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/app/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/app/timers/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-07 06:11:32.000000 fake-bpy-module-latest-20240407/bpy/app/timers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/app/timers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/app/translations/
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-07 06:11:32.000000 fake-bpy-module-latest-20240407/bpy/app/translations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/app/translations/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/msgbus/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-07 06:11:32.000000 fake-bpy-module-latest-20240407/bpy/msgbus/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/msgbus/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-07 06:11:25.000000 fake-bpy-module-latest-20240407/bpy/ops/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/ops/action/
--rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-04-07 06:11:30.000000 fake-bpy-module-latest-20240407/bpy/ops/action/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/action/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/ops/anim/
--rw-r--r--   0 runner    (1001) docker     (127)    27997 2024-04-07 06:11:28.000000 fake-bpy-module-latest-20240407/bpy/ops/anim/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/anim/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/ops/armature/
--rw-r--r--   0 runner    (1001) docker     (127)    24971 2024-04-07 06:11:31.000000 fake-bpy-module-latest-20240407/bpy/ops/armature/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/armature/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/ops/asset/
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-04-07 06:11:25.000000 fake-bpy-module-latest-20240407/bpy/ops/asset/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/asset/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/ops/boid/
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-07 06:11:26.000000 fake-bpy-module-latest-20240407/bpy/ops/boid/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/boid/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/ops/brush/
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-07 06:11:27.000000 fake-bpy-module-latest-20240407/bpy/ops/brush/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/brush/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/ops/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-07 06:11:29.000000 fake-bpy-module-latest-20240407/bpy/ops/buttons/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/buttons/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/ops/cachefile/
--rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-04-07 06:11:31.000000 fake-bpy-module-latest-20240407/bpy/ops/cachefile/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/cachefile/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.338709 fake-bpy-module-latest-20240407/bpy/ops/camera/
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-07 06:11:26.000000 fake-bpy-module-latest-20240407/bpy/ops/camera/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/camera/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/clip/
--rw-r--r--   0 runner    (1001) docker     (127)    52196 2024-04-07 06:11:28.000000 fake-bpy-module-latest-20240407/bpy/ops/clip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/clip/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/cloth/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-07 06:11:30.000000 fake-bpy-module-latest-20240407/bpy/ops/cloth/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/cloth/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/collection/
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-07 06:11:27.000000 fake-bpy-module-latest-20240407/bpy/ops/collection/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/collection/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/console/
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-07 06:11:26.000000 fake-bpy-module-latest-20240407/bpy/ops/console/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/console/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/constraint/
--rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-04-07 06:11:30.000000 fake-bpy-module-latest-20240407/bpy/ops/constraint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/constraint/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/curve/
--rw-r--r--   0 runner    (1001) docker     (127)    30992 2024-04-07 06:11:31.000000 fake-bpy-module-latest-20240407/bpy/ops/curve/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/curve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/curves/
--rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-04-07 06:11:31.000000 fake-bpy-module-latest-20240407/bpy/ops/curves/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/curves/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/cycles/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-07 06:11:30.000000 fake-bpy-module-latest-20240407/bpy/ops/cycles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/cycles/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/dpaint/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-07 06:11:28.000000 fake-bpy-module-latest-20240407/bpy/ops/dpaint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/dpaint/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/ed/
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-04-07 06:11:25.000000 fake-bpy-module-latest-20240407/bpy/ops/ed/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/ed/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/export_anim/
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-07 06:11:26.000000 fake-bpy-module-latest-20240407/bpy/ops/export_anim/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/export_anim/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/export_mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-07 06:11:26.000000 fake-bpy-module-latest-20240407/bpy/ops/export_mesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/export_mesh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.342709 fake-bpy-module-latest-20240407/bpy/ops/export_scene/
--rw-r--r--   0 runner    (1001) docker     (127)    42387 2024-04-07 06:11:30.000000 fake-bpy-module-latest-20240407/bpy/ops/export_scene/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/export_scene/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/file/
--rw-r--r--   0 runner    (1001) docker     (127)    23620 2024-04-07 06:11:27.000000 fake-bpy-module-latest-20240407/bpy/ops/file/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/file/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/fluid/
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-07 06:11:26.000000 fake-bpy-module-latest-20240407/bpy/ops/fluid/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/fluid/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/font/
--rw-r--r--   0 runner    (1001) docker     (127)    17772 2024-04-07 06:11:27.000000 fake-bpy-module-latest-20240407/bpy/ops/font/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/font/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-07 06:11:27.000000 fake-bpy-module-latest-20240407/bpy/ops/geometry/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/geometry/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/gizmogroup/
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-07 06:11:26.000000 fake-bpy-module-latest-20240407/bpy/ops/gizmogroup/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/gizmogroup/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/gpencil/
--rw-r--r--   0 runner    (1001) docker     (127)   100401 2024-04-07 06:11:25.000000 fake-bpy-module-latest-20240407/bpy/ops/gpencil/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/gpencil/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/graph/
--rw-r--r--   0 runner    (1001) docker     (127)    47020 2024-04-07 06:11:27.000000 fake-bpy-module-latest-20240407/bpy/ops/graph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/graph/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/grease_pencil/
--rw-r--r--   0 runner    (1001) docker     (127)    28042 2024-04-07 06:11:27.000000 fake-bpy-module-latest-20240407/bpy/ops/grease_pencil/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/grease_pencil/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)    44935 2024-04-07 06:11:30.000000 fake-bpy-module-latest-20240407/bpy/ops/image/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/image/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/import_anim/
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-07 06:11:26.000000 fake-bpy-module-latest-20240407/bpy/ops/import_anim/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/import_anim/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/import_curve/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-07 06:11:27.000000 fake-bpy-module-latest-20240407/bpy/ops/import_curve/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/import_curve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/import_mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-07 06:11:30.000000 fake-bpy-module-latest-20240407/bpy/ops/import_mesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/import_mesh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.346709 fake-bpy-module-latest-20240407/bpy/ops/import_scene/
--rw-r--r--   0 runner    (1001) docker     (127)    10603 2024-04-07 06:11:28.000000 fake-bpy-module-latest-20240407/bpy/ops/import_scene/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/import_scene/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.350709 fake-bpy-module-latest-20240407/bpy/ops/info/
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-07 06:11:27.000000 fake-bpy-module-latest-20240407/bpy/ops/info/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/info/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.350709 fake-bpy-module-latest-20240407/bpy/ops/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-07 06:11:31.000000 fake-bpy-module-latest-20240407/bpy/ops/lattice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/lattice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.350709 fake-bpy-module-latest-20240407/bpy/ops/marker/
--rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-04-07 06:11:31.000000 fake-bpy-module-latest-20240407/bpy/ops/marker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/marker/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.350709 fake-bpy-module-latest-20240407/bpy/ops/mask/
--rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-04-07 06:11:28.000000 fake-bpy-module-latest-20240407/bpy/ops/mask/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/mask/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.350709 fake-bpy-module-latest-20240407/bpy/ops/material/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-07 06:11:29.000000 fake-bpy-module-latest-20240407/bpy/ops/material/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/material/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.350709 fake-bpy-module-latest-20240407/bpy/ops/mball/
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-07 06:11:29.000000 fake-bpy-module-latest-20240407/bpy/ops/mball/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/mball/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.350709 fake-bpy-module-latest-20240407/bpy/ops/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)   140802 2024-04-07 06:11:25.000000 fake-bpy-module-latest-20240407/bpy/ops/mesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/mesh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.350709 fake-bpy-module-latest-20240407/bpy/ops/nla/
--rw-r--r--   0 runner    (1001) docker     (127)    22280 2024-04-07 06:11:25.000000 fake-bpy-module-latest-20240407/bpy/ops/nla/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/nla/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.350709 fake-bpy-module-latest-20240407/bpy/ops/node/
--rw-r--r--   0 runner    (1001) docker     (127)    56637 2024-04-07 06:11:29.000000 fake-bpy-module-latest-20240407/bpy/ops/node/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/node/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.350709 fake-bpy-module-latest-20240407/bpy/ops/object/
--rw-r--r--   0 runner    (1001) docker     (127)   187382 2024-04-07 06:11:25.000000 fake-bpy-module-latest-20240407/bpy/ops/object/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/object/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.350709 fake-bpy-module-latest-20240407/bpy/ops/outliner/
--rw-r--r--   0 runner    (1001) docker     (127)    33247 2024-04-07 06:11:25.000000 fake-bpy-module-latest-20240407/bpy/ops/outliner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/outliner/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.354709 fake-bpy-module-latest-20240407/bpy/ops/paint/
--rw-r--r--   0 runner    (1001) docker     (127)    37743 2024-04-07 06:11:31.000000 fake-bpy-module-latest-20240407/bpy/ops/paint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/paint/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.354709 fake-bpy-module-latest-20240407/bpy/ops/paintcurve/
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-07 06:11:31.000000 fake-bpy-module-latest-20240407/bpy/ops/paintcurve/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/paintcurve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.354709 fake-bpy-module-latest-20240407/bpy/ops/palette/
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-07 06:11:26.000000 fake-bpy-module-latest-20240407/bpy/ops/palette/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/palette/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.354709 fake-bpy-module-latest-20240407/bpy/ops/particle/
--rw-r--r--   0 runner    (1001) docker     (127)    16933 2024-04-07 06:11:25.000000 fake-bpy-module-latest-20240407/bpy/ops/particle/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/particle/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.354709 fake-bpy-module-latest-20240407/bpy/ops/pose/
--rw-r--r--   0 runner    (1001) docker     (127)    25918 2024-04-07 06:11:31.000000 fake-bpy-module-latest-20240407/bpy/ops/pose/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/pose/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.354709 fake-bpy-module-latest-20240407/bpy/ops/poselib/
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-07 06:11:31.000000 fake-bpy-module-latest-20240407/bpy/ops/poselib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/poselib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.354709 fake-bpy-module-latest-20240407/bpy/ops/preferences/
--rw-r--r--   0 runner    (1001) docker     (127)    25658 2024-04-07 06:11:29.000000 fake-bpy-module-latest-20240407/bpy/ops/preferences/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/preferences/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.354709 fake-bpy-module-latest-20240407/bpy/ops/ptcache/
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-07 06:11:28.000000 fake-bpy-module-latest-20240407/bpy/ops/ptcache/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/ptcache/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.354709 fake-bpy-module-latest-20240407/bpy/ops/render/
--rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-04-07 06:11:30.000000 fake-bpy-module-latest-20240407/bpy/ops/render/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/render/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.354709 fake-bpy-module-latest-20240407/bpy/ops/rigidbody/
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-07 06:11:28.000000 fake-bpy-module-latest-20240407/bpy/ops/rigidbody/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/rigidbody/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.354709 fake-bpy-module-latest-20240407/bpy/ops/scene/
--rw-r--r--   0 runner    (1001) docker     (127)    18273 2024-04-07 06:11:29.000000 fake-bpy-module-latest-20240407/bpy/ops/scene/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/scene/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.354709 fake-bpy-module-latest-20240407/bpy/ops/screen/
--rw-r--r--   0 runner    (1001) docker     (127)    24924 2024-04-07 06:11:28.000000 fake-bpy-module-latest-20240407/bpy/ops/screen/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/screen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.358709 fake-bpy-module-latest-20240407/bpy/ops/script/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-07 06:11:30.000000 fake-bpy-module-latest-20240407/bpy/ops/script/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/script/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.358709 fake-bpy-module-latest-20240407/bpy/ops/sculpt/
--rw-r--r--   0 runner    (1001) docker     (127)    34542 2024-04-07 06:11:31.000000 fake-bpy-module-latest-20240407/bpy/ops/sculpt/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/sculpt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.358709 fake-bpy-module-latest-20240407/bpy/ops/sculpt_curves/
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-07 06:11:30.000000 fake-bpy-module-latest-20240407/bpy/ops/sculpt_curves/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/sculpt_curves/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.358709 fake-bpy-module-latest-20240407/bpy/ops/sequencer/
--rw-r--r--   0 runner    (1001) docker     (127)    82020 2024-04-07 06:11:26.000000 fake-bpy-module-latest-20240407/bpy/ops/sequencer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/sequencer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.358709 fake-bpy-module-latest-20240407/bpy/ops/sound/
--rw-r--r--   0 runner    (1001) docker     (127)    18620 2024-04-07 06:11:29.000000 fake-bpy-module-latest-20240407/bpy/ops/sound/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/sound/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.358709 fake-bpy-module-latest-20240407/bpy/ops/spreadsheet/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-07 06:11:28.000000 fake-bpy-module-latest-20240407/bpy/ops/spreadsheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/spreadsheet/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.358709 fake-bpy-module-latest-20240407/bpy/ops/surface/
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-07 06:11:26.000000 fake-bpy-module-latest-20240407/bpy/ops/surface/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/surface/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.358709 fake-bpy-module-latest-20240407/bpy/ops/text/
--rw-r--r--   0 runner    (1001) docker     (127)    25158 2024-04-07 06:11:28.000000 fake-bpy-module-latest-20240407/bpy/ops/text/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/text/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.358709 fake-bpy-module-latest-20240407/bpy/ops/text_editor/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-07 06:11:29.000000 fake-bpy-module-latest-20240407/bpy/ops/text_editor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/text_editor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.358709 fake-bpy-module-latest-20240407/bpy/ops/texture/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-07 06:11:27.000000 fake-bpy-module-latest-20240407/bpy/ops/texture/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/texture/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.358709 fake-bpy-module-latest-20240407/bpy/ops/transform/
--rw-r--r--   0 runner    (1001) docker     (127)    61699 2024-04-07 06:11:28.000000 fake-bpy-module-latest-20240407/bpy/ops/transform/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/transform/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.358709 fake-bpy-module-latest-20240407/bpy/ops/ui/
--rw-r--r--   0 runner    (1001) docker     (127)    14340 2024-04-07 06:11:25.000000 fake-bpy-module-latest-20240407/bpy/ops/ui/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/ui/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.362709 fake-bpy-module-latest-20240407/bpy/ops/uilist/
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-07 06:11:27.000000 fake-bpy-module-latest-20240407/bpy/ops/uilist/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/uilist/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.362709 fake-bpy-module-latest-20240407/bpy/ops/uv/
--rw-r--r--   0 runner    (1001) docker     (127)    46784 2024-04-07 06:11:29.000000 fake-bpy-module-latest-20240407/bpy/ops/uv/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/uv/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.362709 fake-bpy-module-latest-20240407/bpy/ops/view2d/
--rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-04-07 06:11:29.000000 fake-bpy-module-latest-20240407/bpy/ops/view2d/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/view2d/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.362709 fake-bpy-module-latest-20240407/bpy/ops/view3d/
--rw-r--r--   0 runner    (1001) docker     (127)    37160 2024-04-07 06:11:29.000000 fake-bpy-module-latest-20240407/bpy/ops/view3d/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/view3d/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.362709 fake-bpy-module-latest-20240407/bpy/ops/wm/
--rw-r--r--   0 runner    (1001) docker     (127)   231946 2024-04-07 06:11:27.000000 fake-bpy-module-latest-20240407/bpy/ops/wm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/ops/wm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.362709 fake-bpy-module-latest-20240407/bpy/ops/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-07 06:11:30.000000 fake-bpy-module-latest-20240407/bpy/ops/workspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/workspace/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.362709 fake-bpy-module-latest-20240407/bpy/ops/world/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-07 06:11:30.000000 fake-bpy-module-latest-20240407/bpy/ops/world/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/ops/world/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.362709 fake-bpy-module-latest-20240407/bpy/path/
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-07 06:11:32.000000 fake-bpy-module-latest-20240407/bpy/path/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/path/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.362709 fake-bpy-module-latest-20240407/bpy/props/
--rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-04-07 06:11:32.000000 fake-bpy-module-latest-20240407/bpy/props/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/props/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.366709 fake-bpy-module-latest-20240407/bpy/types/
--rw-r--r--   0 runner    (1001) docker     (127)  3254021 2024-04-07 06:11:25.000000 fake-bpy-module-latest-20240407/bpy/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:23.000000 fake-bpy-module-latest-20240407/bpy/types/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.366709 fake-bpy-module-latest-20240407/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-04-07 06:11:32.000000 fake-bpy-module-latest-20240407/bpy/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.366709 fake-bpy-module-latest-20240407/bpy/utils/previews/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-07 06:11:32.000000 fake-bpy-module-latest-20240407/bpy/utils/previews/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/utils/previews/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.366709 fake-bpy-module-latest-20240407/bpy/utils/units/
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-07 06:11:32.000000 fake-bpy-module-latest-20240407/bpy/utils/units/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy/utils/units/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.370709 fake-bpy-module-latest-20240407/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-07 06:11:35.000000 fake-bpy-module-latest-20240407/bpy_extras/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.370709 fake-bpy-module-latest-20240407/bpy_extras/anim_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-07 06:11:36.000000 fake-bpy-module-latest-20240407/bpy_extras/anim_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_extras/anim_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.370709 fake-bpy-module-latest-20240407/bpy_extras/asset_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-07 06:11:35.000000 fake-bpy-module-latest-20240407/bpy_extras/asset_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_extras/asset_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.370709 fake-bpy-module-latest-20240407/bpy_extras/id_map_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-07 06:11:35.000000 fake-bpy-module-latest-20240407/bpy_extras/id_map_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_extras/id_map_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.370709 fake-bpy-module-latest-20240407/bpy_extras/image_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-07 06:11:35.000000 fake-bpy-module-latest-20240407/bpy_extras/image_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_extras/image_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.370709 fake-bpy-module-latest-20240407/bpy_extras/io_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-04-07 06:11:35.000000 fake-bpy-module-latest-20240407/bpy_extras/io_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_extras/io_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.370709 fake-bpy-module-latest-20240407/bpy_extras/keyconfig_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-07 06:11:35.000000 fake-bpy-module-latest-20240407/bpy_extras/keyconfig_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_extras/keyconfig_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.370709 fake-bpy-module-latest-20240407/bpy_extras/mesh_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-07 06:11:35.000000 fake-bpy-module-latest-20240407/bpy_extras/mesh_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_extras/mesh_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.370709 fake-bpy-module-latest-20240407/bpy_extras/node_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-07 06:11:35.000000 fake-bpy-module-latest-20240407/bpy_extras/node_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_extras/node_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.370709 fake-bpy-module-latest-20240407/bpy_extras/object_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-07 06:11:36.000000 fake-bpy-module-latest-20240407/bpy_extras/object_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_extras/object_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_extras/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.370709 fake-bpy-module-latest-20240407/bpy_extras/view3d_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-07 06:11:36.000000 fake-bpy-module-latest-20240407/bpy_extras/view3d_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_extras/view3d_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.370709 fake-bpy-module-latest-20240407/bpy_restrict_state/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-07 06:11:51.000000 fake-bpy-module-latest-20240407/bpy_restrict_state/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_restrict_state/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.374709 fake-bpy-module-latest-20240407/bpy_types/
--rw-r--r--   0 runner    (1001) docker     (127)    58139 2024-04-07 06:11:48.000000 fake-bpy-module-latest-20240407/bpy_types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/bpy_types/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.374709 fake-bpy-module-latest-20240407/console_python/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-07 06:11:51.000000 fake-bpy-module-latest-20240407/console_python/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/console_python/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.374709 fake-bpy-module-latest-20240407/console_shell/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-07 06:11:50.000000 fake-bpy-module-latest-20240407/console_shell/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/console_shell/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.386709 fake-bpy-module-latest-20240407/fake_bpy_module_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-07 06:12:19.000000 fake-bpy-module-latest-20240407/fake_bpy_module_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-04-07 06:12:19.000000 fake-bpy-module-latest-20240407/fake_bpy_module_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:12:19.000000 fake-bpy-module-latest-20240407/fake_bpy_module_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-07 06:12:19.000000 fake-bpy-module-latest-20240407/fake_bpy_module_latest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.374709 fake-bpy-module-latest-20240407/freestyle/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-07 06:11:34.000000 fake-bpy-module-latest-20240407/freestyle/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.374709 fake-bpy-module-latest-20240407/freestyle/chainingiterators/
--rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-04-07 06:11:35.000000 fake-bpy-module-latest-20240407/freestyle/chainingiterators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/freestyle/chainingiterators/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.374709 fake-bpy-module-latest-20240407/freestyle/functions/
--rw-r--r--   0 runner    (1001) docker     (127)    48266 2024-04-07 06:11:34.000000 fake-bpy-module-latest-20240407/freestyle/functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/freestyle/functions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.374709 fake-bpy-module-latest-20240407/freestyle/predicates/
--rw-r--r--   0 runner    (1001) docker     (127)    14121 2024-04-07 06:11:35.000000 fake-bpy-module-latest-20240407/freestyle/predicates/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/freestyle/predicates/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/freestyle/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.374709 fake-bpy-module-latest-20240407/freestyle/shaders/
--rw-r--r--   0 runner    (1001) docker     (127)    22831 2024-04-07 06:11:35.000000 fake-bpy-module-latest-20240407/freestyle/shaders/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/freestyle/shaders/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.374709 fake-bpy-module-latest-20240407/freestyle/types/
--rw-r--r--   0 runner    (1001) docker     (127)    97490 2024-04-07 06:11:35.000000 fake-bpy-module-latest-20240407/freestyle/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/freestyle/types/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.374709 fake-bpy-module-latest-20240407/freestyle/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.374709 fake-bpy-module-latest-20240407/freestyle/utils/ContextFunctions/
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-07 06:11:34.000000 fake-bpy-module-latest-20240407/freestyle/utils/ContextFunctions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/freestyle/utils/ContextFunctions/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-07 06:11:34.000000 fake-bpy-module-latest-20240407/freestyle/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/freestyle/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/gpu/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-07 06:11:33.000000 fake-bpy-module-latest-20240407/gpu/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/gpu/capabilities/
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-07 06:11:33.000000 fake-bpy-module-latest-20240407/gpu/capabilities/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/gpu/capabilities/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/gpu/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-07 06:11:33.000000 fake-bpy-module-latest-20240407/gpu/matrix/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/gpu/matrix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/gpu/platform/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-07 06:11:34.000000 fake-bpy-module-latest-20240407/gpu/platform/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/gpu/platform/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/gpu/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/gpu/select/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-07 06:11:33.000000 fake-bpy-module-latest-20240407/gpu/select/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/gpu/select/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/gpu/shader/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-07 06:11:34.000000 fake-bpy-module-latest-20240407/gpu/shader/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/gpu/shader/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/gpu/state/
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-07 06:11:34.000000 fake-bpy-module-latest-20240407/gpu/state/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/gpu/state/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/gpu/texture/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-07 06:11:34.000000 fake-bpy-module-latest-20240407/gpu/texture/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/gpu/texture/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/gpu/types/
--rw-r--r--   0 runner    (1001) docker     (127)    26172 2024-04-07 06:11:34.000000 fake-bpy-module-latest-20240407/gpu/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/gpu/types/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-07 06:11:34.000000 fake-bpy-module-latest-20240407/gpu_extras/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/gpu_extras/batch/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-07 06:11:34.000000 fake-bpy-module-latest-20240407/gpu_extras/batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/gpu_extras/batch/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/gpu_extras/presets/
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-07 06:11:34.000000 fake-bpy-module-latest-20240407/gpu_extras/presets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/gpu_extras/presets/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/gpu_extras/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.378709 fake-bpy-module-latest-20240407/graphviz_export/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-07 06:11:51.000000 fake-bpy-module-latest-20240407/graphviz_export/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/graphviz_export/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.382709 fake-bpy-module-latest-20240407/idprop/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 06:11:36.000000 fake-bpy-module-latest-20240407/idprop/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/idprop/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.382709 fake-bpy-module-latest-20240407/idprop/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-07 06:11:36.000000 fake-bpy-module-latest-20240407/idprop/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/idprop/types/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.382709 fake-bpy-module-latest-20240407/imbuf/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-07 06:11:37.000000 fake-bpy-module-latest-20240407/imbuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/imbuf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.382709 fake-bpy-module-latest-20240407/imbuf/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-07 06:11:37.000000 fake-bpy-module-latest-20240407/imbuf/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/imbuf/types/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.382709 fake-bpy-module-latest-20240407/keyingsets_builtins/
--rw-r--r--   0 runner    (1001) docker     (127)    48336 2024-04-07 06:11:37.000000 fake-bpy-module-latest-20240407/keyingsets_builtins/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/keyingsets_builtins/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.382709 fake-bpy-module-latest-20240407/keyingsets_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-07 06:11:50.000000 fake-bpy-module-latest-20240407/keyingsets_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/keyingsets_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.382709 fake-bpy-module-latest-20240407/mathutils/
--rw-r--r--   0 runner    (1001) docker     (127)    72812 2024-04-07 06:11:33.000000 fake-bpy-module-latest-20240407/mathutils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.382709 fake-bpy-module-latest-20240407/mathutils/bvhtree/
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-07 06:11:33.000000 fake-bpy-module-latest-20240407/mathutils/bvhtree/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/mathutils/bvhtree/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.382709 fake-bpy-module-latest-20240407/mathutils/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)    21014 2024-04-07 06:11:33.000000 fake-bpy-module-latest-20240407/mathutils/geometry/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/mathutils/geometry/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.382709 fake-bpy-module-latest-20240407/mathutils/interpolate/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-07 06:11:33.000000 fake-bpy-module-latest-20240407/mathutils/interpolate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/mathutils/interpolate/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.382709 fake-bpy-module-latest-20240407/mathutils/kdtree/
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-07 06:11:33.000000 fake-bpy-module-latest-20240407/mathutils/kdtree/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/mathutils/kdtree/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.386709 fake-bpy-module-latest-20240407/mathutils/noise/
--rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-04-07 06:11:33.000000 fake-bpy-module-latest-20240407/mathutils/noise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/mathutils/noise/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/mathutils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.386709 fake-bpy-module-latest-20240407/nodeitems_builtins/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-07 06:11:49.000000 fake-bpy-module-latest-20240407/nodeitems_builtins/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/nodeitems_builtins/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.386709 fake-bpy-module-latest-20240407/nodeitems_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-07 06:11:48.000000 fake-bpy-module-latest-20240407/nodeitems_utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/nodeitems_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-07 06:12:16.000000 fake-bpy-module-latest-20240407/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.386709 fake-bpy-module-latest-20240407/rna_info/
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-07 06:11:50.000000 fake-bpy-module-latest-20240407/rna_info/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/rna_info/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.386709 fake-bpy-module-latest-20240407/rna_keymap_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-07 06:11:51.000000 fake-bpy-module-latest-20240407/rna_keymap_ui/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/rna_keymap_ui/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.386709 fake-bpy-module-latest-20240407/rna_prop_ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-07 06:11:50.000000 fake-bpy-module-latest-20240407/rna_prop_ui/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/rna_prop_ui/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.386709 fake-bpy-module-latest-20240407/rna_xml/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-07 06:11:48.000000 fake-bpy-module-latest-20240407/rna_xml/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/rna_xml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 06:12:19.386709 fake-bpy-module-latest-20240407/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-07 06:12:16.000000 fake-bpy-module-latest-20240407/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:12:19.386709 fake-bpy-module-latest-20240407/sys_info/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 06:11:52.000000 fake-bpy-module-latest-20240407/sys_info/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:11:24.000000 fake-bpy-module-latest-20240407/sys_info/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.807798 fake-bpy-module-latest-20240408/
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-08 06:13:21.807798 fake-bpy-module-latest-20240408/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-08 06:13:19.000000 fake-bpy-module-latest-20240408/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.695798 fake-bpy-module-latest-20240408/addon_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-08 06:12:55.000000 fake-bpy-module-latest-20240408/addon_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/addon_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.695798 fake-bpy-module-latest-20240408/animsys_refactor/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-08 06:12:54.000000 fake-bpy-module-latest-20240408/animsys_refactor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/animsys_refactor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.695798 fake-bpy-module-latest-20240408/aud/
+-rw-r--r--   0 runner    (1001) docker     (127)    30520 2024-04-08 06:12:40.000000 fake-bpy-module-latest-20240408/aud/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/aud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.695798 fake-bpy-module-latest-20240408/bgl/
+-rw-r--r--   0 runner    (1001) docker     (127)   105957 2024-04-08 06:12:37.000000 fake-bpy-module-latest-20240408/bgl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bgl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.695798 fake-bpy-module-latest-20240408/bl_app_override/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-08 06:12:55.000000 fake-bpy-module-latest-20240408/bl_app_override/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.695798 fake-bpy-module-latest-20240408/bl_app_override/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-08 06:12:55.000000 fake-bpy-module-latest-20240408/bl_app_override/helpers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_app_override/helpers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_app_override/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.695798 fake-bpy-module-latest-20240408/bl_app_template_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 06:12:56.000000 fake-bpy-module-latest-20240408/bl_app_template_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_app_template_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.699798 fake-bpy-module-latest-20240408/bl_console_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 06:12:52.000000 fake-bpy-module-latest-20240408/bl_console_utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.699798 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-08 06:12:52.000000 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.699798 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/complete_calltip/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 06:12:52.000000 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/complete_calltip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/complete_calltip/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.699798 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/complete_import/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-08 06:12:52.000000 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/complete_import/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/complete_import/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.699798 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/complete_namespace/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-08 06:12:52.000000 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/complete_namespace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/complete_namespace/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.699798 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/intellisense/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 06:12:52.000000 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/intellisense/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/intellisense/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_console_utils/autocomplete/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_console_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.699798 fake-bpy-module-latest-20240408/bl_i18n_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 06:12:53.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.699798 fake-bpy-module-latest-20240408/bl_i18n_utils/bl_extract_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-08 06:12:53.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/bl_extract_messages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/bl_extract_messages/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.699798 fake-bpy-module-latest-20240408/bl_i18n_utils/merge_po/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 06:12:53.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/merge_po/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/merge_po/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.699798 fake-bpy-module-latest-20240408/bl_i18n_utils/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-08 06:12:53.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/settings/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/settings/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.699798 fake-bpy-module-latest-20240408/bl_i18n_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-08 06:12:53.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.699798 fake-bpy-module-latest-20240408/bl_i18n_utils/utils_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-08 06:12:53.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/utils_cli/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/utils_cli/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.703798 fake-bpy-module-latest-20240408/bl_i18n_utils/utils_languages_menu/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-08 06:12:53.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/utils_languages_menu/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/utils_languages_menu/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.703798 fake-bpy-module-latest-20240408/bl_i18n_utils/utils_rtl/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 06:12:53.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/utils_rtl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_i18n_utils/utils_rtl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.703798 fake-bpy-module-latest-20240408/bl_keymap_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 06:12:53.000000 fake-bpy-module-latest-20240408/bl_keymap_utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.703798 fake-bpy-module-latest-20240408/bl_keymap_utils/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-08 06:12:54.000000 fake-bpy-module-latest-20240408/bl_keymap_utils/io/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_keymap_utils/io/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.703798 fake-bpy-module-latest-20240408/bl_keymap_utils/keymap_from_toolbar/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 06:12:54.000000 fake-bpy-module-latest-20240408/bl_keymap_utils/keymap_from_toolbar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_keymap_utils/keymap_from_toolbar/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.703798 fake-bpy-module-latest-20240408/bl_keymap_utils/keymap_hierarchy/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 06:12:54.000000 fake-bpy-module-latest-20240408/bl_keymap_utils/keymap_hierarchy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_keymap_utils/keymap_hierarchy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.703798 fake-bpy-module-latest-20240408/bl_keymap_utils/platform_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-08 06:12:54.000000 fake-bpy-module-latest-20240408/bl_keymap_utils/platform_helpers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_keymap_utils/platform_helpers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_keymap_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.703798 fake-bpy-module-latest-20240408/bl_keymap_utils/versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 06:12:54.000000 fake-bpy-module-latest-20240408/bl_keymap_utils/versioning/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_keymap_utils/versioning/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.703798 fake-bpy-module-latest-20240408/bl_math/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-08 06:12:41.000000 fake-bpy-module-latest-20240408/bl_math/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_math/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.703798 fake-bpy-module-latest-20240408/bl_operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-08 06:12:41.000000 fake-bpy-module-latest-20240408/bl_operators/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.703798 fake-bpy-module-latest-20240408/bl_operators/add_mesh_torus/
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-08 06:12:44.000000 fake-bpy-module-latest-20240408/bl_operators/add_mesh_torus/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/add_mesh_torus/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.703798 fake-bpy-module-latest-20240408/bl_operators/anim/
+-rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-04-08 06:12:43.000000 fake-bpy-module-latest-20240408/bl_operators/anim/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/anim/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.707798 fake-bpy-module-latest-20240408/bl_operators/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-08 06:12:42.000000 fake-bpy-module-latest-20240408/bl_operators/assets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/assets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.707798 fake-bpy-module-latest-20240408/bl_operators/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-08 06:12:43.000000 fake-bpy-module-latest-20240408/bl_operators/bmesh/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.707798 fake-bpy-module-latest-20240408/bl_operators/bmesh/find_adjacent/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-08 06:12:43.000000 fake-bpy-module-latest-20240408/bl_operators/bmesh/find_adjacent/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/bmesh/find_adjacent/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/bmesh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.707798 fake-bpy-module-latest-20240408/bl_operators/clip/
+-rw-r--r--   0 runner    (1001) docker     (127)    20846 2024-04-08 06:12:43.000000 fake-bpy-module-latest-20240408/bl_operators/clip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/clip/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.707798 fake-bpy-module-latest-20240408/bl_operators/console/
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-04-08 06:12:44.000000 fake-bpy-module-latest-20240408/bl_operators/console/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/console/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.707798 fake-bpy-module-latest-20240408/bl_operators/constraint/
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-08 06:12:42.000000 fake-bpy-module-latest-20240408/bl_operators/constraint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/constraint/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.707798 fake-bpy-module-latest-20240408/bl_operators/file/
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-04-08 06:12:43.000000 fake-bpy-module-latest-20240408/bl_operators/file/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/file/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.707798 fake-bpy-module-latest-20240408/bl_operators/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-04-08 06:12:43.000000 fake-bpy-module-latest-20240408/bl_operators/freestyle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/freestyle/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.707798 fake-bpy-module-latest-20240408/bl_operators/geometry_nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)    36068 2024-04-08 06:12:42.000000 fake-bpy-module-latest-20240408/bl_operators/geometry_nodes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/geometry_nodes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.707798 fake-bpy-module-latest-20240408/bl_operators/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-08 06:12:43.000000 fake-bpy-module-latest-20240408/bl_operators/image/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/image/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.707798 fake-bpy-module-latest-20240408/bl_operators/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-08 06:12:43.000000 fake-bpy-module-latest-20240408/bl_operators/mesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/mesh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.711798 fake-bpy-module-latest-20240408/bl_operators/node/
+-rw-r--r--   0 runner    (1001) docker     (127)    27034 2024-04-08 06:12:42.000000 fake-bpy-module-latest-20240408/bl_operators/node/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/node/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.711798 fake-bpy-module-latest-20240408/bl_operators/object/
+-rw-r--r--   0 runner    (1001) docker     (127)    30487 2024-04-08 06:12:42.000000 fake-bpy-module-latest-20240408/bl_operators/object/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/object/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.711798 fake-bpy-module-latest-20240408/bl_operators/object_align/
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-08 06:12:44.000000 fake-bpy-module-latest-20240408/bl_operators/object_align/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/object_align/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.711798 fake-bpy-module-latest-20240408/bl_operators/object_quick_effects/
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-04-08 06:12:42.000000 fake-bpy-module-latest-20240408/bl_operators/object_quick_effects/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/object_quick_effects/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.711798 fake-bpy-module-latest-20240408/bl_operators/object_randomize_transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-08 06:12:43.000000 fake-bpy-module-latest-20240408/bl_operators/object_randomize_transform/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/object_randomize_transform/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.711798 fake-bpy-module-latest-20240408/bl_operators/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)    55588 2024-04-08 06:12:43.000000 fake-bpy-module-latest-20240408/bl_operators/presets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/presets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.711798 fake-bpy-module-latest-20240408/bl_operators/rigidbody/
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-08 06:12:42.000000 fake-bpy-module-latest-20240408/bl_operators/rigidbody/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/rigidbody/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.711798 fake-bpy-module-latest-20240408/bl_operators/screen_play_rendered_anim/
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-08 06:12:44.000000 fake-bpy-module-latest-20240408/bl_operators/screen_play_rendered_anim/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/screen_play_rendered_anim/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.711798 fake-bpy-module-latest-20240408/bl_operators/sequencer/
+-rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-04-08 06:12:44.000000 fake-bpy-module-latest-20240408/bl_operators/sequencer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/sequencer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.711798 fake-bpy-module-latest-20240408/bl_operators/spreadsheet/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-08 06:12:42.000000 fake-bpy-module-latest-20240408/bl_operators/spreadsheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/spreadsheet/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.715798 fake-bpy-module-latest-20240408/bl_operators/userpref/
+-rw-r--r--   0 runner    (1001) docker     (127)    51510 2024-04-08 06:12:42.000000 fake-bpy-module-latest-20240408/bl_operators/userpref/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/userpref/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.715798 fake-bpy-module-latest-20240408/bl_operators/uvcalc_follow_active/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-08 06:12:42.000000 fake-bpy-module-latest-20240408/bl_operators/uvcalc_follow_active/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/uvcalc_follow_active/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.715798 fake-bpy-module-latest-20240408/bl_operators/uvcalc_lightmap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-08 06:12:44.000000 fake-bpy-module-latest-20240408/bl_operators/uvcalc_lightmap/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/uvcalc_lightmap/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.715798 fake-bpy-module-latest-20240408/bl_operators/uvcalc_transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-08 06:12:42.000000 fake-bpy-module-latest-20240408/bl_operators/uvcalc_transform/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/uvcalc_transform/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.715798 fake-bpy-module-latest-20240408/bl_operators/vertexpaint_dirt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-08 06:12:43.000000 fake-bpy-module-latest-20240408/bl_operators/vertexpaint_dirt/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/vertexpaint_dirt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.715798 fake-bpy-module-latest-20240408/bl_operators/view3d/
+-rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-04-08 06:12:42.000000 fake-bpy-module-latest-20240408/bl_operators/view3d/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/view3d/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.715798 fake-bpy-module-latest-20240408/bl_operators/wm/
+-rw-r--r--   0 runner    (1001) docker     (127)    94752 2024-04-08 06:12:41.000000 fake-bpy-module-latest-20240408/bl_operators/wm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_operators/wm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.715798 fake-bpy-module-latest-20240408/bl_previews_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 06:12:55.000000 fake-bpy-module-latest-20240408/bl_previews_utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.715798 fake-bpy-module-latest-20240408/bl_previews_utils/bl_previews_render/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-08 06:12:55.000000 fake-bpy-module-latest-20240408/bl_previews_utils/bl_previews_render/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_previews_utils/bl_previews_render/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_previews_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.715798 fake-bpy-module-latest-20240408/bl_rna_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-08 06:12:55.000000 fake-bpy-module-latest-20240408/bl_rna_utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.715798 fake-bpy-module-latest-20240408/bl_rna_utils/data_path/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 06:12:55.000000 fake-bpy-module-latest-20240408/bl_rna_utils/data_path/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_rna_utils/data_path/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_rna_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.719798 fake-bpy-module-latest-20240408/bl_text_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 06:12:55.000000 fake-bpy-module-latest-20240408/bl_text_utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.719798 fake-bpy-module-latest-20240408/bl_text_utils/external_editor/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-08 06:12:55.000000 fake-bpy-module-latest-20240408/bl_text_utils/external_editor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_text_utils/external_editor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_text_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.719798 fake-bpy-module-latest-20240408/bl_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    10870 2024-04-08 06:12:44.000000 fake-bpy-module-latest-20240408/bl_ui/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.719798 fake-bpy-module-latest-20240408/bl_ui/anim/
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-08 06:12:49.000000 fake-bpy-module-latest-20240408/bl_ui/anim/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/anim/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.719798 fake-bpy-module-latest-20240408/bl_ui/asset_shelf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-08 06:12:52.000000 fake-bpy-module-latest-20240408/bl_ui/asset_shelf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/asset_shelf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.719798 fake-bpy-module-latest-20240408/bl_ui/generic_ui_list/
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-08 06:12:51.000000 fake-bpy-module-latest-20240408/bl_ui/generic_ui_list/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/generic_ui_list/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.719798 fake-bpy-module-latest-20240408/bl_ui/node_add_menu/
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-08 06:12:51.000000 fake-bpy-module-latest-20240408/bl_ui/node_add_menu/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/node_add_menu/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.719798 fake-bpy-module-latest-20240408/bl_ui/node_add_menu_compositor/
+-rw-r--r--   0 runner    (1001) docker     (127)    50565 2024-04-08 06:12:47.000000 fake-bpy-module-latest-20240408/bl_ui/node_add_menu_compositor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/node_add_menu_compositor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.719798 fake-bpy-module-latest-20240408/bl_ui/node_add_menu_geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)   134623 2024-04-08 06:12:45.000000 fake-bpy-module-latest-20240408/bl_ui/node_add_menu_geometry/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/node_add_menu_geometry/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.719798 fake-bpy-module-latest-20240408/bl_ui/node_add_menu_shader/
+-rw-r--r--   0 runner    (1001) docker     (127)    28547 2024-04-08 06:12:48.000000 fake-bpy-module-latest-20240408/bl_ui/node_add_menu_shader/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/node_add_menu_shader/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.719798 fake-bpy-module-latest-20240408/bl_ui/node_add_menu_texture/
+-rw-r--r--   0 runner    (1001) docker     (127)    25256 2024-04-08 06:12:49.000000 fake-bpy-module-latest-20240408/bl_ui/node_add_menu_texture/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/node_add_menu_texture/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.723798 fake-bpy-module-latest-20240408/bl_ui/properties_animviz/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-08 06:12:47.000000 fake-bpy-module-latest-20240408/bl_ui/properties_animviz/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_animviz/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.723798 fake-bpy-module-latest-20240408/bl_ui/properties_collection/
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-04-08 06:12:51.000000 fake-bpy-module-latest-20240408/bl_ui/properties_collection/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_collection/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.723798 fake-bpy-module-latest-20240408/bl_ui/properties_constraint/
+-rw-r--r--   0 runner    (1001) docker     (127)   426665 2024-04-08 06:12:46.000000 fake-bpy-module-latest-20240408/bl_ui/properties_constraint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_constraint/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.723798 fake-bpy-module-latest-20240408/bl_ui/properties_data_armature/
+-rw-r--r--   0 runner    (1001) docker     (127)    29413 2024-04-08 06:12:46.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_armature/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_armature/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.723798 fake-bpy-module-latest-20240408/bl_ui/properties_data_bone/
+-rw-r--r--   0 runner    (1001) docker     (127)    23826 2024-04-08 06:12:50.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_bone/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_bone/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.723798 fake-bpy-module-latest-20240408/bl_ui/properties_data_camera/
+-rw-r--r--   0 runner    (1001) docker     (127)    35270 2024-04-08 06:12:47.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_camera/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_camera/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.723798 fake-bpy-module-latest-20240408/bl_ui/properties_data_curve/
+-rw-r--r--   0 runner    (1001) docker     (127)    36121 2024-04-08 06:12:47.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_curve/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_curve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.723798 fake-bpy-module-latest-20240408/bl_ui/properties_data_curves/
+-rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-04-08 06:12:50.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_curves/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_curves/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.723798 fake-bpy-module-latest-20240408/bl_ui/properties_data_empty/
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-08 06:12:51.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_empty/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_empty/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.727798 fake-bpy-module-latest-20240408/bl_ui/properties_data_gpencil/
+-rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-04-08 06:12:48.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_gpencil/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_gpencil/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.727798 fake-bpy-module-latest-20240408/bl_ui/properties_data_grease_pencil/
+-rw-r--r--   0 runner    (1001) docker     (127)    31889 2024-04-08 06:12:47.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_grease_pencil/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_grease_pencil/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.727798 fake-bpy-module-latest-20240408/bl_ui/properties_data_lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-08 06:12:51.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_lattice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_lattice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.727798 fake-bpy-module-latest-20240408/bl_ui/properties_data_light/
+-rw-r--r--   0 runner    (1001) docker     (127)    24093 2024-04-08 06:12:48.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_light/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_light/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.727798 fake-bpy-module-latest-20240408/bl_ui/properties_data_lightprobe/
+-rw-r--r--   0 runner    (1001) docker     (127)    14426 2024-04-08 06:12:50.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_lightprobe/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_lightprobe/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.727798 fake-bpy-module-latest-20240408/bl_ui/properties_data_mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    49618 2024-04-08 06:12:48.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_mesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_mesh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.727798 fake-bpy-module-latest-20240408/bl_ui/properties_data_metaball/
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-08 06:12:50.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_metaball/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_metaball/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.727798 fake-bpy-module-latest-20240408/bl_ui/properties_data_modifier/
+-rw-r--r--   0 runner    (1001) docker     (127)    25817 2024-04-08 06:12:46.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_modifier/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_modifier/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.727798 fake-bpy-module-latest-20240408/bl_ui/properties_data_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    12873 2024-04-08 06:12:47.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_pointcloud/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_pointcloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.727798 fake-bpy-module-latest-20240408/bl_ui/properties_data_shaderfx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-08 06:12:52.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_shaderfx/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_shaderfx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.731798 fake-bpy-module-latest-20240408/bl_ui/properties_data_speaker/
+-rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-04-08 06:12:47.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_speaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_speaker/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.731798 fake-bpy-module-latest-20240408/bl_ui/properties_data_volume/
+-rw-r--r--   0 runner    (1001) docker     (127)    19050 2024-04-08 06:12:50.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_volume/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_data_volume/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.731798 fake-bpy-module-latest-20240408/bl_ui/properties_freestyle/
+-rw-r--r--   0 runner    (1001) docker     (127)    62310 2024-04-08 06:12:44.000000 fake-bpy-module-latest-20240408/bl_ui/properties_freestyle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_freestyle/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.731798 fake-bpy-module-latest-20240408/bl_ui/properties_grease_pencil_common/
+-rw-r--r--   0 runner    (1001) docker     (127)    39922 2024-04-08 06:12:51.000000 fake-bpy-module-latest-20240408/bl_ui/properties_grease_pencil_common/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_grease_pencil_common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.731798 fake-bpy-module-latest-20240408/bl_ui/properties_mask_common/
+-rw-r--r--   0 runner    (1001) docker     (127)    20923 2024-04-08 06:12:50.000000 fake-bpy-module-latest-20240408/bl_ui/properties_mask_common/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_mask_common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.731798 fake-bpy-module-latest-20240408/bl_ui/properties_material/
+-rw-r--r--   0 runner    (1001) docker     (127)    36095 2024-04-08 06:12:48.000000 fake-bpy-module-latest-20240408/bl_ui/properties_material/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_material/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.731798 fake-bpy-module-latest-20240408/bl_ui/properties_material_gpencil/
+-rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-08 06:12:49.000000 fake-bpy-module-latest-20240408/bl_ui/properties_material_gpencil/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_material_gpencil/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.731798 fake-bpy-module-latest-20240408/bl_ui/properties_object/
+-rw-r--r--   0 runner    (1001) docker     (127)    33035 2024-04-08 06:12:48.000000 fake-bpy-module-latest-20240408/bl_ui/properties_object/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_object/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.731798 fake-bpy-module-latest-20240408/bl_ui/properties_output/
+-rw-r--r--   0 runner    (1001) docker     (127)    44922 2024-04-08 06:12:48.000000 fake-bpy-module-latest-20240408/bl_ui/properties_output/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_output/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.731798 fake-bpy-module-latest-20240408/bl_ui/properties_paint_common/
+-rw-r--r--   0 runner    (1001) docker     (127)    18891 2024-04-08 06:12:46.000000 fake-bpy-module-latest-20240408/bl_ui/properties_paint_common/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_paint_common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.735798 fake-bpy-module-latest-20240408/bl_ui/properties_particle/
+-rw-r--r--   0 runner    (1001) docker     (127)   125718 2024-04-08 06:12:45.000000 fake-bpy-module-latest-20240408/bl_ui/properties_particle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_particle/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.735798 fake-bpy-module-latest-20240408/bl_ui/properties_physics_cloth/
+-rw-r--r--   0 runner    (1001) docker     (127)    34539 2024-04-08 06:12:46.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_cloth/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_cloth/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.735798 fake-bpy-module-latest-20240408/bl_ui/properties_physics_common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-08 06:12:50.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_common/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.735798 fake-bpy-module-latest-20240408/bl_ui/properties_physics_dynamicpaint/
+-rw-r--r--   0 runner    (1001) docker     (127)    67182 2024-04-08 06:12:46.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_dynamicpaint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_dynamicpaint/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.735798 fake-bpy-module-latest-20240408/bl_ui/properties_physics_field/
+-rw-r--r--   0 runner    (1001) docker     (127)    25951 2024-04-08 06:12:50.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_field/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_field/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.735798 fake-bpy-module-latest-20240408/bl_ui/properties_physics_fluid/
+-rw-r--r--   0 runner    (1001) docker     (127)    92051 2024-04-08 06:12:45.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_fluid/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_fluid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.735798 fake-bpy-module-latest-20240408/bl_ui/properties_physics_geometry_nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-08 06:12:52.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_geometry_nodes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_geometry_nodes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.735798 fake-bpy-module-latest-20240408/bl_ui/properties_physics_rigidbody/
+-rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-04-08 06:12:48.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_rigidbody/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_rigidbody/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.735798 fake-bpy-module-latest-20240408/bl_ui/properties_physics_rigidbody_constraint/
+-rw-r--r--   0 runner    (1001) docker     (127)    31264 2024-04-08 06:12:49.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_rigidbody_constraint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_rigidbody_constraint/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.735798 fake-bpy-module-latest-20240408/bl_ui/properties_physics_softbody/
+-rw-r--r--   0 runner    (1001) docker     (127)    36573 2024-04-08 06:12:50.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_softbody/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_physics_softbody/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.739798 fake-bpy-module-latest-20240408/bl_ui/properties_render/
+-rw-r--r--   0 runner    (1001) docker     (127)   124916 2024-04-08 06:12:48.000000 fake-bpy-module-latest-20240408/bl_ui/properties_render/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_render/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.739798 fake-bpy-module-latest-20240408/bl_ui/properties_scene/
+-rw-r--r--   0 runner    (1001) docker     (127)    33211 2024-04-08 06:12:47.000000 fake-bpy-module-latest-20240408/bl_ui/properties_scene/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_scene/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.739798 fake-bpy-module-latest-20240408/bl_ui/properties_texture/
+-rw-r--r--   0 runner    (1001) docker     (127)    62820 2024-04-08 06:12:49.000000 fake-bpy-module-latest-20240408/bl_ui/properties_texture/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_texture/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.739798 fake-bpy-module-latest-20240408/bl_ui/properties_view_layer/
+-rw-r--r--   0 runner    (1001) docker     (127)    42615 2024-04-08 06:12:49.000000 fake-bpy-module-latest-20240408/bl_ui/properties_view_layer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_view_layer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.739798 fake-bpy-module-latest-20240408/bl_ui/properties_workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)     9707 2024-04-08 06:12:51.000000 fake-bpy-module-latest-20240408/bl_ui/properties_workspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_workspace/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.739798 fake-bpy-module-latest-20240408/bl_ui/properties_world/
+-rw-r--r--   0 runner    (1001) docker     (127)    16818 2024-04-08 06:12:51.000000 fake-bpy-module-latest-20240408/bl_ui/properties_world/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/properties_world/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.739798 fake-bpy-module-latest-20240408/bl_ui/space_clip/
+-rw-r--r--   0 runner    (1001) docker     (127)   175596 2024-04-08 06:12:47.000000 fake-bpy-module-latest-20240408/bl_ui/space_clip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_clip/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.739798 fake-bpy-module-latest-20240408/bl_ui/space_console/
+-rw-r--r--   0 runner    (1001) docker     (127)    15952 2024-04-08 06:12:46.000000 fake-bpy-module-latest-20240408/bl_ui/space_console/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_console/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.739798 fake-bpy-module-latest-20240408/bl_ui/space_dopesheet/
+-rw-r--r--   0 runner    (1001) docker     (127)    67891 2024-04-08 06:12:46.000000 fake-bpy-module-latest-20240408/bl_ui/space_dopesheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_dopesheet/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.743798 fake-bpy-module-latest-20240408/bl_ui/space_filebrowser/
+-rw-r--r--   0 runner    (1001) docker     (127)    74428 2024-04-08 06:12:50.000000 fake-bpy-module-latest-20240408/bl_ui/space_filebrowser/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_filebrowser/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.743798 fake-bpy-module-latest-20240408/bl_ui/space_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)    52963 2024-04-08 06:12:51.000000 fake-bpy-module-latest-20240408/bl_ui/space_graph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_graph/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.743798 fake-bpy-module-latest-20240408/bl_ui/space_image/
+-rw-r--r--   0 runner    (1001) docker     (127)   191743 2024-04-08 06:12:45.000000 fake-bpy-module-latest-20240408/bl_ui/space_image/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_image/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.743798 fake-bpy-module-latest-20240408/bl_ui/space_info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-04-08 06:12:51.000000 fake-bpy-module-latest-20240408/bl_ui/space_info/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_info/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.743798 fake-bpy-module-latest-20240408/bl_ui/space_nla/
+-rw-r--r--   0 runner    (1001) docker     (127)    45091 2024-04-08 06:12:51.000000 fake-bpy-module-latest-20240408/bl_ui/space_nla/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_nla/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.743798 fake-bpy-module-latest-20240408/bl_ui/space_node/
+-rw-r--r--   0 runner    (1001) docker     (127)    88748 2024-04-08 06:12:49.000000 fake-bpy-module-latest-20240408/bl_ui/space_node/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_node/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.743798 fake-bpy-module-latest-20240408/bl_ui/space_outliner/
+-rw-r--r--   0 runner    (1001) docker     (127)    37796 2024-04-08 06:12:49.000000 fake-bpy-module-latest-20240408/bl_ui/space_outliner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_outliner/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.743798 fake-bpy-module-latest-20240408/bl_ui/space_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-08 06:12:49.000000 fake-bpy-module-latest-20240408/bl_ui/space_properties/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_properties/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.747798 fake-bpy-module-latest-20240408/bl_ui/space_sequencer/
+-rw-r--r--   0 runner    (1001) docker     (127)   190965 2024-04-08 06:12:44.000000 fake-bpy-module-latest-20240408/bl_ui/space_sequencer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_sequencer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.747798 fake-bpy-module-latest-20240408/bl_ui/space_spreadsheet/
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-08 06:12:52.000000 fake-bpy-module-latest-20240408/bl_ui/space_spreadsheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_spreadsheet/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.747798 fake-bpy-module-latest-20240408/bl_ui/space_statusbar/
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-08 06:12:52.000000 fake-bpy-module-latest-20240408/bl_ui/space_statusbar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_statusbar/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.747798 fake-bpy-module-latest-20240408/bl_ui/space_text/
+-rw-r--r--   0 runner    (1001) docker     (127)    41578 2024-04-08 06:12:49.000000 fake-bpy-module-latest-20240408/bl_ui/space_text/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_text/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.747798 fake-bpy-module-latest-20240408/bl_ui/space_time/
+-rw-r--r--   0 runner    (1001) docker     (127)    18567 2024-04-08 06:12:47.000000 fake-bpy-module-latest-20240408/bl_ui/space_time/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_time/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.747798 fake-bpy-module-latest-20240408/bl_ui/space_toolsystem_common/
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-08 06:12:50.000000 fake-bpy-module-latest-20240408/bl_ui/space_toolsystem_common/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_toolsystem_common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.747798 fake-bpy-module-latest-20240408/bl_ui/space_toolsystem_toolbar/
+-rw-r--r--   0 runner    (1001) docker     (127)    24608 2024-04-08 06:12:46.000000 fake-bpy-module-latest-20240408/bl_ui/space_toolsystem_toolbar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_toolsystem_toolbar/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.747798 fake-bpy-module-latest-20240408/bl_ui/space_topbar/
+-rw-r--r--   0 runner    (1001) docker     (127)    68597 2024-04-08 06:12:48.000000 fake-bpy-module-latest-20240408/bl_ui/space_topbar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_topbar/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.747798 fake-bpy-module-latest-20240408/bl_ui/space_userpref/
+-rw-r--r--   0 runner    (1001) docker     (127)   208885 2024-04-08 06:12:45.000000 fake-bpy-module-latest-20240408/bl_ui/space_userpref/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_userpref/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.751798 fake-bpy-module-latest-20240408/bl_ui/space_view3d/
+-rw-r--r--   0 runner    (1001) docker     (127)   685989 2024-04-08 06:12:45.000000 fake-bpy-module-latest-20240408/bl_ui/space_view3d/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_view3d/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.751798 fake-bpy-module-latest-20240408/bl_ui/space_view3d_toolbar/
+-rw-r--r--   0 runner    (1001) docker     (127)   259201 2024-04-08 06:12:45.000000 fake-bpy-module-latest-20240408/bl_ui/space_view3d_toolbar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/space_view3d_toolbar/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.751798 fake-bpy-module-latest-20240408/bl_ui/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-08 06:12:52.000000 fake-bpy-module-latest-20240408/bl_ui/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.751798 fake-bpy-module-latest-20240408/bl_ui_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 06:12:55.000000 fake-bpy-module-latest-20240408/bl_ui_utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.751798 fake-bpy-module-latest-20240408/bl_ui_utils/bug_report_url/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-08 06:12:56.000000 fake-bpy-module-latest-20240408/bl_ui_utils/bug_report_url/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui_utils/bug_report_url/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.751798 fake-bpy-module-latest-20240408/bl_ui_utils/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-08 06:12:56.000000 fake-bpy-module-latest-20240408/bl_ui_utils/layout/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui_utils/layout/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bl_ui_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.751798 fake-bpy-module-latest-20240408/blend_render_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 06:12:55.000000 fake-bpy-module-latest-20240408/blend_render_info/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/blend_render_info/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.751798 fake-bpy-module-latest-20240408/blf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-08 06:12:37.000000 fake-bpy-module-latest-20240408/blf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/blf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.751798 fake-bpy-module-latest-20240408/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-08 06:12:40.000000 fake-bpy-module-latest-20240408/bmesh/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.751798 fake-bpy-module-latest-20240408/bmesh/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 06:12:41.000000 fake-bpy-module-latest-20240408/bmesh/geometry/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bmesh/geometry/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.751798 fake-bpy-module-latest-20240408/bmesh/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)    70887 2024-04-08 06:12:41.000000 fake-bpy-module-latest-20240408/bmesh/ops/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bmesh/ops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bmesh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.755798 fake-bpy-module-latest-20240408/bmesh/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    39319 2024-04-08 06:12:41.000000 fake-bpy-module-latest-20240408/bmesh/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bmesh/types/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.755798 fake-bpy-module-latest-20240408/bmesh/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-08 06:12:41.000000 fake-bpy-module-latest-20240408/bmesh/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bmesh/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.755798 fake-bpy-module-latest-20240408/bpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.755798 fake-bpy-module-latest-20240408/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-08 06:12:29.000000 fake-bpy-module-latest-20240408/bpy/app/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.755798 fake-bpy-module-latest-20240408/bpy/app/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-08 06:12:29.000000 fake-bpy-module-latest-20240408/bpy/app/handlers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/app/handlers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.755798 fake-bpy-module-latest-20240408/bpy/app/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-08 06:12:29.000000 fake-bpy-module-latest-20240408/bpy/app/icons/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/app/icons/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/app/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.755798 fake-bpy-module-latest-20240408/bpy/app/timers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-08 06:12:29.000000 fake-bpy-module-latest-20240408/bpy/app/timers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/app/timers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.755798 fake-bpy-module-latest-20240408/bpy/app/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-08 06:12:30.000000 fake-bpy-module-latest-20240408/bpy/app/translations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/app/translations/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.755798 fake-bpy-module-latest-20240408/bpy/msgbus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-08 06:12:37.000000 fake-bpy-module-latest-20240408/bpy/msgbus/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/msgbus/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.755798 fake-bpy-module-latest-20240408/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-08 06:12:30.000000 fake-bpy-module-latest-20240408/bpy/ops/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.755798 fake-bpy-module-latest-20240408/bpy/ops/action/
+-rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-04-08 06:12:34.000000 fake-bpy-module-latest-20240408/bpy/ops/action/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/action/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.755798 fake-bpy-module-latest-20240408/bpy/ops/anim/
+-rw-r--r--   0 runner    (1001) docker     (127)    27997 2024-04-08 06:12:30.000000 fake-bpy-module-latest-20240408/bpy/ops/anim/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/anim/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.759798 fake-bpy-module-latest-20240408/bpy/ops/armature/
+-rw-r--r--   0 runner    (1001) docker     (127)    24971 2024-04-08 06:12:35.000000 fake-bpy-module-latest-20240408/bpy/ops/armature/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/armature/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.759798 fake-bpy-module-latest-20240408/bpy/ops/asset/
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-04-08 06:12:34.000000 fake-bpy-module-latest-20240408/bpy/ops/asset/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/asset/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.759798 fake-bpy-module-latest-20240408/bpy/ops/boid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-08 06:12:34.000000 fake-bpy-module-latest-20240408/bpy/ops/boid/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/boid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.759798 fake-bpy-module-latest-20240408/bpy/ops/brush/
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-08 06:12:35.000000 fake-bpy-module-latest-20240408/bpy/ops/brush/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/brush/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.759798 fake-bpy-module-latest-20240408/bpy/ops/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-08 06:12:33.000000 fake-bpy-module-latest-20240408/bpy/ops/buttons/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/buttons/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.759798 fake-bpy-module-latest-20240408/bpy/ops/cachefile/
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-04-08 06:12:36.000000 fake-bpy-module-latest-20240408/bpy/ops/cachefile/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/cachefile/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.759798 fake-bpy-module-latest-20240408/bpy/ops/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-08 06:12:33.000000 fake-bpy-module-latest-20240408/bpy/ops/camera/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/camera/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.759798 fake-bpy-module-latest-20240408/bpy/ops/clip/
+-rw-r--r--   0 runner    (1001) docker     (127)    52196 2024-04-08 06:12:36.000000 fake-bpy-module-latest-20240408/bpy/ops/clip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/clip/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.759798 fake-bpy-module-latest-20240408/bpy/ops/cloth/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-08 06:12:34.000000 fake-bpy-module-latest-20240408/bpy/ops/cloth/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/cloth/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.759798 fake-bpy-module-latest-20240408/bpy/ops/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-08 06:12:31.000000 fake-bpy-module-latest-20240408/bpy/ops/collection/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/collection/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.759798 fake-bpy-module-latest-20240408/bpy/ops/console/
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-08 06:12:33.000000 fake-bpy-module-latest-20240408/bpy/ops/console/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/console/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.759798 fake-bpy-module-latest-20240408/bpy/ops/constraint/
+-rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-04-08 06:12:33.000000 fake-bpy-module-latest-20240408/bpy/ops/constraint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/constraint/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.763798 fake-bpy-module-latest-20240408/bpy/ops/curve/
+-rw-r--r--   0 runner    (1001) docker     (127)    30992 2024-04-08 06:12:33.000000 fake-bpy-module-latest-20240408/bpy/ops/curve/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/curve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.763798 fake-bpy-module-latest-20240408/bpy/ops/curves/
+-rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-04-08 06:12:36.000000 fake-bpy-module-latest-20240408/bpy/ops/curves/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/curves/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.763798 fake-bpy-module-latest-20240408/bpy/ops/cycles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-08 06:12:33.000000 fake-bpy-module-latest-20240408/bpy/ops/cycles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/cycles/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.763798 fake-bpy-module-latest-20240408/bpy/ops/dpaint/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-08 06:12:35.000000 fake-bpy-module-latest-20240408/bpy/ops/dpaint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/dpaint/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.763798 fake-bpy-module-latest-20240408/bpy/ops/ed/
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-04-08 06:12:32.000000 fake-bpy-module-latest-20240408/bpy/ops/ed/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/ed/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.763798 fake-bpy-module-latest-20240408/bpy/ops/export_anim/
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-08 06:12:30.000000 fake-bpy-module-latest-20240408/bpy/ops/export_anim/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/export_anim/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.763798 fake-bpy-module-latest-20240408/bpy/ops/export_mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-08 06:12:35.000000 fake-bpy-module-latest-20240408/bpy/ops/export_mesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/export_mesh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.763798 fake-bpy-module-latest-20240408/bpy/ops/export_scene/
+-rw-r--r--   0 runner    (1001) docker     (127)    42387 2024-04-08 06:12:36.000000 fake-bpy-module-latest-20240408/bpy/ops/export_scene/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/export_scene/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.763798 fake-bpy-module-latest-20240408/bpy/ops/file/
+-rw-r--r--   0 runner    (1001) docker     (127)    23620 2024-04-08 06:12:35.000000 fake-bpy-module-latest-20240408/bpy/ops/file/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/file/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.763798 fake-bpy-module-latest-20240408/bpy/ops/fluid/
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-08 06:12:31.000000 fake-bpy-module-latest-20240408/bpy/ops/fluid/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/fluid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.763798 fake-bpy-module-latest-20240408/bpy/ops/font/
+-rw-r--r--   0 runner    (1001) docker     (127)    17772 2024-04-08 06:12:31.000000 fake-bpy-module-latest-20240408/bpy/ops/font/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/font/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.763798 fake-bpy-module-latest-20240408/bpy/ops/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-08 06:12:31.000000 fake-bpy-module-latest-20240408/bpy/ops/geometry/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/geometry/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/gizmogroup/
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-08 06:12:32.000000 fake-bpy-module-latest-20240408/bpy/ops/gizmogroup/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/gizmogroup/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/gpencil/
+-rw-r--r--   0 runner    (1001) docker     (127)   100401 2024-04-08 06:12:30.000000 fake-bpy-module-latest-20240408/bpy/ops/gpencil/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/gpencil/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)    47020 2024-04-08 06:12:32.000000 fake-bpy-module-latest-20240408/bpy/ops/graph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/graph/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/grease_pencil/
+-rw-r--r--   0 runner    (1001) docker     (127)    28042 2024-04-08 06:12:33.000000 fake-bpy-module-latest-20240408/bpy/ops/grease_pencil/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/grease_pencil/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)    44935 2024-04-08 06:12:32.000000 fake-bpy-module-latest-20240408/bpy/ops/image/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/image/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/import_anim/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-08 06:12:33.000000 fake-bpy-module-latest-20240408/bpy/ops/import_anim/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/import_anim/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/import_curve/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-08 06:12:33.000000 fake-bpy-module-latest-20240408/bpy/ops/import_curve/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/import_curve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/import_mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-08 06:12:31.000000 fake-bpy-module-latest-20240408/bpy/ops/import_mesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/import_mesh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/import_scene/
+-rw-r--r--   0 runner    (1001) docker     (127)    10603 2024-04-08 06:12:31.000000 fake-bpy-module-latest-20240408/bpy/ops/import_scene/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/import_scene/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-08 06:12:36.000000 fake-bpy-module-latest-20240408/bpy/ops/info/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/info/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-08 06:12:36.000000 fake-bpy-module-latest-20240408/bpy/ops/lattice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/lattice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/marker/
+-rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-04-08 06:12:31.000000 fake-bpy-module-latest-20240408/bpy/ops/marker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/marker/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.767798 fake-bpy-module-latest-20240408/bpy/ops/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-04-08 06:12:32.000000 fake-bpy-module-latest-20240408/bpy/ops/mask/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/mask/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.771798 fake-bpy-module-latest-20240408/bpy/ops/material/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-08 06:12:36.000000 fake-bpy-module-latest-20240408/bpy/ops/material/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/material/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.771798 fake-bpy-module-latest-20240408/bpy/ops/mball/
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-08 06:12:31.000000 fake-bpy-module-latest-20240408/bpy/ops/mball/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/mball/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.771798 fake-bpy-module-latest-20240408/bpy/ops/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)   140802 2024-04-08 06:12:34.000000 fake-bpy-module-latest-20240408/bpy/ops/mesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/mesh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.771798 fake-bpy-module-latest-20240408/bpy/ops/nla/
+-rw-r--r--   0 runner    (1001) docker     (127)    22280 2024-04-08 06:12:34.000000 fake-bpy-module-latest-20240408/bpy/ops/nla/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/nla/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.771798 fake-bpy-module-latest-20240408/bpy/ops/node/
+-rw-r--r--   0 runner    (1001) docker     (127)    56637 2024-04-08 06:12:32.000000 fake-bpy-module-latest-20240408/bpy/ops/node/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/node/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.771798 fake-bpy-module-latest-20240408/bpy/ops/object/
+-rw-r--r--   0 runner    (1001) docker     (127)   187382 2024-04-08 06:12:35.000000 fake-bpy-module-latest-20240408/bpy/ops/object/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/object/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.771798 fake-bpy-module-latest-20240408/bpy/ops/outliner/
+-rw-r--r--   0 runner    (1001) docker     (127)    33247 2024-04-08 06:12:36.000000 fake-bpy-module-latest-20240408/bpy/ops/outliner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/outliner/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.771798 fake-bpy-module-latest-20240408/bpy/ops/paint/
+-rw-r--r--   0 runner    (1001) docker     (127)    37743 2024-04-08 06:12:33.000000 fake-bpy-module-latest-20240408/bpy/ops/paint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/paint/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.771798 fake-bpy-module-latest-20240408/bpy/ops/paintcurve/
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-08 06:12:33.000000 fake-bpy-module-latest-20240408/bpy/ops/paintcurve/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/paintcurve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.771798 fake-bpy-module-latest-20240408/bpy/ops/palette/
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-08 06:12:30.000000 fake-bpy-module-latest-20240408/bpy/ops/palette/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/palette/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.771798 fake-bpy-module-latest-20240408/bpy/ops/particle/
+-rw-r--r--   0 runner    (1001) docker     (127)    16933 2024-04-08 06:12:32.000000 fake-bpy-module-latest-20240408/bpy/ops/particle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/particle/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.775798 fake-bpy-module-latest-20240408/bpy/ops/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)    25918 2024-04-08 06:12:31.000000 fake-bpy-module-latest-20240408/bpy/ops/pose/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/pose/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.775798 fake-bpy-module-latest-20240408/bpy/ops/poselib/
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-08 06:12:30.000000 fake-bpy-module-latest-20240408/bpy/ops/poselib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/poselib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.775798 fake-bpy-module-latest-20240408/bpy/ops/preferences/
+-rw-r--r--   0 runner    (1001) docker     (127)    25658 2024-04-08 06:12:32.000000 fake-bpy-module-latest-20240408/bpy/ops/preferences/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/preferences/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.775798 fake-bpy-module-latest-20240408/bpy/ops/ptcache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-08 06:12:34.000000 fake-bpy-module-latest-20240408/bpy/ops/ptcache/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/ptcache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.775798 fake-bpy-module-latest-20240408/bpy/ops/render/
+-rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-04-08 06:12:34.000000 fake-bpy-module-latest-20240408/bpy/ops/render/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/render/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.775798 fake-bpy-module-latest-20240408/bpy/ops/rigidbody/
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-08 06:12:34.000000 fake-bpy-module-latest-20240408/bpy/ops/rigidbody/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/rigidbody/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.775798 fake-bpy-module-latest-20240408/bpy/ops/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)    18273 2024-04-08 06:12:30.000000 fake-bpy-module-latest-20240408/bpy/ops/scene/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/scene/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.775798 fake-bpy-module-latest-20240408/bpy/ops/screen/
+-rw-r--r--   0 runner    (1001) docker     (127)    24924 2024-04-08 06:12:32.000000 fake-bpy-module-latest-20240408/bpy/ops/screen/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/screen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.775798 fake-bpy-module-latest-20240408/bpy/ops/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-08 06:12:36.000000 fake-bpy-module-latest-20240408/bpy/ops/script/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/script/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.775798 fake-bpy-module-latest-20240408/bpy/ops/sculpt/
+-rw-r--r--   0 runner    (1001) docker     (127)    34542 2024-04-08 06:12:31.000000 fake-bpy-module-latest-20240408/bpy/ops/sculpt/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/sculpt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.775798 fake-bpy-module-latest-20240408/bpy/ops/sculpt_curves/
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-08 06:12:32.000000 fake-bpy-module-latest-20240408/bpy/ops/sculpt_curves/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/sculpt_curves/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.775798 fake-bpy-module-latest-20240408/bpy/ops/sequencer/
+-rw-r--r--   0 runner    (1001) docker     (127)    82020 2024-04-08 06:12:30.000000 fake-bpy-module-latest-20240408/bpy/ops/sequencer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/sequencer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.779798 fake-bpy-module-latest-20240408/bpy/ops/sound/
+-rw-r--r--   0 runner    (1001) docker     (127)    18620 2024-04-08 06:12:36.000000 fake-bpy-module-latest-20240408/bpy/ops/sound/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/sound/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.779798 fake-bpy-module-latest-20240408/bpy/ops/spreadsheet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-08 06:12:31.000000 fake-bpy-module-latest-20240408/bpy/ops/spreadsheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/spreadsheet/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.779798 fake-bpy-module-latest-20240408/bpy/ops/surface/
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-08 06:12:30.000000 fake-bpy-module-latest-20240408/bpy/ops/surface/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/surface/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.779798 fake-bpy-module-latest-20240408/bpy/ops/text/
+-rw-r--r--   0 runner    (1001) docker     (127)    25158 2024-04-08 06:12:33.000000 fake-bpy-module-latest-20240408/bpy/ops/text/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/text/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.779798 fake-bpy-module-latest-20240408/bpy/ops/text_editor/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-08 06:12:36.000000 fake-bpy-module-latest-20240408/bpy/ops/text_editor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/text_editor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.779798 fake-bpy-module-latest-20240408/bpy/ops/texture/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-08 06:12:34.000000 fake-bpy-module-latest-20240408/bpy/ops/texture/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/texture/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.779798 fake-bpy-module-latest-20240408/bpy/ops/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)    61699 2024-04-08 06:12:30.000000 fake-bpy-module-latest-20240408/bpy/ops/transform/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/transform/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.779798 fake-bpy-module-latest-20240408/bpy/ops/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    14340 2024-04-08 06:12:35.000000 fake-bpy-module-latest-20240408/bpy/ops/ui/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/ui/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.779798 fake-bpy-module-latest-20240408/bpy/ops/uilist/
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-08 06:12:35.000000 fake-bpy-module-latest-20240408/bpy/ops/uilist/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/uilist/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.779798 fake-bpy-module-latest-20240408/bpy/ops/uv/
+-rw-r--r--   0 runner    (1001) docker     (127)    46784 2024-04-08 06:12:35.000000 fake-bpy-module-latest-20240408/bpy/ops/uv/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/uv/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.779798 fake-bpy-module-latest-20240408/bpy/ops/view2d/
+-rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-04-08 06:12:31.000000 fake-bpy-module-latest-20240408/bpy/ops/view2d/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/view2d/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.779798 fake-bpy-module-latest-20240408/bpy/ops/view3d/
+-rw-r--r--   0 runner    (1001) docker     (127)    37160 2024-04-08 06:12:34.000000 fake-bpy-module-latest-20240408/bpy/ops/view3d/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/view3d/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.783798 fake-bpy-module-latest-20240408/bpy/ops/wm/
+-rw-r--r--   0 runner    (1001) docker     (127)   231946 2024-04-08 06:12:35.000000 fake-bpy-module-latest-20240408/bpy/ops/wm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/wm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.783798 fake-bpy-module-latest-20240408/bpy/ops/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-08 06:12:34.000000 fake-bpy-module-latest-20240408/bpy/ops/workspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/workspace/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.783798 fake-bpy-module-latest-20240408/bpy/ops/world/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 06:12:32.000000 fake-bpy-module-latest-20240408/bpy/ops/world/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/ops/world/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.783798 fake-bpy-module-latest-20240408/bpy/path/
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-08 06:12:36.000000 fake-bpy-module-latest-20240408/bpy/path/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/path/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.783798 fake-bpy-module-latest-20240408/bpy/props/
+-rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-04-08 06:12:37.000000 fake-bpy-module-latest-20240408/bpy/props/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/props/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.787798 fake-bpy-module-latest-20240408/bpy/types/
+-rw-r--r--   0 runner    (1001) docker     (127)  3254021 2024-04-08 06:12:29.000000 fake-bpy-module-latest-20240408/bpy/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/types/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.787798 fake-bpy-module-latest-20240408/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-04-08 06:12:37.000000 fake-bpy-module-latest-20240408/bpy/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.787798 fake-bpy-module-latest-20240408/bpy/utils/previews/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-08 06:12:37.000000 fake-bpy-module-latest-20240408/bpy/utils/previews/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/utils/previews/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.787798 fake-bpy-module-latest-20240408/bpy/utils/units/
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-08 06:12:37.000000 fake-bpy-module-latest-20240408/bpy/utils/units/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy/utils/units/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.787798 fake-bpy-module-latest-20240408/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 06:12:39.000000 fake-bpy-module-latest-20240408/bpy_extras/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.787798 fake-bpy-module-latest-20240408/bpy_extras/anim_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-08 06:12:40.000000 fake-bpy-module-latest-20240408/bpy_extras/anim_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_extras/anim_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.787798 fake-bpy-module-latest-20240408/bpy_extras/asset_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 06:12:40.000000 fake-bpy-module-latest-20240408/bpy_extras/asset_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_extras/asset_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.787798 fake-bpy-module-latest-20240408/bpy_extras/id_map_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-08 06:12:40.000000 fake-bpy-module-latest-20240408/bpy_extras/id_map_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_extras/id_map_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.791798 fake-bpy-module-latest-20240408/bpy_extras/image_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-08 06:12:40.000000 fake-bpy-module-latest-20240408/bpy_extras/image_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_extras/image_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.791798 fake-bpy-module-latest-20240408/bpy_extras/io_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-04-08 06:12:40.000000 fake-bpy-module-latest-20240408/bpy_extras/io_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_extras/io_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.791798 fake-bpy-module-latest-20240408/bpy_extras/keyconfig_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 06:12:40.000000 fake-bpy-module-latest-20240408/bpy_extras/keyconfig_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_extras/keyconfig_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.791798 fake-bpy-module-latest-20240408/bpy_extras/mesh_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-08 06:12:40.000000 fake-bpy-module-latest-20240408/bpy_extras/mesh_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_extras/mesh_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.791798 fake-bpy-module-latest-20240408/bpy_extras/node_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 06:12:40.000000 fake-bpy-module-latest-20240408/bpy_extras/node_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_extras/node_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.791798 fake-bpy-module-latest-20240408/bpy_extras/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-08 06:12:39.000000 fake-bpy-module-latest-20240408/bpy_extras/object_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_extras/object_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_extras/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.791798 fake-bpy-module-latest-20240408/bpy_extras/view3d_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-08 06:12:40.000000 fake-bpy-module-latest-20240408/bpy_extras/view3d_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_extras/view3d_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.791798 fake-bpy-module-latest-20240408/bpy_restrict_state/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-08 06:12:54.000000 fake-bpy-module-latest-20240408/bpy_restrict_state/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_restrict_state/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.791798 fake-bpy-module-latest-20240408/bpy_types/
+-rw-r--r--   0 runner    (1001) docker     (127)    58139 2024-04-08 06:12:54.000000 fake-bpy-module-latest-20240408/bpy_types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/bpy_types/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.791798 fake-bpy-module-latest-20240408/console_python/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 06:12:54.000000 fake-bpy-module-latest-20240408/console_python/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/console_python/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.791798 fake-bpy-module-latest-20240408/console_shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 06:12:53.000000 fake-bpy-module-latest-20240408/console_shell/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/console_shell/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.807798 fake-bpy-module-latest-20240408/fake_bpy_module_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-08 06:13:21.000000 fake-bpy-module-latest-20240408/fake_bpy_module_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-04-08 06:13:21.000000 fake-bpy-module-latest-20240408/fake_bpy_module_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:13:21.000000 fake-bpy-module-latest-20240408/fake_bpy_module_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 06:13:21.000000 fake-bpy-module-latest-20240408/fake_bpy_module_latest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.795798 fake-bpy-module-latest-20240408/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 06:12:39.000000 fake-bpy-module-latest-20240408/freestyle/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.795798 fake-bpy-module-latest-20240408/freestyle/chainingiterators/
+-rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-04-08 06:12:39.000000 fake-bpy-module-latest-20240408/freestyle/chainingiterators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/freestyle/chainingiterators/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.795798 fake-bpy-module-latest-20240408/freestyle/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)    48266 2024-04-08 06:12:39.000000 fake-bpy-module-latest-20240408/freestyle/functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/freestyle/functions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.795798 fake-bpy-module-latest-20240408/freestyle/predicates/
+-rw-r--r--   0 runner    (1001) docker     (127)    14121 2024-04-08 06:12:39.000000 fake-bpy-module-latest-20240408/freestyle/predicates/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/freestyle/predicates/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/freestyle/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.795798 fake-bpy-module-latest-20240408/freestyle/shaders/
+-rw-r--r--   0 runner    (1001) docker     (127)    22831 2024-04-08 06:12:39.000000 fake-bpy-module-latest-20240408/freestyle/shaders/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/freestyle/shaders/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.795798 fake-bpy-module-latest-20240408/freestyle/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    97490 2024-04-08 06:12:39.000000 fake-bpy-module-latest-20240408/freestyle/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/freestyle/types/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.795798 fake-bpy-module-latest-20240408/freestyle/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.795798 fake-bpy-module-latest-20240408/freestyle/utils/ContextFunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-08 06:12:39.000000 fake-bpy-module-latest-20240408/freestyle/utils/ContextFunctions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/freestyle/utils/ContextFunctions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-08 06:12:39.000000 fake-bpy-module-latest-20240408/freestyle/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/freestyle/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.795798 fake-bpy-module-latest-20240408/gpu/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 06:12:38.000000 fake-bpy-module-latest-20240408/gpu/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.795798 fake-bpy-module-latest-20240408/gpu/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-08 06:12:38.000000 fake-bpy-module-latest-20240408/gpu/capabilities/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/gpu/capabilities/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.799798 fake-bpy-module-latest-20240408/gpu/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-08 06:12:39.000000 fake-bpy-module-latest-20240408/gpu/matrix/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/gpu/matrix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.799798 fake-bpy-module-latest-20240408/gpu/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 06:12:39.000000 fake-bpy-module-latest-20240408/gpu/platform/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/gpu/platform/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/gpu/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.799798 fake-bpy-module-latest-20240408/gpu/select/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 06:12:38.000000 fake-bpy-module-latest-20240408/gpu/select/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/gpu/select/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.799798 fake-bpy-module-latest-20240408/gpu/shader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-08 06:12:38.000000 fake-bpy-module-latest-20240408/gpu/shader/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/gpu/shader/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.799798 fake-bpy-module-latest-20240408/gpu/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-08 06:12:38.000000 fake-bpy-module-latest-20240408/gpu/state/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/gpu/state/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.799798 fake-bpy-module-latest-20240408/gpu/texture/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 06:12:38.000000 fake-bpy-module-latest-20240408/gpu/texture/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/gpu/texture/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.799798 fake-bpy-module-latest-20240408/gpu/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    26172 2024-04-08 06:12:38.000000 fake-bpy-module-latest-20240408/gpu/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/gpu/types/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.799798 fake-bpy-module-latest-20240408/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 06:12:38.000000 fake-bpy-module-latest-20240408/gpu_extras/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.799798 fake-bpy-module-latest-20240408/gpu_extras/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-08 06:12:38.000000 fake-bpy-module-latest-20240408/gpu_extras/batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/gpu_extras/batch/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.799798 fake-bpy-module-latest-20240408/gpu_extras/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-08 06:12:38.000000 fake-bpy-module-latest-20240408/gpu_extras/presets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/gpu_extras/presets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/gpu_extras/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.799798 fake-bpy-module-latest-20240408/graphviz_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 06:12:56.000000 fake-bpy-module-latest-20240408/graphviz_export/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/graphviz_export/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.799798 fake-bpy-module-latest-20240408/idprop/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 06:12:41.000000 fake-bpy-module-latest-20240408/idprop/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/idprop/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.803798 fake-bpy-module-latest-20240408/idprop/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-08 06:12:41.000000 fake-bpy-module-latest-20240408/idprop/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/idprop/types/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.803798 fake-bpy-module-latest-20240408/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-08 06:12:41.000000 fake-bpy-module-latest-20240408/imbuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/imbuf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.803798 fake-bpy-module-latest-20240408/imbuf/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-08 06:12:41.000000 fake-bpy-module-latest-20240408/imbuf/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/imbuf/types/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.803798 fake-bpy-module-latest-20240408/keyingsets_builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)    48336 2024-04-08 06:12:53.000000 fake-bpy-module-latest-20240408/keyingsets_builtins/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/keyingsets_builtins/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.803798 fake-bpy-module-latest-20240408/keyingsets_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-08 06:12:56.000000 fake-bpy-module-latest-20240408/keyingsets_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/keyingsets_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.803798 fake-bpy-module-latest-20240408/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (127)    72812 2024-04-08 06:12:37.000000 fake-bpy-module-latest-20240408/mathutils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.803798 fake-bpy-module-latest-20240408/mathutils/bvhtree/
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-08 06:12:38.000000 fake-bpy-module-latest-20240408/mathutils/bvhtree/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/mathutils/bvhtree/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.803798 fake-bpy-module-latest-20240408/mathutils/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)    21014 2024-04-08 06:12:37.000000 fake-bpy-module-latest-20240408/mathutils/geometry/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/mathutils/geometry/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.803798 fake-bpy-module-latest-20240408/mathutils/interpolate/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 06:12:37.000000 fake-bpy-module-latest-20240408/mathutils/interpolate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/mathutils/interpolate/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.803798 fake-bpy-module-latest-20240408/mathutils/kdtree/
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-08 06:12:38.000000 fake-bpy-module-latest-20240408/mathutils/kdtree/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/mathutils/kdtree/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.803798 fake-bpy-module-latest-20240408/mathutils/noise/
+-rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-04-08 06:12:37.000000 fake-bpy-module-latest-20240408/mathutils/noise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/mathutils/noise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/mathutils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.803798 fake-bpy-module-latest-20240408/nodeitems_builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-08 06:12:54.000000 fake-bpy-module-latest-20240408/nodeitems_builtins/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/nodeitems_builtins/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.807798 fake-bpy-module-latest-20240408/nodeitems_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-08 06:12:54.000000 fake-bpy-module-latest-20240408/nodeitems_utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/nodeitems_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-08 06:13:19.000000 fake-bpy-module-latest-20240408/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.807798 fake-bpy-module-latest-20240408/rna_info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-08 06:12:54.000000 fake-bpy-module-latest-20240408/rna_info/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/rna_info/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.807798 fake-bpy-module-latest-20240408/rna_keymap_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-08 06:12:56.000000 fake-bpy-module-latest-20240408/rna_keymap_ui/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/rna_keymap_ui/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.807798 fake-bpy-module-latest-20240408/rna_prop_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-08 06:12:53.000000 fake-bpy-module-latest-20240408/rna_prop_ui/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/rna_prop_ui/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.807798 fake-bpy-module-latest-20240408/rna_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-08 06:12:55.000000 fake-bpy-module-latest-20240408/rna_xml/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/rna_xml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 06:13:21.807798 fake-bpy-module-latest-20240408/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-08 06:13:19.000000 fake-bpy-module-latest-20240408/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:13:21.807798 fake-bpy-module-latest-20240408/sys_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 06:12:56.000000 fake-bpy-module-latest-20240408/sys_info/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:12:28.000000 fake-bpy-module-latest-20240408/sys_info/py.typed
```

### Comparing `fake-bpy-module-latest-20240407/PKG-INFO` & `fake-bpy-module-latest-20240408/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake-bpy-module-latest
-Version: 20240407
+Version: 20240408
 Summary: Collection of the fake Blender Python API module for the code completion.
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 Project-URL: Homepage, https://github.com/nutti/fake-bpy-module
 Project-URL: Documentation, https://github.com/nutti/fake-bpy-module/blob/master/README.md
```

### Comparing `fake-bpy-module-latest-20240407/README.md` & `fake-bpy-module-latest-20240408/README.md`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/addon_utils/__init__.pyi` & `fake-bpy-module-latest-20240408/addon_utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/animsys_refactor/__init__.pyi` & `fake-bpy-module-latest-20240408/animsys_refactor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/aud/__init__.pyi` & `fake-bpy-module-latest-20240408/aud/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bgl/__init__.pyi` & `fake-bpy-module-latest-20240408/bgl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_app_override/helpers/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_app_override/helpers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_i18n_utils/bl_extract_messages/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_i18n_utils/bl_extract_messages/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_i18n_utils/settings/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_i18n_utils/settings/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_i18n_utils/utils/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_i18n_utils/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_keymap_utils/io/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_keymap_utils/io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_math/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/add_mesh_torus/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/add_mesh_torus/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/anim/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/anim/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/assets/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/assets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/bmesh/find_adjacent/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/bmesh/find_adjacent/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/clip/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/clip/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/console/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/console/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/constraint/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/constraint/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/file/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/file/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/freestyle/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/freestyle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/geometry_nodes/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/geometry_nodes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/image/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/image/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/mesh/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/mesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/node/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/node/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/object/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/object/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/object_align/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/object_align/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/object_quick_effects/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/object_quick_effects/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/object_randomize_transform/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/object_randomize_transform/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/presets/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/presets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/rigidbody/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/rigidbody/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/screen_play_rendered_anim/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/screen_play_rendered_anim/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/sequencer/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/sequencer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/spreadsheet/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/spreadsheet/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/userpref/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/userpref/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/uvcalc_follow_active/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/uvcalc_follow_active/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/uvcalc_lightmap/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/uvcalc_lightmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/uvcalc_transform/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/uvcalc_transform/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/vertexpaint_dirt/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/vertexpaint_dirt/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/view3d/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/view3d/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_operators/wm/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_operators/wm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_previews_utils/bl_previews_render/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_previews_utils/bl_previews_render/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/anim/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/anim/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/asset_shelf/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/asset_shelf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/generic_ui_list/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/generic_ui_list/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/node_add_menu/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/node_add_menu/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/node_add_menu_compositor/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/node_add_menu_compositor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/node_add_menu_geometry/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/node_add_menu_geometry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/node_add_menu_shader/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/node_add_menu_shader/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/node_add_menu_texture/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/node_add_menu_texture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_animviz/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_animviz/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_collection/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_collection/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_constraint/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_constraint/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_armature/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_armature/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_bone/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_bone/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_camera/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_curve/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_curve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_curves/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_curves/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_empty/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_empty/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_gpencil/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_gpencil/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_grease_pencil/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_grease_pencil/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_lattice/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_lattice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_light/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_light/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_lightprobe/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_lightprobe/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_mesh/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_mesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_metaball/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_metaball/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_modifier/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_modifier/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_pointcloud/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_pointcloud/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_shaderfx/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_shaderfx/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_speaker/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_speaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_data_volume/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_data_volume/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_freestyle/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_freestyle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_grease_pencil_common/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_grease_pencil_common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_mask_common/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_mask_common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_material/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_material/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_material_gpencil/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_material_gpencil/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_object/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_object/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_output/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_output/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_paint_common/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_paint_common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_particle/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_particle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_physics_cloth/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_physics_cloth/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_physics_common/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_physics_common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_physics_dynamicpaint/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_physics_dynamicpaint/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_physics_field/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_physics_field/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_physics_fluid/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_physics_fluid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_physics_geometry_nodes/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_physics_geometry_nodes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_physics_rigidbody/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_physics_rigidbody/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_physics_rigidbody_constraint/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_physics_rigidbody_constraint/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_physics_softbody/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_physics_softbody/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_render/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_render/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_scene/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_scene/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_texture/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_texture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_view_layer/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_view_layer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_workspace/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_workspace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/properties_world/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/properties_world/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_clip/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_clip/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_console/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_console/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_dopesheet/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_dopesheet/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_filebrowser/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_filebrowser/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_graph/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_graph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_image/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_image/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_info/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_info/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_nla/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_nla/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_node/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_node/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_outliner/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_outliner/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_properties/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_properties/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_sequencer/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_sequencer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_spreadsheet/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_spreadsheet/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_statusbar/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_statusbar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_text/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_text/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_time/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_toolsystem_common/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_toolsystem_common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_toolsystem_toolbar/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_toolsystem_toolbar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_topbar/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_topbar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_userpref/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_userpref/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_view3d/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_view3d/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/space_view3d_toolbar/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/space_view3d_toolbar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bl_ui/utils/__init__.pyi` & `fake-bpy-module-latest-20240408/bl_ui/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/blf/__init__.pyi` & `fake-bpy-module-latest-20240408/blf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bmesh/__init__.pyi` & `fake-bpy-module-latest-20240408/bmesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bmesh/geometry/__init__.pyi` & `fake-bpy-module-latest-20240408/bmesh/geometry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bmesh/ops/__init__.pyi` & `fake-bpy-module-latest-20240408/bmesh/ops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bmesh/types/__init__.pyi` & `fake-bpy-module-latest-20240408/bmesh/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bmesh/utils/__init__.pyi` & `fake-bpy-module-latest-20240408/bmesh/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/app/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/app/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/app/handlers/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/app/handlers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/app/icons/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/app/icons/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/app/timers/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/app/timers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/app/translations/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/app/translations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/msgbus/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/msgbus/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/action/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/action/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/anim/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/anim/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/armature/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/armature/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/asset/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/asset/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/boid/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/boid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/brush/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/brush/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/buttons/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/buttons/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/cachefile/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/cachefile/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/camera/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/clip/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/clip/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/cloth/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/cloth/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/collection/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/collection/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/console/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/console/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/constraint/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/constraint/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/curve/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/curve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/curves/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/curves/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/cycles/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/cycles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/dpaint/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/dpaint/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/ed/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/ed/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/export_anim/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/export_anim/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/export_mesh/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/export_mesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/export_scene/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/export_scene/__init__.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,20 @@
     use_active_collection: typing.Union[bool, typing.Any] = False,
     global_scale: typing.Any = 1.0,
     apply_unit_scale: typing.Union[bool, typing.Any] = True,
     apply_scale_options: typing.Any = "FBX_SCALE_NONE",
     use_space_transform: typing.Union[bool, typing.Any] = True,
     bake_space_transform: typing.Union[bool, typing.Any] = False,
     object_types: typing.Any = {
-        '"EMPTY"',
-        '"OTHER"',
-        '"LIGHT"',
         '"CAMERA"',
-        '"ARMATURE"',
         '"MESH"',
+        '"OTHER"',
+        '"ARMATURE"',
+        '"EMPTY"',
+        '"LIGHT"',
     },
     use_mesh_modifiers: typing.Union[bool, typing.Any] = True,
     use_mesh_modifiers_render: typing.Union[bool, typing.Any] = True,
     mesh_smooth_type: typing.Any = "OFF",
     colors_type: typing.Any = "SRGB",
     prioritize_active_color: typing.Union[bool, typing.Any] = False,
     use_subsurf: typing.Union[bool, typing.Any] = False,
```

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/file/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/file/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/fluid/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/fluid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/font/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/font/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/geometry/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/geometry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/gizmogroup/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/gizmogroup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/gpencil/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/gpencil/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/graph/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/graph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/grease_pencil/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/grease_pencil/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/image/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/image/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/import_anim/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/import_anim/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/import_curve/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/import_curve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/import_mesh/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/import_mesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/import_scene/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/import_scene/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/info/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/info/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/lattice/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/lattice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/marker/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/marker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/mask/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/mask/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/material/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/material/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/mball/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/mball/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/mesh/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/mesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/nla/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/nla/__init__.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -96,19 +96,19 @@
     visual_keying: typing.Union[bool, typing.Any] = False,
     clear_constraints: typing.Union[bool, typing.Any] = False,
     clear_parents: typing.Union[bool, typing.Any] = False,
     use_current_action: typing.Union[bool, typing.Any] = False,
     clean_curves: typing.Union[bool, typing.Any] = False,
     bake_types: typing.Any = {'"POSE"'},
     channel_types: typing.Any = {
-        '"PROPS"',
         '"LOCATION"',
-        '"BBONE"',
+        '"PROPS"',
         '"SCALE"',
         '"ROTATION"',
+        '"BBONE"',
     },
 ):
     """Bake all selected objects location/scale/rotation animation to an action
 
         :type override_context: typing.Union[dict, bpy.types.Context]
         :type execution_context: str
         :type undo: bool
```

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/node/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/node/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/object/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/object/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/outliner/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/outliner/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/paint/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/paint/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/paintcurve/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/paintcurve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/palette/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/palette/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/particle/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/particle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/pose/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/pose/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/poselib/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/poselib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/preferences/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/preferences/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/ptcache/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/ptcache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/render/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/render/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/rigidbody/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/rigidbody/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/scene/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/scene/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/screen/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/screen/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/script/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/script/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/sculpt/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/sculpt/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     area_normal_radius: typing.Any = 0.25,
     strength: typing.Any = 1.0,
     iteration_count: typing.Any = 1,
     event_history: bpy.types.bpy_prop_collection[
         bpy.types.OperatorStrokeElement
     ] = None,
     type: typing.Any = "GRAVITY",
-    force_axis: typing.Any = {'"X"', '"Y"', '"Z"'},
+    force_axis: typing.Any = {'"Y"', '"Z"', '"X"'},
     orientation: typing.Any = "LOCAL",
     cloth_mass: typing.Any = 1.0,
     cloth_damping: typing.Any = 0.0,
     use_face_sets: typing.Union[bool, typing.Any] = False,
     use_collisions: typing.Union[bool, typing.Any] = False,
 ):
     """Applies a cloth simulation deformation to the entire mesh
@@ -595,15 +595,15 @@
     area_normal_radius: typing.Any = 0.25,
     strength: typing.Any = 1.0,
     iteration_count: typing.Any = 1,
     event_history: bpy.types.bpy_prop_collection[
         bpy.types.OperatorStrokeElement
     ] = None,
     type: typing.Any = "INFLATE",
-    deform_axis: typing.Any = {'"X"', '"Y"', '"Z"'},
+    deform_axis: typing.Any = {'"Y"', '"Z"', '"X"'},
     orientation: typing.Any = "LOCAL",
     surface_smooth_shape_preservation: typing.Any = 0.5,
     surface_smooth_current_vertex: typing.Any = 0.5,
     sharpen_smooth_ratio: typing.Any = 0.35,
     sharpen_intensify_detail_strength: typing.Any = 0.0,
     sharpen_curvature_smooth_iterations: typing.Any = 0,
 ):
```

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/sculpt_curves/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/sculpt_curves/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/sequencer/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/sequencer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/sound/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/sound/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/spreadsheet/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/spreadsheet/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/surface/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/surface/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/text/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/text/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/text_editor/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/text_editor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/texture/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/texture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/transform/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/transform/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/ui/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/ui/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/uilist/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/uilist/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/uv/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/uv/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/view2d/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/view2d/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/view3d/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/view3d/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/wm/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/wm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/ops/workspace/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/ops/workspace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/path/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/path/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/props/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/props/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/types/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/types/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -263,823 +263,823 @@
 00001060: 0a0a 2020 2020 6465 6620 5f5f 6c65 6e5f  ..    def __len_
 00001070: 5f28 7365 6c66 2920 2d3e 2047 656e 6572  _(self) -> Gener
 00001080: 6963 5479 7065 3a0a 2020 2020 2020 2020  icType:.        
 00001090: 2222 220a 0a20 2020 2020 2020 203a 7265  """..        :re
 000010a0: 7475 726e 3a0a 2020 2020 2020 2020 3a72  turn:.        :r
 000010b0: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
 000010c0: 2020 2222 220a 2020 2020 2020 2020 2e2e    """.        ..
-000010d0: 2e0a 0a63 6c61 7373 2062 7079 5f73 7472  ...class bpy_str
-000010e0: 7563 7428 7479 7069 6e67 2e47 656e 6572  uct(typing.Gener
-000010f0: 6963 5b47 656e 6572 6963 5479 7065 5d29  ic[GenericType])
-00001100: 3a0a 2020 2020 2222 2262 7569 6c74 2d69  :.    """built-i
-00001110: 6e20 6261 7365 2063 6c61 7373 2066 6f72  n base class for
-00001120: 2061 6c6c 2063 6c61 7373 6573 2069 6e20   all classes in 
-00001130: 6270 792e 7479 7065 732e 2222 220a 0a20  bpy.types.""".. 
-00001140: 2020 2069 645f 6461 7461 3a20 7479 7069     id_data: typi
-00001150: 6e67 2e41 6e79 0a20 2020 2022 2222 2054  ng.Any.    """ T
-00001160: 6865 2060 6270 792e 7479 7065 732e 4944  he `bpy.types.ID
-00001170: 6020 6f62 6a65 6374 2074 6869 7320 6461  ` object this da
-00001180: 7461 626c 6f63 6b20 6973 2066 726f 6d20  tablock is from 
-00001190: 6f72 204e 6f6e 652c 2028 6e6f 7420 6176  or None, (not av
-000011a0: 6169 6c61 626c 6520 666f 7220 616c 6c20  ailable for all 
-000011b0: 6461 7461 2074 7970 6573 2922 2222 0a0a  data types)"""..
-000011c0: 2020 2020 6465 6620 6173 5f70 6f69 6e74      def as_point
-000011d0: 6572 2873 656c 6629 3a0a 2020 2020 2020  er(self):.      
-000011e0: 2020 2222 2252 6574 7572 6e73 2074 6865    """Returns the
-000011f0: 206d 656d 6f72 7920 6164 6472 6573 7320   memory address 
-00001200: 7768 6963 6820 686f 6c64 7320 6120 706f  which holds a po
-00001210: 696e 7465 7220 746f 2042 6c65 6e64 6572  inter to Blender
-00001220: 2773 2069 6e74 6572 6e61 6c20 6461 7461  's internal data
-00001230: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00001240: 6e3a 2069 6e74 2028 6d65 6d6f 7279 2061  n: int (memory a
-00001250: 6464 7265 7373 292e 0a20 2020 2020 2020  ddress)..       
-00001260: 2022 2222 0a20 2020 2020 2020 202e 2e2e   """.        ...
-00001270: 0a0a 2020 2020 6465 6620 6472 6976 6572  ..    def driver
-00001280: 5f61 6464 2873 656c 662c 2070 6174 683a  _add(self, path:
-00001290: 2073 7472 2c20 696e 6465 783d 2d31 293a   str, index=-1):
-000012a0: 0a20 2020 2020 2020 2022 2222 4164 6473  .        """Adds
-000012b0: 2064 7269 7665 7228 7329 2074 6f20 7468   driver(s) to th
-000012c0: 6520 6769 7665 6e20 7072 6f70 6572 7479  e given property
-000012d0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000012e0: 2070 6174 683a 2070 6174 6820 746f 2074   path: path to t
-000012f0: 6865 2070 726f 7065 7274 7920 746f 2064  he property to d
-00001300: 7269 7665 2c20 616e 616c 6f67 6f75 7320  rive, analogous 
-00001310: 746f 2074 6865 2066 6375 7276 6527 7320  to the fcurve's 
-00001320: 6461 7461 2070 6174 682e 0a20 2020 2020  data path..     
-00001330: 2020 203a 7479 7065 2070 6174 683a 2073     :type path: s
-00001340: 7472 0a20 2020 2020 2020 203a 7061 7261  tr.        :para
-00001350: 6d20 696e 6465 783a 2061 7272 6179 2069  m index: array i
-00001360: 6e64 6578 206f 6620 7468 6520 7072 6f70  ndex of the prop
-00001370: 6572 7479 2064 7269 7665 2e20 4465 6661  erty drive. Defa
-00001380: 756c 7473 2074 6f20 2d31 2066 6f72 2061  ults to -1 for a
-00001390: 6c6c 2069 6e64 6963 6573 206f 7220 6120  ll indices or a 
-000013a0: 7369 6e67 6c65 2063 6861 6e6e 656c 2069  single channel i
-000013b0: 6620 7468 6520 7072 6f70 6572 7479 2069  f the property i
-000013c0: 7320 6e6f 7420 616e 2061 7272 6179 2e0a  s not an array..
-000013d0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-000013e0: 2054 6865 2064 7269 7665 7228 7329 2061   The driver(s) a
-000013f0: 6464 6564 2e0a 2020 2020 2020 2020 3a72  dded..        :r
-00001400: 7479 7065 3a20 4643 7572 7665 0a20 2020  type: FCurve.   
-00001410: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00001420: 202e 2e2e 0a0a 2020 2020 6465 6620 6472   .....    def dr
-00001430: 6976 6572 5f72 656d 6f76 6528 7365 6c66  iver_remove(self
-00001440: 2c20 7061 7468 3a20 7374 722c 2069 6e64  , path: str, ind
-00001450: 6578 3d2d 3129 3a0a 2020 2020 2020 2020  ex=-1):.        
-00001460: 2222 2252 656d 6f76 6520 6472 6976 6572  """Remove driver
-00001470: 2873 2920 6672 6f6d 2074 6865 2067 6976  (s) from the giv
-00001480: 656e 2070 726f 7065 7274 790a 0a20 2020  en property..   
-00001490: 2020 2020 203a 7061 7261 6d20 7061 7468       :param path
-000014a0: 3a20 7061 7468 2074 6f20 7468 6520 7072  : path to the pr
-000014b0: 6f70 6572 7479 2074 6f20 6472 6976 652c  operty to drive,
-000014c0: 2061 6e61 6c6f 676f 7573 2074 6f20 7468   analogous to th
-000014d0: 6520 6663 7572 7665 2773 2064 6174 6120  e fcurve's data 
-000014e0: 7061 7468 2e0a 2020 2020 2020 2020 3a74  path..        :t
-000014f0: 7970 6520 7061 7468 3a20 7374 720a 2020  ype path: str.  
-00001500: 2020 2020 2020 3a70 6172 616d 2069 6e64        :param ind
-00001510: 6578 3a20 6172 7261 7920 696e 6465 7820  ex: array index 
-00001520: 6f66 2074 6865 2070 726f 7065 7274 7920  of the property 
-00001530: 6472 6976 652e 2044 6566 6175 6c74 7320  drive. Defaults 
-00001540: 746f 202d 3120 666f 7220 616c 6c20 696e  to -1 for all in
-00001550: 6469 6365 7320 6f72 2061 2073 696e 676c  dices or a singl
-00001560: 6520 6368 616e 6e65 6c20 6966 2074 6865  e channel if the
-00001570: 2070 726f 7065 7274 7920 6973 206e 6f74   property is not
-00001580: 2061 6e20 6172 7261 792e 0a20 2020 2020   an array..     
-00001590: 2020 203a 7265 7475 726e 3a20 5375 6363     :return: Succ
-000015a0: 6573 7320 6f66 2064 7269 7665 7220 7265  ess of driver re
-000015b0: 6d6f 7661 6c2e 0a20 2020 2020 2020 203a  moval..        :
-000015c0: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
-000015d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000015e0: 2e2e 2e0a 0a20 2020 2064 6566 2067 6574  .....    def get
-000015f0: 2873 656c 662c 206b 6579 3a20 7374 722c  (self, key: str,
-00001600: 2064 6566 6175 6c74 3d4e 6f6e 6529 3a0a   default=None):.
-00001610: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00001620: 6e73 2074 6865 2076 616c 7565 206f 6620  ns the value of 
-00001630: 7468 6520 6375 7374 6f6d 2070 726f 7065  the custom prope
-00001640: 7274 7920 6173 7369 676e 6564 2074 6f20  rty assigned to 
-00001650: 6b65 7920 6f72 2064 6566 6175 6c74 0a20  key or default. 
-00001660: 2020 2020 2020 2077 6865 6e20 6e6f 7420         when not 
-00001670: 666f 756e 6420 286d 6174 6368 6573 2050  found (matches P
-00001680: 7974 686f 6e27 7320 6469 6374 696f 6e61  ython's dictiona
-00001690: 7279 2066 756e 6374 696f 6e20 6f66 2074  ry function of t
-000016a0: 6865 2073 616d 6520 6e61 6d65 292e 0a0a  he same name)...
-000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016c0: 3a70 6172 616d 206b 6579 3a20 5468 6520  :param key: The 
-000016d0: 6b65 7920 6173 736f 6369 6174 6564 2077  key associated w
-000016e0: 6974 6820 7468 6520 6375 7374 6f6d 2070  ith the custom p
-000016f0: 726f 7065 7274 792e 0a20 2020 2020 2020  roperty..       
-00001700: 2020 2020 2020 2020 203a 7479 7065 206b           :type k
-00001710: 6579 3a20 7374 720a 2020 2020 2020 2020  ey: str.        
-00001720: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00001730: 6566 6175 6c74 3a20 4f70 7469 6f6e 616c  efault: Optional
-00001740: 2061 7267 756d 656e 7420 666f 7220 7468   argument for th
-00001750: 6520 7661 6c75 6520 746f 2072 6574 7572  e value to retur
-00001760: 6e20 6966 0a20 2020 2020 2020 206b 6579  n if.        key
-00001770: 2069 7320 6e6f 7420 666f 756e 642e 0a20   is not found.. 
-00001780: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00001790: 2020 202e 2e2e 0a0a 2020 2020 6465 6620     .....    def 
-000017a0: 6964 5f70 726f 7065 7274 6965 735f 636c  id_properties_cl
-000017b0: 6561 7228 7365 6c66 293a 0a20 2020 2020  ear(self):.     
-000017c0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-000017d0: 3a72 6574 7572 6e3a 2052 656d 6f76 6520  :return: Remove 
-000017e0: 7468 6520 7061 7265 6e74 2067 726f 7570  the parent group
-000017f0: 2066 6f72 2061 6e20 524e 4120 7374 7275   for an RNA stru
-00001800: 6374 2773 2063 7573 746f 6d20 4944 5072  ct's custom IDPr
-00001810: 6f70 6572 7469 6573 2e0a 2020 2020 2020  operties..      
-00001820: 2020 2222 220a 2020 2020 2020 2020 2e2e    """.        ..
-00001830: 2e0a 0a20 2020 2064 6566 2069 645f 7072  ...    def id_pr
-00001840: 6f70 6572 7469 6573 5f65 6e73 7572 6528  operties_ensure(
-00001850: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00001860: 2222 0a0a 2020 2020 2020 2020 3a72 6574  ""..        :ret
-00001870: 7572 6e3a 2074 6865 2070 6172 656e 7420  urn: the parent 
-00001880: 6772 6f75 7020 666f 7220 616e 2052 4e41  group for an RNA
-00001890: 2073 7472 7563 7427 7320 6375 7374 6f6d   struct's custom
-000018a0: 2049 4450 726f 7065 7274 6965 732e 0a20   IDProperties.. 
-000018b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000018c0: 2020 202e 2e2e 0a0a 2020 2020 6465 6620     .....    def 
-000018d0: 6964 5f70 726f 7065 7274 6965 735f 7569  id_properties_ui
-000018e0: 2873 656c 662c 206b 6579 293a 0a20 2020  (self, key):.   
-000018f0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00001900: 2020 3a70 6172 616d 206b 6579 3a20 5374    :param key: St
-00001910: 7269 6e67 206e 616d 6520 6f66 2074 6865  ring name of the
-00001920: 2070 726f 7065 7274 792e 0a20 2020 2020   property..     
-00001930: 2020 203a 7265 7475 726e 3a20 5265 7475     :return: Retu
-00001940: 726e 2061 6e20 6f62 6a65 6374 2075 7365  rn an object use
-00001950: 6420 746f 206d 616e 6167 6520 616e 2049  d to manage an I
-00001960: 4450 726f 7065 7274 7927 7320 5549 2064  DProperty's UI d
-00001970: 6174 612e 0a20 2020 2020 2020 2022 2222  ata..        """
-00001980: 0a20 2020 2020 2020 202e 2e2e 0a0a 2020  .        .....  
-00001990: 2020 6465 6620 6973 5f70 726f 7065 7274    def is_propert
-000019a0: 795f 6869 6464 656e 2873 656c 662c 2070  y_hidden(self, p
-000019b0: 726f 7065 7274 7929 3a0a 2020 2020 2020  roperty):.      
-000019c0: 2020 2222 2243 6865 636b 2069 6620 6120    """Check if a 
-000019d0: 7072 6f70 6572 7479 2069 7320 6869 6464  property is hidd
-000019e0: 656e 2e0a 0a20 2020 2020 2020 203a 7061  en...        :pa
-000019f0: 7261 6d20 7072 6f70 6572 7479 3a0a 2020  ram property:.  
-00001a00: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
-00001a10: 7275 6520 7768 656e 2074 6865 2070 726f  rue when the pro
-00001a20: 7065 7274 7920 6973 2068 6964 6465 6e2e  perty is hidden.
-00001a30: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00001a40: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
-00001a50: 220a 2020 2020 2020 2020 2e2e 2e0a 0a20  ".        ..... 
-00001a60: 2020 2064 6566 2069 735f 7072 6f70 6572     def is_proper
-00001a70: 7479 5f6f 7665 7272 6964 6162 6c65 5f6c  ty_overridable_l
-00001a80: 6962 7261 7279 2873 656c 662c 2070 726f  ibrary(self, pro
-00001a90: 7065 7274 7929 3a0a 2020 2020 2020 2020  perty):.        
-00001aa0: 2222 2243 6865 636b 2069 6620 6120 7072  """Check if a pr
-00001ab0: 6f70 6572 7479 2069 7320 6f76 6572 7269  operty is overri
-00001ac0: 6461 626c 652e 0a0a 2020 2020 2020 2020  dable...        
-00001ad0: 3a70 6172 616d 2070 726f 7065 7274 793a  :param property:
-00001ae0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00001af0: 3a20 5472 7565 2077 6865 6e20 7468 6520  : True when the 
-00001b00: 7072 6f70 6572 7479 2069 7320 6f76 6572  property is over
-00001b10: 7269 6461 626c 652e 0a20 2020 2020 2020  ridable..       
-00001b20: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
-00001b30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00001b40: 2020 2e2e 2e0a 0a20 2020 2064 6566 2069    .....    def i
-00001b50: 735f 7072 6f70 6572 7479 5f72 6561 646f  s_property_reado
-00001b60: 6e6c 7928 7365 6c66 2c20 7072 6f70 6572  nly(self, proper
-00001b70: 7479 293a 0a20 2020 2020 2020 2022 2222  ty):.        """
-00001b80: 4368 6563 6b20 6966 2061 2070 726f 7065  Check if a prope
-00001b90: 7274 7920 6973 2072 6561 646f 6e6c 792e  rty is readonly.
-00001ba0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00001bb0: 2070 726f 7065 7274 793a 0a20 2020 2020   property:.     
-00001bc0: 2020 203a 7265 7475 726e 3a20 5472 7565     :return: True
-00001bd0: 2077 6865 6e20 7468 6520 7072 6f70 6572   when the proper
-00001be0: 7479 2069 7320 7265 6164 6f6e 6c79 2028  ty is readonly (
-00001bf0: 6e6f 7420 7772 6974 6162 6c65 292e 0a20  not writable).. 
-00001c00: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
-00001c10: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
-00001c20: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
-00001c30: 2064 6566 2069 735f 7072 6f70 6572 7479   def is_property
-00001c40: 5f73 6574 2873 656c 662c 2070 726f 7065  _set(self, prope
-00001c50: 7274 792c 2067 686f 7374 3a20 626f 6f6c  rty, ghost: bool
-00001c60: 203d 2054 7275 6529 202d 3e20 626f 6f6c   = True) -> bool
-00001c70: 3a0a 2020 2020 2020 2020 2222 2243 6865  :.        """Che
-00001c80: 636b 2069 6620 6120 7072 6f70 6572 7479  ck if a property
-00001c90: 2069 7320 7365 742c 2075 7365 2066 6f72   is set, use for
-00001ca0: 2074 6573 7469 6e67 206f 7065 7261 746f   testing operato
-00001cb0: 7220 7072 6f70 6572 7469 6573 2e0a 0a20  r properties... 
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-00001cd0: 7061 7261 6d20 7072 6f70 6572 7479 3a0a  param property:.
-00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cf0: 3a70 6172 616d 2067 686f 7374 3a20 5573  :param ghost: Us
-00001d00: 6564 2066 6f72 206f 7065 7261 746f 7273  ed for operators
-00001d10: 2074 6861 7420 7265 2d72 756e 2077 6974   that re-run wit
-00001d20: 6820 7072 6576 696f 7573 2073 6574 7469  h previous setti
-00001d30: 6e67 732e 0a20 2020 2020 2020 2049 6e20  ngs..        In 
-00001d40: 7468 6973 2063 6173 6520 7468 6520 7072  this case the pr
-00001d50: 6f70 6572 7479 2069 7320 6e6f 7420 6d61  operty is not ma
-00001d60: 726b 6564 2061 7320 7365 742c 0a20 2020  rked as set,.   
-00001d70: 2020 2020 2079 6574 2074 6865 2076 616c       yet the val
-00001d80: 7565 2066 726f 6d20 7468 6520 7072 6576  ue from the prev
-00001d90: 696f 7573 2065 7865 6375 7469 6f6e 2069  ious execution i
-00001da0: 7320 7573 6564 2e0a 0a20 2020 2020 2020  s used...       
-00001db0: 2049 6e20 7261 7265 2063 6173 6573 2079   In rare cases y
-00001dc0: 6f75 206d 6179 2077 616e 7420 746f 2073  ou may want to s
-00001dd0: 6574 2074 6869 7320 6f70 7469 6f6e 2074  et this option t
-00001de0: 6f20 6661 6c73 652e 0a20 2020 2020 2020  o false..       
-00001df0: 2020 2020 2020 2020 203a 7479 7065 2067           :type g
-00001e00: 686f 7374 3a20 626f 6f6c 0a20 2020 2020  host: bool.     
-00001e10: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
-00001e20: 726e 3a20 5472 7565 2077 6865 6e20 7468  rn: True when th
-00001e30: 6520 7072 6f70 6572 7479 2068 6173 2062  e property has b
-00001e40: 6565 6e20 7365 742e 0a20 2020 2020 2020  een set..       
-00001e50: 2020 2020 2020 2020 203a 7274 7970 653a           :rtype:
-00001e60: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
-00001e70: 220a 2020 2020 2020 2020 2e2e 2e0a 0a20  ".        ..... 
-00001e80: 2020 2064 6566 2069 7465 6d73 2873 656c     def items(sel
-00001e90: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
-00001ea0: 2020 2020 2222 2252 6574 7572 6e73 2074      """Returns t
-00001eb0: 6865 2069 7465 6d73 206f 6620 7468 6973  he items of this
-00001ec0: 206f 626a 6563 7473 2063 7573 746f 6d20   objects custom 
-00001ed0: 7072 6f70 6572 7469 6573 2028 6d61 7463  properties (matc
-00001ee0: 6865 7320 5079 7468 6f6e 2773 0a20 2020  hes Python's.   
-00001ef0: 2020 2020 2064 6963 7469 6f6e 6172 7920       dictionary 
-00001f00: 6675 6e63 7469 6f6e 206f 6620 7468 6520  function of the 
-00001f10: 7361 6d65 206e 616d 6529 2e0a 0a20 2020  same name)...   
-00001f20: 2020 2020 2020 2020 2020 2020 203a 7265               :re
-00001f30: 7475 726e 3a20 6375 7374 6f6d 2070 726f  turn: custom pro
-00001f40: 7065 7274 7920 6b65 792c 2076 616c 7565  perty key, value
-00001f50: 2070 6169 7273 2e0a 2020 2020 2020 2020   pairs..        
-00001f60: 2222 220a 2020 2020 2020 2020 2e2e 2e0a  """.        ....
-00001f70: 0a20 2020 2064 6566 206b 6579 6672 616d  .    def keyfram
-00001f80: 655f 6465 6c65 7465 280a 2020 2020 2020  e_delete(.      
-00001f90: 2020 7365 6c66 2c20 6461 7461 5f70 6174    self, data_pat
-00001fa0: 683a 2073 7472 2c20 696e 6465 783d 2d31  h: str, index=-1
-00001fb0: 2c20 6672 616d 653d 4e6f 6e65 2c20 6772  , frame=None, gr
-00001fc0: 6f75 703a 2073 7472 203d 2022 220a 2020  oup: str = "".  
-00001fd0: 2020 2920 2d3e 2073 7472 3a0a 2020 2020    ) -> str:.    
-00001fe0: 2020 2020 2222 2252 656d 6f76 6520 6120      """Remove a 
-00001ff0: 6b65 7966 7261 6d65 2066 726f 6d20 7468  keyframe from th
-00002000: 6973 2070 726f 7065 7274 6965 7320 6663  is properties fc
-00002010: 7572 7665 2e0a 0a20 2020 2020 2020 203a  urve...        :
-00002020: 7061 7261 6d20 6461 7461 5f70 6174 683a  param data_path:
-00002030: 2070 6174 6820 746f 2074 6865 2070 726f   path to the pro
-00002040: 7065 7274 7920 746f 2072 656d 6f76 6520  perty to remove 
-00002050: 6120 6b65 792c 2061 6e61 6c6f 676f 7573  a key, analogous
-00002060: 2074 6f20 7468 6520 6663 7572 7665 2773   to the fcurve's
-00002070: 2064 6174 6120 7061 7468 2e0a 2020 2020   data path..    
-00002080: 2020 2020 3a74 7970 6520 6461 7461 5f70      :type data_p
-00002090: 6174 683a 2073 7472 0a20 2020 2020 2020  ath: str.       
-000020a0: 203a 7061 7261 6d20 696e 6465 783a 2061   :param index: a
-000020b0: 7272 6179 2069 6e64 6578 206f 6620 7468  rray index of th
-000020c0: 6520 7072 6f70 6572 7479 2074 6f20 7265  e property to re
-000020d0: 6d6f 7665 2061 206b 6579 2e20 4465 6661  move a key. Defa
-000020e0: 756c 7473 2074 6f20 2d31 2072 656d 6f76  ults to -1 remov
-000020f0: 696e 6720 616c 6c20 696e 6469 6365 7320  ing all indices 
-00002100: 6f72 2061 2073 696e 676c 6520 6368 616e  or a single chan
-00002110: 6e65 6c20 6966 2074 6865 2070 726f 7065  nel if the prope
-00002120: 7274 7920 6973 206e 6f74 2061 6e20 6172  rty is not an ar
-00002130: 7261 792e 0a20 2020 2020 2020 203a 7061  ray..        :pa
-00002140: 7261 6d20 6672 616d 653a 2054 6865 2066  ram frame: The f
-00002150: 7261 6d65 206f 6e20 7768 6963 6820 7468  rame on which th
-00002160: 6520 6b65 7966 7261 6d65 2069 7320 6465  e keyframe is de
-00002170: 6c65 7465 642c 2064 6566 6175 6c74 696e  leted, defaultin
-00002180: 6720 746f 2074 6865 2063 7572 7265 6e74  g to the current
-00002190: 2066 7261 6d65 2e0a 2020 2020 2020 2020   frame..        
-000021a0: 3a70 6172 616d 2067 726f 7570 3a20 5468  :param group: Th
-000021b0: 6520 6e61 6d65 206f 6620 7468 6520 6772  e name of the gr
-000021c0: 6f75 7020 7468 6520 462d 4375 7276 6520  oup the F-Curve 
-000021d0: 7368 6f75 6c64 2062 6520 6164 6465 6420  should be added 
-000021e0: 746f 2069 6620 6974 2064 6f65 736e 2774  to if it doesn't
-000021f0: 2065 7869 7374 2079 6574 2e0a 2020 2020   exist yet..    
-00002200: 2020 2020 3a74 7970 6520 6772 6f75 703a      :type group:
-00002210: 2073 7472 0a20 2020 2020 2020 203a 7265   str.        :re
-00002220: 7475 726e 3a20 5375 6363 6573 7320 6f66  turn: Success of
-00002230: 206b 6579 6672 616d 6520 6465 6c65 7469   keyframe deleti
-00002240: 6f6e 2e0a 2020 2020 2020 2020 3a72 7479  on..        :rty
-00002250: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
-00002260: 2022 2222 0a20 2020 2020 2020 202e 2e2e   """.        ...
-00002270: 0a0a 2020 2020 6465 6620 6b65 7966 7261  ..    def keyfra
-00002280: 6d65 5f69 6e73 6572 7428 0a20 2020 2020  me_insert(.     
-00002290: 2020 2073 656c 662c 2064 6174 615f 7061     self, data_pa
-000022a0: 7468 3a20 7374 722c 2069 6e64 6578 3d2d  th: str, index=-
-000022b0: 312c 2066 7261 6d65 3d4e 6f6e 652c 2067  1, frame=None, g
-000022c0: 726f 7570 3a20 7374 7220 3d20 2222 2c20  roup: str = "", 
-000022d0: 6f70 7469 6f6e 733d 4e6f 6e65 2829 0a20  options=None(). 
-000022e0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-000022f0: 2249 6e73 6572 7420 6120 6b65 7966 7261  "Insert a keyfra
-00002300: 6d65 206f 6e20 7468 6520 7072 6f70 6572  me on the proper
-00002310: 7479 2067 6976 656e 2c20 6164 6469 6e67  ty given, adding
-00002320: 2066 6375 7276 6573 2061 6e64 2061 6e69   fcurves and ani
-00002330: 6d61 7469 6f6e 2064 6174 6120 7768 656e  mation data when
-00002340: 206e 6563 6573 7361 7279 2e54 6869 7320   necessary.This 
-00002350: 6973 2074 6865 206d 6f73 7420 7369 6d70  is the most simp
-00002360: 6c65 2065 7861 6d70 6c65 206f 6620 696e  le example of in
-00002370: 7365 7274 696e 6720 6120 6b65 7966 7261  serting a keyfra
-00002380: 6d65 2066 726f 6d20 7079 7468 6f6e 2e4e  me from python.N
-00002390: 6f74 6520 7468 6174 2077 6865 6e20 6b65  ote that when ke
-000023a0: 7969 6e67 2064 6174 6120 7061 7468 7320  ying data paths 
-000023b0: 7768 6963 6820 636f 6e74 6169 6e20 6e65  which contain ne
-000023c0: 7374 6564 2070 726f 7065 7274 6965 7320  sted properties 
-000023d0: 7468 6973 206d 7573 7420 6265 0a20 2020  this must be.   
-000023e0: 2020 2020 2064 6f6e 6520 6672 6f6d 2074       done from t
-000023f0: 6865 2060 4944 6020 7375 6263 6c61 7373  he `ID` subclass
-00002400: 2c20 696e 2074 6869 7320 6361 7365 2074  , in this case t
-00002410: 6865 2060 4172 6d61 7475 7265 6020 7261  he `Armature` ra
-00002420: 7468 6572 0a20 2020 2020 2020 2074 6861  ther.        tha
-00002430: 6e20 7468 6520 626f 6e65 2e0a 0a20 2020  n the bone...   
-00002440: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
-00002450: 7261 6d20 6461 7461 5f70 6174 683a 2070  ram data_path: p
-00002460: 6174 6820 746f 2074 6865 2070 726f 7065  ath to the prope
-00002470: 7274 7920 746f 206b 6579 2c20 616e 616c  rty to key, anal
-00002480: 6f67 6f75 7320 746f 2074 6865 2066 6375  ogous to the fcu
-00002490: 7276 6527 7320 6461 7461 2070 6174 682e  rve's data path.
-000024a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000024b0: 203a 7479 7065 2064 6174 615f 7061 7468   :type data_path
-000024c0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-000024d0: 2020 2020 2020 3a70 6172 616d 2069 6e64        :param ind
-000024e0: 6578 3a20 6172 7261 7920 696e 6465 7820  ex: array index 
-000024f0: 6f66 2074 6865 2070 726f 7065 7274 7920  of the property 
-00002500: 746f 206b 6579 2e0a 2020 2020 2020 2020  to key..        
-00002510: 4465 6661 756c 7473 2074 6f20 2d31 2077  Defaults to -1 w
-00002520: 6869 6368 2077 696c 6c20 6b65 7920 616c  hich will key al
-00002530: 6c20 696e 6469 6365 7320 6f72 2061 2073  l indices or a s
-00002540: 696e 676c 6520 6368 616e 6e65 6c20 6966  ingle channel if
-00002550: 2074 6865 2070 726f 7065 7274 7920 6973   the property is
-00002560: 206e 6f74 2061 6e20 6172 7261 792e 0a20   not an array.. 
-00002570: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-00002580: 7061 7261 6d20 6672 616d 653a 2054 6865  param frame: The
-00002590: 2066 7261 6d65 206f 6e20 7768 6963 6820   frame on which 
-000025a0: 7468 6520 6b65 7966 7261 6d65 2069 7320  the keyframe is 
-000025b0: 696e 7365 7274 6564 2c20 6465 6661 756c  inserted, defaul
-000025c0: 7469 6e67 2074 6f20 7468 6520 6375 7272  ting to the curr
-000025d0: 656e 7420 6672 616d 652e 0a20 2020 2020  ent frame..     
-000025e0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-000025f0: 6d20 6772 6f75 703a 2054 6865 206e 616d  m group: The nam
-00002600: 6520 6f66 2074 6865 2067 726f 7570 2074  e of the group t
-00002610: 6865 2046 2d43 7572 7665 2073 686f 756c  he F-Curve shoul
-00002620: 6420 6265 2061 6464 6564 2074 6f20 6966  d be added to if
-00002630: 2069 7420 646f 6573 6e27 7420 6578 6973   it doesn't exis
-00002640: 7420 7965 742e 0a20 2020 2020 2020 2020  t yet..         
-00002650: 2020 2020 2020 203a 7479 7065 2067 726f         :type gro
-00002660: 7570 3a20 7374 720a 2020 2020 2020 2020  up: str.        
-00002670: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
-00002680: 7074 696f 6e73 3a20 4f70 7469 6f6e 616c  ptions: Optional
-00002690: 2073 6574 206f 6620 666c 6167 733a 0a0a   set of flags:..
-000026a0: 2020 2020 2020 2020 494e 5345 5254 4b45          INSERTKE
-000026b0: 595f 4e45 4544 4544 204f 6e6c 7920 696e  Y_NEEDED Only in
-000026c0: 7365 7274 206b 6579 6672 616d 6573 2077  sert keyframes w
-000026d0: 6865 7265 2074 6865 7927 7265 206e 6565  here they're nee
-000026e0: 6465 6420 696e 2074 6865 2072 656c 6576  ded in the relev
-000026f0: 616e 7420 462d 4375 7276 6573 2e0a 0a20  ant F-Curves... 
-00002700: 2020 2020 2020 2049 4e53 4552 544b 4559         INSERTKEY
-00002710: 5f56 4953 5541 4c20 496e 7365 7274 206b  _VISUAL Insert k
-00002720: 6579 6672 616d 6573 2062 6173 6564 206f  eyframes based o
-00002730: 6e20 2776 6973 7561 6c20 7472 616e 7366  n 'visual transf
-00002740: 6f72 6d73 272e 0a0a 2020 2020 2020 2020  orms'...        
-00002750: 494e 5345 5254 4b45 595f 5859 5a5f 544f  INSERTKEY_XYZ_TO
-00002760: 5f52 4742 2054 6869 7320 666c 6167 2069  _RGB This flag i
-00002770: 7320 6e6f 206c 6f6e 6765 7220 696e 2075  s no longer in u
-00002780: 7365 2c20 616e 6420 6973 2068 6572 6520  se, and is here 
-00002790: 736f 2074 6861 7420 636f 6465 2074 6861  so that code tha
-000027a0: 7420 7573 6573 2069 7420 646f 6573 6e27  t uses it doesn'
-000027b0: 7420 6272 6561 6b2e 2054 6865 2058 595a  t break. The XYZ
-000027c0: 3d52 4742 2063 6f6c 6f72 696e 6720 6973  =RGB coloring is
-000027d0: 2064 6574 6572 6d69 6e65 6420 6279 2074   determined by t
-000027e0: 6865 2061 6e69 6d61 7469 6f6e 2070 7265  he animation pre
-000027f0: 6665 7265 6e63 6573 2e0a 0a20 2020 2020  ferences...     
-00002800: 2020 2049 4e53 4552 544b 4559 5f52 4550     INSERTKEY_REP
-00002810: 4c41 4345 204f 6e6c 7920 7265 706c 6163  LACE Only replac
-00002820: 6520 616c 7265 6164 7920 6578 6973 7469  e already existi
-00002830: 6e67 206b 6579 6672 616d 6573 2e0a 0a20  ng keyframes... 
-00002840: 2020 2020 2020 2049 4e53 4552 544b 4559         INSERTKEY
-00002850: 5f41 5641 494c 4142 4c45 204f 6e6c 7920  _AVAILABLE Only 
-00002860: 696e 7365 7274 2069 6e74 6f20 616c 7265  insert into alre
-00002870: 6164 7920 6578 6973 7469 6e67 2046 2d43  ady existing F-C
-00002880: 7572 7665 732e 0a0a 2020 2020 2020 2020  urves...        
-00002890: 494e 5345 5254 4b45 595f 4359 434c 455f  INSERTKEY_CYCLE_
-000028a0: 4157 4152 4520 5461 6b65 2063 7963 6c69  AWARE Take cycli
-000028b0: 6320 6578 7472 6170 6f6c 6174 696f 6e20  c extrapolation 
-000028c0: 696e 746f 2061 6363 6f75 6e74 2028 4379  into account (Cy
-000028d0: 636c 652d 4177 6172 6520 4b65 7969 6e67  cle-Aware Keying
-000028e0: 206f 7074 696f 6e29 2e0a 2020 2020 2020   option)..      
-000028f0: 2020 2020 2020 2020 2020 3a72 6574 7572            :retur
-00002900: 6e3a 2053 7563 6365 7373 206f 6620 6b65  n: Success of ke
-00002910: 7966 7261 6d65 2069 6e73 6572 7469 6f6e  yframe insertion
-00002920: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002930: 2020 3a72 7479 7065 3a20 626f 6f6c 0a20    :rtype: bool. 
-00002940: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00002950: 2020 202e 2e2e 0a0a 2020 2020 6465 6620     .....    def 
-00002960: 6b65 7973 2873 656c 6629 202d 3e20 626f  keys(self) -> bo
-00002970: 6f6c 3a0a 2020 2020 2020 2020 2222 2252  ol:.        """R
-00002980: 6574 7572 6e73 2074 6865 206b 6579 7320  eturns the keys 
-00002990: 6f66 2074 6869 7320 6f62 6a65 6374 7320  of this objects 
-000029a0: 6375 7374 6f6d 2070 726f 7065 7274 6965  custom propertie
-000029b0: 7320 286d 6174 6368 6573 2050 7974 686f  s (matches Pytho
-000029c0: 6e27 730a 2020 2020 2020 2020 6469 6374  n's.        dict
-000029d0: 696f 6e61 7279 2066 756e 6374 696f 6e20  ionary function 
-000029e0: 6f66 2074 6865 2073 616d 6520 6e61 6d65  of the same name
-000029f0: 292e 0a0a 2020 2020 2020 2020 2020 2020  )...            
-00002a00: 2020 2020 3a72 6574 7572 6e3a 2063 7573      :return: cus
-00002a10: 746f 6d20 7072 6f70 6572 7479 206b 6579  tom property key
-00002a20: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00002a30: 2020 2020 2020 202e 2e2e 0a0a 2020 2020         .....    
-00002a40: 6465 6620 7061 7468 5f66 726f 6d5f 6964  def path_from_id
-00002a50: 2873 656c 662c 2070 726f 7065 7274 793a  (self, property:
-00002a60: 2073 7472 203d 2022 2229 202d 3e20 7374   str = "") -> st
-00002a70: 723a 0a20 2020 2020 2020 2022 2222 5265  r:.        """Re
-00002a80: 7475 726e 7320 7468 6520 6461 7461 2070  turns the data p
-00002a90: 6174 6820 6672 6f6d 2074 6865 2049 4420  ath from the ID 
-00002aa0: 746f 2074 6869 7320 6f62 6a65 6374 2028  to this object (
-00002ab0: 7374 7269 6e67 292e 0a0a 2020 2020 2020  string)...      
-00002ac0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00002ad0: 2070 726f 7065 7274 793a 204f 7074 696f   property: Optio
-00002ae0: 6e61 6c20 7072 6f70 6572 7479 206e 616d  nal property nam
-00002af0: 6520 7768 6963 6820 6361 6e20 6265 2075  e which can be u
-00002b00: 7365 6420 6966 2074 6865 2070 6174 6820  sed if the path 
-00002b10: 6973 0a20 2020 2020 2020 2074 6f20 6120  is.        to a 
-00002b20: 7072 6f70 6572 7479 206f 6620 7468 6973  property of this
-00002b30: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
-00002b40: 2020 2020 2020 2020 203a 7479 7065 2070           :type p
-00002b50: 726f 7065 7274 793a 2073 7472 0a20 2020  roperty: str.   
-00002b60: 2020 2020 2020 2020 2020 2020 203a 7265               :re
-00002b70: 7475 726e 3a20 5468 6520 7061 7468 2066  turn: The path f
-00002b80: 726f 6d20 6062 7079 2e74 7970 6573 2e62  rom `bpy.types.b
-00002b90: 7079 5f73 7472 7563 742e 6964 5f64 6174  py_struct.id_dat
-00002ba0: 6160 0a20 2020 2020 2020 2074 6f20 7468  a`.        to th
-00002bb0: 6973 2073 7472 7563 7420 616e 6420 7072  is struct and pr
-00002bc0: 6f70 6572 7479 2028 7768 656e 2067 6976  operty (when giv
-00002bd0: 656e 292e 0a20 2020 2020 2020 2020 2020  en)..           
-00002be0: 2020 2020 203a 7274 7970 653a 2073 7472       :rtype: str
-00002bf0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00002c00: 2020 2020 202e 2e2e 0a0a 2020 2020 6465       .....    de
-00002c10: 6620 7061 7468 5f72 6573 6f6c 7665 2873  f path_resolve(s
-00002c20: 656c 662c 2070 6174 683a 2073 7472 2c20  elf, path: str, 
-00002c30: 636f 6572 6365 3a20 626f 6f6c 203d 2054  coerce: bool = T
-00002c40: 7275 6529 3a0a 2020 2020 2020 2020 2222  rue):.        ""
-00002c50: 2252 6574 7572 6e73 2074 6865 2070 726f  "Returns the pro
-00002c60: 7065 7274 7920 6672 6f6d 2074 6865 2070  perty from the p
-00002c70: 6174 682c 2072 6169 7365 2061 6e20 6578  ath, raise an ex
-00002c80: 6365 7074 696f 6e20 7768 656e 206e 6f74  ception when not
-00002c90: 2066 6f75 6e64 2e0a 0a20 2020 2020 2020   found...       
-00002ca0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-00002cb0: 7061 7468 3a20 7061 7468 2077 6869 6368  path: path which
-00002cc0: 2074 6869 7320 7072 6f70 6572 7479 2072   this property r
-00002cd0: 6573 6f6c 7665 732e 0a20 2020 2020 2020  esolves..       
-00002ce0: 2020 2020 2020 2020 203a 7479 7065 2070           :type p
-00002cf0: 6174 683a 2073 7472 0a20 2020 2020 2020  ath: str.       
-00002d00: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
-00002d10: 636f 6572 6365 3a20 6f70 7469 6f6e 616c  coerce: optional
-00002d20: 2061 7267 756d 656e 742c 2077 6865 6e20   argument, when 
-00002d30: 5472 7565 2c20 7468 6520 7072 6f70 6572  True, the proper
-00002d40: 7479 2077 696c 6c20 6265 2063 6f6e 7665  ty will be conve
-00002d50: 7274 6564 0a20 2020 2020 2020 2069 6e74  rted.        int
-00002d60: 6f20 6974 7320 5079 7468 6f6e 2072 6570  o its Python rep
-00002d70: 7265 7365 6e74 6174 696f 6e2e 0a20 2020  resentation..   
-00002d80: 2020 2020 2020 2020 2020 2020 203a 7479               :ty
-00002d90: 7065 2063 6f65 7263 653a 2062 6f6f 6c0a  pe coerce: bool.
-00002da0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00002db0: 2020 2020 2e2e 2e0a 0a20 2020 2064 6566      .....    def
-00002dc0: 2070 6f70 2873 656c 662c 206b 6579 3a20   pop(self, key: 
-00002dd0: 7374 722c 2064 6566 6175 6c74 3d4e 6f6e  str, default=Non
-00002de0: 6529 3a0a 2020 2020 2020 2020 2222 2252  e):.        """R
-00002df0: 656d 6f76 6520 616e 6420 7265 7475 726e  emove and return
-00002e00: 2074 6865 2076 616c 7565 206f 6620 7468   the value of th
-00002e10: 6520 6375 7374 6f6d 2070 726f 7065 7274  e custom propert
-00002e20: 7920 6173 7369 676e 6564 2074 6f20 6b65  y assigned to ke
-00002e30: 7920 6f72 2064 6566 6175 6c74 0a20 2020  y or default.   
-00002e40: 2020 2020 2077 6865 6e20 6e6f 7420 666f       when not fo
-00002e50: 756e 6420 286d 6174 6368 6573 2050 7974  und (matches Pyt
-00002e60: 686f 6e27 7320 6469 6374 696f 6e61 7279  hon's dictionary
-00002e70: 2066 756e 6374 696f 6e20 6f66 2074 6865   function of the
-00002e80: 2073 616d 6520 6e61 6d65 292e 0a0a 2020   same name)...  
-00002e90: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
-00002ea0: 6172 616d 206b 6579 3a20 5468 6520 6b65  aram key: The ke
-00002eb0: 7920 6173 736f 6369 6174 6564 2077 6974  y associated wit
-00002ec0: 6820 7468 6520 6375 7374 6f6d 2070 726f  h the custom pro
-00002ed0: 7065 7274 792e 0a20 2020 2020 2020 2020  perty..         
-00002ee0: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
-00002ef0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-00002f00: 2020 2020 2020 3a70 6172 616d 2064 6566        :param def
-00002f10: 6175 6c74 3a20 4f70 7469 6f6e 616c 2061  ault: Optional a
-00002f20: 7267 756d 656e 7420 666f 7220 7468 6520  rgument for the 
-00002f30: 7661 6c75 6520 746f 2072 6574 7572 6e20  value to return 
-00002f40: 6966 0a20 2020 2020 2020 206b 6579 2069  if.        key i
-00002f50: 7320 6e6f 7420 666f 756e 642e 0a20 2020  s not found..   
-00002f60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00002f70: 202e 2e2e 0a0a 2020 2020 6465 6620 7072   .....    def pr
-00002f80: 6f70 6572 7479 5f6f 7665 7272 6964 6162  operty_overridab
-00002f90: 6c65 5f6c 6962 7261 7279 5f73 6574 2873  le_library_set(s
-00002fa0: 656c 662c 2070 726f 7065 7274 792c 206f  elf, property, o
-00002fb0: 7665 7272 6964 6162 6c65 293a 0a20 2020  verridable):.   
-00002fc0: 2020 2020 2022 2222 4465 6669 6e65 2061       """Define a
-00002fd0: 2070 726f 7065 7274 7920 6173 206f 7665   property as ove
-00002fe0: 7272 6964 6162 6c65 206f 7220 6e6f 7420  rridable or not 
-00002ff0: 286f 6e6c 7920 666f 7220 6375 7374 6f6d  (only for custom
-00003000: 2070 726f 7065 7274 6965 7321 292e 0a0a   properties!)...
-00003010: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-00003020: 726f 7065 7274 793a 0a20 2020 2020 2020  roperty:.       
-00003030: 203a 7061 7261 6d20 6f76 6572 7269 6461   :param overrida
-00003040: 626c 653a 0a20 2020 2020 2020 203a 7265  ble:.        :re
-00003050: 7475 726e 3a20 5472 7565 2077 6865 6e20  turn: True when 
-00003060: 7468 6520 6f76 6572 7269 6461 626c 6520  the overridable 
-00003070: 7374 6174 7573 206f 6620 7468 6520 7072  status of the pr
-00003080: 6f70 6572 7479 2077 6173 2073 7563 6365  operty was succe
-00003090: 7373 6675 6c6c 7920 7365 742e 0a20 2020  ssfully set..   
-000030a0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-000030b0: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
-000030c0: 2020 2020 2020 2e2e 2e0a 0a20 2020 2064        .....    d
-000030d0: 6566 2070 726f 7065 7274 795f 756e 7365  ef property_unse
-000030e0: 7428 7365 6c66 2c20 7072 6f70 6572 7479  t(self, property
-000030f0: 293a 0a20 2020 2020 2020 2022 2222 556e  ):.        """Un
-00003100: 7365 7420 6120 7072 6f70 6572 7479 2c20  set a property, 
-00003110: 7769 6c6c 2075 7365 2064 6566 6175 6c74  will use default
-00003120: 2076 616c 7565 2061 6674 6572 7761 7264   value afterward
-00003130: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00003140: 6d20 7072 6f70 6572 7479 3a0a 2020 2020  m property:.    
-00003150: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00003160: 2e2e 2e0a 0a20 2020 2064 6566 2074 7970  .....    def typ
-00003170: 655f 7265 6361 7374 2873 656c 6629 3a0a  e_recast(self):.
-00003180: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00003190: 6e20 6120 6e65 7720 696e 7374 616e 6365  n a new instance
-000031a0: 2c20 7468 6973 2069 7320 6e65 6564 6564  , this is needed
-000031b0: 2062 6563 6175 7365 2074 7970 6573 0a20   because types. 
-000031c0: 2020 2020 2020 2073 7563 6820 6173 2074         such as t
-000031d0: 6578 7475 7265 7320 6361 6e20 6265 2063  extures can be c
-000031e0: 6861 6e67 6564 2061 7420 7275 6e74 696d  hanged at runtim
-000031f0: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
-00003200: 2020 2020 3a72 6574 7572 6e3a 2061 206e      :return: a n
-00003210: 6577 2069 6e73 7461 6e63 6520 6f66 2074  ew instance of t
-00003220: 6869 7320 6f62 6a65 6374 2077 6974 6820  his object with 
-00003230: 7468 6520 7479 7065 2069 6e69 7469 616c  the type initial
-00003240: 697a 6564 2061 6761 696e 2e0a 2020 2020  ized again..    
-00003250: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00003260: 2e2e 2e0a 0a20 2020 2064 6566 2076 616c  .....    def val
-00003270: 7565 7328 7365 6c66 293a 0a20 2020 2020  ues(self):.     
-00003280: 2020 2022 2222 5265 7475 726e 7320 7468     """Returns th
-00003290: 6520 7661 6c75 6573 206f 6620 7468 6973  e values of this
-000032a0: 206f 626a 6563 7473 2063 7573 746f 6d20   objects custom 
-000032b0: 7072 6f70 6572 7469 6573 2028 6d61 7463  properties (matc
-000032c0: 6865 7320 5079 7468 6f6e 2773 0a20 2020  hes Python's.   
-000032d0: 2020 2020 2064 6963 7469 6f6e 6172 7920       dictionary 
-000032e0: 6675 6e63 7469 6f6e 206f 6620 7468 6520  function of the 
-000032f0: 7361 6d65 206e 616d 6529 2e0a 0a20 2020  same name)...   
-00003300: 2020 2020 2020 2020 2020 2020 203a 7265               :re
-00003310: 7475 726e 3a20 6375 7374 6f6d 2070 726f  turn: custom pro
-00003320: 7065 7274 7920 7661 6c75 6573 2e0a 2020  perty values..  
-00003330: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00003340: 2020 2e2e 2e0a 0a20 2020 2064 6566 205f    .....    def _
-00003350: 5f67 6574 6974 656d 5f5f 2873 656c 662c  _getitem__(self,
-00003360: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
-00003370: 6f6e 5b69 6e74 2c20 7374 725d 2920 2d3e  on[int, str]) ->
-00003380: 2074 7970 696e 672e 556e 696f 6e5b 696e   typing.Union[in
-00003390: 742c 2073 7472 5d3a 0a20 2020 2020 2020  t, str]:.       
-000033a0: 2022 2222 0a0a 2020 2020 2020 2020 3a70   """..        :p
-000033b0: 6172 616d 206b 6579 3a0a 2020 2020 2020  aram key:.      
-000033c0: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
-000033d0: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
-000033e0: 7472 5d0a 2020 2020 2020 2020 3a72 6574  tr].        :ret
-000033f0: 7572 6e3a 0a20 2020 2020 2020 203a 7274  urn:.        :rt
-00003400: 7970 653a 2074 7970 696e 672e 416e 790a  ype: typing.Any.
-00003410: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003420: 2020 2020 2e2e 2e0a 0a20 2020 2064 6566      .....    def
-00003430: 205f 5f73 6574 6974 656d 5f5f 2873 656c   __setitem__(sel
-00003440: 662c 206b 6579 3a20 7479 7069 6e67 2e55  f, key: typing.U
-00003450: 6e69 6f6e 5b69 6e74 2c20 7374 725d 2c20  nion[int, str], 
-00003460: 7661 6c75 653a 2074 7970 696e 672e 416e  value: typing.An
-00003470: 7929 3a0a 2020 2020 2020 2020 2222 220a  y):.        """.
-00003480: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00003490: 6b65 793a 0a20 2020 2020 2020 203a 7479  key:.        :ty
-000034a0: 7065 206b 6579 3a20 7479 7069 6e67 2e55  pe key: typing.U
-000034b0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 0a20  nion[int, str]. 
-000034c0: 2020 2020 2020 203a 7061 7261 6d20 7661         :param va
-000034d0: 6c75 653a 0a20 2020 2020 2020 203a 7479  lue:.        :ty
-000034e0: 7065 2076 616c 7565 3a20 7479 7069 6e67  pe value: typing
-000034f0: 2e41 6e79 0a20 2020 2020 2020 2022 2222  .Any.        """
-00003500: 0a20 2020 2020 2020 202e 2e2e 0a0a 2020  .        .....  
-00003510: 2020 6465 6620 5f5f 6465 6c69 7465 6d5f    def __delitem_
-00003520: 5f28 7365 6c66 2c20 6b65 793a 2074 7970  _(self, key: typ
-00003530: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
-00003540: 7472 5d29 202d 3e20 7479 7069 6e67 2e55  tr]) -> typing.U
-00003550: 6e69 6f6e 5b69 6e74 2c20 7374 725d 3a0a  nion[int, str]:.
-00003560: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00003570: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
-00003580: 0a20 2020 2020 2020 203a 7479 7065 206b  .        :type k
-00003590: 6579 3a20 7479 7069 6e67 2e55 6e69 6f6e  ey: typing.Union
-000035a0: 5b69 6e74 2c20 7374 725d 0a20 2020 2020  [int, str].     
-000035b0: 2020 203a 7265 7475 726e 3a0a 2020 2020     :return:.    
-000035c0: 2020 2020 3a72 7479 7065 3a20 7479 7069      :rtype: typi
-000035d0: 6e67 2e41 6e79 0a20 2020 2020 2020 2022  ng.Any.        "
-000035e0: 2222 0a20 2020 2020 2020 202e 2e2e 0a0a  "".        .....
-000035f0: 636c 6173 7320 6270 795f 7072 6f70 5f63  class bpy_prop_c
-00003600: 6f6c 6c65 6374 696f 6e28 7479 7069 6e67  ollection(typing
-00003610: 2e47 656e 6572 6963 5b47 656e 6572 6963  .Generic[Generic
-00003620: 5479 7065 5d29 3a0a 2020 2020 2222 2262  Type]):.    """b
-00003630: 7569 6c74 2d69 6e20 636c 6173 7320 7573  uilt-in class us
-00003640: 6564 2066 6f72 2061 6c6c 2063 6f6c 6c65  ed for all colle
-00003650: 6374 696f 6e73 2e22 2222 0a0a 2020 2020  ctions."""..    
-00003660: 6465 6620 6669 6e64 2873 656c 662c 206b  def find(self, k
-00003670: 6579 3a20 7374 7229 202d 3e20 7374 723a  ey: str) -> str:
-00003680: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00003690: 726e 7320 7468 6520 696e 6465 7820 6f66  rns the index of
-000036a0: 2061 206b 6579 2069 6e20 6120 636f 6c6c   a key in a coll
-000036b0: 6563 7469 6f6e 206f 7220 2d31 2077 6865  ection or -1 whe
-000036c0: 6e20 6e6f 7420 666f 756e 640a 2020 2020  n not found.    
-000036d0: 2020 2020 286d 6174 6368 6573 2050 7974      (matches Pyt
-000036e0: 686f 6e27 7320 7374 7269 6e67 2066 696e  hon's string fin
-000036f0: 6420 6675 6e63 7469 6f6e 206f 6620 7468  d function of th
-00003700: 6520 7361 6d65 206e 616d 6529 2e0a 0a20  e same name)... 
-00003710: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-00003720: 7061 7261 6d20 6b65 793a 2054 6865 2069  param key: The i
-00003730: 6465 6e74 6966 6965 7220 666f 7220 7468  dentifier for th
-00003740: 6520 636f 6c6c 6563 7469 6f6e 206d 656d  e collection mem
-00003750: 6265 722e 0a20 2020 2020 2020 2020 2020  ber..           
-00003760: 2020 2020 203a 7479 7065 206b 6579 3a20       :type key: 
-00003770: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-00003780: 2020 2020 3a72 6574 7572 6e3a 2069 6e64      :return: ind
-00003790: 6578 206f 6620 7468 6520 6b65 792e 0a20  ex of the key.. 
-000037a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000037b0: 2020 202e 2e2e 0a0a 2020 2020 6465 6620     .....    def 
-000037c0: 666f 7265 6163 685f 6765 7428 7365 6c66  foreach_get(self
-000037d0: 2c20 6174 7472 2c20 7365 7129 3a0a 2020  , attr, seq):.  
-000037e0: 2020 2020 2020 2222 2254 6869 7320 6973        """This is
-000037f0: 2061 2066 756e 6374 696f 6e20 746f 2067   a function to g
-00003800: 6976 6520 6661 7374 2061 6363 6573 7320  ive fast access 
-00003810: 746f 2061 7474 7269 6275 7465 7320 7769  to attributes wi
-00003820: 7468 696e 2061 2063 6f6c 6c65 6374 696f  thin a collectio
-00003830: 6e2e 4f6e 6c79 2077 6f72 6b73 2066 6f72  n.Only works for
-00003840: 2027 6261 7369 6320 7479 7065 2720 7072   'basic type' pr
-00003850: 6f70 6572 7469 6573 2028 626f 6f6c 2c20  operties (bool, 
-00003860: 696e 7420 616e 6420 666c 6f61 7429 210a  int and float)!.
-00003870: 2020 2020 2020 2020 4d75 6c74 692d 6469          Multi-di
-00003880: 6d65 6e73 696f 6e61 6c20 6172 7261 7973  mensional arrays
-00003890: 2028 6c69 6b65 2061 7272 6179 206f 6620   (like array of 
-000038a0: 7665 6374 6f72 7329 2077 696c 6c20 6265  vectors) will be
-000038b0: 2066 6c61 7474 656e 6564 2069 6e74 6f20   flattened into 
-000038c0: 7365 712e 0a0a 2020 2020 2020 2020 2020  seq...          
-000038d0: 2020 2020 2020 3a70 6172 616d 2061 7474        :param att
-000038e0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-000038f0: 2020 203a 7061 7261 6d20 7365 713a 0a20     :param seq:. 
-00003900: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00003910: 2020 202e 2e2e 0a0a 2020 2020 6465 6620     .....    def 
-00003920: 666f 7265 6163 685f 7365 7428 7365 6c66  foreach_set(self
-00003930: 2c20 6174 7472 2c20 7365 7129 3a0a 2020  , attr, seq):.  
-00003940: 2020 2020 2020 2222 2254 6869 7320 6973        """This is
-00003950: 2061 2066 756e 6374 696f 6e20 746f 2067   a function to g
-00003960: 6976 6520 6661 7374 2061 6363 6573 7320  ive fast access 
-00003970: 746f 2061 7474 7269 6275 7465 7320 7769  to attributes wi
-00003980: 7468 696e 2061 2063 6f6c 6c65 6374 696f  thin a collectio
-00003990: 6e2e 4f6e 6c79 2077 6f72 6b73 2066 6f72  n.Only works for
-000039a0: 2027 6261 7369 6320 7479 7065 2720 7072   'basic type' pr
-000039b0: 6f70 6572 7469 6573 2028 626f 6f6c 2c20  operties (bool, 
-000039c0: 696e 7420 616e 6420 666c 6f61 7429 210a  int and float)!.
-000039d0: 2020 2020 2020 2020 7365 7120 6d75 7374          seq must
-000039e0: 2062 6520 756e 692d 6469 6d65 6e73 696f   be uni-dimensio
-000039f0: 6e61 6c2c 206d 756c 7469 2d64 696d 656e  nal, multi-dimen
-00003a00: 7369 6f6e 616c 2061 7272 6179 7320 286c  sional arrays (l
-00003a10: 696b 6520 6172 7261 7920 6f66 2076 6563  ike array of vec
-00003a20: 746f 7273 2920 7769 6c6c 2062 6520 7265  tors) will be re
-00003a30: 2d63 7265 6174 6564 2066 726f 6d20 6974  -created from it
-00003a40: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
-00003a50: 2020 203a 7061 7261 6d20 6174 7472 3a0a     :param attr:.
-00003a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a70: 3a70 6172 616d 2073 6571 3a0a 2020 2020  :param seq:.    
-00003a80: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00003a90: 2e2e 2e0a 0a20 2020 2064 6566 2067 6574  .....    def get
-00003aa0: 2873 656c 662c 206b 6579 3a20 7374 722c  (self, key: str,
-00003ab0: 2064 6566 6175 6c74 3d4e 6f6e 6529 3a0a   default=None):.
-00003ac0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00003ad0: 6e73 2074 6865 2076 616c 7565 206f 6620  ns the value of 
-00003ae0: 7468 6520 6974 656d 2061 7373 6967 6e65  the item assigne
-00003af0: 6420 746f 206b 6579 206f 7220 6465 6661  d to key or defa
-00003b00: 756c 7420 7768 656e 206e 6f74 2066 6f75  ult when not fou
-00003b10: 6e64 0a20 2020 2020 2020 2028 6d61 7463  nd.        (matc
-00003b20: 6865 7320 5079 7468 6f6e 2773 2064 6963  hes Python's dic
-00003b30: 7469 6f6e 6172 7920 6675 6e63 7469 6f6e  tionary function
-00003b40: 206f 6620 7468 6520 7361 6d65 206e 616d   of the same nam
-00003b50: 6529 2e0a 0a20 2020 2020 2020 2020 2020  e)...           
-00003b60: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
-00003b70: 2054 6865 2069 6465 6e74 6966 6965 7220   The identifier 
-00003b80: 666f 7220 7468 6520 636f 6c6c 6563 7469  for the collecti
-00003b90: 6f6e 206d 656d 6265 722e 0a20 2020 2020  on member..     
-00003ba0: 2020 2020 2020 2020 2020 203a 7479 7065             :type
-00003bb0: 206b 6579 3a20 7374 720a 2020 2020 2020   key: str.      
-00003bc0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
-00003bd0: 2064 6566 6175 6c74 3a20 4f70 7469 6f6e   default: Option
-00003be0: 616c 2061 7267 756d 656e 7420 666f 7220  al argument for 
-00003bf0: 7468 6520 7661 6c75 6520 746f 2072 6574  the value to ret
-00003c00: 7572 6e20 6966 0a20 2020 2020 2020 206b  urn if.        k
-00003c10: 6579 2069 7320 6e6f 7420 666f 756e 642e  ey is not found.
-00003c20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00003c30: 2020 2020 202e 2e2e 0a0a 2020 2020 6465       .....    de
-00003c40: 6620 6974 656d 7328 7365 6c66 293a 0a20  f items(self):. 
-00003c50: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-00003c60: 2074 6865 2069 6465 6e74 6966 6965 7273   the identifiers
-00003c70: 206f 6620 636f 6c6c 6563 7469 6f6e 206d   of collection m
-00003c80: 656d 6265 7273 0a20 2020 2020 2020 2028  embers.        (
-00003c90: 6d61 7463 6869 6e67 2050 7974 686f 6e27  matching Python'
-00003ca0: 7320 6469 6374 2e69 7465 6d73 2829 2066  s dict.items() f
-00003cb0: 756e 6374 696f 6e61 6c69 7479 292e 0a0a  unctionality)...
-00003cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cd0: 3a72 6574 7572 6e3a 2028 6b65 792c 2076  :return: (key, v
-00003ce0: 616c 7565 2920 7061 6972 7320 666f 7220  alue) pairs for 
-00003cf0: 6561 6368 206d 656d 6265 7220 6f66 2074  each member of t
-00003d00: 6869 7320 636f 6c6c 6563 7469 6f6e 2e0a  his collection..
-00003d10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003d20: 2020 2020 2e2e 2e0a 0a20 2020 2064 6566      .....    def
-00003d30: 206b 6579 7328 7365 6c66 293a 0a20 2020   keys(self):.   
-00003d40: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
-00003d50: 6865 2069 6465 6e74 6966 6965 7273 206f  he identifiers o
-00003d60: 6620 636f 6c6c 6563 7469 6f6e 206d 656d  f collection mem
-00003d70: 6265 7273 0a20 2020 2020 2020 2028 6d61  bers.        (ma
-00003d80: 7463 6869 6e67 2050 7974 686f 6e27 7320  tching Python's 
-00003d90: 6469 6374 2e6b 6579 7328 2920 6675 6e63  dict.keys() func
-00003da0: 7469 6f6e 616c 6974 7929 2e0a 0a20 2020  tionality)...   
-00003db0: 2020 2020 2020 2020 2020 2020 203a 7265               :re
-00003dc0: 7475 726e 3a20 7468 6520 6964 656e 7469  turn: the identi
-00003dd0: 6669 6572 7320 666f 7220 6561 6368 206d  fiers for each m
-00003de0: 656d 6265 7220 6f66 2074 6869 7320 636f  ember of this co
-00003df0: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
-00003e00: 2020 2020 2020 2020 2020 3a72 7479 7065            :rtype
-00003e10: 3a20 7479 7069 6e67 2e4c 6973 745b 7374  : typing.List[st
-00003e20: 725d 0a20 2020 2020 2020 2022 2222 0a20  r].        """. 
-00003e30: 2020 2020 2020 202e 2e2e 0a0a 2020 2020         .....    
-00003e40: 6465 6620 7661 6c75 6573 2873 656c 6629  def values(self)
-00003e50: 202d 3e20 7479 7069 6e67 2e4c 6973 745b   -> typing.List[
-00003e60: 7374 725d 3a0a 2020 2020 2020 2020 2222  str]:.        ""
-00003e70: 2252 6574 7572 6e20 7468 6520 7661 6c75  "Return the valu
-00003e80: 6573 206f 6620 636f 6c6c 6563 7469 6f6e  es of collection
-00003e90: 0a20 2020 2020 2020 2028 6d61 7463 6869  .        (matchi
-00003ea0: 6e67 2050 7974 686f 6e27 7320 6469 6374  ng Python's dict
-00003eb0: 2e76 616c 7565 7328 2920 6675 6e63 7469  .values() functi
-00003ec0: 6f6e 616c 6974 7929 2e0a 0a20 2020 2020  onality)...     
-00003ed0: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
-00003ee0: 726e 3a20 7468 6520 6d65 6d62 6572 7320  rn: the members 
-00003ef0: 6f66 2074 6869 7320 636f 6c6c 6563 7469  of this collecti
-00003f00: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-00003f10: 2020 2020 3a72 7479 7065 3a20 6c69 7374      :rtype: list
-00003f20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00003f30: 2020 2020 202e 2e2e 0a0a 2020 2020 6465       .....    de
-00003f40: 6620 5f5f 6765 7469 7465 6d5f 5f28 7365  f __getitem__(se
-00003f50: 6c66 2c20 6b65 793a 2074 7970 696e 672e  lf, key: typing.
-00003f60: 556e 696f 6e5b 696e 742c 2073 7472 5d29  Union[int, str])
-00003f70: 202d 3e20 7479 7069 6e67 2e55 6e69 6f6e   -> typing.Union
-00003f80: 5b69 6e74 2c20 7374 725d 3a0a 2020 2020  [int, str]:.    
-00003f90: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00003fa0: 203a 7061 7261 6d20 6b65 793a 0a20 2020   :param key:.   
-00003fb0: 2020 2020 203a 7479 7065 206b 6579 3a20       :type key: 
-00003fc0: 7479 7069 6e67 2e55 6e69 6f6e 5b69 6e74  typing.Union[int
-00003fd0: 2c20 7374 725d 0a20 2020 2020 2020 203a  , str].        :
-00003fe0: 7265 7475 726e 3a0a 2020 2020 2020 2020  return:.        
-00003ff0: 3a72 7479 7065 3a20 4765 6e65 7269 6354  :rtype: GenericT
-00004000: 7970 650a 2020 2020 2020 2020 2222 220a  ype.        """.
-00004010: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
-00004020: 2064 6566 205f 5f73 6574 6974 656d 5f5f   def __setitem__
-00004030: 2873 656c 662c 206b 6579 3a20 7479 7069  (self, key: typi
-00004040: 6e67 2e55 6e69 6f6e 5b69 6e74 2c20 7374  ng.Union[int, st
-00004050: 725d 2c20 7661 6c75 653a 2047 656e 6572  r], value: Gener
-00004060: 6963 5479 7065 293a 0a20 2020 2020 2020  icType):.       
-00004070: 2022 2222 0a0a 2020 2020 2020 2020 3a70   """..        :p
-00004080: 6172 616d 206b 6579 3a0a 2020 2020 2020  aram key:.      
-00004090: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
-000040a0: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
-000040b0: 7472 5d0a 2020 2020 2020 2020 3a70 6172  tr].        :par
-000040c0: 616d 2076 616c 7565 3a0a 2020 2020 2020  am value:.      
-000040d0: 2020 3a74 7970 6520 7661 6c75 653a 2047    :type value: G
-000040e0: 656e 6572 6963 5479 7065 0a20 2020 2020  enericType.     
-000040f0: 2020 2022 2222 0a20 2020 2020 2020 202e     """.        .
-00004100: 2e2e 0a0a 2020 2020 6465 6620 5f5f 6465  ....    def __de
-00004110: 6c69 7465 6d5f 5f28 7365 6c66 2c20 6b65  litem__(self, ke
-00004120: 793a 2074 7970 696e 672e 556e 696f 6e5b  y: typing.Union[
-00004130: 696e 742c 2073 7472 5d29 202d 3e20 7479  int, str]) -> ty
-00004140: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-00004150: 7374 725d 3a0a 2020 2020 2020 2020 2222  str]:.        ""
-00004160: 220a 0a20 2020 2020 2020 203a 7061 7261  "..        :para
-00004170: 6d20 6b65 793a 0a20 2020 2020 2020 203a  m key:.        :
-00004180: 7479 7065 206b 6579 3a20 7479 7069 6e67  type key: typing
-00004190: 2e55 6e69 6f6e 5b69 6e74 2c20 7374 725d  .Union[int, str]
-000041a0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000041b0: 3a0a 2020 2020 2020 2020 3a72 7479 7065  :.        :rtype
-000041c0: 3a20 4765 6e65 7269 6354 7970 650a 2020  : GenericType.  
-000041d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000041e0: 2020 2e2e 2e0a 0a20 2020 2064 6566 205f    .....    def _
-000041f0: 5f69 7465 725f 5f28 7365 6c66 2920 2d3e  _iter__(self) ->
-00004200: 2047 656e 6572 6963 5479 7065 3a0a 2020   GenericType:.  
-00004210: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00004220: 2020 203a 7265 7475 726e 3a0a 2020 2020     :return:.    
-00004230: 2020 2020 3a72 7479 7065 3a20 7479 7069      :rtype: typi
-00004240: 6e67 2e49 7465 7261 746f 725b 4765 6e65  ng.Iterator[Gene
-00004250: 7269 6354 7970 655d 0a20 2020 2020 2020  ricType].       
-00004260: 2022 2222 0a20 2020 2020 2020 202e 2e2e   """.        ...
-00004270: 0a0a 2020 2020 6465 6620 5f5f 6e65 7874  ..    def __next
-00004280: 5f5f 2873 656c 6629 202d 3e20 7479 7069  __(self) -> typi
-00004290: 6e67 2e49 7465 7261 746f 725b 4765 6e65  ng.Iterator[Gene
-000042a0: 7269 6354 7970 655d 3a0a 2020 2020 2020  ricType]:.      
-000042b0: 2020 2222 220a 0a20 2020 2020 2020 203a    """..        :
-000042c0: 7265 7475 726e 3a0a 2020 2020 2020 2020  return:.        
-000042d0: 3a72 7479 7065 3a20 4765 6e65 7269 6354  :rtype: GenericT
-000042e0: 7970 650a 2020 2020 2020 2020 2222 220a  ype.        """.
-000042f0: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
-00004300: 2064 6566 205f 5f6c 656e 5f5f 2873 656c   def __len__(sel
-00004310: 6629 202d 3e20 4765 6e65 7269 6354 7970  f) -> GenericTyp
-00004320: 653a 0a20 2020 2020 2020 2022 2222 0a0a  e:.        """..
-00004330: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00004340: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00004350: 2069 6e74 0a20 2020 2020 2020 2022 2222   int.        """
+000010d0: 2e0a 0a63 6c61 7373 2062 7079 5f70 726f  ...class bpy_pro
+000010e0: 705f 636f 6c6c 6563 7469 6f6e 2874 7970  p_collection(typ
+000010f0: 696e 672e 4765 6e65 7269 635b 4765 6e65  ing.Generic[Gene
+00001100: 7269 6354 7970 655d 293a 0a20 2020 2022  ricType]):.    "
+00001110: 2222 6275 696c 742d 696e 2063 6c61 7373  ""built-in class
+00001120: 2075 7365 6420 666f 7220 616c 6c20 636f   used for all co
+00001130: 6c6c 6563 7469 6f6e 732e 2222 220a 0a20  llections.""".. 
+00001140: 2020 2064 6566 2066 696e 6428 7365 6c66     def find(self
+00001150: 2c20 6b65 793a 2073 7472 2920 2d3e 2073  , key: str) -> s
+00001160: 7472 3a0a 2020 2020 2020 2020 2222 2252  tr:.        """R
+00001170: 6574 7572 6e73 2074 6865 2069 6e64 6578  eturns the index
+00001180: 206f 6620 6120 6b65 7920 696e 2061 2063   of a key in a c
+00001190: 6f6c 6c65 6374 696f 6e20 6f72 202d 3120  ollection or -1 
+000011a0: 7768 656e 206e 6f74 2066 6f75 6e64 0a20  when not found. 
+000011b0: 2020 2020 2020 2028 6d61 7463 6865 7320         (matches 
+000011c0: 5079 7468 6f6e 2773 2073 7472 696e 6720  Python's string 
+000011d0: 6669 6e64 2066 756e 6374 696f 6e20 6f66  find function of
+000011e0: 2074 6865 2073 616d 6520 6e61 6d65 292e   the same name).
+000011f0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001200: 2020 3a70 6172 616d 206b 6579 3a20 5468    :param key: Th
+00001210: 6520 6964 656e 7469 6669 6572 2066 6f72  e identifier for
+00001220: 2074 6865 2063 6f6c 6c65 6374 696f 6e20   the collection 
+00001230: 6d65 6d62 6572 2e0a 2020 2020 2020 2020  member..        
+00001240: 2020 2020 2020 2020 3a74 7970 6520 6b65          :type ke
+00001250: 793a 2073 7472 0a20 2020 2020 2020 2020  y: str.         
+00001260: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00001270: 696e 6465 7820 6f66 2074 6865 206b 6579  index of the key
+00001280: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00001290: 2020 2020 2020 2e2e 2e0a 0a20 2020 2064        .....    d
+000012a0: 6566 2066 6f72 6561 6368 5f67 6574 2873  ef foreach_get(s
+000012b0: 656c 662c 2061 7474 722c 2073 6571 293a  elf, attr, seq):
+000012c0: 0a20 2020 2020 2020 2022 2222 5468 6973  .        """This
+000012d0: 2069 7320 6120 6675 6e63 7469 6f6e 2074   is a function t
+000012e0: 6f20 6769 7665 2066 6173 7420 6163 6365  o give fast acce
+000012f0: 7373 2074 6f20 6174 7472 6962 7574 6573  ss to attributes
+00001300: 2077 6974 6869 6e20 6120 636f 6c6c 6563   within a collec
+00001310: 7469 6f6e 2e4f 6e6c 7920 776f 726b 7320  tion.Only works 
+00001320: 666f 7220 2762 6173 6963 2074 7970 6527  for 'basic type'
+00001330: 2070 726f 7065 7274 6965 7320 2862 6f6f   properties (boo
+00001340: 6c2c 2069 6e74 2061 6e64 2066 6c6f 6174  l, int and float
+00001350: 2921 0a20 2020 2020 2020 204d 756c 7469  )!.        Multi
+00001360: 2d64 696d 656e 7369 6f6e 616c 2061 7272  -dimensional arr
+00001370: 6179 7320 286c 696b 6520 6172 7261 7920  ays (like array 
+00001380: 6f66 2076 6563 746f 7273 2920 7769 6c6c  of vectors) will
+00001390: 2062 6520 666c 6174 7465 6e65 6420 696e   be flattened in
+000013a0: 746f 2073 6571 2e0a 0a20 2020 2020 2020  to seq...       
+000013b0: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+000013c0: 6174 7472 3a0a 2020 2020 2020 2020 2020  attr:.          
+000013d0: 2020 2020 2020 3a70 6172 616d 2073 6571        :param seq
+000013e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000013f0: 2020 2020 2020 2e2e 2e0a 0a20 2020 2064        .....    d
+00001400: 6566 2066 6f72 6561 6368 5f73 6574 2873  ef foreach_set(s
+00001410: 656c 662c 2061 7474 722c 2073 6571 293a  elf, attr, seq):
+00001420: 0a20 2020 2020 2020 2022 2222 5468 6973  .        """This
+00001430: 2069 7320 6120 6675 6e63 7469 6f6e 2074   is a function t
+00001440: 6f20 6769 7665 2066 6173 7420 6163 6365  o give fast acce
+00001450: 7373 2074 6f20 6174 7472 6962 7574 6573  ss to attributes
+00001460: 2077 6974 6869 6e20 6120 636f 6c6c 6563   within a collec
+00001470: 7469 6f6e 2e4f 6e6c 7920 776f 726b 7320  tion.Only works 
+00001480: 666f 7220 2762 6173 6963 2074 7970 6527  for 'basic type'
+00001490: 2070 726f 7065 7274 6965 7320 2862 6f6f   properties (boo
+000014a0: 6c2c 2069 6e74 2061 6e64 2066 6c6f 6174  l, int and float
+000014b0: 2921 0a20 2020 2020 2020 2073 6571 206d  )!.        seq m
+000014c0: 7573 7420 6265 2075 6e69 2d64 696d 656e  ust be uni-dimen
+000014d0: 7369 6f6e 616c 2c20 6d75 6c74 692d 6469  sional, multi-di
+000014e0: 6d65 6e73 696f 6e61 6c20 6172 7261 7973  mensional arrays
+000014f0: 2028 6c69 6b65 2061 7272 6179 206f 6620   (like array of 
+00001500: 7665 6374 6f72 7329 2077 696c 6c20 6265  vectors) will be
+00001510: 2072 652d 6372 6561 7465 6420 6672 6f6d   re-created from
+00001520: 2069 742e 0a0a 2020 2020 2020 2020 2020   it...          
+00001530: 2020 2020 2020 3a70 6172 616d 2061 7474        :param att
+00001540: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+00001550: 2020 203a 7061 7261 6d20 7365 713a 0a20     :param seq:. 
+00001560: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00001570: 2020 202e 2e2e 0a0a 2020 2020 6465 6620     .....    def 
+00001580: 6765 7428 7365 6c66 2c20 6b65 793a 2073  get(self, key: s
+00001590: 7472 2c20 6465 6661 756c 743d 4e6f 6e65  tr, default=None
+000015a0: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+000015b0: 7475 726e 7320 7468 6520 7661 6c75 6520  turns the value 
+000015c0: 6f66 2074 6865 2069 7465 6d20 6173 7369  of the item assi
+000015d0: 676e 6564 2074 6f20 6b65 7920 6f72 2064  gned to key or d
+000015e0: 6566 6175 6c74 2077 6865 6e20 6e6f 7420  efault when not 
+000015f0: 666f 756e 640a 2020 2020 2020 2020 286d  found.        (m
+00001600: 6174 6368 6573 2050 7974 686f 6e27 7320  atches Python's 
+00001610: 6469 6374 696f 6e61 7279 2066 756e 6374  dictionary funct
+00001620: 696f 6e20 6f66 2074 6865 2073 616d 6520  ion of the same 
+00001630: 6e61 6d65 292e 0a0a 2020 2020 2020 2020  name)...        
+00001640: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
+00001650: 6579 3a20 5468 6520 6964 656e 7469 6669  ey: The identifi
+00001660: 6572 2066 6f72 2074 6865 2063 6f6c 6c65  er for the colle
+00001670: 6374 696f 6e20 6d65 6d62 6572 2e0a 2020  ction member..  
+00001680: 2020 2020 2020 2020 2020 2020 2020 3a74                :t
+00001690: 7970 6520 6b65 793a 2073 7472 0a20 2020  ype key: str.   
+000016a0: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+000016b0: 7261 6d20 6465 6661 756c 743a 204f 7074  ram default: Opt
+000016c0: 696f 6e61 6c20 6172 6775 6d65 6e74 2066  ional argument f
+000016d0: 6f72 2074 6865 2076 616c 7565 2074 6f20  or the value to 
+000016e0: 7265 7475 726e 2069 660a 2020 2020 2020  return if.      
+000016f0: 2020 6b65 7920 6973 206e 6f74 2066 6f75    key is not fou
+00001700: 6e64 2e0a 2020 2020 2020 2020 2222 220a  nd..        """.
+00001710: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
+00001720: 2064 6566 2069 7465 6d73 2873 656c 6629   def items(self)
+00001730: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+00001740: 7572 6e20 7468 6520 6964 656e 7469 6669  urn the identifi
+00001750: 6572 7320 6f66 2063 6f6c 6c65 6374 696f  ers of collectio
+00001760: 6e20 6d65 6d62 6572 730a 2020 2020 2020  n members.      
+00001770: 2020 286d 6174 6368 696e 6720 5079 7468    (matching Pyth
+00001780: 6f6e 2773 2064 6963 742e 6974 656d 7328  on's dict.items(
+00001790: 2920 6675 6e63 7469 6f6e 616c 6974 7929  ) functionality)
+000017a0: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
+000017b0: 2020 203a 7265 7475 726e 3a20 286b 6579     :return: (key
+000017c0: 2c20 7661 6c75 6529 2070 6169 7273 2066  , value) pairs f
+000017d0: 6f72 2065 6163 6820 6d65 6d62 6572 206f  or each member o
+000017e0: 6620 7468 6973 2063 6f6c 6c65 6374 696f  f this collectio
+000017f0: 6e2e 0a20 2020 2020 2020 2022 2222 0a20  n..        """. 
+00001800: 2020 2020 2020 202e 2e2e 0a0a 2020 2020         .....    
+00001810: 6465 6620 6b65 7973 2873 656c 6629 3a0a  def keys(self):.
+00001820: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00001830: 6e20 7468 6520 6964 656e 7469 6669 6572  n the identifier
+00001840: 7320 6f66 2063 6f6c 6c65 6374 696f 6e20  s of collection 
+00001850: 6d65 6d62 6572 730a 2020 2020 2020 2020  members.        
+00001860: 286d 6174 6368 696e 6720 5079 7468 6f6e  (matching Python
+00001870: 2773 2064 6963 742e 6b65 7973 2829 2066  's dict.keys() f
+00001880: 756e 6374 696f 6e61 6c69 7479 292e 0a0a  unctionality)...
+00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018a0: 3a72 6574 7572 6e3a 2074 6865 2069 6465  :return: the ide
+000018b0: 6e74 6966 6965 7273 2066 6f72 2065 6163  ntifiers for eac
+000018c0: 6820 6d65 6d62 6572 206f 6620 7468 6973  h member of this
+000018d0: 2063 6f6c 6c65 6374 696f 6e2e 0a20 2020   collection..   
+000018e0: 2020 2020 2020 2020 2020 2020 203a 7274               :rt
+000018f0: 7970 653a 2074 7970 696e 672e 4c69 7374  ype: typing.List
+00001900: 5b73 7472 5d0a 2020 2020 2020 2020 2222  [str].        ""
+00001910: 220a 2020 2020 2020 2020 2e2e 2e0a 0a20  ".        ..... 
+00001920: 2020 2064 6566 2076 616c 7565 7328 7365     def values(se
+00001930: 6c66 2920 2d3e 2074 7970 696e 672e 4c69  lf) -> typing.Li
+00001940: 7374 5b73 7472 5d3a 0a20 2020 2020 2020  st[str]:.       
+00001950: 2022 2222 5265 7475 726e 2074 6865 2076   """Return the v
+00001960: 616c 7565 7320 6f66 2063 6f6c 6c65 6374  alues of collect
+00001970: 696f 6e0a 2020 2020 2020 2020 286d 6174  ion.        (mat
+00001980: 6368 696e 6720 5079 7468 6f6e 2773 2064  ching Python's d
+00001990: 6963 742e 7661 6c75 6573 2829 2066 756e  ict.values() fun
+000019a0: 6374 696f 6e61 6c69 7479 292e 0a0a 2020  ctionality)...  
+000019b0: 2020 2020 2020 2020 2020 2020 2020 3a72                :r
+000019c0: 6574 7572 6e3a 2074 6865 206d 656d 6265  eturn: the membe
+000019d0: 7273 206f 6620 7468 6973 2063 6f6c 6c65  rs of this colle
+000019e0: 6374 696f 6e2e 0a20 2020 2020 2020 2020  ction..         
+000019f0: 2020 2020 2020 203a 7274 7970 653a 206c         :rtype: l
+00001a00: 6973 740a 2020 2020 2020 2020 2222 220a  ist.        """.
+00001a10: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
+00001a20: 2064 6566 205f 5f67 6574 6974 656d 5f5f   def __getitem__
+00001a30: 2873 656c 662c 206b 6579 3a20 7479 7069  (self, key: typi
+00001a40: 6e67 2e55 6e69 6f6e 5b69 6e74 2c20 7374  ng.Union[int, st
+00001a50: 725d 2920 2d3e 2074 7970 696e 672e 556e  r]) -> typing.Un
+00001a60: 696f 6e5b 696e 742c 2073 7472 5d3a 0a20  ion[int, str]:. 
+00001a70: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00001a80: 2020 2020 3a70 6172 616d 206b 6579 3a0a      :param key:.
+00001a90: 2020 2020 2020 2020 3a74 7970 6520 6b65          :type ke
+00001aa0: 793a 2074 7970 696e 672e 556e 696f 6e5b  y: typing.Union[
+00001ab0: 696e 742c 2073 7472 5d0a 2020 2020 2020  int, str].      
+00001ac0: 2020 3a72 6574 7572 6e3a 0a20 2020 2020    :return:.     
+00001ad0: 2020 203a 7274 7970 653a 2047 656e 6572     :rtype: Gener
+00001ae0: 6963 5479 7065 0a20 2020 2020 2020 2022  icType.        "
+00001af0: 2222 0a20 2020 2020 2020 202e 2e2e 0a0a  "".        .....
+00001b00: 2020 2020 6465 6620 5f5f 7365 7469 7465      def __setite
+00001b10: 6d5f 5f28 7365 6c66 2c20 6b65 793a 2074  m__(self, key: t
+00001b20: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+00001b30: 2073 7472 5d2c 2076 616c 7565 3a20 4765   str], value: Ge
+00001b40: 6e65 7269 6354 7970 6529 3a0a 2020 2020  nericType):.    
+00001b50: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00001b60: 203a 7061 7261 6d20 6b65 793a 0a20 2020   :param key:.   
+00001b70: 2020 2020 203a 7479 7065 206b 6579 3a20       :type key: 
+00001b80: 7479 7069 6e67 2e55 6e69 6f6e 5b69 6e74  typing.Union[int
+00001b90: 2c20 7374 725d 0a20 2020 2020 2020 203a  , str].        :
+00001ba0: 7061 7261 6d20 7661 6c75 653a 0a20 2020  param value:.   
+00001bb0: 2020 2020 203a 7479 7065 2076 616c 7565       :type value
+00001bc0: 3a20 4765 6e65 7269 6354 7970 650a 2020  : GenericType.  
+00001bd0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00001be0: 2020 2e2e 2e0a 0a20 2020 2064 6566 205f    .....    def _
+00001bf0: 5f64 656c 6974 656d 5f5f 2873 656c 662c  _delitem__(self,
+00001c00: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
+00001c10: 6f6e 5b69 6e74 2c20 7374 725d 2920 2d3e  on[int, str]) ->
+00001c20: 2074 7970 696e 672e 556e 696f 6e5b 696e   typing.Union[in
+00001c30: 742c 2073 7472 5d3a 0a20 2020 2020 2020  t, str]:.       
+00001c40: 2022 2222 0a0a 2020 2020 2020 2020 3a70   """..        :p
+00001c50: 6172 616d 206b 6579 3a0a 2020 2020 2020  aram key:.      
+00001c60: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
+00001c70: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
+00001c80: 7472 5d0a 2020 2020 2020 2020 3a72 6574  tr].        :ret
+00001c90: 7572 6e3a 0a20 2020 2020 2020 203a 7274  urn:.        :rt
+00001ca0: 7970 653a 2047 656e 6572 6963 5479 7065  ype: GenericType
+00001cb0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00001cc0: 2020 2020 202e 2e2e 0a0a 2020 2020 6465       .....    de
+00001cd0: 6620 5f5f 6974 6572 5f5f 2873 656c 6629  f __iter__(self)
+00001ce0: 202d 3e20 4765 6e65 7269 6354 7970 653a   -> GenericType:
+00001cf0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00001d00: 2020 2020 2020 3a72 6574 7572 6e3a 0a20        :return:. 
+00001d10: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
+00001d20: 7970 696e 672e 4974 6572 6174 6f72 5b47  yping.Iterator[G
+00001d30: 656e 6572 6963 5479 7065 5d0a 2020 2020  enericType].    
+00001d40: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00001d50: 2e2e 2e0a 0a20 2020 2064 6566 205f 5f6e  .....    def __n
+00001d60: 6578 745f 5f28 7365 6c66 2920 2d3e 2074  ext__(self) -> t
+00001d70: 7970 696e 672e 4974 6572 6174 6f72 5b47  yping.Iterator[G
+00001d80: 656e 6572 6963 5479 7065 5d3a 0a20 2020  enericType]:.   
+00001d90: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00001da0: 2020 3a72 6574 7572 6e3a 0a20 2020 2020    :return:.     
+00001db0: 2020 203a 7274 7970 653a 2047 656e 6572     :rtype: Gener
+00001dc0: 6963 5479 7065 0a20 2020 2020 2020 2022  icType.        "
+00001dd0: 2222 0a20 2020 2020 2020 202e 2e2e 0a0a  "".        .....
+00001de0: 2020 2020 6465 6620 5f5f 6c65 6e5f 5f28      def __len__(
+00001df0: 7365 6c66 2920 2d3e 2047 656e 6572 6963  self) -> Generic
+00001e00: 5479 7065 3a0a 2020 2020 2020 2020 2222  Type:.        ""
+00001e10: 220a 0a20 2020 2020 2020 203a 7265 7475  "..        :retu
+00001e20: 726e 3a0a 2020 2020 2020 2020 3a72 7479  rn:.        :rty
+00001e30: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
+00001e40: 2222 220a 2020 2020 2020 2020 2e2e 2e0a  """.        ....
+00001e50: 0a63 6c61 7373 2062 7079 5f73 7472 7563  .class bpy_struc
+00001e60: 7428 7479 7069 6e67 2e47 656e 6572 6963  t(typing.Generic
+00001e70: 5b47 656e 6572 6963 5479 7065 5d29 3a0a  [GenericType]):.
+00001e80: 2020 2020 2222 2262 7569 6c74 2d69 6e20      """built-in 
+00001e90: 6261 7365 2063 6c61 7373 2066 6f72 2061  base class for a
+00001ea0: 6c6c 2063 6c61 7373 6573 2069 6e20 6270  ll classes in bp
+00001eb0: 792e 7479 7065 732e 2222 220a 0a20 2020  y.types."""..   
+00001ec0: 2069 645f 6461 7461 3a20 7479 7069 6e67   id_data: typing
+00001ed0: 2e41 6e79 0a20 2020 2022 2222 2054 6865  .Any.    """ The
+00001ee0: 2060 6270 792e 7479 7065 732e 4944 6020   `bpy.types.ID` 
+00001ef0: 6f62 6a65 6374 2074 6869 7320 6461 7461  object this data
+00001f00: 626c 6f63 6b20 6973 2066 726f 6d20 6f72  block is from or
+00001f10: 204e 6f6e 652c 2028 6e6f 7420 6176 6169   None, (not avai
+00001f20: 6c61 626c 6520 666f 7220 616c 6c20 6461  lable for all da
+00001f30: 7461 2074 7970 6573 2922 2222 0a0a 2020  ta types)"""..  
+00001f40: 2020 6465 6620 6173 5f70 6f69 6e74 6572    def as_pointer
+00001f50: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00001f60: 2222 2252 6574 7572 6e73 2074 6865 206d  """Returns the m
+00001f70: 656d 6f72 7920 6164 6472 6573 7320 7768  emory address wh
+00001f80: 6963 6820 686f 6c64 7320 6120 706f 696e  ich holds a poin
+00001f90: 7465 7220 746f 2042 6c65 6e64 6572 2773  ter to Blender's
+00001fa0: 2069 6e74 6572 6e61 6c20 6461 7461 0a0a   internal data..
+00001fb0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00001fc0: 2069 6e74 2028 6d65 6d6f 7279 2061 6464   int (memory add
+00001fd0: 7265 7373 292e 0a20 2020 2020 2020 2022  ress)..        "
+00001fe0: 2222 0a20 2020 2020 2020 202e 2e2e 0a0a  "".        .....
+00001ff0: 2020 2020 6465 6620 6472 6976 6572 5f61      def driver_a
+00002000: 6464 2873 656c 662c 2070 6174 683a 2073  dd(self, path: s
+00002010: 7472 2c20 696e 6465 783d 2d31 293a 0a20  tr, index=-1):. 
+00002020: 2020 2020 2020 2022 2222 4164 6473 2064         """Adds d
+00002030: 7269 7665 7228 7329 2074 6f20 7468 6520  river(s) to the 
+00002040: 6769 7665 6e20 7072 6f70 6572 7479 0a0a  given property..
+00002050: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+00002060: 6174 683a 2070 6174 6820 746f 2074 6865  ath: path to the
+00002070: 2070 726f 7065 7274 7920 746f 2064 7269   property to dri
+00002080: 7665 2c20 616e 616c 6f67 6f75 7320 746f  ve, analogous to
+00002090: 2074 6865 2066 6375 7276 6527 7320 6461   the fcurve's da
+000020a0: 7461 2070 6174 682e 0a20 2020 2020 2020  ta path..       
+000020b0: 203a 7479 7065 2070 6174 683a 2073 7472   :type path: str
+000020c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000020d0: 696e 6465 783a 2061 7272 6179 2069 6e64  index: array ind
+000020e0: 6578 206f 6620 7468 6520 7072 6f70 6572  ex of the proper
+000020f0: 7479 2064 7269 7665 2e20 4465 6661 756c  ty drive. Defaul
+00002100: 7473 2074 6f20 2d31 2066 6f72 2061 6c6c  ts to -1 for all
+00002110: 2069 6e64 6963 6573 206f 7220 6120 7369   indices or a si
+00002120: 6e67 6c65 2063 6861 6e6e 656c 2069 6620  ngle channel if 
+00002130: 7468 6520 7072 6f70 6572 7479 2069 7320  the property is 
+00002140: 6e6f 7420 616e 2061 7272 6179 2e0a 2020  not an array..  
+00002150: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
+00002160: 6865 2064 7269 7665 7228 7329 2061 6464  he driver(s) add
+00002170: 6564 2e0a 2020 2020 2020 2020 3a72 7479  ed..        :rty
+00002180: 7065 3a20 4643 7572 7665 0a20 2020 2020  pe: FCurve.     
+00002190: 2020 2022 2222 0a20 2020 2020 2020 202e     """.        .
+000021a0: 2e2e 0a0a 2020 2020 6465 6620 6472 6976  ....    def driv
+000021b0: 6572 5f72 656d 6f76 6528 7365 6c66 2c20  er_remove(self, 
+000021c0: 7061 7468 3a20 7374 722c 2069 6e64 6578  path: str, index
+000021d0: 3d2d 3129 3a0a 2020 2020 2020 2020 2222  =-1):.        ""
+000021e0: 2252 656d 6f76 6520 6472 6976 6572 2873  "Remove driver(s
+000021f0: 2920 6672 6f6d 2074 6865 2067 6976 656e  ) from the given
+00002200: 2070 726f 7065 7274 790a 0a20 2020 2020   property..     
+00002210: 2020 203a 7061 7261 6d20 7061 7468 3a20     :param path: 
+00002220: 7061 7468 2074 6f20 7468 6520 7072 6f70  path to the prop
+00002230: 6572 7479 2074 6f20 6472 6976 652c 2061  erty to drive, a
+00002240: 6e61 6c6f 676f 7573 2074 6f20 7468 6520  nalogous to the 
+00002250: 6663 7572 7665 2773 2064 6174 6120 7061  fcurve's data pa
+00002260: 7468 2e0a 2020 2020 2020 2020 3a74 7970  th..        :typ
+00002270: 6520 7061 7468 3a20 7374 720a 2020 2020  e path: str.    
+00002280: 2020 2020 3a70 6172 616d 2069 6e64 6578      :param index
+00002290: 3a20 6172 7261 7920 696e 6465 7820 6f66  : array index of
+000022a0: 2074 6865 2070 726f 7065 7274 7920 6472   the property dr
+000022b0: 6976 652e 2044 6566 6175 6c74 7320 746f  ive. Defaults to
+000022c0: 202d 3120 666f 7220 616c 6c20 696e 6469   -1 for all indi
+000022d0: 6365 7320 6f72 2061 2073 696e 676c 6520  ces or a single 
+000022e0: 6368 616e 6e65 6c20 6966 2074 6865 2070  channel if the p
+000022f0: 726f 7065 7274 7920 6973 206e 6f74 2061  roperty is not a
+00002300: 6e20 6172 7261 792e 0a20 2020 2020 2020  n array..       
+00002310: 203a 7265 7475 726e 3a20 5375 6363 6573   :return: Succes
+00002320: 7320 6f66 2064 7269 7665 7220 7265 6d6f  s of driver remo
+00002330: 7661 6c2e 0a20 2020 2020 2020 203a 7274  val..        :rt
+00002340: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+00002350: 2020 2222 220a 2020 2020 2020 2020 2e2e    """.        ..
+00002360: 2e0a 0a20 2020 2064 6566 2067 6574 2873  ...    def get(s
+00002370: 656c 662c 206b 6579 3a20 7374 722c 2064  elf, key: str, d
+00002380: 6566 6175 6c74 3d4e 6f6e 6529 3a0a 2020  efault=None):.  
+00002390: 2020 2020 2020 2222 2252 6574 7572 6e73        """Returns
+000023a0: 2074 6865 2076 616c 7565 206f 6620 7468   the value of th
+000023b0: 6520 6375 7374 6f6d 2070 726f 7065 7274  e custom propert
+000023c0: 7920 6173 7369 676e 6564 2074 6f20 6b65  y assigned to ke
+000023d0: 7920 6f72 2064 6566 6175 6c74 0a20 2020  y or default.   
+000023e0: 2020 2020 2077 6865 6e20 6e6f 7420 666f       when not fo
+000023f0: 756e 6420 286d 6174 6368 6573 2050 7974  und (matches Pyt
+00002400: 686f 6e27 7320 6469 6374 696f 6e61 7279  hon's dictionary
+00002410: 2066 756e 6374 696f 6e20 6f66 2074 6865   function of the
+00002420: 2073 616d 6520 6e61 6d65 292e 0a0a 2020   same name)...  
+00002430: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
+00002440: 6172 616d 206b 6579 3a20 5468 6520 6b65  aram key: The ke
+00002450: 7920 6173 736f 6369 6174 6564 2077 6974  y associated wit
+00002460: 6820 7468 6520 6375 7374 6f6d 2070 726f  h the custom pro
+00002470: 7065 7274 792e 0a20 2020 2020 2020 2020  perty..         
+00002480: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
+00002490: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+000024a0: 2020 2020 2020 3a70 6172 616d 2064 6566        :param def
+000024b0: 6175 6c74 3a20 4f70 7469 6f6e 616c 2061  ault: Optional a
+000024c0: 7267 756d 656e 7420 666f 7220 7468 6520  rgument for the 
+000024d0: 7661 6c75 6520 746f 2072 6574 7572 6e20  value to return 
+000024e0: 6966 0a20 2020 2020 2020 206b 6579 2069  if.        key i
+000024f0: 7320 6e6f 7420 666f 756e 642e 0a20 2020  s not found..   
+00002500: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00002510: 202e 2e2e 0a0a 2020 2020 6465 6620 6964   .....    def id
+00002520: 5f70 726f 7065 7274 6965 735f 636c 6561  _properties_clea
+00002530: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+00002540: 2022 2222 0a0a 2020 2020 2020 2020 3a72   """..        :r
+00002550: 6574 7572 6e3a 2052 656d 6f76 6520 7468  eturn: Remove th
+00002560: 6520 7061 7265 6e74 2067 726f 7570 2066  e parent group f
+00002570: 6f72 2061 6e20 524e 4120 7374 7275 6374  or an RNA struct
+00002580: 2773 2063 7573 746f 6d20 4944 5072 6f70  's custom IDProp
+00002590: 6572 7469 6573 2e0a 2020 2020 2020 2020  erties..        
+000025a0: 2222 220a 2020 2020 2020 2020 2e2e 2e0a  """.        ....
+000025b0: 0a20 2020 2064 6566 2069 645f 7072 6f70  .    def id_prop
+000025c0: 6572 7469 6573 5f65 6e73 7572 6528 7365  erties_ensure(se
+000025d0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000025e0: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+000025f0: 6e3a 2074 6865 2070 6172 656e 7420 6772  n: the parent gr
+00002600: 6f75 7020 666f 7220 616e 2052 4e41 2073  oup for an RNA s
+00002610: 7472 7563 7427 7320 6375 7374 6f6d 2049  truct's custom I
+00002620: 4450 726f 7065 7274 6965 732e 0a20 2020  DProperties..   
+00002630: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00002640: 202e 2e2e 0a0a 2020 2020 6465 6620 6964   .....    def id
+00002650: 5f70 726f 7065 7274 6965 735f 7569 2873  _properties_ui(s
+00002660: 656c 662c 206b 6579 293a 0a20 2020 2020  elf, key):.     
+00002670: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00002680: 3a70 6172 616d 206b 6579 3a20 5374 7269  :param key: Stri
+00002690: 6e67 206e 616d 6520 6f66 2074 6865 2070  ng name of the p
+000026a0: 726f 7065 7274 792e 0a20 2020 2020 2020  roperty..       
+000026b0: 203a 7265 7475 726e 3a20 5265 7475 726e   :return: Return
+000026c0: 2061 6e20 6f62 6a65 6374 2075 7365 6420   an object used 
+000026d0: 746f 206d 616e 6167 6520 616e 2049 4450  to manage an IDP
+000026e0: 726f 7065 7274 7927 7320 5549 2064 6174  roperty's UI dat
+000026f0: 612e 0a20 2020 2020 2020 2022 2222 0a20  a..        """. 
+00002700: 2020 2020 2020 202e 2e2e 0a0a 2020 2020         .....    
+00002710: 6465 6620 6973 5f70 726f 7065 7274 795f  def is_property_
+00002720: 6869 6464 656e 2873 656c 662c 2070 726f  hidden(self, pro
+00002730: 7065 7274 7929 3a0a 2020 2020 2020 2020  perty):.        
+00002740: 2222 2243 6865 636b 2069 6620 6120 7072  """Check if a pr
+00002750: 6f70 6572 7479 2069 7320 6869 6464 656e  operty is hidden
+00002760: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00002770: 6d20 7072 6f70 6572 7479 3a0a 2020 2020  m property:.    
+00002780: 2020 2020 3a72 6574 7572 6e3a 2054 7275      :return: Tru
+00002790: 6520 7768 656e 2074 6865 2070 726f 7065  e when the prope
+000027a0: 7274 7920 6973 2068 6964 6465 6e2e 0a20  rty is hidden.. 
+000027b0: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
+000027c0: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
+000027d0: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
+000027e0: 2064 6566 2069 735f 7072 6f70 6572 7479   def is_property
+000027f0: 5f6f 7665 7272 6964 6162 6c65 5f6c 6962  _overridable_lib
+00002800: 7261 7279 2873 656c 662c 2070 726f 7065  rary(self, prope
+00002810: 7274 7929 3a0a 2020 2020 2020 2020 2222  rty):.        ""
+00002820: 2243 6865 636b 2069 6620 6120 7072 6f70  "Check if a prop
+00002830: 6572 7479 2069 7320 6f76 6572 7269 6461  erty is overrida
+00002840: 626c 652e 0a0a 2020 2020 2020 2020 3a70  ble...        :p
+00002850: 6172 616d 2070 726f 7065 7274 793a 0a20  aram property:. 
+00002860: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00002870: 5472 7565 2077 6865 6e20 7468 6520 7072  True when the pr
+00002880: 6f70 6572 7479 2069 7320 6f76 6572 7269  operty is overri
+00002890: 6461 626c 652e 0a20 2020 2020 2020 203a  dable..        :
+000028a0: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
+000028b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000028c0: 2e2e 2e0a 0a20 2020 2064 6566 2069 735f  .....    def is_
+000028d0: 7072 6f70 6572 7479 5f72 6561 646f 6e6c  property_readonl
+000028e0: 7928 7365 6c66 2c20 7072 6f70 6572 7479  y(self, property
+000028f0: 293a 0a20 2020 2020 2020 2022 2222 4368  ):.        """Ch
+00002900: 6563 6b20 6966 2061 2070 726f 7065 7274  eck if a propert
+00002910: 7920 6973 2072 6561 646f 6e6c 792e 0a0a  y is readonly...
+00002920: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+00002930: 726f 7065 7274 793a 0a20 2020 2020 2020  roperty:.       
+00002940: 203a 7265 7475 726e 3a20 5472 7565 2077   :return: True w
+00002950: 6865 6e20 7468 6520 7072 6f70 6572 7479  hen the property
+00002960: 2069 7320 7265 6164 6f6e 6c79 2028 6e6f   is readonly (no
+00002970: 7420 7772 6974 6162 6c65 292e 0a20 2020  t writable)..   
+00002980: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+00002990: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
+000029a0: 2020 2020 2020 2e2e 2e0a 0a20 2020 2064        .....    d
+000029b0: 6566 2069 735f 7072 6f70 6572 7479 5f73  ef is_property_s
+000029c0: 6574 2873 656c 662c 2070 726f 7065 7274  et(self, propert
+000029d0: 792c 2067 686f 7374 3a20 626f 6f6c 203d  y, ghost: bool =
+000029e0: 2054 7275 6529 202d 3e20 626f 6f6c 3a0a   True) -> bool:.
+000029f0: 2020 2020 2020 2020 2222 2243 6865 636b          """Check
+00002a00: 2069 6620 6120 7072 6f70 6572 7479 2069   if a property i
+00002a10: 7320 7365 742c 2075 7365 2066 6f72 2074  s set, use for t
+00002a20: 6573 7469 6e67 206f 7065 7261 746f 7220  esting operator 
+00002a30: 7072 6f70 6572 7469 6573 2e0a 0a20 2020  properties...   
+00002a40: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+00002a50: 7261 6d20 7072 6f70 6572 7479 3a0a 2020  ram property:.  
+00002a60: 2020 2020 2020 2020 2020 2020 2020 3a70                :p
+00002a70: 6172 616d 2067 686f 7374 3a20 5573 6564  aram ghost: Used
+00002a80: 2066 6f72 206f 7065 7261 746f 7273 2074   for operators t
+00002a90: 6861 7420 7265 2d72 756e 2077 6974 6820  hat re-run with 
+00002aa0: 7072 6576 696f 7573 2073 6574 7469 6e67  previous setting
+00002ab0: 732e 0a20 2020 2020 2020 2049 6e20 7468  s..        In th
+00002ac0: 6973 2063 6173 6520 7468 6520 7072 6f70  is case the prop
+00002ad0: 6572 7479 2069 7320 6e6f 7420 6d61 726b  erty is not mark
+00002ae0: 6564 2061 7320 7365 742c 0a20 2020 2020  ed as set,.     
+00002af0: 2020 2079 6574 2074 6865 2076 616c 7565     yet the value
+00002b00: 2066 726f 6d20 7468 6520 7072 6576 696f   from the previo
+00002b10: 7573 2065 7865 6375 7469 6f6e 2069 7320  us execution is 
+00002b20: 7573 6564 2e0a 0a20 2020 2020 2020 2049  used...        I
+00002b30: 6e20 7261 7265 2063 6173 6573 2079 6f75  n rare cases you
+00002b40: 206d 6179 2077 616e 7420 746f 2073 6574   may want to set
+00002b50: 2074 6869 7320 6f70 7469 6f6e 2074 6f20   this option to 
+00002b60: 6661 6c73 652e 0a20 2020 2020 2020 2020  false..         
+00002b70: 2020 2020 2020 203a 7479 7065 2067 686f         :type gho
+00002b80: 7374 3a20 626f 6f6c 0a20 2020 2020 2020  st: bool.       
+00002b90: 2020 2020 2020 2020 203a 7265 7475 726e           :return
+00002ba0: 3a20 5472 7565 2077 6865 6e20 7468 6520  : True when the 
+00002bb0: 7072 6f70 6572 7479 2068 6173 2062 6565  property has bee
+00002bc0: 6e20 7365 742e 0a20 2020 2020 2020 2020  n set..         
+00002bd0: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
+00002be0: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
+00002bf0: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
+00002c00: 2064 6566 2069 7465 6d73 2873 656c 6629   def items(self)
+00002c10: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00002c20: 2020 2222 2252 6574 7572 6e73 2074 6865    """Returns the
+00002c30: 2069 7465 6d73 206f 6620 7468 6973 206f   items of this o
+00002c40: 626a 6563 7473 2063 7573 746f 6d20 7072  bjects custom pr
+00002c50: 6f70 6572 7469 6573 2028 6d61 7463 6865  operties (matche
+00002c60: 7320 5079 7468 6f6e 2773 0a20 2020 2020  s Python's.     
+00002c70: 2020 2064 6963 7469 6f6e 6172 7920 6675     dictionary fu
+00002c80: 6e63 7469 6f6e 206f 6620 7468 6520 7361  nction of the sa
+00002c90: 6d65 206e 616d 6529 2e0a 0a20 2020 2020  me name)...     
+00002ca0: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
+00002cb0: 726e 3a20 6375 7374 6f6d 2070 726f 7065  rn: custom prope
+00002cc0: 7274 7920 6b65 792c 2076 616c 7565 2070  rty key, value p
+00002cd0: 6169 7273 2e0a 2020 2020 2020 2020 2222  airs..        ""
+00002ce0: 220a 2020 2020 2020 2020 2e2e 2e0a 0a20  ".        ..... 
+00002cf0: 2020 2064 6566 206b 6579 6672 616d 655f     def keyframe_
+00002d00: 6465 6c65 7465 280a 2020 2020 2020 2020  delete(.        
+00002d10: 7365 6c66 2c20 6461 7461 5f70 6174 683a  self, data_path:
+00002d20: 2073 7472 2c20 696e 6465 783d 2d31 2c20   str, index=-1, 
+00002d30: 6672 616d 653d 4e6f 6e65 2c20 6772 6f75  frame=None, grou
+00002d40: 703a 2073 7472 203d 2022 220a 2020 2020  p: str = "".    
+00002d50: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+00002d60: 2020 2222 2252 656d 6f76 6520 6120 6b65    """Remove a ke
+00002d70: 7966 7261 6d65 2066 726f 6d20 7468 6973  yframe from this
+00002d80: 2070 726f 7065 7274 6965 7320 6663 7572   properties fcur
+00002d90: 7665 2e0a 0a20 2020 2020 2020 203a 7061  ve...        :pa
+00002da0: 7261 6d20 6461 7461 5f70 6174 683a 2070  ram data_path: p
+00002db0: 6174 6820 746f 2074 6865 2070 726f 7065  ath to the prope
+00002dc0: 7274 7920 746f 2072 656d 6f76 6520 6120  rty to remove a 
+00002dd0: 6b65 792c 2061 6e61 6c6f 676f 7573 2074  key, analogous t
+00002de0: 6f20 7468 6520 6663 7572 7665 2773 2064  o the fcurve's d
+00002df0: 6174 6120 7061 7468 2e0a 2020 2020 2020  ata path..      
+00002e00: 2020 3a74 7970 6520 6461 7461 5f70 6174    :type data_pat
+00002e10: 683a 2073 7472 0a20 2020 2020 2020 203a  h: str.        :
+00002e20: 7061 7261 6d20 696e 6465 783a 2061 7272  param index: arr
+00002e30: 6179 2069 6e64 6578 206f 6620 7468 6520  ay index of the 
+00002e40: 7072 6f70 6572 7479 2074 6f20 7265 6d6f  property to remo
+00002e50: 7665 2061 206b 6579 2e20 4465 6661 756c  ve a key. Defaul
+00002e60: 7473 2074 6f20 2d31 2072 656d 6f76 696e  ts to -1 removin
+00002e70: 6720 616c 6c20 696e 6469 6365 7320 6f72  g all indices or
+00002e80: 2061 2073 696e 676c 6520 6368 616e 6e65   a single channe
+00002e90: 6c20 6966 2074 6865 2070 726f 7065 7274  l if the propert
+00002ea0: 7920 6973 206e 6f74 2061 6e20 6172 7261  y is not an arra
+00002eb0: 792e 0a20 2020 2020 2020 203a 7061 7261  y..        :para
+00002ec0: 6d20 6672 616d 653a 2054 6865 2066 7261  m frame: The fra
+00002ed0: 6d65 206f 6e20 7768 6963 6820 7468 6520  me on which the 
+00002ee0: 6b65 7966 7261 6d65 2069 7320 6465 6c65  keyframe is dele
+00002ef0: 7465 642c 2064 6566 6175 6c74 696e 6720  ted, defaulting 
+00002f00: 746f 2074 6865 2063 7572 7265 6e74 2066  to the current f
+00002f10: 7261 6d65 2e0a 2020 2020 2020 2020 3a70  rame..        :p
+00002f20: 6172 616d 2067 726f 7570 3a20 5468 6520  aram group: The 
+00002f30: 6e61 6d65 206f 6620 7468 6520 6772 6f75  name of the grou
+00002f40: 7020 7468 6520 462d 4375 7276 6520 7368  p the F-Curve sh
+00002f50: 6f75 6c64 2062 6520 6164 6465 6420 746f  ould be added to
+00002f60: 2069 6620 6974 2064 6f65 736e 2774 2065   if it doesn't e
+00002f70: 7869 7374 2079 6574 2e0a 2020 2020 2020  xist yet..      
+00002f80: 2020 3a74 7970 6520 6772 6f75 703a 2073    :type group: s
+00002f90: 7472 0a20 2020 2020 2020 203a 7265 7475  tr.        :retu
+00002fa0: 726e 3a20 5375 6363 6573 7320 6f66 206b  rn: Success of k
+00002fb0: 6579 6672 616d 6520 6465 6c65 7469 6f6e  eyframe deletion
+00002fc0: 2e0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+00002fd0: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
+00002fe0: 2222 0a20 2020 2020 2020 202e 2e2e 0a0a  "".        .....
+00002ff0: 2020 2020 6465 6620 6b65 7966 7261 6d65      def keyframe
+00003000: 5f69 6e73 6572 7428 0a20 2020 2020 2020  _insert(.       
+00003010: 2073 656c 662c 2064 6174 615f 7061 7468   self, data_path
+00003020: 3a20 7374 722c 2069 6e64 6578 3d2d 312c  : str, index=-1,
+00003030: 2066 7261 6d65 3d4e 6f6e 652c 2067 726f   frame=None, gro
+00003040: 7570 3a20 7374 7220 3d20 2222 2c20 6f70  up: str = "", op
+00003050: 7469 6f6e 733d 4e6f 6e65 2829 0a20 2020  tions=None().   
+00003060: 2029 3a0a 2020 2020 2020 2020 2222 2249   ):.        """I
+00003070: 6e73 6572 7420 6120 6b65 7966 7261 6d65  nsert a keyframe
+00003080: 206f 6e20 7468 6520 7072 6f70 6572 7479   on the property
+00003090: 2067 6976 656e 2c20 6164 6469 6e67 2066   given, adding f
+000030a0: 6375 7276 6573 2061 6e64 2061 6e69 6d61  curves and anima
+000030b0: 7469 6f6e 2064 6174 6120 7768 656e 206e  tion data when n
+000030c0: 6563 6573 7361 7279 2e54 6869 7320 6973  ecessary.This is
+000030d0: 2074 6865 206d 6f73 7420 7369 6d70 6c65   the most simple
+000030e0: 2065 7861 6d70 6c65 206f 6620 696e 7365   example of inse
+000030f0: 7274 696e 6720 6120 6b65 7966 7261 6d65  rting a keyframe
+00003100: 2066 726f 6d20 7079 7468 6f6e 2e4e 6f74   from python.Not
+00003110: 6520 7468 6174 2077 6865 6e20 6b65 7969  e that when keyi
+00003120: 6e67 2064 6174 6120 7061 7468 7320 7768  ng data paths wh
+00003130: 6963 6820 636f 6e74 6169 6e20 6e65 7374  ich contain nest
+00003140: 6564 2070 726f 7065 7274 6965 7320 7468  ed properties th
+00003150: 6973 206d 7573 7420 6265 0a20 2020 2020  is must be.     
+00003160: 2020 2064 6f6e 6520 6672 6f6d 2074 6865     done from the
+00003170: 2060 4944 6020 7375 6263 6c61 7373 2c20   `ID` subclass, 
+00003180: 696e 2074 6869 7320 6361 7365 2074 6865  in this case the
+00003190: 2060 4172 6d61 7475 7265 6020 7261 7468   `Armature` rath
+000031a0: 6572 0a20 2020 2020 2020 2074 6861 6e20  er.        than 
+000031b0: 7468 6520 626f 6e65 2e0a 0a20 2020 2020  the bone...     
+000031c0: 2020 2020 2020 2020 2020 203a 7061 7261             :para
+000031d0: 6d20 6461 7461 5f70 6174 683a 2070 6174  m data_path: pat
+000031e0: 6820 746f 2074 6865 2070 726f 7065 7274  h to the propert
+000031f0: 7920 746f 206b 6579 2c20 616e 616c 6f67  y to key, analog
+00003200: 6f75 7320 746f 2074 6865 2066 6375 7276  ous to the fcurv
+00003210: 6527 7320 6461 7461 2070 6174 682e 0a20  e's data path.. 
+00003220: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+00003230: 7479 7065 2064 6174 615f 7061 7468 3a20  type data_path: 
+00003240: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+00003250: 2020 2020 3a70 6172 616d 2069 6e64 6578      :param index
+00003260: 3a20 6172 7261 7920 696e 6465 7820 6f66  : array index of
+00003270: 2074 6865 2070 726f 7065 7274 7920 746f   the property to
+00003280: 206b 6579 2e0a 2020 2020 2020 2020 4465   key..        De
+00003290: 6661 756c 7473 2074 6f20 2d31 2077 6869  faults to -1 whi
+000032a0: 6368 2077 696c 6c20 6b65 7920 616c 6c20  ch will key all 
+000032b0: 696e 6469 6365 7320 6f72 2061 2073 696e  indices or a sin
+000032c0: 676c 6520 6368 616e 6e65 6c20 6966 2074  gle channel if t
+000032d0: 6865 2070 726f 7065 7274 7920 6973 206e  he property is n
+000032e0: 6f74 2061 6e20 6172 7261 792e 0a20 2020  ot an array..   
+000032f0: 2020 2020 2020 2020 2020 2020 203a 7061               :pa
+00003300: 7261 6d20 6672 616d 653a 2054 6865 2066  ram frame: The f
+00003310: 7261 6d65 206f 6e20 7768 6963 6820 7468  rame on which th
+00003320: 6520 6b65 7966 7261 6d65 2069 7320 696e  e keyframe is in
+00003330: 7365 7274 6564 2c20 6465 6661 756c 7469  serted, defaulti
+00003340: 6e67 2074 6f20 7468 6520 6375 7272 656e  ng to the curren
+00003350: 7420 6672 616d 652e 0a20 2020 2020 2020  t frame..       
+00003360: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00003370: 6772 6f75 703a 2054 6865 206e 616d 6520  group: The name 
+00003380: 6f66 2074 6865 2067 726f 7570 2074 6865  of the group the
+00003390: 2046 2d43 7572 7665 2073 686f 756c 6420   F-Curve should 
+000033a0: 6265 2061 6464 6564 2074 6f20 6966 2069  be added to if i
+000033b0: 7420 646f 6573 6e27 7420 6578 6973 7420  t doesn't exist 
+000033c0: 7965 742e 0a20 2020 2020 2020 2020 2020  yet..           
+000033d0: 2020 2020 203a 7479 7065 2067 726f 7570       :type group
+000033e0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+000033f0: 2020 2020 2020 3a70 6172 616d 206f 7074        :param opt
+00003400: 696f 6e73 3a20 4f70 7469 6f6e 616c 2073  ions: Optional s
+00003410: 6574 206f 6620 666c 6167 733a 0a0a 2020  et of flags:..  
+00003420: 2020 2020 2020 494e 5345 5254 4b45 595f        INSERTKEY_
+00003430: 4e45 4544 4544 204f 6e6c 7920 696e 7365  NEEDED Only inse
+00003440: 7274 206b 6579 6672 616d 6573 2077 6865  rt keyframes whe
+00003450: 7265 2074 6865 7927 7265 206e 6565 6465  re they're neede
+00003460: 6420 696e 2074 6865 2072 656c 6576 616e  d in the relevan
+00003470: 7420 462d 4375 7276 6573 2e0a 0a20 2020  t F-Curves...   
+00003480: 2020 2020 2049 4e53 4552 544b 4559 5f56       INSERTKEY_V
+00003490: 4953 5541 4c20 496e 7365 7274 206b 6579  ISUAL Insert key
+000034a0: 6672 616d 6573 2062 6173 6564 206f 6e20  frames based on 
+000034b0: 2776 6973 7561 6c20 7472 616e 7366 6f72  'visual transfor
+000034c0: 6d73 272e 0a0a 2020 2020 2020 2020 494e  ms'...        IN
+000034d0: 5345 5254 4b45 595f 5859 5a5f 544f 5f52  SERTKEY_XYZ_TO_R
+000034e0: 4742 2054 6869 7320 666c 6167 2069 7320  GB This flag is 
+000034f0: 6e6f 206c 6f6e 6765 7220 696e 2075 7365  no longer in use
+00003500: 2c20 616e 6420 6973 2068 6572 6520 736f  , and is here so
+00003510: 2074 6861 7420 636f 6465 2074 6861 7420   that code that 
+00003520: 7573 6573 2069 7420 646f 6573 6e27 7420  uses it doesn't 
+00003530: 6272 6561 6b2e 2054 6865 2058 595a 3d52  break. The XYZ=R
+00003540: 4742 2063 6f6c 6f72 696e 6720 6973 2064  GB coloring is d
+00003550: 6574 6572 6d69 6e65 6420 6279 2074 6865  etermined by the
+00003560: 2061 6e69 6d61 7469 6f6e 2070 7265 6665   animation prefe
+00003570: 7265 6e63 6573 2e0a 0a20 2020 2020 2020  rences...       
+00003580: 2049 4e53 4552 544b 4559 5f52 4550 4c41   INSERTKEY_REPLA
+00003590: 4345 204f 6e6c 7920 7265 706c 6163 6520  CE Only replace 
+000035a0: 616c 7265 6164 7920 6578 6973 7469 6e67  already existing
+000035b0: 206b 6579 6672 616d 6573 2e0a 0a20 2020   keyframes...   
+000035c0: 2020 2020 2049 4e53 4552 544b 4559 5f41       INSERTKEY_A
+000035d0: 5641 494c 4142 4c45 204f 6e6c 7920 696e  VAILABLE Only in
+000035e0: 7365 7274 2069 6e74 6f20 616c 7265 6164  sert into alread
+000035f0: 7920 6578 6973 7469 6e67 2046 2d43 7572  y existing F-Cur
+00003600: 7665 732e 0a0a 2020 2020 2020 2020 494e  ves...        IN
+00003610: 5345 5254 4b45 595f 4359 434c 455f 4157  SERTKEY_CYCLE_AW
+00003620: 4152 4520 5461 6b65 2063 7963 6c69 6320  ARE Take cyclic 
+00003630: 6578 7472 6170 6f6c 6174 696f 6e20 696e  extrapolation in
+00003640: 746f 2061 6363 6f75 6e74 2028 4379 636c  to account (Cycl
+00003650: 652d 4177 6172 6520 4b65 7969 6e67 206f  e-Aware Keying o
+00003660: 7074 696f 6e29 2e0a 2020 2020 2020 2020  ption)..        
+00003670: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00003680: 2053 7563 6365 7373 206f 6620 6b65 7966   Success of keyf
+00003690: 7261 6d65 2069 6e73 6572 7469 6f6e 2e0a  rame insertion..
+000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036b0: 3a72 7479 7065 3a20 626f 6f6c 0a20 2020  :rtype: bool.   
+000036c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000036d0: 202e 2e2e 0a0a 2020 2020 6465 6620 6b65   .....    def ke
+000036e0: 7973 2873 656c 6629 202d 3e20 626f 6f6c  ys(self) -> bool
+000036f0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+00003700: 7572 6e73 2074 6865 206b 6579 7320 6f66  urns the keys of
+00003710: 2074 6869 7320 6f62 6a65 6374 7320 6375   this objects cu
+00003720: 7374 6f6d 2070 726f 7065 7274 6965 7320  stom properties 
+00003730: 286d 6174 6368 6573 2050 7974 686f 6e27  (matches Python'
+00003740: 730a 2020 2020 2020 2020 6469 6374 696f  s.        dictio
+00003750: 6e61 7279 2066 756e 6374 696f 6e20 6f66  nary function of
+00003760: 2074 6865 2073 616d 6520 6e61 6d65 292e   the same name).
+00003770: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003780: 2020 3a72 6574 7572 6e3a 2063 7573 746f    :return: custo
+00003790: 6d20 7072 6f70 6572 7479 206b 6579 732e  m property keys.
+000037a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000037b0: 2020 2020 202e 2e2e 0a0a 2020 2020 6465       .....    de
+000037c0: 6620 7061 7468 5f66 726f 6d5f 6964 2873  f path_from_id(s
+000037d0: 656c 662c 2070 726f 7065 7274 793a 2073  elf, property: s
+000037e0: 7472 203d 2022 2229 202d 3e20 7374 723a  tr = "") -> str:
+000037f0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00003800: 726e 7320 7468 6520 6461 7461 2070 6174  rns the data pat
+00003810: 6820 6672 6f6d 2074 6865 2049 4420 746f  h from the ID to
+00003820: 2074 6869 7320 6f62 6a65 6374 2028 7374   this object (st
+00003830: 7269 6e67 292e 0a0a 2020 2020 2020 2020  ring)...        
+00003840: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+00003850: 726f 7065 7274 793a 204f 7074 696f 6e61  roperty: Optiona
+00003860: 6c20 7072 6f70 6572 7479 206e 616d 6520  l property name 
+00003870: 7768 6963 6820 6361 6e20 6265 2075 7365  which can be use
+00003880: 6420 6966 2074 6865 2070 6174 6820 6973  d if the path is
+00003890: 0a20 2020 2020 2020 2074 6f20 6120 7072  .        to a pr
+000038a0: 6f70 6572 7479 206f 6620 7468 6973 206f  operty of this o
+000038b0: 626a 6563 742e 0a20 2020 2020 2020 2020  bject..         
+000038c0: 2020 2020 2020 203a 7479 7065 2070 726f         :type pro
+000038d0: 7065 7274 793a 2073 7472 0a20 2020 2020  perty: str.     
+000038e0: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
+000038f0: 726e 3a20 5468 6520 7061 7468 2066 726f  rn: The path fro
+00003900: 6d20 6062 7079 2e74 7970 6573 2e62 7079  m `bpy.types.bpy
+00003910: 5f73 7472 7563 742e 6964 5f64 6174 6160  _struct.id_data`
+00003920: 0a20 2020 2020 2020 2074 6f20 7468 6973  .        to this
+00003930: 2073 7472 7563 7420 616e 6420 7072 6f70   struct and prop
+00003940: 6572 7479 2028 7768 656e 2067 6976 656e  erty (when given
+00003950: 292e 0a20 2020 2020 2020 2020 2020 2020  )..             
+00003960: 2020 203a 7274 7970 653a 2073 7472 0a20     :rtype: str. 
+00003970: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00003980: 2020 202e 2e2e 0a0a 2020 2020 6465 6620     .....    def 
+00003990: 7061 7468 5f72 6573 6f6c 7665 2873 656c  path_resolve(sel
+000039a0: 662c 2070 6174 683a 2073 7472 2c20 636f  f, path: str, co
+000039b0: 6572 6365 3a20 626f 6f6c 203d 2054 7275  erce: bool = Tru
+000039c0: 6529 3a0a 2020 2020 2020 2020 2222 2252  e):.        """R
+000039d0: 6574 7572 6e73 2074 6865 2070 726f 7065  eturns the prope
+000039e0: 7274 7920 6672 6f6d 2074 6865 2070 6174  rty from the pat
+000039f0: 682c 2072 6169 7365 2061 6e20 6578 6365  h, raise an exce
+00003a00: 7074 696f 6e20 7768 656e 206e 6f74 2066  ption when not f
+00003a10: 6f75 6e64 2e0a 0a20 2020 2020 2020 2020  ound...         
+00003a20: 2020 2020 2020 203a 7061 7261 6d20 7061         :param pa
+00003a30: 7468 3a20 7061 7468 2077 6869 6368 2074  th: path which t
+00003a40: 6869 7320 7072 6f70 6572 7479 2072 6573  his property res
+00003a50: 6f6c 7665 732e 0a20 2020 2020 2020 2020  olves..         
+00003a60: 2020 2020 2020 203a 7479 7065 2070 6174         :type pat
+00003a70: 683a 2073 7472 0a20 2020 2020 2020 2020  h: str.         
+00003a80: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
+00003a90: 6572 6365 3a20 6f70 7469 6f6e 616c 2061  erce: optional a
+00003aa0: 7267 756d 656e 742c 2077 6865 6e20 5472  rgument, when Tr
+00003ab0: 7565 2c20 7468 6520 7072 6f70 6572 7479  ue, the property
+00003ac0: 2077 696c 6c20 6265 2063 6f6e 7665 7274   will be convert
+00003ad0: 6564 0a20 2020 2020 2020 2069 6e74 6f20  ed.        into 
+00003ae0: 6974 7320 5079 7468 6f6e 2072 6570 7265  its Python repre
+00003af0: 7365 6e74 6174 696f 6e2e 0a20 2020 2020  sentation..     
+00003b00: 2020 2020 2020 2020 2020 203a 7479 7065             :type
+00003b10: 2063 6f65 7263 653a 2062 6f6f 6c0a 2020   coerce: bool.  
+00003b20: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00003b30: 2020 2e2e 2e0a 0a20 2020 2064 6566 2070    .....    def p
+00003b40: 6f70 2873 656c 662c 206b 6579 3a20 7374  op(self, key: st
+00003b50: 722c 2064 6566 6175 6c74 3d4e 6f6e 6529  r, default=None)
+00003b60: 3a0a 2020 2020 2020 2020 2222 2252 656d  :.        """Rem
+00003b70: 6f76 6520 616e 6420 7265 7475 726e 2074  ove and return t
+00003b80: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
+00003b90: 6375 7374 6f6d 2070 726f 7065 7274 7920  custom property 
+00003ba0: 6173 7369 676e 6564 2074 6f20 6b65 7920  assigned to key 
+00003bb0: 6f72 2064 6566 6175 6c74 0a20 2020 2020  or default.     
+00003bc0: 2020 2077 6865 6e20 6e6f 7420 666f 756e     when not foun
+00003bd0: 6420 286d 6174 6368 6573 2050 7974 686f  d (matches Pytho
+00003be0: 6e27 7320 6469 6374 696f 6e61 7279 2066  n's dictionary f
+00003bf0: 756e 6374 696f 6e20 6f66 2074 6865 2073  unction of the s
+00003c00: 616d 6520 6e61 6d65 292e 0a0a 2020 2020  ame name)...    
+00003c10: 2020 2020 2020 2020 2020 2020 3a70 6172              :par
+00003c20: 616d 206b 6579 3a20 5468 6520 6b65 7920  am key: The key 
+00003c30: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
+00003c40: 7468 6520 6375 7374 6f6d 2070 726f 7065  the custom prope
+00003c50: 7274 792e 0a20 2020 2020 2020 2020 2020  rty..           
+00003c60: 2020 2020 203a 7479 7065 206b 6579 3a20       :type key: 
+00003c70: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+00003c80: 2020 2020 3a70 6172 616d 2064 6566 6175      :param defau
+00003c90: 6c74 3a20 4f70 7469 6f6e 616c 2061 7267  lt: Optional arg
+00003ca0: 756d 656e 7420 666f 7220 7468 6520 7661  ument for the va
+00003cb0: 6c75 6520 746f 2072 6574 7572 6e20 6966  lue to return if
+00003cc0: 0a20 2020 2020 2020 206b 6579 2069 7320  .        key is 
+00003cd0: 6e6f 7420 666f 756e 642e 0a20 2020 2020  not found..     
+00003ce0: 2020 2022 2222 0a20 2020 2020 2020 202e     """.        .
+00003cf0: 2e2e 0a0a 2020 2020 6465 6620 7072 6f70  ....    def prop
+00003d00: 6572 7479 5f6f 7665 7272 6964 6162 6c65  erty_overridable
+00003d10: 5f6c 6962 7261 7279 5f73 6574 2873 656c  _library_set(sel
+00003d20: 662c 2070 726f 7065 7274 792c 206f 7665  f, property, ove
+00003d30: 7272 6964 6162 6c65 293a 0a20 2020 2020  rridable):.     
+00003d40: 2020 2022 2222 4465 6669 6e65 2061 2070     """Define a p
+00003d50: 726f 7065 7274 7920 6173 206f 7665 7272  roperty as overr
+00003d60: 6964 6162 6c65 206f 7220 6e6f 7420 286f  idable or not (o
+00003d70: 6e6c 7920 666f 7220 6375 7374 6f6d 2070  nly for custom p
+00003d80: 726f 7065 7274 6965 7321 292e 0a0a 2020  roperties!)...  
+00003d90: 2020 2020 2020 3a70 6172 616d 2070 726f        :param pro
+00003da0: 7065 7274 793a 0a20 2020 2020 2020 203a  perty:.        :
+00003db0: 7061 7261 6d20 6f76 6572 7269 6461 626c  param overridabl
+00003dc0: 653a 0a20 2020 2020 2020 203a 7265 7475  e:.        :retu
+00003dd0: 726e 3a20 5472 7565 2077 6865 6e20 7468  rn: True when th
+00003de0: 6520 6f76 6572 7269 6461 626c 6520 7374  e overridable st
+00003df0: 6174 7573 206f 6620 7468 6520 7072 6f70  atus of the prop
+00003e00: 6572 7479 2077 6173 2073 7563 6365 7373  erty was success
+00003e10: 6675 6c6c 7920 7365 742e 0a20 2020 2020  fully set..     
+00003e20: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
+00003e30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00003e40: 2020 2020 2e2e 2e0a 0a20 2020 2064 6566      .....    def
+00003e50: 2070 726f 7065 7274 795f 756e 7365 7428   property_unset(
+00003e60: 7365 6c66 2c20 7072 6f70 6572 7479 293a  self, property):
+00003e70: 0a20 2020 2020 2020 2022 2222 556e 7365  .        """Unse
+00003e80: 7420 6120 7072 6f70 6572 7479 2c20 7769  t a property, wi
+00003e90: 6c6c 2075 7365 2064 6566 6175 6c74 2076  ll use default v
+00003ea0: 616c 7565 2061 6674 6572 7761 7264 2e0a  alue afterward..
+00003eb0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00003ec0: 7072 6f70 6572 7479 3a0a 2020 2020 2020  property:.      
+00003ed0: 2020 2222 220a 2020 2020 2020 2020 2e2e    """.        ..
+00003ee0: 2e0a 0a20 2020 2064 6566 2074 7970 655f  ...    def type_
+00003ef0: 7265 6361 7374 2873 656c 6629 3a0a 2020  recast(self):.  
+00003f00: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00003f10: 6120 6e65 7720 696e 7374 616e 6365 2c20  a new instance, 
+00003f20: 7468 6973 2069 7320 6e65 6564 6564 2062  this is needed b
+00003f30: 6563 6175 7365 2074 7970 6573 0a20 2020  ecause types.   
+00003f40: 2020 2020 2073 7563 6820 6173 2074 6578       such as tex
+00003f50: 7475 7265 7320 6361 6e20 6265 2063 6861  tures can be cha
+00003f60: 6e67 6564 2061 7420 7275 6e74 696d 652e  nged at runtime.
+00003f70: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003f80: 2020 3a72 6574 7572 6e3a 2061 206e 6577    :return: a new
+00003f90: 2069 6e73 7461 6e63 6520 6f66 2074 6869   instance of thi
+00003fa0: 7320 6f62 6a65 6374 2077 6974 6820 7468  s object with th
+00003fb0: 6520 7479 7065 2069 6e69 7469 616c 697a  e type initializ
+00003fc0: 6564 2061 6761 696e 2e0a 2020 2020 2020  ed again..      
+00003fd0: 2020 2222 220a 2020 2020 2020 2020 2e2e    """.        ..
+00003fe0: 2e0a 0a20 2020 2064 6566 2076 616c 7565  ...    def value
+00003ff0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00004000: 2022 2222 5265 7475 726e 7320 7468 6520   """Returns the 
+00004010: 7661 6c75 6573 206f 6620 7468 6973 206f  values of this o
+00004020: 626a 6563 7473 2063 7573 746f 6d20 7072  bjects custom pr
+00004030: 6f70 6572 7469 6573 2028 6d61 7463 6865  operties (matche
+00004040: 7320 5079 7468 6f6e 2773 0a20 2020 2020  s Python's.     
+00004050: 2020 2064 6963 7469 6f6e 6172 7920 6675     dictionary fu
+00004060: 6e63 7469 6f6e 206f 6620 7468 6520 7361  nction of the sa
+00004070: 6d65 206e 616d 6529 2e0a 0a20 2020 2020  me name)...     
+00004080: 2020 2020 2020 2020 2020 203a 7265 7475             :retu
+00004090: 726e 3a20 6375 7374 6f6d 2070 726f 7065  rn: custom prope
+000040a0: 7274 7920 7661 6c75 6573 2e0a 2020 2020  rty values..    
+000040b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000040c0: 2e2e 2e0a 0a20 2020 2064 6566 205f 5f67  .....    def __g
+000040d0: 6574 6974 656d 5f5f 2873 656c 662c 206b  etitem__(self, k
+000040e0: 6579 3a20 7479 7069 6e67 2e55 6e69 6f6e  ey: typing.Union
+000040f0: 5b69 6e74 2c20 7374 725d 2920 2d3e 2074  [int, str]) -> t
+00004100: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+00004110: 2073 7472 5d3a 0a20 2020 2020 2020 2022   str]:.        "
+00004120: 2222 0a0a 2020 2020 2020 2020 3a70 6172  ""..        :par
+00004130: 616d 206b 6579 3a0a 2020 2020 2020 2020  am key:.        
+00004140: 3a74 7970 6520 6b65 793a 2074 7970 696e  :type key: typin
+00004150: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
+00004160: 5d0a 2020 2020 2020 2020 3a72 6574 7572  ].        :retur
+00004170: 6e3a 0a20 2020 2020 2020 203a 7274 7970  n:.        :rtyp
+00004180: 653a 2074 7970 696e 672e 416e 790a 2020  e: typing.Any.  
+00004190: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000041a0: 2020 2e2e 2e0a 0a20 2020 2064 6566 205f    .....    def _
+000041b0: 5f73 6574 6974 656d 5f5f 2873 656c 662c  _setitem__(self,
+000041c0: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
+000041d0: 6f6e 5b69 6e74 2c20 7374 725d 2c20 7661  on[int, str], va
+000041e0: 6c75 653a 2074 7970 696e 672e 416e 7929  lue: typing.Any)
+000041f0: 3a0a 2020 2020 2020 2020 2222 220a 0a20  :.        """.. 
+00004200: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
+00004210: 793a 0a20 2020 2020 2020 203a 7479 7065  y:.        :type
+00004220: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
+00004230: 6f6e 5b69 6e74 2c20 7374 725d 0a20 2020  on[int, str].   
+00004240: 2020 2020 203a 7061 7261 6d20 7661 6c75       :param valu
+00004250: 653a 0a20 2020 2020 2020 203a 7479 7065  e:.        :type
+00004260: 2076 616c 7565 3a20 7479 7069 6e67 2e41   value: typing.A
+00004270: 6e79 0a20 2020 2020 2020 2022 2222 0a20  ny.        """. 
+00004280: 2020 2020 2020 202e 2e2e 0a0a 2020 2020         .....    
+00004290: 6465 6620 5f5f 6465 6c69 7465 6d5f 5f28  def __delitem__(
+000042a0: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
+000042b0: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
+000042c0: 5d29 202d 3e20 7479 7069 6e67 2e55 6e69  ]) -> typing.Uni
+000042d0: 6f6e 5b69 6e74 2c20 7374 725d 3a0a 2020  on[int, str]:.  
+000042e0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+000042f0: 2020 203a 7061 7261 6d20 6b65 793a 0a20     :param key:. 
+00004300: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
+00004310: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b69  : typing.Union[i
+00004320: 6e74 2c20 7374 725d 0a20 2020 2020 2020  nt, str].       
+00004330: 203a 7265 7475 726e 3a0a 2020 2020 2020   :return:.      
+00004340: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
+00004350: 2e41 6e79 0a20 2020 2020 2020 2022 2222  .Any.        """
 00004360: 0a20 2020 2020 2020 202e 2e2e 0a0a 636c  .        .....cl
 00004370: 6173 7320 4465 7073 6772 6170 683a 0a20  ass Depsgraph:. 
 00004380: 2020 2022 2222 2022 2222 0a0a 2020 2020     """ """..    
 00004390: 6964 733a 2062 7079 5f70 726f 705f 636f  ids: bpy_prop_co
 000043a0: 6c6c 6563 7469 6f6e 5b49 445d 0a20 2020  llection[ID].   
 000043b0: 2022 2222 2041 6c6c 2065 7661 6c75 6174   """ All evaluat
 000043c0: 6564 2064 6174 612d 626c 6f63 6b73 0a0a  ed data-blocks..
@@ -89148,18 +89148,18 @@
 0015c3b0: 564f 4b45 5f44 4546 4155 4c54 222c 0a20  VOKE_DEFAULT",. 
 0015c3c0: 2020 2020 2020 2070 726f 7065 7274 6965         propertie
 0015c3d0: 733a 2074 7970 696e 672e 556e 696f 6e5b  s: typing.Union[
 0015c3e0: 4f70 6572 6174 6f72 5072 6f70 6572 7469  OperatorProperti
 0015c3f0: 6573 2c20 7479 7069 6e67 2e41 6e79 5d20  es, typing.Any] 
 0015c400: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
 0015c410: 696e 636c 7564 653a 2074 7970 696e 672e  include: typing.
-0015c420: 416e 7920 3d20 7b27 224e 444f 4622 272c  Any = {'"NDOF"',
-0015c430: 2027 224d 4f55 5345 2227 2c20 2722 4143   '"MOUSE"', '"AC
-0015c440: 5449 4f4e 5a4f 4e45 2227 2c20 2722 4b45  TIONZONE"', '"KE
-0015c450: 5942 4f41 5244 2227 7d2c 0a20 2020 2020  YBOARD"'},.     
+0015c420: 416e 7920 3d20 7b27 224b 4559 424f 4152  Any = {'"KEYBOAR
+0015c430: 4422 272c 2027 224d 4f55 5345 2227 2c20  D"', '"MOUSE"', 
+0015c440: 2722 4143 5449 4f4e 5a4f 4e45 2227 2c20  '"ACTIONZONE"', 
+0015c450: 2722 4e44 4f46 2227 7d2c 0a20 2020 2020  '"NDOF"'},.     
 0015c460: 2020 2065 7863 6c75 6465 3a20 7479 7069     exclude: typi
 0015c470: 6e67 2e41 6e79 203d 207b 7d2c 0a20 2020  ng.Any = {},.   
 0015c480: 2029 202d 3e20 7479 7069 6e67 2e41 6e79   ) -> typing.Any
 0015c490: 3a0a 2020 2020 2020 2020 2222 2266 696e  :.        """fin
 0015c4a0: 645f 6974 656d 5f66 726f 6d5f 6f70 6572  d_item_from_oper
 0015c4b0: 6174 6f72 0a0a 2020 2020 2020 2020 2020  ator..          
 0015c4c0: 2020 2020 2020 3a70 6172 616d 2069 646e        :param idn
@@ -89913,17 +89913,17 @@
 0015f380: 6e67 2e41 6e79 5d2c 0a20 2020 2020 2020  ng.Any],.       
 0015f390: 2070 726f 7065 7274 6965 733a 2074 7970   properties: typ
 0015f3a0: 696e 672e 556e 696f 6e5b 4f70 6572 6174  ing.Union[Operat
 0015f3b0: 6f72 5072 6f70 6572 7469 6573 2c20 7479  orProperties, ty
 0015f3c0: 7069 6e67 2e41 6e79 5d20 3d20 4e6f 6e65  ping.Any] = None
 0015f3d0: 2c0a 2020 2020 2020 2020 696e 636c 7564  ,.        includ
 0015f3e0: 653a 2074 7970 696e 672e 416e 7920 3d20  e: typing.Any = 
-0015f3f0: 7b27 224e 444f 4622 272c 2027 224d 4f55  {'"NDOF"', '"MOU
-0015f400: 5345 2227 2c20 2722 4143 5449 4f4e 5a4f  SE"', '"ACTIONZO
-0015f410: 4e45 2227 2c20 2722 4b45 5942 4f41 5244  NE"', '"KEYBOARD
+0015f3f0: 7b27 224b 4559 424f 4152 4422 272c 2027  {'"KEYBOARD"', '
+0015f400: 224d 4f55 5345 2227 2c20 2722 4143 5449  "MOUSE"', '"ACTI
+0015f410: 4f4e 5a4f 4e45 2227 2c20 2722 4e44 4f46  ONZONE"', '"NDOF
 0015f420: 2227 7d2c 0a20 2020 2020 2020 2065 7863  "'},.        exc
 0015f430: 6c75 6465 3a20 7479 7069 6e67 2e41 6e79  lude: typing.Any
 0015f440: 203d 207b 7d2c 0a20 2020 2029 202d 3e20   = {},.    ) -> 
 0015f450: 7479 7069 6e67 2e41 6e79 3a0a 2020 2020  typing.Any:.    
 0015f460: 2020 2020 2222 2266 696e 645f 6672 6f6d      """find_from
 0015f470: 5f6f 7065 7261 746f 720a 0a20 2020 2020  _operator..     
 0015f480: 2020 203a 7061 7261 6d20 6964 6e61 6d65     :param idname
```

### Comparing `fake-bpy-module-latest-20240407/bpy/utils/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/utils/previews/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/utils/previews/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy/utils/units/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy/utils/units/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy_extras/anim_utils/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy_extras/anim_utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy_extras/image_utils/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy_extras/image_utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy_extras/io_utils/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy_extras/io_utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy_extras/mesh_utils/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy_extras/mesh_utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy_extras/object_utils/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy_extras/object_utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy_extras/view3d_utils/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy_extras/view3d_utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/bpy_types/__init__.pyi` & `fake-bpy-module-latest-20240408/bpy_types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/console_python/__init__.pyi` & `fake-bpy-module-latest-20240408/console_python/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/fake_bpy_module_latest.egg-info/PKG-INFO` & `fake-bpy-module-latest-20240408/fake_bpy_module_latest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake-bpy-module-latest
-Version: 20240407
+Version: 20240408
 Summary: Collection of the fake Blender Python API module for the code completion.
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 Project-URL: Homepage, https://github.com/nutti/fake-bpy-module
 Project-URL: Documentation, https://github.com/nutti/fake-bpy-module/blob/master/README.md
```

### Comparing `fake-bpy-module-latest-20240407/fake_bpy_module_latest.egg-info/SOURCES.txt` & `fake-bpy-module-latest-20240408/fake_bpy_module_latest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/freestyle/chainingiterators/__init__.pyi` & `fake-bpy-module-latest-20240408/freestyle/chainingiterators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/freestyle/functions/__init__.pyi` & `fake-bpy-module-latest-20240408/freestyle/functions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/freestyle/predicates/__init__.pyi` & `fake-bpy-module-latest-20240408/freestyle/predicates/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/freestyle/shaders/__init__.pyi` & `fake-bpy-module-latest-20240408/freestyle/shaders/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/freestyle/types/__init__.pyi` & `fake-bpy-module-latest-20240408/freestyle/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/freestyle/utils/ContextFunctions/__init__.pyi` & `fake-bpy-module-latest-20240408/freestyle/utils/ContextFunctions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/freestyle/utils/__init__.pyi` & `fake-bpy-module-latest-20240408/freestyle/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/gpu/capabilities/__init__.pyi` & `fake-bpy-module-latest-20240408/gpu/capabilities/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/gpu/matrix/__init__.pyi` & `fake-bpy-module-latest-20240408/gpu/matrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/gpu/platform/__init__.pyi` & `fake-bpy-module-latest-20240408/gpu/platform/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/gpu/shader/__init__.pyi` & `fake-bpy-module-latest-20240408/gpu/shader/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/gpu/state/__init__.pyi` & `fake-bpy-module-latest-20240408/gpu/state/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/gpu/texture/__init__.pyi` & `fake-bpy-module-latest-20240408/gpu/texture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/gpu/types/__init__.pyi` & `fake-bpy-module-latest-20240408/gpu/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/gpu_extras/batch/__init__.pyi` & `fake-bpy-module-latest-20240408/gpu_extras/batch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/gpu_extras/presets/__init__.pyi` & `fake-bpy-module-latest-20240408/gpu_extras/presets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/idprop/types/__init__.pyi` & `fake-bpy-module-latest-20240408/idprop/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/imbuf/__init__.pyi` & `fake-bpy-module-latest-20240408/imbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/imbuf/types/__init__.pyi` & `fake-bpy-module-latest-20240408/imbuf/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/keyingsets_builtins/__init__.pyi` & `fake-bpy-module-latest-20240408/keyingsets_builtins/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/keyingsets_utils/__init__.pyi` & `fake-bpy-module-latest-20240408/keyingsets_utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/mathutils/__init__.pyi` & `fake-bpy-module-latest-20240408/mathutils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/mathutils/bvhtree/__init__.pyi` & `fake-bpy-module-latest-20240408/mathutils/bvhtree/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/mathutils/geometry/__init__.pyi` & `fake-bpy-module-latest-20240408/mathutils/geometry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/mathutils/kdtree/__init__.pyi` & `fake-bpy-module-latest-20240408/mathutils/kdtree/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/mathutils/noise/__init__.pyi` & `fake-bpy-module-latest-20240408/mathutils/noise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/nodeitems_builtins/__init__.pyi` & `fake-bpy-module-latest-20240408/nodeitems_builtins/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/nodeitems_utils/__init__.pyi` & `fake-bpy-module-latest-20240408/nodeitems_utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/pyproject.toml` & `fake-bpy-module-latest-20240408/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/rna_info/__init__.pyi` & `fake-bpy-module-latest-20240408/rna_info/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/rna_keymap_ui/__init__.pyi` & `fake-bpy-module-latest-20240408/rna_keymap_ui/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/rna_prop_ui/__init__.pyi` & `fake-bpy-module-latest-20240408/rna_prop_ui/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20240407/rna_xml/__init__.pyi` & `fake-bpy-module-latest-20240408/rna_xml/__init__.pyi`

 * *Files identical despite different names*

