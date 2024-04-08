# Comparing `tmp/pyodide_mkdocs_theme-0.1.0.tar.gz` & `tmp/pyodide_mkdocs_theme-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-0.1.0.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-0.1.1.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-0.1.0.tar` & `pyodide_mkdocs_theme-0.1.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-07 16:13:56.353971 pyodide_mkdocs_theme-0.1.0/README.md
--rw-r--r--   0        0        0     1347 2024-04-07 16:21:13.598780 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     6047 2024-04-06 19:37:06.626242 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-04-07 16:21:13.638781 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      752 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     4832 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     4935 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
--rw-r--r--   0        0        0    21850 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
--rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0     4062 2024-04-06 19:50:40.682880 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11234 2024-04-07 10:49:12.948368 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0     6948 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0     4007 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4462 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0     7301 2024-04-04 20:47:10.474631 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11890 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0    12226 2024-04-07 16:15:00.119838 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
--rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     2899 2024-04-04 17:32:31.188228 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     8427 2024-04-04 20:46:58.718283 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2653 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0      374 2024-04-04 10:11:40.443879 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     6553 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     7206 2024-04-07 06:55:38.270867 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     1214 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     9589 2024-04-04 09:56:58.154964 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
--rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
--rw-r--r--   0        0        0     3530 2024-04-06 11:30:24.316895 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-extrahead.css
--rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
--rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
--rw-r--r--   0        0        0     6051 2024-04-04 09:56:58.154964 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
--rw-r--r--   0        0        0    16436 2024-04-04 09:56:58.154964 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
--rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
--rw-r--r--   0        0        0      137 2024-03-05 13:24:26.138158 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/README.md
--rw-r--r--   0        0        0     3986 2024-04-07 12:16:07.564974 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/0_config-libs.js
--rw-r--r--   0        0        0     7119 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/functools-libs.js
--rw-r--r--   0        0        0     1675 2024-04-07 10:49:36.669062 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/jsLogger-libs.js
--rw-r--r--   0        0        0     4297 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/securedPagesData-libs.js
--rw-r--r--   0        0        0     3626 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0     1078 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/z_header-btns-extrahead.css
--rw-r--r--   0        0        0     1490 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
--rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
--rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
--rw-r--r--   0        0        0     3582 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-extrahead.css
--rw-r--r--   0        0        0    31978 2024-04-04 09:56:58.202965 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-extrahead.css
--rw-r--r--   0        0        0     1527 2024-04-04 09:56:58.202965 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-extrahead.css
--rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
--rw-r--r--   0        0        0     4233 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
--rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
--rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
--rw-r--r--   0        0        0     3774 2024-04-07 09:15:49.456003 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/qcm/qcm-extrahead.css
--rw-r--r--   0        0        0    12598 2024-04-07 10:53:56.264647 pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
--rw-r--r--   0        0        0     1701 2024-04-06 21:01:46.405035 pyodide_mkdocs_theme-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-07 16:13:56.353971 pyodide_mkdocs_theme-0.1.1/README.md
+-rw-r--r--   0        0        0     1347 2024-04-08 14:31:57.819181 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     6071 2024-04-07 19:41:30.518314 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-08 14:31:57.855182 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      752 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     4832 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     4935 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
+-rw-r--r--   0        0        0    21850 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
+-rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0     4062 2024-04-06 19:50:40.682880 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11234 2024-04-07 10:49:12.948368 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0     6948 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0     4007 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4462 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0     7303 2024-04-08 14:28:15.731641 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11890 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0    12230 2024-04-08 14:28:15.731641 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
+-rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     2899 2024-04-04 17:32:31.188228 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     8427 2024-04-04 20:46:58.718283 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2653 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1064 2024-04-08 14:31:57.763179 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     6553 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     7206 2024-04-07 06:55:38.270867 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     1214 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     9589 2024-04-04 09:56:58.154964 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
+-rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
+-rw-r--r--   0        0        0     3530 2024-04-06 11:30:24.316895 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-extrahead.css
+-rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
+-rw-r--r--   0        0        0     6051 2024-04-04 09:56:58.154964 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
+-rw-r--r--   0        0        0    16436 2024-04-04 09:56:58.154964 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
+-rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0      137 2024-03-05 13:24:26.138158 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/README.md
+-rw-r--r--   0        0        0     3986 2024-04-07 12:16:07.564974 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/0_config-libs.js
+-rw-r--r--   0        0        0     7119 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/functools-libs.js
+-rw-r--r--   0        0        0     1675 2024-04-07 10:49:36.669062 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/jsLogger-libs.js
+-rw-r--r--   0        0        0     4297 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/securedPagesData-libs.js
+-rw-r--r--   0        0        0     3626 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0     1078 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/z_header-btns-extrahead.css
+-rw-r--r--   0        0        0     1490 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
+-rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
+-rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
+-rw-r--r--   0        0        0     3582 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-extrahead.css
+-rw-r--r--   0        0        0    31978 2024-04-04 09:56:58.202965 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-extrahead.css
+-rw-r--r--   0        0        0     1527 2024-04-04 09:56:58.202965 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-extrahead.css
+-rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
+-rw-r--r--   0        0        0     4233 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
+-rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
+-rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
+-rw-r--r--   0        0        0     3774 2024-04-07 09:15:49.456003 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/qcm/qcm-extrahead.css
+-rw-r--r--   0        0        0    12598 2024-04-07 10:53:56.264647 pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
+-rw-r--r--   0        0        0     1687 2024-04-08 14:31:54.439055 pyodide_mkdocs_theme-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.1.1/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-0.1.0/LICENSE` & `pyodide_mkdocs_theme-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/README.md` & `pyodide_mkdocs_theme-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
   - material/search         # Les plugins de material-mkdocs doivent être préfixés!
 
   - exclude:                # (pip install mkdocs-exclude)
       glob:                 # Patterns identifiant des pages à ne pas inclure dans le build.
         - sous_dossier/**/*REM.md   # Les fichiers de remarques DOIVENT être exclus
         - sous_dossier/**/*.py      # Les fichiers python DOIVENT être exclus
 
