# Comparing `tmp/djangocms_text-0.1.0.tar.gz` & `tmp/djangocms_text-0.1.1.tar.gz`

## Comparing `djangocms_text-0.1.0.tar` & `djangocms_text-0.1.1.tar`

### file list

```diff
@@ -1,802 +1,818 @@
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/apps.py
--rw-r--r--   0        0        0    28095 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/cms_plugins.py
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/cms_toolbars.py
--rw-r--r--   0        0        0    27864 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/editors.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/fields.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/forms.py
--rw-r--r--   0        0        0    13217 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/html.py
--rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/models.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/settings.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/utils.py
--rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/__init__.py
--rw-r--r--   0        0        0   314777 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/CHANGES.md
--rw-r--r--   0        0        0    78399 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/LICENSE.md
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/SECURITY.md
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/bender-runner.config.json
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/build-config.js
--rw-r--r--   0        0        0   680302 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/ckeditor.js
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/config.js
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/contents.css
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/styles.js
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/adapters/jquery.js
--rw-r--r--   0        0        0    12599 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/af.js
--rw-r--r--   0        0        0    15803 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ar.js
--rw-r--r--   0        0        0    13612 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/az.js
--rw-r--r--   0        0        0    18969 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/bg.js
--rw-r--r--   0        0        0    16521 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/bn.js
--rw-r--r--   0        0        0    12681 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/bs.js
--rw-r--r--   0        0        0    13924 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ca.js
--rw-r--r--   0        0        0    13874 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/cs.js
--rw-r--r--   0        0        0    12979 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/cy.js
--rw-r--r--   0        0        0    13251 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/da.js
--rw-r--r--   0        0        0    13952 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/de-ch.js
--rw-r--r--   0        0        0    13945 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/de.js
--rw-r--r--   0        0        0    20454 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/el.js
--rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en-au.js
--rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en-ca.js
--rw-r--r--   0        0        0    12637 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en-gb.js
--rw-r--r--   0        0        0    12635 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en.js
--rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/eo.js
--rw-r--r--   0        0        0    14075 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/es-mx.js
--rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/es.js
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/et.js
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/eu.js
--rw-r--r--   0        0        0    17129 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fa.js
--rw-r--r--   0        0        0    13363 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fi.js
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fo.js
--rw-r--r--   0        0        0    13769 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fr-ca.js
--rw-r--r--   0        0        0    14495 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fr.js
--rw-r--r--   0        0        0    14005 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/gl.js
--rw-r--r--   0        0        0    20558 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/gu.js
--rw-r--r--   0        0        0    15395 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/he.js
--rw-r--r--   0        0        0    16668 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/hi.js
--rw-r--r--   0        0        0    12953 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/hr.js
--rw-r--r--   0        0        0    14158 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/hu.js
--rw-r--r--   0        0        0    12953 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/id.js
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/is.js
--rw-r--r--   0        0        0    14079 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/it.js
--rw-r--r--   0        0        0    15353 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ja.js
--rw-r--r--   0        0        0    21596 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ka.js
--rw-r--r--   0        0        0    23848 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/km.js
--rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ko.js
--rw-r--r--   0        0        0    18533 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ku.js
--rw-r--r--   0        0        0    13787 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/lt.js
--rw-r--r--   0        0        0    14013 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/lv.js
--rw-r--r--   0        0        0    14072 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/mk.js
--rw-r--r--   0        0        0    16013 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/mn.js
--rw-r--r--   0        0        0    12801 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ms.js
--rw-r--r--   0        0        0    12872 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/nb.js
--rw-r--r--   0        0        0    13274 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/nl.js
--rw-r--r--   0        0        0    12917 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/no.js
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/oc.js
--rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/pl.js
--rw-r--r--   0        0        0    14028 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/pt-br.js
--rw-r--r--   0        0        0    13937 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/pt.js
--rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ro.js
--rw-r--r--   0        0        0    19388 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ru.js
--rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/si.js
--rw-r--r--   0        0        0    13968 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sk.js
--rw-r--r--   0        0        0    13157 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sl.js
--rw-r--r--   0        0        0    14209 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sq.js
--rw-r--r--   0        0        0    13226 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sr-latn.js
--rw-r--r--   0        0        0    18199 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sr.js
--rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sv.js
--rw-r--r--   0        0        0    19588 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/th.js
--rw-r--r--   0        0        0    13898 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/tr.js
--rw-r--r--   0        0        0    16206 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/tt.js
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ug.js
--rw-r--r--   0        0        0    19509 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/uk.js
--rw-r--r--   0        0        0    15078 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/vi.js
--rw-r--r--   0        0        0    12353 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/zh-cn.js
--rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/zh.js
--rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/icons.png
--rw-r--r--   0        0        0    18632 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/icons_hidpi.png
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/a11yhelp.js
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/_translationstatus.txt
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/af.js
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ar.js
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/az.js
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/bg.js
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ca.js
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/cs.js
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/cy.js
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/da.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/de-ch.js
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/de.js
--rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/el.js
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/en-au.js
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/en-gb.js
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/en.js
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/eo.js
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/es-mx.js
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/es.js
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/et.js
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/eu.js
--rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fa.js
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fi.js
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fo.js
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fr-ca.js
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fr.js
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/gl.js
--rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/gu.js
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/he.js
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/hi.js
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/hr.js
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/hu.js
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/id.js
--rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/it.js
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ja.js
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/km.js
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ko.js
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ku.js
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/lt.js
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/lv.js
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/mk.js
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/mn.js
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/nb.js
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/nl.js
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/no.js
--rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/oc.js
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/pl.js
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/pt-br.js
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/pt.js
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ro.js
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ru.js
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/si.js
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sk.js
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sl.js
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sq.js
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sr-latn.js
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sr.js
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sv.js
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/th.js
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/tr.js
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/tt.js
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ug.js
--rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/uk.js
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/vi.js
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/zh-cn.js
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/zh.js
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/about/dialogs/about.js
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/about/dialogs/logo_ckeditor.png
--rw-r--r--   0        0        0    12236 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/about/dialogs/hidpi/logo_ckeditor.png
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/clipboard/dialogs/paste.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/dialog/dialogDefinition.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/dialog/styles/dialog.css
--rw-r--r--   0        0        0    21529 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/image/dialogs/image.js
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/image/images/noimage.png
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/dialogs/anchor.js
--rw-r--r--   0        0        0    13234 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/dialogs/link.js
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/images/anchor.png
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/images/hidpi/anchor.png
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/magicline/images/icon-rtl.png
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/magicline/images/icon.png
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/magicline/images/hidpi/icon-rtl.png
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/magicline/images/hidpi/icon.png
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastefromgdocs/filter/default.js
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastefromlibreoffice/filter/default.js
--rw-r--r--   0        0        0    19902 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastefromword/filter/default.js
--rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastetools/filter/common.js
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastetools/filter/image.js
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/CHANGELOG.md
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/LICENSE.md
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/README.md
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/dialogs/dialog.css
--rw-r--r--   0        0        0    16136 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/dialogs/options.js
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/dialogs/toolbar.css
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/skins/moono-lisa/scayt.css
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/specialchar.js
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/_translationstatus.txt
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/af.js
--rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ar.js
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/az.js
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/bg.js
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ca.js
--rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/cs.js
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/cy.js
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/da.js
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/de-ch.js
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/de.js
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/el.js
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en-au.js
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en-ca.js
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en-gb.js
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en.js
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/eo.js
--rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/es-mx.js
--rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/es.js
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/et.js
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/eu.js
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fa.js
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fi.js
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fr-ca.js
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fr.js
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/gl.js
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/he.js
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/hr.js
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/hu.js
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/id.js
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/it.js
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ja.js
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/km.js
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ko.js
--rw-r--r--   0        0        0     7578 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ku.js
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/lt.js
--rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/lv.js
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/nb.js
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/nl.js
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/no.js
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/oc.js
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/pl.js
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/pt-br.js
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/pt.js
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ro.js
--rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ru.js
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/si.js
--rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sk.js
--rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sl.js
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sq.js
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sr-latn.js
--rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sr.js
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sv.js
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/th.js
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/tr.js
--rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/tt.js
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ug.js
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/uk.js
--rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/vi.js
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/zh-cn.js
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/zh.js
--rw-r--r--   0        0        0     9043 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/table/dialogs/table.js
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/tableselection/styles/tableselection.css
--rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/tabletools/dialogs/tableCell.js
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/widget/images/handle.png
--rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/index.html
--rw-r--r--   0        0        0    67340 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/css/samples.css
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/github-top.png
--rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/header-bg.png
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/header-separator.png
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/logo.png
--rw-r--r--   0        0        0    10887 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/logo.svg
--rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/navigation-tip.png
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/js/sample.js
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/js/sf.js
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/ajax.html
--rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/api.html
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/appendto.html
--rw-r--r--   0        0        0    47840 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/datafiltering.html
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/divreplace.html
--rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/index.html
--rw-r--r--   0        0        0    10399 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/inlineall.html
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/inlinebycode.html
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/inlinetextarea.html
--rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/jquery.html
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/readonly.html
--rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/replacebyclass.html
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/replacebycode.html
--rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/sample.css
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/sample.js
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/sample_posteddata.php
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/tabindex.html
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/uicolor.html
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/uilanguages.html
--rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/xhtmlstyle.html
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/posteddata.php
--rw-r--r--   0        0        0    14449 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/sample.jpg
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/inlineall/logo.png
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/outputxhtml/outputxhtml.css
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/uilanguages/languages.js
--rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/dialog/dialog.html
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/dialog/assets/my_dialog.js
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/enterkey/enterkey.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/htmlwriter/outputhtml.html
--rw-r--r--   0        0        0     8585 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/magicline/magicline.html
--rw-r--r--   0        0        0     9122 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/toolbar/toolbar.html
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/wysiwygarea/fullpage.html
--rw-r--r--   0        0        0    15808 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/index.html
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/css/fontello.css
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/LICENSE.txt
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/config.json
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.eot
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.svg
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.ttf
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.woff
--rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/abstracttoolbarmodifier.js
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/fulltoolbareditor.js
--rw-r--r--   0        0        0    16651 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/toolbarmodifier.js
--rw-r--r--   0        0        0     6850 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/toolbartextmodifier.js
--rw-r--r--   0        0        0    13634 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog.css
--rw-r--r--   0        0        0    14657 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog_ie.css
--rw-r--r--   0        0        0    15206 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog_ie8.css
--rw-r--r--   0        0        0    14686 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog_iequirks.css
--rw-r--r--   0        0        0    35906 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor.css
--rw-r--r--   0        0        0    35987 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_gecko.css
--rw-r--r--   0        0        0    36905 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_ie.css
--rw-r--r--   0        0        0    37711 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_ie8.css
--rw-r--r--   0        0        0    37554 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_iequirks.css
--rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/icons.png
--rw-r--r--   0        0        0    18632 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/icons_hidpi.png
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/readme.md
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/arrow.png
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/close.png
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/lock-open.png
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/lock.png
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/refresh.png
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/spinner.gif
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/close.png
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/lock-open.png
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/lock.png
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/refresh.png
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/vendor/promise.js
--rw-r--r--   0        0        0   116891 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsdialog/plugin.js
--rw-r--r--   0        0        0    23630 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsplugins/plugin.js
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsplugins/icons/cmsplugins.svg
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsresize/plugin.js
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmswidget/plugin.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor5/__init__.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor5/static/djangocms_text/css/cms.ckeditor5.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_quill/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_quill/static/djangocms_text/css/cms.quill.css
--rw-r--r--   0        0        0    26009 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/bubble.css
--rw-r--r--   0        0        0    25223 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/quill.bubble.css
--rw-r--r--   0        0        0    10236 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/quill.core.css
--rw-r--r--   0        0        0    24613 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/quill.snow.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_tinymce/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/contrib/text_tinymce/static/djangocms_text/css/cms.tinymce.css
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/bn/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/da/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/el/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/et/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/eu/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/fi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/gl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/hi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/hr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/hu/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/is/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/lt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/no/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/sv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/migrations/0001_initial.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/migrations/0002_text_json_text_rte.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/migrations/__init__.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/css/cms.ckeditor4.css
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/css/cms.normalize.css
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/css/cms.text.css
--rw-r--r--   0        0        0   890296 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/js/ckeditor4.js
--rw-r--r--   0        0        0  1084627 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/js/ckeditor4.js.map
--rw-r--r--   0        0        0    13818 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/js/editor.js.map
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/config.js
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/contents.css
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/styles.js
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/adapters/jquery.js
--rw-r--r--   0        0        0    17242 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/af.js
--rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ar.js
--rw-r--r--   0        0        0    19066 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/az.js
--rw-r--r--   0        0        0    26179 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/bg.js
--rw-r--r--   0        0        0    22656 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/bn.js
--rw-r--r--   0        0        0    17291 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/bs.js
--rw-r--r--   0        0        0    18989 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ca.js
--rw-r--r--   0        0        0    19007 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/cs.js
--rw-r--r--   0        0        0    17696 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/cy.js
--rw-r--r--   0        0        0    18066 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/da.js
--rw-r--r--   0        0        0    18861 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/de-ch.js
--rw-r--r--   0        0        0    18839 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/de.js
--rw-r--r--   0        0        0    28070 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/el.js
--rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en-au.js
--rw-r--r--   0        0        0    17192 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en-ca.js
--rw-r--r--   0        0        0    17217 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en-gb.js
--rw-r--r--   0        0        0    17207 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en.js
--rw-r--r--   0        0        0    18418 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/eo.js
--rw-r--r--   0        0        0    19675 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/es-mx.js
--rw-r--r--   0        0        0    19174 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/es.js
--rw-r--r--   0        0        0    17828 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/et.js
--rw-r--r--   0        0        0    18860 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/eu.js
--rw-r--r--   0        0        0    23657 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fa.js
--rw-r--r--   0        0        0    18273 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fi.js
--rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fo.js
--rw-r--r--   0        0        0    18774 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fr-ca.js
--rw-r--r--   0        0        0    19665 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fr.js
--rw-r--r--   0        0        0    19221 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/gl.js
--rw-r--r--   0        0        0    28283 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/gu.js
--rw-r--r--   0        0        0    21259 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/he.js
--rw-r--r--   0        0        0    23097 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/hi.js
--rw-r--r--   0        0        0    17804 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/hr.js
--rw-r--r--   0        0        0    19372 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/hu.js
--rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/id.js
--rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/is.js
--rw-r--r--   0        0        0    19072 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/it.js
--rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ja.js
--rw-r--r--   0        0        0    30679 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ka.js
--rw-r--r--   0        0        0    31712 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/km.js
--rw-r--r--   0        0        0    18627 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ko.js
--rw-r--r--   0        0        0    25736 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ku.js
--rw-r--r--   0        0        0    18928 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/lt.js
--rw-r--r--   0        0        0    19144 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/lv.js
--rw-r--r--   0        0        0    18944 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/mk.js
--rw-r--r--   0        0        0    21951 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/mn.js
--rw-r--r--   0        0        0    17496 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ms.js
--rw-r--r--   0        0        0    17594 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/nb.js
--rw-r--r--   0        0        0    18213 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/nl.js
--rw-r--r--   0        0        0    17615 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/no.js
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/oc.js
--rw-r--r--   0        0        0    19199 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/pl.js
--rw-r--r--   0        0        0    19239 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/pt-br.js
--rw-r--r--   0        0        0    19110 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/pt.js
--rw-r--r--   0        0        0    19938 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ro.js
--rw-r--r--   0        0        0    27017 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ru.js
--rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/si.js
--rw-r--r--   0        0        0    19290 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sk.js
--rw-r--r--   0        0        0    17995 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sl.js
--rw-r--r--   0        0        0    19705 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sq.js
--rw-r--r--   0        0        0    18158 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sr-latn.js
--rw-r--r--   0        0        0    25230 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sr.js
--rw-r--r--   0        0        0    17749 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sv.js
--rw-r--r--   0        0        0    26591 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/th.js
--rw-r--r--   0        0        0    18840 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/tr.js
--rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/tt.js
--rw-r--r--   0        0        0    25273 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ug.js
--rw-r--r--   0        0        0    27018 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/uk.js
--rw-r--r--   0        0        0    20670 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/vi.js
--rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/zh-cn.js
--rw-r--r--   0        0        0    16747 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/zh.js
--rw-r--r--   0        0        0    11937 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/icons.png
--rw-r--r--   0        0        0    37595 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/icons_hidpi.png
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/a11yhelp.js
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/_translationstatus.txt
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/af.js
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ar.js
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/az.js
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/bg.js
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ca.js
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/cs.js
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/cy.js
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/da.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/de-ch.js
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/de.js
--rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/el.js
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/en-au.js
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/en-gb.js
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/en.js
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/eo.js
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/es-mx.js
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/es.js
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/et.js
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/eu.js
--rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fa.js
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fi.js
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fo.js
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fr-ca.js
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fr.js
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/gl.js
--rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/gu.js
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/he.js
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/hi.js
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/hr.js
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/hu.js
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/id.js
--rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/it.js
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ja.js
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/km.js
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ko.js
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ku.js
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/lt.js
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/lv.js
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/mk.js
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/mn.js
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/nb.js
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/nl.js
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/no.js
--rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/oc.js
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/pl.js
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/pt-br.js
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/pt.js
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ro.js
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ru.js
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/si.js
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sk.js
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sl.js
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sq.js
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sr-latn.js
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sr.js
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sv.js
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/th.js
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/tr.js
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/tt.js
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ug.js
--rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/uk.js
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/vi.js
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/zh-cn.js
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/zh.js
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/about/dialogs/about.js
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/about/dialogs/logo_ckeditor.png
--rw-r--r--   0        0        0    12236 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/about/dialogs/hidpi/logo_ckeditor.png
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/clipboard/dialogs/paste.js
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/colordialog/dialogs/colordialog.css
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/colordialog/dialogs/colordialog.js
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/copyformatting/cursors/cursor-disabled.svg
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/copyformatting/cursors/cursor.svg
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/copyformatting/styles/copyformatting.css
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/dialog/dialogDefinition.js
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/dialog/styles/dialog.css
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/div/dialogs/div.js
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/CHANGELOG.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/LICENSE.md
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/README.md
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/plugindefinition.js
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/authentication.js
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/exportpdf.js
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/notification.js
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/resourcespaths.js
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/statistics.js
--rw-r--r--   0        0        0     9882 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/stylesheets.js
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/_helpers/tools.js
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/configfilename.html
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/configfilename.md
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/emptyeditor.html
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/emptyeditor.md
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integration.html
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integration.md
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notifications.html
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notifications.md
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notificationsasync.html
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notificationsasync.md
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/paperformat.html
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/paperformat.md
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/readonly.html
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/readonly.md
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/stylesheets.html
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/stylesheets.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenfetching.html
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenfetching.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.html
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.md
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokentwoeditorswrong.html
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokentwoeditorswrong.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenwithouturl.html
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenwithouturl.md
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/wrongendpoint.html
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/wrongendpoint.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integrations/easyimage.html
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integrations/easyimage.md
--rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/find/dialogs/find.js
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/button.js
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/checkbox.js
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/form.js
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/hiddenfield.js
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/radio.js
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/select.js
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/textarea.js
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/textfield.js
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/images/hiddenfield.gif
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/iframe/dialogs/iframe.js
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/iframe/images/placeholder.png
--rw-r--r--   0        0        0    21529 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/image/dialogs/image.js
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/image/images/noimage.png
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/dialogs/anchor.js
--rw-r--r--   0        0        0    13234 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/dialogs/link.js
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/images/anchor.png
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/images/hidpi/anchor.png
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/liststyle/dialogs/liststyle.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/magicline/images/icon-rtl.png
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/magicline/images/icon.png
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/magicline/images/hidpi/icon-rtl.png
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/magicline/images/hidpi/icon.png
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pagebreak/images/pagebreak.gif
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastefromgdocs/filter/default.js
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastefromlibreoffice/filter/default.js
--rw-r--r--   0        0        0    19568 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastefromword/filter/default.js
--rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastetools/filter/common.js
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastetools/filter/image.js
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/preview/preview.html
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/preview/images/pagebreak.gif
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/preview/styles/screen.css
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/CHANGELOG.md
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/LICENSE.md
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/README.md
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/dialogs/dialog.css
--rw-r--r--   0        0        0    16136 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/dialogs/options.js
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/dialogs/toolbar.css
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/skins/moono-lisa/scayt.css
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_address.png
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_blockquote.png
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_div.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_h1.png
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_h2.png
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_h3.png
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_h4.png
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_h5.png
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_h6.png
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_p.png
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_pre.png
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/dialogs/smiley.js
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angel_smile.gif
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angel_smile.png
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angry_smile.gif
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angry_smile.png
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/broken_heart.gif
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/broken_heart.png
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/confused_smile.gif
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/confused_smile.png
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/cry_smile.gif
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/cry_smile.png
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/devil_smile.gif
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/devil_smile.png
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/embaressed_smile.gif
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/embarrassed_smile.gif
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/embarrassed_smile.png
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/envelope.gif
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/envelope.png
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/heart.gif
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/heart.png
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/kiss.gif
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/kiss.png
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/lightbulb.gif
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/lightbulb.png
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/omg_smile.gif
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/omg_smile.png
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/regular_smile.gif
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/regular_smile.png
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/sad_smile.gif
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/sad_smile.png
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/shades_smile.gif
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/shades_smile.png
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/teeth_smile.gif
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/teeth_smile.png
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_down.gif
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_down.png
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_up.gif
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_up.png
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/tongue_smile.gif
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/tongue_smile.png
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/tounge_smile.gif
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/whatchutalkingabout_smile.gif
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/whatchutalkingabout_smile.png
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/wink_smile.gif
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/wink_smile.png
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/specialchar.js
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/_translationstatus.txt
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/af.js
--rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ar.js
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/az.js
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/bg.js
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ca.js
--rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/cs.js
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/cy.js
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/da.js
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/de-ch.js
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/de.js
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/el.js
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en-au.js
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en-ca.js
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en-gb.js
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en.js
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/eo.js
--rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/es-mx.js
--rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/es.js
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/et.js
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/eu.js
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fa.js
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fi.js
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fr-ca.js
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fr.js
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/gl.js
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/he.js
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/hr.js
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/hu.js
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/id.js
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/it.js
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ja.js
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/km.js
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ko.js
--rw-r--r--   0        0        0     7578 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ku.js
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/lt.js
--rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/lv.js
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/nb.js
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/nl.js
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/no.js
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/oc.js
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/pl.js
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/pt-br.js
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/pt.js
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ro.js
--rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ru.js
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/si.js
--rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sk.js
--rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sl.js
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sq.js
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sr-latn.js
--rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sr.js
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sv.js
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/th.js
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/tr.js
--rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/tt.js
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ug.js
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/uk.js
--rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/vi.js
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/zh-cn.js
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/zh.js
--rw-r--r--   0        0        0     9043 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/table/dialogs/table.js
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/tableselection/styles/tableselection.css
--rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/tabletools/dialogs/tableCell.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templatedefinition.js
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/dialogs/templates.css
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/dialogs/templates.js
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/default.js
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/images/template1.gif
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/images/template2.gif
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/images/template3.gif
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/widget/images/handle.png
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/LICENSE.md
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/README.md
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/ciframe.html
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/tmpFrameset.html
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/wsc.css
--rw-r--r--   0        0        0    47292 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/wsc.js
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/wsc_ie.js
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/skins/moono-lisa/wsc.css
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog.css
--rw-r--r--   0        0        0    15866 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog_ie.css
--rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog_ie8.css
--rw-r--r--   0        0        0    15895 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog_iequirks.css
--rw-r--r--   0        0        0    24410 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor.css
--rw-r--r--   0        0        0    24491 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_gecko.css
--rw-r--r--   0        0        0    25409 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_ie.css
--rw-r--r--   0        0        0    26258 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_ie8.css
--rw-r--r--   0        0        0    26058 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_iequirks.css
--rw-r--r--   0        0        0    11937 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/icons.png
--rw-r--r--   0        0        0    37595 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/icons_hidpi.png
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/readme.md
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/arrow.png
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/close.png
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/lock-open.png
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/lock.png
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/refresh.png
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/spinner.gif
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/close.png
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/lock-open.png
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/lock.png
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/refresh.png
--rw-r--r--   0        0        0    20702 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text_ckeditor/js/cms.ckeditor.js
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text_ckeditor/js/post.js
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/static/djangocms_text_ckeditor/js/pre.js
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/templates/cms/plugins/inline.html
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/templates/cms/plugins/render_plugin_preview.html
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/templates/cms/plugins/text.html
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/templates/cms/plugins/text_plugin_change_formx.html
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/templates/cms/plugins/widgets/ckeditor.html
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/templates/cms/plugins/widgets/editor.html
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/templates/cms/toolbar/icon-button.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/templatetags/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text/templatetags/djangocms_text_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text_ckeditor/__init__.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text_ckeditor/fields.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/djangocms_text_ckeditor/widgets.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/LICENSE
--rw-r--r--   0        0        0    28512 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/README.rst
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 djangocms_text-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/apps.py
+-rw-r--r--   0        0        0    28095 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/cms_plugins.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/cms_toolbars.py
+-rw-r--r--   0        0        0    28207 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/editors.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/fields.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/forms.py
+-rw-r--r--   0        0        0    13217 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/html.py
+-rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/models.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/settings.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/utils.py
+-rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/__init__.py
+-rw-r--r--   0        0        0   314777 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/CHANGES.md
+-rw-r--r--   0        0        0    78399 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/LICENSE.md
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/SECURITY.md
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/bender-runner.config.json
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/build-config.js
+-rw-r--r--   0        0        0   680302 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/ckeditor.js
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/config.js
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/contents.css
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/styles.js
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/adapters/jquery.js
+-rw-r--r--   0        0        0    12599 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/af.js
+-rw-r--r--   0        0        0    15803 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ar.js
+-rw-r--r--   0        0        0    13612 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/az.js
+-rw-r--r--   0        0        0    18969 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/bg.js
+-rw-r--r--   0        0        0    16521 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/bn.js
+-rw-r--r--   0        0        0    12681 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/bs.js
+-rw-r--r--   0        0        0    13924 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ca.js
+-rw-r--r--   0        0        0    13874 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/cs.js
+-rw-r--r--   0        0        0    12979 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/cy.js
+-rw-r--r--   0        0        0    13251 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/da.js
+-rw-r--r--   0        0        0    13952 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/de-ch.js
+-rw-r--r--   0        0        0    13945 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/de.js
+-rw-r--r--   0        0        0    20454 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/el.js
+-rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en-au.js
+-rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en-ca.js
+-rw-r--r--   0        0        0    12637 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en-gb.js
+-rw-r--r--   0        0        0    12635 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en.js
+-rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/eo.js
+-rw-r--r--   0        0        0    14075 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/es-mx.js
+-rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/es.js
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/et.js
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/eu.js
+-rw-r--r--   0        0        0    17129 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fa.js
+-rw-r--r--   0        0        0    13363 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fi.js
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fo.js
+-rw-r--r--   0        0        0    13769 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fr-ca.js
+-rw-r--r--   0        0        0    14495 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fr.js
+-rw-r--r--   0        0        0    14005 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/gl.js
+-rw-r--r--   0        0        0    20558 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/gu.js
+-rw-r--r--   0        0        0    15395 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/he.js
+-rw-r--r--   0        0        0    16668 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/hi.js
+-rw-r--r--   0        0        0    12953 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/hr.js
+-rw-r--r--   0        0        0    14158 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/hu.js
+-rw-r--r--   0        0        0    12953 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/id.js
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/is.js
+-rw-r--r--   0        0        0    14079 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/it.js
+-rw-r--r--   0        0        0    15353 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ja.js
+-rw-r--r--   0        0        0    21596 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ka.js
+-rw-r--r--   0        0        0    23848 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/km.js
+-rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ko.js
+-rw-r--r--   0        0        0    18533 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ku.js
+-rw-r--r--   0        0        0    13787 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/lt.js
+-rw-r--r--   0        0        0    14013 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/lv.js
+-rw-r--r--   0        0        0    14072 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/mk.js
+-rw-r--r--   0        0        0    16013 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/mn.js
+-rw-r--r--   0        0        0    12801 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ms.js
+-rw-r--r--   0        0        0    12872 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/nb.js
+-rw-r--r--   0        0        0    13274 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/nl.js
+-rw-r--r--   0        0        0    12917 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/no.js
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/oc.js
+-rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/pl.js
+-rw-r--r--   0        0        0    14028 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/pt-br.js
+-rw-r--r--   0        0        0    13937 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/pt.js
+-rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ro.js
+-rw-r--r--   0        0        0    19388 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ru.js
+-rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/si.js
+-rw-r--r--   0        0        0    13968 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sk.js
+-rw-r--r--   0        0        0    13157 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sl.js
+-rw-r--r--   0        0        0    14209 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sq.js
+-rw-r--r--   0        0        0    13226 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sr-latn.js
+-rw-r--r--   0        0        0    18199 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sr.js
+-rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sv.js
+-rw-r--r--   0        0        0    19588 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/th.js
+-rw-r--r--   0        0        0    13898 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/tr.js
+-rw-r--r--   0        0        0    16206 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/tt.js
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ug.js
+-rw-r--r--   0        0        0    19509 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/uk.js
+-rw-r--r--   0        0        0    15078 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/vi.js
+-rw-r--r--   0        0        0    12353 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/zh-cn.js
+-rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/zh.js
+-rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/icons.png
+-rw-r--r--   0        0        0    18632 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/icons_hidpi.png
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/a11yhelp.js
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/_translationstatus.txt
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/af.js
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ar.js
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/az.js
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/bg.js
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ca.js
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/cs.js
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/cy.js
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/da.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/de-ch.js
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/de.js
+-rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/el.js
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/en-au.js
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/en-gb.js
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/en.js
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/eo.js
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/es-mx.js
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/es.js
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/et.js
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/eu.js
+-rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fa.js
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fi.js
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fo.js
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fr-ca.js
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fr.js
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/gl.js
+-rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/gu.js
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/he.js
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/hi.js
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/hr.js
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/hu.js
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/id.js
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/it.js
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ja.js
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/km.js
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ko.js
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ku.js
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/lt.js
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/lv.js
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/mk.js
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/mn.js
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/nb.js
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/nl.js
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/no.js
+-rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/oc.js
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/pl.js
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/pt-br.js
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/pt.js
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ro.js
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ru.js
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/si.js
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sk.js
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sl.js
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sq.js
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sr-latn.js
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sr.js
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sv.js
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/th.js
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/tr.js
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/tt.js
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ug.js
+-rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/uk.js
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/vi.js
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/zh-cn.js
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/zh.js
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/about/dialogs/about.js
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/about/dialogs/logo_ckeditor.png
+-rw-r--r--   0        0        0    12236 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/about/dialogs/hidpi/logo_ckeditor.png
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/clipboard/dialogs/paste.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/dialog/dialogDefinition.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/dialog/styles/dialog.css
+-rw-r--r--   0        0        0    21529 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/image/dialogs/image.js
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/image/images/noimage.png
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/dialogs/anchor.js
+-rw-r--r--   0        0        0    13234 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/dialogs/link.js
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/images/anchor.png
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/images/hidpi/anchor.png
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/magicline/images/icon-rtl.png
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/magicline/images/icon.png
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/magicline/images/hidpi/icon-rtl.png
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/magicline/images/hidpi/icon.png
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastefromgdocs/filter/default.js
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastefromlibreoffice/filter/default.js
+-rw-r--r--   0        0        0    19902 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastefromword/filter/default.js
+-rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastetools/filter/common.js
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastetools/filter/image.js
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/CHANGELOG.md
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/LICENSE.md
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/README.md
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/dialogs/dialog.css
+-rw-r--r--   0        0        0    16136 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/dialogs/options.js
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/dialogs/toolbar.css
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/skins/moono-lisa/scayt.css
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/specialchar.js
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/_translationstatus.txt
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/af.js
+-rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ar.js
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/az.js
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/bg.js
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ca.js
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/cs.js
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/cy.js
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/da.js
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/de-ch.js
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/de.js
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/el.js
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en-au.js
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en-ca.js
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en-gb.js
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en.js
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/eo.js
+-rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/es-mx.js
+-rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/es.js
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/et.js
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/eu.js
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fa.js
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fi.js
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fr-ca.js
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fr.js
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/gl.js
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/he.js
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/hr.js
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/hu.js
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/id.js
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/it.js
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ja.js
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/km.js
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ko.js
+-rw-r--r--   0        0        0     7578 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ku.js
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/lt.js
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/lv.js
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/nb.js
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/nl.js
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/no.js
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/oc.js
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/pl.js
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/pt-br.js
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/pt.js
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ro.js
+-rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ru.js
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/si.js
+-rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sk.js
+-rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sl.js
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sq.js
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sr-latn.js
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sr.js
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sv.js
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/th.js
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/tr.js
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/tt.js
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ug.js
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/uk.js
+-rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/vi.js
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/zh-cn.js
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/zh.js
+-rw-r--r--   0        0        0     9043 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/table/dialogs/table.js
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/tableselection/styles/tableselection.css
+-rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/tabletools/dialogs/tableCell.js
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/widget/images/handle.png
+-rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/index.html
+-rw-r--r--   0        0        0    67340 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/css/samples.css
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/github-top.png
+-rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/header-bg.png
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/header-separator.png
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/logo.png
+-rw-r--r--   0        0        0    10887 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/logo.svg
+-rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/navigation-tip.png
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/js/sample.js
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/js/sf.js
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/ajax.html
+-rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/api.html
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/appendto.html
+-rw-r--r--   0        0        0    47840 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/datafiltering.html
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/divreplace.html
+-rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/index.html
+-rw-r--r--   0        0        0    10399 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/inlineall.html
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/inlinebycode.html
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/inlinetextarea.html
+-rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/jquery.html
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/readonly.html
+-rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/replacebyclass.html
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/replacebycode.html
+-rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/sample.css
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/sample.js
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/sample_posteddata.php
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/tabindex.html
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/uicolor.html
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/uilanguages.html
+-rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/xhtmlstyle.html
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/posteddata.php
+-rw-r--r--   0        0        0    14449 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/sample.jpg
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/inlineall/logo.png
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/outputxhtml/outputxhtml.css
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/uilanguages/languages.js
+-rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/dialog/dialog.html
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/dialog/assets/my_dialog.js
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/enterkey/enterkey.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/htmlwriter/outputhtml.html
+-rw-r--r--   0        0        0     8585 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/magicline/magicline.html
+-rw-r--r--   0        0        0     9122 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/toolbar/toolbar.html
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/wysiwygarea/fullpage.html
+-rw-r--r--   0        0        0    15808 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/index.html
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/css/fontello.css
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/LICENSE.txt
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/config.json
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.eot
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.svg
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.ttf
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.woff
+-rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/abstracttoolbarmodifier.js
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/fulltoolbareditor.js
+-rw-r--r--   0        0        0    16651 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/toolbarmodifier.js
+-rw-r--r--   0        0        0     6850 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/toolbartextmodifier.js
+-rw-r--r--   0        0        0    13634 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog.css
+-rw-r--r--   0        0        0    14657 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog_ie.css
+-rw-r--r--   0        0        0    15206 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog_ie8.css
+-rw-r--r--   0        0        0    14686 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog_iequirks.css
+-rw-r--r--   0        0        0    35906 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor.css
+-rw-r--r--   0        0        0    35987 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_gecko.css
+-rw-r--r--   0        0        0    36905 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_ie.css
+-rw-r--r--   0        0        0    37711 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_ie8.css
+-rw-r--r--   0        0        0    37554 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_iequirks.css
+-rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/icons.png
+-rw-r--r--   0        0        0    18632 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/icons_hidpi.png
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/readme.md
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/arrow.png
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/close.png
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/lock-open.png
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/lock.png
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/refresh.png
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/spinner.gif
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/close.png
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/lock-open.png
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/lock.png
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/refresh.png
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/vendor/promise.js
+-rw-r--r--   0        0        0   116891 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsdialog/plugin.js
+-rw-r--r--   0        0        0    23630 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsplugins/plugin.js
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsplugins/icons/cmsplugins.svg
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsresize/plugin.js
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmswidget/plugin.js
+-rw-r--r--   0        0        0   898878 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/djangocms_text/bundles/bundle.ckeditor4.min.js
+-rw-r--r--   0        0        0  1099251 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/djangocms_text/bundles/bundle.ckeditor4.min.js.map
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/djangocms_text/css/bundle.ckeditor4.min.css
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/djangocms_text/css/bundle.ckeditor4.min.css.map
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor5/__init__.py
+-rw-r--r--   0        0        0  4535961 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor5/static/djangocms_text/bundles/bundle.ckeditor5.min.js
+-rw-r--r--   0        0        0  5445187 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor5/static/djangocms_text/bundles/bundle.ckeditor5.min.js.map
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor5/static/djangocms_text/css/cms.ckeditor5.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_quill/__init__.py
+-rw-r--r--   0        0        0   448362 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_quill/static/djangocms_text/bundles/bundle.quill.min.js
+-rw-r--r--   0        0        0   531953 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_quill/static/djangocms_text/bundles/bundle.quill.min.js.map
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_quill/static/djangocms_text/css/cms.quill.css
+-rw-r--r--   0        0        0    26009 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/bubble.css
+-rw-r--r--   0        0        0    25223 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/quill.bubble.css
+-rw-r--r--   0        0        0    10236 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/quill.core.css
+-rw-r--r--   0        0        0    24613 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/quill.snow.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_tinymce/__init__.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_tinymce/static/djangocms_text/bundles/bundle.tinymce.min.js
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_tinymce/static/djangocms_text/bundles/bundle.tinymce.min.js.map
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/contrib/text_tinymce/static/djangocms_text/css/cms.tinymce.css
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/bn/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/da/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/et/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/eu/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/gl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/hi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/hr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/hu/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/is/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/lt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/no/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/migrations/0001_initial.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/migrations/0002_text_json_text_rte.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/migrations/__init__.py
+-rw-r--r--   0        0        0    19802 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/bundles/bundle.editor.min.js
+-rw-r--r--   0        0        0    23204 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/bundles/bundle.editor.min.js.map
+-rw-r--r--   0        0        0  1039837 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/bundles/bundle.tiptap.min.js
+-rw-r--r--   0        0        0  1265764 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/bundles/bundle.tiptap.min.js.map
+-rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/css/bundle.tiptap.min.css
+-rw-r--r--   0        0        0    18096 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/css/bundle.tiptap.min.css.map
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/css/cms.ckeditor4.css
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/css/cms.normalize.css
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/css/cms.text.css
+-rw-r--r--   0        0        0   890296 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/js/ckeditor4.js
+-rw-r--r--   0        0        0  1084627 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/js/ckeditor4.js.map
+-rw-r--r--   0        0        0    13818 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/js/editor.js.map
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/config.js
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/contents.css
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/styles.js
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/adapters/jquery.js
+-rw-r--r--   0        0        0    17242 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/af.js
+-rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ar.js
+-rw-r--r--   0        0        0    19066 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/az.js
+-rw-r--r--   0        0        0    26179 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/bg.js
+-rw-r--r--   0        0        0    22656 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/bn.js
+-rw-r--r--   0        0        0    17291 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/bs.js
+-rw-r--r--   0        0        0    18989 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ca.js
+-rw-r--r--   0        0        0    19007 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/cs.js
+-rw-r--r--   0        0        0    17696 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/cy.js
+-rw-r--r--   0        0        0    18066 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/da.js
+-rw-r--r--   0        0        0    18861 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/de-ch.js
+-rw-r--r--   0        0        0    18839 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/de.js
+-rw-r--r--   0        0        0    28070 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/el.js
+-rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en-au.js
+-rw-r--r--   0        0        0    17192 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en-ca.js
+-rw-r--r--   0        0        0    17217 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en-gb.js
+-rw-r--r--   0        0        0    17207 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en.js
+-rw-r--r--   0        0        0    18418 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/eo.js
+-rw-r--r--   0        0        0    19675 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/es-mx.js
+-rw-r--r--   0        0        0    19174 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/es.js
+-rw-r--r--   0        0        0    17828 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/et.js
+-rw-r--r--   0        0        0    18860 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/eu.js
+-rw-r--r--   0        0        0    23657 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fa.js
+-rw-r--r--   0        0        0    18273 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fi.js
+-rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fo.js
+-rw-r--r--   0        0        0    18774 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fr-ca.js
+-rw-r--r--   0        0        0    19665 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fr.js
+-rw-r--r--   0        0        0    19221 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/gl.js
+-rw-r--r--   0        0        0    28283 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/gu.js
+-rw-r--r--   0        0        0    21259 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/he.js
+-rw-r--r--   0        0        0    23097 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/hi.js
+-rw-r--r--   0        0        0    17804 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/hr.js
+-rw-r--r--   0        0        0    19372 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/hu.js
+-rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/id.js
+-rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/is.js
+-rw-r--r--   0        0        0    19072 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/it.js
+-rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ja.js
+-rw-r--r--   0        0        0    30679 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ka.js
+-rw-r--r--   0        0        0    31712 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/km.js
+-rw-r--r--   0        0        0    18627 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ko.js
+-rw-r--r--   0        0        0    25736 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ku.js
+-rw-r--r--   0        0        0    18928 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/lt.js
+-rw-r--r--   0        0        0    19144 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/lv.js
+-rw-r--r--   0        0        0    18944 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/mk.js
+-rw-r--r--   0        0        0    21951 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/mn.js
+-rw-r--r--   0        0        0    17496 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ms.js
+-rw-r--r--   0        0        0    17594 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/nb.js
+-rw-r--r--   0        0        0    18213 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/nl.js
+-rw-r--r--   0        0        0    17615 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/no.js
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/oc.js
+-rw-r--r--   0        0        0    19199 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/pl.js
+-rw-r--r--   0        0        0    19239 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/pt-br.js
+-rw-r--r--   0        0        0    19110 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/pt.js
+-rw-r--r--   0        0        0    19938 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ro.js
+-rw-r--r--   0        0        0    27017 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ru.js
+-rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/si.js
+-rw-r--r--   0        0        0    19290 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sk.js
+-rw-r--r--   0        0        0    17995 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sl.js
+-rw-r--r--   0        0        0    19705 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sq.js
+-rw-r--r--   0        0        0    18158 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sr-latn.js
+-rw-r--r--   0        0        0    25230 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sr.js
+-rw-r--r--   0        0        0    17749 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sv.js
+-rw-r--r--   0        0        0    26591 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/th.js
+-rw-r--r--   0        0        0    18840 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/tr.js
+-rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/tt.js
+-rw-r--r--   0        0        0    25273 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ug.js
+-rw-r--r--   0        0        0    27018 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/uk.js
+-rw-r--r--   0        0        0    20670 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/vi.js
+-rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/zh-cn.js
+-rw-r--r--   0        0        0    16747 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/zh.js
+-rw-r--r--   0        0        0    11937 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/icons.png
+-rw-r--r--   0        0        0    37595 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/icons_hidpi.png
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/a11yhelp.js
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/_translationstatus.txt
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/af.js
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ar.js
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/az.js
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/bg.js
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ca.js
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/cs.js
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/cy.js
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/da.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/de-ch.js
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/de.js
+-rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/el.js
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/en-au.js
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/en-gb.js
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/en.js
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/eo.js
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/es-mx.js
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/es.js
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/et.js
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/eu.js
+-rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fa.js
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fi.js
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fo.js
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fr-ca.js
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fr.js
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/gl.js
+-rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/gu.js
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/he.js
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/hi.js
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/hr.js
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/hu.js
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/id.js
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/it.js
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ja.js
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/km.js
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ko.js
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ku.js
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/lt.js
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/lv.js
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/mk.js
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/mn.js
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/nb.js
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/nl.js
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/no.js
+-rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/oc.js
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/pl.js
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/pt-br.js
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/pt.js
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ro.js
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ru.js
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/si.js
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sk.js
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sl.js
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sq.js
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sr-latn.js
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sr.js
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sv.js
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/th.js
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/tr.js
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/tt.js
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ug.js
+-rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/uk.js
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/vi.js
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/zh-cn.js
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/zh.js
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/about/dialogs/about.js
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/about/dialogs/logo_ckeditor.png
+-rw-r--r--   0        0        0    12236 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/about/dialogs/hidpi/logo_ckeditor.png
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/clipboard/dialogs/paste.js
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/colordialog/dialogs/colordialog.css
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/colordialog/dialogs/colordialog.js
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/copyformatting/cursors/cursor-disabled.svg
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/copyformatting/cursors/cursor.svg
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/copyformatting/styles/copyformatting.css
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/dialog/dialogDefinition.js
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/dialog/styles/dialog.css
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/div/dialogs/div.js
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/CHANGELOG.md
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/LICENSE.md
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/README.md
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/plugindefinition.js
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/authentication.js
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/exportpdf.js
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/notification.js
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/resourcespaths.js
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/statistics.js
+-rw-r--r--   0        0        0     9882 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/stylesheets.js
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/_helpers/tools.js
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/configfilename.html
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/configfilename.md
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/emptyeditor.html
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/emptyeditor.md
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integration.html
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integration.md
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notifications.html
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notifications.md
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notificationsasync.html
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notificationsasync.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/paperformat.html
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/paperformat.md
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/readonly.html
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/readonly.md
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/stylesheets.html
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/stylesheets.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenfetching.html
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenfetching.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.html
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.md
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokentwoeditorswrong.html
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokentwoeditorswrong.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenwithouturl.html
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenwithouturl.md
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/wrongendpoint.html
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/wrongendpoint.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integrations/easyimage.html
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integrations/easyimage.md
+-rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/find/dialogs/find.js
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/button.js
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/checkbox.js
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/form.js
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/hiddenfield.js
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/radio.js
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/select.js
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/textarea.js
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/textfield.js
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/images/hiddenfield.gif
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/iframe/dialogs/iframe.js
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/iframe/images/placeholder.png
+-rw-r--r--   0        0        0    21529 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/image/dialogs/image.js
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/image/images/noimage.png
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/dialogs/anchor.js
+-rw-r--r--   0        0        0    13234 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/dialogs/link.js
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/images/anchor.png
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/images/hidpi/anchor.png
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/liststyle/dialogs/liststyle.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/magicline/images/icon-rtl.png
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/magicline/images/icon.png
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/magicline/images/hidpi/icon-rtl.png
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/magicline/images/hidpi/icon.png
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pagebreak/images/pagebreak.gif
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastefromgdocs/filter/default.js
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastefromlibreoffice/filter/default.js
+-rw-r--r--   0        0        0    19568 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastefromword/filter/default.js
+-rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastetools/filter/common.js
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastetools/filter/image.js
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/preview/preview.html
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/preview/images/pagebreak.gif
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/preview/styles/screen.css
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/CHANGELOG.md
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/LICENSE.md
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/README.md
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/dialogs/dialog.css
+-rw-r--r--   0        0        0    16136 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/dialogs/options.js
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/dialogs/toolbar.css
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/skins/moono-lisa/scayt.css
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_address.png
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_blockquote.png
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_div.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_h1.png
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_h2.png
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_h3.png
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_h4.png
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_h5.png
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_h6.png
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_p.png
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/showblocks/images/block_pre.png
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/dialogs/smiley.js
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angel_smile.gif
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angel_smile.png
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angry_smile.gif
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angry_smile.png
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/broken_heart.gif
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/broken_heart.png
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/confused_smile.gif
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/confused_smile.png
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/cry_smile.gif
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/cry_smile.png
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/devil_smile.gif
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/devil_smile.png
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/embaressed_smile.gif
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/embarrassed_smile.gif
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/embarrassed_smile.png
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/envelope.gif
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/envelope.png
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/heart.gif
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/heart.png
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/kiss.gif
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/kiss.png
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/lightbulb.gif
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/lightbulb.png
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/omg_smile.gif
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/omg_smile.png
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/regular_smile.gif
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/regular_smile.png
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/sad_smile.gif
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/sad_smile.png
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/shades_smile.gif
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/shades_smile.png
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/teeth_smile.gif
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/teeth_smile.png
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_down.gif
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_down.png
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_up.gif
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_up.png
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/tongue_smile.gif
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/tongue_smile.png
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/tounge_smile.gif
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/whatchutalkingabout_smile.gif
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/whatchutalkingabout_smile.png
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/wink_smile.gif
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/wink_smile.png
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/specialchar.js
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/_translationstatus.txt
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/af.js
+-rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ar.js
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/az.js
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/bg.js
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ca.js
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/cs.js
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/cy.js
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/da.js
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/de-ch.js
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/de.js
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/el.js
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en-au.js
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en-ca.js
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en-gb.js
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en.js
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/eo.js
+-rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/es-mx.js
+-rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/es.js
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/et.js
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/eu.js
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fa.js
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fi.js
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fr-ca.js
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fr.js
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/gl.js
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/he.js
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/hr.js
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/hu.js
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/id.js
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/it.js
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ja.js
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/km.js
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ko.js
+-rw-r--r--   0        0        0     7578 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ku.js
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/lt.js
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/lv.js
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/nb.js
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/nl.js
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/no.js
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/oc.js
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/pl.js
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/pt-br.js
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/pt.js
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ro.js
+-rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ru.js
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/si.js
+-rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sk.js
+-rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sl.js
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sq.js
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sr-latn.js
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sr.js
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sv.js
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/th.js
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/tr.js
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/tt.js
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ug.js
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/uk.js
+-rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/vi.js
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/zh-cn.js
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/zh.js
+-rw-r--r--   0        0        0     9043 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/table/dialogs/table.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/tableselection/styles/tableselection.css
+-rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/tabletools/dialogs/tableCell.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templatedefinition.js
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/dialogs/templates.css
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/dialogs/templates.js
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/default.js
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/images/template1.gif
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/images/template2.gif
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/images/template3.gif
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/widget/images/handle.png
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/LICENSE.md
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/README.md
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/ciframe.html
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/tmpFrameset.html
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/wsc.css
+-rw-r--r--   0        0        0    47292 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/wsc.js
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/wsc_ie.js
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/skins/moono-lisa/wsc.css
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog.css
+-rw-r--r--   0        0        0    15866 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog_ie.css
+-rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog_ie8.css
+-rw-r--r--   0        0        0    15895 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog_iequirks.css
+-rw-r--r--   0        0        0    24410 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor.css
+-rw-r--r--   0        0        0    24491 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_gecko.css
+-rw-r--r--   0        0        0    25409 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_ie.css
+-rw-r--r--   0        0        0    26258 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_ie8.css
+-rw-r--r--   0        0        0    26058 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_iequirks.css
+-rw-r--r--   0        0        0    11937 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/icons.png
+-rw-r--r--   0        0        0    37595 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/icons_hidpi.png
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/readme.md
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/arrow.png
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/close.png
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/lock-open.png
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/lock.png
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/refresh.png
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/spinner.gif
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/close.png
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/lock-open.png
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/lock.png
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/refresh.png
+-rw-r--r--   0        0        0    20702 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text_ckeditor/js/cms.ckeditor.js
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text_ckeditor/js/post.js
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/static/djangocms_text_ckeditor/js/pre.js
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/templates/cms/plugins/inline.html
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/templates/cms/plugins/render_plugin_preview.html
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/templates/cms/plugins/text.html
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/templates/cms/plugins/text_plugin_change_formx.html
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/templates/cms/plugins/widgets/ckeditor.html
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/templates/cms/plugins/widgets/editor.html
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/templates/cms/toolbar/icon-button.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/templatetags/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text/templatetags/djangocms_text_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text_ckeditor/__init__.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text_ckeditor/fields.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/djangocms_text_ckeditor/widgets.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/LICENSE
+-rw-r--r--   0        0        0    28588 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/README.rst
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    30095 2020-02-02 00:00:00.000000 djangocms_text-0.1.1/PKG-INFO
```

