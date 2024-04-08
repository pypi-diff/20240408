# Comparing `tmp/django_xprez-0.2.8.tar.gz` & `tmp/django_xprez-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_xprez-0.2.8.tar", last modified: Thu Dec 21 11:16:26 2023, max compression
+gzip compressed data, was "django_xprez-0.2.9.tar", last modified: Fri Dec 22 15:48:06 2023, max compression
```

## Comparing `django_xprez-0.2.8.tar` & `django_xprez-0.2.9.tar`

### file list

```diff
@@ -1,822 +1,822 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.288081 django_xprez-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-21 11:16:17.000000 django_xprez-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-21 11:16:17.000000 django_xprez-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2023-12-21 11:16:26.288081 django_xprez-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2023-12-21 11:16:17.000000 django_xprez-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.288081 django_xprez-0.2.8/django_xprez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2023-12-21 11:16:26.000000 django_xprez-0.2.8/django_xprez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    39409 2023-12-21 11:16:26.000000 django_xprez-0.2.8/django_xprez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 11:16:26.000000 django_xprez-0.2.8/django_xprez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-21 11:16:26.000000 django_xprez-0.2.8/django_xprez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-21 11:16:26.000000 django_xprez-0.2.8/django_xprez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 11:16:26.288081 django_xprez-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-12-21 11:16:17.000000 django_xprez-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.148080 django_xprez-0.2.8/xprez/
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8387 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/admin_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.148080 django_xprez-0.2.8/xprez/ck_editor/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/parse_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.128080 django_xprez-0.2.8/xprez/ck_editor/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.128080 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.148080 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/js/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/js/ck_editor_widget.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.128080 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.152080 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/
--rw-r--r--   0 runner    (1001) docker     (127)   899705 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/ckeditor.js
--rw-r--r--   0 runner    (1001) docker     (127)  4801287 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/ckeditor.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.168080 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/af.js
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ar.js
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ast.js
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/az.js
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/bg.js
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/cs.js
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/da.js
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/de-ch.js
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/de.js
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/el.js
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/en-au.js
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/en-gb.js
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/eo.js
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/es.js
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/et.js
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/eu.js
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/fa.js
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/fi.js
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/fr.js
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/gl.js
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/gu.js
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/he.js
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/hi.js
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/hr.js
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/hu.js
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/id.js
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/it.js
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ja.js
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/km.js
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/kn.js
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ko.js
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ku.js
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/lt.js
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/lv.js
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/nb.js
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ne.js
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/nl.js
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/no.js
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/oc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/pl.js
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/pt-br.js
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/pt.js
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ro.js
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ru.js
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/si.js
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sk.js
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sl.js
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sq.js
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sr-latn.js
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sr.js
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sv.js
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/th.js
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/tk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/tr.js
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/tt.js
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ug.js
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/uk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/vi.js
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/zh-cn.js
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/zh.js
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/ck_editor/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.168080 django_xprez-0.2.8/xprez/code_snippet/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/code_snippet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/code_snippet/admin_forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.168080 django_xprez-0.2.8/xprez/code_snippet/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/code_snippet/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/code_snippet/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/code_snippet/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.128080 django_xprez-0.2.8/xprez/code_snippet/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.128080 django_xprez-0.2.8/xprez/code_snippet/static/xprez/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.128080 django_xprez-0.2.8/xprez/code_snippet/static/xprez/css/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.172080 django_xprez-0.2.8/xprez/code_snippet/static/xprez/css/pygments/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/code_snippet/static/xprez/css/pygments/colorful.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.172080 django_xprez-0.2.8/xprez/code_snippet/static/xprez/js/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/code_snippet/static/xprez/js/textarea_with_tabs.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.128080 django_xprez-0.2.8/xprez/code_snippet/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.172080 django_xprez-0.2.8/xprez/code_snippet/templates/xprez/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.172080 django_xprez-0.2.8/xprez/code_snippet/templates/xprez/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/code_snippet/templates/xprez/admin/code_snippet.html
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/code_snippet/templates/xprez/code_snippet.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.172080 django_xprez-0.2.8/xprez/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/conf/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.172080 django_xprez-0.2.8/xprez/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.172080 django_xprez-0.2.8/xprez/contrib/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/contrib/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/contrib/rest_framework/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.172080 django_xprez-0.2.8/xprez/contrib/sorl_thumbnail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/contrib/sorl_thumbnail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/contrib/sorl_thumbnail/thumbnail_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/form_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.172080 django_xprez-0.2.8/xprez/medium_editor/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/medium_editor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.128080 django_xprez-0.2.8/xprez/medium_editor/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.128080 django_xprez-0.2.8/xprez/medium_editor/static/medium_editor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.172080 django_xprez-0.2.8/xprez/medium_editor/static/medium_editor/css/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/medium_editor/static/medium_editor/css/medium_editor_widget.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.172080 django_xprez-0.2.8/xprez/medium_editor/static/medium_editor/js/
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/medium_editor/static/medium_editor/js/medium_editor_widget.js
--rw-r--r--   0 runner    (1001) docker     (127)      322 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/medium_editor/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/medium_editor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/medium_editor/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/medium_editor/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.176081 django_xprez-0.2.8/xprez/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    14460 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0002_auto_20180115_1306.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0003_auto_20180117_0930.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0004_auto_20180504_1516.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0005_auto_20191025_1352.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0006_contentscontainer_content_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0006_gridboxes.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0007_auto_20191221_1522.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0007_auto_20191227_2150.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0008_merge_20200129_1159.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0009_gridboxes_width.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0010_auto_20220204_1540.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0010_ckeditor.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0011_auto_20220204_1559.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0012_auto_20220204_1600.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0013_merge_20220207_1020.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0014_remove_content_margin_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0015_ckeditor_content_centered.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0016_auto_20220208_1355.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0017_auto_20220208_1401.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0018_auto_20220312_1845.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0019_photo_alt_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0020_alter_gridboxes_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0021_alter_ckeditor_options_alter_downloadcontent_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0022_content_alternate_color_content_background_color_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/0023_remove_content_padding_vertical_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.180081 django_xprez-0.2.8/xprez/models/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17310 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/models/contents.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/models/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.128080 django_xprez-0.2.8/xprez/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.180081 django_xprez-0.2.8/xprez/static/xprez/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.132080 django_xprez-0.2.8/xprez/static/xprez/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.180081 django_xprez-0.2.8/xprez/static/xprez/admin/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/js/ajax_upload_formset.js
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/js/contents.js
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/js/grid_boxes.js
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/js/jquery_revert_noconflict.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.140080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.180081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.180081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/canvas-to-blob.js
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/canvas-to-blob.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/canvas-to-blob.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.184080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/test.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.184080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)   158571 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/chai.js
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/load-image.js
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/mocha.css
--rw-r--r--   0 runner    (1001) docker     (127)   421025 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/mocha.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.184080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.184080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/css/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/css/jquery.fileupload-noscript.css
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/css/jquery.fileupload-ui-noscript.css
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/css/jquery.fileupload-ui.css
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/css/jquery.fileupload.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.184080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/img/
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/img/loading.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/img/progressbar.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.188080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.188080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/cors/
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/cors/jquery.postmessage-transport.js
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/cors/jquery.xdr-transport.js
--rw-r--r--   0 runner    (1001) docker     (127)    16607 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-angular.js
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-audio.js
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-image.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     5171 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-process.js
--rw-r--r--   0 runner    (1001) docker     (127)    27848 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-ui.js
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-validate.js
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-video.js
--rw-r--r--   0 runner    (1001) docker     (127)    63666 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload.js
--rw-r--r--   0 runner    (1001) docker     (127)    10723 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.iframe-transport.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.188080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)    16089 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/vendor/jquery.ui.widget.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.188080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11510 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.188080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/css/demo.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.188080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/css/vendor/
--rwxr-xr-x   0 runner    (1001) docker     (127)      329 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/css/vendor/Jcrop.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)     3280 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/css/vendor/jquery.Jcrop.css
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.192081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.192081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/demo/demo.js
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/index.js
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-exif-map.js
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-exif.js
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-fetch.js
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-meta.js
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-orientation.js
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-scale.js
--rw-r--r--   0 runner    (1001) docker     (127)    17766 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image.all.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    21215 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image.all.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.192081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/vendor/
--rwxr-xr-x   0 runner    (1001) docker     (127)    42434 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/vendor/jquery.Jcrop.js
--rw-r--r--   0 runner    (1001) docker     (127)   284394 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/vendor/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.192081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    20717 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/test.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.196081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/canvas-to-blob.js
--rw-r--r--   0 runner    (1001) docker     (127)   158571 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/chai.js
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/mocha.css
--rw-r--r--   0 runner    (1001) docker     (127)   421025 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/mocha.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.196081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11622 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.196081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/css/demo.css
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.196081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2718 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/compile.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.196081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/demo/demo.js
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/runtime.js
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/tmpl.js
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/tmpl.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/tmpl.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.196081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/test/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/test/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/test/test.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.200080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)   158571 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/chai.js
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/mocha.css
--rw-r--r--   0 runner    (1001) docker     (127)   421025 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/mocha.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.200080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/dropzone/
--rw-r--r--   0 runner    (1001) docker     (127)    64399 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/dropzone/dropzone.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.204080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/bower.json
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/component.json
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/composer.json
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars-source.gemspec
--rw-r--r--   0 runner    (1001) docker     (127)   566752 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.amd.js
--rw-r--r--   0 runner    (1001) docker     (127)    73497 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.amd.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   159587 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.js
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.js.nuspec
--rw-r--r--   0 runner    (1001) docker     (127)    72614 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    98277 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.amd.js
--rw-r--r--   0 runner    (1001) docker     (127)    14091 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.amd.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    34239 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.js
--rw-r--r--   0 runner    (1001) docker     (127)    14050 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.204080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/MIT-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.216081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/dist/
--rw-r--r--   0 runner    (1001) docker     (127)   247597 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/dist/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)    84380 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/dist/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   127576 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/dist/jquery.min.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.220080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.224080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax/
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax/jsonp.js
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax/load.js
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax/parseJSON.js
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax/parseXML.js
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax/script.js
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax/xhr.js
--rw-r--r--   0 runner    (1001) docker     (127)    21168 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.224080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/attributes/
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/attributes/attr.js
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/attributes/classes.js
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/attributes/prop.js
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/attributes/support.js
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/attributes/val.js
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/attributes.js
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/callbacks.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.224080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/core/access.js
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/core/init.js
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/core/parseHTML.js
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/core/ready.js
--rw-r--r--   0 runner    (1001) docker     (127)    11790 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/core.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.224080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css/addGetHookIf.js
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css/curCSS.js
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css/defaultDisplay.js
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css/hiddenVisibleSelectors.js
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css/support.js
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css/swap.js
--rw-r--r--   0 runner    (1001) docker     (127)    12346 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.228081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/data/Data.js
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/data/accepts.js
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/data.js
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/deferred.js
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/deprecated.js
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/dimensions.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.228081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/effects/
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/effects/Tween.js
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/effects/animatedSelector.js
--rw-r--r--   0 runner    (1001) docker     (127)    16914 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/effects.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.228081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/event/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/event/ajax.js
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/event/alias.js
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/event/support.js
--rw-r--r--   0 runner    (1001) docker     (127)    24475 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/event.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.228081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/exports/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/exports/amd.js
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/exports/global.js
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/intro.js
--rw-r--r--   0 runner    (1001) docker     (127)      574 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.228081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/manipulation/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/manipulation/_evalUrl.js
--rw-r--r--   0 runner    (1001) docker     (127)      975 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/manipulation/support.js
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/manipulation.js
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/offset.js
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/outro.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.228081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/queue/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/queue/delay.js
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/queue.js
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/selector-native.js
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/selector-sizzle.js
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/selector.js
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/serialize.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.136080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/sizzle/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.228081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/
--rw-r--r--   0 runner    (1001) docker     (127)    59443 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/sizzle.js
--rw-r--r--   0 runner    (1001) docker     (127)    18626 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/sizzle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    29161 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/sizzle.min.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.228081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/traversing/
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/traversing/findFilter.js
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/traversing.js
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/wrap.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.208081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/Gemfile
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/Gemfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/Guardfile
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/README.mkd
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/TODO
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/bower.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      328 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/build.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/config.rb
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/config.ru
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/package.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      104 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/push-tag.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/release.sh
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/sortable.jquery.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.212081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_limited_drop_targets.html.haml
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_nested_bootstrap.html.haml
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_nested_with_switch.html.haml
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_serialization.html.haml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_simple_with_animation.html.haml
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_simple_with_no_drop.html.haml
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_table.html.haml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.212081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/css/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/css/_base.sass
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/css/application.css.sass
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/css/bootstrap-switch.css
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/css/coderay.css
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/css/example.css
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/css/jquery-sortable.css.sass
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/css/vendor.css
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/debug.html.erb
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/example.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.212081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/img/glyphicons-halflings-white.png
--rw-r--r--   0 runner    (1001) docker     (127)    13826 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/img/glyphicons-halflings.png
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/index.html.haml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.212081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/application.js
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/debug.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.216081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/basic.js
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/limited_drop_targets.js
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/nested_bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/nested_with_switch.js
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/serialization.js
--rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/simple_with_animation.js
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/simple_with_no_drop.js
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/table.js
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/jquery-sortable-min.js
--rw-r--r--   0 runner    (1001) docker     (127)    23872 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/jquery-sortable.js
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/test.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.216081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-button.js
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-dropdown.js
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-scrollspy.js
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-switch.js
--rw-r--r--   0 runner    (1001) docker     (127)    15347 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/jquery.color.js
--rw-r--r--   0 runner    (1001) docker     (127)    84245 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.216081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/layouts/debug.haml
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/layouts/layout.haml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/test.html.haml
--rwxr-xr-x   0 runner    (1001) docker     (127)      318 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/update-pages.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.228081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.232081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    36668 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.232081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/API.md
--rw-r--r--   0 runner    (1001) docker     (127)     9164 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/CUSTOM-EVENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19490 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/OPTIONS.md
--rw-r--r--   0 runner    (1001) docker     (127)    32677 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      914 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.140080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.236081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/medium-editor.css
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/medium-editor.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.240080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/beagle.css
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/beagle.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/default.css
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/default.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/flat.css
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/flat.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/mani.css
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/mani.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/roman.css
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/roman.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/tim.css
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/tim.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.240080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/js/
--rw-r--r--   0 runner    (1001) docker     (127)   283535 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/js/medium-editor.js
--rw-r--r--   0 runner    (1001) docker     (127)    94969 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/js/medium-editor.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.232081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.136080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.232081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin-frontend.css
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin-frontend.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin.css
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.236081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/js/
--rw-r--r--   0 runner    (1001) docker     (127)    71452 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/js/medium-editor-insert-plugin.js
--rw-r--r--   0 runner    (1001) docker     (127)    34764 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/js/medium-editor-insert-plugin.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.136080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.236081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/
--rw-r--r--   0 runner    (1001) docker     (127)    17682 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/core.js
--rw-r--r--   0 runner    (1001) docker     (127)    21015 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/embeds.js
--rw-r--r--   0 runner    (1001) docker     (127)    21380 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/images.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.236081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/core-buttons.hbs
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/core-caption.hbs
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/core-empty-line.hbs
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/embeds-toolbar.hbs
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/embeds-wrapper.hbs
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/images-fileupload.hbs
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/images-image.hbs
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/images-progressbar.hbs
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/images-toolbar.hbs
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.236081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/_core.scss
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/_embeds.scss
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/_images.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/medium-editor-insert-plugin-frontend.scss
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/medium-editor-insert-plugin.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.244081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/
--rw-r--r--   0 runner    (1001) docker     (127)      941 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/Authors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/bower.json
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/composer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.244081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/
--rw-r--r--   0 runner    (1001) docker     (127)    44683 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/picturefill.js
--rw-r--r--   0 runner    (1001) docker     (127)    11807 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/picturefill.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.140080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.244081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/intrinsic-dimension/
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/intrinsic-dimension/pf.intrinsic.js
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/intrinsic-dimension/pf.intrinsic.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.244081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/mutation/
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/mutation/pf.mutation.js
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/mutation/pf.mutation.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.244081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/oldie/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/oldie/pf.oldie.js
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/oldie/pf.oldie.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.244081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/print/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/print/pf.print.js
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/print/pf.print.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.244081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/typesupport/
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/typesupport/pf.type.js
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/typesupport/pf.type.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/gruntfile.js
--rw-r--r--   0 runner    (1001) docker     (127)    27976 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.248081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/logos/
--rw-r--r--   0 runner    (1001) docker     (127)    31957 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/logos/bocoup-lg.png
--rw-r--r--   0 runner    (1001) docker     (127)    31223 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/logos/bocoup-sm.png
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/logos/fg-lg.png
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/logos/fg-sm.png
--rw-r--r--   0 runner    (1001) docker     (127)    57789 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/logos/ricg-seal.png
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.248081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/
--rw-r--r--   0 runner    (1001) docker     (127)    42604 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/picturefill.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.140080 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.248081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/gecko-picture/
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/gecko-picture/pf.gecko-picture.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.248081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/intrinsic-dimension/
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/intrinsic-dimension/pf.intrinsic.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.248081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/mutation/
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/mutation/pf.mutation.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.248081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/oldie/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/oldie/pf.oldie.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.248081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/print/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/print/pf.print.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.248081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/typesupport/
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/typesupport/pf.type.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.252081 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/bower.json
--rw-r--r--   0 runner    (1001) docker     (127)    47159 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-classapplier.js
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-classapplier.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   161307 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-core.js
--rw-r--r--   0 runner    (1001) docker     (127)    47642 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-core.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    26513 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-highlighter.js
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-highlighter.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-selectionsaverestore.js
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-selectionsaverestore.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    12701 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-serializer.js
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-serializer.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    81960 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-textrange.js
--rw-r--r--   0 runner    (1001) docker     (127)    21370 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-textrange.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.252081 django_xprez-0.2.8/xprez/static/xprez/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.252081 django_xprez-0.2.8/xprez/static/xprez/fonts/backup/
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/backup/xprez.eot
--rw-r--r--   0 runner    (1001) docker     (127)    15289 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/backup/xprez.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/backup/xprez.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/backup/xprez.woff
--rw-r--r--   0 runner    (1001) docker     (127)    26407 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/selection.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.252081 django_xprez-0.2.8/xprez/static/xprez/fonts/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.260081 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/add_circle.svg
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/align-center.svg
--rw-r--r--   0 runner    (1001) docker     (127)      217 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/arrow_down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/arrow_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/art_track.svg
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/attach_file.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/background.svg
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/border.svg
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/cancel.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/chevron-small-down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/chevron-small-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)      441 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/cloud_download.svg
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/code.svg
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/code_template.svg
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/control_point.svg
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/copy.svg
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/crop.svg
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/delete.svg
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/done.svg
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/eye.svg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/feature_boxes.svg
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/gallery.svg
--rw-r--r--   0 runner    (1001) docker     (127)      820 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/grid-boxes.svg
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/layout_1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/layout_2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/layout_3.svg
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/layout_4.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/layout_6.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/layout_8.svg
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/layout_stream.svg
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/linked_article.svg
--rw-r--r--   0 runner    (1001) docker     (127)      544 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/numbers.svg
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/play_arrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/play_circle_filled.svg
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/play_circle_outline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/quote.svg
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/text_box.svg
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/text_content.svg
--rw-r--r--   0 runner    (1001) docker     (127)      548 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/video.svg
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/videocam.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25740 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/src/selection.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     7144 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/xprez.eot
--rwxr-xr-x   0 runner    (1001) docker     (127)    15763 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/xprez.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6988 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/xprez.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)     7064 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/fonts/xprez.woff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.260081 django_xprez-0.2.8/xprez/static/xprez/img/
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/img/avatar.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.264081 django_xprez-0.2.8/xprez/static/xprez/js/
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/js/modernizr-detection.js
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/js/numbers.js
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/js/photoswipe.js
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/js/video.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.264081 django_xprez-0.2.8/xprez/static/xprez/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.264081 django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)    18026 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/bower.json
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/counterup.jquery.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.264081 django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/demo/demo.html
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/jquery.counterup.js
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/jquery.counterup.min.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     9028 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/jquery.waypoints.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.264081 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/.bower.json
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/Gruntfile.js
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/bower.json
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/component.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.268081 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.268081 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/default-skin/
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/default-skin/default-skin.css
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/default-skin/default-skin.png
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/default-skin/default-skin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/default-skin/preloader.gif
--rw-r--r--   0 runner    (1001) docker     (127)    21504 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/photoswipe-ui-default.js
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/photoswipe-ui-default.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/photoswipe.css
--rw-r--r--   0 runner    (1001) docker     (127)    93517 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/photoswipe.js
--rw-r--r--   0 runner    (1001) docker     (127)    31726 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/photoswipe.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/photoswipe.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.144080 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.268081 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/_main-settings.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.268081 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.268081 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin-svg.sketch/
--rw-r--r--   0 runner    (1001) docker     (127)    57208 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin-svg.sketch/Data
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin-svg.sketch/metadata
--rw-r--r--   0 runner    (1001) docker     (127)        2 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin-svg.sketch/version
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.png
--rw-r--r--   0 runner    (1001) docker     (127)    73357 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.psd
--rw-r--r--   0 runner    (1001) docker     (127)     9773 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/preloader.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/main.css
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.272081 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/
--rw-r--r--   0 runner    (1001) docker     (127)    25570 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/core.js
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/desktop-zoom.js
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/framework-bridge.js
--rw-r--r--   0 runner    (1001) docker     (127)    30716 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/gestures.js
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/history.js
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/items-controller.js
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/show-hide-transition.js
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/tap.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.272081 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/ui/
--rw-r--r--   0 runner    (1001) docker     (127)    21393 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/ui/photoswipe-ui-default.js
--rw-r--r--   0 runner    (1001) docker     (127)    11807 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/libs/picturefill.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   143998 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.272081 django_xprez-0.2.8/xprez/static/xprez/styles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.272081 django_xprez-0.2.8/xprez/static/xprez/styles/scss/
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/_config.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.276081 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_add-module.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_admin-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_ck-editor.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_form-elements.scss
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_grid-boxes.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_image-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_medium-editor.scss
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_messaging.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_photo-gallery.scss
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_text-content.scss
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/xprez-backend.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.276081 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_boxed-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_button.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_download.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_editor_media.scss
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_faq.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_feature-boxes.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_grid-boxes.scss
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_module-relations.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_numbers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_photo-gallery.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_quote.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_text-image.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_video.scss
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/xprez-frontend.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.280081 django_xprez-0.2.8/xprez/static/xprez/styles/scss/library/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/library/_lib-prefixer.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/library/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/scss/library/_rfs.scss
--rw-r--r--   0 runner    (1001) docker     (127)    32579 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/xprez-backend.css
--rw-r--r--   0 runner    (1001) docker     (127)     8693 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/xprez-backend.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    31558 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/xprez-frontend.css
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/static/xprez/styles/xprez-frontend.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.144080 django_xprez-0.2.8/xprez/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.280081 django_xprez-0.2.8/xprez/templates/xprez/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.280081 django_xprez-0.2.8/xprez/templates/xprez/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.280081 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/ck_editor.html
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/code_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/code_template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.280081 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/download/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/download/attachment.html
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/download/download.html
--rw-r--r--   0 runner    (1001) docker     (127)      842 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/feature_boxes.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.280081 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/gallery/
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/gallery/gallery.html
--rw-r--r--   0 runner    (1001) docker     (127)      859 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/gallery/photo.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.280081 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/grid_boxes/
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/grid_boxes/box.html
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/grid_boxes/grid_boxes.html
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/medium_editor.html
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/numbers.html
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/quote.html
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/text_image.html
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/contents/video.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.284081 django_xprez-0.2.8/xprez/templates/xprez/admin/form/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/form/field_errors.html
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/form/multi_row.html
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/form/row.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.284081 django_xprez-0.2.8/xprez/templates/xprez/admin/includes/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/includes/add_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      736 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/xprez.html
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/admin/xprez_changeform.html
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/container.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.284081 django_xprez-0.2.8/xprez/templates/xprez/contents/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/contents/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      502 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/contents/ck_editor.html
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/contents/code_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/contents/download.html
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/contents/feature_boxes.html
--rw-r--r--   0 runner    (1001) docker     (127)    13245 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/contents/gallery.html
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/contents/grid_boxes.html
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/contents/medium_editor.html
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/contents/numbers.html
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/contents/quote.html
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/contents/text_image.html
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/contents/video.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.284081 django_xprez-0.2.8/xprez/templates/xprez/includes/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/includes/ckeditor_image.html
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/includes/editor_image.html
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/includes/medium_image.html
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/includes/photoswipe.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.284081 django_xprez-0.2.8/xprez/templates/xprez/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templates/xprez/widgets/ck_editor.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 11:16:26.284081 django_xprez-0.2.8/xprez/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/templatetags/xprez.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2023-12-21 11:16:17.000000 django_xprez-0.2.8/xprez/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.669188 django_xprez-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-22 15:47:58.000000 django_xprez-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-22 15:47:58.000000 django_xprez-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2023-12-22 15:48:06.669188 django_xprez-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2023-12-22 15:47:58.000000 django_xprez-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.669188 django_xprez-0.2.9/django_xprez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2023-12-22 15:48:06.000000 django_xprez-0.2.9/django_xprez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39409 2023-12-22 15:48:06.000000 django_xprez-0.2.9/django_xprez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 15:48:06.000000 django_xprez-0.2.9/django_xprez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-22 15:48:06.000000 django_xprez-0.2.9/django_xprez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-22 15:48:06.000000 django_xprez-0.2.9/django_xprez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 15:48:06.669188 django_xprez-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-12-22 15:47:58.000000 django_xprez-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.533188 django_xprez-0.2.9/xprez/
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8387 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/admin_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.533188 django_xprez-0.2.9/xprez/ck_editor/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/parse_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.509188 django_xprez-0.2.9/xprez/ck_editor/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.513188 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.533188 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/js/ck_editor_widget.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.513188 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.533188 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/
+-rw-r--r--   0 runner    (1001) docker     (127)   899705 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/ckeditor.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4801287 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/ckeditor.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.553188 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/af.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ast.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/az.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/bg.js
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/cs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/da.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/de-ch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/de.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/el.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/en-au.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/en-gb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/eo.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/es.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/et.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/eu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/fa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/fi.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/fr.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/gl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/gu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/he.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/hi.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/hr.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/hu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/id.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/it.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ja.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/km.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/kn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ko.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ku.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/lt.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/lv.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/nb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ne.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/nl.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/no.js
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/oc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/pl.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/pt-br.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/pt.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ro.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ru.js
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/si.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sl.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sq.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sr-latn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sr.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sv.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/th.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/tk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/tr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/tt.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ug.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/uk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/vi.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/zh-cn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/zh.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/ck_editor/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.553188 django_xprez-0.2.9/xprez/code_snippet/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/code_snippet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/code_snippet/admin_forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.553188 django_xprez-0.2.9/xprez/code_snippet/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/code_snippet/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/code_snippet/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/code_snippet/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.513188 django_xprez-0.2.9/xprez/code_snippet/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.513188 django_xprez-0.2.9/xprez/code_snippet/static/xprez/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.513188 django_xprez-0.2.9/xprez/code_snippet/static/xprez/css/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.553188 django_xprez-0.2.9/xprez/code_snippet/static/xprez/css/pygments/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/code_snippet/static/xprez/css/pygments/colorful.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.553188 django_xprez-0.2.9/xprez/code_snippet/static/xprez/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/code_snippet/static/xprez/js/textarea_with_tabs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.513188 django_xprez-0.2.9/xprez/code_snippet/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.553188 django_xprez-0.2.9/xprez/code_snippet/templates/xprez/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.553188 django_xprez-0.2.9/xprez/code_snippet/templates/xprez/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/code_snippet/templates/xprez/admin/code_snippet.html
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/code_snippet/templates/xprez/code_snippet.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.557188 django_xprez-0.2.9/xprez/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/conf/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.557188 django_xprez-0.2.9/xprez/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.557188 django_xprez-0.2.9/xprez/contrib/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/contrib/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/contrib/rest_framework/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.557188 django_xprez-0.2.9/xprez/contrib/sorl_thumbnail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/contrib/sorl_thumbnail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/contrib/sorl_thumbnail/thumbnail_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/form_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.557188 django_xprez-0.2.9/xprez/medium_editor/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/medium_editor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.513188 django_xprez-0.2.9/xprez/medium_editor/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.513188 django_xprez-0.2.9/xprez/medium_editor/static/medium_editor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.557188 django_xprez-0.2.9/xprez/medium_editor/static/medium_editor/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/medium_editor/static/medium_editor/css/medium_editor_widget.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.557188 django_xprez-0.2.9/xprez/medium_editor/static/medium_editor/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/medium_editor/static/medium_editor/js/medium_editor_widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/medium_editor/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/medium_editor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/medium_editor/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/medium_editor/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.561188 django_xprez-0.2.9/xprez/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0002_auto_20180115_1306.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0003_auto_20180117_0930.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0004_auto_20180504_1516.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0005_auto_20191025_1352.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0006_contentscontainer_content_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0006_gridboxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0007_auto_20191221_1522.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0007_auto_20191227_2150.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0008_merge_20200129_1159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0009_gridboxes_width.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0010_auto_20220204_1540.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0010_ckeditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0011_auto_20220204_1559.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0012_auto_20220204_1600.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0013_merge_20220207_1020.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0014_remove_content_margin_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0015_ckeditor_content_centered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0016_auto_20220208_1355.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0017_auto_20220208_1401.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0018_auto_20220312_1845.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0019_photo_alt_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0020_alter_gridboxes_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0021_alter_ckeditor_options_alter_downloadcontent_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0022_content_alternate_color_content_background_color_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/0023_remove_content_padding_vertical_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.561188 django_xprez-0.2.9/xprez/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17310 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/models/contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/models/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.513188 django_xprez-0.2.9/xprez/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.565188 django_xprez-0.2.9/xprez/static/xprez/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.513188 django_xprez-0.2.9/xprez/static/xprez/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.565188 django_xprez-0.2.9/xprez/static/xprez/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/js/ajax_upload_formset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/js/contents.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/js/grid_boxes.js
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/js/jquery_revert_noconflict.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.525188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.565188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.565188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/canvas-to-blob.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/canvas-to-blob.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/canvas-to-blob.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.565188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/test.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.569188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)   158571 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/chai.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/load-image.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/mocha.css
+-rw-r--r--   0 runner    (1001) docker     (127)   421025 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/mocha.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.569188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.569188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/css/jquery.fileupload-noscript.css
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/css/jquery.fileupload-ui-noscript.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/css/jquery.fileupload-ui.css
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/css/jquery.fileupload.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.569188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/img/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/img/progressbar.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.573188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.573188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/cors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/cors/jquery.postmessage-transport.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/cors/jquery.xdr-transport.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16607 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-angular.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-audio.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-image.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5171 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-process.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27848 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-validate.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-video.js
+-rw-r--r--   0 runner    (1001) docker     (127)    63666 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10723 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.iframe-transport.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.573188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)    16089 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/vendor/jquery.ui.widget.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.573188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11510 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.573188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/css/demo.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.573188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/css/vendor/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      329 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/css/vendor/Jcrop.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3280 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/css/vendor/jquery.Jcrop.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.577188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.577188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/demo/demo.js
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-exif-map.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-exif.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-fetch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-meta.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-orientation.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-scale.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17766 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image.all.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21215 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image.all.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.577188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/vendor/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42434 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/vendor/jquery.Jcrop.js
+-rw-r--r--   0 runner    (1001) docker     (127)   284394 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/vendor/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.577188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20717 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/test.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.577188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/canvas-to-blob.js
+-rw-r--r--   0 runner    (1001) docker     (127)   158571 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/chai.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/mocha.css
+-rw-r--r--   0 runner    (1001) docker     (127)   421025 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/mocha.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.581188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11622 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.581188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/css/demo.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.581188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2718 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/compile.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.581188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/demo/demo.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/runtime.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/tmpl.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/tmpl.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/tmpl.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.581188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/test/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/test/test.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.581188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)   158571 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/chai.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/mocha.css
+-rw-r--r--   0 runner    (1001) docker     (127)   421025 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/mocha.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.585188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/dropzone/
+-rw-r--r--   0 runner    (1001) docker     (127)    64399 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/dropzone/dropzone.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.589188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/component.json
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/composer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars-source.gemspec
+-rw-r--r--   0 runner    (1001) docker     (127)   566752 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.amd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    73497 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.amd.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   159587 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.js
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.js.nuspec
+-rw-r--r--   0 runner    (1001) docker     (127)    72614 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    98277 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.amd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14091 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.amd.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34239 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14050 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.589188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/MIT-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.601188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)   247597 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/dist/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)    84380 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/dist/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   127576 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/dist/jquery.min.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.605188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.605188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax/
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax/jsonp.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax/load.js
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax/parseJSON.js
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax/parseXML.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax/script.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax/xhr.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21168 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.609188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/attributes/attr.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/attributes/classes.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/attributes/prop.js
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/attributes/support.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/attributes/val.js
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/attributes.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/callbacks.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.609188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/core/access.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/core/init.js
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/core/parseHTML.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/core/ready.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11790 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/core.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.609188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css/addGetHookIf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css/curCSS.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css/defaultDisplay.js
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css/hiddenVisibleSelectors.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css/support.js
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css/swap.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12346 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.609188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/data/Data.js
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/data/accepts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/data.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/deferred.js
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/deprecated.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/dimensions.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.609188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/effects/
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/effects/Tween.js
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/effects/animatedSelector.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16914 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/effects.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.609188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/event/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/event/ajax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/event/alias.js
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/event/support.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24475 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/event.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.613188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/exports/amd.js
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/exports/global.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/intro.js
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.613188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/manipulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/manipulation/_evalUrl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/manipulation/support.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/manipulation.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/offset.js
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/outro.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.613188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/queue/delay.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/queue.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/selector-native.js
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/selector-sizzle.js
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/selector.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/serialize.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.521188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/sizzle/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.613188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)    59443 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/sizzle.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18626 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/sizzle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29161 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/sizzle.min.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.613188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/traversing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/traversing/findFilter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/traversing.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/wrap.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.593188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/Gemfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/Gemfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/Guardfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/README.mkd
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/TODO
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/bower.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      328 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/config.rb
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/config.ru
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/package.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      104 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/push-tag.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/release.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/sortable.jquery.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.593188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_limited_drop_targets.html.haml
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_nested_bootstrap.html.haml
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_nested_with_switch.html.haml
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_serialization.html.haml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_simple_with_animation.html.haml
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_simple_with_no_drop.html.haml
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_table.html.haml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.597188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/css/_base.sass
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/css/application.css.sass
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/css/bootstrap-switch.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/css/coderay.css
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/css/example.css
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/css/jquery-sortable.css.sass
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/css/vendor.css
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/debug.html.erb
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/example.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.597188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/img/glyphicons-halflings-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13826 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/img/glyphicons-halflings.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/index.html.haml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.597188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/application.js
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/debug.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.597188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/basic.js
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/limited_drop_targets.js
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/nested_bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/nested_with_switch.js
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/serialization.js
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/simple_with_animation.js
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/simple_with_no_drop.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/table.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/jquery-sortable-min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    23872 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/jquery-sortable.js
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/test.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.601188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-button.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-dropdown.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-scrollspy.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-switch.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15347 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/jquery.color.js
+-rw-r--r--   0 runner    (1001) docker     (127)    84245 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.601188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/layouts/debug.haml
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/layouts/layout.haml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/test.html.haml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      318 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/update-pages.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.613188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.613188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    36668 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.617188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/API.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9164 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/CUSTOM-EVENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19490 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/OPTIONS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32677 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.521188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.621188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/medium-editor.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/medium-editor.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.625188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/beagle.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/beagle.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/default.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/default.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/flat.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/flat.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/mani.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/mani.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/roman.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/roman.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/tim.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/tim.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.625188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   283535 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/js/medium-editor.js
+-rw-r--r--   0 runner    (1001) docker     (127)    94969 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/js/medium-editor.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.617188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.521188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.617188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin-frontend.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin-frontend.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.617188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    71452 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/js/medium-editor-insert-plugin.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34764 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/js/medium-editor-insert-plugin.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.521188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.617188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    17682 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/core.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21015 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/embeds.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21380 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/images.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.621188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/core-buttons.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/core-caption.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/core-empty-line.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/embeds-toolbar.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/embeds-wrapper.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/images-fileupload.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/images-image.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/images-progressbar.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/images-toolbar.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.621188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/_core.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/_embeds.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/_images.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/medium-editor-insert-plugin-frontend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/medium-editor-insert-plugin.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.629188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/Authors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/composer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.629188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)    44683 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/picturefill.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11807 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/picturefill.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.521188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.629188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/intrinsic-dimension/
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/intrinsic-dimension/pf.intrinsic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/intrinsic-dimension/pf.intrinsic.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.629188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/mutation/
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/mutation/pf.mutation.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/mutation/pf.mutation.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.629188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/oldie/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/oldie/pf.oldie.js
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/oldie/pf.oldie.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.629188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/print/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/print/pf.print.js
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/print/pf.print.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.629188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/typesupport/
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/typesupport/pf.type.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/typesupport/pf.type.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/gruntfile.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27976 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.629188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    31957 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/logos/bocoup-lg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31223 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/logos/bocoup-sm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/logos/fg-lg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/logos/fg-sm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57789 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/logos/ricg-seal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.629188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    42604 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/picturefill.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.525188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.633188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/gecko-picture/
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/gecko-picture/pf.gecko-picture.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.633188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/intrinsic-dimension/
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/intrinsic-dimension/pf.intrinsic.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.633188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/mutation/
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/mutation/pf.mutation.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.633188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/oldie/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/oldie/pf.oldie.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.633188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/print/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/print/pf.print.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.633188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/typesupport/
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/typesupport/pf.type.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.637188 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47159 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-classapplier.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-classapplier.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   161307 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-core.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47642 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-core.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    26513 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-highlighter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-highlighter.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-selectionsaverestore.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-selectionsaverestore.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12701 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-serializer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-serializer.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    81960 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-textrange.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21370 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-textrange.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.637188 django_xprez-0.2.9/xprez/static/xprez/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.637188 django_xprez-0.2.9/xprez/static/xprez/fonts/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/backup/xprez.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/backup/xprez.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/backup/xprez.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/backup/xprez.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    26407 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/selection.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.637188 django_xprez-0.2.9/xprez/static/xprez/fonts/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.645188 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/add_circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/align-center.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/arrow_down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/arrow_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/art_track.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/attach_file.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/background.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/border.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/cancel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/chevron-small-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/chevron-small-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/cloud_download.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/code.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/code_template.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/control_point.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/crop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/done.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/eye.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/feature_boxes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/gallery.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/grid-boxes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/layout_1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/layout_2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/layout_3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/layout_4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/layout_6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/layout_8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/layout_stream.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/linked_article.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/numbers.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/play_arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/play_circle_filled.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/play_circle_outline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/quote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/text_box.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/text_content.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/video.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/videocam.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25740 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/src/selection.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7144 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/xprez.eot
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15763 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/xprez.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6988 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/xprez.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7064 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/fonts/xprez.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.645188 django_xprez-0.2.9/xprez/static/xprez/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/img/avatar.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.645188 django_xprez-0.2.9/xprez/static/xprez/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/js/modernizr-detection.js
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/js/numbers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/js/photoswipe.js
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/js/video.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.645188 django_xprez-0.2.9/xprez/static/xprez/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.649188 django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18026 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/counterup.jquery.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.649188 django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/demo/demo.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/jquery.counterup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/jquery.counterup.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9028 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/jquery.waypoints.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.649188 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/Gruntfile.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/component.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.649188 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.649188 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/default-skin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/default-skin/default-skin.css
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/default-skin/default-skin.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/default-skin/default-skin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/default-skin/preloader.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    21504 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/photoswipe-ui-default.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/photoswipe-ui-default.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/photoswipe.css
+-rw-r--r--   0 runner    (1001) docker     (127)    93517 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/photoswipe.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31726 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/photoswipe.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/photoswipe.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.525188 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.653188 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/_main-settings.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.653188 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.653188 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin-svg.sketch/
+-rw-r--r--   0 runner    (1001) docker     (127)    57208 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin-svg.sketch/Data
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin-svg.sketch/metadata
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin-svg.sketch/version
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73357 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.psd
+-rw-r--r--   0 runner    (1001) docker     (127)     9773 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/preloader.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/main.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.653188 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    25570 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/core.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/desktop-zoom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/framework-bridge.js
+-rw-r--r--   0 runner    (1001) docker     (127)    30716 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/gestures.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/history.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/items-controller.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/show-hide-transition.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/tap.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.653188 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    21393 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/ui/photoswipe-ui-default.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11807 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/libs/picturefill.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   143998 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.657188 django_xprez-0.2.9/xprez/static/xprez/styles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.657188 django_xprez-0.2.9/xprez/static/xprez/styles/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/_config.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.657188 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_add-module.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_admin-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_ck-editor.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_form-elements.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_grid-boxes.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_image-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_medium-editor.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_messaging.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_photo-gallery.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_text-content.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/xprez-backend.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.661188 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_boxed-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_button.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_download.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_editor_media.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_faq.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_feature-boxes.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_grid-boxes.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_module-relations.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_numbers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_photo-gallery.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_quote.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_text-image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_video.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/xprez-frontend.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.661188 django_xprez-0.2.9/xprez/static/xprez/styles/scss/library/
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/library/_lib-prefixer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/library/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/scss/library/_rfs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    32579 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/xprez-backend.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8693 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/xprez-backend.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    31558 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/xprez-frontend.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/static/xprez/styles/xprez-frontend.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.529188 django_xprez-0.2.9/xprez/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.661188 django_xprez-0.2.9/xprez/templates/xprez/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.661188 django_xprez-0.2.9/xprez/templates/xprez/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.665188 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/ck_editor.html
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/code_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/code_template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.665188 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/download/attachment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/download/download.html
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/feature_boxes.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.665188 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/gallery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/gallery/gallery.html
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/gallery/photo.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.665188 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/grid_boxes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/grid_boxes/box.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/grid_boxes/grid_boxes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/medium_editor.html
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/numbers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/quote.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/text_image.html
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/contents/video.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.665188 django_xprez-0.2.9/xprez/templates/xprez/admin/form/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/form/field_errors.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/form/multi_row.html
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/form/row.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.665188 django_xprez-0.2.9/xprez/templates/xprez/admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/includes/add_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/xprez.html
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/admin/xprez_changeform.html
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/container.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.669188 django_xprez-0.2.9/xprez/templates/xprez/contents/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/contents/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/contents/ck_editor.html
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/contents/code_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/contents/download.html
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/contents/feature_boxes.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13250 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/contents/gallery.html
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/contents/grid_boxes.html
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/contents/medium_editor.html
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/contents/numbers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/contents/quote.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/contents/text_image.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/contents/video.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.669188 django_xprez-0.2.9/xprez/templates/xprez/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/includes/ckeditor_image.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/includes/editor_image.html
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/includes/medium_image.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/includes/photoswipe.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.669188 django_xprez-0.2.9/xprez/templates/xprez/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templates/xprez/widgets/ck_editor.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 15:48:06.669188 django_xprez-0.2.9/xprez/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/templatetags/xprez.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2023-12-22 15:47:58.000000 django_xprez-0.2.9/xprez/utils.py
```

### Comparing `django_xprez-0.2.8/PKG-INFO` & `django_xprez-0.2.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_xprez
-Version: 0.2.8
+Version: 0.2.9
 Summary: Django CMS for presentation websites
 Home-page: https://github.com/s-cape/django_xprez
 Author: Michal Májský, Martin Kappel, Jakub Dolejšek, Michal Tilsch - s-cape.cz & mimatik.com
 Author-email: michal.majsky@s-cape.cz
 License: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -130,15 +130,15 @@
 To rebuild css styles
 
     cd xprez/static/xprez
     npm install
     npm run build (or `watch` for developing)
 
 
