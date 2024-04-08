# Comparing `tmp/taipy-gui-3.1.0.tar.gz` & `tmp/taipy-gui-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-gui-3.1.0.tar", last modified: Mon Mar  4 15:25:55 2024, max compression
+gzip compressed data, was "taipy-gui-3.1.1.tar", last modified: Mon Apr  8 13:09:31 2024, max compression
```

## Comparing `taipy-gui-3.1.0.tar` & `taipy-gui-3.1.1.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.356296 taipy-gui-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-04 15:25:52.000000 taipy-gui-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-03-04 15:25:55.356296 taipy-gui-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 15:25:55.356296 taipy-gui-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-04 15:25:52.000000 taipy-gui-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.320297 taipy-gui-3.1.0/taipy/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-04 15:25:52.000000 taipy-gui-3.1.0/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.324297 taipy-gui-3.1.0/taipy/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_default_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_gui_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_gui_section.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.324297 taipy-gui-3.1.0/taipy/gui/_renderers/
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.324297 taipy-gui-3.1.0/taipy/gui/_renderers/_html/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/_html/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/_html/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.324297 taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/blocproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/postproc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)    44767 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    25088 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_renderers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.324297 taipy-gui-3.1.0/taipy/gui/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75359 2024-03-04 15:22:43.000000 taipy-gui-3.1.0/taipy/gui/builder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/builder/_api_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/builder/_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/builder/_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/builder/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/builder/page.py
--rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.328297 taipy-gui-3.1.0/taipy/gui/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/custom/_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.328297 taipy-gui-3.1.0/taipy/gui/data/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/array_dict_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/content_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/data_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/data_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.328297 taipy-gui-3.1.0/taipy/gui/data/decimator/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/decimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/decimator/lttb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/decimator/minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/decimator/rdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/decimator/scatter_decimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/numpy_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/pandas_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.328297 taipy-gui-3.1.0/taipy/gui/extension/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17898 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/extension/library.py
--rw-r--r--   0 runner    (1001) docker     (127)   111956 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-04 15:22:42.000000 taipy-gui-3.1.0/taipy/gui/gui.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19646 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/gui_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/partial.py
--rw-r--r--   0 runner    (1001) docker     (127)    13696 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-04 15:25:52.000000 taipy-gui-3.1.0/taipy/gui/setup.requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.332296 taipy-gui-3.1.0/taipy/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15828 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/_locals_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/_map_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/_runtime_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/_variable_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/chart_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/clientvarname.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/expr_var_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/filename.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/filter_locals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/get_imported_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/get_module_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/get_page_from_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/getdatecolstrname.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/is_debugging.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/is_port_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/isnotebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/table_col_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/utils/varnamefromcontent.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/version.json
--rw-r--r--   0 runner    (1001) docker     (127)    62608 2024-03-04 15:21:03.000000 taipy-gui-3.1.0/taipy/gui/viselements.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.348296 taipy-gui-3.1.0/taipy/gui/webapp/
--rw-r--r--   0 runner    (1001) docker     (127)  3626049 2024-03-04 15:24:56.000000 taipy-gui-3.1.0/taipy/gui/webapp/236.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-04 15:24:56.000000 taipy-gui-3.1.0/taipy/gui/webapp/236.taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   112749 2024-03-04 15:24:56.000000 taipy-gui-3.1.0/taipy/gui/webapp/294.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (127)   207070 2024-03-04 15:24:56.000000 taipy-gui-3.1.0/taipy/gui/webapp/587.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-04 15:23:15.000000 taipy-gui-3.1.0/taipy/gui/webapp/677.taipy-gui-base.js
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-04 15:24:56.000000 taipy-gui-3.1.0/taipy/gui/webapp/677.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.348296 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.352296 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/base/base.css
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/base/fontfaces.css
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/base/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.352296 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/blocks/layout.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.352296 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/button.css
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/chart.css
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/date.css
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/expandable.css
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/image.css
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/input.css
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/navbar.css
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/number.css
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/selector.css
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/slider.css
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/table.css
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/toggle.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.352296 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/elements/card.css
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/elements/container.css
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/elements/header.css
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/elements/sidebar.css
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/stylekit.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.356296 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/utilities/colors.css
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/utilities/misc.css
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/utilities/spacing.css
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/utilities/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.356296 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/colors.css
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/elements.css
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/misc.css
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/shapes.css
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/spacing.css
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/typography.css
--rw-r--r--   0 runner    (1001) docker     (127)    47350 2024-03-04 15:23:15.000000 taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui-base.js
--rw-r--r--   0 runner    (1001) docker     (127)   216794 2024-03-04 15:23:45.000000 taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui-deps-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)  4990278 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui-deps.dll.js
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-04 15:23:45.000000 taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui-dom.js
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)  1187368 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-04 15:24:56.000000 taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-04 15:25:18.000000 taipy-gui-3.1.0/taipy/gui/webapp/taipy.status.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:25:55.356296 taipy-gui-3.1.0/taipy_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-03-04 15:25:55.000000 taipy-gui-3.1.0/taipy_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-03-04 15:25:55.000000 taipy-gui-3.1.0/taipy_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:25:55.000000 taipy-gui-3.1.0/taipy_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:25:53.000000 taipy-gui-3.1.0/taipy_gui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-04 15:25:55.000000 taipy-gui-3.1.0/taipy_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 15:25:55.000000 taipy-gui-3.1.0/taipy_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.164938 taipy-gui-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 13:09:29.000000 taipy-gui-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-08 13:09:31.164938 taipy-gui-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:09:31.164938 taipy-gui-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-08 13:09:29.000000 taipy-gui-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.124937 taipy-gui-3.1.1/taipy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-08 13:09:29.000000 taipy-gui-3.1.1/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.128937 taipy-gui-3.1.1/taipy/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_gui_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_gui_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.132938 taipy-gui-3.1.1/taipy/gui/_renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.132938 taipy-gui-3.1.1/taipy/gui/_renderers/_html/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/_html/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/_html/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.132938 taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/blocproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/postproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44892 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25088 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_renderers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.132938 taipy-gui-3.1.1/taipy/gui/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75359 2024-04-08 13:06:22.000000 taipy-gui-3.1.1/taipy/gui/builder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/builder/_api_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/builder/_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/builder/_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/builder/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/builder/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.132938 taipy-gui-3.1.1/taipy/gui/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/custom/_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.136937 taipy-gui-3.1.1/taipy/gui/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/array_dict_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/content_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/data_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.136937 taipy-gui-3.1.1/taipy/gui/data/decimator/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/decimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/decimator/lttb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/decimator/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/decimator/rdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/decimator/scatter_decimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/numpy_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/pandas_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.136937 taipy-gui-3.1.1/taipy/gui/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17898 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/extension/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111956 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-08 13:06:21.000000 taipy-gui-3.1.1/taipy/gui/gui.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19646 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/gui_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13696 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 13:09:29.000000 taipy-gui-3.1.1/taipy/gui/setup.requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.140937 taipy-gui-3.1.1/taipy/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15828 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/_locals_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/_map_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/_runtime_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/_variable_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/chart_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/clientvarname.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/expr_var_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/filename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/filter_locals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/get_imported_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/get_module_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/get_page_from_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/getdatecolstrname.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/is_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/is_port_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/isnotebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/table_col_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/utils/varnamefromcontent.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/version.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62608 2024-04-08 13:03:51.000000 taipy-gui-3.1.1/taipy/gui/viselements.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.156937 taipy-gui-3.1.1/taipy/gui/webapp/
+-rw-r--r--   0 runner    (1001) docker     (127)  3626049 2024-04-08 13:08:33.000000 taipy-gui-3.1.1/taipy/gui/webapp/236.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-08 13:08:33.000000 taipy-gui-3.1.1/taipy/gui/webapp/236.taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   112749 2024-04-08 13:08:33.000000 taipy-gui-3.1.1/taipy/gui/webapp/294.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (127)   207070 2024-04-08 13:08:33.000000 taipy-gui-3.1.1/taipy/gui/webapp/587.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-08 13:06:56.000000 taipy-gui-3.1.1/taipy/gui/webapp/677.taipy-gui-base.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-08 13:08:33.000000 taipy-gui-3.1.1/taipy/gui/webapp/677.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.156937 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.156937 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/base/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/base/fontfaces.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/base/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.156937 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/blocks/layout.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.160938 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/button.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/chart.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/date.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/expandable.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/image.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/input.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/navbar.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/number.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/selector.css
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/slider.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/table.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/toggle.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.160938 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/elements/card.css
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/elements/container.css
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/elements/header.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/elements/sidebar.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/stylekit.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.160938 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/utilities/colors.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/utilities/misc.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/utilities/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/utilities/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.164938 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/colors.css
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/elements.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/misc.css
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/shapes.css
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/typography.css
+-rw-r--r--   0 runner    (1001) docker     (127)    47350 2024-04-08 13:06:56.000000 taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui-base.js
+-rw-r--r--   0 runner    (1001) docker     (127)   216794 2024-04-08 13:07:25.000000 taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui-deps-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)  4990278 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui-deps.dll.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-08 13:07:25.000000 taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui-dom.js
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)  1187475 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-08 13:08:33.000000 taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 13:08:55.000000 taipy-gui-3.1.1/taipy/gui/webapp/taipy.status.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:09:31.164938 taipy-gui-3.1.1/taipy_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-08 13:09:31.000000 taipy-gui-3.1.1/taipy_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-08 13:09:31.000000 taipy-gui-3.1.1/taipy_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:09:31.000000 taipy-gui-3.1.1/taipy_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:09:29.000000 taipy-gui-3.1.1/taipy_gui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-08 13:09:31.000000 taipy-gui-3.1.1/taipy_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 13:09:31.000000 taipy-gui-3.1.1/taipy_gui.egg-info/top_level.txt
```

### Comparing `taipy-gui-3.1.0/LICENSE` & `taipy-gui-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/PKG-INFO` & `taipy-gui-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-gui
-Version: 3.1.0
+Version: 3.1.1
 Summary: Low-code library to create graphical user interfaces on the Web for your Python applications.
 Home-page: https://github.com/avaiga/taipy-gui
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-gui
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 Requires-Dist: gitignore-parser<=0.1.11,>=0.1
 Requires-Dist: kthread<=0.2.3,>=0.2.3
 Requires-Dist: markdown<=3.5.2,>=3.4.4
 Requires-Dist: pandas<=2.2.0,>=1.3.5
 Requires-Dist: python-dotenv<=1.0.1,>=1.0.0
 Requires-Dist: pytz<=2023.3.post1,>=2021.3
 Requires-Dist: simple-websocket<=1.0.0,>=0.10.1