### Comparing `djangocms_text-0.1.0/djangocms_text/__init__.py` & `djangocms_text-0.1.1/djangocms_text/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 See PEP 440 (https://www.python.org/dev/peps/pep-0440/)
 
 Release logic:
  1. Increase version number (change __version__ below).
- 2. Ensure the static bundle is upto date with ``nvm use && gulp bundle``
- 3. Assure that all changes have been documented in CHANGELOG.rst.
- 4. In setup.py check that
+ 2. Assure that all changes have been documented in CHANGELOG.rst.
+ 3. In setup.py check that
    - versions from all third party packages are pinned in ``REQUIREMENTS``.
    - the list of ``CLASSIFIERS`` is up to date.
- 5. git add djangocms_text_ckeditor/__init__.py CHANGELOG.rst setup.py
- 6. git commit -m 'Bump to {new version}'
- 7. git push
- 8. Assure that all tests pass on https://github.com/django-cms/djangocms-text-ckeditor/actions
- 9. Create a new release on https://github.com/django-cms/djangocms-text-ckeditor/releases/new
-10. Publish the release when ready
-11. Github actions will publish the new package to pypi
+ 4. git add djangocms_text_ckeditor/__init__.py CHANGELOG.rst setup.py
+ 5. git commit -m 'Bump to {new version}'
+ 6. git push
+ 7. Assure that all tests pass on https://github.com/django-cms/djangocms-text-ckeditor/actions
+ 8. Create a new release on https://github.com/django-cms/djangocms-text-ckeditor/releases/new
+ 9. Publish the release when ready
+10. Github actions will publish the new package to pypi
 """
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

### Comparing `djangocms_text-0.1.0/djangocms_text/apps.py` & `djangocms_text-0.1.1/djangocms_text/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/cms_plugins.py` & `djangocms_text-0.1.1/djangocms_text/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/cms_toolbars.py` & `djangocms_text-0.1.1/djangocms_text/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/editors.py` & `djangocms_text-0.1.1/djangocms_text/editors.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,15 @@
         + '   viewBox="0 0 16 16"  xmlns="http://www.w3.org/2000/svg">'
         + '  <path d="m 10.660156,1.96875 a 3.0002541,3.0002541 0 0 0 -2.2460935,0.875 l -1.015625,1.015625 0.7050781,0.7070312 1.015625,-1.015625 A 2.0011676,2.0011676 0 1 1 11.949219,6.3808594 L 11.15625,7.171875 c 0.04831,0.1811506 0.08077,0.3654706 0.103516,0.5507812 l 0.380859,0.3808594 1.015625,-1.015625 A 3.0002541,3.0002541 0 0 0 10.660156,1.96875 Z M 3.8613281,7.3964844 3.34375,7.9140625 A 3.0002541,3.0002541 0 1 0 7.5859375,12.15625 l 0.515625,-0.515625 C 7.8663008,11.405107 7.6295925,11.171326 7.3945312,10.935547 L 6.8808594,11.449219 A 2.0011676,2.0011676 0 0 1 4.0507812,8.6191406 L 4.5683594,8.1035156 C 4.3326823,7.8675541 4.0973009,7.6320603 3.8613281,7.3964844 Z" />\n'
         + '  <path fill-rule="evenodd" d="m 13.718276,13.311496 a 0.5,0.5 0 0 1 -0.708,0 L 2.0102757,2.3114959 a 0.5006316,0.5006316 0 0 1 0.708,-0.708 L 13.718276,12.603496 a 0.5,0.5 0 0 1 0,0.708" />'
         + "</svg>",
     },
     "Table": {
         "title": _("Table"),
+        "icon": '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-table" viewBox="0 0 16 16"><path d="M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2zm15 2h-4v3h4zm0 4h-4v3h4zm0 4h-4v3h3a1 1 0 0 0 1-1zm-5 3v-3H6v3zm-5 0v-3H1v2a1 1 0 0 0 1 1zm-4-4h4V8H1zm0-4h4V4H1zm5-3v3h4V4zm4 4H6v3h4z"/></svg>',
     },
     "Code": {
         "title": _("Code"),
         "icon": '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-code" viewBox="0 0 16 16">\n'
         + '  <path d="M5.854 4.854a.5.5 0 1 0-.708-.708l-3.5 3.5a.5.5 0 0 0 0 .708l3.5 3.5a.5.5 0 0 0 .708-.708L2.707 8zm4.292 0a.5.5 0 0 1 .708-.708l3.5 3.5a.5.5 0 0 1 0 .708l-3.5 3.5a.5.5 0 0 1-.708-.708L13.293 8z"/>\n'
         + "</svg>",
     },
@@ -357,15 +358,15 @@
         "-",
         "RemoveFormat",
     ],
     ["JustifyLeft", "JustifyCenter", "JustifyRight", "JustifyBlock"],
     ["Link", "Unlink"],
     ["NumberedList", "BulletedList"],
     ["HorizontalRule", "CodeBlock"],
-    ["Outdent", "Indent", "-", "Blockquote", "-", "Link", "Unlink", "-", "Table"],
+    ["Outdent", "Indent", "-", "Blockquote", "-", "Table"],
     ["Source"],
 ]
 
 
 class RTEConfig:
     """
     Initializes an instance of RTEConfig.