-Deploying new version (old)
+Deploying new version
 ----------------
 
 #### Tagging new version
 
 Update setup.py -> VERSION, commit and push to master.
 
 On localhost run:
@@ -158,64 +158,14 @@
 ```
 
 #### Deploying new version to pypi
 
 Go to https://github.com/s-cape/django_xprez/actions/workflows/pypi.yml and run workflow.
 
 
-
-Deploying new version (archive)
-----------------
-
-#### Tagging new version
-
-Update setup.py -> VERSION, commit and push to master.
-
-On localhost run:
-```
-    git tag vX.Y.Z
-    git push origin vX.Y.Z
-```
-
-#### Draft release on github
-
-Go to: `https://github.com/s-cape/django_xprez/releases` -> `Draft new release`
-Select tag `vX.Y.Z` and name `vX.Y.Z`
-
-
-#### requirements
-
-    python -m pip install --user --upgrade setuptools wheel twine
-
-
-#### cleanup old builds (if exists)
-
-    rm -rf ./dist ./build
-
-#### create dist package
-
-    python setup.py sdist bdist_wheel
-
-#### to check package add this to requirements.txt
-
-    file:/<path_to_package>/dist/django_xprez-<version>.tar.gz
-
-#### upload to testpypi
-
-    python -m twine upload --repository testpypi dist/*
-
-#### to check package from testpypi add (temporary) this to top of requirements.txt:
-
-    --extra-index-url https://test.pypi.org/simple/
-
-#### upload to pypi
-
-    python -m twine upload dist/*
-
-
 TODO
 -------
 
 - add custom module tutorial to Readme
 - fix template content to save only relative path to database
 - check template content raising UnicodeDecodeError
 - create manual for various situations (ck_editor branch)
```

### Comparing `django_xprez-0.2.8/README.md` & `django_xprez-0.2.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 To rebuild css styles
 
     cd xprez/static/xprez
     npm install
     npm run build (or `watch` for developing)
 
 
-Deploying new version (old)
+Deploying new version
 ----------------
 
 #### Tagging new version
 
 Update setup.py -> VERSION, commit and push to master.
 
 On localhost run:
@@ -135,64 +135,14 @@
 ```
 
 #### Deploying new version to pypi
 
 Go to https://github.com/s-cape/django_xprez/actions/workflows/pypi.yml and run workflow.
 
 
-
-Deploying new version (archive)
-----------------
-
-#### Tagging new version
-
-Update setup.py -> VERSION, commit and push to master.
-
-On localhost run:
-```
-    git tag vX.Y.Z
-    git push origin vX.Y.Z
-```
-
-#### Draft release on github
-
-Go to: `https://github.com/s-cape/django_xprez/releases` -> `Draft new release`
-Select tag `vX.Y.Z` and name `vX.Y.Z`
-
-
-#### requirements
-
-    python -m pip install --user --upgrade setuptools wheel twine
-
-
-#### cleanup old builds (if exists)
-
-    rm -rf ./dist ./build
-
-#### create dist package
-
-    python setup.py sdist bdist_wheel
-
-#### to check package add this to requirements.txt
-
-    file:/<path_to_package>/dist/django_xprez-<version>.tar.gz
-
-#### upload to testpypi
-
-    python -m twine upload --repository testpypi dist/*
-
-#### to check package from testpypi add (temporary) this to top of requirements.txt:
-
-    --extra-index-url https://test.pypi.org/simple/
-
-#### upload to pypi
-
-    python -m twine upload dist/*
-
-
 TODO
 -------
 
 - add custom module tutorial to Readme
 - fix template content to save only relative path to database
 - check template content raising UnicodeDecodeError
 - create manual for various situations (ck_editor branch)
```

### Comparing `django_xprez-0.2.8/django_xprez.egg-info/PKG-INFO` & `django_xprez-0.2.9/django_xprez.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-xprez
-Version: 0.2.8
+Version: 0.2.9
 Summary: Django CMS for presentation websites
 Home-page: https://github.com/s-cape/django_xprez
 Author: Michal Májský, Martin Kappel, Jakub Dolejšek, Michal Tilsch - s-cape.cz & mimatik.com
 Author-email: michal.majsky@s-cape.cz
 License: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -130,15 +130,15 @@
 To rebuild css styles
 
     cd xprez/static/xprez
     npm install
     npm run build (or `watch` for developing)
 
 
-Deploying new version (old)
+Deploying new version
 ----------------
 
 #### Tagging new version
 
 Update setup.py -> VERSION, commit and push to master.
 
 On localhost run:
@@ -158,64 +158,14 @@
 ```
 
 #### Deploying new version to pypi
 
 Go to https://github.com/s-cape/django_xprez/actions/workflows/pypi.yml and run workflow.
 
 
-
-Deploying new version (archive)
-----------------
-
-#### Tagging new version
-
-Update setup.py -> VERSION, commit and push to master.
-
-On localhost run:
-```
-    git tag vX.Y.Z
-    git push origin vX.Y.Z
-```
-
-#### Draft release on github
-
-Go to: `https://github.com/s-cape/django_xprez/releases` -> `Draft new release`
-Select tag `vX.Y.Z` and name `vX.Y.Z`
-
-
-#### requirements
-
-    python -m pip install --user --upgrade setuptools wheel twine
-
-
-#### cleanup old builds (if exists)
-
-    rm -rf ./dist ./build
-
-#### create dist package
-
-    python setup.py sdist bdist_wheel
-
-#### to check package add this to requirements.txt
-
-    file:/<path_to_package>/dist/django_xprez-<version>.tar.gz
-
-#### upload to testpypi
-
-    python -m twine upload --repository testpypi dist/*
-
-#### to check package from testpypi add (temporary) this to top of requirements.txt:
-
-    --extra-index-url https://test.pypi.org/simple/
-
-#### upload to pypi
-
-    python -m twine upload dist/*
-
-
 TODO
 -------
 
 - add custom module tutorial to Readme
 - fix template content to save only relative path to database
 - check template content raising UnicodeDecodeError
 - create manual for various situations (ck_editor branch)
```

### Comparing `django_xprez-0.2.8/django_xprez.egg-info/SOURCES.txt` & `django_xprez-0.2.9/django_xprez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/setup.py` & `django_xprez-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 PACKAGE = "xprez"
 NAME = "django_xprez"
 DESCRIPTION = "Django CMS for presentation websites"
 AUTHOR = "Michal Májský, Martin Kappel, Jakub Dolejšek, Michal Tilsch - s-cape.cz & mimatik.com"
 AUTHOR_EMAIL = "michal.majsky@s-cape.cz"
 URL = "https://github.com/s-cape/django_xprez"
-VERSION = "0.2.8"
+VERSION = "0.2.9"
 LICENSE = "Mozilla Public License 2.0 (MPL 2.0)"
 
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=(Path(__file__).parent / "README.md").read_text(),
```

### Comparing `django_xprez-0.2.8/xprez/__init__.py` & `django_xprez-0.2.9/xprez/__init__.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/admin.py` & `django_xprez-0.2.9/xprez/admin.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/admin_forms.py` & `django_xprez-0.2.9/xprez/admin_forms.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/apps.py` & `django_xprez-0.2.9/xprez/apps.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/fields.py` & `django_xprez-0.2.9/xprez/ck_editor/fields.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/parse_text.py` & `django_xprez-0.2.9/xprez/ck_editor/parse_text.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/js/ck_editor_widget.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/js/ck_editor_widget.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/ckeditor.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/ckeditor.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/ckeditor.js.map` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/ckeditor.js.map`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ar.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ar.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ast.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ast.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/az.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/az.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/bg.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/bg.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ca.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ca.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/cs.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/cs.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/da.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/da.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/de-ch.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/de-ch.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/de.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/de.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/el.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/el.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/en-au.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/en-au.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/en-gb.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/en-gb.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/eo.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/eo.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/es.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/es.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/et.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/et.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/eu.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/eu.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/fa.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/fa.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/fi.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/fi.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/fr.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/fr.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/gl.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/gl.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/he.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/he.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/hi.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/hi.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/hr.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/hr.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/hu.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/hu.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/id.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/id.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/it.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/it.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ja.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ja.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/km.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/km.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/kn.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/kn.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ko.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ko.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ku.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ku.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/lt.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/lt.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/lv.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/lv.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/nb.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/nb.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ne.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ne.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/nl.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/nl.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/no.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/no.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/pl.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/pl.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/pt-br.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/pt-br.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/pt.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/pt.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ro.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ro.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ru.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ru.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/si.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/si.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sk.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sk.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sl.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sl.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sq.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sq.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sr-latn.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sr-latn.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sr.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sr.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sv.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/sv.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/th.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/th.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/tk.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/tk.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/tr.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/tr.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ug.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/ug.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/uk.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/uk.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/vi.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/vi.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/zh-cn.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/zh-cn.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/zh.js` & `django_xprez-0.2.9/xprez/ck_editor/static/ck_editor/libs/ck_editor/translations/zh.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/ck_editor/widgets.py` & `django_xprez-0.2.9/xprez/ck_editor/widgets.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/code_snippet/migrations/0001_initial.py` & `django_xprez-0.2.9/xprez/code_snippet/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/code_snippet/models.py` & `django_xprez-0.2.9/xprez/code_snippet/models.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/code_snippet/static/xprez/css/pygments/colorful.css` & `django_xprez-0.2.9/xprez/code_snippet/static/xprez/css/pygments/colorful.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/code_snippet/static/xprez/js/textarea_with_tabs.js` & `django_xprez-0.2.9/xprez/code_snippet/static/xprez/js/textarea_with_tabs.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/code_snippet/templates/xprez/admin/code_snippet.html` & `django_xprez-0.2.9/xprez/code_snippet/templates/xprez/admin/code_snippet.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/conf/defaults.py` & `django_xprez-0.2.9/xprez/conf/defaults.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/contrib/sorl_thumbnail/thumbnail_backend.py` & `django_xprez-0.2.9/xprez/contrib/sorl_thumbnail/thumbnail_backend.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/form_fields.py` & `django_xprez-0.2.9/xprez/form_fields.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/medium_editor/static/medium_editor/js/medium_editor_widget.js` & `django_xprez-0.2.9/xprez/medium_editor/static/medium_editor/js/medium_editor_widget.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/medium_editor/utils.py` & `django_xprez-0.2.9/xprez/medium_editor/utils.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/medium_editor/views.py` & `django_xprez-0.2.9/xprez/medium_editor/views.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/medium_editor/widgets.py` & `django_xprez-0.2.9/xprez/medium_editor/widgets.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0001_initial.py` & `django_xprez-0.2.9/xprez/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0002_auto_20180115_1306.py` & `django_xprez-0.2.9/xprez/migrations/0002_auto_20180115_1306.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0003_auto_20180117_0930.py` & `django_xprez-0.2.9/xprez/migrations/0003_auto_20180117_0930.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0005_auto_20191025_1352.py` & `django_xprez-0.2.9/xprez/migrations/0005_auto_20191025_1352.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0006_gridboxes.py` & `django_xprez-0.2.9/xprez/migrations/0006_gridboxes.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0007_auto_20191221_1522.py` & `django_xprez-0.2.9/xprez/migrations/0007_auto_20191221_1522.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0007_auto_20191227_2150.py` & `django_xprez-0.2.9/xprez/migrations/0007_auto_20191227_2150.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0009_gridboxes_width.py` & `django_xprez-0.2.9/xprez/migrations/0009_gridboxes_width.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0010_auto_20220204_1540.py` & `django_xprez-0.2.9/xprez/migrations/0010_auto_20220204_1540.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0010_ckeditor.py` & `django_xprez-0.2.9/xprez/migrations/0010_ckeditor.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0011_auto_20220204_1559.py` & `django_xprez-0.2.9/xprez/migrations/0011_auto_20220204_1559.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0012_auto_20220204_1600.py` & `django_xprez-0.2.9/xprez/migrations/0012_auto_20220204_1600.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0016_auto_20220208_1355.py` & `django_xprez-0.2.9/xprez/migrations/0016_auto_20220208_1355.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0017_auto_20220208_1401.py` & `django_xprez-0.2.9/xprez/migrations/0017_auto_20220208_1401.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0021_alter_ckeditor_options_alter_downloadcontent_options_and_more.py` & `django_xprez-0.2.9/xprez/migrations/0021_alter_ckeditor_options_alter_downloadcontent_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0022_content_alternate_color_content_background_color_and_more.py` & `django_xprez-0.2.9/xprez/migrations/0022_content_alternate_color_content_background_color_and_more.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/migrations/0023_remove_content_padding_vertical_and_more.py` & `django_xprez-0.2.9/xprez/migrations/0023_remove_content_padding_vertical_and_more.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/models/base.py` & `django_xprez-0.2.9/xprez/models/base.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/models/contents.py` & `django_xprez-0.2.9/xprez/models/contents.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/models/fields.py` & `django_xprez-0.2.9/xprez/models/fields.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/js/ajax_upload_formset.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/js/ajax_upload_formset.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/js/contents.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/js/contents.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/js/grid_boxes.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/js/grid_boxes.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/README.md` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/README.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/canvas-to-blob.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/canvas-to-blob.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/canvas-to-blob.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/canvas-to-blob.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/canvas-to-blob.min.js.map` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/js/canvas-to-blob.min.js.map`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/package.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/package.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/index.html` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/index.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/test.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/test.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/chai.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/chai.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/load-image.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/load-image.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/mocha.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/mocha.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/mocha.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-canvas-to-blob/test/vendor/mocha.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/.bower.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/.bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/bower.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/css/jquery.fileupload-ui.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/css/jquery.fileupload-ui.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/css/jquery.fileupload.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/css/jquery.fileupload.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/img/loading.gif` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/img/loading.gif`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/img/progressbar.gif` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/img/progressbar.gif`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/cors/jquery.postmessage-transport.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/cors/jquery.postmessage-transport.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/cors/jquery.xdr-transport.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/cors/jquery.xdr-transport.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-angular.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-angular.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-audio.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-audio.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-image.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-image.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-jquery-ui.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-jquery-ui.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-process.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-process.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-ui.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-ui.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-validate.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-validate.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-video.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload-video.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.fileupload.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.iframe-transport.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/jquery.iframe-transport.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-file-upload/js/vendor/jquery.ui.widget.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-file-upload/js/vendor/jquery.ui.widget.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/README.md` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/README.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/css/demo.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/css/demo.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/css/vendor/jquery.Jcrop.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/css/vendor/jquery.Jcrop.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/index.html` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/index.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/demo/demo.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/demo/demo.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-exif-map.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-exif-map.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-exif.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-exif.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-fetch.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-fetch.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-meta.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-meta.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-orientation.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-orientation.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-scale.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image-scale.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image.all.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image.all.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image.all.min.js.map` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image.all.min.js.map`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/load-image.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/vendor/jquery.Jcrop.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/vendor/jquery.Jcrop.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/js/vendor/jquery.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/js/vendor/jquery.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/package.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/package.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/index.html` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/index.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/test.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/test.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/canvas-to-blob.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/canvas-to-blob.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/chai.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/chai.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/mocha.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/mocha.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/mocha.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-load-image/test/vendor/mocha.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/README.md` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/README.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/css/demo.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/css/demo.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/index.html` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/index.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/compile.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/compile.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/demo/demo.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/demo/demo.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/runtime.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/runtime.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/tmpl.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/tmpl.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/tmpl.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/tmpl.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/js/tmpl.min.js.map` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/js/tmpl.min.js.map`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/package.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/package.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/test/index.html` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/test/index.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/test/test.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/test/test.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/chai.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/chai.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/mocha.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/mocha.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/mocha.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/blueimp-tmpl/test/vendor/mocha.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/dropzone/dropzone.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/dropzone/dropzone.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/composer.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/composer.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars-source.gemspec` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars-source.gemspec`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.amd.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.amd.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.amd.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.amd.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.js.nuspec` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.js.nuspec`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.amd.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.amd.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.amd.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.amd.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/handlebars/handlebars.runtime.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/.bower.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/.bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/MIT-LICENSE.txt` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/dist/jquery.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/dist/jquery.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/dist/jquery.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/dist/jquery.min.map` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/dist/jquery.min.map`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax/jsonp.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax/jsonp.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax/load.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax/load.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax/script.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax/script.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax/xhr.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax/xhr.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/ajax.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/ajax.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/attributes/attr.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/attributes/attr.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/attributes/classes.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/attributes/classes.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/attributes/prop.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/attributes/prop.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/attributes/support.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/attributes/support.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/attributes/val.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/attributes/val.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/callbacks.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/callbacks.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/core/access.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/core/access.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/core/init.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/core/init.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/core/parseHTML.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/core/parseHTML.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/core/ready.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/core/ready.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/core.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/core.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css/curCSS.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css/curCSS.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css/defaultDisplay.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css/defaultDisplay.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css/support.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css/support.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css/swap.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css/swap.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/css.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/css.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/data/Data.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/data/Data.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/data.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/data.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/deferred.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/deferred.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/dimensions.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/dimensions.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/effects/Tween.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/effects/Tween.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/effects.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/effects.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/event/alias.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/event/alias.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/event.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/event.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/exports/amd.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/exports/amd.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/exports/global.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/exports/global.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/intro.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/intro.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/jquery.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/jquery.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/manipulation/support.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/manipulation/support.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/manipulation.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/manipulation.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/offset.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/offset.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/queue/delay.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/queue/delay.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/queue.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/queue.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/selector-native.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/selector-native.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/serialize.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/serialize.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/sizzle.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/sizzle.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/sizzle.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/sizzle.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/sizzle.min.map` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/sizzle/dist/sizzle.min.map`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/traversing/findFilter.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/traversing/findFilter.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/traversing.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/traversing.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery/src/wrap.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery/src/wrap.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/.bower.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/.bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/CHANGELOG` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/CHANGELOG`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/Gemfile.lock` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/Gemfile.lock`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/LICENSE` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/LICENSE`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/README.mkd` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/README.mkd`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/TODO` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/TODO`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/config.rb` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/config.rb`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/package.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/package.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/sortable.jquery.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/sortable.jquery.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_limited_drop_targets.html.haml` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_limited_drop_targets.html.haml`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_nested_bootstrap.html.haml` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_nested_bootstrap.html.haml`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_nested_with_switch.html.haml` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_nested_with_switch.html.haml`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_serialization.html.haml` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_serialization.html.haml`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_simple_with_animation.html.haml` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_simple_with_animation.html.haml`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_simple_with_no_drop.html.haml` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_simple_with_no_drop.html.haml`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/_table.html.haml` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/_table.html.haml`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/css/application.css.sass` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/css/application.css.sass`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/css/bootstrap-switch.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/css/bootstrap-switch.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/css/coderay.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/css/coderay.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/css/jquery-sortable.css.sass` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/css/jquery-sortable.css.sass`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/debug.html.erb` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/debug.html.erb`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/img/glyphicons-halflings-white.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/img/glyphicons-halflings.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/index.html.haml` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/index.html.haml`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/application.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/application.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/limited_drop_targets.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/limited_drop_targets.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/nested_with_switch.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/nested_with_switch.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/simple_with_animation.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/simple_with_animation.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/table.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/examples/table.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/jquery-sortable-min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/jquery-sortable-min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/jquery-sortable.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/jquery-sortable.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-button.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-button.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-dropdown.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-dropdown.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-scrollspy.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-scrollspy.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-switch.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/bootstrap-switch.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/jquery.color.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/jquery.color.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/jquery.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/js/vendor/jquery.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery-sortable/source/layouts/layout.haml` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery-sortable/source/layouts/layout.haml`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_444444_256x240.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_555555_256x240.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_777620_256x240.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_777777_256x240.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_cc0000_256x240.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_ffffff_256x240.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/jquery-ui.min.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/jquery_ui/jquery-ui.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/jquery_ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/.bower.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/.bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/API.md` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/API.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/CUSTOM-EVENTS.md` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/CUSTOM-EVENTS.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/LICENSE` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/LICENSE`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/OPTIONS.md` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/OPTIONS.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/README.md` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/README.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/bower.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/medium-editor.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/medium-editor.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/medium-editor.min.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/medium-editor.min.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/beagle.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/beagle.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/beagle.min.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/beagle.min.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/bootstrap.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/bootstrap.min.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/default.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/default.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/default.min.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/default.min.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/flat.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/flat.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/flat.min.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/flat.min.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/mani.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/mani.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/mani.min.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/mani.min.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/roman.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/roman.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/roman.min.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/roman.min.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/tim.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/tim.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/tim.min.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/css/themes/tim.min.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/js/medium-editor.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/js/medium-editor.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor/dist/js/medium-editor.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor/dist/js/medium-editor.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/.bower.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/.bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/CHANGES.md` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/CHANGES.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/LICENSE` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/LICENSE`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/README.md` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/README.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/bower.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin-frontend.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin-frontend.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin-frontend.min.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin-frontend.min.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin.min.css` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin.min.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/js/medium-editor-insert-plugin.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/js/medium-editor-insert-plugin.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/js/medium-editor-insert-plugin.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/dist/js/medium-editor-insert-plugin.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/core.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/core.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/embeds.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/embeds.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/images.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/images.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/embeds-toolbar.hbs` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/embeds-toolbar.hbs`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/images-toolbar.hbs` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates/images-toolbar.hbs`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/js/templates.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/_core.scss` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/_core.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/_embeds.scss` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/_embeds.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/_images.scss` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/_images.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/medium-editor-insert-plugin-frontend.scss` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/medium-editor-insert-plugin/src/sass/medium-editor-insert-plugin-frontend.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/.bower.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/.bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/Authors.txt` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/Authors.txt`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/CONTRIBUTING.md` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/LICENSE` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/LICENSE`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/README.md` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/README.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/bower.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/picturefill.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/picturefill.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/picturefill.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/picturefill.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/intrinsic-dimension/pf.intrinsic.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/intrinsic-dimension/pf.intrinsic.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/intrinsic-dimension/pf.intrinsic.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/intrinsic-dimension/pf.intrinsic.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/mutation/pf.mutation.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/mutation/pf.mutation.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/mutation/pf.mutation.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/mutation/pf.mutation.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/oldie/pf.oldie.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/oldie/pf.oldie.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/oldie/pf.oldie.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/oldie/pf.oldie.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/print/pf.print.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/print/pf.print.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/print/pf.print.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/print/pf.print.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/typesupport/pf.type.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/typesupport/pf.type.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/dist/plugins/typesupport/pf.type.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/dist/plugins/typesupport/pf.type.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/gruntfile.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/gruntfile.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/index.html` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/index.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/logos/bocoup-lg.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/logos/bocoup-lg.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/logos/bocoup-sm.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/logos/bocoup-sm.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/logos/fg-lg.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/logos/fg-lg.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/logos/fg-sm.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/logos/fg-sm.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/logos/ricg-seal.png` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/logos/ricg-seal.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/package.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/package.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/picturefill.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/picturefill.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/gecko-picture/pf.gecko-picture.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/gecko-picture/pf.gecko-picture.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/intrinsic-dimension/pf.intrinsic.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/intrinsic-dimension/pf.intrinsic.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/mutation/pf.mutation.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/mutation/pf.mutation.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/oldie/pf.oldie.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/oldie/pf.oldie.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/print/pf.print.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/print/pf.print.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/picturefill/src/plugins/typesupport/pf.type.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/picturefill/src/plugins/typesupport/pf.type.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/.bower.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/.bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/LICENSE` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/LICENSE`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/bower.json` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-classapplier.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-classapplier.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-classapplier.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-classapplier.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-core.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-core.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-core.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-core.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-highlighter.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-highlighter.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-highlighter.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-highlighter.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-selectionsaverestore.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-selectionsaverestore.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-selectionsaverestore.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-selectionsaverestore.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-serializer.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-serializer.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-serializer.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-serializer.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-textrange.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-textrange.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/admin/libs/rangy/rangy-textrange.min.js` & `django_xprez-0.2.9/xprez/static/xprez/admin/libs/rangy/rangy-textrange.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/backup/xprez.eot` & `django_xprez-0.2.9/xprez/static/xprez/fonts/backup/xprez.eot`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/backup/xprez.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/backup/xprez.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/backup/xprez.ttf` & `django_xprez-0.2.9/xprez/static/xprez/fonts/backup/xprez.ttf`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/backup/xprez.woff` & `django_xprez-0.2.9/xprez/static/xprez/fonts/backup/xprez.woff`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/selection.json` & `django_xprez-0.2.9/xprez/static/xprez/fonts/selection.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/attach_file.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/attach_file.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/background.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/background.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/border.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/border.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/control_point.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/control_point.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/eye.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/eye.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/feature_boxes.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/feature_boxes.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/grid-boxes.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/grid-boxes.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/layout_4.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/layout_4.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/layout_6.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/layout_6.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/layout_8.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/layout_8.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/numbers.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/numbers.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/SVG/video.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/SVG/video.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/src/selection.json` & `django_xprez-0.2.9/xprez/static/xprez/fonts/src/selection.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/xprez.eot` & `django_xprez-0.2.9/xprez/static/xprez/fonts/xprez.eot`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/xprez.svg` & `django_xprez-0.2.9/xprez/static/xprez/fonts/xprez.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/xprez.ttf` & `django_xprez-0.2.9/xprez/static/xprez/fonts/xprez.ttf`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/fonts/xprez.woff` & `django_xprez-0.2.9/xprez/static/xprez/fonts/xprez.woff`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/img/avatar.svg` & `django_xprez-0.2.9/xprez/static/xprez/img/avatar.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/js/modernizr-detection.js` & `django_xprez-0.2.9/xprez/static/xprez/js/modernizr-detection.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/js/photoswipe.js` & `django_xprez-0.2.9/xprez/static/xprez/js/photoswipe.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/js/video.js` & `django_xprez-0.2.9/xprez/static/xprez/js/video.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/.bower.json` & `django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/.bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/LICENSE` & `django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/LICENSE`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/README.md` & `django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/README.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/bower.json` & `django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/counterup.jquery.json` & `django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/counterup.jquery.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/demo/demo.html` & `django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/demo/demo.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/jquery.counterup.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/jquery.counterup.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/counter.up/jquery.counterup.min.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/counter.up/jquery.counterup.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/jquery.waypoints.min.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/jquery.waypoints.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/.bower.json` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/.bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/Gruntfile.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/LICENSE` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/LICENSE`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/README.md` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/README.md`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/bower.json` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/bower.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/component.json` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/component.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/default-skin/default-skin.css` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/default-skin/default-skin.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/default-skin/default-skin.png` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/default-skin/default-skin.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/default-skin/default-skin.svg` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/default-skin/default-skin.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/default-skin/preloader.gif` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/default-skin/preloader.gif`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/photoswipe-ui-default.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/photoswipe-ui-default.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/photoswipe-ui-default.min.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/photoswipe-ui-default.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/photoswipe.css` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/photoswipe.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/photoswipe.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/photoswipe.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/dist/photoswipe.min.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/dist/photoswipe.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/package.json` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/package.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/photoswipe.json` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/photoswipe.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/_main-settings.scss` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/_main-settings.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin-svg.sketch/Data` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin-svg.sketch/Data`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.png` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.png`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.psd` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.psd`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.scss` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.svg` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/default-skin.svg`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/default-skin/preloader.gif` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/default-skin/preloader.gif`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/main.css` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/main.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/css/main.scss` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/css/main.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/core.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/core.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/desktop-zoom.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/desktop-zoom.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/framework-bridge.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/framework-bridge.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/gestures.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/gestures.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/history.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/history.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/items-controller.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/items-controller.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/show-hide-transition.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/show-hide-transition.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/tap.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/tap.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/photoswipe/src/js/ui/photoswipe-ui-default.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/photoswipe/src/js/ui/photoswipe-ui-default.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/libs/picturefill.min.js` & `django_xprez-0.2.9/xprez/static/xprez/libs/picturefill.min.js`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/package-lock.json` & `django_xprez-0.2.9/xprez/static/xprez/package-lock.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/package.json` & `django_xprez-0.2.9/xprez/static/xprez/package.json`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/_config.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/_config.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_add-module.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_add-module.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_admin-buttons.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_admin-buttons.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_form-elements.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_form-elements.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_grid-boxes.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_grid-boxes.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_icons.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_icons.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_image-text.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_image-text.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/_photo-gallery.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/_photo-gallery.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/backend/xprez-backend.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/backend/xprez-backend.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_boxed-text.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_boxed-text.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_button.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_button.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_download.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_download.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_editor_media.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_editor_media.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_feature-boxes.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_feature-boxes.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_grid-boxes.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_grid-boxes.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_layout.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_layout.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_module-relations.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_module-relations.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_numbers.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_numbers.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_photo-gallery.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_photo-gallery.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_quote.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_quote.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_text-image.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_text-image.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_typography.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_typography.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/_video.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/_video.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/frontend/xprez-frontend.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/frontend/xprez-frontend.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/library/_lib-prefixer.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/library/_lib-prefixer.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/library/_mixins.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/library/_mixins.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/scss/library/_rfs.scss` & `django_xprez-0.2.9/xprez/static/xprez/styles/scss/library/_rfs.scss`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/xprez-backend.css` & `django_xprez-0.2.9/xprez/static/xprez/styles/xprez-backend.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/xprez-backend.css.map` & `django_xprez-0.2.9/xprez/static/xprez/styles/xprez-backend.css.map`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/xprez-frontend.css` & `django_xprez-0.2.9/xprez/static/xprez/styles/xprez-frontend.css`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/static/xprez/styles/xprez-frontend.css.map` & `django_xprez-0.2.9/xprez/static/xprez/styles/xprez-frontend.css.map`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/base.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/base.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/ck_editor.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/ck_editor.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/download/attachment.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/download/attachment.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/download/download.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/download/download.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/feature_boxes.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/feature_boxes.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/gallery/gallery.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/gallery/gallery.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/gallery/photo.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/gallery/photo.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/grid_boxes/box.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/grid_boxes/box.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/grid_boxes/grid_boxes.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/grid_boxes/grid_boxes.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/medium_editor.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/medium_editor.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/numbers.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/numbers.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/quote.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/quote.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/text_image.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/text_image.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/contents/video.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/contents/video.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/form/multi_row.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/form/multi_row.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/includes/add_list.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/includes/add_list.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/xprez.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/xprez.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/admin/xprez_changeform.html` & `django_xprez-0.2.9/xprez/templates/xprez/admin/xprez_changeform.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/contents/base.html` & `django_xprez-0.2.9/xprez/templates/xprez/contents/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% block content %}
-<div class="xprez-module-cont xprez-module-margin-bottom-{{ content.margin_bottom }} xprez-module-padding-top-{{ content.padding_top }} xprez-module-padding-bottom-{{ content.padding_bottom }}  {{ content.css_class|default:'' }}"
+<div class="xprez-module-cont xprez-module-margin-bottom-{{ content.margin_bottom }} xprez-module-padding-top-{{ content.padding_top }} xprez-module-padding-bottom-{{ content.padding_bottom }}  {{ content.css_class|default:'' }} {% if content.alternate_color %}xprez-module-alternate-color{% endif %}"
      {% if content.background_color %}style="background-color: {{ content.background_color }};"{% endif %}
 >
     <div
-        class="{% block css_class %}xprez-module {% if content.alternate_color %}xprez-module-alternate-color{% endif %} {% block css_class_extra %}{% endblock %}{% endblock %}"
+        class="{% block css_class %}xprez-module {% block css_class_extra %}{% endblock %}{% endblock %}"
     >
         {% block content_in %}
         {% endblock %}
     </div>
 </div>
 {% endblock %}
```

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/contents/download.html` & `django_xprez-0.2.9/xprez/templates/xprez/contents/download.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/contents/gallery.html` & `django_xprez-0.2.9/xprez/templates/xprez/contents/gallery.html`

 * *Files 2% similar despite different names*

```diff
@@ -118,37 +118,37 @@
                                 {% endthumbnail %}{% thumbnail photo.image "1500x1500" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
                                     {{ thumb.url|build_absolute_uri }} 1500w
                                 {% endthumbnail %}"
                             sizes="(min-width: 500px) 50vw,100vw"
                     {% endif %}
                 {% else %}
                     {% if content.crop %}
-                        src="{% thumbnail photo.image "400x400" crop="30%" format="WEBP" quality=70 filename_stem=alt_text as thumb %}{{ thumb.url|build_absolute_uri }}"
-                            srcset="{{ thumb.url|build_absolute_uri }} 400w,
-                                {% endthumbnail %}{% thumbnail photo.image "800x600" crop="30%" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
+                        src="{% thumbnail photo.image "600x600" crop="30%" format="WEBP" quality=70 filename_stem=alt_text as thumb %}{{ thumb.url|build_absolute_uri }}"
+                            srcset="{{ thumb.url|build_absolute_uri }} 600w,
+                                {% endthumbnail %}{% thumbnail photo.image "1000x769" crop="30%" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
                                     {{ thumb.url|build_absolute_uri }} 800w,
-                                {% endthumbnail %}{% thumbnail photo.image "1000x770" crop="30%" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
-                                    {{ thumb.url|build_absolute_uri }} 1000w,
-                                {% endthumbnail %}{% thumbnail photo.image "1500x1150" crop="30%" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
+                                {% endthumbnail %}{% thumbnail photo.image "1500x1153" crop="30%" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
                                     {{ thumb.url|build_absolute_uri }} 1500w,
-                                {% endthumbnail %}{% thumbnail photo.image "1900x1500" crop="30%" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
-                                    {{ thumb.url|build_absolute_uri }} 1900w
+                                {% endthumbnail %}{% thumbnail photo.image "2000x1538" crop="30%" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
+                                    {{ thumb.url|build_absolute_uri }} 2000w,
+                                {% endthumbnail %}{% thumbnail photo.image "2500x1923" crop="30%" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
+                                    {{ thumb.url|build_absolute_uri }} 2500w
                                 {% endthumbnail %}"
                             sizes="100vw"
                     {% else %}
-                        src="{% thumbnail photo.image "400x400" format="WEBP" quality=70 filename_stem=alt_text as thumb %}{{ thumb.url|build_absolute_uri }}"
-                            srcset="{{ thumb.url|build_absolute_uri }} 400w,
-                                {% endthumbnail %}{% thumbnail photo.image "800x800" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
-                                    {{ thumb.url|build_absolute_uri }} 800w,
+                        src="{% thumbnail photo.image "600x600" format="WEBP" quality=70 filename_stem=alt_text as thumb %}{{ thumb.url|build_absolute_uri }}"
+                            srcset="{{ thumb.url|build_absolute_uri }} 600w,
                                 {% endthumbnail %}{% thumbnail photo.image "1000x1000" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
                                     {{ thumb.url|build_absolute_uri }} 1000w,
                                 {% endthumbnail %}{% thumbnail photo.image "1500x1500" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
                                     {{ thumb.url|build_absolute_uri }} 1500w,
-                                {% endthumbnail %}{% thumbnail photo.image "1900x1900" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
-                                    {{ thumb.url|build_absolute_uri }} 1900w
+                                {% endthumbnail %}{% thumbnail photo.image "2000x2000" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
+                                    {{ thumb.url|build_absolute_uri }} 2000w,
+                                {% endthumbnail %}{% thumbnail photo.image "2500x2500" format="WEBP" quality=70 filename_stem=alt_text as thumb %}
+                                    {{ thumb.url|build_absolute_uri }} 2500w
                                 {% endthumbnail %}"
                             sizes="100vw"
                     {% endif %}
                 {% endif %}
             />
 
             {% if photo.description %}
```

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/contents/grid_boxes.html` & `django_xprez-0.2.9/xprez/templates/xprez/contents/grid_boxes.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/contents/numbers.html` & `django_xprez-0.2.9/xprez/templates/xprez/contents/numbers.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/contents/quote.html` & `django_xprez-0.2.9/xprez/templates/xprez/contents/quote.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/contents/text_image.html` & `django_xprez-0.2.9/xprez/templates/xprez/contents/text_image.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/contents/video.html` & `django_xprez-0.2.9/xprez/templates/xprez/contents/video.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/includes/editor_image.html` & `django_xprez-0.2.9/xprez/templates/xprez/includes/editor_image.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templates/xprez/includes/photoswipe.html` & `django_xprez-0.2.9/xprez/templates/xprez/includes/photoswipe.html`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/templatetags/xprez.py` & `django_xprez-0.2.9/xprez/templatetags/xprez.py`

 * *Files identical despite different names*

### Comparing `django_xprez-0.2.8/xprez/utils.py` & `django_xprez-0.2.9/xprez/utils.py`

 * *Files identical despite different names*