-Requires-Dist: taipy-config==3.1.0
+Requires-Dist: taipy-config<3.2.0,>=3.1.1
 Requires-Dist: twisted<=23.10.0,>=23.8.0
 Requires-Dist: tzlocal<=5.2,>=3.0
 Provides-Extra: ngrok
 Requires-Dist: pyngrok<6.0,>=5.1; extra == "ngrok"
 Provides-Extra: image
 Requires-Dist: python-magic<0.5,>=0.4.24; platform_system != "Windows" and extra == "image"
 Requires-Dist: python-magic-bin<0.5,>=0.4.14; platform_system == "Windows" and extra == "image"
```

### Comparing `taipy-gui-3.1.0/README.md` & `taipy-gui-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/setup.py` & `taipy-gui-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/__init__.py` & `taipy-gui-3.1.1/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/__init__.py` & `taipy-gui-3.1.1/taipy/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_default_config.py` & `taipy-gui-3.1.1/taipy/gui/_default_config.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_gui_cli.py` & `taipy-gui-3.1.1/taipy/gui/_gui_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_gui_section.py` & `taipy-gui-3.1.1/taipy/gui/_gui_section.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_init.py` & `taipy-gui-3.1.1/taipy/gui/_init.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_page.py` & `taipy-gui-3.1.1/taipy/gui/_page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/__init__.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/_html/__init__.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/_html/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/_html/factory.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/_html/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/_html/parser.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/_html/parser.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/__init__.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/blocproc.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/blocproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/control.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/control.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/factory.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/postproc.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/postproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/_markdown/preproc.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/_markdown/preproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/builder.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -771,14 +771,16 @@
                     if native_type and isinstance(val, str):
                         with contextlib.suppress(Exception):
                             val = float(val)
                     self.__set_default_value(var_name, val, native_type=native_type)
                 else:
                     self.__set_default_value(var_name, var_type=var_type)
         else:
