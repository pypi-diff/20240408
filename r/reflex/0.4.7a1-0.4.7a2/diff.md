# Comparing `tmp/reflex-0.4.7a1.tar.gz` & `tmp/reflex-0.4.7a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.4.7a1.tar", max compression
+gzip compressed data, was "reflex-0.4.7a2.tar", max compression
```

## Comparing `reflex-0.4.7a1.tar` & `reflex-0.4.7a2.tar`

### file list

```diff
@@ -1,508 +1,508 @@
--rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.4.7a1/LICENSE
--rw-r--r--   0        0        0     9568 2024-04-04 21:37:03.943217 reflex-0.4.7a1/README.md
--rw-r--r--   0        0        0     2922 2024-04-05 00:24:21.453882 reflex-0.4.7a1/pyproject.toml
--rw-r--r--   0        0        0     4286 2023-11-07 19:58:07.469572 reflex-0.4.7a1/reflex/.templates/apps/blank/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-11-07 19:58:07.469657 reflex-0.4.7a1/reflex/.templates/apps/blank/code/__init__.py
--rw-r--r--   0        0        0      861 2024-04-05 00:24:11.496563 reflex-0.4.7a1/reflex/.templates/apps/blank/code/blank.py
--rw-r--r--   0        0        0       32 2023-11-07 19:58:07.469933 reflex-0.4.7a1/reflex/.templates/apps/demo/.gitignore
--rw-r--r--   0        0        0     4286 2023-11-07 19:58:07.470079 reflex-0.4.7a1/reflex/.templates/apps/demo/assets/favicon.ico
--rw-r--r--   0        0        0     1475 2023-11-07 19:58:07.470183 reflex-0.4.7a1/reflex/.templates/apps/demo/assets/github.svg
--rw-r--r--   0        0        0     1899 2023-11-07 19:58:07.470263 reflex-0.4.7a1/reflex/.templates/apps/demo/assets/icon.svg
--rw-r--r--   0        0        0     5403 2023-11-07 19:58:07.470351 reflex-0.4.7a1/reflex/.templates/apps/demo/assets/logo.svg
--rw-r--r--   0        0        0      807 2023-11-07 19:58:07.470441 reflex-0.4.7a1/reflex/.templates/apps/demo/assets/paneleft.svg
--rw-r--r--   0        0        0       32 2023-11-07 19:58:07.470556 reflex-0.4.7a1/reflex/.templates/apps/demo/code/__init__.py
--rw-r--r--   0        0        0     2928 2024-04-02 19:14:34.394285 reflex-0.4.7a1/reflex/.templates/apps/demo/code/demo.py
--rw-r--r--   0        0        0      194 2023-11-07 19:58:07.470763 reflex-0.4.7a1/reflex/.templates/apps/demo/code/pages/__init__.py
--rw-r--r--   0        0        0      706 2024-04-02 19:14:34.394398 reflex-0.4.7a1/reflex/.templates/apps/demo/code/pages/chatapp.py
--rw-r--r--   0        0        0    10910 2024-04-02 19:14:34.394812 reflex-0.4.7a1/reflex/.templates/apps/demo/code/pages/datatable.py
--rw-r--r--   0        0        0     8383 2024-04-02 19:14:34.395299 reflex-0.4.7a1/reflex/.templates/apps/demo/code/pages/forms.py
--rw-r--r--   0        0        0     8519 2024-04-02 19:14:34.395551 reflex-0.4.7a1/reflex/.templates/apps/demo/code/pages/graphing.py
--rw-r--r--   0        0        0     1822 2024-04-02 19:14:34.395723 reflex-0.4.7a1/reflex/.templates/apps/demo/code/pages/home.py
--rw-r--r--   0        0        0     4722 2024-04-02 19:14:34.395853 reflex-0.4.7a1/reflex/.templates/apps/demo/code/sidebar.py
--rw-r--r--   0        0        0      510 2023-11-07 19:58:07.471657 reflex-0.4.7a1/reflex/.templates/apps/demo/code/state.py
--rw-r--r--   0        0        0      912 2023-11-07 19:58:07.471802 reflex-0.4.7a1/reflex/.templates/apps/demo/code/states/form_state.py
--rw-r--r--   0        0        0     1189 2023-11-07 19:58:07.471905 reflex-0.4.7a1/reflex/.templates/apps/demo/code/states/pie_state.py
--rw-r--r--   0        0        0     1486 2024-04-02 19:14:34.395963 reflex-0.4.7a1/reflex/.templates/apps/demo/code/styles.py
--rw-r--r--   0        0        0        0 2023-11-07 19:58:07.472085 reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/__init__.py
--rw-r--r--   0        0        0      120 2023-11-07 19:58:07.472204 reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/components/__init__.py
--rw-r--r--   0        0        0     3584 2024-04-02 19:14:34.396085 reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/components/chat.py
--rw-r--r--   0        0        0      680 2023-11-07 19:58:07.472372 reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
--rw-r--r--   0        0        0     1829 2024-04-02 19:14:34.396198 reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/components/modal.py
--rw-r--r--   0        0        0     2251 2024-04-02 19:14:34.396306 reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/components/navbar.py
--rw-r--r--   0        0        0     1735 2024-04-02 19:14:34.396392 reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py
--rw-r--r--   0        0        0     4001 2023-11-07 19:58:07.472705 reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/state.py
--rw-r--r--   0        0        0     2281 2024-04-02 19:14:34.396499 reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/styles.py
--rw-r--r--   0        0        0       74 2023-09-18 23:00:36.695709 reflex-0.4.7a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      127 2024-04-02 19:14:34.400175 reflex-0.4.7a1/reflex/.templates/jinja/custom_components/README.md.jinja2
--rw-r--r--   0        0        0       32 2024-04-02 19:14:34.401028 reflex-0.4.7a1/reflex/.templates/jinja/custom_components/__init__.py.jinja2
--rw-r--r--   0        0        0      826 2024-04-02 19:14:34.401442 reflex-0.4.7a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
--rw-r--r--   0        0        0      614 2024-04-04 21:37:03.945011 reflex-0.4.7a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
--rw-r--r--   0        0        0     2403 2024-04-04 21:37:03.945109 reflex-0.4.7a1/reflex/.templates/jinja/custom_components/src.py.jinja2
--rw-r--r--   0        0        0      548 2023-09-25 02:29:12.548714 reflex-0.4.7a1/reflex/.templates/jinja/web/package.json.jinja2
--rw-r--r--   0        0        0      930 2024-04-02 19:14:34.402842 reflex-0.4.7a1/reflex/.templates/jinja/web/pages/_app.js.jinja2
--rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.4.7a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      400 2024-02-13 04:39:14.427011 reflex-0.4.7a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0       86 2023-09-25 02:29:12.549046 reflex-0.4.7a1/reflex/.templates/jinja/web/pages/component.js.jinja2
--rw-r--r--   0        0        0      882 2023-12-04 22:31:51.571558 reflex-0.4.7a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0      343 2024-04-04 21:37:03.945229 reflex-0.4.7a1/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0      388 2024-04-04 21:37:03.945317 reflex-0.4.7a1/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
--rw-r--r--   0        0        0      101 2023-12-04 22:31:51.572637 reflex-0.4.7a1/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
--rw-r--r--   0        0        0     3883 2024-02-10 02:26:35.013845 reflex-0.4.7a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      141 2023-09-18 23:00:36.695917 reflex-0.4.7a1/reflex/.templates/jinja/web/styles/styles.css.jinja2
--rw-r--r--   0        0        0      436 2024-02-10 02:26:35.013954 reflex-0.4.7a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0     3790 2024-04-02 19:14:34.404054 reflex-0.4.7a1/reflex/.templates/jinja/web/utils/context.js.jinja2
--rw-r--r--   0        0        0       37 2023-10-20 19:16:08.667797 reflex-0.4.7a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.4.7a1/reflex/.templates/web/.gitignore
--rw-r--r--   0        0        0      595 2023-10-20 19:16:08.667942 reflex-0.4.7a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
--rw-r--r--   0        0        0      645 2024-04-02 19:14:34.404228 reflex-0.4.7a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
--rw-r--r--   0        0        0       97 2023-09-18 23:00:36.696123 reflex-0.4.7a1/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0      118 2023-11-14 20:34:38.772076 reflex-0.4.7a1/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.4.7a1/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.4.7a1/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     1254 2023-09-06 00:16:27.465104 reflex-0.4.7a1/reflex/.templates/web/utils/client_side_routing.js
--rw-r--r--   0        0        0     1622 2024-02-10 02:26:35.014073 reflex-0.4.7a1/reflex/.templates/web/utils/helpers/dataeditor.js
--rw-r--r--   0        0        0     1152 2023-11-14 20:34:38.772264 reflex-0.4.7a1/reflex/.templates/web/utils/helpers/range.js
--rw-r--r--   0        0        0    21688 2024-04-04 22:32:02.761656 reflex-0.4.7a1/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     5723 2024-04-04 21:37:03.945600 reflex-0.4.7a1/reflex/__init__.py
--rw-r--r--   0        0        0     7649 2024-04-04 22:00:30.126840 reflex-0.4.7a1/reflex/__init__.pyi
--rw-r--r--   0        0        0      108 2023-08-10 23:30:03.955150 reflex-0.4.7a1/reflex/__main__.py
--rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.4.7a1/reflex/admin.py
--rw-r--r--   0        0        0    44562 2024-04-04 21:37:03.945930 reflex-0.4.7a1/reflex/app.py
--rw-r--r--   0        0        0     5010 2024-04-04 21:37:03.946046 reflex-0.4.7a1/reflex/app.pyi
--rw-r--r--   0        0        0     1152 2024-04-02 19:14:34.406758 reflex-0.4.7a1/reflex/app_module_for_backend.py
--rw-r--r--   0        0        0     4250 2024-04-02 19:14:34.407224 reflex-0.4.7a1/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.4.7a1/reflex/compiler/__init__.py
--rw-r--r--   0        0        0    17037 2024-04-04 21:37:03.946194 reflex-0.4.7a1/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     4344 2024-04-02 19:14:34.407873 reflex-0.4.7a1/reflex/compiler/templates.py
--rw-r--r--   0        0        0    14022 2024-04-04 21:37:03.946346 reflex-0.4.7a1/reflex/compiler/utils.py
--rw-r--r--   0        0        0      530 2024-04-02 19:14:34.408438 reflex-0.4.7a1/reflex/components/__init__.py
--rw-r--r--   0        0        0      325 2024-02-10 02:26:35.019008 reflex-0.4.7a1/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      573 2024-02-10 02:26:35.019123 reflex-0.4.7a1/reflex/components/base/app_wrap.py
--rw-r--r--   0        0        0     2890 2024-04-02 19:14:34.408568 reflex-0.4.7a1/reflex/components/base/app_wrap.pyi
--rw-r--r--   0        0        0     1234 2024-04-02 19:14:34.408691 reflex-0.4.7a1/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-12-21 01:07:08.388770 reflex-0.4.7a1/reflex/components/base/body.py
--rw-r--r--   0        0        0     3277 2024-04-02 19:14:34.408849 reflex-0.4.7a1/reflex/components/base/body.pyi
--rw-r--r--   0        0        0      583 2024-04-02 19:14:34.409155 reflex-0.4.7a1/reflex/components/base/document.py
--rw-r--r--   0        0        0    14587 2024-04-02 19:14:34.409362 reflex-0.4.7a1/reflex/components/base/document.pyi
--rw-r--r--   0        0        0      312 2024-02-10 02:26:35.020357 reflex-0.4.7a1/reflex/components/base/fragment.py
--rw-r--r--   0        0        0     3289 2024-04-02 19:14:34.409517 reflex-0.4.7a1/reflex/components/base/fragment.pyi
--rw-r--r--   0        0        0      297 2023-12-21 01:07:08.390493 reflex-0.4.7a1/reflex/components/base/head.py
--rw-r--r--   0        0        0     6073 2024-04-02 19:14:34.409716 reflex-0.4.7a1/reflex/components/base/head.pyi
--rw-r--r--   0        0        0      929 2023-12-21 01:07:08.390801 reflex-0.4.7a1/reflex/components/base/link.py
--rw-r--r--   0        0        0     7132 2024-04-02 19:14:34.410033 reflex-0.4.7a1/reflex/components/base/link.pyi
--rw-r--r--   0        0        0     1438 2023-12-21 01:07:08.390993 reflex-0.4.7a1/reflex/components/base/meta.py
--rw-r--r--   0        0        0    13088 2024-04-02 19:14:34.410197 reflex-0.4.7a1/reflex/components/base/meta.pyi
--rw-r--r--   0        0        0     2298 2023-12-21 01:07:08.391208 reflex-0.4.7a1/reflex/components/base/script.py
--rw-r--r--   0        0        0     4500 2024-04-02 19:14:34.410334 reflex-0.4.7a1/reflex/components/base/script.pyi
--rw-r--r--   0        0        0     6378 2024-04-02 19:14:34.410492 reflex-0.4.7a1/reflex/components/chakra/__init__.py
--rw-r--r--   0        0        0     5242 2024-02-16 18:55:54.269834 reflex-0.4.7a1/reflex/components/chakra/base.py
--rw-r--r--   0        0        0    11059 2024-04-02 19:14:34.410632 reflex-0.4.7a1/reflex/components/chakra/base.pyi
--rw-r--r--   0        0        0      459 2024-04-02 19:14:34.410790 reflex-0.4.7a1/reflex/components/chakra/datadisplay/__init__.py
--rw-r--r--   0        0        0      352 2024-02-10 02:26:35.022081 reflex-0.4.7a1/reflex/components/chakra/datadisplay/badge.py
--rw-r--r--   0        0        0     3725 2024-04-02 19:14:34.410909 reflex-0.4.7a1/reflex/components/chakra/datadisplay/badge.pyi
--rw-r--r--   0        0        0      174 2024-04-02 19:14:34.411078 reflex-0.4.7a1/reflex/components/chakra/datadisplay/code.py
--rw-r--r--   0        0        0     3300 2024-04-02 19:14:34.411266 reflex-0.4.7a1/reflex/components/chakra/datadisplay/code.pyi
--rw-r--r--   0        0        0      657 2024-02-10 02:26:35.022721 reflex-0.4.7a1/reflex/components/chakra/datadisplay/divider.py
--rw-r--r--   0        0        0     4005 2024-04-02 19:14:34.411393 reflex-0.4.7a1/reflex/components/chakra/datadisplay/divider.pyi
--rw-r--r--   0        0        0      180 2024-02-10 02:26:35.022864 reflex-0.4.7a1/reflex/components/chakra/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     3322 2024-04-02 19:14:34.411517 reflex-0.4.7a1/reflex/components/chakra/datadisplay/keyboard_key.pyi
--rw-r--r--   0        0        0     1505 2024-02-10 02:26:35.022985 reflex-0.4.7a1/reflex/components/chakra/datadisplay/list.py
--rw-r--r--   0        0        0    13065 2024-04-02 19:14:34.411638 reflex-0.4.7a1/reflex/components/chakra/datadisplay/list.pyi
--rw-r--r--   0        0        0     2149 2024-02-10 02:26:35.023113 reflex-0.4.7a1/reflex/components/chakra/datadisplay/stat.py
--rw-r--r--   0        0        0    17816 2024-04-02 19:14:34.411771 reflex-0.4.7a1/reflex/components/chakra/datadisplay/stat.pyi
--rw-r--r--   0        0        0     9122 2024-02-10 02:26:35.023268 reflex-0.4.7a1/reflex/components/chakra/datadisplay/table.py
--rw-r--r--   0        0        0    27536 2024-04-02 19:14:34.411949 reflex-0.4.7a1/reflex/components/chakra/datadisplay/table.pyi
--rw-r--r--   0        0        0     2294 2024-02-10 02:26:35.023510 reflex-0.4.7a1/reflex/components/chakra/datadisplay/tag.py
--rw-r--r--   0        0        0    16018 2024-04-02 19:14:34.412089 reflex-0.4.7a1/reflex/components/chakra/datadisplay/tag.pyi
--rw-r--r--   0        0        0      384 2024-02-10 02:26:35.023677 reflex-0.4.7a1/reflex/components/chakra/disclosure/__init__.py
--rw-r--r--   0        0        0     3509 2024-02-10 02:26:35.023748 reflex-0.4.7a1/reflex/components/chakra/disclosure/accordion.py
--rw-r--r--   0        0        0    16087 2024-04-02 19:14:34.412252 reflex-0.4.7a1/reflex/components/chakra/disclosure/accordion.pyi
--rw-r--r--   0        0        0     3295 2024-02-10 02:26:35.024084 reflex-0.4.7a1/reflex/components/chakra/disclosure/tabs.py
--rw-r--r--   0        0        0    18809 2024-04-02 19:14:34.412388 reflex-0.4.7a1/reflex/components/chakra/disclosure/tabs.pyi
--rw-r--r--   0        0        0     1732 2024-02-10 02:26:35.024232 reflex-0.4.7a1/reflex/components/chakra/disclosure/transition.py
--rw-r--r--   0        0        0    20429 2024-04-02 19:14:34.412530 reflex-0.4.7a1/reflex/components/chakra/disclosure/transition.pyi
--rw-r--r--   0        0        0      278 2024-02-10 02:26:35.024533 reflex-0.4.7a1/reflex/components/chakra/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0     3329 2024-04-02 19:14:34.412660 reflex-0.4.7a1/reflex/components/chakra/disclosure/visuallyhidden.pyi
--rw-r--r--   0        0        0      313 2024-02-10 02:26:35.024661 reflex-0.4.7a1/reflex/components/chakra/feedback/__init__.py
--rw-r--r--   0        0        0     1623 2024-02-10 02:26:35.024723 reflex-0.4.7a1/reflex/components/chakra/feedback/alert.py
--rw-r--r--   0        0        0    12594 2024-04-02 19:14:34.412793 reflex-0.4.7a1/reflex/components/chakra/feedback/alert.pyi
--rw-r--r--   0        0        0     2006 2024-02-10 02:26:35.024858 reflex-0.4.7a1/reflex/components/chakra/feedback/circularprogress.py
--rw-r--r--   0        0        0     7708 2024-04-02 19:14:34.412916 reflex-0.4.7a1/reflex/components/chakra/feedback/circularprogress.pyi
--rw-r--r--   0        0        0      871 2024-02-10 02:26:35.024988 reflex-0.4.7a1/reflex/components/chakra/feedback/progress.py
--rw-r--r--   0        0        0     4349 2024-04-02 19:14:34.413051 reflex-0.4.7a1/reflex/components/chakra/feedback/progress.pyi
--rw-r--r--   0        0        0     1776 2024-02-10 02:26:35.025096 reflex-0.4.7a1/reflex/components/chakra/feedback/skeleton.py
--rw-r--r--   0        0        0    10903 2024-04-02 19:14:34.413182 reflex-0.4.7a1/reflex/components/chakra/feedback/skeleton.pyi
--rw-r--r--   0        0        0      704 2024-02-10 02:26:35.025211 reflex-0.4.7a1/reflex/components/chakra/feedback/spinner.py
--rw-r--r--   0        0        0     4178 2024-04-02 19:14:34.413298 reflex-0.4.7a1/reflex/components/chakra/feedback/spinner.pyi
--rw-r--r--   0        0        0     1453 2024-04-02 19:14:34.413424 reflex-0.4.7a1/reflex/components/chakra/forms/__init__.py
--rw-r--r--   0        0        0     2395 2024-02-10 02:26:35.025415 reflex-0.4.7a1/reflex/components/chakra/forms/button.py
--rw-r--r--   0        0        0    10687 2024-04-02 19:14:34.413528 reflex-0.4.7a1/reflex/components/chakra/forms/button.pyi
--rw-r--r--   0        0        0     2764 2024-02-10 02:26:35.025535 reflex-0.4.7a1/reflex/components/chakra/forms/checkbox.py
--rw-r--r--   0        0        0    10443 2024-04-02 19:14:34.413633 reflex-0.4.7a1/reflex/components/chakra/forms/checkbox.pyi
--rw-r--r--   0        0        0     2860 2024-04-02 19:14:34.413744 reflex-0.4.7a1/reflex/components/chakra/forms/colormodeswitch.py
--rw-r--r--   0        0        0    18530 2024-04-02 19:14:34.413852 reflex-0.4.7a1/reflex/components/chakra/forms/colormodeswitch.pyi
--rw-r--r--   0        0        0      246 2024-02-10 02:26:35.025773 reflex-0.4.7a1/reflex/components/chakra/forms/date_picker.py
--rw-r--r--   0        0        0     5841 2024-04-02 19:14:34.413954 reflex-0.4.7a1/reflex/components/chakra/forms/date_picker.pyi
--rw-r--r--   0        0        0      280 2024-02-10 02:26:35.025877 reflex-0.4.7a1/reflex/components/chakra/forms/date_time_picker.py
--rw-r--r--   0        0        0     5854 2024-04-02 19:14:34.414051 reflex-0.4.7a1/reflex/components/chakra/forms/date_time_picker.pyi
--rw-r--r--   0        0        0     2110 2024-02-10 02:26:35.025987 reflex-0.4.7a1/reflex/components/chakra/forms/editable.py
--rw-r--r--   0        0        0    13623 2024-04-02 19:14:34.414156 reflex-0.4.7a1/reflex/components/chakra/forms/editable.pyi
--rw-r--r--   0        0        0      246 2024-02-10 02:26:35.026103 reflex-0.4.7a1/reflex/components/chakra/forms/email.py
--rw-r--r--   0        0        0     5825 2024-04-02 19:14:34.414250 reflex-0.4.7a1/reflex/components/chakra/forms/email.pyi
--rw-r--r--   0        0        0     2579 2024-04-02 19:14:34.414562 reflex-0.4.7a1/reflex/components/chakra/forms/form.py
--rw-r--r--   0        0        0    20832 2024-04-02 19:14:34.414743 reflex-0.4.7a1/reflex/components/chakra/forms/form.pyi
--rw-r--r--   0        0        0      935 2024-02-10 02:26:35.026649 reflex-0.4.7a1/reflex/components/chakra/forms/iconbutton.py
--rw-r--r--   0        0        0     4739 2024-04-02 19:14:34.414896 reflex-0.4.7a1/reflex/components/chakra/forms/iconbutton.pyi
--rw-r--r--   0        0        0     4312 2024-04-02 19:14:34.415230 reflex-0.4.7a1/reflex/components/chakra/forms/input.py
--rw-r--r--   0        0        0    21869 2024-04-02 19:14:34.415375 reflex-0.4.7a1/reflex/components/chakra/forms/input.pyi
--rw-r--r--   0        0        0    12940 2024-02-10 02:26:35.027180 reflex-0.4.7a1/reflex/components/chakra/forms/multiselect.py
--rw-r--r--   0        0        0     4334 2024-02-10 02:26:35.027253 reflex-0.4.7a1/reflex/components/chakra/forms/numberinput.py
--rw-r--r--   0        0        0    18377 2024-04-02 19:14:34.415512 reflex-0.4.7a1/reflex/components/chakra/forms/numberinput.pyi
--rw-r--r--   0        0        0      256 2024-02-10 02:26:35.027395 reflex-0.4.7a1/reflex/components/chakra/forms/password.py
--rw-r--r--   0        0        0     5834 2024-04-02 19:14:34.415639 reflex-0.4.7a1/reflex/components/chakra/forms/password.pyi
--rw-r--r--   0        0        0     6507 2024-04-04 21:37:03.946495 reflex-0.4.7a1/reflex/components/chakra/forms/pininput.py
--rw-r--r--   0        0        0     9432 2024-04-02 19:14:34.415764 reflex-0.4.7a1/reflex/components/chakra/forms/pininput.pyi
--rw-r--r--   0        0        0     3176 2024-02-10 02:26:35.027681 reflex-0.4.7a1/reflex/components/chakra/forms/radio.py
--rw-r--r--   0        0        0     8414 2024-04-02 19:14:34.415876 reflex-0.4.7a1/reflex/components/chakra/forms/radio.pyi
--rw-r--r--   0        0        0     4547 2024-02-10 02:26:35.027836 reflex-0.4.7a1/reflex/components/chakra/forms/rangeslider.py
--rw-r--r--   0        0        0    14156 2024-04-02 19:14:34.415997 reflex-0.4.7a1/reflex/components/chakra/forms/rangeslider.pyi
--rw-r--r--   0        0        0     3624 2024-02-10 02:26:35.027969 reflex-0.4.7a1/reflex/components/chakra/forms/select.py
--rw-r--r--   0        0        0     8868 2024-04-02 19:14:34.416109 reflex-0.4.7a1/reflex/components/chakra/forms/select.pyi
--rw-r--r--   0        0        0     3532 2024-02-10 02:26:35.028089 reflex-0.4.7a1/reflex/components/chakra/forms/slider.py
--rw-r--r--   0        0        0    17745 2024-04-02 19:14:34.416245 reflex-0.4.7a1/reflex/components/chakra/forms/slider.pyi
--rw-r--r--   0        0        0     1838 2024-02-10 02:26:35.028236 reflex-0.4.7a1/reflex/components/chakra/forms/switch.py
--rw-r--r--   0        0        0     6602 2024-04-02 19:14:34.416373 reflex-0.4.7a1/reflex/components/chakra/forms/switch.pyi
--rw-r--r--   0        0        0     2474 2024-02-16 18:55:54.270329 reflex-0.4.7a1/reflex/components/chakra/forms/textarea.py
--rw-r--r--   0        0        0     5419 2024-04-02 19:14:34.416480 reflex-0.4.7a1/reflex/components/chakra/forms/textarea.pyi
--rw-r--r--   0        0        0      246 2024-02-10 02:26:35.028621 reflex-0.4.7a1/reflex/components/chakra/forms/time_picker.py
--rw-r--r--   0        0        0     5841 2024-04-02 19:14:34.416578 reflex-0.4.7a1/reflex/components/chakra/forms/time_picker.pyi
--rw-r--r--   0        0        0      487 2024-04-02 19:14:34.416715 reflex-0.4.7a1/reflex/components/chakra/layout/__init__.py
--rw-r--r--   0        0        0      315 2024-02-10 02:26:35.028815 reflex-0.4.7a1/reflex/components/chakra/layout/aspect_ratio.py
--rw-r--r--   0        0        0     3450 2024-04-02 19:14:34.416820 reflex-0.4.7a1/reflex/components/chakra/layout/aspect_ratio.pyi
--rw-r--r--   0        0        0      755 2024-02-10 02:26:35.028940 reflex-0.4.7a1/reflex/components/chakra/layout/box.py
--rw-r--r--   0        0        0     3733 2024-04-02 19:14:34.416924 reflex-0.4.7a1/reflex/components/chakra/layout/box.pyi
--rw-r--r--   0        0        0     2967 2024-02-10 02:26:35.029073 reflex-0.4.7a1/reflex/components/chakra/layout/card.py
--rw-r--r--   0        0        0    14063 2024-04-02 19:14:34.417040 reflex-0.4.7a1/reflex/components/chakra/layout/card.pyi
--rw-r--r--   0        0        0      389 2024-02-10 02:26:35.029302 reflex-0.4.7a1/reflex/components/chakra/layout/center.py
--rw-r--r--   0        0        0     8905 2024-04-02 19:14:34.417147 reflex-0.4.7a1/reflex/components/chakra/layout/center.pyi
--rw-r--r--   0        0        0      354 2024-02-10 02:26:35.029446 reflex-0.4.7a1/reflex/components/chakra/layout/container.py
--rw-r--r--   0        0        0     3502 2024-04-02 19:14:34.417255 reflex-0.4.7a1/reflex/components/chakra/layout/container.pyi
--rw-r--r--   0        0        0      715 2024-02-10 02:26:35.029582 reflex-0.4.7a1/reflex/components/chakra/layout/flex.py
--rw-r--r--   0        0        0     4209 2024-04-02 19:14:34.417357 reflex-0.4.7a1/reflex/components/chakra/layout/flex.pyi
--rw-r--r--   0        0        0     4318 2024-02-10 02:26:35.029717 reflex-0.4.7a1/reflex/components/chakra/layout/grid.py
--rw-r--r--   0        0        0    14066 2024-04-02 19:14:34.417480 reflex-0.4.7a1/reflex/components/chakra/layout/grid.pyi
--rw-r--r--   0        0        0      179 2024-02-10 02:26:35.029946 reflex-0.4.7a1/reflex/components/chakra/layout/spacer.py
--rw-r--r--   0        0        0     3301 2024-04-02 19:14:34.417588 reflex-0.4.7a1/reflex/components/chakra/layout/spacer.pyi
--rw-r--r--   0        0        0     1077 2024-02-10 02:26:35.030045 reflex-0.4.7a1/reflex/components/chakra/layout/stack.py
--rw-r--r--   0        0        0    12432 2024-04-02 19:14:34.417697 reflex-0.4.7a1/reflex/components/chakra/layout/stack.pyi
--rw-r--r--   0        0        0     1463 2024-02-10 02:26:35.030152 reflex-0.4.7a1/reflex/components/chakra/layout/wrap.py
--rw-r--r--   0        0        0     7014 2024-04-02 19:14:34.417807 reflex-0.4.7a1/reflex/components/chakra/layout/wrap.pyi
--rw-r--r--   0        0        0      190 2024-02-10 02:26:35.030265 reflex-0.4.7a1/reflex/components/chakra/media/__init__.py
--rw-r--r--   0        0        0     1668 2024-02-10 02:26:35.030317 reflex-0.4.7a1/reflex/components/chakra/media/avatar.py
--rw-r--r--   0        0        0    10658 2024-04-02 19:14:34.417938 reflex-0.4.7a1/reflex/components/chakra/media/avatar.pyi
--rw-r--r--   0        0        0     2461 2024-02-10 02:26:35.030430 reflex-0.4.7a1/reflex/components/chakra/media/icon.py
--rw-r--r--   0        0        0     6342 2024-04-02 19:14:34.418161 reflex-0.4.7a1/reflex/components/chakra/media/icon.pyi
--rw-r--r--   0        0        0     2400 2024-02-10 02:26:35.030535 reflex-0.4.7a1/reflex/components/chakra/media/image.py
--rw-r--r--   0        0        0     5423 2024-04-02 19:14:34.418332 reflex-0.4.7a1/reflex/components/chakra/media/image.pyi
--rw-r--r--   0        0        0      419 2024-02-10 02:26:35.030653 reflex-0.4.7a1/reflex/components/chakra/navigation/__init__.py
--rw-r--r--   0        0        0     2925 2024-02-10 02:26:35.030704 reflex-0.4.7a1/reflex/components/chakra/navigation/breadcrumb.py
--rw-r--r--   0        0        0    13646 2024-04-02 19:14:34.418567 reflex-0.4.7a1/reflex/components/chakra/navigation/breadcrumb.pyi
--rw-r--r--   0        0        0     1475 2024-02-10 02:26:35.030830 reflex-0.4.7a1/reflex/components/chakra/navigation/link.py
--rw-r--r--   0        0        0     3999 2024-04-02 19:14:34.418745 reflex-0.4.7a1/reflex/components/chakra/navigation/link.pyi
--rw-r--r--   0        0        0      521 2024-02-10 02:26:35.031182 reflex-0.4.7a1/reflex/components/chakra/navigation/linkoverlay.py
--rw-r--r--   0        0        0     6375 2024-04-02 19:14:34.418852 reflex-0.4.7a1/reflex/components/chakra/navigation/linkoverlay.pyi
--rw-r--r--   0        0        0     2935 2024-02-10 02:26:35.031313 reflex-0.4.7a1/reflex/components/chakra/navigation/stepper.py
--rw-r--r--   0        0        0    28490 2024-04-02 19:14:34.418987 reflex-0.4.7a1/reflex/components/chakra/navigation/stepper.pyi
--rw-r--r--   0        0        0      850 2024-02-10 02:26:35.031514 reflex-0.4.7a1/reflex/components/chakra/overlay/__init__.py
--rw-r--r--   0        0        0     5200 2024-02-10 02:26:35.031625 reflex-0.4.7a1/reflex/components/chakra/overlay/alertdialog.py
--rw-r--r--   0        0        0    24411 2024-04-02 19:14:34.419146 reflex-0.4.7a1/reflex/components/chakra/overlay/alertdialog.pyi
--rw-r--r--   0        0        0     5186 2024-02-10 02:26:35.031772 reflex-0.4.7a1/reflex/components/chakra/overlay/drawer.py
--rw-r--r--   0        0        0    25832 2024-04-02 19:14:34.419276 reflex-0.4.7a1/reflex/components/chakra/overlay/drawer.pyi
--rw-r--r--   0        0        0     6974 2024-02-10 02:26:35.031928 reflex-0.4.7a1/reflex/components/chakra/overlay/menu.py
--rw-r--r--   0        0        0    29108 2024-04-02 19:14:34.419396 reflex-0.4.7a1/reflex/components/chakra/overlay/menu.pyi
--rw-r--r--   0        0        0     5270 2024-02-10 02:26:35.032050 reflex-0.4.7a1/reflex/components/chakra/overlay/modal.py
--rw-r--r--   0        0        0    23975 2024-04-02 19:14:34.419505 reflex-0.4.7a1/reflex/components/chakra/overlay/modal.pyi
--rw-r--r--   0        0        0     5967 2024-02-10 02:26:35.032202 reflex-0.4.7a1/reflex/components/chakra/overlay/popover.py
--rw-r--r--   0        0        0    30461 2024-04-02 19:14:34.419633 reflex-0.4.7a1/reflex/components/chakra/overlay/popover.pyi
--rw-r--r--   0        0        0     2127 2024-02-10 02:26:35.032416 reflex-0.4.7a1/reflex/components/chakra/overlay/tooltip.py
--rw-r--r--   0        0        0     6131 2024-04-02 19:14:34.419766 reflex-0.4.7a1/reflex/components/chakra/overlay/tooltip.pyi
--rw-r--r--   0        0        0      271 2024-02-10 02:26:35.032550 reflex-0.4.7a1/reflex/components/chakra/typography/__init__.py
--rw-r--r--   0        0        0      379 2024-02-10 02:26:35.032612 reflex-0.4.7a1/reflex/components/chakra/typography/heading.py
--rw-r--r--   0        0        0     3777 2024-04-02 19:14:34.419870 reflex-0.4.7a1/reflex/components/chakra/typography/heading.pyi
--rw-r--r--   0        0        0      671 2024-02-10 02:26:35.032741 reflex-0.4.7a1/reflex/components/chakra/typography/highlight.py
--rw-r--r--   0        0        0     3716 2024-04-02 19:14:34.419964 reflex-0.4.7a1/reflex/components/chakra/typography/highlight.pyi
--rw-r--r--   0        0        0      328 2024-02-10 02:26:35.032862 reflex-0.4.7a1/reflex/components/chakra/typography/span.py
--rw-r--r--   0        0        0     3443 2024-04-02 19:14:34.420093 reflex-0.4.7a1/reflex/components/chakra/typography/span.pyi
--rw-r--r--   0        0        0      472 2024-02-10 02:26:35.033013 reflex-0.4.7a1/reflex/components/chakra/typography/text.py
--rw-r--r--   0        0        0     3667 2024-04-02 19:14:34.420216 reflex-0.4.7a1/reflex/components/chakra/typography/text.pyi
--rw-r--r--   0        0        0    64790 2024-04-04 21:37:03.946766 reflex-0.4.7a1/reflex/components/component.py
--rw-r--r--   0        0        0      844 2024-04-02 19:14:34.421147 reflex-0.4.7a1/reflex/components/core/__init__.py
--rw-r--r--   0        0        0     5943 2024-04-04 21:37:03.946911 reflex-0.4.7a1/reflex/components/core/banner.py
--rw-r--r--   0        0        0    17164 2024-04-02 19:14:34.421397 reflex-0.4.7a1/reflex/components/core/banner.pyi
--rw-r--r--   0        0        0     1873 2024-02-10 02:26:35.034230 reflex-0.4.7a1/reflex/components/core/client_side_routing.py
--rw-r--r--   0        0        0     6406 2024-04-02 19:14:34.421550 reflex-0.4.7a1/reflex/components/core/client_side_routing.pyi
--rw-r--r--   0        0        0      590 2024-04-02 19:14:34.421679 reflex-0.4.7a1/reflex/components/core/colors.py
--rw-r--r--   0        0        0     6291 2024-04-02 19:14:34.422113 reflex-0.4.7a1/reflex/components/core/cond.py
--rw-r--r--   0        0        0     4642 2024-04-02 19:14:34.422253 reflex-0.4.7a1/reflex/components/core/debounce.py
--rw-r--r--   0        0        0     4149 2024-04-02 19:14:34.422370 reflex-0.4.7a1/reflex/components/core/debounce.pyi
--rw-r--r--   0        0        0     4031 2024-04-02 18:24:25.099624 reflex-0.4.7a1/reflex/components/core/foreach.py
--rw-r--r--   0        0        0     1033 2024-04-02 19:14:34.422562 reflex-0.4.7a1/reflex/components/core/html.py
--rw-r--r--   0        0        0     6616 2024-04-02 19:14:34.422669 reflex-0.4.7a1/reflex/components/core/html.pyi
--rw-r--r--   0        0        0       30 2024-02-10 02:26:35.035636 reflex-0.4.7a1/reflex/components/core/layout/__init__.py
--rw-r--r--   0        0        0     9989 2024-04-02 19:14:34.422836 reflex-0.4.7a1/reflex/components/core/match.py
--rw-r--r--   0        0        0     1907 2024-04-02 19:14:34.427781 reflex-0.4.7a1/reflex/components/core/responsive.py
--rw-r--r--   0        0        0     9000 2024-04-04 21:37:03.947039 reflex-0.4.7a1/reflex/components/core/upload.py
--rw-r--r--   0        0        0     8667 2024-04-02 19:14:34.429377 reflex-0.4.7a1/reflex/components/core/upload.pyi
--rw-r--r--   0        0        0      357 2024-04-04 21:37:03.947140 reflex-0.4.7a1/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0    11227 2024-04-02 19:14:34.430271 reflex-0.4.7a1/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0    31107 2024-04-02 19:14:34.430442 reflex-0.4.7a1/reflex/components/datadisplay/code.pyi
--rw-r--r--   0        0        0    12632 2024-02-10 02:26:35.036910 reflex-0.4.7a1/reflex/components/datadisplay/dataeditor.py
--rw-r--r--   0        0        0    10485 2024-04-02 19:14:34.430603 reflex-0.4.7a1/reflex/components/datadisplay/dataeditor.pyi
--rw-r--r--   0        0        0     2562 2024-04-04 21:37:03.947200 reflex-0.4.7a1/reflex/components/datadisplay/logo.py
--rw-r--r--   0        0        0       73 2024-02-07 01:47:48.949909 reflex-0.4.7a1/reflex/components/el/__init__.py
--rw-r--r--   0        0        0      113 2023-12-21 01:07:08.429460 reflex-0.4.7a1/reflex/components/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-12-21 01:07:08.429529 reflex-0.4.7a1/reflex/components/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-12-21 01:07:08.429622 reflex-0.4.7a1/reflex/components/el/constants/react.py
--rw-r--r--   0        0        0     1713 2023-12-21 01:07:08.429682 reflex-0.4.7a1/reflex/components/el/constants/reflex.py
--rw-r--r--   0        0        0      494 2023-12-21 01:07:08.429898 reflex-0.4.7a1/reflex/components/el/element.py
--rw-r--r--   0        0        0     3284 2024-04-02 19:14:34.430869 reflex-0.4.7a1/reflex/components/el/element.pyi
--rw-r--r--   0        0        0     3529 2024-04-02 19:14:34.432601 reflex-0.4.7a1/reflex/components/el/elements/__init__.py
--rw-r--r--   0        0        0     1982 2024-04-02 19:14:34.432772 reflex-0.4.7a1/reflex/components/el/elements/base.py
--rw-r--r--   0        0        0     6411 2024-04-02 19:14:34.432874 reflex-0.4.7a1/reflex/components/el/elements/base.pyi
--rw-r--r--   0        0        0    20102 2024-04-04 21:37:03.947356 reflex-0.4.7a1/reflex/components/el/elements/forms.py
--rw-r--r--   0        0        0   100476 2024-04-04 21:37:03.947614 reflex-0.4.7a1/reflex/components/el/elements/forms.pyi
--rw-r--r--   0        0        0     3610 2024-02-10 02:26:35.038470 reflex-0.4.7a1/reflex/components/el/elements/inline.py
--rw-r--r--   0        0        0   166595 2024-04-02 19:14:34.433892 reflex-0.4.7a1/reflex/components/el/elements/inline.pyi
--rw-r--r--   0        0        0     7929 2024-04-02 19:14:34.434037 reflex-0.4.7a1/reflex/components/el/elements/media.py
--rw-r--r--   0        0        0    94561 2024-04-02 19:14:34.434188 reflex-0.4.7a1/reflex/components/el/elements/media.pyi
--rw-r--r--   0        0        0     1337 2023-12-21 01:07:08.433098 reflex-0.4.7a1/reflex/components/el/elements/metadata.py
--rw-r--r--   0        0        0    28386 2024-04-02 19:14:34.434330 reflex-0.4.7a1/reflex/components/el/elements/metadata.pyi
--rw-r--r--   0        0        0     1569 2023-12-21 01:07:08.433349 reflex-0.4.7a1/reflex/components/el/elements/other.py
--rw-r--r--   0        0        0    42530 2024-04-02 19:14:34.434559 reflex-0.4.7a1/reflex/components/el/elements/other.pyi
--rw-r--r--   0        0        0     1406 2024-04-02 19:14:34.434672 reflex-0.4.7a1/reflex/components/el/elements/scripts.py
--rw-r--r--   0        0        0    19828 2024-04-02 19:14:34.434788 reflex-0.4.7a1/reflex/components/el/elements/scripts.pyi
--rw-r--r--   0        0        0     1535 2024-04-02 19:14:34.434940 reflex-0.4.7a1/reflex/components/el/elements/sectioning.py
--rw-r--r--   0        0        0    88307 2024-04-02 19:14:34.435104 reflex-0.4.7a1/reflex/components/el/elements/sectioning.pyi
--rw-r--r--   0        0        0     2767 2024-04-02 19:14:34.435250 reflex-0.4.7a1/reflex/components/el/elements/tables.py
--rw-r--r--   0        0        0    62559 2024-04-02 19:14:34.435538 reflex-0.4.7a1/reflex/components/el/elements/tables.pyi
--rw-r--r--   0        0        0     2432 2024-04-02 19:14:34.436021 reflex-0.4.7a1/reflex/components/el/elements/typography.py
--rw-r--r--   0        0        0    90180 2024-04-02 19:14:34.436215 reflex-0.4.7a1/reflex/components/el/elements/typography.pyi
--rw-r--r--   0        0        0       88 2024-02-10 02:26:35.040149 reflex-0.4.7a1/reflex/components/gridjs/__init__.py
--rw-r--r--   0        0        0     4300 2024-02-10 02:26:35.040226 reflex-0.4.7a1/reflex/components/gridjs/datatable.py
--rw-r--r--   0        0        0     7124 2024-04-02 19:14:34.436409 reflex-0.4.7a1/reflex/components/gridjs/datatable.pyi
--rw-r--r--   0        0        0      501 2024-02-10 02:26:35.040431 reflex-0.4.7a1/reflex/components/literals.py
--rw-r--r--   0        0        0       73 2024-02-10 02:26:35.040887 reflex-0.4.7a1/reflex/components/lucide/__init__.py
--rw-r--r--   0        0        0    34237 2024-04-04 21:37:03.947839 reflex-0.4.7a1/reflex/components/lucide/icon.py
--rw-r--r--   0        0        0    38020 2024-04-04 21:37:03.948033 reflex-0.4.7a1/reflex/components/lucide/icon.pyi
--rw-r--r--   0        0        0       87 2024-02-10 02:26:35.041813 reflex-0.4.7a1/reflex/components/markdown/__init__.py
--rw-r--r--   0        0        0    11448 2024-04-04 21:37:03.948197 reflex-0.4.7a1/reflex/components/markdown/markdown.py
--rw-r--r--   0        0        0     5278 2024-04-04 21:37:03.948324 reflex-0.4.7a1/reflex/components/markdown/markdown.pyi
--rw-r--r--   0        0        0       44 2024-02-10 02:26:35.042167 reflex-0.4.7a1/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      102 2024-02-10 02:26:35.042266 reflex-0.4.7a1/reflex/components/media/icon.py
--rw-r--r--   0        0        0       79 2024-02-10 02:26:35.042315 reflex-0.4.7a1/reflex/components/moment/__init__.py
--rw-r--r--   0        0        0     3925 2024-02-10 02:26:35.042375 reflex-0.4.7a1/reflex/components/moment/moment.py
--rw-r--r--   0        0        0     6870 2024-04-02 19:14:34.438557 reflex-0.4.7a1/reflex/components/moment/moment.pyi
--rw-r--r--   0        0        0      239 2024-02-10 02:26:35.042504 reflex-0.4.7a1/reflex/components/next/__init__.py
--rw-r--r--   0        0        0      189 2024-02-10 02:26:35.042549 reflex-0.4.7a1/reflex/components/next/base.py
--rw-r--r--   0        0        0     3304 2024-04-02 19:14:34.438775 reflex-0.4.7a1/reflex/components/next/base.pyi
--rw-r--r--   0        0        0     3831 2024-02-10 02:26:35.042660 reflex-0.4.7a1/reflex/components/next/image.py
--rw-r--r--   0        0        0     5795 2024-04-02 19:14:34.438919 reflex-0.4.7a1/reflex/components/next/image.pyi
--rw-r--r--   0        0        0      503 2024-02-10 02:26:35.042780 reflex-0.4.7a1/reflex/components/next/link.py
--rw-r--r--   0        0        0     3532 2024-04-02 19:14:34.439026 reflex-0.4.7a1/reflex/components/next/link.pyi
--rw-r--r--   0        0        0      730 2024-02-10 02:26:35.042905 reflex-0.4.7a1/reflex/components/next/video.py
--rw-r--r--   0        0        0     3429 2024-04-02 19:14:34.439128 reflex-0.4.7a1/reflex/components/next/video.pyi
--rw-r--r--   0        0        0       77 2024-02-10 02:26:35.043030 reflex-0.4.7a1/reflex/components/plotly/__init__.py
--rw-r--r--   0        0        0      964 2024-04-02 19:14:34.439545 reflex-0.4.7a1/reflex/components/plotly/plotly.py
--rw-r--r--   0        0        0     7007 2024-04-02 19:14:34.439682 reflex-0.4.7a1/reflex/components/plotly/plotly.pyi
--rw-r--r--   0        0        0      112 2024-04-02 19:14:34.440146 reflex-0.4.7a1/reflex/components/radix/__init__.py
--rw-r--r--   0        0        0      214 2024-04-02 19:14:34.440350 reflex-0.4.7a1/reflex/components/radix/primitives/__init__.py
--rw-r--r--   0        0        0    21406 2024-04-02 19:14:34.440707 reflex-0.4.7a1/reflex/components/radix/primitives/accordion.py
--rw-r--r--   0        0        0    26956 2024-04-02 19:14:34.440903 reflex-0.4.7a1/reflex/components/radix/primitives/accordion.pyi
--rw-r--r--   0        0        0      869 2024-02-10 02:26:35.044768 reflex-0.4.7a1/reflex/components/radix/primitives/base.py
--rw-r--r--   0        0        0     6620 2024-04-02 19:14:34.441366 reflex-0.4.7a1/reflex/components/radix/primitives/base.pyi
--rw-r--r--   0        0        0     8660 2024-04-02 19:14:34.442162 reflex-0.4.7a1/reflex/components/radix/primitives/drawer.py
--rw-r--r--   0        0        0    34981 2024-04-02 19:14:34.442473 reflex-0.4.7a1/reflex/components/radix/primitives/drawer.pyi
--rw-r--r--   0        0        0     4760 2024-04-02 19:14:34.442846 reflex-0.4.7a1/reflex/components/radix/primitives/form.py
--rw-r--r--   0        0        0    48365 2024-04-02 19:14:34.443076 reflex-0.4.7a1/reflex/components/radix/primitives/form.pyi
--rw-r--r--   0        0        0     3996 2024-04-02 19:14:34.443510 reflex-0.4.7a1/reflex/components/radix/primitives/progress.py
--rw-r--r--   0        0        0    22997 2024-04-02 19:14:34.444066 reflex-0.4.7a1/reflex/components/radix/primitives/progress.pyi
--rw-r--r--   0        0        0     5004 2024-04-02 19:14:34.444533 reflex-0.4.7a1/reflex/components/radix/primitives/slider.py
--rw-r--r--   0        0        0    17052 2024-04-02 19:14:34.444665 reflex-0.4.7a1/reflex/components/radix/primitives/slider.pyi
--rw-r--r--   0        0        0      292 2024-04-02 19:14:34.444811 reflex-0.4.7a1/reflex/components/radix/themes/__init__.py
--rw-r--r--   0        0        0     8097 2024-04-02 19:14:34.445088 reflex-0.4.7a1/reflex/components/radix/themes/base.py
--rw-r--r--   0        0        0    24216 2024-04-02 19:14:34.445340 reflex-0.4.7a1/reflex/components/radix/themes/base.pyi
--rw-r--r--   0        0        0     3007 2024-04-02 19:14:34.445446 reflex-0.4.7a1/reflex/components/radix/themes/color_mode.py
--rw-r--r--   0        0        0    21283 2024-04-02 19:14:34.445570 reflex-0.4.7a1/reflex/components/radix/themes/color_mode.pyi
--rw-r--r--   0        0        0     1776 2024-04-02 19:14:34.445724 reflex-0.4.7a1/reflex/components/radix/themes/components/__init__.py
--rw-r--r--   0        0        0     3267 2024-04-02 19:14:34.446644 reflex-0.4.7a1/reflex/components/radix/themes/components/alert_dialog.py
--rw-r--r--   0        0        0    24434 2024-04-02 19:14:34.446757 reflex-0.4.7a1/reflex/components/radix/themes/components/alert_dialog.pyi
--rw-r--r--   0        0        0    40237 2024-04-02 19:14:34.447529 reflex-0.4.7a1/reflex/components/radix/themes/components/alertdialog.pyi
--rw-r--r--   0        0        0      400 2024-04-02 19:14:34.447703 reflex-0.4.7a1/reflex/components/radix/themes/components/aspect_ratio.py
--rw-r--r--   0        0        0     3640 2024-04-02 19:14:34.447802 reflex-0.4.7a1/reflex/components/radix/themes/components/aspect_ratio.pyi
--rw-r--r--   0        0        0     5724 2024-04-02 19:14:34.448082 reflex-0.4.7a1/reflex/components/radix/themes/components/aspectratio.pyi
--rw-r--r--   0        0        0      989 2024-04-02 19:14:34.448493 reflex-0.4.7a1/reflex/components/radix/themes/components/avatar.py
--rw-r--r--   0        0        0     6562 2024-04-02 19:14:34.448953 reflex-0.4.7a1/reflex/components/radix/themes/components/avatar.pyi
--rw-r--r--   0        0        0      815 2024-04-02 19:14:34.449058 reflex-0.4.7a1/reflex/components/radix/themes/components/badge.py
--rw-r--r--   0        0        0     9315 2024-04-02 19:14:34.449155 reflex-0.4.7a1/reflex/components/radix/themes/components/badge.pyi
--rw-r--r--   0        0        0     1084 2024-04-02 19:14:34.449285 reflex-0.4.7a1/reflex/components/radix/themes/components/button.py
--rw-r--r--   0        0        0    11758 2024-04-02 19:14:34.449372 reflex-0.4.7a1/reflex/components/radix/themes/components/button.pyi
--rw-r--r--   0        0        0     2378 2024-04-02 19:14:34.449904 reflex-0.4.7a1/reflex/components/radix/themes/components/callout.py
--rw-r--r--   0        0        0    38710 2024-04-02 19:14:34.450185 reflex-0.4.7a1/reflex/components/radix/themes/components/callout.pyi
--rw-r--r--   0        0        0      659 2024-04-02 19:14:34.450330 reflex-0.4.7a1/reflex/components/radix/themes/components/card.py
--rw-r--r--   0        0        0     7200 2024-04-02 19:14:34.450427 reflex-0.4.7a1/reflex/components/radix/themes/components/card.pyi
--rw-r--r--   0        0        0     4679 2024-04-02 19:14:34.451369 reflex-0.4.7a1/reflex/components/radix/themes/components/checkbox.py
--rw-r--r--   0        0        0    20877 2024-04-02 19:14:34.451567 reflex-0.4.7a1/reflex/components/radix/themes/components/checkbox.pyi
--rw-r--r--   0        0        0     5049 2024-04-02 19:14:34.451786 reflex-0.4.7a1/reflex/components/radix/themes/components/context_menu.py
--rw-r--r--   0        0        0    31192 2024-04-02 19:14:34.451890 reflex-0.4.7a1/reflex/components/radix/themes/components/context_menu.pyi
--rw-r--r--   0        0        0    44130 2024-04-02 19:14:34.452056 reflex-0.4.7a1/reflex/components/radix/themes/components/contextmenu.pyi
--rw-r--r--   0        0        0     2600 2024-04-02 19:14:34.452261 reflex-0.4.7a1/reflex/components/radix/themes/components/dialog.py
--rw-r--r--   0        0        0    24895 2024-04-02 19:14:34.452419 reflex-0.4.7a1/reflex/components/radix/themes/components/dialog.pyi
--rw-r--r--   0        0        0    11256 2024-04-02 19:14:34.452696 reflex-0.4.7a1/reflex/components/radix/themes/components/dropdown_menu.py
--rw-r--r--   0        0        0    37901 2024-04-02 19:14:34.452840 reflex-0.4.7a1/reflex/components/radix/themes/components/dropdown_menu.pyi
--rw-r--r--   0        0        0    52185 2024-04-02 19:14:34.453086 reflex-0.4.7a1/reflex/components/radix/themes/components/dropdownmenu.pyi
--rw-r--r--   0        0        0     2405 2024-04-02 19:14:34.453445 reflex-0.4.7a1/reflex/components/radix/themes/components/hover_card.py
--rw-r--r--   0        0        0    17744 2024-04-02 19:14:34.453581 reflex-0.4.7a1/reflex/components/radix/themes/components/hover_card.pyi
--rw-r--r--   0        0        0    26453 2024-04-02 19:14:34.453788 reflex-0.4.7a1/reflex/components/radix/themes/components/hovercard.pyi
--rw-r--r--   0        0        0     2789 2024-04-02 19:14:34.454202 reflex-0.4.7a1/reflex/components/radix/themes/components/icon_button.py
--rw-r--r--   0        0        0    11916 2024-04-02 19:14:34.454271 reflex-0.4.7a1/reflex/components/radix/themes/components/icon_button.pyi
--rw-r--r--   0        0        0    12021 2024-04-02 19:14:34.454397 reflex-0.4.7a1/reflex/components/radix/themes/components/iconbutton.pyi
--rw-r--r--   0        0        0     1015 2024-04-02 19:14:34.454891 reflex-0.4.7a1/reflex/components/radix/themes/components/inset.py
--rw-r--r--   0        0        0     7889 2024-04-02 19:14:34.455045 reflex-0.4.7a1/reflex/components/radix/themes/components/inset.pyi
--rw-r--r--   0        0        0     3177 2024-04-02 19:14:34.455306 reflex-0.4.7a1/reflex/components/radix/themes/components/popover.py
--rw-r--r--   0        0        0    17404 2024-04-02 19:14:34.455466 reflex-0.4.7a1/reflex/components/radix/themes/components/popover.pyi
--rw-r--r--   0        0        0     6253 2024-04-02 19:14:34.455911 reflex-0.4.7a1/reflex/components/radix/themes/components/radio_group.py
--rw-r--r--   0        0        0    24106 2024-04-02 19:14:34.456002 reflex-0.4.7a1/reflex/components/radix/themes/components/radio_group.pyi
--rw-r--r--   0        0        0    26222 2024-04-02 19:14:34.457988 reflex-0.4.7a1/reflex/components/radix/themes/components/radiogroup.pyi
--rw-r--r--   0        0        0      920 2024-04-02 19:14:34.458077 reflex-0.4.7a1/reflex/components/radix/themes/components/scroll_area.py
--rw-r--r--   0        0        0     4427 2024-04-02 19:14:34.458156 reflex-0.4.7a1/reflex/components/radix/themes/components/scroll_area.pyi
--rw-r--r--   0        0        0     6513 2024-04-02 19:14:34.458390 reflex-0.4.7a1/reflex/components/radix/themes/components/scrollarea.pyi
--rw-r--r--   0        0        0     8028 2024-04-04 21:37:03.948474 reflex-0.4.7a1/reflex/components/radix/themes/components/select.py
--rw-r--r--   0        0        0    45123 2024-04-02 19:14:34.459754 reflex-0.4.7a1/reflex/components/radix/themes/components/select.pyi
--rw-r--r--   0        0        0      868 2024-04-02 19:14:34.459929 reflex-0.4.7a1/reflex/components/radix/themes/components/separator.py
--rw-r--r--   0        0        0     6078 2024-04-02 19:14:34.460031 reflex-0.4.7a1/reflex/components/radix/themes/components/separator.pyi
--rw-r--r--   0        0        0     3234 2024-04-02 19:14:34.460186 reflex-0.4.7a1/reflex/components/radix/themes/components/slider.py
--rw-r--r--   0        0        0     8162 2024-04-02 19:14:34.460283 reflex-0.4.7a1/reflex/components/radix/themes/components/slider.pyi
--rw-r--r--   0        0        0     1976 2024-04-02 19:14:34.460390 reflex-0.4.7a1/reflex/components/radix/themes/components/switch.py
--rw-r--r--   0        0        0     7404 2024-04-02 19:14:34.460484 reflex-0.4.7a1/reflex/components/radix/themes/components/switch.pyi
--rw-r--r--   0        0        0     3111 2024-04-02 19:14:34.460743 reflex-0.4.7a1/reflex/components/radix/themes/components/table.py
--rw-r--r--   0        0        0    47387 2024-04-02 19:14:34.460872 reflex-0.4.7a1/reflex/components/radix/themes/components/table.pyi
--rw-r--r--   0        0        0     2213 2024-04-02 19:14:34.463534 reflex-0.4.7a1/reflex/components/radix/themes/components/tabs.py
--rw-r--r--   0        0        0    17321 2024-04-02 19:14:34.463662 reflex-0.4.7a1/reflex/components/radix/themes/components/tabs.pyi
--rw-r--r--   0        0        0     3233 2024-04-02 19:14:34.463765 reflex-0.4.7a1/reflex/components/radix/themes/components/text_area.py
--rw-r--r--   0        0        0    11711 2024-04-02 19:14:34.463961 reflex-0.4.7a1/reflex/components/radix/themes/components/text_area.pyi
--rw-r--r--   0        0        0     5106 2024-04-02 19:14:34.464711 reflex-0.4.7a1/reflex/components/radix/themes/components/text_field.py
--rw-r--r--   0        0        0    43043 2024-04-02 19:14:34.464805 reflex-0.4.7a1/reflex/components/radix/themes/components/text_field.pyi
--rw-r--r--   0        0        0    43365 2024-04-02 19:14:34.464956 reflex-0.4.7a1/reflex/components/radix/themes/components/textfield.pyi
--rw-r--r--   0        0        0     4465 2024-04-02 19:14:34.465166 reflex-0.4.7a1/reflex/components/radix/themes/components/tooltip.py
--rw-r--r--   0        0        0     8092 2024-04-02 19:14:34.465305 reflex-0.4.7a1/reflex/components/radix/themes/components/tooltip.pyi
--rw-r--r--   0        0        0      811 2024-04-02 19:14:34.465647 reflex-0.4.7a1/reflex/components/radix/themes/layout/__init__.py
--rw-r--r--   0        0        0     1201 2024-04-02 19:14:34.465990 reflex-0.4.7a1/reflex/components/radix/themes/layout/base.py
--rw-r--r--   0        0        0     7643 2024-04-02 19:14:34.466154 reflex-0.4.7a1/reflex/components/radix/themes/layout/base.pyi
--rw-r--r--   0        0        0      281 2024-02-10 02:26:35.060028 reflex-0.4.7a1/reflex/components/radix/themes/layout/box.py
--rw-r--r--   0        0        0     6462 2024-04-02 19:14:34.466266 reflex-0.4.7a1/reflex/components/radix/themes/layout/box.pyi
--rw-r--r--   0        0        0      422 2024-04-02 19:14:34.466627 reflex-0.4.7a1/reflex/components/radix/themes/layout/center.py
--rw-r--r--   0        0        0     8245 2024-04-02 19:14:34.466794 reflex-0.4.7a1/reflex/components/radix/themes/layout/center.pyi
--rw-r--r--   0        0        0      552 2024-02-10 02:26:35.060445 reflex-0.4.7a1/reflex/components/radix/themes/layout/container.py
--rw-r--r--   0        0        0     6779 2024-04-02 19:14:34.466930 reflex-0.4.7a1/reflex/components/radix/themes/layout/container.pyi
--rw-r--r--   0        0        0     1374 2024-04-02 19:14:34.467197 reflex-0.4.7a1/reflex/components/radix/themes/layout/flex.py
--rw-r--r--   0        0        0     8501 2024-04-02 19:14:34.467710 reflex-0.4.7a1/reflex/components/radix/themes/layout/flex.pyi
--rw-r--r--   0        0        0     1498 2024-04-02 19:14:34.468616 reflex-0.4.7a1/reflex/components/radix/themes/layout/grid.py
--rw-r--r--   0        0        0     8907 2024-04-02 19:14:34.468790 reflex-0.4.7a1/reflex/components/radix/themes/layout/grid.pyi
--rw-r--r--   0        0        0     4889 2024-04-02 19:14:34.469076 reflex-0.4.7a1/reflex/components/radix/themes/layout/list.py
--rw-r--r--   0        0        0    29367 2024-04-02 19:14:34.469203 reflex-0.4.7a1/reflex/components/radix/themes/layout/list.pyi
--rw-r--r--   0        0        0      458 2024-02-10 02:26:35.060937 reflex-0.4.7a1/reflex/components/radix/themes/layout/section.py
--rw-r--r--   0        0        0     6758 2024-04-02 19:14:34.469367 reflex-0.4.7a1/reflex/components/radix/themes/layout/section.pyi
--rw-r--r--   0        0        0      412 2024-04-02 19:14:34.469593 reflex-0.4.7a1/reflex/components/radix/themes/layout/spacer.py
--rw-r--r--   0        0        0     8245 2024-04-02 19:14:34.469727 reflex-0.4.7a1/reflex/components/radix/themes/layout/spacer.pyi
--rw-r--r--   0        0        0     1270 2024-04-02 19:14:34.469849 reflex-0.4.7a1/reflex/components/radix/themes/layout/stack.py
--rw-r--r--   0        0        0    22132 2024-04-02 19:14:34.470027 reflex-0.4.7a1/reflex/components/radix/themes/layout/stack.pyi
--rw-r--r--   0        0        0      343 2024-04-02 19:14:34.470193 reflex-0.4.7a1/reflex/components/radix/themes/typography/__init__.py
--rw-r--r--   0        0        0      408 2024-02-10 02:26:35.061693 reflex-0.4.7a1/reflex/components/radix/themes/typography/base.py
--rw-r--r--   0        0        0      799 2024-02-10 02:26:35.061822 reflex-0.4.7a1/reflex/components/radix/themes/typography/blockquote.py
--rw-r--r--   0        0        0     9316 2024-04-02 19:14:34.470311 reflex-0.4.7a1/reflex/components/radix/themes/typography/blockquote.pyi
--rw-r--r--   0        0        0      909 2024-02-10 02:26:35.062001 reflex-0.4.7a1/reflex/components/radix/themes/typography/code.py
--rw-r--r--   0        0        0     9513 2024-04-02 19:14:34.470410 reflex-0.4.7a1/reflex/components/radix/themes/typography/code.pyi
--rw-r--r--   0        0        0     8547 2024-04-02 19:14:34.470588 reflex-0.4.7a1/reflex/components/radix/themes/typography/em.pyi
--rw-r--r--   0        0        0     1324 2024-02-10 02:26:35.062444 reflex-0.4.7a1/reflex/components/radix/themes/typography/heading.py
--rw-r--r--   0        0        0    10106 2024-04-02 19:14:34.470692 reflex-0.4.7a1/reflex/components/radix/themes/typography/heading.pyi
--rw-r--r--   0        0        0     8872 2024-04-02 19:14:34.470802 reflex-0.4.7a1/reflex/components/radix/themes/typography/kbd.pyi
--rw-r--r--   0        0        0     3154 2024-04-02 19:14:34.471091 reflex-0.4.7a1/reflex/components/radix/themes/typography/link.py
--rw-r--r--   0        0        0    12063 2024-04-02 19:14:34.471230 reflex-0.4.7a1/reflex/components/radix/themes/typography/link.pyi
--rw-r--r--   0        0        0     8701 2024-04-02 19:14:34.471467 reflex-0.4.7a1/reflex/components/radix/themes/typography/quote.pyi
--rw-r--r--   0        0        0     8563 2024-04-02 19:14:34.471621 reflex-0.4.7a1/reflex/components/radix/themes/typography/strong.pyi
--rw-r--r--   0        0        0     2604 2024-04-02 19:14:34.472005 reflex-0.4.7a1/reflex/components/radix/themes/typography/text.py
--rw-r--r--   0        0        0    57238 2024-04-02 19:14:34.472171 reflex-0.4.7a1/reflex/components/radix/themes/typography/text.pyi
--rw-r--r--   0        0        0      144 2024-02-10 02:26:35.063629 reflex-0.4.7a1/reflex/components/react_player/__init__.py
--rw-r--r--   0        0        0      185 2024-02-10 02:26:35.063689 reflex-0.4.7a1/reflex/components/react_player/audio.py
--rw-r--r--   0        0        0     4398 2024-04-02 19:14:34.472284 reflex-0.4.7a1/reflex/components/react_player/audio.pyi
--rw-r--r--   0        0        0     1087 2024-02-10 02:26:35.063804 reflex-0.4.7a1/reflex/components/react_player/react_player.py
--rw-r--r--   0        0        0     4425 2024-04-02 19:14:34.472391 reflex-0.4.7a1/reflex/components/react_player/react_player.pyi
--rw-r--r--   0        0        0      185 2024-02-10 02:26:35.063907 reflex-0.4.7a1/reflex/components/react_player/video.py
--rw-r--r--   0        0        0     4398 2024-04-02 19:14:34.472479 reflex-0.4.7a1/reflex/components/react_player/video.pyi
--rw-r--r--   0        0        0     2373 2024-02-10 02:26:35.064033 reflex-0.4.7a1/reflex/components/recharts/__init__.py
--rw-r--r--   0        0        0    19595 2024-02-10 02:26:35.064126 reflex-0.4.7a1/reflex/components/recharts/cartesian.py
--rw-r--r--   0        0        0    85500 2024-04-02 19:14:34.472660 reflex-0.4.7a1/reflex/components/recharts/cartesian.pyi
--rw-r--r--   0        0        0    18493 2024-02-10 02:26:35.064337 reflex-0.4.7a1/reflex/components/recharts/charts.py
--rw-r--r--   0        0        0    48757 2024-04-02 19:14:34.472846 reflex-0.4.7a1/reflex/components/recharts/charts.pyi
--rw-r--r--   0        0        0     5624 2024-02-10 02:26:35.064489 reflex-0.4.7a1/reflex/components/recharts/general.py
--rw-r--r--   0        0        0    23071 2024-04-02 19:14:34.472964 reflex-0.4.7a1/reflex/components/recharts/general.pyi
--rw-r--r--   0        0        0    10410 2024-02-10 02:26:35.064657 reflex-0.4.7a1/reflex/components/recharts/polar.py
--rw-r--r--   0        0        0    24752 2024-04-02 19:14:34.473068 reflex-0.4.7a1/reflex/components/recharts/polar.pyi
--rw-r--r--   0        0        0     2870 2024-02-10 02:26:35.064789 reflex-0.4.7a1/reflex/components/recharts/recharts.py
--rw-r--r--   0        0        0     8606 2024-04-02 19:14:34.473190 reflex-0.4.7a1/reflex/components/recharts/recharts.pyi
--rw-r--r--   0        0        0      109 2024-02-10 02:26:35.064909 reflex-0.4.7a1/reflex/components/suneditor/__init__.py
--rw-r--r--   0        0        0     7360 2024-02-10 02:26:35.064985 reflex-0.4.7a1/reflex/components/suneditor/editor.py
--rw-r--r--   0        0        0    10330 2024-04-02 19:14:34.473324 reflex-0.4.7a1/reflex/components/suneditor/editor.pyi
--rw-r--r--   0        0        0      152 2024-02-10 02:26:35.065200 reflex-0.4.7a1/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-12-21 01:07:08.463011 reflex-0.4.7a1/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3620 2024-02-10 02:26:35.065323 reflex-0.4.7a1/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0      387 2024-02-10 02:26:35.065376 reflex-0.4.7a1/reflex/components/tags/match_tag.py
--rw-r--r--   0        0        0     2778 2024-04-02 19:14:34.473664 reflex-0.4.7a1/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-12-21 01:07:08.463394 reflex-0.4.7a1/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0    11082 2024-04-04 21:37:03.948613 reflex-0.4.7a1/reflex/config.py
--rw-r--r--   0        0        0     3318 2024-04-04 21:37:03.948873 reflex-0.4.7a1/reflex/config.pyi
--rw-r--r--   0        0        0     2036 2024-04-02 19:14:34.474441 reflex-0.4.7a1/reflex/constants/__init__.py
--rw-r--r--   0        0        0     5640 2024-04-04 22:32:02.761988 reflex-0.4.7a1/reflex/constants/base.py
--rw-r--r--   0        0        0     2980 2024-04-04 22:32:02.762262 reflex-0.4.7a1/reflex/constants/base.pyi
--rw-r--r--   0        0        0     1599 2024-04-02 19:14:34.474865 reflex-0.4.7a1/reflex/constants/colors.py
--rw-r--r--   0        0        0     4137 2024-04-04 21:37:03.949234 reflex-0.4.7a1/reflex/constants/compiler.py
--rw-r--r--   0        0        0     1331 2024-02-10 02:26:35.066956 reflex-0.4.7a1/reflex/constants/config.py
--rw-r--r--   0        0        0     1268 2024-04-02 19:14:34.475565 reflex-0.4.7a1/reflex/constants/custom_components.py
--rw-r--r--   0        0        0     2668 2024-02-10 02:26:35.067613 reflex-0.4.7a1/reflex/constants/event.py
--rw-r--r--   0        0        0     3177 2024-04-02 19:14:34.475856 reflex-0.4.7a1/reflex/constants/installer.py
--rw-r--r--   0        0        0     1940 2024-04-02 19:14:34.476122 reflex-0.4.7a1/reflex/constants/route.py
--rw-r--r--   0        0        0      636 2024-02-10 02:26:35.067842 reflex-0.4.7a1/reflex/constants/style.py
--rw-r--r--   0        0        0       36 2024-04-02 19:14:34.476236 reflex-0.4.7a1/reflex/custom_components/__init__.py
--rw-r--r--   0        0        0    32034 2024-04-04 22:32:02.762748 reflex-0.4.7a1/reflex/custom_components/custom_components.py
--rw-r--r--   0        0        0    26634 2024-04-04 20:48:44.974653 reflex-0.4.7a1/reflex/event.py
--rw-r--r--   0        0        0      287 2024-04-04 21:37:03.949637 reflex-0.4.7a1/reflex/experimental/__init__.py
--rw-r--r--   0        0        0     1647 2024-04-04 21:37:03.949706 reflex-0.4.7a1/reflex/experimental/hooks.py
--rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.4.7a1/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1484 2024-04-02 19:14:34.477238 reflex-0.4.7a1/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1169 2023-12-04 22:31:51.618237 reflex-0.4.7a1/reflex/middleware/middleware.py
--rw-r--r--   0        0        0    13091 2024-04-02 19:14:34.477579 reflex-0.4.7a1/reflex/model.py
--rw-r--r--   0        0        0     1921 2024-04-04 21:37:03.949824 reflex-0.4.7a1/reflex/page.py
--rw-r--r--   0        0        0    17871 2024-04-04 22:32:02.763178 reflex-0.4.7a1/reflex/reflex.py
--rw-r--r--   0        0        0     2908 2024-04-02 19:14:34.478054 reflex-0.4.7a1/reflex/route.py
--rw-r--r--   0        0        0   105642 2024-04-02 19:14:34.478448 reflex-0.4.7a1/reflex/state.py
--rw-r--r--   0        0        0     8834 2024-04-04 21:37:03.950185 reflex-0.4.7a1/reflex/style.py
--rw-r--r--   0        0        0    29808 2024-04-04 22:32:02.763768 reflex-0.4.7a1/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-11-07 19:58:07.486037 reflex-0.4.7a1/reflex/utils/__init__.py
--rw-r--r--   0        0        0     8573 2024-02-10 02:26:35.070031 reflex-0.4.7a1/reflex/utils/build.py
--rw-r--r--   0        0        0     5018 2024-04-04 22:32:02.764358 reflex-0.4.7a1/reflex/utils/console.py
--rw-r--r--   0        0        0      504 2024-02-10 02:26:35.070129 reflex-0.4.7a1/reflex/utils/exceptions.py
--rw-r--r--   0        0        0     9969 2024-04-04 21:37:03.950843 reflex-0.4.7a1/reflex/utils/exec.py
--rw-r--r--   0        0        0     2357 2024-04-04 21:37:03.951057 reflex-0.4.7a1/reflex/utils/export.py
--rw-r--r--   0        0        0    22648 2024-04-02 19:14:34.479804 reflex-0.4.7a1/reflex/utils/format.py
--rw-r--r--   0        0        0     1919 2023-12-04 22:31:51.620673 reflex-0.4.7a1/reflex/utils/imports.py
--rw-r--r--   0        0        0     4737 2024-02-10 02:26:35.070893 reflex-0.4.7a1/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    45683 2024-04-04 22:32:02.765051 reflex-0.4.7a1/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     8481 2024-04-04 21:37:03.951498 reflex-0.4.7a1/reflex/utils/processes.py
--rw-r--r--   0        0        0    27674 2024-04-02 19:14:34.480893 reflex-0.4.7a1/reflex/utils/pyi_generator.py
--rw-r--r--   0        0        0     8538 2024-04-02 19:14:34.481008 reflex-0.4.7a1/reflex/utils/serializers.py
--rw-r--r--   0        0        0     4013 2024-04-04 21:37:03.951599 reflex-0.4.7a1/reflex/utils/telemetry.py
--rw-r--r--   0        0        0    13585 2024-04-02 19:14:34.481602 reflex-0.4.7a1/reflex/utils/types.py
--rw-r--r--   0        0        0     2609 2023-11-21 01:55:15.773146 reflex-0.4.7a1/reflex/utils/watch.py
--rw-r--r--   0        0        0    67152 2024-04-04 21:37:03.951876 reflex-0.4.7a1/reflex/vars.py
--rw-r--r--   0        0        0     5583 2024-04-04 21:37:03.951997 reflex-0.4.7a1/reflex/vars.pyi
--rw-r--r--   0        0        0    11815 1970-01-01 00:00:00.000000 reflex-0.4.7a1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.4.7a2/LICENSE
+-rw-r--r--   0        0        0     9568 2024-04-04 21:37:03.943217 reflex-0.4.7a2/README.md
+-rw-r--r--   0        0        0     2922 2024-04-08 21:11:30.570683 reflex-0.4.7a2/pyproject.toml
+-rw-r--r--   0        0        0     4286 2023-11-07 19:58:07.469572 reflex-0.4.7a2/reflex/.templates/apps/blank/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-11-07 19:58:07.469657 reflex-0.4.7a2/reflex/.templates/apps/blank/code/__init__.py
+-rw-r--r--   0        0        0      861 2024-04-05 00:24:11.496563 reflex-0.4.7a2/reflex/.templates/apps/blank/code/blank.py
+-rw-r--r--   0        0        0       32 2023-11-07 19:58:07.469933 reflex-0.4.7a2/reflex/.templates/apps/demo/.gitignore
+-rw-r--r--   0        0        0     4286 2023-11-07 19:58:07.470079 reflex-0.4.7a2/reflex/.templates/apps/demo/assets/favicon.ico
+-rw-r--r--   0        0        0     1475 2023-11-07 19:58:07.470183 reflex-0.4.7a2/reflex/.templates/apps/demo/assets/github.svg
+-rw-r--r--   0        0        0     1899 2023-11-07 19:58:07.470263 reflex-0.4.7a2/reflex/.templates/apps/demo/assets/icon.svg
+-rw-r--r--   0        0        0     5403 2023-11-07 19:58:07.470351 reflex-0.4.7a2/reflex/.templates/apps/demo/assets/logo.svg
+-rw-r--r--   0        0        0      807 2023-11-07 19:58:07.470441 reflex-0.4.7a2/reflex/.templates/apps/demo/assets/paneleft.svg
+-rw-r--r--   0        0        0       32 2023-11-07 19:58:07.470556 reflex-0.4.7a2/reflex/.templates/apps/demo/code/__init__.py
+-rw-r--r--   0        0        0     2928 2024-04-02 19:14:34.394285 reflex-0.4.7a2/reflex/.templates/apps/demo/code/demo.py
+-rw-r--r--   0        0        0      194 2023-11-07 19:58:07.470763 reflex-0.4.7a2/reflex/.templates/apps/demo/code/pages/__init__.py
+-rw-r--r--   0        0        0      706 2024-04-02 19:14:34.394398 reflex-0.4.7a2/reflex/.templates/apps/demo/code/pages/chatapp.py
+-rw-r--r--   0        0        0    10910 2024-04-02 19:14:34.394812 reflex-0.4.7a2/reflex/.templates/apps/demo/code/pages/datatable.py
+-rw-r--r--   0        0        0     8383 2024-04-02 19:14:34.395299 reflex-0.4.7a2/reflex/.templates/apps/demo/code/pages/forms.py
+-rw-r--r--   0        0        0     8519 2024-04-02 19:14:34.395551 reflex-0.4.7a2/reflex/.templates/apps/demo/code/pages/graphing.py
+-rw-r--r--   0        0        0     1822 2024-04-02 19:14:34.395723 reflex-0.4.7a2/reflex/.templates/apps/demo/code/pages/home.py
+-rw-r--r--   0        0        0     4722 2024-04-02 19:14:34.395853 reflex-0.4.7a2/reflex/.templates/apps/demo/code/sidebar.py
+-rw-r--r--   0        0        0      510 2023-11-07 19:58:07.471657 reflex-0.4.7a2/reflex/.templates/apps/demo/code/state.py
+-rw-r--r--   0        0        0      912 2023-11-07 19:58:07.471802 reflex-0.4.7a2/reflex/.templates/apps/demo/code/states/form_state.py
+-rw-r--r--   0        0        0     1189 2023-11-07 19:58:07.471905 reflex-0.4.7a2/reflex/.templates/apps/demo/code/states/pie_state.py
+-rw-r--r--   0        0        0     1486 2024-04-02 19:14:34.395963 reflex-0.4.7a2/reflex/.templates/apps/demo/code/styles.py
+-rw-r--r--   0        0        0        0 2023-11-07 19:58:07.472085 reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/__init__.py
+-rw-r--r--   0        0        0      120 2023-11-07 19:58:07.472204 reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/components/__init__.py
+-rw-r--r--   0        0        0     3584 2024-04-02 19:14:34.396085 reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/components/chat.py
+-rw-r--r--   0        0        0      680 2023-11-07 19:58:07.472372 reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
+-rw-r--r--   0        0        0     1829 2024-04-02 19:14:34.396198 reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/components/modal.py
+-rw-r--r--   0        0        0     2251 2024-04-02 19:14:34.396306 reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/components/navbar.py
+-rw-r--r--   0        0        0     1735 2024-04-02 19:14:34.396392 reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/components/sidebar.py
+-rw-r--r--   0        0        0     4001 2023-11-07 19:58:07.472705 reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/state.py
+-rw-r--r--   0        0        0     2281 2024-04-02 19:14:34.396499 reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/styles.py
+-rw-r--r--   0        0        0       74 2023-09-18 23:00:36.695709 reflex-0.4.7a2/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      127 2024-04-02 19:14:34.400175 reflex-0.4.7a2/reflex/.templates/jinja/custom_components/README.md.jinja2
+-rw-r--r--   0        0        0       32 2024-04-02 19:14:34.401028 reflex-0.4.7a2/reflex/.templates/jinja/custom_components/__init__.py.jinja2
+-rw-r--r--   0        0        0      826 2024-04-02 19:14:34.401442 reflex-0.4.7a2/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
+-rw-r--r--   0        0        0      614 2024-04-04 21:37:03.945011 reflex-0.4.7a2/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
+-rw-r--r--   0        0        0     2403 2024-04-04 21:37:03.945109 reflex-0.4.7a2/reflex/.templates/jinja/custom_components/src.py.jinja2
+-rw-r--r--   0        0        0      548 2023-09-25 02:29:12.548714 reflex-0.4.7a2/reflex/.templates/jinja/web/package.json.jinja2
+-rw-r--r--   0        0        0      930 2024-04-02 19:14:34.402842 reflex-0.4.7a2/reflex/.templates/jinja/web/pages/_app.js.jinja2
+-rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.4.7a2/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      400 2024-02-13 04:39:14.427011 reflex-0.4.7a2/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0       86 2023-09-25 02:29:12.549046 reflex-0.4.7a2/reflex/.templates/jinja/web/pages/component.js.jinja2
+-rw-r--r--   0        0        0      882 2023-12-04 22:31:51.571558 reflex-0.4.7a2/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0      343 2024-04-04 21:37:03.945229 reflex-0.4.7a2/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0      388 2024-04-04 21:37:03.945317 reflex-0.4.7a2/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
+-rw-r--r--   0        0        0      101 2023-12-04 22:31:51.572637 reflex-0.4.7a2/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
+-rw-r--r--   0        0        0     3883 2024-02-10 02:26:35.013845 reflex-0.4.7a2/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      141 2023-09-18 23:00:36.695917 reflex-0.4.7a2/reflex/.templates/jinja/web/styles/styles.css.jinja2
+-rw-r--r--   0        0        0      436 2024-02-10 02:26:35.013954 reflex-0.4.7a2/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0     3790 2024-04-02 19:14:34.404054 reflex-0.4.7a2/reflex/.templates/jinja/web/utils/context.js.jinja2
+-rw-r--r--   0        0        0       37 2023-10-20 19:16:08.667797 reflex-0.4.7a2/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.4.7a2/reflex/.templates/web/.gitignore
+-rw-r--r--   0        0        0      595 2023-10-20 19:16:08.667942 reflex-0.4.7a2/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
+-rw-r--r--   0        0        0      645 2024-04-02 19:14:34.404228 reflex-0.4.7a2/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
+-rw-r--r--   0        0        0       97 2023-09-18 23:00:36.696123 reflex-0.4.7a2/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-11-14 20:34:38.772076 reflex-0.4.7a2/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.4.7a2/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.4.7a2/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     1254 2023-09-06 00:16:27.465104 reflex-0.4.7a2/reflex/.templates/web/utils/client_side_routing.js
+-rw-r--r--   0        0        0     1622 2024-02-10 02:26:35.014073 reflex-0.4.7a2/reflex/.templates/web/utils/helpers/dataeditor.js
+-rw-r--r--   0        0        0     1152 2023-11-14 20:34:38.772264 reflex-0.4.7a2/reflex/.templates/web/utils/helpers/range.js
+-rw-r--r--   0        0        0    21688 2024-04-04 22:32:02.761656 reflex-0.4.7a2/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     5723 2024-04-04 21:37:03.945600 reflex-0.4.7a2/reflex/__init__.py
+-rw-r--r--   0        0        0     7649 2024-04-04 22:00:30.126840 reflex-0.4.7a2/reflex/__init__.pyi
+-rw-r--r--   0        0        0      108 2023-08-10 23:30:03.955150 reflex-0.4.7a2/reflex/__main__.py
+-rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.4.7a2/reflex/admin.py
+-rw-r--r--   0        0        0    44562 2024-04-04 21:37:03.945930 reflex-0.4.7a2/reflex/app.py
+-rw-r--r--   0        0        0     5010 2024-04-04 21:37:03.946046 reflex-0.4.7a2/reflex/app.pyi
+-rw-r--r--   0        0        0     1152 2024-04-02 19:14:34.406758 reflex-0.4.7a2/reflex/app_module_for_backend.py
+-rw-r--r--   0        0        0     4250 2024-04-02 19:14:34.407224 reflex-0.4.7a2/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.4.7a2/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0    17037 2024-04-04 21:37:03.946194 reflex-0.4.7a2/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     4344 2024-04-02 19:14:34.407873 reflex-0.4.7a2/reflex/compiler/templates.py
+-rw-r--r--   0        0        0    14022 2024-04-06 01:57:36.880131 reflex-0.4.7a2/reflex/compiler/utils.py
+-rw-r--r--   0        0        0      530 2024-04-02 19:14:34.408438 reflex-0.4.7a2/reflex/components/__init__.py
+-rw-r--r--   0        0        0      325 2024-02-10 02:26:35.019008 reflex-0.4.7a2/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      573 2024-02-10 02:26:35.019123 reflex-0.4.7a2/reflex/components/base/app_wrap.py
+-rw-r--r--   0        0        0     2890 2024-04-02 19:14:34.408568 reflex-0.4.7a2/reflex/components/base/app_wrap.pyi
+-rw-r--r--   0        0        0     1234 2024-04-02 19:14:34.408691 reflex-0.4.7a2/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-12-21 01:07:08.388770 reflex-0.4.7a2/reflex/components/base/body.py
+-rw-r--r--   0        0        0     3277 2024-04-02 19:14:34.408849 reflex-0.4.7a2/reflex/components/base/body.pyi
+-rw-r--r--   0        0        0      583 2024-04-02 19:14:34.409155 reflex-0.4.7a2/reflex/components/base/document.py
+-rw-r--r--   0        0        0    14587 2024-04-02 19:14:34.409362 reflex-0.4.7a2/reflex/components/base/document.pyi
+-rw-r--r--   0        0        0      312 2024-02-10 02:26:35.020357 reflex-0.4.7a2/reflex/components/base/fragment.py
+-rw-r--r--   0        0        0     3289 2024-04-02 19:14:34.409517 reflex-0.4.7a2/reflex/components/base/fragment.pyi
+-rw-r--r--   0        0        0      297 2023-12-21 01:07:08.390493 reflex-0.4.7a2/reflex/components/base/head.py
+-rw-r--r--   0        0        0     6073 2024-04-02 19:14:34.409716 reflex-0.4.7a2/reflex/components/base/head.pyi
+-rw-r--r--   0        0        0      929 2023-12-21 01:07:08.390801 reflex-0.4.7a2/reflex/components/base/link.py
+-rw-r--r--   0        0        0     7132 2024-04-02 19:14:34.410033 reflex-0.4.7a2/reflex/components/base/link.pyi
+-rw-r--r--   0        0        0     1438 2023-12-21 01:07:08.390993 reflex-0.4.7a2/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    13088 2024-04-02 19:14:34.410197 reflex-0.4.7a2/reflex/components/base/meta.pyi
+-rw-r--r--   0        0        0     2298 2023-12-21 01:07:08.391208 reflex-0.4.7a2/reflex/components/base/script.py
+-rw-r--r--   0        0        0     4500 2024-04-02 19:14:34.410334 reflex-0.4.7a2/reflex/components/base/script.pyi
+-rw-r--r--   0        0        0     6378 2024-04-02 19:14:34.410492 reflex-0.4.7a2/reflex/components/chakra/__init__.py
+-rw-r--r--   0        0        0     5242 2024-02-16 18:55:54.269834 reflex-0.4.7a2/reflex/components/chakra/base.py
+-rw-r--r--   0        0        0    11059 2024-04-02 19:14:34.410632 reflex-0.4.7a2/reflex/components/chakra/base.pyi
+-rw-r--r--   0        0        0      459 2024-04-02 19:14:34.410790 reflex-0.4.7a2/reflex/components/chakra/datadisplay/__init__.py
+-rw-r--r--   0        0        0      352 2024-02-10 02:26:35.022081 reflex-0.4.7a2/reflex/components/chakra/datadisplay/badge.py
+-rw-r--r--   0        0        0     3725 2024-04-02 19:14:34.410909 reflex-0.4.7a2/reflex/components/chakra/datadisplay/badge.pyi
+-rw-r--r--   0        0        0      174 2024-04-02 19:14:34.411078 reflex-0.4.7a2/reflex/components/chakra/datadisplay/code.py
+-rw-r--r--   0        0        0     3300 2024-04-02 19:14:34.411266 reflex-0.4.7a2/reflex/components/chakra/datadisplay/code.pyi
+-rw-r--r--   0        0        0      657 2024-02-10 02:26:35.022721 reflex-0.4.7a2/reflex/components/chakra/datadisplay/divider.py
+-rw-r--r--   0        0        0     4005 2024-04-02 19:14:34.411393 reflex-0.4.7a2/reflex/components/chakra/datadisplay/divider.pyi
+-rw-r--r--   0        0        0      180 2024-02-10 02:26:35.022864 reflex-0.4.7a2/reflex/components/chakra/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     3322 2024-04-02 19:14:34.411517 reflex-0.4.7a2/reflex/components/chakra/datadisplay/keyboard_key.pyi
+-rw-r--r--   0        0        0     1505 2024-02-10 02:26:35.022985 reflex-0.4.7a2/reflex/components/chakra/datadisplay/list.py
+-rw-r--r--   0        0        0    13065 2024-04-02 19:14:34.411638 reflex-0.4.7a2/reflex/components/chakra/datadisplay/list.pyi
+-rw-r--r--   0        0        0     2149 2024-02-10 02:26:35.023113 reflex-0.4.7a2/reflex/components/chakra/datadisplay/stat.py
+-rw-r--r--   0        0        0    17816 2024-04-02 19:14:34.411771 reflex-0.4.7a2/reflex/components/chakra/datadisplay/stat.pyi
+-rw-r--r--   0        0        0     9122 2024-02-10 02:26:35.023268 reflex-0.4.7a2/reflex/components/chakra/datadisplay/table.py
+-rw-r--r--   0        0        0    27536 2024-04-02 19:14:34.411949 reflex-0.4.7a2/reflex/components/chakra/datadisplay/table.pyi
+-rw-r--r--   0        0        0     2294 2024-02-10 02:26:35.023510 reflex-0.4.7a2/reflex/components/chakra/datadisplay/tag.py
+-rw-r--r--   0        0        0    16018 2024-04-02 19:14:34.412089 reflex-0.4.7a2/reflex/components/chakra/datadisplay/tag.pyi
+-rw-r--r--   0        0        0      384 2024-02-10 02:26:35.023677 reflex-0.4.7a2/reflex/components/chakra/disclosure/__init__.py
+-rw-r--r--   0        0        0     3509 2024-02-10 02:26:35.023748 reflex-0.4.7a2/reflex/components/chakra/disclosure/accordion.py
+-rw-r--r--   0        0        0    16087 2024-04-02 19:14:34.412252 reflex-0.4.7a2/reflex/components/chakra/disclosure/accordion.pyi
+-rw-r--r--   0        0        0     3295 2024-02-10 02:26:35.024084 reflex-0.4.7a2/reflex/components/chakra/disclosure/tabs.py
+-rw-r--r--   0        0        0    18809 2024-04-02 19:14:34.412388 reflex-0.4.7a2/reflex/components/chakra/disclosure/tabs.pyi
+-rw-r--r--   0        0        0     1732 2024-02-10 02:26:35.024232 reflex-0.4.7a2/reflex/components/chakra/disclosure/transition.py
+-rw-r--r--   0        0        0    20429 2024-04-02 19:14:34.412530 reflex-0.4.7a2/reflex/components/chakra/disclosure/transition.pyi
+-rw-r--r--   0        0        0      278 2024-02-10 02:26:35.024533 reflex-0.4.7a2/reflex/components/chakra/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0     3329 2024-04-02 19:14:34.412660 reflex-0.4.7a2/reflex/components/chakra/disclosure/visuallyhidden.pyi
+-rw-r--r--   0        0        0      313 2024-02-10 02:26:35.024661 reflex-0.4.7a2/reflex/components/chakra/feedback/__init__.py
+-rw-r--r--   0        0        0     1623 2024-02-10 02:26:35.024723 reflex-0.4.7a2/reflex/components/chakra/feedback/alert.py
+-rw-r--r--   0        0        0    12594 2024-04-02 19:14:34.412793 reflex-0.4.7a2/reflex/components/chakra/feedback/alert.pyi
+-rw-r--r--   0        0        0     2006 2024-02-10 02:26:35.024858 reflex-0.4.7a2/reflex/components/chakra/feedback/circularprogress.py
+-rw-r--r--   0        0        0     7708 2024-04-02 19:14:34.412916 reflex-0.4.7a2/reflex/components/chakra/feedback/circularprogress.pyi
+-rw-r--r--   0        0        0      871 2024-02-10 02:26:35.024988 reflex-0.4.7a2/reflex/components/chakra/feedback/progress.py
+-rw-r--r--   0        0        0     4349 2024-04-02 19:14:34.413051 reflex-0.4.7a2/reflex/components/chakra/feedback/progress.pyi
+-rw-r--r--   0        0        0     1776 2024-02-10 02:26:35.025096 reflex-0.4.7a2/reflex/components/chakra/feedback/skeleton.py
+-rw-r--r--   0        0        0    10903 2024-04-02 19:14:34.413182 reflex-0.4.7a2/reflex/components/chakra/feedback/skeleton.pyi
+-rw-r--r--   0        0        0      704 2024-02-10 02:26:35.025211 reflex-0.4.7a2/reflex/components/chakra/feedback/spinner.py
+-rw-r--r--   0        0        0     4178 2024-04-02 19:14:34.413298 reflex-0.4.7a2/reflex/components/chakra/feedback/spinner.pyi
+-rw-r--r--   0        0        0     1453 2024-04-02 19:14:34.413424 reflex-0.4.7a2/reflex/components/chakra/forms/__init__.py
+-rw-r--r--   0        0        0     2395 2024-02-10 02:26:35.025415 reflex-0.4.7a2/reflex/components/chakra/forms/button.py
+-rw-r--r--   0        0        0    10687 2024-04-02 19:14:34.413528 reflex-0.4.7a2/reflex/components/chakra/forms/button.pyi
+-rw-r--r--   0        0        0     2764 2024-02-10 02:26:35.025535 reflex-0.4.7a2/reflex/components/chakra/forms/checkbox.py
+-rw-r--r--   0        0        0    10443 2024-04-02 19:14:34.413633 reflex-0.4.7a2/reflex/components/chakra/forms/checkbox.pyi
+-rw-r--r--   0        0        0     2860 2024-04-02 19:14:34.413744 reflex-0.4.7a2/reflex/components/chakra/forms/colormodeswitch.py
+-rw-r--r--   0        0        0    18530 2024-04-02 19:14:34.413852 reflex-0.4.7a2/reflex/components/chakra/forms/colormodeswitch.pyi
+-rw-r--r--   0        0        0      246 2024-02-10 02:26:35.025773 reflex-0.4.7a2/reflex/components/chakra/forms/date_picker.py
+-rw-r--r--   0        0        0     5841 2024-04-02 19:14:34.413954 reflex-0.4.7a2/reflex/components/chakra/forms/date_picker.pyi
+-rw-r--r--   0        0        0      280 2024-02-10 02:26:35.025877 reflex-0.4.7a2/reflex/components/chakra/forms/date_time_picker.py
+-rw-r--r--   0        0        0     5854 2024-04-02 19:14:34.414051 reflex-0.4.7a2/reflex/components/chakra/forms/date_time_picker.pyi
+-rw-r--r--   0        0        0     2110 2024-02-10 02:26:35.025987 reflex-0.4.7a2/reflex/components/chakra/forms/editable.py
+-rw-r--r--   0        0        0    13623 2024-04-02 19:14:34.414156 reflex-0.4.7a2/reflex/components/chakra/forms/editable.pyi
+-rw-r--r--   0        0        0      246 2024-02-10 02:26:35.026103 reflex-0.4.7a2/reflex/components/chakra/forms/email.py
+-rw-r--r--   0        0        0     5825 2024-04-02 19:14:34.414250 reflex-0.4.7a2/reflex/components/chakra/forms/email.pyi
+-rw-r--r--   0        0        0     2579 2024-04-02 19:14:34.414562 reflex-0.4.7a2/reflex/components/chakra/forms/form.py
+-rw-r--r--   0        0        0    20832 2024-04-02 19:14:34.414743 reflex-0.4.7a2/reflex/components/chakra/forms/form.pyi
+-rw-r--r--   0        0        0      935 2024-02-10 02:26:35.026649 reflex-0.4.7a2/reflex/components/chakra/forms/iconbutton.py
+-rw-r--r--   0        0        0     4739 2024-04-02 19:14:34.414896 reflex-0.4.7a2/reflex/components/chakra/forms/iconbutton.pyi
+-rw-r--r--   0        0        0     4312 2024-04-02 19:14:34.415230 reflex-0.4.7a2/reflex/components/chakra/forms/input.py
+-rw-r--r--   0        0        0    21869 2024-04-02 19:14:34.415375 reflex-0.4.7a2/reflex/components/chakra/forms/input.pyi
+-rw-r--r--   0        0        0    12940 2024-02-10 02:26:35.027180 reflex-0.4.7a2/reflex/components/chakra/forms/multiselect.py
+-rw-r--r--   0        0        0     4334 2024-02-10 02:26:35.027253 reflex-0.4.7a2/reflex/components/chakra/forms/numberinput.py
+-rw-r--r--   0        0        0    18377 2024-04-02 19:14:34.415512 reflex-0.4.7a2/reflex/components/chakra/forms/numberinput.pyi
+-rw-r--r--   0        0        0      256 2024-02-10 02:26:35.027395 reflex-0.4.7a2/reflex/components/chakra/forms/password.py
+-rw-r--r--   0        0        0     5834 2024-04-02 19:14:34.415639 reflex-0.4.7a2/reflex/components/chakra/forms/password.pyi
+-rw-r--r--   0        0        0     6507 2024-04-04 21:37:03.946495 reflex-0.4.7a2/reflex/components/chakra/forms/pininput.py
+-rw-r--r--   0        0        0     9432 2024-04-02 19:14:34.415764 reflex-0.4.7a2/reflex/components/chakra/forms/pininput.pyi
+-rw-r--r--   0        0        0     3176 2024-02-10 02:26:35.027681 reflex-0.4.7a2/reflex/components/chakra/forms/radio.py
+-rw-r--r--   0        0        0     8414 2024-04-02 19:14:34.415876 reflex-0.4.7a2/reflex/components/chakra/forms/radio.pyi
+-rw-r--r--   0        0        0     4547 2024-02-10 02:26:35.027836 reflex-0.4.7a2/reflex/components/chakra/forms/rangeslider.py
+-rw-r--r--   0        0        0    14156 2024-04-02 19:14:34.415997 reflex-0.4.7a2/reflex/components/chakra/forms/rangeslider.pyi
+-rw-r--r--   0        0        0     3624 2024-02-10 02:26:35.027969 reflex-0.4.7a2/reflex/components/chakra/forms/select.py
+-rw-r--r--   0        0        0     8868 2024-04-02 19:14:34.416109 reflex-0.4.7a2/reflex/components/chakra/forms/select.pyi
+-rw-r--r--   0        0        0     3532 2024-02-10 02:26:35.028089 reflex-0.4.7a2/reflex/components/chakra/forms/slider.py
+-rw-r--r--   0        0        0    17745 2024-04-02 19:14:34.416245 reflex-0.4.7a2/reflex/components/chakra/forms/slider.pyi
+-rw-r--r--   0        0        0     1838 2024-02-10 02:26:35.028236 reflex-0.4.7a2/reflex/components/chakra/forms/switch.py
+-rw-r--r--   0        0        0     6602 2024-04-02 19:14:34.416373 reflex-0.4.7a2/reflex/components/chakra/forms/switch.pyi
+-rw-r--r--   0        0        0     2474 2024-02-16 18:55:54.270329 reflex-0.4.7a2/reflex/components/chakra/forms/textarea.py
+-rw-r--r--   0        0        0     5419 2024-04-02 19:14:34.416480 reflex-0.4.7a2/reflex/components/chakra/forms/textarea.pyi
+-rw-r--r--   0        0        0      246 2024-02-10 02:26:35.028621 reflex-0.4.7a2/reflex/components/chakra/forms/time_picker.py
+-rw-r--r--   0        0        0     5841 2024-04-02 19:14:34.416578 reflex-0.4.7a2/reflex/components/chakra/forms/time_picker.pyi
+-rw-r--r--   0        0        0      487 2024-04-02 19:14:34.416715 reflex-0.4.7a2/reflex/components/chakra/layout/__init__.py
+-rw-r--r--   0        0        0      315 2024-02-10 02:26:35.028815 reflex-0.4.7a2/reflex/components/chakra/layout/aspect_ratio.py
+-rw-r--r--   0        0        0     3450 2024-04-02 19:14:34.416820 reflex-0.4.7a2/reflex/components/chakra/layout/aspect_ratio.pyi
+-rw-r--r--   0        0        0      755 2024-02-10 02:26:35.028940 reflex-0.4.7a2/reflex/components/chakra/layout/box.py
+-rw-r--r--   0        0        0     3733 2024-04-02 19:14:34.416924 reflex-0.4.7a2/reflex/components/chakra/layout/box.pyi
+-rw-r--r--   0        0        0     2967 2024-02-10 02:26:35.029073 reflex-0.4.7a2/reflex/components/chakra/layout/card.py
+-rw-r--r--   0        0        0    14063 2024-04-02 19:14:34.417040 reflex-0.4.7a2/reflex/components/chakra/layout/card.pyi
+-rw-r--r--   0        0        0      389 2024-02-10 02:26:35.029302 reflex-0.4.7a2/reflex/components/chakra/layout/center.py
+-rw-r--r--   0        0        0     8905 2024-04-02 19:14:34.417147 reflex-0.4.7a2/reflex/components/chakra/layout/center.pyi
+-rw-r--r--   0        0        0      354 2024-02-10 02:26:35.029446 reflex-0.4.7a2/reflex/components/chakra/layout/container.py
+-rw-r--r--   0        0        0     3502 2024-04-02 19:14:34.417255 reflex-0.4.7a2/reflex/components/chakra/layout/container.pyi
+-rw-r--r--   0        0        0      715 2024-02-10 02:26:35.029582 reflex-0.4.7a2/reflex/components/chakra/layout/flex.py
+-rw-r--r--   0        0        0     4209 2024-04-02 19:14:34.417357 reflex-0.4.7a2/reflex/components/chakra/layout/flex.pyi
+-rw-r--r--   0        0        0     4318 2024-02-10 02:26:35.029717 reflex-0.4.7a2/reflex/components/chakra/layout/grid.py
+-rw-r--r--   0        0        0    14066 2024-04-02 19:14:34.417480 reflex-0.4.7a2/reflex/components/chakra/layout/grid.pyi
+-rw-r--r--   0        0        0      179 2024-02-10 02:26:35.029946 reflex-0.4.7a2/reflex/components/chakra/layout/spacer.py
+-rw-r--r--   0        0        0     3301 2024-04-02 19:14:34.417588 reflex-0.4.7a2/reflex/components/chakra/layout/spacer.pyi
+-rw-r--r--   0        0        0     1077 2024-02-10 02:26:35.030045 reflex-0.4.7a2/reflex/components/chakra/layout/stack.py
+-rw-r--r--   0        0        0    12432 2024-04-02 19:14:34.417697 reflex-0.4.7a2/reflex/components/chakra/layout/stack.pyi
+-rw-r--r--   0        0        0     1463 2024-02-10 02:26:35.030152 reflex-0.4.7a2/reflex/components/chakra/layout/wrap.py
+-rw-r--r--   0        0        0     7014 2024-04-02 19:14:34.417807 reflex-0.4.7a2/reflex/components/chakra/layout/wrap.pyi
+-rw-r--r--   0        0        0      190 2024-02-10 02:26:35.030265 reflex-0.4.7a2/reflex/components/chakra/media/__init__.py
+-rw-r--r--   0        0        0     1668 2024-02-10 02:26:35.030317 reflex-0.4.7a2/reflex/components/chakra/media/avatar.py
+-rw-r--r--   0        0        0    10658 2024-04-02 19:14:34.417938 reflex-0.4.7a2/reflex/components/chakra/media/avatar.pyi
+-rw-r--r--   0        0        0     2461 2024-02-10 02:26:35.030430 reflex-0.4.7a2/reflex/components/chakra/media/icon.py
+-rw-r--r--   0        0        0     6342 2024-04-02 19:14:34.418161 reflex-0.4.7a2/reflex/components/chakra/media/icon.pyi
+-rw-r--r--   0        0        0     2400 2024-02-10 02:26:35.030535 reflex-0.4.7a2/reflex/components/chakra/media/image.py
+-rw-r--r--   0        0        0     5423 2024-04-02 19:14:34.418332 reflex-0.4.7a2/reflex/components/chakra/media/image.pyi
+-rw-r--r--   0        0        0      419 2024-02-10 02:26:35.030653 reflex-0.4.7a2/reflex/components/chakra/navigation/__init__.py
+-rw-r--r--   0        0        0     2925 2024-02-10 02:26:35.030704 reflex-0.4.7a2/reflex/components/chakra/navigation/breadcrumb.py
+-rw-r--r--   0        0        0    13646 2024-04-02 19:14:34.418567 reflex-0.4.7a2/reflex/components/chakra/navigation/breadcrumb.pyi
+-rw-r--r--   0        0        0     1475 2024-02-10 02:26:35.030830 reflex-0.4.7a2/reflex/components/chakra/navigation/link.py
+-rw-r--r--   0        0        0     3999 2024-04-02 19:14:34.418745 reflex-0.4.7a2/reflex/components/chakra/navigation/link.pyi
+-rw-r--r--   0        0        0      521 2024-02-10 02:26:35.031182 reflex-0.4.7a2/reflex/components/chakra/navigation/linkoverlay.py
+-rw-r--r--   0        0        0     6375 2024-04-02 19:14:34.418852 reflex-0.4.7a2/reflex/components/chakra/navigation/linkoverlay.pyi
+-rw-r--r--   0        0        0     2935 2024-02-10 02:26:35.031313 reflex-0.4.7a2/reflex/components/chakra/navigation/stepper.py
+-rw-r--r--   0        0        0    28490 2024-04-02 19:14:34.418987 reflex-0.4.7a2/reflex/components/chakra/navigation/stepper.pyi
+-rw-r--r--   0        0        0      850 2024-02-10 02:26:35.031514 reflex-0.4.7a2/reflex/components/chakra/overlay/__init__.py
+-rw-r--r--   0        0        0     5200 2024-02-10 02:26:35.031625 reflex-0.4.7a2/reflex/components/chakra/overlay/alertdialog.py
+-rw-r--r--   0        0        0    24411 2024-04-02 19:14:34.419146 reflex-0.4.7a2/reflex/components/chakra/overlay/alertdialog.pyi
+-rw-r--r--   0        0        0     5186 2024-02-10 02:26:35.031772 reflex-0.4.7a2/reflex/components/chakra/overlay/drawer.py
+-rw-r--r--   0        0        0    25832 2024-04-02 19:14:34.419276 reflex-0.4.7a2/reflex/components/chakra/overlay/drawer.pyi
+-rw-r--r--   0        0        0     6974 2024-02-10 02:26:35.031928 reflex-0.4.7a2/reflex/components/chakra/overlay/menu.py
+-rw-r--r--   0        0        0    29108 2024-04-02 19:14:34.419396 reflex-0.4.7a2/reflex/components/chakra/overlay/menu.pyi
+-rw-r--r--   0        0        0     5270 2024-02-10 02:26:35.032050 reflex-0.4.7a2/reflex/components/chakra/overlay/modal.py
+-rw-r--r--   0        0        0    23975 2024-04-02 19:14:34.419505 reflex-0.4.7a2/reflex/components/chakra/overlay/modal.pyi
+-rw-r--r--   0        0        0     5967 2024-02-10 02:26:35.032202 reflex-0.4.7a2/reflex/components/chakra/overlay/popover.py
+-rw-r--r--   0        0        0    30461 2024-04-02 19:14:34.419633 reflex-0.4.7a2/reflex/components/chakra/overlay/popover.pyi
+-rw-r--r--   0        0        0     2127 2024-02-10 02:26:35.032416 reflex-0.4.7a2/reflex/components/chakra/overlay/tooltip.py
+-rw-r--r--   0        0        0     6131 2024-04-02 19:14:34.419766 reflex-0.4.7a2/reflex/components/chakra/overlay/tooltip.pyi
+-rw-r--r--   0        0        0      271 2024-02-10 02:26:35.032550 reflex-0.4.7a2/reflex/components/chakra/typography/__init__.py
+-rw-r--r--   0        0        0      379 2024-02-10 02:26:35.032612 reflex-0.4.7a2/reflex/components/chakra/typography/heading.py
+-rw-r--r--   0        0        0     3777 2024-04-02 19:14:34.419870 reflex-0.4.7a2/reflex/components/chakra/typography/heading.pyi
+-rw-r--r--   0        0        0      671 2024-02-10 02:26:35.032741 reflex-0.4.7a2/reflex/components/chakra/typography/highlight.py
+-rw-r--r--   0        0        0     3716 2024-04-02 19:14:34.419964 reflex-0.4.7a2/reflex/components/chakra/typography/highlight.pyi
+-rw-r--r--   0        0        0      328 2024-02-10 02:26:35.032862 reflex-0.4.7a2/reflex/components/chakra/typography/span.py
+-rw-r--r--   0        0        0     3443 2024-04-02 19:14:34.420093 reflex-0.4.7a2/reflex/components/chakra/typography/span.pyi
+-rw-r--r--   0        0        0      472 2024-02-10 02:26:35.033013 reflex-0.4.7a2/reflex/components/chakra/typography/text.py
+-rw-r--r--   0        0        0     3667 2024-04-02 19:14:34.420216 reflex-0.4.7a2/reflex/components/chakra/typography/text.pyi
+-rw-r--r--   0        0        0    64790 2024-04-04 21:37:03.946766 reflex-0.4.7a2/reflex/components/component.py
+-rw-r--r--   0        0        0      844 2024-04-02 19:14:34.421147 reflex-0.4.7a2/reflex/components/core/__init__.py
+-rw-r--r--   0        0        0     5943 2024-04-04 21:37:03.946911 reflex-0.4.7a2/reflex/components/core/banner.py
+-rw-r--r--   0        0        0    17164 2024-04-02 19:14:34.421397 reflex-0.4.7a2/reflex/components/core/banner.pyi
+-rw-r--r--   0        0        0     1873 2024-02-10 02:26:35.034230 reflex-0.4.7a2/reflex/components/core/client_side_routing.py
+-rw-r--r--   0        0        0     6406 2024-04-02 19:14:34.421550 reflex-0.4.7a2/reflex/components/core/client_side_routing.pyi
+-rw-r--r--   0        0        0      590 2024-04-02 19:14:34.421679 reflex-0.4.7a2/reflex/components/core/colors.py
+-rw-r--r--   0        0        0     6291 2024-04-08 21:11:25.547238 reflex-0.4.7a2/reflex/components/core/cond.py
+-rw-r--r--   0        0        0     4642 2024-04-02 19:14:34.422253 reflex-0.4.7a2/reflex/components/core/debounce.py
+-rw-r--r--   0        0        0     4149 2024-04-02 19:14:34.422370 reflex-0.4.7a2/reflex/components/core/debounce.pyi
+-rw-r--r--   0        0        0     4031 2024-04-02 18:24:25.099624 reflex-0.4.7a2/reflex/components/core/foreach.py
+-rw-r--r--   0        0        0     1033 2024-04-02 19:14:34.422562 reflex-0.4.7a2/reflex/components/core/html.py
+-rw-r--r--   0        0        0     6616 2024-04-02 19:14:34.422669 reflex-0.4.7a2/reflex/components/core/html.pyi
+-rw-r--r--   0        0        0       30 2024-02-10 02:26:35.035636 reflex-0.4.7a2/reflex/components/core/layout/__init__.py
+-rw-r--r--   0        0        0     9989 2024-04-02 19:14:34.422836 reflex-0.4.7a2/reflex/components/core/match.py
+-rw-r--r--   0        0        0     1907 2024-04-02 19:14:34.427781 reflex-0.4.7a2/reflex/components/core/responsive.py
+-rw-r--r--   0        0        0     9000 2024-04-04 21:37:03.947039 reflex-0.4.7a2/reflex/components/core/upload.py
+-rw-r--r--   0        0        0     8667 2024-04-02 19:14:34.429377 reflex-0.4.7a2/reflex/components/core/upload.pyi
+-rw-r--r--   0        0        0      357 2024-04-04 21:37:03.947140 reflex-0.4.7a2/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0    11227 2024-04-02 19:14:34.430271 reflex-0.4.7a2/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0    31107 2024-04-02 19:14:34.430442 reflex-0.4.7a2/reflex/components/datadisplay/code.pyi
+-rw-r--r--   0        0        0    12632 2024-02-10 02:26:35.036910 reflex-0.4.7a2/reflex/components/datadisplay/dataeditor.py
+-rw-r--r--   0        0        0    10485 2024-04-02 19:14:34.430603 reflex-0.4.7a2/reflex/components/datadisplay/dataeditor.pyi
+-rw-r--r--   0        0        0     2562 2024-04-04 21:37:03.947200 reflex-0.4.7a2/reflex/components/datadisplay/logo.py
+-rw-r--r--   0        0        0       73 2024-02-07 01:47:48.949909 reflex-0.4.7a2/reflex/components/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-12-21 01:07:08.429460 reflex-0.4.7a2/reflex/components/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-12-21 01:07:08.429529 reflex-0.4.7a2/reflex/components/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-12-21 01:07:08.429622 reflex-0.4.7a2/reflex/components/el/constants/react.py
+-rw-r--r--   0        0        0     1713 2023-12-21 01:07:08.429682 reflex-0.4.7a2/reflex/components/el/constants/reflex.py
+-rw-r--r--   0        0        0      494 2023-12-21 01:07:08.429898 reflex-0.4.7a2/reflex/components/el/element.py
+-rw-r--r--   0        0        0     3284 2024-04-02 19:14:34.430869 reflex-0.4.7a2/reflex/components/el/element.pyi
+-rw-r--r--   0        0        0     3529 2024-04-02 19:14:34.432601 reflex-0.4.7a2/reflex/components/el/elements/__init__.py
+-rw-r--r--   0        0        0     1982 2024-04-02 19:14:34.432772 reflex-0.4.7a2/reflex/components/el/elements/base.py
+-rw-r--r--   0        0        0     6411 2024-04-02 19:14:34.432874 reflex-0.4.7a2/reflex/components/el/elements/base.pyi
+-rw-r--r--   0        0        0    20102 2024-04-04 21:37:03.947356 reflex-0.4.7a2/reflex/components/el/elements/forms.py
+-rw-r--r--   0        0        0   100476 2024-04-04 21:37:03.947614 reflex-0.4.7a2/reflex/components/el/elements/forms.pyi
+-rw-r--r--   0        0        0     3610 2024-02-10 02:26:35.038470 reflex-0.4.7a2/reflex/components/el/elements/inline.py
+-rw-r--r--   0        0        0   166595 2024-04-02 19:14:34.433892 reflex-0.4.7a2/reflex/components/el/elements/inline.pyi
+-rw-r--r--   0        0        0     7929 2024-04-02 19:14:34.434037 reflex-0.4.7a2/reflex/components/el/elements/media.py
+-rw-r--r--   0        0        0    94561 2024-04-02 19:14:34.434188 reflex-0.4.7a2/reflex/components/el/elements/media.pyi
+-rw-r--r--   0        0        0     1337 2023-12-21 01:07:08.433098 reflex-0.4.7a2/reflex/components/el/elements/metadata.py
+-rw-r--r--   0        0        0    28386 2024-04-02 19:14:34.434330 reflex-0.4.7a2/reflex/components/el/elements/metadata.pyi
+-rw-r--r--   0        0        0     1569 2023-12-21 01:07:08.433349 reflex-0.4.7a2/reflex/components/el/elements/other.py
+-rw-r--r--   0        0        0    42530 2024-04-02 19:14:34.434559 reflex-0.4.7a2/reflex/components/el/elements/other.pyi
+-rw-r--r--   0        0        0     1406 2024-04-02 19:14:34.434672 reflex-0.4.7a2/reflex/components/el/elements/scripts.py
+-rw-r--r--   0        0        0    19828 2024-04-02 19:14:34.434788 reflex-0.4.7a2/reflex/components/el/elements/scripts.pyi
+-rw-r--r--   0        0        0     1535 2024-04-02 19:14:34.434940 reflex-0.4.7a2/reflex/components/el/elements/sectioning.py
+-rw-r--r--   0        0        0    88307 2024-04-02 19:14:34.435104 reflex-0.4.7a2/reflex/components/el/elements/sectioning.pyi
+-rw-r--r--   0        0        0     2767 2024-04-02 19:14:34.435250 reflex-0.4.7a2/reflex/components/el/elements/tables.py
+-rw-r--r--   0        0        0    62559 2024-04-02 19:14:34.435538 reflex-0.4.7a2/reflex/components/el/elements/tables.pyi
+-rw-r--r--   0        0        0     2432 2024-04-02 19:14:34.436021 reflex-0.4.7a2/reflex/components/el/elements/typography.py
+-rw-r--r--   0        0        0    90180 2024-04-02 19:14:34.436215 reflex-0.4.7a2/reflex/components/el/elements/typography.pyi
+-rw-r--r--   0        0        0       88 2024-02-10 02:26:35.040149 reflex-0.4.7a2/reflex/components/gridjs/__init__.py
+-rw-r--r--   0        0        0     4300 2024-02-10 02:26:35.040226 reflex-0.4.7a2/reflex/components/gridjs/datatable.py
+-rw-r--r--   0        0        0     7124 2024-04-02 19:14:34.436409 reflex-0.4.7a2/reflex/components/gridjs/datatable.pyi
+-rw-r--r--   0        0        0      501 2024-02-10 02:26:35.040431 reflex-0.4.7a2/reflex/components/literals.py
+-rw-r--r--   0        0        0       73 2024-02-10 02:26:35.040887 reflex-0.4.7a2/reflex/components/lucide/__init__.py
+-rw-r--r--   0        0        0    34237 2024-04-04 21:37:03.947839 reflex-0.4.7a2/reflex/components/lucide/icon.py
+-rw-r--r--   0        0        0    38020 2024-04-04 21:37:03.948033 reflex-0.4.7a2/reflex/components/lucide/icon.pyi
+-rw-r--r--   0        0        0       87 2024-02-10 02:26:35.041813 reflex-0.4.7a2/reflex/components/markdown/__init__.py
+-rw-r--r--   0        0        0    11448 2024-04-04 21:37:03.948197 reflex-0.4.7a2/reflex/components/markdown/markdown.py
+-rw-r--r--   0        0        0     5278 2024-04-04 21:37:03.948324 reflex-0.4.7a2/reflex/components/markdown/markdown.pyi
+-rw-r--r--   0        0        0       44 2024-02-10 02:26:35.042167 reflex-0.4.7a2/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      102 2024-02-10 02:26:35.042266 reflex-0.4.7a2/reflex/components/media/icon.py
+-rw-r--r--   0        0        0       79 2024-02-10 02:26:35.042315 reflex-0.4.7a2/reflex/components/moment/__init__.py
+-rw-r--r--   0        0        0     3925 2024-02-10 02:26:35.042375 reflex-0.4.7a2/reflex/components/moment/moment.py
+-rw-r--r--   0        0        0     6870 2024-04-02 19:14:34.438557 reflex-0.4.7a2/reflex/components/moment/moment.pyi
+-rw-r--r--   0        0        0      239 2024-02-10 02:26:35.042504 reflex-0.4.7a2/reflex/components/next/__init__.py
+-rw-r--r--   0        0        0      189 2024-02-10 02:26:35.042549 reflex-0.4.7a2/reflex/components/next/base.py
+-rw-r--r--   0        0        0     3304 2024-04-02 19:14:34.438775 reflex-0.4.7a2/reflex/components/next/base.pyi
+-rw-r--r--   0        0        0     3831 2024-02-10 02:26:35.042660 reflex-0.4.7a2/reflex/components/next/image.py
+-rw-r--r--   0        0        0     5795 2024-04-02 19:14:34.438919 reflex-0.4.7a2/reflex/components/next/image.pyi
+-rw-r--r--   0        0        0      503 2024-02-10 02:26:35.042780 reflex-0.4.7a2/reflex/components/next/link.py
+-rw-r--r--   0        0        0     3532 2024-04-02 19:14:34.439026 reflex-0.4.7a2/reflex/components/next/link.pyi
+-rw-r--r--   0        0        0      730 2024-02-10 02:26:35.042905 reflex-0.4.7a2/reflex/components/next/video.py
+-rw-r--r--   0        0        0     3429 2024-04-02 19:14:34.439128 reflex-0.4.7a2/reflex/components/next/video.pyi
+-rw-r--r--   0        0        0       77 2024-02-10 02:26:35.043030 reflex-0.4.7a2/reflex/components/plotly/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-02 19:14:34.439545 reflex-0.4.7a2/reflex/components/plotly/plotly.py
+-rw-r--r--   0        0        0     7007 2024-04-02 19:14:34.439682 reflex-0.4.7a2/reflex/components/plotly/plotly.pyi
+-rw-r--r--   0        0        0      112 2024-04-02 19:14:34.440146 reflex-0.4.7a2/reflex/components/radix/__init__.py
+-rw-r--r--   0        0        0      214 2024-04-02 19:14:34.440350 reflex-0.4.7a2/reflex/components/radix/primitives/__init__.py
+-rw-r--r--   0        0        0    21406 2024-04-02 19:14:34.440707 reflex-0.4.7a2/reflex/components/radix/primitives/accordion.py
+-rw-r--r--   0        0        0    26956 2024-04-02 19:14:34.440903 reflex-0.4.7a2/reflex/components/radix/primitives/accordion.pyi
+-rw-r--r--   0        0        0      869 2024-02-10 02:26:35.044768 reflex-0.4.7a2/reflex/components/radix/primitives/base.py
+-rw-r--r--   0        0        0     6620 2024-04-02 19:14:34.441366 reflex-0.4.7a2/reflex/components/radix/primitives/base.pyi
+-rw-r--r--   0        0        0     8660 2024-04-02 19:14:34.442162 reflex-0.4.7a2/reflex/components/radix/primitives/drawer.py
+-rw-r--r--   0        0        0    34981 2024-04-02 19:14:34.442473 reflex-0.4.7a2/reflex/components/radix/primitives/drawer.pyi
+-rw-r--r--   0        0        0     4760 2024-04-02 19:14:34.442846 reflex-0.4.7a2/reflex/components/radix/primitives/form.py
+-rw-r--r--   0        0        0    48365 2024-04-02 19:14:34.443076 reflex-0.4.7a2/reflex/components/radix/primitives/form.pyi
+-rw-r--r--   0        0        0     3996 2024-04-02 19:14:34.443510 reflex-0.4.7a2/reflex/components/radix/primitives/progress.py
+-rw-r--r--   0        0        0    22997 2024-04-02 19:14:34.444066 reflex-0.4.7a2/reflex/components/radix/primitives/progress.pyi
+-rw-r--r--   0        0        0     5004 2024-04-02 19:14:34.444533 reflex-0.4.7a2/reflex/components/radix/primitives/slider.py
+-rw-r--r--   0        0        0    17052 2024-04-02 19:14:34.444665 reflex-0.4.7a2/reflex/components/radix/primitives/slider.pyi
+-rw-r--r--   0        0        0      292 2024-04-02 19:14:34.444811 reflex-0.4.7a2/reflex/components/radix/themes/__init__.py
+-rw-r--r--   0        0        0     8097 2024-04-02 19:14:34.445088 reflex-0.4.7a2/reflex/components/radix/themes/base.py
+-rw-r--r--   0        0        0    24216 2024-04-02 19:14:34.445340 reflex-0.4.7a2/reflex/components/radix/themes/base.pyi
+-rw-r--r--   0        0        0     3007 2024-04-02 19:14:34.445446 reflex-0.4.7a2/reflex/components/radix/themes/color_mode.py
+-rw-r--r--   0        0        0    21283 2024-04-02 19:14:34.445570 reflex-0.4.7a2/reflex/components/radix/themes/color_mode.pyi
+-rw-r--r--   0        0        0     1776 2024-04-02 19:14:34.445724 reflex-0.4.7a2/reflex/components/radix/themes/components/__init__.py
+-rw-r--r--   0        0        0     3267 2024-04-02 19:14:34.446644 reflex-0.4.7a2/reflex/components/radix/themes/components/alert_dialog.py
+-rw-r--r--   0        0        0    24434 2024-04-02 19:14:34.446757 reflex-0.4.7a2/reflex/components/radix/themes/components/alert_dialog.pyi
+-rw-r--r--   0        0        0    40237 2024-04-02 19:14:34.447529 reflex-0.4.7a2/reflex/components/radix/themes/components/alertdialog.pyi
+-rw-r--r--   0        0        0      400 2024-04-02 19:14:34.447703 reflex-0.4.7a2/reflex/components/radix/themes/components/aspect_ratio.py
+-rw-r--r--   0        0        0     3640 2024-04-02 19:14:34.447802 reflex-0.4.7a2/reflex/components/radix/themes/components/aspect_ratio.pyi
+-rw-r--r--   0        0        0     5724 2024-04-02 19:14:34.448082 reflex-0.4.7a2/reflex/components/radix/themes/components/aspectratio.pyi
+-rw-r--r--   0        0        0      989 2024-04-02 19:14:34.448493 reflex-0.4.7a2/reflex/components/radix/themes/components/avatar.py
+-rw-r--r--   0        0        0     6562 2024-04-02 19:14:34.448953 reflex-0.4.7a2/reflex/components/radix/themes/components/avatar.pyi
+-rw-r--r--   0        0        0      815 2024-04-02 19:14:34.449058 reflex-0.4.7a2/reflex/components/radix/themes/components/badge.py
+-rw-r--r--   0        0        0     9315 2024-04-02 19:14:34.449155 reflex-0.4.7a2/reflex/components/radix/themes/components/badge.pyi
+-rw-r--r--   0        0        0     1084 2024-04-02 19:14:34.449285 reflex-0.4.7a2/reflex/components/radix/themes/components/button.py
+-rw-r--r--   0        0        0    11758 2024-04-02 19:14:34.449372 reflex-0.4.7a2/reflex/components/radix/themes/components/button.pyi
+-rw-r--r--   0        0        0     2378 2024-04-02 19:14:34.449904 reflex-0.4.7a2/reflex/components/radix/themes/components/callout.py
+-rw-r--r--   0        0        0    38710 2024-04-02 19:14:34.450185 reflex-0.4.7a2/reflex/components/radix/themes/components/callout.pyi
+-rw-r--r--   0        0        0      659 2024-04-02 19:14:34.450330 reflex-0.4.7a2/reflex/components/radix/themes/components/card.py
+-rw-r--r--   0        0        0     7200 2024-04-02 19:14:34.450427 reflex-0.4.7a2/reflex/components/radix/themes/components/card.pyi
+-rw-r--r--   0        0        0     4679 2024-04-02 19:14:34.451369 reflex-0.4.7a2/reflex/components/radix/themes/components/checkbox.py
+-rw-r--r--   0        0        0    20877 2024-04-02 19:14:34.451567 reflex-0.4.7a2/reflex/components/radix/themes/components/checkbox.pyi
+-rw-r--r--   0        0        0     5049 2024-04-02 19:14:34.451786 reflex-0.4.7a2/reflex/components/radix/themes/components/context_menu.py
+-rw-r--r--   0        0        0    31192 2024-04-02 19:14:34.451890 reflex-0.4.7a2/reflex/components/radix/themes/components/context_menu.pyi
+-rw-r--r--   0        0        0    44130 2024-04-02 19:14:34.452056 reflex-0.4.7a2/reflex/components/radix/themes/components/contextmenu.pyi
+-rw-r--r--   0        0        0     2600 2024-04-02 19:14:34.452261 reflex-0.4.7a2/reflex/components/radix/themes/components/dialog.py
+-rw-r--r--   0        0        0    24895 2024-04-02 19:14:34.452419 reflex-0.4.7a2/reflex/components/radix/themes/components/dialog.pyi
+-rw-r--r--   0        0        0    11256 2024-04-02 19:14:34.452696 reflex-0.4.7a2/reflex/components/radix/themes/components/dropdown_menu.py
+-rw-r--r--   0        0        0    37901 2024-04-02 19:14:34.452840 reflex-0.4.7a2/reflex/components/radix/themes/components/dropdown_menu.pyi
+-rw-r--r--   0        0        0    52185 2024-04-02 19:14:34.453086 reflex-0.4.7a2/reflex/components/radix/themes/components/dropdownmenu.pyi
+-rw-r--r--   0        0        0     2405 2024-04-02 19:14:34.453445 reflex-0.4.7a2/reflex/components/radix/themes/components/hover_card.py
+-rw-r--r--   0        0        0    17744 2024-04-02 19:14:34.453581 reflex-0.4.7a2/reflex/components/radix/themes/components/hover_card.pyi
+-rw-r--r--   0        0        0    26453 2024-04-02 19:14:34.453788 reflex-0.4.7a2/reflex/components/radix/themes/components/hovercard.pyi
+-rw-r--r--   0        0        0     2789 2024-04-02 19:14:34.454202 reflex-0.4.7a2/reflex/components/radix/themes/components/icon_button.py
+-rw-r--r--   0        0        0    11916 2024-04-02 19:14:34.454271 reflex-0.4.7a2/reflex/components/radix/themes/components/icon_button.pyi
+-rw-r--r--   0        0        0    12021 2024-04-02 19:14:34.454397 reflex-0.4.7a2/reflex/components/radix/themes/components/iconbutton.pyi
+-rw-r--r--   0        0        0     1015 2024-04-02 19:14:34.454891 reflex-0.4.7a2/reflex/components/radix/themes/components/inset.py
+-rw-r--r--   0        0        0     7889 2024-04-02 19:14:34.455045 reflex-0.4.7a2/reflex/components/radix/themes/components/inset.pyi
+-rw-r--r--   0        0        0     3177 2024-04-02 19:14:34.455306 reflex-0.4.7a2/reflex/components/radix/themes/components/popover.py
+-rw-r--r--   0        0        0    17404 2024-04-02 19:14:34.455466 reflex-0.4.7a2/reflex/components/radix/themes/components/popover.pyi
+-rw-r--r--   0        0        0     6253 2024-04-02 19:14:34.455911 reflex-0.4.7a2/reflex/components/radix/themes/components/radio_group.py
+-rw-r--r--   0        0        0    24106 2024-04-02 19:14:34.456002 reflex-0.4.7a2/reflex/components/radix/themes/components/radio_group.pyi
+-rw-r--r--   0        0        0    26222 2024-04-02 19:14:34.457988 reflex-0.4.7a2/reflex/components/radix/themes/components/radiogroup.pyi
+-rw-r--r--   0        0        0      920 2024-04-02 19:14:34.458077 reflex-0.4.7a2/reflex/components/radix/themes/components/scroll_area.py
+-rw-r--r--   0        0        0     4427 2024-04-02 19:14:34.458156 reflex-0.4.7a2/reflex/components/radix/themes/components/scroll_area.pyi
+-rw-r--r--   0        0        0     6513 2024-04-02 19:14:34.458390 reflex-0.4.7a2/reflex/components/radix/themes/components/scrollarea.pyi
+-rw-r--r--   0        0        0     8028 2024-04-04 21:37:03.948474 reflex-0.4.7a2/reflex/components/radix/themes/components/select.py
+-rw-r--r--   0        0        0    45123 2024-04-02 19:14:34.459754 reflex-0.4.7a2/reflex/components/radix/themes/components/select.pyi
+-rw-r--r--   0        0        0      868 2024-04-02 19:14:34.459929 reflex-0.4.7a2/reflex/components/radix/themes/components/separator.py
+-rw-r--r--   0        0        0     6078 2024-04-02 19:14:34.460031 reflex-0.4.7a2/reflex/components/radix/themes/components/separator.pyi
+-rw-r--r--   0        0        0     3234 2024-04-02 19:14:34.460186 reflex-0.4.7a2/reflex/components/radix/themes/components/slider.py
+-rw-r--r--   0        0        0     8162 2024-04-02 19:14:34.460283 reflex-0.4.7a2/reflex/components/radix/themes/components/slider.pyi
+-rw-r--r--   0        0        0     1976 2024-04-02 19:14:34.460390 reflex-0.4.7a2/reflex/components/radix/themes/components/switch.py
+-rw-r--r--   0        0        0     7404 2024-04-02 19:14:34.460484 reflex-0.4.7a2/reflex/components/radix/themes/components/switch.pyi
+-rw-r--r--   0        0        0     3111 2024-04-02 19:14:34.460743 reflex-0.4.7a2/reflex/components/radix/themes/components/table.py
+-rw-r--r--   0        0        0    47387 2024-04-02 19:14:34.460872 reflex-0.4.7a2/reflex/components/radix/themes/components/table.pyi
+-rw-r--r--   0        0        0     2213 2024-04-02 19:14:34.463534 reflex-0.4.7a2/reflex/components/radix/themes/components/tabs.py
+-rw-r--r--   0        0        0    17321 2024-04-02 19:14:34.463662 reflex-0.4.7a2/reflex/components/radix/themes/components/tabs.pyi
+-rw-r--r--   0        0        0     3233 2024-04-02 19:14:34.463765 reflex-0.4.7a2/reflex/components/radix/themes/components/text_area.py
+-rw-r--r--   0        0        0    11711 2024-04-02 19:14:34.463961 reflex-0.4.7a2/reflex/components/radix/themes/components/text_area.pyi
+-rw-r--r--   0        0        0     5106 2024-04-02 19:14:34.464711 reflex-0.4.7a2/reflex/components/radix/themes/components/text_field.py
+-rw-r--r--   0        0        0    43043 2024-04-02 19:14:34.464805 reflex-0.4.7a2/reflex/components/radix/themes/components/text_field.pyi
+-rw-r--r--   0        0        0    43365 2024-04-02 19:14:34.464956 reflex-0.4.7a2/reflex/components/radix/themes/components/textfield.pyi
+-rw-r--r--   0        0        0     4465 2024-04-02 19:14:34.465166 reflex-0.4.7a2/reflex/components/radix/themes/components/tooltip.py
+-rw-r--r--   0        0        0     8092 2024-04-02 19:14:34.465305 reflex-0.4.7a2/reflex/components/radix/themes/components/tooltip.pyi
+-rw-r--r--   0        0        0      811 2024-04-02 19:14:34.465647 reflex-0.4.7a2/reflex/components/radix/themes/layout/__init__.py
+-rw-r--r--   0        0        0     1201 2024-04-02 19:14:34.465990 reflex-0.4.7a2/reflex/components/radix/themes/layout/base.py
+-rw-r--r--   0        0        0     7643 2024-04-02 19:14:34.466154 reflex-0.4.7a2/reflex/components/radix/themes/layout/base.pyi
+-rw-r--r--   0        0        0      281 2024-02-10 02:26:35.060028 reflex-0.4.7a2/reflex/components/radix/themes/layout/box.py
+-rw-r--r--   0        0        0     6462 2024-04-02 19:14:34.466266 reflex-0.4.7a2/reflex/components/radix/themes/layout/box.pyi
+-rw-r--r--   0        0        0      422 2024-04-02 19:14:34.466627 reflex-0.4.7a2/reflex/components/radix/themes/layout/center.py
+-rw-r--r--   0        0        0     8245 2024-04-02 19:14:34.466794 reflex-0.4.7a2/reflex/components/radix/themes/layout/center.pyi
+-rw-r--r--   0        0        0      552 2024-02-10 02:26:35.060445 reflex-0.4.7a2/reflex/components/radix/themes/layout/container.py
+-rw-r--r--   0        0        0     6779 2024-04-02 19:14:34.466930 reflex-0.4.7a2/reflex/components/radix/themes/layout/container.pyi
+-rw-r--r--   0        0        0     1374 2024-04-02 19:14:34.467197 reflex-0.4.7a2/reflex/components/radix/themes/layout/flex.py
+-rw-r--r--   0        0        0     8501 2024-04-02 19:14:34.467710 reflex-0.4.7a2/reflex/components/radix/themes/layout/flex.pyi
+-rw-r--r--   0        0        0     1498 2024-04-02 19:14:34.468616 reflex-0.4.7a2/reflex/components/radix/themes/layout/grid.py
+-rw-r--r--   0        0        0     8907 2024-04-02 19:14:34.468790 reflex-0.4.7a2/reflex/components/radix/themes/layout/grid.pyi
+-rw-r--r--   0        0        0     4889 2024-04-02 19:14:34.469076 reflex-0.4.7a2/reflex/components/radix/themes/layout/list.py
+-rw-r--r--   0        0        0    29367 2024-04-02 19:14:34.469203 reflex-0.4.7a2/reflex/components/radix/themes/layout/list.pyi
+-rw-r--r--   0        0        0      458 2024-02-10 02:26:35.060937 reflex-0.4.7a2/reflex/components/radix/themes/layout/section.py
+-rw-r--r--   0        0        0     6758 2024-04-02 19:14:34.469367 reflex-0.4.7a2/reflex/components/radix/themes/layout/section.pyi
+-rw-r--r--   0        0        0      412 2024-04-02 19:14:34.469593 reflex-0.4.7a2/reflex/components/radix/themes/layout/spacer.py
+-rw-r--r--   0        0        0     8245 2024-04-02 19:14:34.469727 reflex-0.4.7a2/reflex/components/radix/themes/layout/spacer.pyi
+-rw-r--r--   0        0        0     1270 2024-04-02 19:14:34.469849 reflex-0.4.7a2/reflex/components/radix/themes/layout/stack.py
+-rw-r--r--   0        0        0    22132 2024-04-02 19:14:34.470027 reflex-0.4.7a2/reflex/components/radix/themes/layout/stack.pyi
+-rw-r--r--   0        0        0      343 2024-04-02 19:14:34.470193 reflex-0.4.7a2/reflex/components/radix/themes/typography/__init__.py
+-rw-r--r--   0        0        0      408 2024-02-10 02:26:35.061693 reflex-0.4.7a2/reflex/components/radix/themes/typography/base.py
+-rw-r--r--   0        0        0      799 2024-02-10 02:26:35.061822 reflex-0.4.7a2/reflex/components/radix/themes/typography/blockquote.py
+-rw-r--r--   0        0        0     9316 2024-04-02 19:14:34.470311 reflex-0.4.7a2/reflex/components/radix/themes/typography/blockquote.pyi
+-rw-r--r--   0        0        0      909 2024-02-10 02:26:35.062001 reflex-0.4.7a2/reflex/components/radix/themes/typography/code.py
+-rw-r--r--   0        0        0     9513 2024-04-02 19:14:34.470410 reflex-0.4.7a2/reflex/components/radix/themes/typography/code.pyi
+-rw-r--r--   0        0        0     8547 2024-04-02 19:14:34.470588 reflex-0.4.7a2/reflex/components/radix/themes/typography/em.pyi
+-rw-r--r--   0        0        0     1324 2024-02-10 02:26:35.062444 reflex-0.4.7a2/reflex/components/radix/themes/typography/heading.py
+-rw-r--r--   0        0        0    10106 2024-04-02 19:14:34.470692 reflex-0.4.7a2/reflex/components/radix/themes/typography/heading.pyi
+-rw-r--r--   0        0        0     8872 2024-04-02 19:14:34.470802 reflex-0.4.7a2/reflex/components/radix/themes/typography/kbd.pyi
+-rw-r--r--   0        0        0     3154 2024-04-02 19:14:34.471091 reflex-0.4.7a2/reflex/components/radix/themes/typography/link.py
+-rw-r--r--   0        0        0    12063 2024-04-02 19:14:34.471230 reflex-0.4.7a2/reflex/components/radix/themes/typography/link.pyi
+-rw-r--r--   0        0        0     8701 2024-04-02 19:14:34.471467 reflex-0.4.7a2/reflex/components/radix/themes/typography/quote.pyi
+-rw-r--r--   0        0        0     8563 2024-04-02 19:14:34.471621 reflex-0.4.7a2/reflex/components/radix/themes/typography/strong.pyi
+-rw-r--r--   0        0        0     2604 2024-04-02 19:14:34.472005 reflex-0.4.7a2/reflex/components/radix/themes/typography/text.py
+-rw-r--r--   0        0        0    57238 2024-04-02 19:14:34.472171 reflex-0.4.7a2/reflex/components/radix/themes/typography/text.pyi
+-rw-r--r--   0        0        0      144 2024-02-10 02:26:35.063629 reflex-0.4.7a2/reflex/components/react_player/__init__.py
+-rw-r--r--   0        0        0      185 2024-02-10 02:26:35.063689 reflex-0.4.7a2/reflex/components/react_player/audio.py
+-rw-r--r--   0        0        0     4398 2024-04-02 19:14:34.472284 reflex-0.4.7a2/reflex/components/react_player/audio.pyi
+-rw-r--r--   0        0        0     1087 2024-02-10 02:26:35.063804 reflex-0.4.7a2/reflex/components/react_player/react_player.py
+-rw-r--r--   0        0        0     4425 2024-04-02 19:14:34.472391 reflex-0.4.7a2/reflex/components/react_player/react_player.pyi
+-rw-r--r--   0        0        0      185 2024-02-10 02:26:35.063907 reflex-0.4.7a2/reflex/components/react_player/video.py
+-rw-r--r--   0        0        0     4398 2024-04-02 19:14:34.472479 reflex-0.4.7a2/reflex/components/react_player/video.pyi
+-rw-r--r--   0        0        0     2373 2024-02-10 02:26:35.064033 reflex-0.4.7a2/reflex/components/recharts/__init__.py
+-rw-r--r--   0        0        0    19595 2024-02-10 02:26:35.064126 reflex-0.4.7a2/reflex/components/recharts/cartesian.py
+-rw-r--r--   0        0        0    85500 2024-04-02 19:14:34.472660 reflex-0.4.7a2/reflex/components/recharts/cartesian.pyi
+-rw-r--r--   0        0        0    18493 2024-02-10 02:26:35.064337 reflex-0.4.7a2/reflex/components/recharts/charts.py
+-rw-r--r--   0        0        0    48757 2024-04-02 19:14:34.472846 reflex-0.4.7a2/reflex/components/recharts/charts.pyi
+-rw-r--r--   0        0        0     5624 2024-02-10 02:26:35.064489 reflex-0.4.7a2/reflex/components/recharts/general.py
+-rw-r--r--   0        0        0    23071 2024-04-02 19:14:34.472964 reflex-0.4.7a2/reflex/components/recharts/general.pyi
+-rw-r--r--   0        0        0    10410 2024-02-10 02:26:35.064657 reflex-0.4.7a2/reflex/components/recharts/polar.py
+-rw-r--r--   0        0        0    24752 2024-04-02 19:14:34.473068 reflex-0.4.7a2/reflex/components/recharts/polar.pyi
+-rw-r--r--   0        0        0     2870 2024-02-10 02:26:35.064789 reflex-0.4.7a2/reflex/components/recharts/recharts.py
+-rw-r--r--   0        0        0     8606 2024-04-02 19:14:34.473190 reflex-0.4.7a2/reflex/components/recharts/recharts.pyi
+-rw-r--r--   0        0        0      109 2024-02-10 02:26:35.064909 reflex-0.4.7a2/reflex/components/suneditor/__init__.py
+-rw-r--r--   0        0        0     7360 2024-02-10 02:26:35.064985 reflex-0.4.7a2/reflex/components/suneditor/editor.py
+-rw-r--r--   0        0        0    10330 2024-04-02 19:14:34.473324 reflex-0.4.7a2/reflex/components/suneditor/editor.pyi
+-rw-r--r--   0        0        0      152 2024-02-10 02:26:35.065200 reflex-0.4.7a2/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-12-21 01:07:08.463011 reflex-0.4.7a2/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3620 2024-02-10 02:26:35.065323 reflex-0.4.7a2/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0      387 2024-02-10 02:26:35.065376 reflex-0.4.7a2/reflex/components/tags/match_tag.py
+-rw-r--r--   0        0        0     2778 2024-04-02 19:14:34.473664 reflex-0.4.7a2/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-12-21 01:07:08.463394 reflex-0.4.7a2/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0    11082 2024-04-04 21:37:03.948613 reflex-0.4.7a2/reflex/config.py
+-rw-r--r--   0        0        0     3318 2024-04-04 21:37:03.948873 reflex-0.4.7a2/reflex/config.pyi
+-rw-r--r--   0        0        0     2036 2024-04-02 19:14:34.474441 reflex-0.4.7a2/reflex/constants/__init__.py
+-rw-r--r--   0        0        0     5640 2024-04-04 22:32:02.761988 reflex-0.4.7a2/reflex/constants/base.py
+-rw-r--r--   0        0        0     2980 2024-04-04 22:32:02.762262 reflex-0.4.7a2/reflex/constants/base.pyi
+-rw-r--r--   0        0        0     1599 2024-04-02 19:14:34.474865 reflex-0.4.7a2/reflex/constants/colors.py
+-rw-r--r--   0        0        0     4137 2024-04-04 21:37:03.949234 reflex-0.4.7a2/reflex/constants/compiler.py
+-rw-r--r--   0        0        0     1331 2024-02-10 02:26:35.066956 reflex-0.4.7a2/reflex/constants/config.py
+-rw-r--r--   0        0        0     1268 2024-04-02 19:14:34.475565 reflex-0.4.7a2/reflex/constants/custom_components.py
+-rw-r--r--   0        0        0     2668 2024-02-10 02:26:35.067613 reflex-0.4.7a2/reflex/constants/event.py
+-rw-r--r--   0        0        0     3177 2024-04-02 19:14:34.475856 reflex-0.4.7a2/reflex/constants/installer.py
+-rw-r--r--   0        0        0     1940 2024-04-02 19:14:34.476122 reflex-0.4.7a2/reflex/constants/route.py
+-rw-r--r--   0        0        0      636 2024-02-10 02:26:35.067842 reflex-0.4.7a2/reflex/constants/style.py
+-rw-r--r--   0        0        0       36 2024-04-02 19:14:34.476236 reflex-0.4.7a2/reflex/custom_components/__init__.py
+-rw-r--r--   0        0        0    32096 2024-04-08 21:11:25.548185 reflex-0.4.7a2/reflex/custom_components/custom_components.py
+-rw-r--r--   0        0        0    26634 2024-04-05 22:42:13.970118 reflex-0.4.7a2/reflex/event.py
+-rw-r--r--   0        0        0      287 2024-04-04 21:37:03.949637 reflex-0.4.7a2/reflex/experimental/__init__.py
+-rw-r--r--   0        0        0     1647 2024-04-04 21:37:03.949706 reflex-0.4.7a2/reflex/experimental/hooks.py
+-rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.4.7a2/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1484 2024-04-02 19:14:34.477238 reflex-0.4.7a2/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1169 2023-12-04 22:31:51.618237 reflex-0.4.7a2/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0    13091 2024-04-06 01:57:36.880449 reflex-0.4.7a2/reflex/model.py
+-rw-r--r--   0        0        0     1921 2024-04-04 21:37:03.949824 reflex-0.4.7a2/reflex/page.py
+-rw-r--r--   0        0        0    17871 2024-04-04 22:32:02.763178 reflex-0.4.7a2/reflex/reflex.py
+-rw-r--r--   0        0        0     2908 2024-04-02 19:14:34.478054 reflex-0.4.7a2/reflex/route.py
+-rw-r--r--   0        0        0   105642 2024-04-02 19:14:34.478448 reflex-0.4.7a2/reflex/state.py
+-rw-r--r--   0        0        0     8834 2024-04-04 21:37:03.950185 reflex-0.4.7a2/reflex/style.py
+-rw-r--r--   0        0        0    29808 2024-04-04 22:32:02.763768 reflex-0.4.7a2/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-11-07 19:58:07.486037 reflex-0.4.7a2/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     8573 2024-02-10 02:26:35.070031 reflex-0.4.7a2/reflex/utils/build.py
+-rw-r--r--   0        0        0     5018 2024-04-04 22:32:02.764358 reflex-0.4.7a2/reflex/utils/console.py
+-rw-r--r--   0        0        0      504 2024-02-10 02:26:35.070129 reflex-0.4.7a2/reflex/utils/exceptions.py
+-rw-r--r--   0        0        0     9969 2024-04-04 21:37:03.950843 reflex-0.4.7a2/reflex/utils/exec.py
+-rw-r--r--   0        0        0     2357 2024-04-04 21:37:03.951057 reflex-0.4.7a2/reflex/utils/export.py
+-rw-r--r--   0        0        0    22648 2024-04-02 19:14:34.479804 reflex-0.4.7a2/reflex/utils/format.py
+-rw-r--r--   0        0        0     1919 2023-12-04 22:31:51.620673 reflex-0.4.7a2/reflex/utils/imports.py
+-rw-r--r--   0        0        0     4737 2024-02-10 02:26:35.070893 reflex-0.4.7a2/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    45757 2024-04-05 22:41:26.508584 reflex-0.4.7a2/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     8481 2024-04-04 21:37:03.951498 reflex-0.4.7a2/reflex/utils/processes.py
+-rw-r--r--   0        0        0    27674 2024-04-02 19:14:34.480893 reflex-0.4.7a2/reflex/utils/pyi_generator.py
+-rw-r--r--   0        0        0     8538 2024-04-08 18:50:32.983082 reflex-0.4.7a2/reflex/utils/serializers.py
+-rw-r--r--   0        0        0     4013 2024-04-04 21:37:03.951599 reflex-0.4.7a2/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0    13585 2024-04-06 01:57:36.880891 reflex-0.4.7a2/reflex/utils/types.py
+-rw-r--r--   0        0        0     2609 2023-11-21 01:55:15.773146 reflex-0.4.7a2/reflex/utils/watch.py
+-rw-r--r--   0        0        0    67152 2024-04-04 21:37:03.951876 reflex-0.4.7a2/reflex/vars.py
+-rw-r--r--   0        0        0     5583 2024-04-04 21:37:03.951997 reflex-0.4.7a2/reflex/vars.pyi
+-rw-r--r--   0        0        0    11815 1970-01-01 00:00:00.000000 reflex-0.4.7a2/PKG-INFO
```

### Comparing `reflex-0.4.7a1/LICENSE` & `reflex-0.4.7a2/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/README.md` & `reflex-0.4.7a2/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/pyproject.toml` & `reflex-0.4.7a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.4.7a1"
+version = "0.4.7a2"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@reflex.dev>",
     "Alek Petuskey <alek@reflex.dev>",
     "Masen Furer <masen@reflex.dev>",
     "Elijah Ahianyo <elijah@reflex.dev>",
