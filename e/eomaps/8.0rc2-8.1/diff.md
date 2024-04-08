# Comparing `tmp/eomaps-8.0rc2.tar.gz` & `tmp/eomaps-8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eomaps-8.0rc2.tar", last modified: Mon Mar 11 08:59:27 2024, max compression
+gzip compressed data, was "eomaps-8.1.tar", last modified: Mon Apr  8 19:34:29 2024, max compression
```

## Comparing `eomaps-8.0rc2.tar` & `eomaps-8.1.tar`

### file list

```diff
@@ -1,98 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:59:27.562565 eomaps-8.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-11 08:59:19.000000 eomaps-8.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-03-11 08:59:27.562565 eomaps-8.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-03-11 08:59:19.000000 eomaps-8.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:59:27.554565 eomaps-8.0rc2/eomaps/
--rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/NE_features.json
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54130 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/_blit_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    47841 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    50349 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/_webmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    24787 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/annotation_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    49430 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    79076 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/cb_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    56576 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    20504 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/compass.py
--rw-r--r--   0 runner    (1001) docker     (127)    28816 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)   197191 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/eomaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    35784 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16320 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/inset_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)    37068 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/layout_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    86617 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    17423 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/mapsgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/ne_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/projections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:59:27.554565 eomaps-8.0rc2/eomaps/qtcompanion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:59:27.558565 eomaps-8.0rc2/eomaps/qtcompanion/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/close.png
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/edit_layout.png
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/edit_layout_active.png
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/edit_layout_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/eye_closed.png
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/eye_open.png
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/info.png
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/info_checked.png
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/info_hoover.png
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/layers.png
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/layers_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)    86617 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/maximize.png
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/open.png
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/open_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_bottom.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_bottom_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_circle.png
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_circle_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_ellipse.png
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_ellipse_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_left.png
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_left_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_rectangle.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_rectangle_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_right.png
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_right_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_square.png
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_square_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_top.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_top_active.png
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/icons/plus_hoover.png
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/qtcompanion/signal_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    52422 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    56318 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/scalebar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:59:27.558565 eomaps-8.0rc2/eomaps/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/scripts/open.py
--rw-r--r--   0 runner    (1001) docker     (127)    82577 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)    21493 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    91116 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/webmap_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18151 2024-03-11 08:59:19.000000 eomaps-8.0rc2/eomaps/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:59:27.562565 eomaps-8.0rc2/eomaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-03-11 08:59:27.000000 eomaps-8.0rc2/eomaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-03-11 08:59:27.000000 eomaps-8.0rc2/eomaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 08:59:27.000000 eomaps-8.0rc2/eomaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-11 08:59:27.000000 eomaps-8.0rc2/eomaps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-11 08:59:27.000000 eomaps-8.0rc2/eomaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 08:59:27.000000 eomaps-8.0rc2/eomaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-03-11 08:59:19.000000 eomaps-8.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 08:59:27.562565 eomaps-8.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:59:27.562565 eomaps-8.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_WMS_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    43808 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_basic_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    29217 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_doc_codeblocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_doc_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_layout_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_plot_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_raster_aggregaton.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-03-11 08:59:19.000000 eomaps-8.0rc2/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:34:28.999928 eomaps-8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-08 19:34:16.000000 eomaps-8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-04-08 19:34:28.999928 eomaps-8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-04-08 19:34:16.000000 eomaps-8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:34:28.983928 eomaps-8.1/eomaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/NE_features.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54130 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/_blit_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48962 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50349 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/_webmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24787 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/annotation_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49562 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79214 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/cb_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57306 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20504 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/compass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28800 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)   198736 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/eomaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35956 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/inset_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37516 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/layout_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86617 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17423 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/mapsgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/ne_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/projections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:34:28.987928 eomaps-8.1/eomaps/qtcompanion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:34:28.991928 eomaps-8.1/eomaps/qtcompanion/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/close.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/edit_layout.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/edit_layout_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/edit_layout_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/eye_closed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/eye_open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/info.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/info_checked.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/info_hoover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/layers.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/layers_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86617 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/maximize.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/open_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_bottom.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_bottom_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_circle.png
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_circle_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_ellipse.png
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_ellipse_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_left_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_rectangle.png
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_rectangle_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_right_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_square_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_top.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/peek_top_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/icons/plus_hoover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/signal_container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:34:28.995928 eomaps-8.1/eomaps/qtcompanion/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23702 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/widgets/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19962 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/widgets/click_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/widgets/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62338 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/widgets/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/widgets/extent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46849 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/widgets/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15167 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/widgets/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20418 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/widgets/peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/widgets/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31928 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/qtcompanion/widgets/wms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51631 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56857 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/scalebar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:34:28.995928 eomaps-8.1/eomaps/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/scripts/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82983 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21493 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91116 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/webmap_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18151 2024-04-08 19:34:16.000000 eomaps-8.1/eomaps/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:34:28.995928 eomaps-8.1/eomaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-04-08 19:34:28.000000 eomaps-8.1/eomaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-08 19:34:28.000000 eomaps-8.1/eomaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:34:28.000000 eomaps-8.1/eomaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 19:34:28.000000 eomaps-8.1/eomaps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 19:34:28.000000 eomaps-8.1/eomaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 19:34:28.000000 eomaps-8.1/eomaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-08 19:34:16.000000 eomaps-8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:34:28.999928 eomaps-8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:34:28.995928 eomaps-8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_WMS_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44313 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_basic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29217 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_doc_codeblocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_doc_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_layout_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_plot_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_raster_aggregaton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-08 19:34:16.000000 eomaps-8.1/tests/test_widgets.py
```

### Comparing `eomaps-8.0rc2/LICENSE` & `eomaps-8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/PKG-INFO` & `eomaps-8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eomaps
-Version: 8.0rc2
+Version: 8.1
 Summary: A library to create interactive maps of geographical datasets.
 Author-email: Raphael Quast <raphael.quast@geo.tuwien.ac.at>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, The EOmaps authors.
         
         Redistribution and use in source and binary forms, with or without
@@ -66,28 +66,36 @@
 Provides-Extra: classify
 Requires-Dist: mapclassify; extra == "classify"
 Provides-Extra: wms
 Requires-Dist: owslib; extra == "wms"
 Requires-Dist: requests; extra == "wms"
 Provides-Extra: shade
 Requires-Dist: datashader; extra == "shade"
+Requires-Dist: dask[dataframe]; extra == "shade"
 Provides-Extra: gui
 Requires-Dist: PyQt5; extra == "gui"
 Requires-Dist: qtpy; extra == "gui"
 
 
 <p align="center">
     <a href=https://github.com/raphaelquast/EOmaps>
     <img src="https://github.com/raphaelquast/EOmaps/blob/master/docs/_static/logo.png?raw=true" alt="EOmaps logo" width="55%">
     </a>
 </p>
 
