# Comparing `tmp/taipy-3.1.0.tar.gz` & `tmp/taipy-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-3.1.0.tar", last modified: Mon Mar  4 15:30:53 2024, max compression
+gzip compressed data, was "taipy-3.1.1.tar", last modified: Mon Apr  8 13:14:44 2024, max compression
```

## Comparing `taipy-3.1.0.tar` & `taipy-3.1.1.tar`

### file list

```diff
@@ -1,232 +1,233 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.767325 taipy-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-04 15:27:14.000000 taipy-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-04 15:27:17.000000 taipy-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9551 2024-03-04 15:30:53.767325 taipy-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-03-04 15:27:14.000000 taipy-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-04 15:27:14.000000 taipy-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 15:30:53.767325 taipy-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-04 15:27:17.000000 taipy-3.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-04 15:27:17.000000 taipy-3.1.0/setup.requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.723325 taipy-3.1.0/taipy/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.727325 taipy-3.1.0/taipy/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.727325 taipy-3.1.0/taipy/_cli/_base_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/_cli/_base_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/_cli/_base_cli/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/_cli/_help_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/_cli/_run_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/_cli/_scaffold_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.727325 taipy-3.1.0/taipy/config/
--rw-r--r--   0 runner    (1001) docker     (127)    42877 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/config/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/config/version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.727325 taipy-3.1.0/taipy/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.727325 taipy-3.1.0/taipy/core/config/
--rw-r--r--   0 runner    (1001) docker     (127)    17261 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/core/config/config.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/core/version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.727325 taipy-3.1.0/taipy/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/gui/version.json
--rw-r--r--   0 runner    (1001) docker     (127)    62608 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/gui/viselements.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.743325 taipy-3.1.0/taipy/gui/webapp/
--rw-r--r--   0 runner    (1001) docker     (127)  3626049 2024-03-04 15:29:49.000000 taipy-3.1.0/taipy/gui/webapp/236.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-04 15:29:49.000000 taipy-3.1.0/taipy/gui/webapp/236.taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   112749 2024-03-04 15:29:49.000000 taipy-3.1.0/taipy/gui/webapp/294.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (127)   207070 2024-03-04 15:29:49.000000 taipy-3.1.0/taipy/gui/webapp/587.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-04 15:28:06.000000 taipy-3.1.0/taipy/gui/webapp/677.taipy-gui-base.js
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-04 15:29:49.000000 taipy-3.1.0/taipy/gui/webapp/677.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.743325 taipy-3.1.0/taipy/gui/webapp/stylekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.743325 taipy-3.1.0/taipy/gui/webapp/stylekit/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/base/base.css
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/base/fontfaces.css
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/base/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.743325 taipy-3.1.0/taipy/gui/webapp/stylekit/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/blocks/layout.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.747325 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/button.css
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/chart.css
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/date.css
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/expandable.css
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/image.css
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/input.css
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/navbar.css
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/number.css
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/selector.css
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/slider.css
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/table.css
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/controls/toggle.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.747325 taipy-3.1.0/taipy/gui/webapp/stylekit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/elements/card.css
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/elements/container.css
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/elements/header.css
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/elements/sidebar.css
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/stylekit.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.747325 taipy-3.1.0/taipy/gui/webapp/stylekit/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/utilities/colors.css
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/utilities/misc.css
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/utilities/spacing.css
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/utilities/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.747325 taipy-3.1.0/taipy/gui/webapp/stylekit/variables/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/variables/colors.css
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/variables/elements.css
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/variables/misc.css
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/variables/shapes.css
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/variables/spacing.css
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/stylekit/variables/typography.css
--rw-r--r--   0 runner    (1001) docker     (127)    47350 2024-03-04 15:28:06.000000 taipy-3.1.0/taipy/gui/webapp/taipy-gui-base.js
--rw-r--r--   0 runner    (1001) docker     (127)   216794 2024-03-04 15:28:37.000000 taipy-3.1.0/taipy/gui/webapp/taipy-gui-deps-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)  4990278 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/taipy-gui-deps.dll.js
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-04 15:28:37.000000 taipy-3.1.0/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/taipy-gui-dom.js
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/taipy-gui.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)  1187368 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-04 15:29:49.000000 taipy-3.1.0/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-04 15:30:11.000000 taipy-3.1.0/taipy/gui/webapp/taipy.status.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.751325 taipy-3.1.0/taipy/gui_core/
--rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/gui_core/_GuiCoreLib.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/gui_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/gui_core/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)    42617 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/gui_core/_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/gui_core/_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.751325 taipy-3.1.0/taipy/gui_core/lib/
--rw-r--r--   0 runner    (1001) docker     (127)   889349 2024-03-04 15:30:51.000000 taipy-3.1.0/taipy/gui_core/lib/taipy-gui-core.js
--rw-r--r--   0 runner    (1001) docker     (127)    22589 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/gui_core/viselements.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.751325 taipy-3.1.0/taipy/rest/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/rest/version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.751325 taipy-3.1.0/taipy/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.751325 taipy-3.1.0/taipy/templates/default/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.755325 taipy-3.1.0/taipy/templates/default/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/hooks/post_gen_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/hooks/pre_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.755325 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.755325 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.755325 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.755325 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.755325 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/page_example.md
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/page_example.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/root.md
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/root.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.755325 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/import.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/main.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/page_content.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.755325 taipy-3.1.0/taipy/templates/scenario-management/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.755325 taipy-3.1.0/taipy/templates/scenario-management/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/hooks/post_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.755325 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/.taipyignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.755325 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/algos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.759325 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config_with_toml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.759325 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.759325 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/job_page.md
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/job_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/root.md
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.759325 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/data_node_management.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/scenario_page.md
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/scenario_page.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/templates/version.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/version.json
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-04 15:27:14.000000 taipy-3.1.0/taipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.767325 taipy-3.1.0/taipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9551 2024-03-04 15:30:53.000000 taipy-3.1.0/taipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-03-04 15:30:53.000000 taipy-3.1.0/taipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:30:53.000000 taipy-3.1.0/taipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-04 15:30:53.000000 taipy-3.1.0/taipy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:30:51.000000 taipy-3.1.0/taipy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-04 15:30:53.000000 taipy-3.1.0/taipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 15:30:53.000000 taipy-3.1.0/taipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.759325 taipy-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-04 15:27:14.000000 taipy-3.1.0/tests/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.759325 taipy-3.1.0/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.759325 taipy-3.1.0/tools/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/frontend/bundle_build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.759325 taipy-3.1.0/tools/gui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.759325 taipy-3.1.0/tools/gui/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/gui/builder/block.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/gui/builder/control.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.723325 taipy-3.1.0/tools/gui/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.759325 taipy-3.1.0/tools/gui/docker/nginx-prefix/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/gui/docker/nginx-prefix/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/gui/docker/nginx-prefix/default.conf
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/gui/generate_pyi.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/modify_readme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.763325 taipy-3.1.0/tools/packages/
--rw-r--r--   0 runner    (1001) docker     (127)    16056 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/check-dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/check-dependencies.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.763325 taipy-3.1.0/tools/packages/pipfiles/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/pipfiles/Pipfile3.10.max
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/pipfiles/Pipfile3.11.max
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/pipfiles/Pipfile3.12.max
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/pipfiles/Pipfile3.8.max
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/pipfiles/Pipfile3.9.max
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.763325 taipy-3.1.0/tools/packages/taipy/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy/setup.requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.763325 taipy-3.1.0/tools/packages/taipy-config/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-config/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-config/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-config/setup.requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.763325 taipy-3.1.0/tools/packages/taipy-core/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-core/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-core/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-core/setup.requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.763325 taipy-3.1.0/tools/packages/taipy-gui/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-gui/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-gui/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-gui/setup.requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.763325 taipy-3.1.0/tools/packages/taipy-rest/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-rest/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-rest/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-rest/setup.requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.763325 taipy-3.1.0/tools/packages/taipy-templates/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-templates/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-templates/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/packages/taipy-templates/setup.requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:30:53.767325 taipy-3.1.0/tools/release/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/release/build_package_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/release/check_releases.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/release/extract_from_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/release/setup_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/release/update_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/release/update_setup_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-04 15:27:14.000000 taipy-3.1.0/tools/validate_taipy_install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.376420 taipy-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 13:10:52.000000 taipy-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-08 13:10:58.000000 taipy-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-04-08 13:14:44.376420 taipy-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-08 13:10:52.000000 taipy-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-08 13:10:52.000000 taipy-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:14:44.376420 taipy-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-08 13:10:58.000000 taipy-3.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 13:10:58.000000 taipy-3.1.1/setup.requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.332420 taipy-3.1.1/taipy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.336420 taipy-3.1.1/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.336420 taipy-3.1.1/taipy/_cli/_base_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/_cli/_base_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/_cli/_base_cli/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/_cli/_help_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/_cli/_run_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/_cli/_scaffold_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.336420 taipy-3.1.1/taipy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    45678 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/config/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/config/version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.336420 taipy-3.1.1/taipy/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.336420 taipy-3.1.1/taipy/core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    17261 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/core/config/config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/core/version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.336420 taipy-3.1.1/taipy/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/gui/version.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62608 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/gui/viselements.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.352420 taipy-3.1.1/taipy/gui/webapp/
+-rw-r--r--   0 runner    (1001) docker     (127)  3626049 2024-04-08 13:13:37.000000 taipy-3.1.1/taipy/gui/webapp/236.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-08 13:13:37.000000 taipy-3.1.1/taipy/gui/webapp/236.taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   112749 2024-04-08 13:13:37.000000 taipy-3.1.1/taipy/gui/webapp/294.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (127)   207070 2024-04-08 13:13:37.000000 taipy-3.1.1/taipy/gui/webapp/587.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-08 13:11:48.000000 taipy-3.1.1/taipy/gui/webapp/677.taipy-gui-base.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-08 13:13:37.000000 taipy-3.1.1/taipy/gui/webapp/677.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.352420 taipy-3.1.1/taipy/gui/webapp/stylekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.352420 taipy-3.1.1/taipy/gui/webapp/stylekit/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/base/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/base/fontfaces.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/base/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.352420 taipy-3.1.1/taipy/gui/webapp/stylekit/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/blocks/layout.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.356420 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/button.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/chart.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/date.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/expandable.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/image.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/input.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/navbar.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/number.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/selector.css
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/slider.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/table.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/controls/toggle.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.356420 taipy-3.1.1/taipy/gui/webapp/stylekit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/elements/card.css
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/elements/container.css
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/elements/header.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/elements/sidebar.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/stylekit.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.356420 taipy-3.1.1/taipy/gui/webapp/stylekit/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/utilities/colors.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/utilities/misc.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/utilities/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/utilities/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.356420 taipy-3.1.1/taipy/gui/webapp/stylekit/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/variables/colors.css
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/variables/elements.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/variables/misc.css
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/variables/shapes.css
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/variables/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/stylekit/variables/typography.css
+-rw-r--r--   0 runner    (1001) docker     (127)    47350 2024-04-08 13:11:48.000000 taipy-3.1.1/taipy/gui/webapp/taipy-gui-base.js
+-rw-r--r--   0 runner    (1001) docker     (127)   216794 2024-04-08 13:12:20.000000 taipy-3.1.1/taipy/gui/webapp/taipy-gui-deps-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)  4990278 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/taipy-gui-deps.dll.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-08 13:12:20.000000 taipy-3.1.1/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/taipy-gui-dom.js
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/taipy-gui.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)  1187475 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-08 13:13:37.000000 taipy-3.1.1/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 13:14:00.000000 taipy-3.1.1/taipy/gui/webapp/taipy.status.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.360420 taipy-3.1.1/taipy/gui_core/
+-rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/gui_core/_GuiCoreLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/gui_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/gui_core/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42617 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/gui_core/_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/gui_core/_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.360420 taipy-3.1.1/taipy/gui_core/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)   889402 2024-04-08 13:14:41.000000 taipy-3.1.1/taipy/gui_core/lib/taipy-gui-core.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22589 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/gui_core/viselements.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.360420 taipy-3.1.1/taipy/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/rest/version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.360420 taipy-3.1.1/taipy/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.364420 taipy-3.1.1/taipy/templates/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.364420 taipy-3.1.1/taipy/templates/default/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/hooks/post_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/hooks/pre_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.364420 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.364420 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.364420 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.364420 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.364420 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/page_example.md
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/page_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/root.md
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.364420 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/import.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/main.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/page_content.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.364420 taipy-3.1.1/taipy/templates/scenario-management/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.364420 taipy-3.1.1/taipy/templates/scenario-management/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/hooks/post_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.364420 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/.taipyignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.368420 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.368420 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config_with_toml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.368420 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.368420 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/job_page.md
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/job_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/root.md
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.368420 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/data_node_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/scenario_page.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/scenario_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/templates/version.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/version.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-08 13:10:52.000000 taipy-3.1.1/taipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.376420 taipy-3.1.1/taipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-04-08 13:14:44.000000 taipy-3.1.1/taipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-08 13:14:44.000000 taipy-3.1.1/taipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:14:44.000000 taipy-3.1.1/taipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 13:14:44.000000 taipy-3.1.1/taipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:14:41.000000 taipy-3.1.1/taipy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 13:14:44.000000 taipy-3.1.1/taipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 13:14:44.000000 taipy-3.1.1/taipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.368420 taipy-3.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-08 13:10:52.000000 taipy-3.1.1/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.368420 taipy-3.1.1/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.368420 taipy-3.1.1/tools/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/frontend/bundle_build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.368420 taipy-3.1.1/tools/gui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.368420 taipy-3.1.1/tools/gui/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/gui/builder/block.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/gui/builder/control.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.328420 taipy-3.1.1/tools/gui/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.372420 taipy-3.1.1/tools/gui/docker/nginx-prefix/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/gui/docker/nginx-prefix/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/gui/docker/nginx-prefix/default.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/gui/generate_pyi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/modify_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.372420 taipy-3.1.1/tools/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)    16056 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/check-dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/check-dependencies.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.372420 taipy-3.1.1/tools/packages/pipfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/pipfiles/Pipfile3.10.max
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/pipfiles/Pipfile3.11.max
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/pipfiles/Pipfile3.12.max
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/pipfiles/Pipfile3.8.max
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/pipfiles/Pipfile3.9.max
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.372420 taipy-3.1.1/tools/packages/taipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy/setup.requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.372420 taipy-3.1.1/tools/packages/taipy-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-config/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-config/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-config/setup.requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.372420 taipy-3.1.1/tools/packages/taipy-core/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-core/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-core/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-core/setup.requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.372420 taipy-3.1.1/tools/packages/taipy-gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-gui/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-gui/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-gui/setup.requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.372420 taipy-3.1.1/tools/packages/taipy-rest/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-rest/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-rest/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-rest/setup.requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.376420 taipy-3.1.1/tools/packages/taipy-templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-templates/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-templates/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/packages/taipy-templates/setup.requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:44.376420 taipy-3.1.1/tools/release/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/release/build_package_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/release/check_releases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/release/extract_from_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/release/fetch_latest_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/release/setup_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/release/update_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/release/update_setup_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-08 13:10:52.000000 taipy-3.1.1/tools/validate_taipy_install.py
```

### Comparing `taipy-3.1.0/LICENSE` & `taipy-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/MANIFEST.in` & `taipy-3.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/PKG-INFO` & `taipy-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 3.1.0
+Version: 3.1.1
 Summary: A 360° open-source platform from Python pilots to production-ready web apps.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