+            if var_type == PropertyType.data:
+                _warn(f"{self.__control_type}.data property should be bound.")
             value = self.__attributes.get(var_name)
             if value is not None:
                 if native_type:
                     if isinstance(value, str):
                         with contextlib.suppress(Exception):
                             value = float(value)
                     if isinstance(value, (int, float)):
```

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/factory.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/json.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/json.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_renderers/utils.py` & `taipy-gui-3.1.1/taipy/gui/_renderers/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/_warnings.py` & `taipy-gui-3.1.1/taipy/gui/_warnings.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/builder/__init__.py` & `taipy-gui-3.1.1/taipy/gui/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/builder/__init__.pyi` & `taipy-gui-3.1.1/taipy/gui/builder/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1063,27 +1063,27 @@
         """
         ...
 
 class expandable(_Block):
     _ELEMENT_NAME: str
     def __init__(
         self,
-        value=...,
+        title=...,
         expanded=...,
         partial=...,
         page=...,
         id=...,
         properties=...,
         class_name=...,
         hover_text=...,
         on_change=...,
     ) -> None:
         """
         Arguments:
-            value (dynamic(str)): Title of this block element.         expanded (dynamic(bool)): If True, the block is expanded, and the content is displayed.<br/>If False, the block is collapsed and its content is hidden. (default: True)        partial (Partial): A Partial object that holds the content of the block.<br/>This should not be defined if <i>page</i> is set.         page (str): The page name to show as the content of the block.<br/>This should not be defined if <i>partial</i> is set.         id (str): The identifier that will be assigned to the rendered HTML component.         properties (dict[str, any]): Bound to a dictionary that contains additional properties for this element.         class_name (dynamic(str)): The list of CSS class names that will be associated with the generated HTML Element.<br/>These class names will be added to the default <code>taipy-&lt;element_type&gt;</code>.         hover_text (dynamic(str)): The information that is displayed when the user hovers over this element.         on_change (Callback): The name of a function that is triggered when the value is updated.<br/>The parameters of that function are all optional:
+            title (dynamic(str)): Title of this block element.         expanded (dynamic(bool)): If True, the block is expanded, and the content is displayed.<br/>If False, the block is collapsed and its content is hidden. (default: True)        partial (Partial): A Partial object that holds the content of the block.<br/>This should not be defined if <i>page</i> is set.         page (str): The page name to show as the content of the block.<br/>This should not be defined if <i>partial</i> is set.         id (str): The identifier that will be assigned to the rendered HTML component.         properties (dict[str, any]): Bound to a dictionary that contains additional properties for this element.         class_name (dynamic(str)): The list of CSS class names that will be associated with the generated HTML Element.<br/>These class names will be added to the default <code>taipy-&lt;element_type&gt;</code>.         hover_text (dynamic(str)): The information that is displayed when the user hovers over this element.         on_change (Callback): The name of a function that is triggered when the value is updated.<br/>The parameters of that function are all optional:
                 <ul>
                 <li>state (<code>State^</code>): the state instance.</li>
                 <li>var_name (str): the variable name.</li>
                 <li>value (any): the new value.</li>
                 </ul>
         """
         ...
```