-| Tests | Package | Documentation | License | Citation |
-|:-:|:-:|:-:|:-:|:-:|
-| [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/testMaps.yml/badge.svg?branch=master)](https://github.com/raphaelquast/EOmaps/actions/workflows/testMaps.yml)  [![codecov](https://codecov.io/gh/raphaelquast/EOmaps/graph/badge.svg)](https://codecov.io/gh/raphaelquast/EOmaps) | [![pypi](https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/eomaps/)  [![Conda Version](https://img.shields.io/conda/vn/conda-forge/eomaps.svg)](https://anaconda.org/conda-forge/eomaps) | [![Documentation Status](https://readthedocs.org/projects/eomaps/badge/?version=latest)](https://eomaps.readthedocs.io/en/latest/?badge=latest) |  [![License: BSD 3 clause](https://img.shields.io/badge/License-BSD_3_clause-blue.svg)](https://github.com/raphaelquast/EOmaps/blob/master/LICENSE) | [![10.5281/zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/badge/latestdoi/410829039) |
+<div align="center">
+
+
+|     Tests & Review      | [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/testMaps.yml/badge.svg?branch=master)](https://github.com/raphaelquast/EOmaps/actions/workflows/testMaps.yml) | [![codecov](https://codecov.io/gh/raphaelquast/EOmaps/graph/badge.svg)](https://codecov.io/gh/raphaelquast/EOmaps)  |                    [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/138)                    |
+| :---------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------: |
+| Package & Documentation |                                                [![pypi](https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/eomaps/)                                                 | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/eomaps.svg)](https://anaconda.org/conda-forge/eomaps) | [![Documentation Status](https://readthedocs.org/projects/eomaps/badge/?version=latest)](https://eomaps.readthedocs.io/en/latest/?badge=latest) |
+|   License & Citation    |                [![License: BSD 3 clause](https://img.shields.io/badge/License-BSD_3_clause-blue.svg)](https://github.com/raphaelquast/EOmaps/blob/master/LICENSE)                |  [![10.5281/zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/badge/latestdoi/410829039)  |                                                                                                                                                 |
+
+
+</div>
 
 <a href="https://www.buymeacoffee.com/raphaelquast" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png" alt="Buy Me A Coffee" align="right" style="height: 25px !important;" ></a>
 <a href="https://app.gitter.im/#/room/#EOmaps:gitter.im" target="_blank"><img src="https://img.shields.io/gitter/room/raphaelquast/EOmaps?style=social" alt="chat on gitter" align="left" style="height: 20px !important;" ></a>
 
 ----
 
 <h3 align="center">A python package to visualize and analyze geographical datasets.</h3>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eomaps Version: 8.0rc2 Summary: A library to create
+Metadata-Version: 2.1 Name: eomaps Version: 8.1 Summary: A library to create
 interactive maps of geographical datasets. Author-email: Raphael Quast
 geo.tuwien.ac.at> License: BSD 3-Clause License Copyright (c) 2021, The EOmaps
 authors. Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
@@ -34,31 +34,40 @@
 [classify,gui,io,shade,wms]; extra == "all" Provides-Extra: all-nogui Requires-
 Dist: eomaps[classify,io,shade,wms]; extra == "all-nogui" Provides-Extra: io
 Requires-Dist: pandas; extra == "io" Requires-Dist: geopandas; extra == "io"
 Requires-Dist: xarray; extra == "io" Requires-Dist: netcdf4; extra == "io"
 Requires-Dist: rioxarray; extra == "io" Provides-Extra: classify Requires-Dist:
 mapclassify; extra == "classify" Provides-Extra: wms Requires-Dist: owslib;
 extra == "wms" Requires-Dist: requests; extra == "wms" Provides-Extra: shade
-Requires-Dist: datashader; extra == "shade" Provides-Extra: gui Requires-Dist:
-PyQt5; extra == "gui" Requires-Dist: qtpy; extra == "gui"
+Requires-Dist: datashader; extra == "shade" Requires-Dist: dask[dataframe];
+extra == "shade" Provides-Extra: gui Requires-Dist: PyQt5; extra == "gui"
+Requires-Dist: qtpy; extra == "gui"
                                  _[_E_O_m_a_p_s_ _l_o_g_o_]
-| Tests | Package | Documentation | License | Citation | |:-:|:-:|:-:|:-:|:-:
-| | [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/
-testMaps.yml/badge.svg?branch=master)](https://github.com/raphaelquast/EOmaps/
-actions/workflows/testMaps.yml) [![codecov](https://codecov.io/gh/raphaelquast/
-EOmaps/graph/badge.svg)](https://codecov.io/gh/raphaelquast/EOmaps) | [![pypi]
-(https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/eomaps/) [!
-[Conda Version](https://img.shields.io/conda/vn/conda-forge/eomaps.svg)](https:
-//anaconda.org/conda-forge/eomaps) | [![Documentation Status](https://
-readthedocs.org/projects/eomaps/badge/?version=latest)](https://
-eomaps.readthedocs.io/en/latest/?badge=latest) | [![License: BSD 3 clause]
-(https://img.shields.io/badge/License-BSD_3_clause-blue.svg)](https://
-github.com/raphaelquast/EOmaps/blob/master/LICENSE) | [![10.5281/
-zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/
-badge/latestdoi/410829039) | _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]_[_c_h_a_t_ _o_n_ _g_i_t_t_e_r_]----
+ | Tests & Review | [![tests](https://github.com/raphaelquast/EOmaps/actions/
+     workflows/testMaps.yml/badge.svg?branch=master)](https://github.com/
+  raphaelquast/EOmaps/actions/workflows/testMaps.yml) | [![codecov](https://
+  codecov.io/gh/raphaelquast/EOmaps/graph/badge.svg)](https://codecov.io/gh/
+ raphaelquast/EOmaps) | [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://
+github.com/pyOpenSci/software-submission/issues/138) | | :--------------------
+-: | :-------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+----------------------: | :----------------------------------------------------
+-------------------------------------------------------------: | :-------------
+-------------------------------------------------------------------------------
+-------------------------------------------------: | | Package & Documentation
+  | [![pypi](https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/
+   eomaps/) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/
+   eomaps.svg)](https://anaconda.org/conda-forge/eomaps) | [![Documentation
+Status](https://readthedocs.org/projects/eomaps/badge/?version=latest)](https:/
+  /eomaps.readthedocs.io/en/latest/?badge=latest) | | License & Citation | [!
+  [License: BSD 3 clause](https://img.shields.io/badge/License-BSD_3_clause-
+  blue.svg)](https://github.com/raphaelquast/EOmaps/blob/master/LICENSE) | [!
+  [10.5281/zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://
+                   zenodo.org/badge/latestdoi/410829039) | |
+_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]_[_c_h_a_t_ _o_n_ _g_i_t_t_e_r_]----
   ******** AA ppyytthhoonn ppaacckkaaggee ttoo vviissuuaalliizzee aanndd aannaallyyzzee ggeeooggrraapphhiiccaall ddaattaasseettss.. ********
 EEOOmmaappss aims to provide a comprehensive, flexible, well-documented and easy-to-
 use API to create publication-ready maps that can directly be used for
 interactive data analysis.
 ## What can I do with EOmaps? **EOmaps** is built on top of [matplotlib](https:
 //matplotlib.org/) and [cartopy](https://scitools.org.uk/cartopy/docs/latest/
 ) and integrates well with the scientific python infrastructure (e.g., [numpy]
```

### Comparing `eomaps-8.0rc2/README.md` & `eomaps-8.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 
 <p align="center">
     <a href=https://github.com/raphaelquast/EOmaps>
     <img src="https://github.com/raphaelquast/EOmaps/blob/master/docs/_static/logo.png?raw=true" alt="EOmaps logo" width="55%">
     </a>
 </p>
 
-| Tests | Package | Documentation | License | Citation |
-|:-:|:-:|:-:|:-:|:-:|
-| [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/testMaps.yml/badge.svg?branch=master)](https://github.com/raphaelquast/EOmaps/actions/workflows/testMaps.yml)  [![codecov](https://codecov.io/gh/raphaelquast/EOmaps/graph/badge.svg)](https://codecov.io/gh/raphaelquast/EOmaps) | [![pypi](https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/eomaps/)  [![Conda Version](https://img.shields.io/conda/vn/conda-forge/eomaps.svg)](https://anaconda.org/conda-forge/eomaps) | [![Documentation Status](https://readthedocs.org/projects/eomaps/badge/?version=latest)](https://eomaps.readthedocs.io/en/latest/?badge=latest) |  [![License: BSD 3 clause](https://img.shields.io/badge/License-BSD_3_clause-blue.svg)](https://github.com/raphaelquast/EOmaps/blob/master/LICENSE) | [![10.5281/zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/badge/latestdoi/410829039) |
+<div align="center">
+
+
+|     Tests & Review      | [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/testMaps.yml/badge.svg?branch=master)](https://github.com/raphaelquast/EOmaps/actions/workflows/testMaps.yml) | [![codecov](https://codecov.io/gh/raphaelquast/EOmaps/graph/badge.svg)](https://codecov.io/gh/raphaelquast/EOmaps)  |                    [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/138)                    |
+| :---------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------: |
+| Package & Documentation |                                                [![pypi](https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/eomaps/)                                                 | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/eomaps.svg)](https://anaconda.org/conda-forge/eomaps) | [![Documentation Status](https://readthedocs.org/projects/eomaps/badge/?version=latest)](https://eomaps.readthedocs.io/en/latest/?badge=latest) |
+|   License & Citation    |                [![License: BSD 3 clause](https://img.shields.io/badge/License-BSD_3_clause-blue.svg)](https://github.com/raphaelquast/EOmaps/blob/master/LICENSE)                |  [![10.5281/zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/badge/latestdoi/410829039)  |                                                                                                                                                 |
+
+
+</div>
 
 <a href="https://www.buymeacoffee.com/raphaelquast" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png" alt="Buy Me A Coffee" align="right" style="height: 25px !important;" ></a>
 <a href="https://app.gitter.im/#/room/#EOmaps:gitter.im" target="_blank"><img src="https://img.shields.io/gitter/room/raphaelquast/EOmaps?style=social" alt="chat on gitter" align="left" style="height: 20px !important;" ></a>
 
 ----
 
 <h3 align="center">A python package to visualize and analyze geographical datasets.</h3>
```

#### html2text {}

```diff
@@ -1,22 +1,30 @@
                                  _[_E_O_m_a_p_s_ _l_o_g_o_]
-| Tests | Package | Documentation | License | Citation | |:-:|:-:|:-:|:-:|:-:
-| | [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/
-testMaps.yml/badge.svg?branch=master)](https://github.com/raphaelquast/EOmaps/
-actions/workflows/testMaps.yml) [![codecov](https://codecov.io/gh/raphaelquast/
-EOmaps/graph/badge.svg)](https://codecov.io/gh/raphaelquast/EOmaps) | [![pypi]
-(https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/eomaps/) [!
-[Conda Version](https://img.shields.io/conda/vn/conda-forge/eomaps.svg)](https:
-//anaconda.org/conda-forge/eomaps) | [![Documentation Status](https://
-readthedocs.org/projects/eomaps/badge/?version=latest)](https://
-eomaps.readthedocs.io/en/latest/?badge=latest) | [![License: BSD 3 clause]
-(https://img.shields.io/badge/License-BSD_3_clause-blue.svg)](https://
-github.com/raphaelquast/EOmaps/blob/master/LICENSE) | [![10.5281/
-zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/
-badge/latestdoi/410829039) | _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]_[_c_h_a_t_ _o_n_ _g_i_t_t_e_r_]----
+ | Tests & Review | [![tests](https://github.com/raphaelquast/EOmaps/actions/
+     workflows/testMaps.yml/badge.svg?branch=master)](https://github.com/
+  raphaelquast/EOmaps/actions/workflows/testMaps.yml) | [![codecov](https://
+  codecov.io/gh/raphaelquast/EOmaps/graph/badge.svg)](https://codecov.io/gh/
+ raphaelquast/EOmaps) | [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://
+github.com/pyOpenSci/software-submission/issues/138) | | :--------------------
+-: | :-------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+----------------------: | :----------------------------------------------------
+-------------------------------------------------------------: | :-------------
+-------------------------------------------------------------------------------
+-------------------------------------------------: | | Package & Documentation
+  | [![pypi](https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/
+   eomaps/) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/
+   eomaps.svg)](https://anaconda.org/conda-forge/eomaps) | [![Documentation
+Status](https://readthedocs.org/projects/eomaps/badge/?version=latest)](https:/
+  /eomaps.readthedocs.io/en/latest/?badge=latest) | | License & Citation | [!
+  [License: BSD 3 clause](https://img.shields.io/badge/License-BSD_3_clause-
+  blue.svg)](https://github.com/raphaelquast/EOmaps/blob/master/LICENSE) | [!
+  [10.5281/zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://
+                   zenodo.org/badge/latestdoi/410829039) | |
+_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]_[_c_h_a_t_ _o_n_ _g_i_t_t_e_r_]----
   ******** AA ppyytthhoonn ppaacckkaaggee ttoo vviissuuaalliizzee aanndd aannaallyyzzee ggeeooggrraapphhiiccaall ddaattaasseettss.. ********
 EEOOmmaappss aims to provide a comprehensive, flexible, well-documented and easy-to-
 use API to create publication-ready maps that can directly be used for
 interactive data analysis.
 ## What can I do with EOmaps? **EOmaps** is built on top of [matplotlib](https:
 //matplotlib.org/) and [cartopy](https://scitools.org.uk/cartopy/docs/latest/
 ) and integrates well with the scientific python infrastructure (e.g., [numpy]
```

### Comparing `eomaps-8.0rc2/eomaps/NE_features.json` & `eomaps-8.1/eomaps/NE_features.json`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/__init__.py` & `eomaps-8.1/eomaps/__init__.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/_blit_manager.py` & `eomaps-8.1/eomaps/_blit_manager.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/_containers.py` & `eomaps-8.1/eomaps/_containers.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/_data_manager.py` & `eomaps-8.1/eomaps/_data_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -240,54 +240,70 @@
                 parameter = cols[0]
 
             assert len(data[parameter].dims) <= 2, (
                 "EOmaps: provided dataset has more than 2 dimensions..."
                 f"({data[parameter].dims})."
             )
             z_data = data[parameter].values
+            data_dims = data[parameter].dims
         else:
             assert len(data.dims) <= 2, (
                 "EOmaps: provided dataset has more than 2 dimensions..."
                 f"({data.dims})."
             )
 
             z_data = data.values
+            data_dims = data.dims
             parameter = data.name
 
         # use numeric index values
         ids = range(z_data.size)
 
-        if isinstance(x, str) and isinstance(y, str):
+        if isinstance(x, str) and isinstance(y, str):  #
             coords = list(data.coords)
             if (x in coords) and (y in coords):
                 # get the coordinates from coordinates
                 xorig = data.coords[x].values
                 yorig = data.coords[y].values
-                # transpose dat in case x is before y
-                # (to account for matrix indexing order)
-                if coords.index(x) > coords.index(y):
-                    z_data = z_data.T
+                x_dims = data.coords[x].dims
+                y_dims = data.coords[y].dims
 
             elif (x in data) and (y in data):
                 xorig = data[x].values
                 yorig = data[y].values
+                x_dims = data[x].dims
+                y_dims = data[y].dims
 
         elif (x is None) and (y is None):
             coords = list(data.coords)
 
             if len(coords) == 2:
                 # get the coordinates from index-values
                 xorig = data[coords[0]].values
                 yorig = data[coords[1]].values
+                x_dims = data[coords[0]].dims
+                y_dims = data[coords[1]].dims
             else:
                 raise TypeError(
                     "EOmaps: Either specify explicit coordinate-names to use "
                     "for `x` and `y` or pass a Dataset with exactly 2 "
                     "coordinates!"
                 )
+
+        # transpose dat in case data is transposed
+        # (to account for matrix indexing order)
+        # TODO make this prperly
+        if not (data_dims == x_dims and data_dims == y_dims):
+            if len(x_dims) == 2 and len(y_dims) == 2:
+                if data_dims == x_dims[::-1]:
+                    z_data = z_data.T
+            elif len(x_dims) == 1 and len(y_dims) == 1:
+                if data_dims.index(x_dims[0]) > data_dims.index(y_dims[0]):
+                    z_data = z_data.T
+
         return z_data, xorig, yorig, ids, parameter
 
     def _identify_array_like(self, data=None, x=None, y=None, parameter=None):
         def check_dtype(val):
             if val is None:
                 return True
 
@@ -409,14 +425,26 @@
         # in case we use in_crs == plot_crs
         crs1 = CRS.from_user_input(in_crs)
         crs2 = CRS.from_user_input(self.m._crs_plot)
 
         # identify the provided data and get it in the internal format
         z_data, xorig, yorig, ids, parameter = self._identify_data()
 
+        # check if Fill-value is provided, and mask the data accordingly
+        if self.m.data_specs.encoding:
+            fill_value = self.m.data_specs.encoding.get("_FillValue", None)
+            if fill_value:
+                z_data = np.ma.MaskedArray(
+                    data=z_data,
+                    mask=z_data == fill_value,
+                    copy=False,
+                    fill_value=fill_value,
+                    hard_mask=True,
+                )
+
         if cpos is not None and cpos != "c":
             # fix position of pixel-center in the input-crs
             assert (
                 cpos_radius is not None
             ), "you must specify a 'cpos_radius if 'cpos' is not 'c'"
             if isinstance(cpos_radius, (list, tuple)):
                 rx, ry = cpos_radius
@@ -730,15 +758,15 @@
             self._remove_existing_coll()
             # draw the new collection
             coll = self.m._get_coll(props, **self.m._coll_kwargs)
             coll.set_clim(self.m._vmin, self.m._vmax)
 
             coll.set_label("Dataset " f"({self.m.shape.name}  |  {self.z_data.shape})")
 
-            if self.m.shape.name not in ["scatter_points", "contour"]:
+            if self.m.shape.name not in ["scatter_points", "contour", "hexbin"]:
                 # avoid use "autolim=True" since it can cause problems in
                 # case the data-limits are infinite (e.g. for projected
                 # datasets containing points outside the used projection)
                 # the extent is set by calling "._set_lims()" in `m.plot_map()`
                 self.m.ax.add_collection(coll, autolim=False)
 
             if self.m._coll_dynamic:
```

### Comparing `eomaps-8.0rc2/eomaps/_webmap.py` & `eomaps-8.1/eomaps/_webmap.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/annotation_editor.py` & `eomaps-8.1/eomaps/annotation_editor.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/callbacks.py` & `eomaps-8.1/eomaps/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,20 +387,25 @@
             val_precision=4,
             text=text,
             show_all_values=show_all_values,
         )
 
         if printstr is not None:
             # create a new annotation
-            if not multipick:
-                bbox = dict(boxstyle="round", fc="w", ec=val_color)
-                bbox.update(kwargs.pop("bbox", dict()))
+            inp_bbox = kwargs.pop("bbox", dict())
+
+            if inp_bbox is not None:
+                if not multipick:
+                    bbox = dict(boxstyle="round", fc="w", ec=val_color)
+                    bbox.update(inp_bbox)
+                else:
+                    bbox = dict(boxstyle="round", fc="w", ec="k")
+                    bbox.update(inp_bbox)
             else:
-                bbox = dict(boxstyle="round", fc="w", ec="k")
-                bbox.update(kwargs.pop("bbox", dict()))
+                bbox = None
 
             styledict = dict(
                 xytext=(20, 20),
                 textcoords="offset points",
                 bbox=bbox,
                 arrowprops=dict(arrowstyle="->"),
                 annotation_clip=True,
@@ -749,16 +754,17 @@
         layer = self.m.BM._get_showlayer_name(layer, transparent=True)
 
         ID, pos, val, ind, picker_name, val_color = self._popargs(kwargs)
 
         ax = self.m.ax
 
         # default boundary args
-        args = dict(fc="none", ec="k", lw=1.1)
-        args.update(kwargs)
+        kwargs.setdefault("fc", "none")
+        kwargs.setdefault("ec", "k")
+        kwargs.setdefault("lw", 1.1)
 
         if isinstance(how, str):
             # base transformations on transData to ensure correct treatment
             # for shared axes
             if how == "left":
                 x, _ = ax.transData.transform((pos[0], pos[1]))
                 x0, y0 = ax.transAxes.transform((0, 0))
@@ -855,15 +861,15 @@
             clip_path = self.m.cb.click.attach._get_clip_path(
                 x1m, y1m, "out", (w / 2, h / 2), "out", shape, 100
             )
         else:
             raise TypeError(f"EOmaps: {how} is not a valid peek method!")
 
         if clip_path is not None:
-            patch = PathPatch(clip_path, ec="k", fc="none")
+            patch = PathPatch(clip_path, **kwargs)
             marker = self.m.ax.add_patch(patch)
             self.m.cb.click.add_temporary_artist(marker)
 
             # make sure to clear the marker at the next update to avoid savefig issues
             def doit():
                 self.m.BM._artists_to_clear.setdefault("peek", []).append(marker)
                 self.m.BM._clear_temp_artists("peek")
@@ -985,15 +991,15 @@
         if hasattr(self, "picked_vals"):
             del self.picked_vals
 
     def _get_clip_path(self, x, y, xy_crs, radius, radius_crs, shape, n=100):
         shp = self.m.set_shape._get(shape)
 
         if shape == "ellipses":
-            shp_pts = shp._get_ellipse_points(
+            shp_pts = shp._get_points(
                 x=np.atleast_1d(x),
                 y=np.atleast_1d(y),
                 crs=xy_crs,
                 radius=radius,
                 radius_crs=radius_crs,
                 n=n,
             )
@@ -1007,15 +1013,15 @@
                 radius=radius,
                 radius_crs=radius_crs,
                 n=n,
             )
             bnd_verts = shp_pts[0][0]
 
         elif shape == "geod_circles":
-            shp_pts = shp._get_geod_circle_points(
+            shp_pts = shp._get_points(
                 x=np.atleast_1d(x),
                 y=np.atleast_1d(y),
                 crs=xy_crs,
                 radius=radius,
                 # radius_crs=radius_crs,
                 n=n,
             )
```

### Comparing `eomaps-8.0rc2/eomaps/cb_container.py` & `eomaps-8.1/eomaps/cb_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,15 @@
     def _add_callback(
         self,
         *args,
         callback=None,
         double_click=False,
         button=None,
         modifier=None,
+        on_motion=None,
         **kwargs,
     ):
         """
         Attach a callback to the plot that will be executed if a pixel is clicked.
 
         A list of pre-defined callbacks (accessible via `m.cb`) or customly defined
         functions can be used.
@@ -804,22 +805,24 @@
         modifier : str or None
             Define a keypress-modifier to execute the callback only if the
             corresponding key is pressed on the keyboard.
 
             - If None, the callback is executed if no modifier is activated.
 
             The default is None.
-        on_motion : bool
+        on_motion : bool or None, optional
             !! Only relevant for "click" callbacks !!
 
             - True: Continuously execute the callback if the mouse is moved while the
               assigned button is pressed.
             - False: Only execute the callback on clicks.
+            - None: use True for default callbacks that support on_motion and False
+              for all other callbacks (incl. custom callbacks)
 
-            The default is True.
+            The default is None.
         **kwargs :
             kwargs passed to the callback-function
             For documentation of the individual functions check the docs in `m.cb`
 
         Returns
         -------
         cbname : str
@@ -837,16 +840,14 @@
             else:
                 self._init_picker()
 
         cb_name = callback if isinstance(callback, str) else callback.__name__
         # attach "on_move" callbacks
         movecb_name = None
 
-        on_motion = kwargs.pop("on_motion", None)
-
         # set on_motion=True as default for "click" callbacks that
         # are also supported as move callbacks and False otherwise
         if self._method == "click" and on_motion is None:
             if hasattr(self._m.cb._click_move._attach, cb_name):
                 on_motion = True
             else:
                 on_motion = False
```

### Comparing `eomaps-8.0rc2/eomaps/colorbar.py` & `eomaps-8.1/eomaps/colorbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,19 @@
         extend_frac=0.025,
         tick_precision=2,
         margin=None,
         divider_linestyle=None,
         hist_size=0.9,
     ):
         self._parent_cb = None
-        self._hist_size_ = hist_size
+
+        if hist_size is None:
+            self._hist_size_ = 0
+        else:
+            self._hist_size_ = hist_size
 
         self._extend_frac = extend_frac
 
         self.orientation = orientation
 
         self._tick_precision = tick_precision
         self._margin = margin
@@ -100,14 +104,17 @@
         if self._parent_cb is None:
             return self._hist_size_
         else:
             return self._parent_cb._hist_size_
 
     @_hist_size.setter
     def _hist_size(self, size):
+        if size is None:
+            size = 0
+
         if self._parent_cb is None:
             self._hist_size_ = size
         else:
             self._hist_size_ = size
             self._parent_cb._hist_size_ = size
 
     def _get_data(self):
@@ -244,34 +251,48 @@
                     else:
                         self.ax_cb_plot.set_xlim(left=None, right=0, emit=False)
 
         self.ax_cb_plot.callbacks.connect("xlim_changed", xchanged)
         self.ax_cb_plot.callbacks.connect("ylim_changed", ychanged)
 
     def _hide_singular_axes(self):
-        sing_hist = self.ax_cb_plot.bbox.width <= 2 or self.ax_cb_plot.bbox.height <= 2
-        sing_cb = self.ax_cb.bbox.width <= 2 or self.ax_cb.bbox.height <= 2
+
+        sing_hist = (self.ax_cb_plot.bbox.width <= 2) or (
+            self.ax_cb_plot.bbox.height <= 2
+        )
+        sing_cb = (self.ax_cb.bbox.width <= 2) or (self.ax_cb.bbox.height <= 2)
+
+        # trigger a draw to update axes positions before checking singularity
+        # (ignore any errors in here to avoid any remaining issues with singular axes
+        # if hist-updates are triggered faster than draw-events...)
+        try:
+            self._m.f.canvas.draw()
+        except Exception:
+            pass
+
+        sing_hist = (self.ax_cb_plot.bbox.width <= 2) or (
+            self.ax_cb_plot.bbox.height <= 2
+        )
+        sing_cb = (self.ax_cb.bbox.width <= 2) or (self.ax_cb.bbox.height <= 2)
 
         if sing_hist:
             self.ax_cb_plot.set_visible(False)
         else:
             self.ax_cb_plot.set_visible(True)
 
         if sing_cb:
             self.ax_cb.set_visible(False)
         else:
             self.ax_cb.set_visible(True)
 
     def _set_hist_size(self, size=None, update_all=False):
-        if size is None:
-            size = self._hist_size
-        else:
+        if size is not None:
             self._hist_size = size
 
-        assert 0 <= size <= 1, "Histogram size must be between 0 and 1"
+        assert 0 <= self._hist_size <= 1, "Histogram size must be between 0 and 1"
 
         self._hide_singular_axes()
 
         if self._margin is None:
             if self.orientation == "horizontal":
                 self._margin = dict(left=0.1, right=0.1, bottom=0.3, top=0.0)
             else:
@@ -1429,16 +1450,17 @@
             The default is False.
         tick_precision : int or None
             The precision of the tick-labels in the colorbar.
             (e.g. a precision of 2 means that 0.12345 will be shown as 0.12)
             The default is 2.
         log : bool, optional
             Indicator if the y-axis of the plot should be logarithmic or not.
-            The default is False
+            The default is False.
         out_of_range_vals : str or None
+            Set how to treat histogram values outside the visible range of values.
 
             - if "mask": out-of range values will be masked.
               (e.g. values outside the colorbar limits are not represented in the
               histogram and NO extend-arrows are added)
             - if "clip": out-of-range values will be clipped.
               (e.g. values outside the colorbar limits will be represented in the
               min/max bins of the histogram)
```

### Comparing `eomaps-8.0rc2/eomaps/compass.py` & `eomaps-8.1/eomaps/compass.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/draw.py` & `eomaps-8.1/eomaps/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -696,15 +696,15 @@
             if len(pts) == 1:
                 x, y = event.xdata, event.ydata
                 if (x is None) or (y is None):
                     return
 
                 r = np.sqrt((x - pts[0][0]) ** 2 + (y - pts[0][1]) ** 2)
 
-                pts = Shapes._Ellipses(self._m)._get_ellipse_points(
+                pts = Shapes._Ellipses(self._m)._get_points(
                     np.array([pts[0][0]]),
                     np.array([pts[0][1]]),
                     "out",
                     [r, r],
                     "out",
                     100,
                 )
@@ -733,15 +733,15 @@
 
     def _circle(self, **kwargs):
         pts = self._clicks
         if pts is not None and len(pts) == 2:
             pts = np.asarray(pts)
 
             r = np.sqrt(sum((pts[1] - pts[0]) ** 2))
-            pts = Shapes._Ellipses(self._m)._get_ellipse_points(
+            pts = Shapes._Ellipses(self._m)._get_points(
                 np.array([pts[0][0]]), np.array([pts[0][1]]), "out", [r, r], "out", 100
             )
 
             with autoscale_turned_off(self._m.ax):
                 (ph,) = self._m.ax.fill(pts[0][0], pts[1][0], **kwargs)
 
                 if self._dynamic:
```

### Comparing `eomaps-8.0rc2/eomaps/eomaps.py` & `eomaps-8.1/eomaps/eomaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -2797,35 +2797,37 @@
             The default is None.
 
         Returns
         -------
         extent : The extent in the given crs (x0, x1, y0, y1).
 
         """
-        bnds = self._crs_boundary_bounds
 
         # fast track if plot-crs is requested
         if crs == self.crs_plot:
             x0, x1, y0, y1 = (*self.ax.get_xlim(), *self.ax.get_ylim())
+
+            bnds = self._crs_boundary_bounds
+            # clip the map-extent with respect to the boundary bounds
+            # (to avoid returning values outside the crs bounds)
+            try:
+                x0, x1 = np.clip([x0, x1], bnds[0], bnds[2])
+                y0, y1 = np.clip([y0, y1], bnds[1], bnds[3])
+            except Exception:
+                _log.debug(
+                    "EOmaps: Error while trying to clip map extent", exc_info=True
+                )
         else:
             if crs is not None:
                 crs = self._get_cartopy_crs(crs)
             else:
                 crs = self._get_cartopy_crs(4326)
 
             x0, x1, y0, y1 = self.ax.get_extent(crs=crs)
 
-        # clip the map-extent with respect to the boundary bounds
-        # (to avoid returning values outside the crs bounds)
-        try:
-            x0, x1 = np.clip([x0, x1], bnds[0], bnds[2])
-            y0, y1 = np.clip([y0, y1], bnds[1], bnds[3])
-        except Exception:
-            _log.debug("EOmaps: Error while trying to clip map extent", exc_info=True)
-
         return x0, x1, y0, y1
 
     def _calc_vmin_vmax(self, vmin=None, vmax=None):
         if self.data is None:
             return vmin, vmax
 
         calc_min, calc_max = vmin is None, vmax is None
@@ -3076,14 +3078,28 @@
         cbcmap, norm, bins, classified = self._classify_data(
             vmin=self._vmin,
             vmax=self._vmax,
             cmap=cmap,
             classify_specs=self.classify_specs,
         )
 
+        if norm is not None:
+            if "norm" in kwargs:
+                raise TypeError(
+                    "EOmaps: You cannot provide an explicit norm for the dataset if a "
+                    "classification scheme is used!"
+                )
+        else:
+            if "norm" in kwargs:
+                norm = kwargs.pop("norm")
+                norm.vmin = self._vmin
+                norm.vmax = self._vmax
+            else:
+                norm = plt.Normalize(vmin=self._vmin, vmax=self._vmax)
+
         # todo remove duplicate attributes
         self.classify_specs._cbcmap = cbcmap
         self.classify_specs._norm = norm
         self.classify_specs._bins = bins
         self.classify_specs._classified = classified
 
         self._cbcmap = cbcmap
@@ -4332,15 +4348,15 @@
             if cmap._rgba_under:
                 cbcmap.set_under(cmap._rgba_under)
 
         else:
             classified = False
             bins = None
             cbcmap = cmap
-            norm = mpl.colors.Normalize(vmin, vmax)
+            norm = None
 
         return cbcmap, norm, bins, classified
 
     def _set_parent(self):
         """Identify the parent object."""
         assert self._parent is None, "EOmaps: There is already a parent Maps object!"
         # check if the figure to which the Maps-object is added already has a parent
@@ -4553,15 +4569,15 @@
         **kwargs,
     ):
         _log.info(
             "EOmaps: Plotting "
             f"{self._data_manager.z_data.size} datapoints ({self.shape.name})"
         )
 
-        for key in ("array", "norm"):
+        for key in ("array",):
             assert (
                 key not in kwargs
             ), f"The key '{key}' is assigned internally by EOmaps!"
 
         try:
             self._set_extent = set_extent
 
@@ -4605,14 +4621,61 @@
             color = self._sel_c_transp(np.rec.fromarrays(color.T))
         else:
             # still use np.asanyarray in here in case lists are provided
             color = self._sel_c_transp(np.asanyarray(color).reshape(self._zshape))
 
         return color
 
+    @staticmethod
+    def _convert_1d_to_2d(data, x, y, fill_value=np.nan):
+        """A function to convert 1D vectors + data into 2D."""
+
+        if _log.getEffectiveLevel() <= logging.DEBUG:
+            _log.debug(
+                "EOmaps: Required conversion of 1D arrays to 2D for 'raster'"
+                "shape might be slow and consume a lot of memory!"
+            )
+
+        x, y, data = map(np.asanyarray, (x, y, data))
+        assert (
+            x.size == y.size == data.size
+        ), "EOmaps: You cannot use 1D arrays with different sizes for x, y and data"
+
+        x_vals, x_idx = np.unique(x, return_inverse=True)
+        y_vals, y_idx = np.unique(y, return_inverse=True)
+        # Get output array shape
+        m, n = (x_vals.size, y_vals.size)
+
+        # Get linear indices to be used as IDs with bincount
+        lidx = np.ravel_multi_index(np.vstack((x_idx, y_idx)), (m, n))
+        idx2d = np.unravel_index(lidx, (m, n))
+
+        # Distribute data to 2D
+
+        if not np.issubdtype(data.dtype, np.integer):
+            # Integer-dtypes do not support None!
+            data2d = np.full((m, n), fill_value=fill_value, dtype=data.dtype)
+            data2d[idx2d] = data
+
+        else:
+            # use smallest possible value as fill-value
+            fill_value = np.iinfo(data.dtype).min
+            data2d = np.full((m, n), fill_value=fill_value, dtype=data.dtype)
+            data2d[idx2d] = data
+
+            mask2d = np.full((m, n), fill_value=True, dtype=bool)
+            mask2d[idx2d] = False
+
+            data2d = np.ma.masked_array(data2d, mask2d)
+
+        # Distribute coordinates to 2D
+        x_vals, y_vals = np.meshgrid(x_vals, y_vals, indexing="ij")
+
+        return data2d, x_vals, y_vals
+
     def _get_coll(self, props, **kwargs):
         # handle selection of explicitly provided facecolors
         # (e.g. for rgb composites)
 
         # allow only one of the synonyms "color", "fc" and "facecolor"
         if (
             np.count_nonzero(
@@ -4647,42 +4710,25 @@
             coll = self.shape.get_coll(props["xorig"], props["yorig"], "in", **args)
         elif self.shape.name in ["raster"]:
             # if input-data is 1D, try to convert data to 2D (required for raster)
             # TODO make an explicit data-conversion function for 2D-only shapes
             if len(self._xshape) == 2 and len(self._yshape) == 2:
                 coll = self.shape.get_coll(props["xorig"], props["yorig"], "in", **args)
             else:
-                (pd,) = register_modules("pandas")
-                # TODO avoid having pandas as a dependency here
-                if pd:
-                    if (
-                        (len(self._xshape) == 1)
-                        and (len(self._yshape) == 1)
-                        and (len(self._zshape) == 1)
-                        and (props["x0"].size == props["y0"].size)
-                        and (props["x0"].size == props["z_data"].size)
-                    ):
-
-                        df = (
-                            pd.DataFrame(
-                                dict(
-                                    x=props["x0"].ravel(),
-                                    y=props["y0"].ravel(),
-                                    val=props["z_data"].ravel(),
-                                ),
-                                copy=False,
-                            ).set_index(["x", "y"])
-                        )["val"].unstack("y")
+                data2d, x2d, y2d = self._convert_1d_to_2d(
+                    data=props["z_data"].ravel(),
+                    x=props["x0"].ravel(),
+                    y=props["y0"].ravel(),
+                )
 
-                        xg, yg = np.meshgrid(df.index.values, df.columns.values)
+                if args["array"] is not None:
+                    args["array"] = data2d
 
-                        if args["array"] is not None:
-                            args["array"] = df.values.T
+                coll = self.shape.get_coll(x2d, y2d, "out", **args)
 
-                        coll = self.shape.get_coll(xg, yg, "out", **args)
         else:
             # convert to 1D for further processing
             if args["array"] is not None:
                 args["array"] = args["array"].ravel()
 
             coll = self.shape.get_coll(
                 props["x0"].ravel(), props["y0"].ravel(), "out", **args
@@ -5017,15 +5063,20 @@
         # method defined...)
         layers = layers.union(set(self.BM._on_layer_activation[True]))
         layers = layers.union(set(self.BM._on_layer_activation[False]))
 
         # add all (possibly still invisible) layers with artists defined
         # (ONLY do this for unique layers... skip multi-layers )
         layers = layers.union(
-            chain(*(self.BM._parse_multi_layer_str(i)[0] for i in self.BM._bg_artists))
+            chain(
+                *(
+                    self.BM._parse_multi_layer_str(i)[0]
+                    for i in (*self.BM._bg_artists, *self.BM._artists)
+                )
+            )
         )
 
         # exclude private layers
         if exclude_private:
             # for python <3.9 compatibility
             def remove_prefix(text, prefix):
                 if text.startswith(prefix):
```

### Comparing `eomaps-8.0rc2/eomaps/grid.py` & `eomaps-8.1/eomaps/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,17 +232,16 @@
                 raise TypeError(
                     "EOmaps: If you provide a tuple as grid-spacing "
                     "'d=(dlon, dlat)' it must contain 2 items!"
                 )
         elif isinstance(d, (int, float, np.number)):
             dlon = dlat = d
         elif isinstance(d, (list, np.ndarray)):
-            d = np.asanyarray(d)
-            if len(d.shape) == 2:
-                lons, lats = np.asanyarray(d)
+            if len(d) == 2:
+                lons, lats = np.asanyarray(d[0]), np.asanyarray(d[1])
             else:
                 lons = lats = np.asanyarray(d)
         else:
             raise TypeError(f"EOmaps: d={d} is not a valid grid-spacing.")
 
         # evaluate line positions if no explicit positions are provided
         if lons is None:
@@ -688,14 +687,15 @@
 
     def _get_spine_intersections(self, lines, axis=None):
 
         m = self._g.m
 
         # get boundary vertices of current axis spine (in figure coordinates)
         bl = self._get_bound_verts()
+        bndmin, bndmax = bl.min(axis=0), bl.max(axis=0)
 
         # get gridlines
         uselines = np.array(lines[axis])
 
         if len(uselines) == 0:
             return
 
@@ -770,33 +770,36 @@
                 # TODO find a better way to identify position of label
                 # select which lines to draw (e.g. tblr)
                 if self._where != "all":
                     if axis == 0:
                         if xt > 0.99 or xt < 0.01:
                             continue
 
-                        if "t" in self._where:
-                            if "b" not in self._where:
-                                # don't draw the second intersection point
-                                if yt <= 0.5:
-                                    continue
-                        elif "b" in self._where:
-                            if yt > 0.5:
+                        line_in_bnds = l[:, 1].clip(bndmin[1], bndmax[1])
+                        line_center = (line_in_bnds.min() + line_in_bnds.max()) / 2
+                        top = y > line_center
+                        if top:
+                            if not ("t" in self._where):
+                                continue
+                        else:
+                            if not ("b" in self._where):
                                 continue
                     else:
                         if yt > 0.99 or yt < 0.01:
                             continue
 
-                        if "r" in self._where:
-                            if "l" not in self._where:
-                                # don't draw the second intersection point
-                                if xt <= 0.5:
-                                    continue
-                        elif "l" in self._where:
-                            if xt > 0.5:
+                        line_in_bnds = l[:, 0].clip(bndmin[0], bndmax[0])
+                        line_center = (line_in_bnds.min() + line_in_bnds.max()) / 2
+
+                        right = x > line_center
+                        if right:
+                            if not ("r" in self._where):
+                                continue
+                        else:
+                            if not ("l" in self._where):
                                 continue
 
                 # calculate rotation angle of boundary segment
                 r = np.pi + np.arctan2(
                     (ba[1] - bb[1]),
                     (ba[0] - bb[0]),
                 )
```

### Comparing `eomaps-8.0rc2/eomaps/helpers.py` & `eomaps-8.1/eomaps/helpers.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/inset_maps.py` & `eomaps-8.1/eomaps/inset_maps.py`

 * *Files 5% similar despite different names*

```diff
@@ -344,26 +344,32 @@
             verts_t = np.column_stack(
                 m._transf_lonlat_to_plot.transform(*spine_verts.T)
             )
             verts_t = (m.ax.transData + m.f.transFigure.inverted()).transform(verts_t)
             p_map = verts_t.mean(axis=0)
 
             p_inset = verts.mean(axis=0)
-            # find intersection points of lines connecting the centers
+            # find the first intersection point of lines connecting the centers
             # 1) with the inset-map boundary
-            q = _intersect(p_map, p_inset, verts[:-1], verts[1:])
-            if q.any():
-                x0, y0 = _get_intersect(p_map, p_inset, verts[:-1][q], verts[1:][q])
+            q = np.nonzero(_intersect(p_map, p_inset, verts[:-1], verts[1:]))[0]
+
+            if len(q) > 0:
+                x0, y0 = _get_intersect(
+                    p_map, p_inset, verts[:-1][q[0]], verts[1:][q[0]]
+                )
             else:
                 x0, y0 = p_inset
 
             # 2) with the inset-map indicator on the map
-            q = _intersect(p_map, p_inset, verts_t[:-1], verts_t[1:])
-            if q.any():
-                x1, y1 = _get_intersect(p_map, p_inset, verts_t[:-1][q], verts_t[1:][q])
+            q = np.nonzero(_intersect(p_map, p_inset, verts_t[:-1], verts_t[1:]))[0]
+            if len(q) > 0:
+                x1, y1 = _get_intersect(
+                    p_map, p_inset, verts_t[:-1][q[0]], verts_t[1:][q[0]]
+                )
+
                 # update indicator line vertices
                 l.set_xdata([x0, x1])
                 l.set_ydata([y0, y1])
                 continue
 
     # a convenience-method to set the position based on the center of the axis
     def set_inset_position(self, x=None, y=None, size=None):
@@ -421,15 +427,15 @@
 
     def _get_inset_boundary(self, x, y, xy_crs, radius, radius_crs, shape, n=100):
         # get the inset-shape boundary
 
         shp = self.set_shape._get(shape)
 
         if shape == "ellipses":
-            shp_pts = shp._get_ellipse_points(
+            shp_pts = shp._get_points(
                 x=np.atleast_1d(x),
                 y=np.atleast_1d(y),
                 crs=xy_crs,
                 radius=radius,
                 radius_crs=radius_crs,
                 n=n,
             )
@@ -446,20 +452,19 @@
                 radius=radius,
                 radius_crs=radius_crs,
                 n=n,
             )
             bnd_verts = shp_pts[0][0]
 
         elif shape == "geod_circles":
-            shp_pts = shp._get_geod_circle_points(
+            shp_pts = shp._get_points(
                 x=np.atleast_1d(x),
                 y=np.atleast_1d(y),
                 crs=xy_crs,
                 radius=radius,
-                # radius_crs=radius_crs,
                 n=n,
             )
             bnd_verts = np.stack(shp_pts[:2], axis=2).squeeze()
             # make sure vertices are right-handed
             bnd_verts = bnd_verts[::-1]
 
         boundary = Path(bnd_verts)
```

### Comparing `eomaps-8.0rc2/eomaps/layout_editor.py` & `eomaps-8.1/eomaps/layout_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -600,14 +600,18 @@
                 for key in ["pan", "zoom"]:
                     val = toolbar._actions.get(key, None)
                     if val is not None and val.isCheckable() and val.isChecked():
                         val.trigger()
         except AttributeError:
             pass
 
+        # capture scroll events in ipympl backend (e.g. Jupyter Notebooks)
+        self._init_capture_scroll = getattr(self.m.f.canvas, "capture_scroll", False)
+        self.m.f.canvas.capture_scroll = True
+
         self._filepath = filepath
         self.modifier_pressed = True
         _log.info(
             "EOmaps: Layout Editor activated! (press 'esc' to exit " "and 'q' for info)"
         )
 
         self._history.clear()
@@ -719,14 +723,18 @@
             self._info_text.remove()
             # set to None to avoid crating the info-text again
             self._info_text = None
 
         self._history.clear()
         self._history_undone.clear()
 
+        # Reset capturing scroll events to the value before activating the editor
+        # (only relevant for ipympl backend... e.g. Jupyter Notebooks)
+        self.m.f.canvas.capture_scroll = getattr(self, "_init_capture_scroll", False)
+
         toolbar = getattr(self.m.f, "toolbar", None)
         if toolbar is not None:
             # Reset the axes stack to make sure the "home" "back" and "forward" buttons
             # of the toolbar do not reset axis positions
             # see "matplotlib.backend_bases.NavigationToolbar2.update"
             if hasattr(toolbar, "update"):
                 try:
```

### Comparing `eomaps-8.0rc2/eomaps/logo.png` & `eomaps-8.1/eomaps/logo.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/mapsgrid.py` & `eomaps-8.1/eomaps/mapsgrid.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/ne_features.py` & `eomaps-8.1/eomaps/ne_features.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/projections.py` & `eomaps-8.1/eomaps/projections.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/app.py` & `eomaps-8.1/eomaps/qtcompanion/app.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/base.py` & `eomaps-8.1/eomaps/qtcompanion/base.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/edit_layout.png` & `eomaps-8.1/eomaps/qtcompanion/icons/edit_layout.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/edit_layout_active.png` & `eomaps-8.1/eomaps/qtcompanion/icons/edit_layout_active.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/edit_layout_hover.png` & `eomaps-8.1/eomaps/qtcompanion/icons/edit_layout_hover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/eye_closed.png` & `eomaps-8.1/eomaps/qtcompanion/icons/eye_closed.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/eye_open.png` & `eomaps-8.1/eomaps/qtcompanion/icons/eye_open.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/info.png` & `eomaps-8.1/eomaps/qtcompanion/icons/info.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/info_checked.png` & `eomaps-8.1/eomaps/qtcompanion/icons/info_checked.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/info_hoover.png` & `eomaps-8.1/eomaps/qtcompanion/icons/info_hoover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/layers.png` & `eomaps-8.1/eomaps/qtcompanion/icons/layers.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/layers_hover.png` & `eomaps-8.1/eomaps/qtcompanion/icons/layers_hover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/logo.png` & `eomaps-8.1/eomaps/qtcompanion/icons/logo.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/open.png` & `eomaps-8.1/eomaps/qtcompanion/icons/open.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/open_hover.png` & `eomaps-8.1/eomaps/qtcompanion/icons/open_hover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_circle.png` & `eomaps-8.1/eomaps/qtcompanion/icons/peek_circle.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_circle_active.png` & `eomaps-8.1/eomaps/qtcompanion/icons/peek_circle_active.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_ellipse.png` & `eomaps-8.1/eomaps/qtcompanion/icons/peek_ellipse.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/peek_ellipse_active.png` & `eomaps-8.1/eomaps/qtcompanion/icons/peek_ellipse_active.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/plus.png` & `eomaps-8.1/eomaps/qtcompanion/icons/plus.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/icons/plus_hoover.png` & `eomaps-8.1/eomaps/qtcompanion/icons/plus_hoover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/qtcompanion/signal_container.py` & `eomaps-8.1/eomaps/qtcompanion/signal_container.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/reader.py` & `eomaps-8.1/eomaps/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,25 +269,14 @@
             )
 
             # only use masked arrays if mask_and_scale is False!
             # (otherwise the mask is already applied as NaN's in the float-array)
             # Using masked-arrays ensures that we can deal with integers as well!
             if mask_and_scale is False:
                 encoding = usencfile.attrs
-                fill_value = encoding.get("_FillValue", None)
-
-                if fill_value and fill_values == "mask":
-                    data = np.ma.MaskedArray(
-                        data=data,
-                        mask=data == fill_value,
-                        copy=False,
-                        fill_value=fill_value,
-                        hard_mask=True,
-                    )
-
             else:
                 encoding = None
 
             if set_data is not None:
                 set_data.set_data(
                     data=data,
                     x=x,
@@ -551,24 +540,14 @@
             # Using masked-arrays ensures that we can deal with integers as well!
             if mask_and_scale is False:
                 encoding = dict(
                     scale_factor=getattr(usencfile[parameter], "scale_factor", 1),
                     add_offset=getattr(usencfile[parameter], "add_offset", 0),
                     _FillValue=getattr(usencfile[parameter], "_FillValue", None),
                 )
-                fill_value = encoding.get("_FillValue", None)
-                if fill_value and fill_values == "mask":
-                    data = np.ma.MaskedArray(
-                        data=data,
-                        mask=data == fill_value,
-                        copy=False,
-                        fill_value=fill_value,
-                        hard_mask=True,
-                    )
-
             else:
                 encoding = None
 
             if set_data is not None:
                 set_data.set_data(
                     data=data,
                     x=x.values,
```

### Comparing `eomaps-8.0rc2/eomaps/scalebar.py` & `eomaps-8.1/eomaps/scalebar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1181,15 +1181,15 @@
             patch = PathPatch(tp, color=self._label_props["color"], lw=0, zorder=1)
             patch.set_transform(
                 Affine2D().rotate_around(
                     *xy, ang + np.pi / 2 + np.deg2rad(self._label_props["rotation"])
                 )
                 + self._m.ax.transData
             )
-
+            patch.set_clip_on(False)
             self._artists[f"text_{i}"] = self._m.ax.add_artist(patch)
             self._texts[f"text_{i}"] = txt
             self._m.BM.add_artist(self._artists[f"text_{i}"], layer=self._layer)
 
     def _redraw_minitxt(self):
         # re-draw the text patches in case the number of texts changed
 
@@ -1329,14 +1329,20 @@
         # update scalebar props whenever new backgrounds are fetched
         # (e.g. to take care of updates on pan/zoom/resize)
         self._m.BM._before_fetch_bg_actions.append(self._update)
 
         if pickable is True:
             self._make_pickable()
 
+        # make sure scalebar-artists are not clipped with respect
+        # to the spine of the axes
+        for _, a in self._artists.items():
+            if a is not None:
+                a.set_clip_on(False)
+
     def _get_scale_color_names(self):
         colors = []
         for i in self._scale_props["colors"]:
             if isinstance(i, tuple):
                 colors.append(to_hex(i, keep_alpha=True))
             else:
                 colors.append(i)
@@ -1409,18 +1415,24 @@
             # if self._auto_position is False:
             #     print("The position of this scalebar is fixed!")
             #     return
 
             self._pick_drag = True
             # get the offset_position of the click with respect to the
             # reference point of the scalebar
-            lon0, lat0 = self._m._transf_plot_to_lonlat.transform(
-                event.xdata, event.ydata
-            )
-            self._pick_start_offset = self._lon - lon0, self._lat - lat0
+            xdata, ydata = event.xdata, event.ydata
+            if xdata is not None and ydata is not None:
+                lon0, lat0 = self._m._transf_plot_to_lonlat.transform(
+                    event.xdata, event.ydata
+                )
+                self._pick_start_offset = self._lon - lon0, self._lat - lat0
+            else:
+                # None event coordinates happen if you click outside
+                # the axes-spine
+                self._pick_start_offset = 0, 0
 
         elif event.button in ["up", "down"]:
             # pass scroll events that happen on top of the scalebar
             # (they are handled explicitly in "cb_scroll" )
             pass
         elif self._picked:
             self._unpick()
```

### Comparing `eomaps-8.0rc2/eomaps/scripts/open.py` & `eomaps-8.1/eomaps/scripts/open.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/shapes.py` & `eomaps-8.1/eomaps/shapes.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,244 @@
 import numpy as np
 
 from .helpers import register_modules
 
 _log = logging.getLogger(__name__)
 
 
+# a base class for shapes that support setting the number of intermediate points
+class _ShapeBase:
+    name = "none"
+
+    def __init__(self, m):
+        self._m = m
+        self._n = None
+
+        self._select_radius = True
+
+    def _get_auto_n(self):
+        s = self._m._data_manager._get_current_datasize()
+
+        if self.name == "rectangles":
+            # mesh currently only supports n=1
+            if self.mesh is True:
+                return 1
+
+            # if plot crs is same as input-crs there is no need for
+            # intermediate points since the rectangles are not curved!
+            if self._m._crs_plot == self._m.data_specs.crs:
+                return 1
+
+        if s < 10:
+            n = 100
+        elif s < 100:
+            n = 75
+        elif s < 1000:
+            n = 50
+        elif s < 10000:
+            n = 20
+        else:
+            n = 12
+
+        return n
+
+    @property
+    def n(self):
+        if self._n is None:
+            return self._get_auto_n()
+        else:
+            return self._n
+
+    @n.setter
+    def n(self, val):
+        if self.name == "rectangles" and self.mesh is True:
+            if val is not None and val != 1:
+                _log.info("EOmaps: rectangles with 'mesh=True' only support n=1")
+            self._n = 1
+        else:
+            self._n = val
+
+    @property
+    def _selected_radius(self):
+        # option to override radius-selection in case the shape is used
+        # to create markers (e.g. call is independent of plot-extent)
+        if self._select_radius is False:
+            return self.radius
+
+        # if radius was provided as a array (for individual shape radius)
+        # select values according to the dat-manager query to get values
+        # of visible points
+
+        # if no data is assigned, just return the radius
+        if not self._m._data_manager._current_data:
+            return self.radius
+
+        # check if multiple individual x-y radius was provided
+        q1 = isinstance(self.radius, tuple) and isinstance(self.radius[0], np.ndarray)
+        # chedk if multiple radius values were provided
+        q2 = isinstance(self.radius, np.ndarray)
+
+        if q1 or q2:
+            mask = self._m._data_manager._get_q()[0]
+
+            # quick exit if full data is in extent
+            if mask is True:
+                return self.radius
+
+        if q1:
+            radius = (self.radius[0][mask], self.radius[1][mask])
+        elif q2:
+            radius = self.radius[mask]
+        else:
+            radius = self.radius
+
+        return radius
+
+    def _wraparound(self, x, y, xs, ys, crs):
+        # ------------------------- implement some kind of "wraparound"
+        if self._m._crs_plot in (
+            self._m.CRS.Orthographic(),
+            self._m.CRS.Geostationary(),
+            self._m.CRS.NearsidePerspective(),
+        ):
+            # avoid masking in those crs
+            mask = np.full(xs.shape[0], True)
+        else:
+
+            # check if any points are in different halfspaces with respect to x
+            # and if so, mask the ones in the wrong halfspace
+            # (required for proper longitude wrapping)
+            # TODO this might be a lot easier (and faster) to implement!
+
+            xc = 0  # the center-point (e.g. (-180 + 180)/2 = 0 )
+
+            def getQ(x, xc):
+                quadrants = np.full_like(x, -1)
+
+                quadrant = x < xc
+                quadrants[quadrant] = 0
+                quadrant = x > xc
+                quadrants[quadrant] = 1
+
+                return quadrants
+
+            t_in_lonlat = self._m._get_transformer(crs, 4326)
+            t_plot_lonlat = self._m._get_transformer(self._m.crs_plot, 4326)
+
+            # transform the coordinates to lon/lat
+            xp, _ = t_in_lonlat.transform(x, y)
+            xsp, _ = t_plot_lonlat.transform(xs, ys)
+
+            quadrants, pts_quadrants = getQ(xp, xc), getQ(xsp, xc)
+
+            # mask any point that is in a different quadrant than the center point
+            maskx = pts_quadrants != quadrants[:, np.newaxis]
+            # take care of points that are on the center line (e.g. don't mask them)
+            # (use a +- 25 degree around 0 as threshold)
+            cpoints = np.broadcast_to(
+                np.isclose(xp, xc, atol=25)[:, np.newaxis], xs.shape
+            )
+
+            maskx[cpoints] = False
+            xs.mask[maskx] = True
+            ys.mask = xs.mask
+
+            # mask any datapoint that has less than 3 of the ellipse-points unmasked
+            mask = np.count_nonzero(~xs.mask, axis=1) >= 3
+
+        return xs, ys, mask
+
+
+class _CircularShapeBase(_ShapeBase):
+    name = "circular_shape_base"
+    radius_crs = None
+
+    def __init__(self, m):
+        super().__init__(m=m)
+
+    def __call__(self, radius=None, n=None, radius_crs=None):
+        if radius is None:
+            raise TypeError(
+                f"EOmaps: If 'm.set_shape.{self.name}(...)' is used, "
+                "you must provide a radius!"
+            )
+
+        from . import MapsGrid  # do this here to avoid circular imports!
+
+        for m in self._m if isinstance(self._m, MapsGrid) else [self._m]:
+            shape = self.__class__(m)
+            shape.radius = radius
+            shape.radius_crs = radius_crs
+            shape.n = n
+
+            m._shape = shape
+
+    @property
+    def _initargs(self):
+        return dict(radius=self._radius, radius_crs=self.radius_crs, n=self._n)
+
+    @property
+    def radius(self):
+        return self._radius
+
+    @radius.setter
+    def radius(self, val):
+        # string is required to accept "estimate" as radius
+        # tuple is required to provide (rx, ry) explicitly
+        if isinstance(val, (int, float, str, tuple, np.number)):
+            self._radius = val
+        else:
+            self._radius = np.asanyarray(np.atleast_1d(val)).ravel()
+
+    def __repr__(self):
+        try:
+            s = f"{self.name}(radius={self.radius}, n={self.n})"
+        except AttributeError:
+            s = f"{self.name}(radius, n)"
+        except Exception:
+            s = object.__repr__(self)
+
+        return s
+
+    def _get_points(self, x, y, crs, radius, n=20):
+        raise NotImplementedError("get_points is not implemented")
+        xs, ys, mask = [], [], []
+        return xs, ys, mask
+
+    def get_coll(self, x, y, crs, **kwargs):
+        xs, ys, mask = self._get_points(
+            x=x,
+            y=y,
+            crs=crs,
+            radius=self._selected_radius,
+            radius_crs=self.radius_crs,
+            n=self.n,
+        )
+        # compress the coordinates (masked arrays produce artefacts on the boundary
+        # in case intermediate points are masked)
+        verts = (
+            np.column_stack((x.compressed(), y.compressed()))
+            for i, (x, y) in enumerate(zip(xs, ys))
+            if mask[i]
+        )
+        # remember masked points
+        self._m._data_mask = mask
+
+        color_and_array = Shapes._get_colors_and_array(kwargs, mask)
+
+        coll = PolyCollection(
+            verts,
+            # transOffset=self._m.ax.transData,
+            **color_and_array,
+            **kwargs,
+        )
+
+        return coll
+
+
 class _CollectionAccessor:
     """
     Accessor class to handle contours drawn by plt.contour.
 
     The main purpose of this class is to serve as a single Artist-like container
     that executes relevant functions on ALL collections returned by plt.contour.
 
@@ -357,105 +587,15 @@
 
         if len(color_vals) == 0:
             return {"array": array}
         else:
             color_vals["array"] = None
             return color_vals
 
-    # a base class for shapes that support setting the number of intermediate points
-    class _ShapeBase:
-        name = "none"
-
-        def __init__(self, m):
-            self._m = m
-            self._n = None
-
-            self._select_radius = True
-
-        def _get_auto_n(self):
-            s = self._m._data_manager._get_current_datasize()
-
-            if self.name == "rectangles":
-                # mesh currently only supports n=1
-                if self.mesh is True:
-                    return 1
-
-                # if plot crs is same as input-crs there is no need for
-                # intermediate points since the rectangles are not curved!
-                if self._m._crs_plot == self._m.data_specs.crs:
-                    return 1
-
-            if s < 10:
-                n = 100
-            elif s < 100:
-                n = 75
-            elif s < 1000:
-                n = 50
-            elif s < 10000:
-                n = 20
-            else:
-                n = 12
-
-            return n
-
-        @property
-        def n(self):
-            if self._n is None:
-                return self._get_auto_n()
-            else:
-                return self._n
-
-        @n.setter
-        def n(self, val):
-            if self.name == "rectangles" and self.mesh is True:
-                if val is not None and val != 1:
-                    _log.info("EOmaps: rectangles with 'mesh=True' only support n=1")
-                self._n = 1
-            else:
-                self._n = val
-
-        @property
-        def _selected_radius(self):
-            # option to override radius-selection in case the shape is used
-            # to create markers (e.g. call is independent of plot-extent)
-            if self._select_radius is False:
-                return self.radius
-
-            # if radius was provided as a array (for individual shape radius)
-            # select values according to the dat-manager query to get values
-            # of visible points
-
-            # if no data is assigned, just return the radius
-            if not self._m._data_manager._current_data:
-                return self.radius
-
-            # check if multiple individual x-y radius was provided
-            q1 = isinstance(self.radius, tuple) and isinstance(
-                self.radius[0], np.ndarray
-            )
-            # chedk if multiple radius values were provided
-            q2 = isinstance(self.radius, np.ndarray)
-
-            if q1 or q2:
-                mask = self._m._data_manager._get_q()[0]
-
-                # quick exit if full data is in extent
-                if mask is True:
-                    return self.radius
-
-            if q1:
-                radius = (self.radius[0][mask], self.radius[1][mask])
-            elif q2:
-                radius = self.radius[mask]
-            else:
-                radius = self.radius
-
-            return radius
-
-    class _GeodCircles(_ShapeBase):
+    class _GeodCircles(_CircularShapeBase):
         name = "geod_circles"
 
         def __init__(self, m):
             super().__init__(m=m)
 
         def __call__(self, radius=None, n=None):
             """
@@ -475,54 +615,15 @@
 
             Returns
             -------
             self
                 The class representing the plot-shape.
 
             """
-            if radius is None:
-                raise TypeError(
-                    "EOmaps: If 'm.set_shape.geod_circles(...)' is used, "
-                    "you must provide a radius!"
-                )
-
-            from . import MapsGrid  # do this here to avoid circular imports!
-
-            for m in self._m if isinstance(self._m, MapsGrid) else [self._m]:
-                shape = self.__class__(m)
-                shape.radius = radius
-                shape.n = n
-
-                m._shape = shape
-
-        @property
-        def _initargs(self):
-            return dict(radius=self._radius, n=self._n)
-
-        @property
-        def radius(self):
-            return self._radius
-
-        @radius.setter
-        def radius(self, val):
-            if isinstance(val, (int, float, np.number)):
-                self._radius = val
-            else:
-                self._radius = np.asanyarray(np.atleast_1d(val))
-
-        @property
-        def radius_crs(self):
-            return "geod"
-
-        def __repr__(self):
-            try:
-                s = f"geod_circles(radius={self.radius}, n={self.n})"
-            except AttributeError:
-                s = "geod_circles(radius, n)"
-            return s
+            super().__call__(radius=radius, n=n, radius_crs="geod")
 
         def _calc_geod_circle_points(self, lon, lat, radius, n=20, start_angle=0):
             """
             Calculate points on a geodetic circle with a given radius.
 
             Parameters
             ----------
@@ -563,90 +664,42 @@
                 az=np.linspace(
                     [start_angle] * size, [360 - start_angle] * size, n, axis=1
                 ),
                 dist=radius,
                 radians=False,
             )
 
-            return lons.T, lats.T
+            return lons, lats
 
-        def _get_geod_circle_points(self, x, y, crs, radius, n=20):
+        def _get_points(self, x, y, crs, radius, radius_crs="geod", n=20):
+            crs = self._m.get_crs(crs)
             x, y = np.asarray(x), np.asarray(y)
 
             # transform from in-crs to lon/lat
             radius_t = self._m._get_transformer(
-                self._m.get_crs(crs),
+                crs,
                 self._m.CRS.PlateCarree(globe=self._m.crs_plot.globe),
             )
             # transform from lon/lat to the plot_crs
             plot_t = self._m._get_transformer(
                 self._m.CRS.PlateCarree(globe=self._m.crs_plot.globe),
                 CRS.from_user_input(self._m.crs_plot),
             )
 
             lon, lat = radius_t.transform(x, y)
             # calculate some points on the geodesic circle
             lons, lats = self._calc_geod_circle_points(lon, lat, radius, n=n)
 
             xs, ys = np.ma.masked_invalid(plot_t.transform(lons, lats), copy=False)
 
-            if self._m._crs_plot in (
-                self._m.CRS.Orthographic(),
-                self._m.CRS.Geostationary(),
-                self._m.CRS.NearsidePerspective(),
-            ):
-                mask = np.full(lons.shape, True)
-            else:
-                # get the mask for invalid, very distorted or very large shapes
-                dx = xs.max(axis=0) - xs.min(axis=0)
-                dy = ys.max(axis=0) - ys.min(axis=0)
-                mask = (
-                    ~xs.mask.any(axis=0)
-                    & ~ys.mask.any(axis=0)
-                    & ((dx / dy) < 10)
-                    & (dx < np.max(radius) * 50)
-                    & (dy < np.max(radius) * 50)
-                )
-
-                mask = np.broadcast_to(mask[:, None].T, lons.shape)
+            xs, ys, mask = self._wraparound(x, y, xs, ys, crs)
 
             return xs, ys, mask
 
-        def get_coll(self, x, y, crs, **kwargs):
-            xs, ys, mask = self._get_geod_circle_points(
-                x, y, crs, self._selected_radius, self.n
-            )
-
-            # only plot polygons if they contain 2 or more vertices
-            vertmask = np.count_nonzero(mask, axis=0) > 2
-
-            # remember masked points
-            self._m._data_mask = vertmask
-
-            verts = np.stack((xs, ys)).T
-            verts = np.ma.masked_array(
-                verts,
-                np.broadcast_to(~mask[:, None].T.swapaxes(1, 2), verts.shape),
-            )
-            verts = list(
-                i.compressed().reshape(-1, 2) for i, m in zip(verts, vertmask) if m
-            )
-
-            color_and_array = Shapes._get_colors_and_array(kwargs, vertmask)
-
-            coll = PolyCollection(
-                verts,
-                # transOffset=self._m.ax.transData,
-                **color_and_array,
-                **kwargs,
-            )
-
-            return coll
-
-    class _Ellipses(_ShapeBase):
+    class _Ellipses(_CircularShapeBase):
         name = "ellipses"
 
         def __init__(self, m):
             super().__init__(m=m)
 
         def __call__(self, radius="estimate", radius_crs="in", n=None):
             """
@@ -665,51 +718,21 @@
                 The crs in which the dimensions are defined.
                 The default is "in".
             n : int or None
                 The number of intermediate points to calculate on the circle.
                 If None, 100 is used for < 10k pixels and 20 otherwise.
                 The default is None.
             """
-            from . import MapsGrid  # do this here to avoid circular imports!
+            super().__call__(radius=radius, n=n, radius_crs=radius_crs)
 
-            for m in self._m if isinstance(self._m, MapsGrid) else [self._m]:
-                shape = self.__class__(m)
-
-                shape._radius = radius
-                shape.radius_crs = radius_crs
-                shape.n = n
-
-                m._shape = shape
-
-        @property
-        def _initargs(self):
-            return dict(radius=self._radius, radius_crs=self.radius_crs, n=self._n)
-
-        @property
+        @_CircularShapeBase.radius.getter
         def radius(self):
             radius = Shapes._get_radius(self._m, self._radius, self.radius_crs)
             return radius
 
-        @radius.setter
-        def radius(self, val):
-            if isinstance(val, (list, np.ndarray)):
-                self._radius = np.asanyarray(val).ravel()
-            else:
-                self._radius = val
-
-        def __repr__(self):
-            try:
-                try:
-                    s = f"ellipses(radius={self.radius}, radius_crs={self.radius_crs}, n={self.n})"
-                except AttributeError:
-                    s = "ellipses(radius, radius_crs, n)"
-                return s
-            except:
-                return object.__repr__(self)
-
         def _calc_ellipse_points(self, x0, y0, a, b, theta, n, start_angle=0):
             """
             Calculate points on a rotated ellipse.
 
             Parameters
             ----------
             x0, y0 : array-like
@@ -745,15 +768,15 @@
                 x0 + a * np.cos(angs) * np.cos(theta) - b * np.sin(angs) * np.sin(theta)
             )
             ys = (
                 y0 + a * np.cos(angs) * np.sin(theta) + b * np.sin(angs) * np.cos(theta)
             )
             return (xs, ys)
 
-        def _get_ellipse_points(self, x, y, crs, radius, radius_crs="in", n=20):
+        def _get_points(self, x, y, crs, radius, radius_crs="in", n=20):
             crs = self._m.get_crs(crs)
             radius_crs = self._m.get_crs(radius_crs)
             # transform from crs to the plot_crs
             t_in_plot = self._m._get_transformer(crs, self._m.crs_plot)
             # transform from crs to the radius_crs
             t_in_radius = self._m._get_transformer(crs, radius_crs)
             # transform from crs to the radius_crs
@@ -763,122 +786,44 @@
                 rx, ry = radius, radius
             else:
                 rx, ry = radius
 
             # transform corner-points
             if radius_crs == crs:
                 p = (x, y)
-                theta = np.full_like(x, 0)
                 xs, ys = self._calc_ellipse_points(
                     p[0],
                     p[1],
                     np.broadcast_to(rx, x.shape).astype(float),
                     np.broadcast_to(ry, y.shape).astype(float),
                     np.full_like(x, 0),
                     n=n,
                 )
                 xs, ys = np.ma.masked_invalid((xs, ys), copy=False)
                 xs, ys = np.ma.masked_invalid(t_in_plot.transform(xs, ys), copy=False)
             else:
                 p = t_in_radius.transform(x, y)
-                theta = np.full_like(x, 0)
                 xs, ys = self._calc_ellipse_points(
                     p[0],
                     p[1],
                     np.broadcast_to(rx, x.shape).astype(float),
                     np.broadcast_to(ry, y.shape).astype(float),
                     np.full_like(x, 0),
                     n=n,
                 )
 
                 xs, ys = np.ma.masked_invalid((xs, ys), copy=False)
                 xs, ys = np.ma.masked_invalid(
                     t_radius_plot.transform(xs, ys), copy=False
                 )
 
-            # ------------------------- implement some kind of "wraparound"
-            if self._m._crs_plot in (
-                self._m.CRS.Orthographic(),
-                self._m.CRS.Geostationary(),
-                self._m.CRS.NearsidePerspective(),
-            ):
-                # avoid masking in those crs
-                mask = np.full(xs.shape[0], True)
-            else:
-
-                # check if any points are in different halfspaces with respect to x
-                # and if so, mask the ones in the wrong halfspace
-                # (required for proper longitude wrapping)
-                # TODO this might be a lot easier (and faster) to implement!
-
-                xc = 0  # the center-point (e.g. (-180 + 180)/2 = 0 )
-
-                def getQ(x, xc):
-                    quadrants = np.full_like(x, -1)
-
-                    quadrant = x < xc
-                    quadrants[quadrant] = 0
-                    quadrant = x > xc
-                    quadrants[quadrant] = 1
-
-                    return quadrants
-
-                t_in_lonlat = self._m._get_transformer(crs, 4326)
-                t_plot_lonlat = self._m._get_transformer(self._m.crs_plot, 4326)
-
-                # transform the coordinates to lon/lat
-                xp, _ = t_in_lonlat.transform(x, y)
-                xsp, _ = t_plot_lonlat.transform(xs, ys)
-
-                quadrants, pts_quadrants = getQ(xp, xc), getQ(xsp, xc)
-
-                # mask any point that is in a different quadrant than the center point
-                maskx = pts_quadrants != quadrants[:, np.newaxis]
-                # take care of points that are on the center line (e.g. don't mask them)
-                # (use a +- 25 degree around 0 as threshold)
-                cpoints = np.broadcast_to(
-                    np.isclose(xp, xc, atol=25)[:, np.newaxis], xs.shape
-                )
+            xs, ys, mask = self._wraparound(x, y, xs, ys, crs)
 
-                maskx[cpoints] = False
-                xs.mask[maskx] = True
-                ys.mask = xs.mask
-
-                # mask any datapoint that has less than 4 of the ellipse-points unmasked
-                mask = ~(
-                    n - np.count_nonzero(xs.mask, axis=1) <= min(n / 2, 4)
-                ) & np.isfinite(theta)
             return xs, ys, mask
 
-        def get_coll(self, x, y, crs, **kwargs):
-            xs, ys, mask = self._get_ellipse_points(
-                x, y, crs, self._selected_radius, self.radius_crs, n=self.n
-            )
-
-            # compress the coordinates (masked arrays produce artefacts on the boundary
-            # in case intermediate points are masked)
-            verts = (
-                np.column_stack((x.compressed(), y.compressed()))
-                for i, (x, y) in enumerate(zip(xs, ys))
-                if mask[i]
-            )
-            # remember masked points
-            self._m._data_mask = mask
-
-            color_and_array = Shapes._get_colors_and_array(kwargs, mask)
-
-            coll = PolyCollection(
-                verts,
-                # transOffset=self._m.ax.transData,
-                **color_and_array,
-                **kwargs,
-            )
-
-            return coll
-
     class _Rectangles(_ShapeBase):
         name = "rectangles"
 
         def __init__(self, m):
             super().__init__(m=m)
 
         def __call__(self, radius="estimate", radius_crs="in", mesh=False, n=None):
@@ -1131,14 +1076,95 @@
 
         def get_coll(self, x, y, crs, **kwargs):
             if self.mesh is True:
                 return self._get_trimesh_coll(x, y, crs, **kwargs)
             else:
                 return self._get_polygon_coll(x, y, crs, **kwargs)
 
+    class _Hexbin(object):
+        name = "hexbin"
+
+        def __init__(self, m):
+            self._m = m
+
+        def __call__(self, size=100, aggregator="mean"):
+            """
+            Draw a 2D hexagonal binning plot of the data.
+
+            All arguments are forwarded to `matplotlib.pyplot.hexbin()`.
+
+            Parameters
+            ----------
+            size : int, or (int, int), optional
+                If int, the number of hexagons in x-direction.
+                If a tuple of int is provided, the number of hexagons
+                in x- and y-direction
+
+                See matplotlib.pyplot.hexbin for more information about marker styles.
+            aggregator: str or callable
+                The function used to aggregate the data-values.
+                If a string is provided, it is identified as the associated numpy
+                function. The default is "mean".
+            """
+            from . import MapsGrid  # do this here to avoid circular imports!
+
+            for m in self._m if isinstance(self._m, MapsGrid) else [self._m]:
+                shape = self.__class__(m)
+                shape._size = size
+                shape._aggregator = aggregator
+                m._shape = shape
+
+        @property
+        def _initargs(self):
+            return dict(size=self._size, aggregator=self._aggregator)
+
+        @property
+        def radius(self):
+            radius = Shapes._get_radius(self._m, "estimate", "in")
+            return radius
+
+        @property
+        def radius_crs(self):
+            return "in"
+
+        def get_coll(self, x, y, crs, **kwargs):
+            # hide edgecolors if they are not explicitly set (to avoid overlapping
+            # hexagons due to large edge linewidths)
+            # matplotlib's default is currently `ec="face", lw=1`
+            if not any(i in kwargs for i in ("ec", "edgecolor")):
+                special_kwargs = {"ec": "none"}
+            else:
+                special_kwargs = {}
+
+            color_and_array = Shapes._get_colors_and_array(kwargs, None)
+
+            if isinstance(self._aggregator, str):
+                reduce_C_function = getattr(np, self._aggregator)
+            else:
+                reduce_C_function = self._aggregator
+
+            color_and_array["C"] = color_and_array.pop("array", None)
+
+            if "extent" not in kwargs:
+                dm = self._m._data_manager
+
+                extent = (dm._x0min, dm._x0max, dm._y0min, dm._y0max)
+
+            coll = self._m.ax.hexbin(
+                x,
+                y,
+                gridsize=self._size,
+                reduce_C_function=reduce_C_function,
+                extent=kwargs.get("extent", extent),
+                **color_and_array,
+                **kwargs,
+                **special_kwargs,
+            )
+            return coll
+
     class _ScatterPoints(object):
         name = "scatter_points"
 
         def __init__(self, m):
             self._m = m
 
         def __call__(self, size=None, marker=None):
@@ -1162,28 +1188,26 @@
 
                 See matplotlib.markers for more information about marker styles.
             """
             from . import MapsGrid  # do this here to avoid circular imports!
 
             for m in self._m if isinstance(self._m, MapsGrid) else [self._m]:
                 shape = self.__class__(m)
-                shape._size = size
+                shape._size = np.asanyarray(size)  # always convert to numpy
                 shape._marker = marker
                 m._shape = shape
 
         @property
         def _initargs(self):
             return dict(size=self._size, marker=self._marker)
 
         @property
         def _selected_size(self):
             # chedck if multiple size values were provided
-            q = isinstance(self._size, np.ndarray)
-
-            if q:
+            if np.size(self._size) > 1:
                 mask = self._m._data_manager._get_q()[0]
 
                 # quick exit if full data is in extent
                 if mask is True:
                     return self._size
 
                 size = self._size[mask]
@@ -2256,14 +2280,19 @@
         return shp.__call__(*args, **kwargs)
 
     @wraps(_ScatterPoints.__call__)
     def scatter_points(self, *args, **kwargs):
         shp = self._ScatterPoints(m=self._m)
         return shp.__call__(*args, **kwargs)
 
+    @wraps(_Hexbin.__call__)
+    def hexbin(self, *args, **kwargs):
+        shp = self._Hexbin(m=self._m)
+        return shp.__call__(*args, **kwargs)
+
     @wraps(_GeodCircles.__call__)
     def geod_circles(self, *args, **kwargs):
         shp = self._GeodCircles(m=self._m)
         return shp.__call__(*args, **kwargs)
 
     @wraps(_Ellipses.__call__)
     def ellipses(self, *args, **kwargs):
```

### Comparing `eomaps-8.0rc2/eomaps/utilities.py` & `eomaps-8.1/eomaps/utilities.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/webmap_containers.py` & `eomaps-8.1/eomaps/webmap_containers.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps/widgets.py` & `eomaps-8.1/eomaps/widgets.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/eomaps.egg-info/PKG-INFO` & `eomaps-8.1/eomaps.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eomaps
-Version: 8.0rc2
+Version: 8.1
 Summary: A library to create interactive maps of geographical datasets.
 Author-email: Raphael Quast <raphael.quast@geo.tuwien.ac.at>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, The EOmaps authors.
         
         Redistribution and use in source and binary forms, with or without
@@ -66,28 +66,36 @@
 Provides-Extra: classify
 Requires-Dist: mapclassify; extra == "classify"
 Provides-Extra: wms
 Requires-Dist: owslib; extra == "wms"
 Requires-Dist: requests; extra == "wms"
 Provides-Extra: shade
 Requires-Dist: datashader; extra == "shade"
+Requires-Dist: dask[dataframe]; extra == "shade"
 Provides-Extra: gui
 Requires-Dist: PyQt5; extra == "gui"
 Requires-Dist: qtpy; extra == "gui"
 
 
 <p align="center">
     <a href=https://github.com/raphaelquast/EOmaps>
     <img src="https://github.com/raphaelquast/EOmaps/blob/master/docs/_static/logo.png?raw=true" alt="EOmaps logo" width="55%">
     </a>
 </p>
 
-| Tests | Package | Documentation | License | Citation |
-|:-:|:-:|:-:|:-:|:-:|
-| [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/testMaps.yml/badge.svg?branch=master)](https://github.com/raphaelquast/EOmaps/actions/workflows/testMaps.yml)  [![codecov](https://codecov.io/gh/raphaelquast/EOmaps/graph/badge.svg)](https://codecov.io/gh/raphaelquast/EOmaps) | [![pypi](https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/eomaps/)  [![Conda Version](https://img.shields.io/conda/vn/conda-forge/eomaps.svg)](https://anaconda.org/conda-forge/eomaps) | [![Documentation Status](https://readthedocs.org/projects/eomaps/badge/?version=latest)](https://eomaps.readthedocs.io/en/latest/?badge=latest) |  [![License: BSD 3 clause](https://img.shields.io/badge/License-BSD_3_clause-blue.svg)](https://github.com/raphaelquast/EOmaps/blob/master/LICENSE) | [![10.5281/zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/badge/latestdoi/410829039) |
+<div align="center">
+
+
+|     Tests & Review      | [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/testMaps.yml/badge.svg?branch=master)](https://github.com/raphaelquast/EOmaps/actions/workflows/testMaps.yml) | [![codecov](https://codecov.io/gh/raphaelquast/EOmaps/graph/badge.svg)](https://codecov.io/gh/raphaelquast/EOmaps)  |                    [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/138)                    |
+| :---------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------: |
+| Package & Documentation |                                                [![pypi](https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/eomaps/)                                                 | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/eomaps.svg)](https://anaconda.org/conda-forge/eomaps) | [![Documentation Status](https://readthedocs.org/projects/eomaps/badge/?version=latest)](https://eomaps.readthedocs.io/en/latest/?badge=latest) |
+|   License & Citation    |                [![License: BSD 3 clause](https://img.shields.io/badge/License-BSD_3_clause-blue.svg)](https://github.com/raphaelquast/EOmaps/blob/master/LICENSE)                |  [![10.5281/zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/badge/latestdoi/410829039)  |                                                                                                                                                 |
+
+
+</div>
 
 <a href="https://www.buymeacoffee.com/raphaelquast" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png" alt="Buy Me A Coffee" align="right" style="height: 25px !important;" ></a>
 <a href="https://app.gitter.im/#/room/#EOmaps:gitter.im" target="_blank"><img src="https://img.shields.io/gitter/room/raphaelquast/EOmaps?style=social" alt="chat on gitter" align="left" style="height: 20px !important;" ></a>
 
 ----
 
 <h3 align="center">A python package to visualize and analyze geographical datasets.</h3>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eomaps Version: 8.0rc2 Summary: A library to create
+Metadata-Version: 2.1 Name: eomaps Version: 8.1 Summary: A library to create
 interactive maps of geographical datasets. Author-email: Raphael Quast
 geo.tuwien.ac.at> License: BSD 3-Clause License Copyright (c) 2021, The EOmaps
 authors. Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
@@ -34,31 +34,40 @@
 [classify,gui,io,shade,wms]; extra == "all" Provides-Extra: all-nogui Requires-
 Dist: eomaps[classify,io,shade,wms]; extra == "all-nogui" Provides-Extra: io
 Requires-Dist: pandas; extra == "io" Requires-Dist: geopandas; extra == "io"
 Requires-Dist: xarray; extra == "io" Requires-Dist: netcdf4; extra == "io"
 Requires-Dist: rioxarray; extra == "io" Provides-Extra: classify Requires-Dist:
 mapclassify; extra == "classify" Provides-Extra: wms Requires-Dist: owslib;
 extra == "wms" Requires-Dist: requests; extra == "wms" Provides-Extra: shade
-Requires-Dist: datashader; extra == "shade" Provides-Extra: gui Requires-Dist:
-PyQt5; extra == "gui" Requires-Dist: qtpy; extra == "gui"
+Requires-Dist: datashader; extra == "shade" Requires-Dist: dask[dataframe];
+extra == "shade" Provides-Extra: gui Requires-Dist: PyQt5; extra == "gui"
+Requires-Dist: qtpy; extra == "gui"
                                  _[_E_O_m_a_p_s_ _l_o_g_o_]
-| Tests | Package | Documentation | License | Citation | |:-:|:-:|:-:|:-:|:-:
-| | [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/
-testMaps.yml/badge.svg?branch=master)](https://github.com/raphaelquast/EOmaps/
-actions/workflows/testMaps.yml) [![codecov](https://codecov.io/gh/raphaelquast/
-EOmaps/graph/badge.svg)](https://codecov.io/gh/raphaelquast/EOmaps) | [![pypi]
-(https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/eomaps/) [!
-[Conda Version](https://img.shields.io/conda/vn/conda-forge/eomaps.svg)](https:
-//anaconda.org/conda-forge/eomaps) | [![Documentation Status](https://
-readthedocs.org/projects/eomaps/badge/?version=latest)](https://
-eomaps.readthedocs.io/en/latest/?badge=latest) | [![License: BSD 3 clause]
-(https://img.shields.io/badge/License-BSD_3_clause-blue.svg)](https://
-github.com/raphaelquast/EOmaps/blob/master/LICENSE) | [![10.5281/
-zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/
-badge/latestdoi/410829039) | _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]_[_c_h_a_t_ _o_n_ _g_i_t_t_e_r_]----
+ | Tests & Review | [![tests](https://github.com/raphaelquast/EOmaps/actions/
+     workflows/testMaps.yml/badge.svg?branch=master)](https://github.com/
+  raphaelquast/EOmaps/actions/workflows/testMaps.yml) | [![codecov](https://
+  codecov.io/gh/raphaelquast/EOmaps/graph/badge.svg)](https://codecov.io/gh/
+ raphaelquast/EOmaps) | [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://
+github.com/pyOpenSci/software-submission/issues/138) | | :--------------------
+-: | :-------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+----------------------: | :----------------------------------------------------
+-------------------------------------------------------------: | :-------------
+-------------------------------------------------------------------------------
+-------------------------------------------------: | | Package & Documentation
+  | [![pypi](https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/
+   eomaps/) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/
+   eomaps.svg)](https://anaconda.org/conda-forge/eomaps) | [![Documentation
+Status](https://readthedocs.org/projects/eomaps/badge/?version=latest)](https:/
+  /eomaps.readthedocs.io/en/latest/?badge=latest) | | License & Citation | [!
+  [License: BSD 3 clause](https://img.shields.io/badge/License-BSD_3_clause-
+  blue.svg)](https://github.com/raphaelquast/EOmaps/blob/master/LICENSE) | [!
+  [10.5281/zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://
+                   zenodo.org/badge/latestdoi/410829039) | |
+_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]_[_c_h_a_t_ _o_n_ _g_i_t_t_e_r_]----
   ******** AA ppyytthhoonn ppaacckkaaggee ttoo vviissuuaalliizzee aanndd aannaallyyzzee ggeeooggrraapphhiiccaall ddaattaasseettss.. ********
 EEOOmmaappss aims to provide a comprehensive, flexible, well-documented and easy-to-
 use API to create publication-ready maps that can directly be used for
 interactive data analysis.
 ## What can I do with EOmaps? **EOmaps** is built on top of [matplotlib](https:
 //matplotlib.org/) and [cartopy](https://scitools.org.uk/cartopy/docs/latest/
 ) and integrates well with the scientific python infrastructure (e.g., [numpy]
```

### Comparing `eomaps-8.0rc2/eomaps.egg-info/SOURCES.txt` & `eomaps-8.1/eomaps.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -68,14 +68,26 @@
 eomaps/qtcompanion/icons/peek_right_active.png
 eomaps/qtcompanion/icons/peek_square.png
 eomaps/qtcompanion/icons/peek_square_active.png
 eomaps/qtcompanion/icons/peek_top.png
 eomaps/qtcompanion/icons/peek_top_active.png
 eomaps/qtcompanion/icons/plus.png
 eomaps/qtcompanion/icons/plus_hoover.png
+eomaps/qtcompanion/widgets/__init__.py
+eomaps/qtcompanion/widgets/annotate.py
+eomaps/qtcompanion/widgets/click_callbacks.py
+eomaps/qtcompanion/widgets/draw.py
+eomaps/qtcompanion/widgets/editor.py
+eomaps/qtcompanion/widgets/extent.py
+eomaps/qtcompanion/widgets/files.py
+eomaps/qtcompanion/widgets/layer.py
+eomaps/qtcompanion/widgets/peek.py
+eomaps/qtcompanion/widgets/save.py
+eomaps/qtcompanion/widgets/utils.py
+eomaps/qtcompanion/widgets/wms.py
 eomaps/scripts/__init__.py
 eomaps/scripts/open.py
 tests/test_WMS_capabilities.py
 tests/test_basic_functions.py
 tests/test_callbacks.py
 tests/test_config.py
 tests/test_doc_codeblocks.py
```

### Comparing `eomaps-8.0rc2/pyproject.toml` & `eomaps-8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-include = ["eomaps", "eomaps.scripts", "eomaps.qtcompanion"]
+include = ["eomaps", "eomaps.scripts", "eomaps.qtcompanion", "eomaps.qtcompanion.widgets"]
 
 [tool.setuptools.package-data]
 eomaps = ["logo.png", "NE_features.json", "qtcompanion/icons/*"]
 
 
 [project]
 name = "eomaps"
-version = "8.0rc2"
+version = "8.1"
 description = "A library to create interactive maps of geographical datasets."
 readme = "README.md"
 license = {file = "LICENSE"}
 
 requires-python = ">=3.8"
 
 authors = [
@@ -62,15 +62,18 @@
 classify = ["mapclassify"]
 
 wms = [
     "owslib",
     "requests",
 ]
 
-shade = ["datashader"]
+shade = [
+    "datashader",
+    "dask[dataframe]",  # to address https://github.com/dask/dask/issues/10995
+]
 
 gui = [
     "PyQt5",
     "qtpy"
     ]
 
 [project.scripts]
```

### Comparing `eomaps-8.0rc2/tests/test_WMS_capabilities.py` & `eomaps-8.1/tests/test_WMS_capabilities.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/tests/test_basic_functions.py` & `eomaps-8.1/tests/test_basic_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,14 +210,27 @@
         m2 = m.new_layer()
         m2.inherit_data(m)
         m2.set_shape.voronoi_diagram(masked=True, mask_radius=5)
         m2.plot_map()
 
         plt.close("all")
 
+        # hexbin
+        m = Maps(4326)
+        m.set_data(usedata, x="x", y="y", crs=3857)
+        m.set_shape.hexbin()
+        m.plot_map()
+
+        m2 = m.new_layer()
+        m2.inherit_data(m)
+        m2.set_shape.hexbin(size=(50, 25), aggregator=np.median)
+        m2.plot_map()
+
+        plt.close("all")
+
     def test_cpos(self):
         m = Maps(4326)
 
         for cpos, color in zip(["ul", "ur", "ll", "lr", "c"], "rgbcm"):
             m2 = m.new_layer()
             m2.set_shape.ellipses(n=100)
             m2.set_data(
@@ -381,14 +394,22 @@
             np.arange(1710, 1740, 1),
             facecolor=[1, 0, 0, 0.5],
             edgecolor="r",
             shape="rectangles",
         )
 
         m.add_marker(
+            xy=[(20, 3), (20, 4)],
+            xy_crs=4326,
+            shape="scatter_points",
+            radius=1000,
+            facecolor=("red", "green"),
+        )
+
+        m.add_marker(
             np.arange(1410, 1440, 1),
             facecolor=[1, 0, 0, 0.5],
             edgecolor="r",
             radius=50000,
             radius_crs="in",
         )
```

### Comparing `eomaps-8.0rc2/tests/test_callbacks.py` & `eomaps-8.1/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/tests/test_config.py` & `eomaps-8.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/tests/test_doc_codeblocks.py` & `eomaps-8.1/tests/test_doc_codeblocks.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/tests/test_doc_notebooks.py` & `eomaps-8.1/tests/test_doc_notebooks.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/tests/test_drawer.py` & `eomaps-8.1/tests/test_drawer.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/tests/test_examples.py` & `eomaps-8.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/tests/test_from_file.py` & `eomaps-8.1/tests/test_from_file.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/tests/test_layout_editor.py` & `eomaps-8.1/tests/test_layout_editor.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/tests/test_plot_shapes.py` & `eomaps-8.1/tests/test_plot_shapes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,89 +1,124 @@
-import unittest
+import pytest
 
 import pandas as pd
 import numpy as np
+import matplotlib.pyplot as plt
 
 from eomaps import Maps
-import matplotlib.pyplot as plt
 
 # TODO add proper (extensive) tests for each shape!
 
+x, y = np.linspace(-40, 40, 50), np.linspace(-25, 30, 150)
+x2d, y2d = np.meshgrid(x, y, indexing="ij")
+data = x2d**2 + y2d**2
+
+# use an irregular sample of the data to check irregular datasets as well
+data_pandas = dict(
+    data=pd.DataFrame(
+        dict(lon=x2d.ravel(), lat=y2d.ravel(), value=data.ravel())
+    ).sample(1000),
+    x="lon",
+    y="lat",
+    parameter="value",
+)
+data_1d = dict(x=x2d.ravel(), y=y2d.ravel(), data=data.ravel())
+data_1d_2d = dict(x=x, y=y, data=data)
+data_2d = dict(x=x2d, y=y2d, data=data)
+
+testdata = [data_pandas, data_1d, data_1d_2d, data_2d]
+ids = ["pandas", "1D", "1D2D", "2D"]
+
+# %%
+
+
+@pytest.fixture
+def close_all():
+    yield
+    plt.close("all")
+
+
+@pytest.mark.usefixtures("close_all")
+@pytest.mark.parametrize("data", testdata, ids=ids)
+def test_hexbin(data):
+    m = Maps(ax=221, figsize=(10, 6))
+    m.set_data(**data)
+    m.set_shape.hexbin(size=(10, 5))
+    m.plot_map()
+    m.add_colorbar()
+
+    m2 = m.new_map(ax=222, inherit_data=True)
+    m2.set_shape.hexbin(size=20, aggregator="median")
+    m2.plot_map(cmap="RdYlBu")
+    m2.add_colorbar()
+
+    m3 = m.new_map(ax=223, inherit_data=True)
+    m3.set_shape.hexbin(size=10, aggregator="min")
+    m3.plot_map(cmap="RdYlBu")
+    m3.add_colorbar()
+
+    m4 = m.new_map(ax=224, inherit_data=True)
+    m4.set_shape.hexbin(size=10, aggregator="max")
+    m4.set_classify.EqualInterval(k=5)
+    m4.plot_map(cmap="RdYlBu")
+    m4.add_colorbar()
+
+
+@pytest.mark.usefixtures("close_all")
+@pytest.mark.parametrize("data", testdata, ids=ids)
+def test_contour(data):
+    m = Maps(ax=221, figsize=(10, 6))
+    m.subplots_adjust(left=0.01, right=0.99)
+    m.set_data(**data)
+    m.set_shape.contour(filled=True)
+    m.plot_map()
+    m.add_colorbar()
+
+    m1 = m.new_map(ax=222, inherit_data=True)
+    m1.set_shape.contour(filled=False)
+    m1.plot_map()
+    m1.add_colorbar()
+
+    m2 = m.new_map(ax=223, inherit_data=True)
+    m2.add_feature.preset("ocean", "land")
+    m2.set_shape.contour(filled=True)
+    m2.plot_map(
+        colors=["none", "r", (0, 1, 0, 0.25), "r"],
+        hatches=["", "xxxx", "///", "xxxx"],
+    )
+
+    m3 = m.new_map(ax=224, inherit_data=True)
+    m3.set_shape.ellipses()
+    m3.plot_map(alpha=0.25)
+    cb3 = m3.add_colorbar()
+
+    m3_1 = m3.new_layer("contours", inherit_data=True)
+    m3_1.set_shape.contour(filled=False)
+    m3_1.plot_map(linestyles=["--", "-", ":", "-."])
+
+    cb3.indicate_contours(
+        contour_map=m3_1,
+        add_labels="top",
+        exclude_levels=[0, -1],
+        label_kwargs=dict(color="r", rotation=90, xytext=(-5, -10)),
+    )
+
+    cb3.indicate_contours(
+        contour_map=m3_1,
+        add_labels="top",
+        use_levels=[1],
+        label_names=["This one!"],
+        label_kwargs=dict(
+            xytext=(-40, 20), zorder=-1, arrowprops={"arrowstyle": "fancy"}
+        ),
+    )
+
+    # TODO using 'clabel' causes collections to be re-drawn
+    # which puts the new contours on the default layer and leaves
+    # the old contours as "artists without a figure" in the blit-manager!
+    # see https://github.com/raphaelquast/EOmaps/issues/218
+
+    # arts = m3_1.ax.clabel(m3_1.coll.contour_set)
+    # for a in arts:
+    #     m3_1.BM.add_bg_artist(a, layer=m3_1.layer)
 
-class TestPlotShapes(unittest.TestCase):
-    def setUp(self):
-        x, y = np.meshgrid(np.linspace(-40, 40, 50), np.linspace(-25, 30, 50))
-        data = x**2 + y**2
-
-        # use an irregular sample of the data to check irregular datasets as well
-        self.data_pandas = dict(
-            data=pd.DataFrame(
-                dict(lon=x.ravel(), lat=y.ravel(), value=data.ravel())
-            ).sample(500),
-            x="lon",
-            y="lat",
-            parameter="value",
-        )
-
-        self.data_1d = dict(x=x.ravel(), y=y.ravel(), data=data.ravel())
-
-        self.data_2d = dict(x=x, y=y, data=data)
-
-    def test_contour(self):
-        for data in (self.data_pandas, self.data_1d, self.data_2d):
-            m = Maps(ax=221, figsize=(10, 6))
-            m.subplots_adjust(left=0.01, right=0.99)
-            m.set_data(**data)
-            m.set_shape.contour(filled=True)
-            m.plot_map()
-            cb = m.add_colorbar()
-
-            m1 = m.new_map(ax=222, inherit_data=True)
-            m1.set_shape.contour(filled=False)
-            m1.plot_map()
-            cb1 = m1.add_colorbar()
-
-            m2 = m.new_map(ax=223, inherit_data=True)
-            m2.add_feature.preset("ocean", "land")
-            m2.set_shape.contour(filled=True)
-            m2.plot_map(
-                colors=["none", "r", (0, 1, 0, 0.25), "r"],
-                hatches=["", "xxxx", "///", "xxxx"],
-            )
-
-            m3 = m.new_map(ax=224, inherit_data=True)
-            m3.set_shape.ellipses()
-            m3.plot_map(alpha=0.25)
-            cb3 = m3.add_colorbar()
-
-            m3_1 = m3.new_layer("contours", inherit_data=True)
-            m3_1.set_shape.contour(filled=False)
-            m3_1.plot_map(linestyles=["--", "-", ":", "-."])
-
-            cb3.indicate_contours(
-                contour_map=m3_1,
-                add_labels="top",
-                exclude_levels=[0, -1],
-                label_kwargs=dict(color="r", rotation=90, xytext=(-5, -10)),
-            )
-
-            cb3.indicate_contours(
-                contour_map=m3_1,
-                add_labels="top",
-                use_levels=[1],
-                label_names=["This one!"],
-                label_kwargs=dict(
-                    xytext=(-40, 20), zorder=-1, arrowprops={"arrowstyle": "fancy"}
-                ),
-            )
-
-            # TODO using 'clabel' causes collections to be re-drawn
-            # which puts the new contours on the default layer and leaves
-            # the old contours as "artists without a figure" in the blit-manager!
-            # see https://github.com/raphaelquast/EOmaps/issues/218
-
-            # arts = m3_1.ax.clabel(m3_1.coll.contour_set)
-            # for a in arts:
-            #     m3_1.BM.add_bg_artist(a, layer=m3_1.layer)
-
-            m.show_layer("base", "contours")
-            plt.close("all")
+    m.show_layer("base", "contours")
```

### Comparing `eomaps-8.0rc2/tests/test_raster_aggregaton.py` & `eomaps-8.1/tests/test_raster_aggregaton.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.0rc2/tests/test_widgets.py` & `eomaps-8.1/tests/test_widgets.py`

 * *Files identical despite different names*