@@ -17,17 +17,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: backports.zoneinfo<=0.2.1,>=0.2.1; python_version < "3.9"
 Requires-Dist: cookiecutter<=2.5.0,>=2.1.1
-Requires-Dist: taipy-gui==3.1.0
-Requires-Dist: taipy-rest==3.1.0
-Requires-Dist: taipy-templates==3.1.0
+Requires-Dist: taipy-gui<3.2.0,>=3.1.1
+Requires-Dist: taipy-rest<3.2.0,>=3.1.1
+Requires-Dist: taipy-templates<3.2.0,>=3.1.1
 Provides-Extra: ngrok
 Requires-Dist: pyngrok<6.0,>=5.1; extra == "ngrok"
 Provides-Extra: image
 Requires-Dist: python-magic<0.5,>=0.4.24; platform_system != "Windows" and extra == "image"
 Requires-Dist: python-magic-bin<0.5,>=0.4.14; platform_system == "Windows" and extra == "image"
 Provides-Extra: rdp
 Requires-Dist: rdp>=0.8; extra == "rdp"
```

### Comparing `taipy-3.1.0/README.md` & `taipy-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/pyproject.toml` & `taipy-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/setup.py` & `taipy-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/__init__.py` & `taipy-3.1.1/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/_cli/__init__.py` & `taipy-3.1.1/taipy/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/_cli/_base_cli/__init__.py` & `taipy-3.1.1/taipy/_cli/_base_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/_cli/_base_cli/_cli.py` & `taipy-3.1.1/taipy/_cli/_base_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/_cli/_help_cli.py` & `taipy-3.1.1/taipy/_cli/_help_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/_cli/_run_cli.py` & `taipy-3.1.1/taipy/_cli/_run_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/_cli/_scaffold_cli.py` & `taipy-3.1.1/taipy/_cli/_scaffold_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/_entrypoint.py` & `taipy-3.1.1/taipy/_entrypoint.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/_run.py` & `taipy-3.1.1/taipy/_run.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/config/config.pyi` & `taipy-3.1.1/taipy/config/config.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,47 +23,51 @@
 from .common.scope import Scope
 from .global_app.global_app_config import GlobalAppConfig
 from .section import Section
 from .unique_section import UniqueSection
 
 class Config:
     """Configuration singleton."""