```

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/blank/assets/favicon.ico` & `reflex-0.4.7a2/reflex/.templates/apps/blank/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/blank/code/blank.py` & `reflex-0.4.7a2/reflex/.templates/apps/blank/code/blank.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/assets/favicon.ico` & `reflex-0.4.7a2/reflex/.templates/apps/demo/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/assets/github.svg` & `reflex-0.4.7a2/reflex/.templates/apps/demo/assets/github.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/assets/icon.svg` & `reflex-0.4.7a2/reflex/.templates/apps/demo/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/assets/logo.svg` & `reflex-0.4.7a2/reflex/.templates/apps/demo/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/assets/paneleft.svg` & `reflex-0.4.7a2/reflex/.templates/apps/demo/assets/paneleft.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/demo.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/demo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/pages/chatapp.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/pages/chatapp.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/pages/datatable.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/pages/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/pages/forms.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/pages/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/pages/graphing.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/pages/graphing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/pages/home.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/pages/home.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/sidebar.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/states/form_state.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/states/form_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/states/pie_state.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/states/pie_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/styles.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/components/chat.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/components/chat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/components/loading_icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/components/modal.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/components/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/components/navbar.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/components/navbar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/components/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/state.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/apps/demo/code/webui/styles.py` & `reflex-0.4.7a2/reflex/.templates/apps/demo/code/webui/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2` & `reflex-0.4.7a2/reflex/.templates/jinja/custom_components/demo_app.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2` & `reflex-0.4.7a2/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/jinja/custom_components/src.py.jinja2` & `reflex-0.4.7a2/reflex/.templates/jinja/custom_components/src.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/jinja/web/package.json.jinja2` & `reflex-0.4.7a2/reflex/.templates/jinja/web/package.json.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/jinja/web/pages/_app.js.jinja2` & `reflex-0.4.7a2/reflex/.templates/jinja/web/pages/_app.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2` & `reflex-0.4.7a2/reflex/.templates/jinja/web/pages/custom_component.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.4.7a2/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/jinja/web/utils/context.js.jinja2` & `reflex-0.4.7a2/reflex/.templates/jinja/web/utils/context.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js` & `reflex-0.4.7a2/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js` & `reflex-0.4.7a2/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/web/utils/client_side_routing.js` & `reflex-0.4.7a2/reflex/.templates/web/utils/client_side_routing.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/web/utils/helpers/dataeditor.js` & `reflex-0.4.7a2/reflex/.templates/web/utils/helpers/dataeditor.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/web/utils/helpers/range.js` & `reflex-0.4.7a2/reflex/.templates/web/utils/helpers/range.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/.templates/web/utils/state.js` & `reflex-0.4.7a2/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/__init__.py` & `reflex-0.4.7a2/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/__init__.pyi` & `reflex-0.4.7a2/reflex/__init__.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/app.py` & `reflex-0.4.7a2/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/app.pyi` & `reflex-0.4.7a2/reflex/app.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/app_module_for_backend.py` & `reflex-0.4.7a2/reflex/app_module_for_backend.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/base.py` & `reflex-0.4.7a2/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/compiler/compiler.py` & `reflex-0.4.7a2/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/compiler/templates.py` & `reflex-0.4.7a2/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/compiler/utils.py` & `reflex-0.4.7a2/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/__init__.py` & `reflex-0.4.7a2/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/app_wrap.py` & `reflex-0.4.7a2/reflex/components/base/app_wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/app_wrap.pyi` & `reflex-0.4.7a2/reflex/components/base/app_wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/bare.py` & `reflex-0.4.7a2/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/body.pyi` & `reflex-0.4.7a2/reflex/components/base/body.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/document.py` & `reflex-0.4.7a2/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/document.pyi` & `reflex-0.4.7a2/reflex/components/base/document.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/fragment.pyi` & `reflex-0.4.7a2/reflex/components/base/fragment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/head.pyi` & `reflex-0.4.7a2/reflex/components/base/head.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/link.py` & `reflex-0.4.7a2/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/link.pyi` & `reflex-0.4.7a2/reflex/components/base/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/meta.py` & `reflex-0.4.7a2/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/meta.pyi` & `reflex-0.4.7a2/reflex/components/base/meta.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/script.py` & `reflex-0.4.7a2/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/base/script.pyi` & `reflex-0.4.7a2/reflex/components/base/script.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/__init__.py` & `reflex-0.4.7a2/reflex/components/chakra/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/base.py` & `reflex-0.4.7a2/reflex/components/chakra/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/base.pyi` & `reflex-0.4.7a2/reflex/components/chakra/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/badge.pyi` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/code.pyi` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/divider.py` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/divider.pyi` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/keyboard_key.pyi` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/keyboard_key.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/list.py` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/list.pyi` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/stat.py` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/stat.pyi` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/stat.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/table.py` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/table.pyi` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/tag.py` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/datadisplay/tag.pyi` & `reflex-0.4.7a2/reflex/components/chakra/datadisplay/tag.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/disclosure/accordion.py` & `reflex-0.4.7a2/reflex/components/chakra/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/disclosure/accordion.pyi` & `reflex-0.4.7a2/reflex/components/chakra/disclosure/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/disclosure/tabs.py` & `reflex-0.4.7a2/reflex/components/chakra/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/disclosure/tabs.pyi` & `reflex-0.4.7a2/reflex/components/chakra/disclosure/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/disclosure/transition.py` & `reflex-0.4.7a2/reflex/components/chakra/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/disclosure/transition.pyi` & `reflex-0.4.7a2/reflex/components/chakra/disclosure/transition.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/disclosure/visuallyhidden.pyi` & `reflex-0.4.7a2/reflex/components/chakra/disclosure/visuallyhidden.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/feedback/alert.py` & `reflex-0.4.7a2/reflex/components/chakra/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/feedback/alert.pyi` & `reflex-0.4.7a2/reflex/components/chakra/feedback/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/feedback/circularprogress.py` & `reflex-0.4.7a2/reflex/components/chakra/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/feedback/circularprogress.pyi` & `reflex-0.4.7a2/reflex/components/chakra/feedback/circularprogress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/feedback/progress.py` & `reflex-0.4.7a2/reflex/components/chakra/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/feedback/progress.pyi` & `reflex-0.4.7a2/reflex/components/chakra/feedback/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/feedback/skeleton.py` & `reflex-0.4.7a2/reflex/components/chakra/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/feedback/skeleton.pyi` & `reflex-0.4.7a2/reflex/components/chakra/feedback/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/feedback/spinner.py` & `reflex-0.4.7a2/reflex/components/chakra/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/feedback/spinner.pyi` & `reflex-0.4.7a2/reflex/components/chakra/feedback/spinner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/__init__.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/button.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/button.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/checkbox.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/checkbox.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/colormodeswitch.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/colormodeswitch.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/colormodeswitch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/date_picker.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/date_time_picker.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/date_time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/editable.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/editable.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/editable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/email.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/email.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/form.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/form.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/iconbutton.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/iconbutton.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/iconbutton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/input.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/input.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/multiselect.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/numberinput.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/numberinput.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/numberinput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/password.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/password.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/pininput.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/pininput.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/pininput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/radio.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/radio.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/rangeslider.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/rangeslider.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/rangeslider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/select.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/select.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/slider.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/slider.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/switch.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/switch.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/textarea.py` & `reflex-0.4.7a2/reflex/components/chakra/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/textarea.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/textarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/forms/time_picker.pyi` & `reflex-0.4.7a2/reflex/components/chakra/forms/time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/aspect_ratio.pyi` & `reflex-0.4.7a2/reflex/components/chakra/layout/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/box.py` & `reflex-0.4.7a2/reflex/components/chakra/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/box.pyi` & `reflex-0.4.7a2/reflex/components/chakra/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/card.py` & `reflex-0.4.7a2/reflex/components/chakra/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/card.pyi` & `reflex-0.4.7a2/reflex/components/chakra/layout/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/center.pyi` & `reflex-0.4.7a2/reflex/components/chakra/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/container.pyi` & `reflex-0.4.7a2/reflex/components/chakra/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/flex.py` & `reflex-0.4.7a2/reflex/components/chakra/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/flex.pyi` & `reflex-0.4.7a2/reflex/components/chakra/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/grid.py` & `reflex-0.4.7a2/reflex/components/chakra/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/grid.pyi` & `reflex-0.4.7a2/reflex/components/chakra/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/spacer.pyi` & `reflex-0.4.7a2/reflex/components/chakra/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/stack.py` & `reflex-0.4.7a2/reflex/components/chakra/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/stack.pyi` & `reflex-0.4.7a2/reflex/components/chakra/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/wrap.py` & `reflex-0.4.7a2/reflex/components/chakra/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/layout/wrap.pyi` & `reflex-0.4.7a2/reflex/components/chakra/layout/wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/media/avatar.py` & `reflex-0.4.7a2/reflex/components/chakra/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/media/avatar.pyi` & `reflex-0.4.7a2/reflex/components/chakra/media/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/media/icon.py` & `reflex-0.4.7a2/reflex/components/chakra/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/media/icon.pyi` & `reflex-0.4.7a2/reflex/components/chakra/media/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/media/image.py` & `reflex-0.4.7a2/reflex/components/chakra/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/media/image.pyi` & `reflex-0.4.7a2/reflex/components/chakra/media/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/navigation/breadcrumb.py` & `reflex-0.4.7a2/reflex/components/chakra/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/navigation/breadcrumb.pyi` & `reflex-0.4.7a2/reflex/components/chakra/navigation/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/navigation/link.py` & `reflex-0.4.7a2/reflex/components/chakra/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/navigation/link.pyi` & `reflex-0.4.7a2/reflex/components/chakra/navigation/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/navigation/linkoverlay.py` & `reflex-0.4.7a2/reflex/components/chakra/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/navigation/linkoverlay.pyi` & `reflex-0.4.7a2/reflex/components/chakra/navigation/linkoverlay.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/navigation/stepper.py` & `reflex-0.4.7a2/reflex/components/chakra/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/navigation/stepper.pyi` & `reflex-0.4.7a2/reflex/components/chakra/navigation/stepper.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/__init__.py` & `reflex-0.4.7a2/reflex/components/chakra/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/alertdialog.py` & `reflex-0.4.7a2/reflex/components/chakra/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/alertdialog.pyi` & `reflex-0.4.7a2/reflex/components/chakra/overlay/alertdialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/drawer.py` & `reflex-0.4.7a2/reflex/components/chakra/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/drawer.pyi` & `reflex-0.4.7a2/reflex/components/chakra/overlay/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/menu.py` & `reflex-0.4.7a2/reflex/components/chakra/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/menu.pyi` & `reflex-0.4.7a2/reflex/components/chakra/overlay/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/modal.py` & `reflex-0.4.7a2/reflex/components/chakra/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/modal.pyi` & `reflex-0.4.7a2/reflex/components/chakra/overlay/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/popover.py` & `reflex-0.4.7a2/reflex/components/chakra/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/popover.pyi` & `reflex-0.4.7a2/reflex/components/chakra/overlay/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/tooltip.py` & `reflex-0.4.7a2/reflex/components/chakra/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/overlay/tooltip.pyi` & `reflex-0.4.7a2/reflex/components/chakra/overlay/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/typography/heading.pyi` & `reflex-0.4.7a2/reflex/components/chakra/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/typography/highlight.py` & `reflex-0.4.7a2/reflex/components/chakra/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/typography/highlight.pyi` & `reflex-0.4.7a2/reflex/components/chakra/typography/highlight.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/typography/span.pyi` & `reflex-0.4.7a2/reflex/components/chakra/typography/span.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/chakra/typography/text.pyi` & `reflex-0.4.7a2/reflex/components/chakra/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/component.py` & `reflex-0.4.7a2/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/__init__.py` & `reflex-0.4.7a2/reflex/components/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/banner.py` & `reflex-0.4.7a2/reflex/components/core/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/banner.pyi` & `reflex-0.4.7a2/reflex/components/core/banner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/client_side_routing.py` & `reflex-0.4.7a2/reflex/components/core/client_side_routing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/client_side_routing.pyi` & `reflex-0.4.7a2/reflex/components/core/client_side_routing.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/colors.py` & `reflex-0.4.7a2/reflex/components/core/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/cond.py` & `reflex-0.4.7a2/reflex/components/core/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/debounce.py` & `reflex-0.4.7a2/reflex/components/core/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/debounce.pyi` & `reflex-0.4.7a2/reflex/components/core/debounce.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/foreach.py` & `reflex-0.4.7a2/reflex/components/core/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/html.py` & `reflex-0.4.7a2/reflex/components/core/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/html.pyi` & `reflex-0.4.7a2/reflex/components/core/html.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/match.py` & `reflex-0.4.7a2/reflex/components/core/match.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/responsive.py` & `reflex-0.4.7a2/reflex/components/core/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/upload.py` & `reflex-0.4.7a2/reflex/components/core/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/core/upload.pyi` & `reflex-0.4.7a2/reflex/components/core/upload.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/datadisplay/code.py` & `reflex-0.4.7a2/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/datadisplay/code.pyi` & `reflex-0.4.7a2/reflex/components/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/datadisplay/dataeditor.py` & `reflex-0.4.7a2/reflex/components/datadisplay/dataeditor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/datadisplay/dataeditor.pyi` & `reflex-0.4.7a2/reflex/components/datadisplay/dataeditor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/datadisplay/logo.py` & `reflex-0.4.7a2/reflex/components/datadisplay/logo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/constants/html.py` & `reflex-0.4.7a2/reflex/components/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/constants/react.py` & `reflex-0.4.7a2/reflex/components/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/constants/reflex.py` & `reflex-0.4.7a2/reflex/components/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/element.pyi` & `reflex-0.4.7a2/reflex/components/el/element.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/__init__.py` & `reflex-0.4.7a2/reflex/components/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/base.py` & `reflex-0.4.7a2/reflex/components/el/elements/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/base.pyi` & `reflex-0.4.7a2/reflex/components/el/elements/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/forms.py` & `reflex-0.4.7a2/reflex/components/el/elements/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/forms.pyi` & `reflex-0.4.7a2/reflex/components/el/elements/forms.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/inline.py` & `reflex-0.4.7a2/reflex/components/el/elements/inline.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/inline.pyi` & `reflex-0.4.7a2/reflex/components/el/elements/inline.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/media.py` & `reflex-0.4.7a2/reflex/components/el/elements/media.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/media.pyi` & `reflex-0.4.7a2/reflex/components/el/elements/media.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/metadata.py` & `reflex-0.4.7a2/reflex/components/el/elements/metadata.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/metadata.pyi` & `reflex-0.4.7a2/reflex/components/el/elements/metadata.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/other.py` & `reflex-0.4.7a2/reflex/components/el/elements/other.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/other.pyi` & `reflex-0.4.7a2/reflex/components/el/elements/other.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/scripts.py` & `reflex-0.4.7a2/reflex/components/el/elements/scripts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/scripts.pyi` & `reflex-0.4.7a2/reflex/components/el/elements/scripts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/sectioning.py` & `reflex-0.4.7a2/reflex/components/el/elements/sectioning.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/sectioning.pyi` & `reflex-0.4.7a2/reflex/components/el/elements/sectioning.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/tables.py` & `reflex-0.4.7a2/reflex/components/el/elements/tables.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/tables.pyi` & `reflex-0.4.7a2/reflex/components/el/elements/tables.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/typography.py` & `reflex-0.4.7a2/reflex/components/el/elements/typography.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/el/elements/typography.pyi` & `reflex-0.4.7a2/reflex/components/el/elements/typography.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/gridjs/datatable.py` & `reflex-0.4.7a2/reflex/components/gridjs/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/gridjs/datatable.pyi` & `reflex-0.4.7a2/reflex/components/gridjs/datatable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/lucide/icon.py` & `reflex-0.4.7a2/reflex/components/lucide/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/lucide/icon.pyi` & `reflex-0.4.7a2/reflex/components/lucide/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/markdown/markdown.py` & `reflex-0.4.7a2/reflex/components/markdown/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/markdown/markdown.pyi` & `reflex-0.4.7a2/reflex/components/markdown/markdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/moment/moment.py` & `reflex-0.4.7a2/reflex/components/moment/moment.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/moment/moment.pyi` & `reflex-0.4.7a2/reflex/components/moment/moment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/next/base.pyi` & `reflex-0.4.7a2/reflex/components/next/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/next/image.py` & `reflex-0.4.7a2/reflex/components/next/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/next/image.pyi` & `reflex-0.4.7a2/reflex/components/next/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/next/link.pyi` & `reflex-0.4.7a2/reflex/components/next/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/next/video.py` & `reflex-0.4.7a2/reflex/components/next/video.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/next/video.pyi` & `reflex-0.4.7a2/reflex/components/next/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/plotly/plotly.py` & `reflex-0.4.7a2/reflex/components/plotly/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/plotly/plotly.pyi` & `reflex-0.4.7a2/reflex/components/plotly/plotly.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/primitives/accordion.py` & `reflex-0.4.7a2/reflex/components/radix/primitives/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/primitives/accordion.pyi` & `reflex-0.4.7a2/reflex/components/radix/primitives/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/primitives/base.py` & `reflex-0.4.7a2/reflex/components/radix/primitives/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/primitives/base.pyi` & `reflex-0.4.7a2/reflex/components/radix/primitives/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/primitives/drawer.py` & `reflex-0.4.7a2/reflex/components/radix/primitives/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/primitives/drawer.pyi` & `reflex-0.4.7a2/reflex/components/radix/primitives/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/primitives/form.py` & `reflex-0.4.7a2/reflex/components/radix/primitives/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/primitives/form.pyi` & `reflex-0.4.7a2/reflex/components/radix/primitives/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/primitives/progress.py` & `reflex-0.4.7a2/reflex/components/radix/primitives/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/primitives/progress.pyi` & `reflex-0.4.7a2/reflex/components/radix/primitives/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/primitives/slider.py` & `reflex-0.4.7a2/reflex/components/radix/primitives/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/primitives/slider.pyi` & `reflex-0.4.7a2/reflex/components/radix/primitives/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/base.py` & `reflex-0.4.7a2/reflex/components/radix/themes/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/base.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/color_mode.py` & `reflex-0.4.7a2/reflex/components/radix/themes/color_mode.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/color_mode.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/color_mode.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/__init__.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/alert_dialog.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/alert_dialog.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/alert_dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/alertdialog.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/alertdialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/aspect_ratio.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/aspectratio.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/aspectratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/avatar.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/avatar.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/badge.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/badge.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/badge.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/button.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/button.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/callout.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/callout.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/callout.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/callout.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/card.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/card.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/checkbox.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/checkbox.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/context_menu.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/context_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/context_menu.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/context_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/contextmenu.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/contextmenu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/dialog.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/dialog.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/dropdown_menu.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/dropdown_menu.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/dropdown_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/dropdownmenu.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/dropdownmenu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/hover_card.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/hover_card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/hover_card.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/hover_card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/hovercard.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/hovercard.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/icon_button.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/icon_button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/icon_button.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/icon_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/iconbutton.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/iconbutton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/inset.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/inset.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/inset.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/inset.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/popover.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/popover.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/radio_group.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/radio_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/radio_group.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/radio_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/radiogroup.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/radiogroup.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/scroll_area.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/scroll_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/scroll_area.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/scroll_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/scrollarea.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/scrollarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/select.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/select.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/separator.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/separator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/separator.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/separator.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/slider.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/slider.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/switch.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/switch.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/table.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/table.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/tabs.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/tabs.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/text_area.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/text_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/text_area.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/text_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/text_field.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/text_field.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/text_field.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/text_field.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/textfield.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/textfield.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/tooltip.py` & `reflex-0.4.7a2/reflex/components/radix/themes/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/components/tooltip.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/components/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/__init__.py` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/base.py` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/base.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/box.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/center.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/container.py` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/container.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/container.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/flex.py` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/flex.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/grid.py` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/grid.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/list.py` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/list.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/section.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/section.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/spacer.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/stack.py` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/layout/stack.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/blockquote.py` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/blockquote.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/blockquote.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/blockquote.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/code.py` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/code.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/em.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/em.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/heading.py` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/heading.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/heading.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/kbd.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/kbd.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/link.py` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/link.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/quote.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/quote.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/strong.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/strong.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/text.py` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/text.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/radix/themes/typography/text.pyi` & `reflex-0.4.7a2/reflex/components/radix/themes/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/react_player/audio.pyi` & `reflex-0.4.7a2/reflex/components/react_player/audio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/react_player/react_player.py` & `reflex-0.4.7a2/reflex/components/react_player/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/react_player/react_player.pyi` & `reflex-0.4.7a2/reflex/components/react_player/react_player.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/react_player/video.pyi` & `reflex-0.4.7a2/reflex/components/react_player/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/recharts/__init__.py` & `reflex-0.4.7a2/reflex/components/recharts/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/recharts/cartesian.py` & `reflex-0.4.7a2/reflex/components/recharts/cartesian.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/recharts/cartesian.pyi` & `reflex-0.4.7a2/reflex/components/recharts/cartesian.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/recharts/charts.py` & `reflex-0.4.7a2/reflex/components/recharts/charts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/recharts/charts.pyi` & `reflex-0.4.7a2/reflex/components/recharts/charts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/recharts/general.py` & `reflex-0.4.7a2/reflex/components/recharts/general.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/recharts/general.pyi` & `reflex-0.4.7a2/reflex/components/recharts/general.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/recharts/polar.py` & `reflex-0.4.7a2/reflex/components/recharts/polar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/recharts/polar.pyi` & `reflex-0.4.7a2/reflex/components/recharts/polar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/recharts/recharts.py` & `reflex-0.4.7a2/reflex/components/recharts/recharts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/recharts/recharts.pyi` & `reflex-0.4.7a2/reflex/components/recharts/recharts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/suneditor/editor.py` & `reflex-0.4.7a2/reflex/components/suneditor/editor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/suneditor/editor.pyi` & `reflex-0.4.7a2/reflex/components/suneditor/editor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/tags/iter_tag.py` & `reflex-0.4.7a2/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/tags/tag.py` & `reflex-0.4.7a2/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/components/tags/tagless.py` & `reflex-0.4.7a2/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/config.py` & `reflex-0.4.7a2/reflex/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/config.pyi` & `reflex-0.4.7a2/reflex/config.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/constants/__init__.py` & `reflex-0.4.7a2/reflex/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/constants/base.py` & `reflex-0.4.7a2/reflex/constants/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/constants/base.pyi` & `reflex-0.4.7a2/reflex/constants/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/constants/colors.py` & `reflex-0.4.7a2/reflex/constants/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/constants/compiler.py` & `reflex-0.4.7a2/reflex/constants/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/constants/config.py` & `reflex-0.4.7a2/reflex/constants/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/constants/custom_components.py` & `reflex-0.4.7a2/reflex/constants/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/constants/event.py` & `reflex-0.4.7a2/reflex/constants/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/constants/installer.py` & `reflex-0.4.7a2/reflex/constants/installer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/constants/route.py` & `reflex-0.4.7a2/reflex/constants/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/constants/style.py` & `reflex-0.4.7a2/reflex/constants/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/custom_components/custom_components.py` & `reflex-0.4.7a2/reflex/custom_components/custom_components.py`

 * *Files 0% similar despite different names*