### Comparing `taipy-gui-3.1.0/taipy/gui/builder/_api_generator.py` & `taipy-gui-3.1.1/taipy/gui/builder/_api_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,21 @@
             setattr(
                 library_module,
                 element_name,
                 _ElementApiGenerator().create_control_api(
                     element_name, f"{library_name}.{element_name}", element.default_attribute
                 ),
             )
+            # Allow element to be accessed from the root module
+            if hasattr(self.__module, element_name):
+                _TaipyLogger()._get_logger().info(
+                    f"Can't add element `{element_name}` of library `{library_name}` to the root of Builder API as another element with the same name already exists."  # noqa: E501
+                )
+                continue
+            setattr(self.__module, element_name, getattr(library_module, element_name))
 
     @staticmethod
     def create_block_api(
         classname: str,
         element_name: str,
         default_property: str,
     ):
```

### Comparing `taipy-gui-3.1.0/taipy/gui/builder/_context_manager.py` & `taipy-gui-3.1.1/taipy/gui/builder/_context_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/builder/_element.py` & `taipy-gui-3.1.1/taipy/gui/builder/_element.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/builder/_factory.py` & `taipy-gui-3.1.1/taipy/gui/builder/_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/builder/page.py` & `taipy-gui-3.1.1/taipy/gui/builder/page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/config.py` & `taipy-gui-3.1.1/taipy/gui/config.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/custom/__init__.py` & `taipy-gui-3.1.1/taipy/gui/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/custom/_page.py` & `taipy-gui-3.1.1/taipy/gui/custom/_page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/__init__.py` & `taipy-gui-3.1.1/taipy/gui/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/array_dict_data_accessor.py` & `taipy-gui-3.1.1/taipy/gui/data/array_dict_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/content_accessor.py` & `taipy-gui-3.1.1/taipy/gui/data/content_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/data_accessor.py` & `taipy-gui-3.1.1/taipy/gui/data/data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/data_format.py` & `taipy-gui-3.1.1/taipy/gui/data/data_format.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/data_scope.py` & `taipy-gui-3.1.1/taipy/gui/data/data_scope.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/decimator/__init__.py` & `taipy-gui-3.1.1/taipy/gui/data/decimator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/decimator/lttb.py` & `taipy-gui-3.1.1/taipy/gui/data/decimator/lttb.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/decimator/minmax.py` & `taipy-gui-3.1.1/taipy/gui/data/decimator/minmax.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/decimator/rdp.py` & `taipy-gui-3.1.1/taipy/gui/data/decimator/rdp.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/decimator/scatter_decimator.py` & `taipy-gui-3.1.1/taipy/gui/data/decimator/scatter_decimator.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/numpy_data_accessor.py` & `taipy-gui-3.1.1/taipy/gui/data/numpy_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/pandas_data_accessor.py` & `taipy-gui-3.1.1/taipy/gui/data/pandas_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/data/utils.py` & `taipy-gui-3.1.1/taipy/gui/data/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/extension/__init__.py` & `taipy-gui-3.1.1/taipy/gui/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/extension/library.py` & `taipy-gui-3.1.1/taipy/gui/extension/library.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/gui.py` & `taipy-gui-3.1.1/taipy/gui/gui.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/gui.pyi` & `taipy-gui-3.1.1/taipy/gui/gui.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     on_init: Incomplete
     on_navigate: Incomplete
     on_exception: Incomplete
     on_status: Incomplete
     on_user_content: Incomplete
     def __init__(
         self,
-        page: t.Optional[t.Union[str, Page]] = None,
-        pages: t.Optional[dict] = None,
-        css_file: t.Optional[str] = None,
-        path_mapping: t.Optional[dict] = None,
-        env_filename: t.Optional[str] = None,
-        libraries: t.Optional[t.List[ElementLibrary]] = None,
-        flask: t.Optional[Flask] = None,
+        page: str | Page | None = None,
+        pages: dict | None = None,
+        css_file: str | None = None,
+        path_mapping: dict | None = None,
+        env_filename: str | None = None,
+        libraries: t.List[ElementLibrary] | None = None,
+        flask: Flask | None = None,
     ) -> None: ...
     @staticmethod
     def add_library(library: ElementLibrary) -> None: ...
     @staticmethod
     def register_content_provider(
         content_type: type, content_provider: t.Callable[..., str]
     ) -> None: ...