```

### Comparing `djangocms_text-0.1.0/djangocms_text/fields.py` & `djangocms_text-0.1.1/djangocms_text/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/forms.py` & `djangocms_text-0.1.1/djangocms_text/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/html.py` & `djangocms_text-0.1.1/djangocms_text/html.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/models.py` & `djangocms_text-0.1.1/djangocms_text/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/settings.py` & `djangocms_text-0.1.1/djangocms_text/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/utils.py` & `djangocms_text-0.1.1/djangocms_text/utils.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/widgets.py` & `djangocms_text-0.1.1/djangocms_text/widgets.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/CHANGES.md` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/CHANGES.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/LICENSE.md` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/LICENSE.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/README.md` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/SECURITY.md` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/SECURITY.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/build-config.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/build-config.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/ckeditor.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/ckeditor.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/contents.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/contents.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/styles.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/styles.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/adapters/jquery.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/adapters/jquery.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/af.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/af.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ar.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ar.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/az.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/az.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/bg.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/bg.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/bn.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/bn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/bs.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/bs.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ca.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/cs.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/cs.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/cy.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/cy.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/da.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/da.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/de-ch.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/de.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/de.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/el.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/el.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en-au.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en-ca.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en-ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en-gb.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/en.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/eo.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/eo.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/es-mx.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/es-mx.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/es.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/es.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/et.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/et.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/eu.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/eu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fa.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fa.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fi.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fo.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fo.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fr-ca.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fr.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/fr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/gl.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/gl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/gu.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/gu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/he.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/he.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/hi.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/hi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/hr.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/hr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/hu.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/hu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/id.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/id.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/is.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/is.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/it.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/it.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ja.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ja.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ka.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ka.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/km.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/km.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ko.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ko.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ku.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ku.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/lt.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/lt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/lv.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/lv.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/mk.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/mk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/mn.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/mn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ms.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ms.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/nb.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/nb.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/nl.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/nl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/no.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/no.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/oc.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/oc.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/pl.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/pl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/pt-br.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/pt.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/pt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ro.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ro.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ru.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ru.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/si.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/si.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sk.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sl.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sq.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sq.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sr-latn.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sr.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sv.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/sv.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/th.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/th.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/tr.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/tr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/tt.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/tt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ug.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/ug.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/uk.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/uk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/vi.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/vi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/zh-cn.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/zh.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/lang/zh.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/icons.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/icons.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/icons_hidpi.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/a11yhelp.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/a11yhelp.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/_translationstatus.txt` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/_translationstatus.txt`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/af.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/af.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ar.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/az.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/az.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/bg.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ca.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/cs.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/cy.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/da.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/da.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/de-ch.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/de.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/de.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/el.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/el.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/en-au.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/en-gb.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/en.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/en.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/eo.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/eo.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/es-mx.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/es-mx.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/es.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/es.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/et.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/et.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/eu.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/eu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fa.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fi.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fo.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fo.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fr-ca.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fr.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/gl.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/gu.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/gu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/he.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/he.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/hi.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/hi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/hr.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/hu.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/id.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/id.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/it.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/it.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ja.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/km.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/km.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ko.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ku.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ku.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/lt.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/lt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/lv.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/lv.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/mk.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/mk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/mn.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/mn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/nb.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/nl.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/no.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/no.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/oc.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/pl.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/pt-br.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/pt.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/pt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ro.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ro.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ru.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/si.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/si.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sk.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sl.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sq.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sq.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sr-latn.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sr.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sv.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/th.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/th.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/tr.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/tt.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/tt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ug.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/ug.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/uk.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/vi.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/zh-cn.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/zh.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/a11yhelp/dialogs/lang/zh.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/about/dialogs/about.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/about/dialogs/about.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/about/dialogs/logo_ckeditor.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/about/dialogs/logo_ckeditor.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/about/dialogs/hidpi/logo_ckeditor.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/about/dialogs/hidpi/logo_ckeditor.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/clipboard/dialogs/paste.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/clipboard/dialogs/paste.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/image/dialogs/image.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/image/dialogs/image.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/image/images/noimage.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/image/images/noimage.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/dialogs/anchor.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/dialogs/anchor.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/dialogs/link.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/dialogs/link.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/images/anchor.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/images/anchor.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/images/hidpi/anchor.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/link/images/hidpi/anchor.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastefromgdocs/filter/default.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastefromgdocs/filter/default.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastefromlibreoffice/filter/default.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastefromlibreoffice/filter/default.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastefromword/filter/default.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastefromword/filter/default.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastetools/filter/common.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastetools/filter/common.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastetools/filter/image.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/pastetools/filter/image.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/LICENSE.md` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/LICENSE.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/README.md` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/dialogs/options.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/dialogs/options.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/dialogs/toolbar.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/scayt/dialogs/toolbar.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/specialchar.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/specialchar.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/_translationstatus.txt` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/_translationstatus.txt`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/af.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/af.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ar.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/az.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/az.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/bg.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ca.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/cs.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/cy.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/da.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/da.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/de-ch.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/de.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/de.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/el.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/el.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en-au.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en-ca.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en-ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en-gb.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/en.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/eo.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/eo.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/es-mx.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/es-mx.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/es.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/es.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/et.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/et.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/eu.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/eu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fa.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fi.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fr-ca.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fr.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/gl.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/he.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/he.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/hr.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/hu.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/id.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/id.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/it.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/it.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ja.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/km.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/km.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ko.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ku.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ku.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/lt.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/lt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/lv.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/lv.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/nb.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/nl.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/no.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/no.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/oc.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/pl.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/pt-br.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/pt.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/pt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ro.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ro.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ru.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/si.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/si.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sk.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sl.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sq.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sq.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sr-latn.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sr.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sv.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/th.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/th.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/tr.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/tt.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/tt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ug.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/ug.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/uk.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/vi.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/zh-cn.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/zh.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/specialchar/dialogs/lang/zh.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/table/dialogs/table.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/table/dialogs/table.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/tableselection/styles/tableselection.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/tableselection/styles/tableselection.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/tabletools/dialogs/tableCell.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/plugins/tabletools/dialogs/tableCell.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/index.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/index.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/css/samples.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/css/samples.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/header-bg.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/header-bg.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/logo.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/logo.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/logo.svg` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/logo.svg`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/navigation-tip.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/img/navigation-tip.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/js/sample.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/js/sample.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/js/sf.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/js/sf.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/ajax.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/ajax.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/api.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/api.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/appendto.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/appendto.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/datafiltering.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/datafiltering.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/divreplace.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/divreplace.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/index.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/index.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/inlineall.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/inlineall.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/inlinebycode.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/inlinebycode.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/inlinetextarea.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/inlinetextarea.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/jquery.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/jquery.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/readonly.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/readonly.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/replacebyclass.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/replacebyclass.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/replacebycode.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/replacebycode.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/sample.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/sample.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/sample.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/sample.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/sample_posteddata.php` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/sample_posteddata.php`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/tabindex.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/tabindex.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/uicolor.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/uicolor.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/uilanguages.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/uilanguages.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/xhtmlstyle.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/xhtmlstyle.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/posteddata.php` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/posteddata.php`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/sample.jpg` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/sample.jpg`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/inlineall/logo.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/inlineall/logo.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/outputxhtml/outputxhtml.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/outputxhtml/outputxhtml.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/uilanguages/languages.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/assets/uilanguages/languages.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/dialog/dialog.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/dialog/dialog.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/dialog/assets/my_dialog.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/dialog/assets/my_dialog.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/enterkey/enterkey.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/enterkey/enterkey.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/htmlwriter/outputhtml.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/htmlwriter/outputhtml.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/magicline/magicline.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/magicline/magicline.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/toolbar/toolbar.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/toolbar/toolbar.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/wysiwygarea/fullpage.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/old/wysiwygarea/fullpage.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/index.html` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/index.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/css/fontello.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/css/fontello.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/config.json` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/config.json`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.eot` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.eot`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.svg` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.svg`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.ttf` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.woff` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/font/fontello.woff`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/abstracttoolbarmodifier.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/abstracttoolbarmodifier.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/fulltoolbareditor.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/fulltoolbareditor.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/toolbarmodifier.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/toolbarmodifier.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/toolbartextmodifier.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/samples/toolbarconfigurator/js/toolbartextmodifier.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog_ie.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog_ie.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog_ie8.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog_ie8.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog_iequirks.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/dialog_iequirks.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_gecko.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_gecko.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_ie.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_ie.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_ie8.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_ie8.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_iequirks.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/editor_iequirks.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/icons.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/icons.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/icons_hidpi.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/readme.md` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/readme.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/close.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/close.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/refresh.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/refresh.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/spinner.gif` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/close.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/close.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/lock-open.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/lock-open.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/lock.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/lock.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/refresh.png` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/skins/moono-lisa/images/hidpi/refresh.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor/vendor/promise.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor/vendor/promise.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsdialog/plugin.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsdialog/plugin.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsplugins/plugin.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsplugins/plugin.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsplugins/icons/cmsplugins.svg` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsplugins/icons/cmsplugins.svg`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsresize/plugin.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmsresize/plugin.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmswidget/plugin.js` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor4/static/ckeditor_plugins/cmswidget/plugin.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_ckeditor5/static/djangocms_text/css/cms.ckeditor5.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_ckeditor5/static/djangocms_text/css/cms.ckeditor5.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/bubble.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/bubble.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/quill.bubble.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/quill.bubble.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/quill.core.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/quill.core.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/quill.snow.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_quill/static/djangocms_text/vendor/quill/quill.snow.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/contrib/text_tinymce/static/djangocms_text/css/cms.tinymce.css` & `djangocms_text-0.1.1/djangocms_text/contrib/text_tinymce/static/djangocms_text/css/cms.tinymce.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/ar/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/bn/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/bn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/ca/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/cs/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/da/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/de/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/el/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/en/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/es/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/et/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/eu/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/fa/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/fi/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/fr/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/gl/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/he/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/hi/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/hr/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/hu/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/is/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/it/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/ja/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/lt/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/nl/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/no/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/no/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/pl/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/pt/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/ro/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/ru/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/sv/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/tr/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/uk/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/locale/zh_CN/LC_MESSAGES/django.po` & `djangocms_text-0.1.1/djangocms_text/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/migrations/0001_initial.py` & `djangocms_text-0.1.1/djangocms_text/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/migrations/0002_text_json_text_rte.py` & `djangocms_text-0.1.1/djangocms_text/migrations/0002_text_json_text_rte.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/css/cms.ckeditor4.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/css/cms.ckeditor4.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/css/cms.normalize.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/css/cms.normalize.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/js/ckeditor4.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/js/ckeditor4.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/js/ckeditor4.js.map` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/js/ckeditor4.js.map`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/js/editor.js.map` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/js/editor.js.map`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/contents.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/contents.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/styles.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/styles.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/adapters/jquery.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/adapters/jquery.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/af.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/af.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ar.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ar.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/az.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/az.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/bg.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/bg.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/bn.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/bn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/bs.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/bs.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ca.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/cs.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/cs.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/cy.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/cy.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/da.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/da.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/de-ch.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/de.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/de.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/el.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/el.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en-au.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en-ca.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en-ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en-gb.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/en.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/eo.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/eo.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/es-mx.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/es-mx.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/es.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/es.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/et.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/et.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/eu.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/eu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fa.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fa.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fi.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fo.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fo.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fr-ca.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fr.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/fr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/gl.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/gl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/gu.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/gu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/he.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/he.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/hi.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/hi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/hr.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/hr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/hu.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/hu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/id.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/id.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/is.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/is.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/it.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/it.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ja.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ja.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ka.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ka.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/km.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/km.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ko.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ko.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ku.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ku.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/lt.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/lt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/lv.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/lv.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/mk.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/mk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/mn.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/mn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ms.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ms.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/nb.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/nb.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/nl.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/nl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/no.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/no.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/oc.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/oc.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/pl.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/pl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/pt-br.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/pt.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/pt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ro.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ro.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ru.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ru.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/si.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/si.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sk.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sl.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sq.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sq.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sr-latn.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sr.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sv.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/sv.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/th.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/th.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/tr.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/tr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/tt.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/tt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ug.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/ug.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/uk.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/uk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/vi.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/vi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/zh-cn.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/zh.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/lang/zh.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/icons.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/icons.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/icons_hidpi.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/a11yhelp.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/a11yhelp.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/_translationstatus.txt` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/_translationstatus.txt`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/af.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/af.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ar.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/az.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/az.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/bg.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ca.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/cs.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/cy.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/da.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/da.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/de-ch.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/de.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/de.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/el.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/el.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/en-au.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/en-gb.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/en.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/en.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/eo.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/eo.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/es-mx.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/es-mx.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/es.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/es.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/et.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/et.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/eu.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/eu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fa.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fi.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fo.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fo.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fr-ca.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fr.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/gl.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/gu.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/gu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/he.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/he.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/hi.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/hi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/hr.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/hu.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/id.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/id.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/it.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/it.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ja.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/km.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/km.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ko.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ku.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ku.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/lt.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/lt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/lv.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/lv.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/mk.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/mk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/mn.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/mn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/nb.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/nl.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/no.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/no.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/oc.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/pl.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/pt-br.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/pt.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/pt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ro.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ro.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ru.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/si.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/si.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sk.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sl.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sq.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sq.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sr-latn.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sr.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sv.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/th.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/th.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/tr.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/tt.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/tt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ug.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/ug.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/uk.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/vi.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/zh-cn.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/zh.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/a11yhelp/dialogs/lang/zh.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/about/dialogs/about.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/about/dialogs/about.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/about/dialogs/logo_ckeditor.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/about/dialogs/logo_ckeditor.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/about/dialogs/hidpi/logo_ckeditor.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/about/dialogs/hidpi/logo_ckeditor.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/clipboard/dialogs/paste.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/clipboard/dialogs/paste.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/colordialog/dialogs/colordialog.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/colordialog/dialogs/colordialog.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/colordialog/dialogs/colordialog.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/colordialog/dialogs/colordialog.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/copyformatting/cursors/cursor-disabled.svg` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/copyformatting/cursors/cursor-disabled.svg`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/copyformatting/cursors/cursor.svg` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/copyformatting/cursors/cursor.svg`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/copyformatting/styles/copyformatting.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/copyformatting/styles/copyformatting.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/div/dialogs/div.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/div/dialogs/div.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/CHANGELOG.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/LICENSE.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/LICENSE.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/README.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/authentication.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/authentication.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/exportpdf.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/exportpdf.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/notification.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/notification.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/resourcespaths.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/resourcespaths.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/statistics.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/statistics.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/stylesheets.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/stylesheets.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/_helpers/tools.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/_helpers/tools.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/configfilename.html` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/configfilename.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/configfilename.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/configfilename.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/emptyeditor.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/emptyeditor.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integration.html` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integration.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integration.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integration.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notifications.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notifications.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notificationsasync.html` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notificationsasync.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notificationsasync.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/notificationsasync.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/paperformat.html` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/paperformat.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/paperformat.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/paperformat.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/readonly.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/readonly.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/stylesheets.html` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/stylesheets.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/stylesheets.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/stylesheets.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenfetching.html` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenfetching.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenfetching.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenfetching.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.html` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokentwoeditorswrong.html` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokentwoeditorswrong.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenwithouturl.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/tokenwithouturl.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/wrongendpoint.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/wrongendpoint.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integrations/easyimage.html` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integrations/easyimage.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integrations/easyimage.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/exportpdf/tests/manual/integrations/easyimage.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/find/dialogs/find.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/find/dialogs/find.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/button.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/button.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/checkbox.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/checkbox.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/form.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/form.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/hiddenfield.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/hiddenfield.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/radio.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/radio.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/select.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/select.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/textarea.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/textarea.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/textfield.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/forms/dialogs/textfield.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/iframe/dialogs/iframe.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/iframe/dialogs/iframe.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/image/dialogs/image.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/image/dialogs/image.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/image/images/noimage.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/image/images/noimage.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/dialogs/anchor.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/dialogs/anchor.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/dialogs/link.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/dialogs/link.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/images/anchor.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/images/anchor.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/images/hidpi/anchor.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/link/images/hidpi/anchor.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/liststyle/dialogs/liststyle.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/liststyle/dialogs/liststyle.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastefromgdocs/filter/default.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastefromgdocs/filter/default.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastefromlibreoffice/filter/default.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastefromlibreoffice/filter/default.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastefromword/filter/default.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastefromword/filter/default.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastetools/filter/common.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastetools/filter/common.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastetools/filter/image.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/pastetools/filter/image.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/LICENSE.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/LICENSE.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/README.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/dialogs/options.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/dialogs/options.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/dialogs/toolbar.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/scayt/dialogs/toolbar.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/dialogs/smiley.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/dialogs/smiley.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angel_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angel_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angel_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angel_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angry_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angry_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angry_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/angry_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/broken_heart.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/broken_heart.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/broken_heart.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/broken_heart.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/confused_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/confused_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/confused_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/confused_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/cry_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/cry_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/cry_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/cry_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/devil_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/devil_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/devil_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/devil_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/embaressed_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/embaressed_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/embarrassed_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/embarrassed_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/embarrassed_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/embarrassed_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/envelope.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/envelope.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/heart.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/heart.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/heart.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/heart.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/kiss.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/kiss.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/kiss.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/kiss.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/lightbulb.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/lightbulb.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/lightbulb.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/lightbulb.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/omg_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/omg_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/omg_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/omg_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/regular_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/regular_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/regular_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/regular_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/sad_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/sad_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/sad_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/sad_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/shades_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/shades_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/shades_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/shades_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/teeth_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/teeth_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/teeth_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/teeth_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_down.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_down.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_down.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_down.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_up.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_up.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_up.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/thumbs_up.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/tongue_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/tongue_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/tongue_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/tongue_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/tounge_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/tounge_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/whatchutalkingabout_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/whatchutalkingabout_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/whatchutalkingabout_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/whatchutalkingabout_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/wink_smile.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/wink_smile.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/wink_smile.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/smiley/images/wink_smile.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/specialchar.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/specialchar.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/_translationstatus.txt` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/_translationstatus.txt`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/af.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/af.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ar.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/az.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/az.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/bg.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ca.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/cs.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/cy.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/da.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/da.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/de-ch.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/de.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/de.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/el.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/el.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en-au.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en-ca.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en-ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en-gb.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/en.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/eo.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/eo.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/es-mx.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/es-mx.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/es.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/es.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/et.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/et.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/eu.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/eu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fa.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fi.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fr-ca.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fr.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/gl.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/he.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/he.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/hr.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/hu.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/id.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/id.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/it.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/it.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ja.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/km.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/km.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ko.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ku.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ku.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/lt.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/lt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/lv.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/lv.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/nb.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/nl.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/no.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/no.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/oc.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/pl.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/pt-br.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/pt.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/pt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ro.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ro.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ru.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/si.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/si.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sk.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sl.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sl.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sq.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sq.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sr-latn.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sr.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sv.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/th.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/th.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/tr.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/tt.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/tt.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ug.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/ug.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/uk.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/vi.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/zh-cn.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/zh.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/specialchar/dialogs/lang/zh.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/table/dialogs/table.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/table/dialogs/table.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/tableselection/styles/tableselection.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/tableselection/styles/tableselection.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/tabletools/dialogs/tableCell.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/tabletools/dialogs/tableCell.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/dialogs/templates.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/dialogs/templates.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/dialogs/templates.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/dialogs/templates.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/default.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/default.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/images/template1.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/images/template1.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/images/template3.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/templates/templates/images/template3.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/LICENSE.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/LICENSE.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/README.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/ciframe.html` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/ciframe.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/tmpFrameset.html` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/tmpFrameset.html`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/wsc.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/wsc.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/wsc.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/wsc.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/wsc_ie.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/dialogs/wsc_ie.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/skins/moono-lisa/wsc.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/plugins/wsc/skins/moono-lisa/wsc.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog_ie.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog_ie.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog_ie8.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog_ie8.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog_iequirks.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/dialog_iequirks.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_gecko.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_gecko.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_ie.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_ie.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_ie8.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_ie8.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_iequirks.css` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/editor_iequirks.css`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/icons.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/icons.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/icons_hidpi.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/readme.md` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/readme.md`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/close.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/close.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/refresh.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/refresh.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/spinner.gif` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/close.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/close.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/lock-open.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/lock-open.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/lock.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/lock.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/refresh.png` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text/vendor/ckeditor4/skins/moono-lisa/images/hidpi/refresh.png`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/static/djangocms_text_ckeditor/js/cms.ckeditor.js` & `djangocms_text-0.1.1/djangocms_text/static/djangocms_text_ckeditor/js/cms.ckeditor.js`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text/templatetags/djangocms_text_tags.py` & `djangocms_text-0.1.1/djangocms_text/templatetags/djangocms_text_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/djangocms_text_ckeditor/fields.py` & `djangocms_text-0.1.1/djangocms_text_ckeditor/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/.gitignore` & `djangocms_text-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/LICENSE` & `djangocms_text-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_text-0.1.0/README.rst` & `djangocms_text-0.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 - **djangocms-text-ckeditor Compatibility**: Initial version includes a port of the
   CKEditor 4 interface and child plugin functionality. This editor is compatible with
   the ``djangocms-text-ckeditor`` plugin, and can be used as a drop-in replacement.
 
 Installation
 ------------
 