```diff
@@ -711,24 +711,24 @@
             "If you decide to do this later, you can run `reflex component share` command. Thank you!"
         )
         return
 
     _collect_details_for_gallery()
 
 
-def _process_entered_list(input: str) -> list | None:
+def _process_entered_list(input: str | None) -> list | None:
     """Process the user entered comma separated list into a list if applicable.
 
     Args:
         input: the user entered comma separated list
 
     Returns:
         The list of items or None.
     """
-    return [t.strip() for t in input.split(",") if t if input] or None
+    return [t.strip() for t in (input or "").split(",") if t if input] or None
 
 
 def _validate_project_info():
     """Validate the project information in the pyproject.toml file.
 
     Raises:
         Exit: If the pyproject.toml file is ill-formed.
@@ -769,22 +769,23 @@
     if keyword_action == "r":
         new_keywords = (
             _process_entered_list(
                 console.ask("Enter new set of keywords separated by commas")
             )
             or []
         )
+        project["keywords"] = new_keywords
     elif keyword_action == "a":
         new_keywords = (
             _process_entered_list(
                 console.ask("Enter new set of keywords separated by commas")
             )
             or []
         )
-    project["keywords"] = project.get("keywords", []) + new_keywords
+        project["keywords"] = project.get("keywords", []) + new_keywords
 
     if not project.get("urls"):
         project["urls"] = {}
     project["urls"]["homepage"] = console.ask(
         "homepage URL", default=project["urls"].get("homepage", "")
     )
     project["urls"]["source"] = console.ask(
```