-
     @_Classproperty
     def unique_sections(cls) -> Dict[str, UniqueSection]:
         """Return all unique sections."""
+
     @_Classproperty
     def sections(cls) -> Dict[str, Dict[str, Section]]:
         """Return all non unique sections."""
+
     @_Classproperty
     def global_config(cls) -> GlobalAppConfig:
         """Return configuration values related to the global application as a `GlobalAppConfig^`."""
+
     @classmethod
     @_ConfigBlocker._check()
     def load(cls, filename):
         """Load a configuration file.
 
         The current Python configuration is replaced and the Config compilation is triggered.
 
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
+
     @classmethod
     def export(cls, filename):
         """Export a configuration.
 
         The export is done in a toml file.
 
         The exported configuration is taken from the Python code configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the file to export.
         Note:
             If *filename* already exists, it is overwritten.
         """
+
     @classmethod
     def backup(cls, filename):
         """Backup a configuration.
 
         The backup is done in a toml file.
 
         The backed up configuration is a compilation from the three possible methods to configure
@@ -71,93 +75,112 @@
         configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the file to export.
         Note:
             If *filename* already exists, it is overwritten.
         """
+
     @classmethod
     @_ConfigBlocker._check()
     def restore(cls, filename):
         """Restore a configuration file and replace the current applied configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