@@ -41,21 +41,19 @@
     def __enter__(self): ...
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         traceback: types.TracebackType | None,
     ): ...
-    def add_page(
-        self, name: str, page: t.Union[str, Page], style: t.Optional[str] = ""
-    ) -> None: ...
+    def add_page(self, name: str, page: str | Page, style: str | None = "") -> None: ...
     def add_pages(
-        self, pages: t.Optional[t.Union[t.Mapping[str, t.Union[str, Page]], str]] = None
+        self, pages: t.Mapping[str, str | Page] | str | None = None
     ) -> None: ...
-    def add_partial(self, page: t.Union[str, Page]) -> Partial: ...
+    def add_partial(self, page: str | Page) -> Partial: ...
     def load_config(self, config: Config) -> None: ...
     def get_flask_app(self) -> Flask: ...
     state: Incomplete
     def run(
         self,
         allow_unsafe_werkzeug: bool = ...,
         async_mode: str = ...,
@@ -88,10 +86,10 @@
         stylekit: t.Union[bool, Stylekit] = ...,
         upload_folder: t.Optional[str] = ...,
         use_arrow: bool = ...,
         use_reloader: bool = ...,
         watermark: t.Optional[str] = ...,
         webapp_path: t.Optional[str] = ...,
         port: int = ...,
-    ) -> t.Optional[Flask]: ...
+    ) -> Flask | None: ...
     def reload(self) -> None: ...
     def stop(self) -> None: ...