### Comparing `reflex-0.4.7a1/reflex/event.py` & `reflex-0.4.7a2/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/experimental/hooks.py` & `reflex-0.4.7a2/reflex/experimental/hooks.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/middleware/hydrate_middleware.py` & `reflex-0.4.7a2/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/middleware/middleware.py` & `reflex-0.4.7a2/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/model.py` & `reflex-0.4.7a2/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/page.py` & `reflex-0.4.7a2/reflex/page.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/reflex.py` & `reflex-0.4.7a2/reflex/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/route.py` & `reflex-0.4.7a2/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/state.py` & `reflex-0.4.7a2/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/style.py` & `reflex-0.4.7a2/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/testing.py` & `reflex-0.4.7a2/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/build.py` & `reflex-0.4.7a2/reflex/utils/build.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/console.py` & `reflex-0.4.7a2/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/exec.py` & `reflex-0.4.7a2/reflex/utils/exec.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/export.py` & `reflex-0.4.7a2/reflex/utils/export.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/format.py` & `reflex-0.4.7a2/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/imports.py` & `reflex-0.4.7a2/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/path_ops.py` & `reflex-0.4.7a2/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/prerequisites.py` & `reflex-0.4.7a2/reflex/utils/prerequisites.py`

 * *Files 1% similar despite different names*