+
     @classmethod
     @_ConfigBlocker._check()
     def override(cls, filename):
         """Load a configuration from a file and overrides the current config.
 
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
+
     @classmethod
     def block_update(cls):
         """Block update on the configuration signgleton."""
+
     @classmethod
     def unblock_update(cls):
         """Unblock update on the configuration signgleton."""
+
     @classmethod
     @_ConfigBlocker._check()
     def configure_global_app(cls, **properties) -> GlobalAppConfig:
         """Configure the global application.
 
         Parameters:
             **properties (Dict[str, Any]): A dictionary of additional properties.
         Returns:
             The global application configuration.
         """
+
     @classmethod
     def check(cls) -> IssueCollector:
         """Check configuration.
 
         This method logs issue messages and returns an issue collector.
 
         Returns:
             Collector containing the info, warning and error issues.
         """
+
     @classmethod
     @_ConfigBlocker._check()
     def _register_default(cls, default_section: Section):
         """"""
+
     @classmethod
     @_ConfigBlocker._check()
     def _register(cls, section):
         """"""
+
     @classmethod
     def _override_env_file(cls):
         """"""
+
     @classmethod
     def _compile_configs(cls):
         """"""
+
     @classmethod
     def _to_json(cls, _config: _Config) -> str:
         """"""
+
     @classmethod
     def _from_json(cls, config_as_str: str) -> _Config:
         """"""
+
     @_Classproperty
     def job_config(cls) -> JobConfig:
         """"""
+
     @_Classproperty
     def data_nodes(cls) -> Dict[str, DataNodeConfig]:
         """"""
+
     @_Classproperty
     def tasks(cls) -> Dict[str, TaskConfig]:
         """"""
+
     @_Classproperty
     def scenarios(cls) -> Dict[str, ScenarioConfig]:
         """"""
+
     @_Classproperty
     def migration_functions(cls) -> Dict[str, MigrationConfig]:
         """"""
+
     @_Classproperty
     def core(cls) -> Dict[str, CoreSection]:
         """"""
+
     @staticmethod
     def configure_scenario(
         id: str,
         task_configs: Optional[List[TaskConfig]] = None,
         additional_data_node_configs: Optional[List[DataNodeConfig]] = None,
         frequency: Optional[Frequency] = None,
         comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
@@ -186,14 +209,15 @@
             sequences (Optional[Dict[str, List[TaskConfig]]]): Dictionary of sequence descriptions.
                 The default value is None.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new scenario configuration.
         """