```

### Comparing `taipy-gui-3.1.0/taipy/gui/gui_actions.py` & `taipy-gui-3.1.1/taipy/gui/gui_actions.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/icon.py` & `taipy-gui-3.1.1/taipy/gui/icon.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/page.py` & `taipy-gui-3.1.1/taipy/gui/page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/partial.py` & `taipy-gui-3.1.1/taipy/gui/partial.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/server.py` & `taipy-gui-3.1.1/taipy/gui/server.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/state.py` & `taipy-gui-3.1.1/taipy/gui/state.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/types.py` & `taipy-gui-3.1.1/taipy/gui/types.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/__init__.py` & `taipy-gui-3.1.1/taipy/gui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/_adapter.py` & `taipy-gui-3.1.1/taipy/gui/utils/_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/_attributes.py` & `taipy-gui-3.1.1/taipy/gui/utils/_attributes.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/_bindings.py` & `taipy-gui-3.1.1/taipy/gui/utils/_bindings.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/_evaluator.py` & `taipy-gui-3.1.1/taipy/gui/utils/_evaluator.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/_locals_context.py` & `taipy-gui-3.1.1/taipy/gui/utils/_locals_context.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/_map_dict.py` & `taipy-gui-3.1.1/taipy/gui/utils/_map_dict.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/_runtime_manager.py` & `taipy-gui-3.1.1/taipy/gui/utils/_runtime_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/_variable_directory.py` & `taipy-gui-3.1.1/taipy/gui/utils/_variable_directory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/boolean.py` & `taipy-gui-3.1.1/taipy/gui/utils/boolean.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/chart_config_builder.py` & `taipy-gui-3.1.1/taipy/gui/utils/chart_config_builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/clientvarname.py` & `taipy-gui-3.1.1/taipy/gui/utils/clientvarname.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/datatype.py` & `taipy-gui-3.1.1/taipy/gui/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/date.py` & `taipy-gui-3.1.1/taipy/gui/utils/date.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/expr_var_name.py` & `taipy-gui-3.1.1/taipy/gui/utils/expr_var_name.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/filename.py` & `taipy-gui-3.1.1/taipy/gui/utils/filename.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/filter_locals.py` & `taipy-gui-3.1.1/taipy/gui/utils/filter_locals.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/get_imported_var.py` & `taipy-gui-3.1.1/taipy/gui/utils/get_imported_var.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/get_module_name.py` & `taipy-gui-3.1.1/taipy/gui/utils/get_module_name.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/get_page_from_module.py` & `taipy-gui-3.1.1/taipy/gui/utils/get_page_from_module.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/getdatecolstrname.py` & `taipy-gui-3.1.1/taipy/gui/utils/getdatecolstrname.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/html.py` & `taipy-gui-3.1.1/taipy/gui/utils/html.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/is_debugging.py` & `taipy-gui-3.1.1/taipy/gui/utils/is_debugging.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/is_port_open.py` & `taipy-gui-3.1.1/taipy/gui/utils/is_port_open.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/isnotebook.py` & `taipy-gui-3.1.1/taipy/gui/utils/isnotebook.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/proxy.py` & `taipy-gui-3.1.1/taipy/gui/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/singleton.py` & `taipy-gui-3.1.1/taipy/gui/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/table_col_builder.py` & `taipy-gui-3.1.1/taipy/gui/utils/table_col_builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/types.py` & `taipy-gui-3.1.1/taipy/gui/utils/types.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/utils/varnamefromcontent.py` & `taipy-gui-3.1.1/taipy/gui/utils/varnamefromcontent.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/viselements.json` & `taipy-gui-3.1.1/taipy/gui/viselements.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996744791666666%*

 * *Differences: {"'blocks'": "{1: {1: {'properties': {0: {'name': 'title'}}}}}"}*