```diff
@@ -848,15 +848,15 @@
         Whether the app needs to be reinitialized.
 
     Raises:
         Exit: If the app is not initialized.
     """
     if not os.path.exists(constants.Config.FILE):
         console.error(
-            f"{constants.Config.FILE} not found. Run [bold]{constants.Reflex.MODULE_NAME} init[/bold] first."
+            f"[cyan]{constants.Config.FILE}[/cyan] not found. Move to the root folder of your project, or run [bold]{constants.Reflex.MODULE_NAME} init[/bold] to start a new project."
         )
         raise typer.Exit(1)
 
     # Make sure the .reflex directory exists.
     if not os.path.exists(constants.Reflex.DIR):
         return True
```

### Comparing `reflex-0.4.7a1/reflex/utils/processes.py` & `reflex-0.4.7a2/reflex/utils/processes.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/pyi_generator.py` & `reflex-0.4.7a2/reflex/utils/pyi_generator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/serializers.py` & `reflex-0.4.7a2/reflex/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/telemetry.py` & `reflex-0.4.7a2/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/types.py` & `reflex-0.4.7a2/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/utils/watch.py` & `reflex-0.4.7a2/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/vars.py` & `reflex-0.4.7a2/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/reflex/vars.pyi` & `reflex-0.4.7a2/reflex/vars.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.7a1/PKG-INFO` & `reflex-0.4.7a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.4.7a1
+Version: 0.4.7a2
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@reflex.dev
 Requires-Python: >=3.8,<4.0
```