-  - exclude-search:         # (pip install mkdocs-exclude-search)
+  - exclude-search:         # APRÈS le plugin search (pip install mkdocs-exclude-search)
       exclude:              # Pour les fichiers inclus dans le build, que la recherche ne doit pas indexer
         - bac_a_sable.md
 
   - pyodide_macros          # !!REQUIS!!
 
 
 validation:                 # Si mkdocs est lancé en mode strict (mkdocs ... --strict), les warnings lèveront une erreur
```

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     macros_with_indents = C.Type(str, default='')
     """
     Allow to register external macros that will use the `PyodideMacrosPlugin.get_indent` logistic
     to insert indented multiline contents in the page.
     `macro_with_indents` is a space separated string of all the names of the macros to register.
     """
 
-    show_indent_errors = C.Type(bool, default=False)
+    bypass_indent_errors = C.Type(bool, default=False)
     """
     If True, all errors related to indentation logistic for macros are bypassed and a message is
     printed in the console instead.
     The purpose of this option is _not_ to deactivate the securities, but to allow gathering info
     about all the problems at once: note that the resulting markdown content will most likely be
     incorrect and rendered the wrong way.
     """
```

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                 id_reason=id_reason,
             )
         return target
 
 
 
     def _handle_error(self, env:'BaseMaestro', err_msg:str, epilogue:str='', id_reason:str=""):
-        if env.show_indent_errors:
+        if env.bypass_indent_errors:
             id_reason = id_reason or "invalid call structure?"
             logger.warning(                 # pylint: disable-next=protected-access
                 f"[INDENT] - Macro {env._running_macro}, in {env.page.file.src_uri} ({id_reason})"
             )
         else:
             if id_reason:
                 err_msg = (
@@ -201,15 +201,15 @@
     skip_py_md_paths_names_validation: bool = ConfigExtractor()
     check_python_files: bool  = ConfigExtractor()
     soft_check: bool          = ConfigExtractor()
     load_yaml_encoding: str   = ConfigExtractor()
     _dev_mode: bool           = ConfigExtractor()
     encrypt_corrections_and_rems: bool = ConfigExtractor()
     macros_with_indents: str  = ConfigExtractor()
-    show_indent_errors: bool = ConfigExtractor()
+    bypass_indent_errors: bool = ConfigExtractor()
     ignore_macros_plugin_diffs: bool = ConfigExtractor()
 
     scripts_url: str    = ConfigExtractor("others")
     site_root: str      = ConfigExtractor("others")
 
     page: Page  # just as a reminder: defined by MacrosPlugin
```

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/__init__.py` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/main.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-extrahead.css` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-extrahead.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/0_config-libs.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/0_config-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/functools-libs.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/functools-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/jsLogger-libs.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/securedPagesData-libs.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/securedPagesData-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/z_header-btns-extrahead.css` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/z_header-btns-extrahead.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-extrahead.css` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-extrahead.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-extrahead.css` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-extrahead.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-extrahead.css` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-extrahead.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/qcm/qcm-extrahead.css` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/qcm/qcm-extrahead.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js` & `pyodide_mkdocs_theme-0.1.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.0/pyproject.toml` & `pyodide_mkdocs_theme-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "0.1.0"
+version = "0.1.1"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
@@ -37,19 +37,19 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 mkdocs-material = "^9.5"
 mkdocs-macros-plugin = "^1.0"
 
 
 [tool.poetry.group.dev.dependencies]
-pylint = "^3.1.0"
-pytest = "^8.1.1"
-mkdocs-addresses = "^0.2.4"
-mkdocs-awesome-pages-plugin = "^2.9.2"
-mkdocs-exclude = "^1.0.2"
-mkdocs-exclude-search = "^0.6.6"
-mkdocs-enumerate-headings-plugin = "^0.6.1"
+pylint = "^3.1"
+pytest = "^8.1"
+mkdocs-addresses = "^0.2"
+mkdocs-awesome-pages-plugin = "^2.9"
+mkdocs-exclude = "^1.0"
+mkdocs-exclude-search = "^0.6"
+mkdocs-enumerate-headings-plugin = "^0.6"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyodide_mkdocs_theme-0.1.0/PKG-INFO` & `pyodide_mkdocs_theme-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