```diff
@@ -46,15 +46,15 @@
                     "shared",
                     "on_change"
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "doc": "Title of this block element.",
-                        "name": "value",
+                        "name": "title",
                         "type": "dynamic(str)"
                     },
                     {
                         "default_value": "True",
                         "doc": "If True, the block is expanded, and the content is displayed.<br/>If False, the block is collapsed and its content is hidden.",
                         "name": "expanded",
                         "type": "dynamic(bool)"
```

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/236.taipy-gui.js` & `taipy-gui-3.1.1/taipy/gui/webapp/236.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/236.taipy-gui.js.LICENSE.txt` & `taipy-gui-3.1.1/taipy/gui/webapp/236.taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/294.taipy-gui.js` & `taipy-gui-3.1.1/taipy/gui/webapp/294.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/587.taipy-gui.js` & `taipy-gui-3.1.1/taipy/gui/webapp/587.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/677.taipy-gui-base.js` & `taipy-gui-3.1.1/taipy/gui/webapp/677.taipy-gui-base.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/677.taipy-gui.js` & `taipy-gui-3.1.1/taipy/gui/webapp/677.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/favicon.ico` & `taipy-gui-3.1.1/taipy/gui/webapp/favicon.ico`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/favicon.png` & `taipy-gui-3.1.1/taipy/gui/webapp/favicon.png`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/index.html` & `taipy-gui-3.1.1/taipy/gui/webapp/index.html`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/base/base.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/base/base.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/base/fontfaces.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/base/fontfaces.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/base/typography.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/base/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/blocks/layout.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/blocks/layout.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/button.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/button.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/chart.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/chart.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/date.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/date.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/expandable.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/expandable.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/image.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/image.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/input.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/input.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/navbar.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/navbar.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/number.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/number.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/selector.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/selector.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/slider.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/slider.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/table.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/table.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/controls/toggle.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/controls/toggle.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/elements/card.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/elements/card.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/elements/container.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/elements/container.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/elements/header.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/elements/header.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/elements/sidebar.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/elements/sidebar.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/stylekit.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/stylekit.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/utilities/colors.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/utilities/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/utilities/misc.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/utilities/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/utilities/spacing.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/utilities/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/utilities/typography.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/utilities/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/colors.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/elements.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/elements.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/misc.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/shapes.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/shapes.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/spacing.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/stylekit/variables/typography.css` & `taipy-gui-3.1.1/taipy/gui/webapp/stylekit/variables/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui-base.js` & `taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui-base.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui-deps-manifest.json` & `taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui-deps-manifest.json`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui-deps.dll.js` & `taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui-deps.dll.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt` & `taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui-dom.js` & `taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui-dom.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui.d.ts` & `taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui.d.ts`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui.js` & `taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -17841,16 +17841,19 @@
             As = (0, r.lazy)((() => i.e(236).then(i.bind(i, 1236)))),
             Ss = {
                 position: "relative",
                 display: "inline-block"
             },
             ks = /^(\d+)\/(.*)/,
             Cs = e => {
-                const t = ks.exec(e);
-                return t && t.length > 2 && t[2] || e
+                if (e) {
+                    const t = ks.exec(e);
+                    if (t && t.length > 2) return t[2] || e
+                }
+                return e
             },
             Ts = (e, t, n, r = !1) => {
                 const o = Es(e, wn(t, n));
                 if (!r || o.length) return o
             },
             Es = (e, t) => {
                 if (e && t) {
@@ -17935,34 +17938,35 @@
                     if (i && (w || !c[g])) {
                         const e = Object.values(E.columns).map((e => e.dfid)),
                             t = e.join("-") + (E.decimators ? `--${E.decimators.join("")}` : "");
                         v(t), !w && c[t] || p(Zi(i, l, x, e, t, Ms(E.decimators, m.current, E.modes, E.columns, E.traces)))
                     }
                 }), [w, p, E.columns, E.traces, E.modes, E.decimators, i, l, x]), gs(p, l, x, s);
                 const P = (0, r.useMemo)((() => {
-                        const n = Object.assign({}, T);
-                        let r;
+                        var n, r;
+                        const o = Object.assign({}, T);
+                        let a;
                         try {
                             const t = e.template && JSON.parse(e.template),
                                 n = "dark" === b.palette.mode ? e.template_Dark_ ? JSON.parse(e.template_Dark_) : Ls : e.template_Light_ && JSON.parse(e.template_Light_);
-                            r = t ? n ? Object.assign(Object.assign({}, t), n) : t : n || void 0
+                            a = t ? n ? Object.assign(Object.assign({}, t), n) : t : n || void 0
                         } catch (e) {
                             console.info(`Error while parsing Chart.template\n${e.message||e}`)
                         }
-                        return r && (n.template = r), e.figure ? Object.assign(Object.assign(Object.assign({}, e.figure[0].layout), n), {
-                            title: t || n.title || e.figure[0].layout.title,
+                        return a && (o.template = a), e.figure ? Object.assign(Object.assign(Object.assign({}, e.figure[0].layout), o), {
+                            title: t || o.title || e.figure[0].layout.title,
                             clickmode: "event+select"
-                        }) : Object.assign(Object.assign({}, n), {
-                            title: t || n.title,
+                        }) : Object.assign(Object.assign({}, o), {
+                            title: t || o.title,
                             xaxis: Object.assign({
-                                title: E.traces.length && E.traces[0].length && E.traces[0][0] ? Cs(E.columns[E.traces[0][0]].dfid) : void 0
-                            }, n.xaxis),
+                                title: E.traces.length && E.traces[0].length && E.traces[0][0] ? Cs(null === (n = E.columns[E.traces[0][0]]) || void 0 === n ? void 0 : n.dfid) : void 0
+                            }, o.xaxis),
                             yaxis: Object.assign({
-                                title: 1 == E.traces.length && E.traces[0].length > 1 && E.columns[E.traces[0][1]] ? Cs(E.columns[E.traces[0][1]].dfid) : void 0
-                            }, n.yaxis),
+                                title: 1 == E.traces.length && E.traces[0].length > 1 && E.columns[E.traces[0][1]] ? Cs(null === (r = E.columns[E.traces[0][1]]) || void 0 === r ? void 0 : r.dfid) : void 0
+                            }, o.yaxis),
                             clickmode: "event+select"
                         })
                     }), [b.palette.mode, t, E.columns, E.traces, T, e.template, e.template_Dark_, e.template_Light_, e.figure]),
                     M = (0, r.useMemo)((() => void 0 === a ? Object.assign(Object.assign({}, Ss), {
                         width: o
                     }) : Object.assign(Object.assign({}, Ss), {
                         width: o,
@@ -17977,15 +17981,15 @@
                         const t = c[g];
                         return y.current = t ? E.traces.map(((e, n) => {
                             const r = Object.assign(Object.assign({}, wn(E.options, n, {})), {
                                 type: E.types[n],
                                 mode: E.modes[n],
                                 name: wn(E.names, n) || (E.columns[e[1]] ? Cs(E.columns[e[1]].dfid) : void 0)
                             });
-                            r.marker = wn(E.markers, n, r.marker || {}), Ns.forEach((e => {
+                            r.marker = Object.assign({}, wn(E.markers, n, r.marker || {})), Ns.forEach((e => {
                                 const n = r.marker[e];
                                 if ("string" == typeof n) {
                                     const o = Es(t, n);
                                     o.length && (r.marker[e] = o)
                                 }
                             }));
                             const o = Ts(t, e, 0) || [],
```