-Install ``djangocms-text`` using pip:
+Install ``djangocms-text`` using pip: ``pip install djangocms-text``.
+
+Build latest development branch using git:
 
 .. code-block:: bash
 
     git clone git@github.com:fsbraun/djangocms-text.git
     cd djangocms-text
     nvm use
     npm install
```

### Comparing `djangocms_text-0.1.0/pyproject.toml` & `djangocms_text-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -56,7 +56,11 @@
 path = "djangocms_text/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/djangocms_text",
     "/djangocms_text_ckeditor"
 ]
+artifacts = [
+    "djangocms_text/static/**",
+    "djangocms_text/contrib/**/static/**",
+]
```

### Comparing `djangocms_text-0.1.0/PKG-INFO` & `djangocms_text-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: djangocms-text
-Version: 0.1.0
+Version: 0.1.1
 Summary: Rich Text Plugin for django CMS
 Project-URL: Homepage, https://github.com/django-cms/djangocms-text
 Author-email: Django CMS Association and contributors <info@django-cms.org>
 Maintainer-email: Django CMS Association and contributors <info@django-cms.org>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,15 +58,17 @@
 - **djangocms-text-ckeditor Compatibility**: Initial version includes a port of the
   CKEditor 4 interface and child plugin functionality. This editor is compatible with
   the ``djangocms-text-ckeditor`` plugin, and can be used as a drop-in replacement.
 
 Installation
 ------------
 
-Install ``djangocms-text`` using pip:
+Install ``djangocms-text`` using pip: ``pip install djangocms-text``.
+
+Build latest development branch using git:
 
 .. code-block:: bash
 
     git clone git@github.com:fsbraun/djangocms-text.git
     cd djangocms-text
     nvm use
     npm install
```