+
     @staticmethod
     def set_default_scenario_configuration(
         task_configs: Optional[List[TaskConfig]] = None,
         additional_data_node_configs: List[DataNodeConfig] = None,
         frequency: Optional[Frequency] = None,
         comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
         sequences: Optional[Dict[str, List[TaskConfig]]] = None,
@@ -223,41 +247,43 @@
                 `taipy.compare_scenarios()^` more more details.
             sequences (Optional[Dict[str, List[TaskConfig]]]): Dictionary of sequences. The default value is None.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new default scenario configuration.
         """
+
     @staticmethod
     def set_default_data_node_configuration(
         storage_type: str, scope: Optional[Scope] = None, validity_period: Optional[timedelta] = None, **properties
     ) -> "DataNodeConfig":
         """Set the default values for data node configurations.
 
         This function creates the _default data node configuration_ object,
         where all data node configuration objects will find their default
         values when needed.
 
         Parameters:
             storage_type (str): The default storage type for all data node configurations.
                 The possible values are *"pickle"* (the default value), *"csv"*, *"excel"*,
-                *"sql"*, *"mongo_collection"*, *"in_memory"*, *"json"*, *"parquet"* or
-                *"generic"*.
+                *"sql"*, *"mongo_collection"*, *"in_memory"*, *"json"*, *"parquet"*, *"generic"*,
+                or *"s3_object"*.
             scope (Optional[Scope^]): The default scope for all data node configurations.<br/>
                 The default value is `Scope.SCENARIO`.
             validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
                 considered up-to-date. Once the validity period has passed, the data node is considered stale and
                 relevant tasks will run even if they are skippable (see the
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The default data node configuration.
         """
+
     @classmethod
     def configure_data_node_from(
         cls,
         source_configuration: "DataNodeConfig",
         id: str,
         **properties,
     ) -> "DataNodeConfig":
@@ -268,14 +294,15 @@
             id (str): The unique identifier of the new data node configuration.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.<br/>
                 The default properties are the properties of the source data node configuration.
 
         Returns:
             The new data node configuration.
         """
+
     @classmethod
     def configure_data_node(
         cls,
         id: str,
         storage_type: Optional[str] = None,
         scope: Optional[Scope] = None,
         validity_period: Optional[timedelta] = None,
@@ -300,14 +327,15 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new data node configuration.
         """
+
     @classmethod
     def configure_csv_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         encoding: Optional[str] = None,
         has_header: Optional[bool] = None,
@@ -333,14 +361,15 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new CSV data node configuration.
         """
+
     @classmethod
     def configure_json_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         encoding: Optional[str] = None,
         encoder: Optional[json.JSONEncoder] = None,
@@ -364,14 +393,15 @@
                 relevant tasks will run even if they are skippable (see the
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The new JSON data node configuration.
         """
+
     @classmethod
     def configure_parquet_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         engine: Optional[str] = None,
         compression: Optional[str] = None,
@@ -408,14 +438,15 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new Parquet data node configuration.
         """
+
     @classmethod
     def configure_excel_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         has_header: Optional[bool] = None,
         sheet_name: Optional[Union[List[str], str]] = None,
@@ -442,14 +473,15 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new Excel data node configuration.
         """
+
     @classmethod
     def configure_generic_data_node(
         cls,
         id: str,
         read_fct: Optional[Callable] = None,
         write_fct: Optional[Callable] = None,
         read_fct_args: Optional[List] = None,
@@ -476,14 +508,15 @@
                 relevant tasks will run even if they are skippable (see the
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The new Generic data node configuration.
         """
+
     @classmethod
     def configure_in_memory_data_node(
         cls,
         id: str,
         default_data: Optional[Any] = None,
         scope: Optional[Scope] = None,
         validity_period: Optional[timedelta] = None,
@@ -503,14 +536,15 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new *in-memory* data node configuration.
         """
+
     @classmethod
     def configure_pickle_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         default_data: Optional[Any] = None,
         scope: Optional[Scope] = None,
@@ -532,14 +566,15 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new pickle data node configuration.
         """
+
     @classmethod
     def configure_sql_table_data_node(
         cls,
         id: str,
         db_name: str,
         db_engine: str,
         table_name: str,
@@ -589,22 +624,24 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new SQL data node configuration.
         """
+
     @classmethod
     def configure_sql_data_node(
         cls,
         id: str,
         db_name: str,
         db_engine: str,
         read_query: str,
         write_query_builder: Callable,
+        append_query_builder: Optional[Callable] = None,
         db_username: Optional[str] = None,
         db_password: Optional[str] = None,
         db_host: Optional[str] = None,
         db_port: Optional[int] = None,
         db_driver: Optional[str] = None,
         sqlite_folder_path: Optional[str] = None,
         sqlite_file_extension: Optional[str] = None,
@@ -619,15 +656,17 @@
         Parameters:
             id (str): The unique identifier of the new SQL data node configuration.
             db_name (str): The database name, or the name of the SQLite database file.
             db_engine (str): The database engine. Possible values are *"sqlite"*, *"mssql"*, *"mysql"*,
                 or *"postgresql"*.
             read_query (str): The SQL query string used to read the data from the database.
             write_query_builder (Callable): A callback function that takes the data as an input parameter
-                and returns a list of SQL queries.
+                and returns a list of SQL queries to be executed when writing data to the data node.
+            append_query_builder (Optional[Callable]): A callback function that takes the data as an input parameter
+                and returns a list of SQL queries to be executed when appending data to the data node.
             db_username (Optional[str]): The database username. Required by the *"mssql"*, *"mysql"*, and
                 *"postgresql"* engines.
             db_password (Optional[str]): The database password. Required by the *"mssql"*, *"mysql"*, and
                 *"postgresql"* engines.
             db_host (Optional[str]): The database host.<br/>
                 The default value is "localhost".
             db_port (Optional[int]): The database port.<br/>
@@ -648,14 +687,15 @@
                 relevant tasks will run even if they are skippable (see the
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The new SQL data node configuration.
         """
+
     @classmethod
     def configure_mongo_collection_data_node(
         cls,
         id: str,
         db_name: str,
         collection_name: str,
         custom_document: Optional[Any] = None,
@@ -697,14 +737,53 @@
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new Mongo collection data node configuration.
         """
+
+    @classmethod
+    def configure_s3_object_data_node(
+        cls,
+        id: str,
+        aws_access_key: str,
+        aws_secret_access_key: str,
+        aws_s3_bucket_name: str,
+        aws_s3_object_key: str,
+        aws_region: Optional[str] = None,
+        aws_s3_object_parameters: Optional[Dict[str, Any]] = None,
+        scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
+        **properties,
+    ) -> "DataNodeConfig":
+        """Configure a new S3 object data node configuration.
+
+        Parameters:
+            id (str): The unique identifier of the new S3 Object data node configuration.
+            aws_access_key (str): Amazon Web Services ID for to identify account.
+            aws_secret_access_key (str): Amazon Web Services access key to authenticate programmatic requests.
+            aws_s3_bucket_name (str): The bucket in S3 to read from and to write the data to.
+            aws_region (Optional[str]): Self-contained geographic area where Amazon Web Services (AWS)
+                infrastructure is located.
+            aws_s3_object_parameters (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
+                into AWS S3 bucket access string.
+            scope (Optional[Scope^]): The scope of the S3 Object data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
+        Returns:
+            The new S3 object data node configuration.
+        """
+
     @staticmethod
     def configure_task(
         id: str,
         function,
         input: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         output: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         skippable: Optional[bool] = False,
@@ -725,14 +804,15 @@
                 been made on inputs.<br/>
                 The default value is False.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new task configuration.
         """
+
     @staticmethod
     def set_default_task_configuration(
         function,
         input: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         output: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         skippable: Optional[bool] = False,
         **properties,
@@ -755,14 +835,15 @@
                 been made on inputs.<br/>
                 The default value is False.
             **properties (dict[str, any]): A keyworded variable length list of additional
                 arguments.
         Returns:
             The default task configuration.
         """
+
     @staticmethod
     def configure_job_executions(
         mode: Optional[str] = None, max_nb_of_workers: Optional[Union[int, str]] = None, **properties
     ) -> "JobConfig":
         """Configure job execution.
 
         Parameters:
@@ -775,14 +856,15 @@
                 variable. The string must follow the pattern: `ENV[&lt;env_var&gt;]` where
                 `&lt;env_var&gt;` is the name of an environment variable.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new job execution configuration.
         """
+
     @staticmethod
     def add_migration_function(
         target_version: str,
         config: Union[Section, str],
         migration_fct: Callable,
         **properties,
     ):
@@ -793,34 +875,39 @@
             config (Union[Section, str]): The configuration or the `id` of the config that needs to migrate.
             migration_fct (Callable): Migration function that takes an entity as input and returns a new entity
                 that is compatible with the target production version.
             **properties (Dict[str, Any]): A keyworded variable length list of additional arguments.
         Returns:
             `MigrationConfig^`: The Migration configuration.
         """
+
     @staticmethod
     def configure_core(
         root_folder: Optional[str] = None,
         storage_folder: Optional[str] = None,
+        taipy_storage_folder: Optional[str] = None,
         repository_type: Optional[str] = None,
         repository_properties: Optional[Dict[str, Union[str, int]]] = None,
         read_entity_retry: Optional[int] = None,
         mode: Optional[str] = None,
         version_number: Optional[str] = None,
         force: Optional[bool] = None,
         **properties,
     ) -> "CoreSection":
         """Configure the Core service.
 
         Parameters:
             root_folder (Optional[str]): Path of the base folder for the taipy application.
                 The default value is "./taipy/"
-            storage_folder (Optional[str]): Folder name used to store Taipy data. The default value is ".data/".
-                It is used in conjunction with the `root_folder` field. That means the storage path is
-                <root_folder><storage_folder> (The default path is "./taipy/.data/").
+            storage_folder (str): Folder name used to store user data. The default value is "user_data/". It is used in
+                conjunction with the *root_folder* attribute. That means the storage path is
+                <root_folder><storage_folder> (The default path is "./taipy/user_data/").
+            taipy_storage_folder (str): Folder name used to store Taipy data. The default value is ".taipy/". It is
+                used in conjunction with the *root_folder* attribute. That means the storage path is
+                <root_folder><storage_folder> (The default path is "./taipy/.taipy/").
             repository_type (Optional[str]): The type of the repository to be used to store Taipy data.
                 The default value is "filesystem".
             repository_properties (Optional[Dict[str, Union[str, int]]]): A dictionary of additional properties
                 to be used by the repository.
             read_entity_retry (Optional[int]): Number of retries to read an entity from the repository
                 before return failure. The default value is 3.
             mode (Optional[str]): Indicates the mode of the version management system.
```

### Comparing `taipy-3.1.0/taipy/core/config/config.schema.json` & `taipy-3.1.1/taipy/core/config/config.schema.json`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/viselements.json` & `taipy-3.1.1/taipy/gui/viselements.json`

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

### Comparing `taipy-3.1.0/taipy/gui/webapp/236.taipy-gui.js` & `taipy-3.1.1/taipy/gui/webapp/236.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/236.taipy-gui.js.LICENSE.txt` & `taipy-3.1.1/taipy/gui/webapp/236.taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/294.taipy-gui.js` & `taipy-3.1.1/taipy/gui/webapp/294.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/587.taipy-gui.js` & `taipy-3.1.1/taipy/gui/webapp/587.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/677.taipy-gui-base.js` & `taipy-3.1.1/taipy/gui/webapp/677.taipy-gui-base.js`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/677.taipy-gui.js` & `taipy-3.1.1/taipy/gui/webapp/677.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/favicon.ico` & `taipy-3.1.1/taipy/gui/webapp/favicon.ico`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/favicon.png` & `taipy-3.1.1/taipy/gui/webapp/favicon.png`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/index.html` & `taipy-3.1.1/taipy/gui/webapp/index.html`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/base/base.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/base/base.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/base/fontfaces.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/base/fontfaces.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/base/typography.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/base/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/blocks/layout.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/blocks/layout.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/controls/button.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/controls/button.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/controls/chart.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/controls/chart.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/controls/date.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/controls/date.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/controls/expandable.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/controls/expandable.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/controls/image.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/controls/image.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/controls/input.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/controls/input.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/controls/navbar.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/controls/navbar.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/controls/number.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/controls/number.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/controls/selector.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/controls/selector.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/controls/slider.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/controls/slider.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/controls/table.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/controls/table.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/controls/toggle.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/controls/toggle.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/elements/card.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/elements/card.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/elements/container.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/elements/container.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/elements/header.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/elements/header.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/elements/sidebar.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/elements/sidebar.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/stylekit.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/stylekit.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/utilities/colors.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/utilities/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/utilities/misc.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/utilities/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/utilities/spacing.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/utilities/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/utilities/typography.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/utilities/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/variables/colors.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/variables/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/variables/elements.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/variables/elements.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/variables/misc.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/variables/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/variables/shapes.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/variables/shapes.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/variables/spacing.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/variables/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/stylekit/variables/typography.css` & `taipy-3.1.1/taipy/gui/webapp/stylekit/variables/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/taipy-gui-base.js` & `taipy-3.1.1/taipy/gui/webapp/taipy-gui-base.js`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/taipy-gui-deps-manifest.json` & `taipy-3.1.1/taipy/gui/webapp/taipy-gui-deps-manifest.json`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/taipy-gui-deps.dll.js` & `taipy-3.1.1/taipy/gui/webapp/taipy-gui-deps.dll.js`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt` & `taipy-3.1.1/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/taipy-gui-dom.js` & `taipy-3.1.1/taipy/gui/webapp/taipy-gui-dom.js`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/taipy-gui.d.ts` & `taipy-3.1.1/taipy/gui/webapp/taipy-gui.d.ts`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui/webapp/taipy-gui.js` & `taipy-3.1.1/taipy/gui/webapp/taipy-gui.js`

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

### Comparing `taipy-3.1.0/taipy/gui/webapp/taipy-gui.js.LICENSE.txt` & `taipy-3.1.1/taipy/gui/webapp/taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui_core/_GuiCoreLib.py` & `taipy-3.1.1/taipy/gui_core/_GuiCoreLib.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui_core/__init__.py` & `taipy-3.1.1/taipy/gui_core/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui_core/_adapters.py` & `taipy-3.1.1/taipy/gui_core/_adapters.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui_core/_context.py` & `taipy-3.1.1/taipy/gui_core/_context.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui_core/_init.py` & `taipy-3.1.1/taipy/gui_core/_init.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/gui_core/lib/taipy-gui-core.js` & `taipy-3.1.1/taipy/gui_core/lib/taipy-gui-core.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -44282,17 +44282,17 @@
                     const r = (e || HE)[_E.id],
                         o = t[_E.id] !== r;
                     return t[_E.id] && o && x.current && g((0, fp.createSendActionNameAction)(i, v, n.onLock, {
                         id: t[_E.id],
                         lock: !1
                     })), e && !o || V(f ? YE.Data : YE.Properties), e ? (x.current = e[_E.editInProgress], Y((e => !(!e || o || z != YE.History || (g((0, fp.createSendActionNameAction)(i, v, n.onIdSelect, {
                         history_id: r
-                    })), 0)))), q((e => o ? !(!e || z != YE.Data || (g((0, fp.createSendActionNameAction)(i, v, n.onIdSelect, {
+                    })), 0)))), q((() => z == YE.Data && (g((0, fp.createSendActionNameAction)(i, v, n.onIdSelect, {
                         data_id: r
-                    })), 0)) : e)), mb()(t, e) ? t : e) : HE
+                    })), !0))), mb()(t, e) ? t : e) : HE
                 }))
             }), [n.dataNode, n.defaultDataNode, f, i, g, v, n.onLock, n.onIdSelect]), (0, t.useEffect)((() => () => {
                 T && x.current && g((0, fp.createSendActionNameAction)(i, v, n.onLock, {
                     id: T,
                     lock: !1
                 }))
             }), [T, i, g, v, n.onLock]);
@@ -44755,15 +44755,15 @@
                                                             sx: ff,
                                                             children: (0, e.jsx)(Si.Cancel, {
                                                                 color: "inherit"
                                                             })
                                                         })
                                                     })]
                                                 })]
-                                            }) : "date" == fe ? (0, e.jsxs)(aS, {
+                                            }) : "date" == fe && (null === be || be instanceof Date) ? (0, e.jsxs)(aS, {
                                                 dateAdapter: Ul,
                                                 children: [(0, e.jsx)(wt, {
                                                     item: !0,
                                                     xs: 10,
                                                     children: (0, e.jsx)(eE, {
                                                         value: be,
                                                         onChange: Ce,
@@ -44847,15 +44847,15 @@
                                                 xs: 8,
                                                 children: "boolean" == typeof me ? (0, e.jsx)(Am, {
                                                     defaultChecked: me,
                                                     disabled: !0,
                                                     title: `${me}`
                                                 }) : (0, e.jsx)(Re, {
                                                     variant: "subtitle2",
-                                                    children: "date" == fe ? be && Va(be, "yyyy/MM/dd HH:mm:ss") : "float" == fe && null === me ? "NaN" : me
+                                                    children: "date" == fe ? (null === be || be instanceof Date) && Va(be, "yyyy/MM/dd HH:mm:ss") : "float" == fe && null === me ? "NaN" : me
                                                 })
                                             })]
                                         })
                                     })
                                 }) : ve ? (0, e.jsx)(Re, {
                                     children: ve
                                 }) : ge ? (0, e.jsx)(e.Fragment, {
```

### Comparing `taipy-3.1.0/taipy/gui_core/viselements.json` & `taipy-3.1.1/taipy/gui_core/viselements.json`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/CODE_OF_CONDUCT.md` & `taipy-3.1.1/taipy/templates/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/CONTRIBUTING.md` & `taipy-3.1.1/taipy/templates/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/LICENSE` & `taipy-3.1.1/taipy/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/README.md` & `taipy-3.1.1/taipy/templates/README.md`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/default/cookiecutter.json` & `taipy-3.1.1/taipy/templates/default/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/default/hooks/post_gen_project.py` & `taipy-3.1.1/taipy/templates/default/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/default/hooks/pre_gen_project.py` & `taipy-3.1.1/taipy/templates/default/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/__init__.py` & `taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/algorithms.py` & `taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/algorithms.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/__init__.py` & `taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/config.py` & `taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/config.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/__init__.py` & `taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/page_example.py` & `taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/page_example.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/root.py` & `taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/root.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py` & `taipy-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/cookiecutter.json` & `taipy-3.1.1/taipy/templates/scenario-management/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/hooks/post_gen_project.py` & `taipy-3.1.1/taipy/templates/scenario-management/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/__init__.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/algos.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/algos.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/__init__.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.toml` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.toml`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config_with_toml.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config_with_toml.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/__init__.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/__init__.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/job_page.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/job_page.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/root.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/root.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/__init__.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/data_node_management.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/data_node_management.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/scenario_page.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/scenario_page.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py` & `taipy-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/templates/setup.py` & `taipy-3.1.1/taipy/templates/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy/version.py` & `taipy-3.1.1/taipy/version.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/taipy.egg-info/PKG-INFO` & `taipy-3.1.1/taipy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 3.1.0
+Version: 3.1.1
 Summary: A 360° open-source platform from Python pilots to production-ready web apps.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
@@ -17,17 +17,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: backports.zoneinfo<=0.2.1,>=0.2.1; python_version < "3.9"
 Requires-Dist: cookiecutter<=2.5.0,>=2.1.1
-Requires-Dist: taipy-gui==3.1.0
-Requires-Dist: taipy-rest==3.1.0
-Requires-Dist: taipy-templates==3.1.0
+Requires-Dist: taipy-gui<3.2.0,>=3.1.1
+Requires-Dist: taipy-rest<3.2.0,>=3.1.1
+Requires-Dist: taipy-templates<3.2.0,>=3.1.1
 Provides-Extra: ngrok
 Requires-Dist: pyngrok<6.0,>=5.1; extra == "ngrok"
 Provides-Extra: image
 Requires-Dist: python-magic<0.5,>=0.4.24; platform_system != "Windows" and extra == "image"
 Requires-Dist: python-magic-bin<0.5,>=0.4.14; platform_system == "Windows" and extra == "image"
 Provides-Extra: rdp
 Requires-Dist: rdp>=0.8; extra == "rdp"
```

### Comparing `taipy-3.1.0/taipy.egg-info/SOURCES.txt` & `taipy-3.1.1/taipy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -168,10 +168,11 @@
 tools/packages/taipy-rest/setup.requirements.txt
 tools/packages/taipy-templates/MANIFEST.in
 tools/packages/taipy-templates/setup.py
 tools/packages/taipy-templates/setup.requirements.txt
 tools/release/build_package_structure.py
 tools/release/check_releases.py
 tools/release/extract_from_setup.py
+tools/release/fetch_latest_versions.py
 tools/release/setup_version.py
 tools/release/update_setup.py
 tools/release/update_setup_requirements.py
```

### Comparing `taipy-3.1.0/tests/test_run.py` & `taipy-3.1.1/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/frontend/bundle_build.py` & `taipy-3.1.1/tools/frontend/bundle_build.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/gui/generate_pyi.py` & `taipy-3.1.1/tools/gui/generate_pyi.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/modify_readme.py` & `taipy-3.1.1/tools/modify_readme.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/check-dependencies.py` & `taipy-3.1.1/tools/packages/check-dependencies.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/check-dependencies.sh` & `taipy-3.1.1/tools/packages/check-dependencies.sh`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/pipfiles/Pipfile3.10.max` & `taipy-3.1.1/tools/packages/pipfiles/Pipfile3.10.max`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/pipfiles/Pipfile3.11.max` & `taipy-3.1.1/tools/packages/pipfiles/Pipfile3.11.max`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/pipfiles/Pipfile3.12.max` & `taipy-3.1.1/tools/packages/pipfiles/Pipfile3.12.max`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/pipfiles/Pipfile3.8.max` & `taipy-3.1.1/tools/packages/pipfiles/Pipfile3.8.max`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/pipfiles/Pipfile3.9.max` & `taipy-3.1.1/tools/packages/pipfiles/Pipfile3.9.max`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/taipy/MANIFEST.in` & `taipy-3.1.1/tools/packages/taipy/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/taipy/setup.py` & `taipy-3.1.1/tools/packages/taipy/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/taipy-config/setup.py` & `taipy-3.1.1/tools/packages/taipy-config/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/taipy-core/setup.py` & `taipy-3.1.1/tools/packages/taipy-core/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/taipy-gui/setup.py` & `taipy-3.1.1/tools/packages/taipy-gui/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/taipy-rest/setup.py` & `taipy-3.1.1/tools/packages/taipy-rest/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/packages/taipy-templates/setup.py` & `taipy-3.1.1/tools/packages/taipy-templates/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/release/build_package_structure.py` & `taipy-3.1.1/tools/release/build_package_structure.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/release/check_releases.py` & `taipy-3.1.1/tools/release/check_releases.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/release/setup_version.py` & `taipy-3.1.1/tools/release/setup_version.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/release/update_setup.py` & `taipy-3.1.1/tools/release/update_setup.py`

 * *Files identical despite different names*

### Comparing `taipy-3.1.0/tools/release/update_setup_requirements.py` & `taipy-3.1.1/tools/release/update_setup_requirements.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 from typing import Dict
 
 BASE_PATH = "./tools/packages"
 
 
 def __build_taipy_package_line(line: str, version: str, publish_on_py_pi: bool) -> str:
     _line = line.strip()
+    max_version = f'{version.split(".")[0]}.{int(version.split(".")[1]) + 1}.0'
     if publish_on_py_pi:
-        return f"{_line}=={version}\n"
+        return f"{_line}>={version}, <{max_version}\n"
+
     tag = f"{version}-{_line.split('-')[1]}"
     tar_name = f"{_line}-{version}"
     return f"{_line} @ https://github.com/Avaiga/taipy/releases/download/{tag}/{tar_name}.tar.gz\n"
 
 
 def update_setup_requirements(package: str, versions: Dict, publish_on_py_pi: bool) -> None:
     _path = os.path.join(BASE_PATH, package, "setup.requirements.txt")
```

### Comparing `taipy-3.1.0/tools/validate_taipy_install.py` & `taipy-3.1.1/tools/validate_taipy_install.py`

 * *Files identical despite different names*