### Comparing `taipy-gui-3.1.0/taipy/gui/webapp/taipy-gui.js.LICENSE.txt` & `taipy-gui-3.1.1/taipy/gui/webapp/taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy_gui.egg-info/PKG-INFO` & `taipy-gui-3.1.1/taipy_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-gui
-Version: 3.1.0
+Version: 3.1.1
 Summary: Low-code library to create graphical user interfaces on the Web for your Python applications.
 Home-page: https://github.com/avaiga/taipy-gui
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-gui
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 Requires-Dist: gitignore-parser<=0.1.11,>=0.1
 Requires-Dist: kthread<=0.2.3,>=0.2.3
 Requires-Dist: markdown<=3.5.2,>=3.4.4
 Requires-Dist: pandas<=2.2.0,>=1.3.5
 Requires-Dist: python-dotenv<=1.0.1,>=1.0.0
 Requires-Dist: pytz<=2023.3.post1,>=2021.3
 Requires-Dist: simple-websocket<=1.0.0,>=0.10.1
-Requires-Dist: taipy-config==3.1.0
+Requires-Dist: taipy-config<3.2.0,>=3.1.1
 Requires-Dist: twisted<=23.10.0,>=23.8.0
 Requires-Dist: tzlocal<=5.2,>=3.0
 Provides-Extra: ngrok
 Requires-Dist: pyngrok<6.0,>=5.1; extra == "ngrok"
 Provides-Extra: image
 Requires-Dist: python-magic<0.5,>=0.4.24; platform_system != "Windows" and extra == "image"
 Requires-Dist: python-magic-bin<0.5,>=0.4.14; platform_system == "Windows" and extra == "image"
```

### Comparing `taipy-gui-3.1.0/taipy_gui.egg-info/SOURCES.txt` & `taipy-gui-3.1.1/taipy_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-3.1.0/taipy_gui.egg-info/requires.txt` & `taipy-gui-3.1.1/taipy_gui.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 gitignore-parser<=0.1.11,>=0.1
 kthread<=0.2.3,>=0.2.3
 markdown<=3.5.2,>=3.4.4
 pandas<=2.2.0,>=1.3.5
 python-dotenv<=1.0.1,>=1.0.0
 pytz<=2023.3.post1,>=2021.3
 simple-websocket<=1.0.0,>=0.10.1
-taipy-config==3.1.0
+taipy-config<3.2.0,>=3.1.1
 twisted<=23.10.0,>=23.8.0
 tzlocal<=5.2,>=3.0
 
 [:python_version < "3.9"]
 backports.zoneinfo<=0.2.1,>=0.2.1
 
 [arrow]
```

